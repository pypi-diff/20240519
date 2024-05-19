# Comparing `tmp/zhlyr-4.8-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/zhlyr-4.9-cp312-cp312-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 348702 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 19:32 zhlyr-4.8.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 19:32 zhlyr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-15 19:32 zhlyr.libs/
--rwxrwxrwx  2.0 unx     4083 b- defN 24-May-15 19:32 zhlyr-4.8.dist-info/METADATA
--rwxrwxrwx  2.0 unx      152 b- defN 24-May-15 19:32 zhlyr-4.8.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        6 b- defN 24-May-15 19:32 zhlyr-4.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      691 b- defN 24-May-15 19:32 zhlyr-4.8.dist-info/RECORD
--rwxrwxrwx  2.0 unx   486116 b- defN 24-May-15 19:32 zhlyr/serialize.c
--rwxrwxrwx  2.0 unx     2179 b- defN 24-May-15 19:32 zhlyr/zhlyr.py
--rwxrwxrwx  2.0 unx     1875 b- defN 24-May-15 19:32 zhlyr/recosnize.py
--rwxrwxrwx  2.0 unx   650528 b- defN 24-May-15 19:32 zhlyr/serialize.cpython-312-x86_64-linux-gnu.so
--rwxrwxrwx  2.0 unx       93 b- defN 24-May-15 19:32 zhlyr/__init__.py
-12 files, 1145723 bytes uncompressed, 347244 bytes compressed:  69.7%
+Zip file size: 692200 bytes, number of entries: 11
+-rwxrwxrwx  2.0 unx   486116 b- defN 24-May-15 19:05 build/lib.linux-x86_64-cpython-312/zhlyr/serialize.c
+-rwxrwxrwx  2.0 unx   650528 b- defN 24-May-15 19:05 build/lib.linux-x86_64-cpython-312/zhlyr/serialize.cpython-312-x86_64-linux-gnu.so
+-rwxrwxrwx  2.0 unx       93 b- defN 24-May-15 19:28 zhlyr/__init__.py
+-rwxrwxrwx  2.0 unx     1480 b- defN 24-May-18 22:35 zhlyr/recosnize.py
+-rwxrwxrwx  2.0 unx   486116 b- defN 24-May-15 19:05 zhlyr/serialize.c
+-rwxrwxrwx  2.0 unx   650528 b- defN 24-May-15 19:05 zhlyr/serialize.cpython-312-x86_64-linux-gnu.so
+-rwxrwxrwx  2.0 unx     2179 b- defN 24-May-10 18:26 zhlyr/zhlyr.py
+-rwxrwxrwx  2.0 unx     3907 b- defN 24-May-19 05:10 zhlyr-4.9.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      102 b- defN 24-May-19 05:10 zhlyr-4.9.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        6 b- defN 24-May-19 05:10 zhlyr-4.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      934 b- defN 24-May-19 05:10 zhlyr-4.9.dist-info/RECORD
+11 files, 2281989 bytes uncompressed, 690624 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,37 +1,34 @@
-Filename: zhlyr-4.8.dist-info/
+Filename: build/lib.linux-x86_64-cpython-312/zhlyr/serialize.c
 Comment: 
 
-Filename: zhlyr/
+Filename: build/lib.linux-x86_64-cpython-312/zhlyr/serialize.cpython-312-x86_64-linux-gnu.so
 Comment: 
 
-Filename: zhlyr.libs/
-Comment: 
-
-Filename: zhlyr-4.8.dist-info/METADATA
+Filename: zhlyr/__init__.py
 Comment: 
 
-Filename: zhlyr-4.8.dist-info/WHEEL
+Filename: zhlyr/recosnize.py
 Comment: 
 
-Filename: zhlyr-4.8.dist-info/top_level.txt
+Filename: zhlyr/serialize.c
 Comment: 
 
-Filename: zhlyr-4.8.dist-info/RECORD
+Filename: zhlyr/serialize.cpython-312-x86_64-linux-gnu.so
 Comment: 
 
-Filename: zhlyr/serialize.c
+Filename: zhlyr/zhlyr.py
 Comment: 
 
-Filename: zhlyr/zhlyr.py
+Filename: zhlyr-4.9.dist-info/METADATA
 Comment: 
 
