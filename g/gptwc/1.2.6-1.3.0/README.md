# Comparing `tmp/gptwc-1.2.6.tar.gz` & `tmp/gptwc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptwc-1.2.6.tar", last modified: Fri Mar  1 23:26:23 2024, max compression
+gzip compressed data, was "gptwc-1.3.0.tar", last modified: Sun May 19 18:25:01 2024, max compression
```

## Comparing `gptwc-1.2.6.tar` & `gptwc-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 nealla    (1000) nealla    (1000)        0 2024-03-01 23:26:23.912399 gptwc-1.2.6/
--rw-rw-r--   0 nealla    (1000) nealla    (1000)     1059 2023-03-17 01:42:38.000000 gptwc-1.2.6/LICENSE
--rw-rw-r--   0 nealla    (1000) nealla    (1000)     3234 2024-03-01 23:26:23.912399 gptwc-1.2.6/PKG-INFO
--rw-rw-r--   0 nealla    (1000) nealla    (1000)     2883 2023-03-17 02:20:42.000000 gptwc-1.2.6/README.md
-drwxrwxr-x   0 nealla    (1000) nealla    (1000)        0 2024-03-01 23:26:23.912399 gptwc-1.2.6/gptwc/
--rw-rw-r--   0 nealla    (1000) nealla    (1000)       31 2023-03-17 06:38:04.000000 gptwc-1.2.6/gptwc/__init__.py
--rw-rw-r--   0 nealla    (1000) nealla    (1000)     2284 2024-03-01 23:26:02.000000 gptwc-1.2.6/gptwc/gptwc.py
-drwxrwxr-x   0 nealla    (1000) nealla    (1000)        0 2024-03-01 23:26:23.912399 gptwc-1.2.6/gptwc.egg-info/
--rw-rw-r--   0 nealla    (1000) nealla    (1000)     3234 2024-03-01 23:26:23.000000 gptwc-1.2.6/gptwc.egg-info/PKG-INFO
--rw-rw-r--   0 nealla    (1000) nealla    (1000)      235 2024-03-01 23:26:23.000000 gptwc-1.2.6/gptwc.egg-info/SOURCES.txt
--rw-rw-r--   0 nealla    (1000) nealla    (1000)        1 2024-03-01 23:26:23.000000 gptwc-1.2.6/gptwc.egg-info/dependency_links.txt
--rw-rw-r--   0 nealla    (1000) nealla    (1000)       44 2024-03-01 23:26:23.000000 gptwc-1.2.6/gptwc.egg-info/entry_points.txt
--rw-rw-r--   0 nealla    (1000) nealla    (1000)       19 2024-03-01 23:26:23.000000 gptwc-1.2.6/gptwc.egg-info/requires.txt
--rw-rw-r--   0 nealla    (1000) nealla    (1000)        6 2024-03-01 23:26:23.000000 gptwc-1.2.6/gptwc.egg-info/top_level.txt
--rw-rw-r--   0 nealla    (1000) nealla    (1000)       38 2024-03-01 23:26:23.912399 gptwc-1.2.6/setup.cfg
--rw-rw-r--   0 nealla    (1000) nealla    (1000)      705 2024-03-01 23:26:08.000000 gptwc-1.2.6/setup.py
+drwxrwxr-x   0 nealla    (1000) nealla    (1000)        0 2024-05-19 18:25:01.884884 gptwc-1.3.0/
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)     1059 2023-03-17 01:42:38.000000 gptwc-1.3.0/LICENSE
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)     3247 2024-05-19 18:25:01.884884 gptwc-1.3.0/PKG-INFO
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)     2896 2024-05-19 18:16:13.000000 gptwc-1.3.0/README.md
+drwxrwxr-x   0 nealla    (1000) nealla    (1000)        0 2024-05-19 18:25:01.884884 gptwc-1.3.0/gptwc/
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)       31 2023-03-17 06:38:04.000000 gptwc-1.3.0/gptwc/__init__.py
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)     2301 2024-05-19 18:15:59.000000 gptwc-1.3.0/gptwc/gptwc.py
+drwxrwxr-x   0 nealla    (1000) nealla    (1000)        0 2024-05-19 18:25:01.884884 gptwc-1.3.0/gptwc.egg-info/
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)     3247 2024-05-19 18:25:01.000000 gptwc-1.3.0/gptwc.egg-info/PKG-INFO
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)      235 2024-05-19 18:25:01.000000 gptwc-1.3.0/gptwc.egg-info/SOURCES.txt
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)        1 2024-05-19 18:25:01.000000 gptwc-1.3.0/gptwc.egg-info/dependency_links.txt
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)       44 2024-05-19 18:25:01.000000 gptwc-1.3.0/gptwc.egg-info/entry_points.txt
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)       26 2024-05-19 18:25:01.000000 gptwc-1.3.0/gptwc.egg-info/requires.txt
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)        6 2024-05-19 18:25:01.000000 gptwc-1.3.0/gptwc.egg-info/top_level.txt
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)       38 2024-05-19 18:25:01.884884 gptwc-1.3.0/setup.cfg
+-rw-rw-r--   0 nealla    (1000) nealla    (1000)      712 2024-05-19 18:14:04.000000 gptwc-1.3.0/setup.py
```

### Comparing `gptwc-1.2.6/LICENSE` & `gptwc-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gptwc-1.2.6/PKG-INFO` & `gptwc-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptwc
-Version: 1.2.6
+Version: 1.3.0
 Summary: A package to count tokens in input text using OpenAI's tiktoken library.
 Home-page: https://github.com/lwneal/gptwc
 Author: Lawrence Neal
 Author-email: nealla@lwneal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -65,24 +65,25 @@
 
 positional arguments:
   FILE             Text files to count tokens in
 
 options:
   -h, --help       show this help message and exit
   --files0-from F  Read input from the files specified by NUL-terminated names in file F
