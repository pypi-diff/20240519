# Comparing `tmp/zbl-0.2.1-cp39-none-win_amd64.whl.zip` & `tmp/zbl-0.4.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 183611 bytes, number of entries: 7
--rw-r--r--  4.6 unx     2979 b- defN 24-Mar-10 21:02 zbl-0.2.1.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 24-Mar-10 21:02 zbl-0.2.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     1087 b- defN 24-Mar-10 21:02 zbl-0.2.1.dist-info/license_files/LICENSE.txt
--rw-r--r--  4.6 unx     2630 b- defN 24-Mar-10 21:02 zbl/__init__.py
--rw-r--r--  4.6 unx      338 b- defN 24-Mar-10 21:02 zbl/__main__.py
--rwxr-xr-x  4.6 unx   412672 b- defN 24-Mar-10 21:02 zbl/zbl.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      524 b- defN 24-Mar-10 21:02 zbl-0.2.1.dist-info/RECORD
-7 files, 420325 bytes uncompressed, 182697 bytes compressed:  56.5%
+Zip file size: 184511 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     2981 b- defN 24-May-18 12:32 zbl-0.4.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-18 12:32 zbl-0.4.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1087 b- defN 24-May-18 12:32 zbl-0.4.0.dist-info/license_files/LICENSE.txt
+-rw-r--r--  4.6 unx     2726 b- defN 24-May-18 12:32 zbl/__init__.py
+-rw-r--r--  4.6 unx      338 b- defN 24-May-18 12:32 zbl/__main__.py
+-rwxr-xr-x  4.6 unx   413696 b- defN 24-May-18 12:32 zbl/zbl.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      524 b- defN 24-May-18 12:32 zbl-0.4.0.dist-info/RECORD
+7 files, 421446 bytes uncompressed, 183597 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: zbl-0.2.1.dist-info/METADATA
+Filename: zbl-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: zbl-0.2.1.dist-info/WHEEL
+Filename: zbl-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: zbl-0.2.1.dist-info/license_files/LICENSE.txt
+Filename: zbl-0.4.0.dist-info/license_files/LICENSE.txt
 Comment: 
 
 Filename: zbl/__init__.py
 Comment: 
 
 Filename: zbl/__main__.py
 Comment: 
 
 Filename: zbl/zbl.cp39-win_amd64.pyd
 Comment: 
 
-Filename: zbl-0.2.1.dist-info/RECORD
+Filename: zbl-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zbl/__init__.py

```diff
@@ -11,32 +11,36 @@
 
 # set proces to be DPI-aware
 _ = C.windll.shcore.SetProcessDpiAwareness(2)
 
 
 def frame_to_numpy_array(frame: Frame) -> numpy.ndarray:
     arr = numpy.ctypeslib.as_array(
-        C.cast(frame.ptr, uint8_ptr), shape=(frame.height, frame.row_pitch))
+        C.cast(frame.ptr, uint8_ptr), shape=(frame.height, frame.row_pitch)
+    )
     if frame.row_pitch == frame.width * 4:
         return arr.reshape(frame.height, frame.width, 4)
     else:
         # TODO copy to avoid slow access?
-        return arr[:, :frame.width * 4].reshape((frame.height, frame.width, 4))
+        return arr[:, : frame.width * 4].reshape((frame.height, frame.width, 4))
 
 
 class Capture:
 
     def __init__(
         self,
         window_name: Optional[str] = None,
         window_handle: Optional[str] = None,
         display_id: Optional[int] = None,
         capture_cursor: bool = False,
+        use_staging_texture: bool = True,
     ):
-        self._inner = _NativeCapture(window_name, window_handle, display_id, capture_cursor)
+        self._inner = _NativeCapture(
+            window_name, window_handle, display_id, capture_cursor, use_staging_texture
+        )
 
     @property
     def handle(self) -> int:
         return self._inner.handle()
 
     def raw_frames(self) -> Iterator[Frame]:
         while True:
@@ -45,48 +49,48 @@
                 break
             yield next_frame
 
     def frames(self) -> Iterator[numpy.ndarray]:
         for frame in self.raw_frames():
             yield frame_to_numpy_array(frame)
 
-    def __enter__(self) -> 'Capture':
+    def __enter__(self) -> "Capture":
         self._inner.start()
         return self
 
     def __exit__(self, *_):
         self._inner.stop()
 
 
 def show(args):
     from time import perf_counter
     import cv2
 
     try:
-        cv2.namedWindow('zbl', cv2.WINDOW_NORMAL | cv2.WINDOW_KEEPRATIO)
+        cv2.namedWindow("zbl", cv2.WINDOW_NORMAL | cv2.WINDOW_KEEPRATIO)
 
         with Capture(
             window_name=args.window_name,
             display_id=args.display_id,
-            capture_cursor=args.capture_cursor
+            capture_cursor=args.capture_cursor,
         ) as cap:
             t = perf_counter()
             last_print = perf_counter()
             t_total = 0
             frames = 0
             for frame in cap.frames():
                 t = perf_counter() - t
                 t_total += t
                 frames += 1
                 if perf_counter() - last_print > 1:
-                    print(f'[zbl] capture fps: {frames / t_total:.3f}')
+                    print(f"[zbl] capture fps: {frames / t_total:.3f}")
                     t_total = 0
                     frames = 0
                     last_print = perf_counter()
-                cv2.imshow('zbl', frame)
+                cv2.imshow("zbl", frame)
                 if cv2.waitKey(8) != -1:
                     break
                 t = perf_counter()
 
         cv2.destroyAllWindows()
     except KeyboardInterrupt:
         pass
```

## zbl/__main__.py

```diff
@@ -1,9 +1,9 @@
 import argparse
 import zbl
 
-parser = argparse.ArgumentParser('zbl')
-parser.add_argument('--window-name', type=str, required=False, default=None)
-parser.add_argument('--display-id', type=int, required=False, default=None)
-parser.add_argument('--capture-cursor', action='store_true', required=False)
+parser = argparse.ArgumentParser("zbl")
+parser.add_argument("--window-name", type=str, required=False, default=None)
+parser.add_argument("--display-id", type=int, required=False, default=None)
+parser.add_argument("--capture-cursor", action="store_true", required=False)
 
 zbl.show(parser.parse_args())
```

## Comparing `zbl-0.2.1.dist-info/METADATA` & `zbl-0.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: zbl
-Version: 0.2.1
+Version: 0.4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy
-Requires-Dist: opencv-python~=4.6.0; extra == 'example'
+Requires-Dist: opencv-python ~=4.6.0 ; extra == 'example'
 Provides-Extra: example
 License-File: LICENSE.txt
 Summary: real-time window capture library based on D3D11 and Windows.Graphics.Capture
 Keywords: windows,d3d11,window-capture,graphics-capture,cv
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Repository, https://github.com/modelflat/zbl
 Project-URL: Homepage, https://github.com/modelflat/zbl
+Project-URL: Repository, https://github.com/modelflat/zbl
 
 # zbl
 
 [![PyPI version](https://badge.fury.io/py/zbl.svg)](https://badge.fury.io/py/zbl)
 
 `zbl` is a Rust and Python library for screen/window capturing. It provides an interface
 to `Windows.Graphics.Capture` API with a focus on simplifying integrating computer vision applications for Windows Desktop apps.
```

## Comparing `zbl-0.2.1.dist-info/license_files/LICENSE.txt` & `zbl-0.4.0.dist-info/license_files/LICENSE.txt`

 * *Files identical despite different names*