-Filename: zhlyr/recosnize.py
+Filename: zhlyr-4.9.dist-info/WHEEL
 Comment: 
 
-Filename: zhlyr/serialize.cpython-312-x86_64-linux-gnu.so
+Filename: zhlyr-4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: zhlyr/__init__.py
+Filename: zhlyr-4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## zhlyr/recosnize.py

```diff
@@ -1,12 +1,11 @@
 from typing import Union, Optional
 from shazamio import Shazam as RecoSnizer
 import json , os , asyncio
 from pathlib import Path
-from .serialize import Serializer
 RecoSnizer_ = RecoSnizer()
 class RecoSnize(RecoSnizer):
     '''
     :param `data`: `bytes` | `bytearray` or `str path` | `Path` object 
     to get info from it.
     :param `proxy`: `str` | `None` to set `proxy` for your `request`
     '''
@@ -35,17 +34,8 @@
     async def text(self):
         '''
         Returns a string of the recognizer.
         '''
         return str(await self.recognizer)
 
 
-Serializer({'hello':'hi'})
-# Example to use to RecoSnizer :
 
-# async def main():
-#     data_path = r'C:\Users\Mtsky\Downloads\Telegram Desktop\mzaf_17549133339911745381.plus.aac.ep (2).m4a'
-#     result = await RecoSnize(data_path).json()
-#     print(Serializer(result).track.title)
-
-# loop = asyncio.new_event_loop()
-# loop.run_until_complete(main())
```

## Comparing `zhlyr-4.8.dist-info/METADATA` & `zhlyr-4.9.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhlyr
-Version: 4.8
+Version: 4.9
 Summary: Python library for music handling
 Home-page: https://gaoc3.github.io/zhlyr/
 Author: Mtsky
 Author-email: secon2636@gmail.com
 License: MIT
 Keywords: lyrics,music,shazam,serialize,serializer,recognize
 Classifier: Development Status :: 1 - Planning
@@ -20,124 +20,130 @@
 Requires-Dist: requests
 Requires-Dist: shazamio
 Requires-Dist: shazam
 Requires-Dist: cython
 
 - ## What is zhlyr?
 - **A python library aimed at music enthusiasts, providing tools for managing and discovering music, fetching song lyrics, and utilizing machine learning algorithms to predict the name of a song from a short audio snippet.**
-
 - ## Code Area :
 
+
   <details> 
   <summary>
   <i>⏬Install Zhlyr</i>
   </summary>
-    
+
   ```python3
   💲pip install zhlyr
   ```
-  ------
+
+  ---
+
   </details>
-  
+
   <details>
     <summary>
     <i>🎵 Recognize track</i>
     </summary>
     <br>Recognize a track based on a file</br>
-  
-    ```python3
-    # Get full track json response object info
-  
-    import asynico
-    from zhlyr import Reconize
-    data = '/root/user/dir/simple.mp3'
-    async def get_info():
-      reco = await Reconize(data)
-      print(reco.json())
-    loop = asynico.new_event_loop()
-    loop.run_until_complete(get_info)
-  
-    # You can get respnose info as string response 
-    reco = Reconize(data)
-    print(reco.text)
-    ```
-  ------
-  
+
+  ```python3
+  # Get full track json response object info
+
+  import asynico
+  from zhlyr import Reconize
+  data = '/root/user/dir/simple.mp3'
+  async def get_info():
+    reco = await Reconize(data)
+    print(reco.json())
+  loop = asynico.new_event_loop()
+  loop.run_until_complete(get_info)
+
+  # You can get respnose info as string response 
+  reco = Reconize(data)
+  print(reco.text)
+  ```
+
+  ---
+
   </details>
-  
+
   <details>
     <summary>
     <i>🔍🎼 Get the lyrics of the track </i>
     </summary>
     <br>