-  --model MODEL    Model name to use for tokenization (default: text-davinci-003)
+  --model MODEL    Model name to use for tokenization (default: gpt-4)
   -c, --clipboard  Read input from the system clipboard
   --version        show program's version number and exit
 ```
 
 ## Which Tokenizer Does Each Model Use?
 
 From [tiktoken/model.py](https://github.com/openai/tiktoken/blob/main/tiktoken/model.py)
 
 ```
+"gpt-4o": "o200k_base",
 "gpt-4": "cl100k_base",
 "gpt-3.5-turbo": "cl100k_base",
 "text-embedding-ada-002": "cl100k_base",
 
 "text-davinci-003": "p50k_base",
 "text-davinci-002": "p50k_base",
 "code-davinci-002": "p50k_base",
```

### Comparing `gptwc-1.2.6/README.md` & `gptwc-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,24 +52,25 @@
 
 positional arguments:
   FILE             Text files to count tokens in
 
 options:
   -h, --help       show this help message and exit
   --files0-from F  Read input from the files specified by NUL-terminated names in file F
-  --model MODEL    Model name to use for tokenization (default: text-davinci-003)
+  --model MODEL    Model name to use for tokenization (default: gpt-4)
   -c, --clipboard  Read input from the system clipboard
   --version        show program's version number and exit
 ```
 
 ## Which Tokenizer Does Each Model Use?
 
 From [tiktoken/model.py](https://github.com/openai/tiktoken/blob/main/tiktoken/model.py)
 
 ```
+"gpt-4o": "o200k_base",
 "gpt-4": "cl100k_base",
 "gpt-3.5-turbo": "cl100k_base",
 "text-embedding-ada-002": "cl100k_base",
 
 "text-davinci-003": "p50k_base",
 "text-davinci-002": "p50k_base",
 "code-davinci-002": "p50k_base",
```

### Comparing `gptwc-1.2.6/gptwc/gptwc.py` & `gptwc-1.3.0/gptwc/gptwc.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     return len(encoding.encode(text))
 
 
 def main():
     parser = argparse.ArgumentParser(description="Count tokens in text files using OpenAI's tiktoken library.")
     parser.add_argument("files", metavar="FILE", nargs="*", type=Path, help="Text files to count tokens in")
     parser.add_argument("--files0-from", metavar="F", type=Path, help="Read input from the files specified by NUL-terminated names in file F")
-    parser.add_argument("--model", default="cl100k_base", metavar="MODEL", help="Encoding or model to use for tokenization (default: cl100k_base, which is used by GPT-3.5 and GPT-4)")
+    parser.add_argument("--model", default="o200k_base", metavar="MODEL", help="Encoding or model to use for tokenization (default: o200k_base, used by GPT-4o. Use cl100k_base for GPT-3.5 and GPT-4)")
     parser.add_argument("-c", "--clipboard", action="store_true", help="Read input from the system clipboard")
     parser.add_argument("--version", action="version", version="%(prog)s 1.2.6")
     args = parser.parse_args()
 
     if args.files0_from:
         with args.files0_from.open("r", encoding="utf-8") as file_list:
             args.files.extend(Path(line.strip()) for line in file_list)
```

### Comparing `gptwc-1.2.6/gptwc.egg-info/PKG-INFO` & `gptwc-1.3.0/gptwc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptwc
-Version: 1.2.6
+Version: 1.3.0
 Summary: A package to count tokens in input text using OpenAI's tiktoken library.
 Home-page: https://github.com/lwneal/gptwc
 Author: Lawrence Neal
 Author-email: nealla@lwneal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -65,24 +65,25 @@
 
 positional arguments:
   FILE             Text files to count tokens in
 
 options:
   -h, --help       show this help message and exit
   --files0-from F  Read input from the files specified by NUL-terminated names in file F
-  --model MODEL    Model name to use for tokenization (default: text-davinci-003)
+  --model MODEL    Model name to use for tokenization (default: gpt-4)
   -c, --clipboard  Read input from the system clipboard
   --version        show program's version number and exit
 ```
 
 ## Which Tokenizer Does Each Model Use?
 
 From [tiktoken/model.py](https://github.com/openai/tiktoken/blob/main/tiktoken/model.py)
 
 ```
+"gpt-4o": "o200k_base",
 "gpt-4": "cl100k_base",
 "gpt-3.5-turbo": "cl100k_base",
 "text-embedding-ada-002": "cl100k_base",
 
 "text-davinci-003": "p50k_base",
 "text-davinci-002": "p50k_base",
 "code-davinci-002": "p50k_base",
```

### Comparing `gptwc-1.2.6/setup.py` & `gptwc-1.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gptwc",
-    version="1.2.6",
+    version="1.3.0",
     author="Lawrence Neal",
     author_email="nealla@lwneal.com",
     description="A package to count tokens in input text using OpenAI's tiktoken library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lwneal/gptwc",
     packages=find_packages(),
     install_requires=[
-        "tiktoken",
+        "tiktoken>=0.7.0",
         "pyperclip",
     ],
     python_requires=">=3.6",
     entry_points={
         "console_scripts": [
             "gptwc=gptwc.gptwc:main",
         ],
```

