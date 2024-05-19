# Comparing `tmp/fleepit-4.tar.gz` & `tmp/fleepit-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleepit-4.tar", last modified: Thu May  9 00:21:34 2024, max compression
+gzip compressed data, was "fleepit-5.tar", last modified: Sun May 19 19:10:55 2024, max compression
```

## Comparing `fleepit-4.tar` & `fleepit-5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-09 00:21:34.115545 fleepit-4/
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)    11358 2024-05-08 23:36:33.000000 fleepit-4/LICENSE
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      106 2024-05-08 23:46:21.000000 fleepit-4/NOTICE
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      833 2024-05-09 00:21:34.115545 fleepit-4/PKG-INFO
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      456 2024-05-08 23:59:32.000000 fleepit-4/README.md
-drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-09 00:21:34.114545 fleepit-4/fleepit.egg-info/
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      833 2024-05-09 00:21:34.000000 fleepit-4/fleepit.egg-info/PKG-INFO
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      202 2024-05-09 00:21:34.000000 fleepit-4/fleepit.egg-info/SOURCES.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)        1 2024-05-09 00:21:34.000000 fleepit-4/fleepit.egg-info/dependency_links.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)       41 2024-05-09 00:21:34.000000 fleepit-4/fleepit.egg-info/entry_points.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)        8 2024-05-09 00:21:34.000000 fleepit-4/fleepit.egg-info/top_level.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)     2925 2024-05-09 00:20:47.000000 fleepit-4/fleepit.py
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)       38 2024-05-09 00:21:34.115545 fleepit-4/setup.cfg
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      849 2024-05-09 00:20:24.000000 fleepit-4/setup.py
+drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-19 19:10:55.831530 fleepit-5/
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)    11358 2024-05-08 23:36:33.000000 fleepit-5/LICENSE
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      106 2024-05-08 23:46:21.000000 fleepit-5/NOTICE
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)     1185 2024-05-19 19:10:55.831530 fleepit-5/PKG-INFO
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      808 2024-05-19 19:02:22.000000 fleepit-5/README.md
+drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-19 19:10:55.830531 fleepit-5/fleepit.egg-info/
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)     1185 2024-05-19 19:10:55.000000 fleepit-5/fleepit.egg-info/PKG-INFO
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      202 2024-05-19 19:10:55.000000 fleepit-5/fleepit.egg-info/SOURCES.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)        1 2024-05-19 19:10:55.000000 fleepit-5/fleepit.egg-info/dependency_links.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)       41 2024-05-19 19:10:55.000000 fleepit-5/fleepit.egg-info/entry_points.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)        8 2024-05-19 19:10:55.000000 fleepit-5/fleepit.egg-info/top_level.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)     3747 2024-05-19 19:06:15.000000 fleepit-5/fleepit.py
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)       38 2024-05-19 19:10:55.831530 fleepit-5/setup.cfg
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      849 2024-05-19 18:31:21.000000 fleepit-5/setup.py
```

### Comparing `fleepit-4/LICENSE` & `fleepit-5/LICENSE`

 * *Files identical despite different names*

### Comparing `fleepit-4/fleepit.py` & `fleepit-5/fleepit.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,28 +13,38 @@
 # limitations under the License.
 
 # Requirements: xclip, xdotool
 
 import subprocess
 import argparse
 import typing
+import json
 
 
+# Built-in langsets
 LANGSETS = {
     'qwerty-en-ru': (
-        r"""`1234567890-=qwertyuiop[]\asdfghjkl;'zxcvbnm,.~!@#$%^&*()_+QWERTYUIOP{}|ASDFGHJKL:"ZXCVBNM<>""",
-        r"""ё1234567890-=йцукенгшщзхъ\фывапролджэячсмитьбюЁ!"№;%:?*()_+ЙЦУКЕНГШЩЗХЪ/ФЫВАПРОЛДЖЭЯЧСМИТЬБЮ""",
+        r"""`1234567890-=qwertyuiop[]\asdfghjkl;'zxcvbnm,.~!#%&*()_+QWERTYUIOP{}|ASDFGHJKL:"ZXCVBNM<>""",
+        r"""ё1234567890-=йцукенгшщзхъ\фывапролджэячсмитьбюЁ!№%?*()_+ЙЦУКЕНГШЩЗХЪ/ФЫВАПРОЛДЖЭЯЧСМИТЬБЮ""",
     ),
 }
 
 
-def make_langset_dict(langset: str) -> typing.Dict[str, str]:
-    ls = LANGSETS[langset]
+def make_langset_dict(langset: typing.Tuple[str, str]) -> typing.Dict[str, str]:
     flipper = {}
-    for (a, b) in zip(*ls):
+
+    if len(langset) != 2 or len(langset[0]) != len(langset[1]):
+        raise ValueError("langset alternatives not matching")
+
+    for (a, b) in zip(*langset):
+        if a in flipper:
+            raise ValueError(f'alternative for "{ a }" already exists')
+        if b in flipper:
+            raise ValueError(f'alternative for "{ b }" already exists')
+
         flipper[a] = b
         flipper[b] = a
     return flipper
 
 
 def flip_langset(clip: str, conv: typing.Dict[str, str]) -> str:
     return ''.join([conv[c] if c in conv else c for c in clip])
@@ -54,15 +64,19 @@
         print(f'clipboard: "{ clip }"')
 
     # Clear selection
     result = subprocess.run([ 'xclip', '-i', '-selection', 'primary' ], text=True, input='')
     result.check_returncode()
 
     # Do convert
-    conv = make_langset_dict(args.langset)
+    if args.langset:
+        conv = make_langset_dict(LANGSETS[args.langset])
+    else:
+        with open(args.langset_file, 'r') as f:
+            conv = make_langset_dict(json.load(f)['langset'])
     converted = flip_langset(clip, conv)
 
     if args.verbose:
         print(f'converted: "{ converted }"')
 
     # Write selection
     result = subprocess.run([ 'xclip', '-i', '-selection', 'clipboard' ], text=True, input=converted)
@@ -78,25 +92,33 @@
     parser.add_argument(
         '-m', '--mode',
         type=str,
         choices=[
             'x11',
             'wayland',
         ],
+        help='compositor compatibility mode',
         required=True,
     )
     parser.add_argument(
         '-v', '--verbose',
+        help='verbose logging ',
         action='store_true',
     )
-    parser.add_argument(
+    langset_group = parser.add_mutually_exclusive_group(required=True)
+    langset_group.add_argument(
         '-l', '--langset',
+        help='use one of embedded langsets',
         type=str,
         choices=list(LANGSETS.keys()),
-        required=True,
+    )
+    langset_group.add_argument(
+        '-f', '--langset-file',
+        help='use langset from json file containing',
+        type=str,
     )
     args = parser.parse_args()
 
     if args.mode == 'x11':
         do_x11(args)
     else:
         raise NotImplementedError()
```

### Comparing `fleepit-4/setup.py` & `fleepit-5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description_content_type = 'text/markdown'
 except:
     long_description = None
     long_description_content_type = None
 
 setup(
     name='fleepit',
-    version='4',
+    version='5',
     py_modules=['fleepit'],
     description='Text seleciton keyboard layout switcher based on xclip / etc for X11 & wayland',
     url='https://git.pegasko.art/bitrate16/fleepit',
     author_email='pegasko@pegasko.art',
     license='Apache 2.0',
     keywords='keyboard layout shortcut layout-switcher',
     entry_points='''
```