-    
-    Get lyrics from title of the track
-    </br>
-    
-    ```python3
-    from zhlyr import ZhLyr
-    lyrics = ZhLyr.GetByTitle(title='save your trears',srt=false)
-    # :GetByTitle: `title`: str : title of the track to get trrack from it.
-    # :GetByTitle: `srt`: bool : if `true` he will return time as `srt` format.
-    # :GetByTitle: return json object
-    
-    for time , lyric in lyrics.items():
-      print(f'time {time} >>> lyric : {lyric}')
-    ```
-    
-    <br>
-    
-    Get lyrics from details of track
-    </br>
-    ```python3
-    lyrics = ZhLyr.GetByDetails(title='save your trears',artist='the weeknd',duration='3:35',srt=false)
-    # :GetByDetails: `title`: str : title of the track to get trrack from it.
-    # :GetByDetails: `artist`: str : artist of the track to get lyrics from it.
-    # :GetByDetails: `duration` : Optional[str]=None : duration of the track to get lyrics from it.
-    # :GetByDetails: `srt`: bool : if `true` he will return time as `srt` format.
-    # :GetByDetails: return json object
-    
-    for time , lyric in lyrics.items():
-      print(f'time {time} >>> lyric : {lyric}')
-    ```
-  ------
+
+  Get lyrics from title of the track
+  `</br>`
+
+  ```python3
+  from zhlyr import ZhLyr
+  lyrics = ZhLyr.GetByTitle(title='save your trears',srt=false)
+  # :GetByTitle: `title`: str : title of the track to get trrack from it.
+  # :GetByTitle: `srt`: bool : if `true` he will return time as `srt` format.
+  # :GetByTitle: return json object
+
+  for time , lyric in lyrics.items():
+    print(f'time {time} >>> lyric : {lyric}')
+  ```
+
+  <br>
+
+  Get lyrics from details of track
+  `</br>`
+
+  ```python3
+  lyrics = ZhLyr.GetByDetails(title='save your trears',artist='the weeknd',duration='3:35',srt=false)
+  # :GetByDetails: `title`: str : title of the track to get trrack from it.
+  # :GetByDetails: `artist`: str : artist of the track to get lyrics from it.
+  # :GetByDetails: `duration` : Optional[str]=None : duration of the track to get lyrics from it.
+  # :GetByDetails: `srt`: bool : if `true` he will return time as `srt` format.
+  # :GetByDetails: return json object
+
+  for time , lyric in lyrics.items():
+    print(f'time {time} >>> lyric : {lyric}')
+  ```
+
+  ---
+
   </details>
-  
+
   <details>
-    
-  
-  
-    <summary>
+
+  <summary>
       <i>ℹ️ How to use data serialization </i>
     </summary>
     <br>
-    
-    Serialized data from response.
-    </br>
-    
-    ```python3
-    from zhlyr import Serializer
-    data = your_json_data
-    serialize = Serializer(data)
-    print(serialize)
-    ```
-    <br>
-    
-    Get vlue from key with serialized data.
-    </br>
-  
-    ```python3
-    data = {'key1':'hello world!'}
-    serialize = Serializer(data)
-    print(serialize.key1)
-    ```
-  ------
-  
-  </details>
 
+  Serialized data from response.
+  `</br>`
+
+  ```python3
+  from zhlyr import Serializer
+  data = your_json_data
+  serialize = Serializer(data)
+  print(serialize)
+  ```
+
+  <br>
+
+  Get vlue from key with serialized data.
+  `</br>`
+
+  ```python3
+  data = {'key1':'hello world!'}
+  serialize = Serializer(data)
+  print(serialize.key1)
+  ```
+
+  ---
+
+  </details>
 
 ## My Accounts
-- [GitHub](https://github.com/Gaoc3/) [<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub" width="20" height="20">](https://github.com/)
-- [Instagram](https://www.instagram.com/mtsky.sensei/) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" width="20" height="20">](https://www.instagram.com/)
-- [Telegram](https://nar4nar.t.me) [<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram" width="20" height="20">](https://web.telegram.org/)
-  
-------
+
+- [GitHub](https://github.com/Gaoc3/)[`<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub" width="20" height="20">`](https://github.com/)
+- [Instagram](https://www.instagram.com/mtsky.sensei/)[`<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" width="20" height="20">`](https://www.instagram.com/)
+- [Telegram](https://nar4nar.t.me)[`<img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram" width="20" height="20">`](https://web.telegram.org/)
+
+---
```

