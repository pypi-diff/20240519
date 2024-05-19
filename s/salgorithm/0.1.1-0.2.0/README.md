# Comparing `tmp/salgorithm-0.1.1.tar.gz` & `tmp/salgorithm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salgorithm-0.1.1.tar", last modified: Mon Mar  4 14:22:02 2024, max compression
+gzip compressed data, was "salgorithm-0.2.0.tar", last modified: Sun May 19 00:40:03 2024, max compression
```

## Comparing `salgorithm-0.1.1.tar` & `salgorithm-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-04 14:22:02.462774 salgorithm-0.1.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-03-03 14:16:26.000000 salgorithm-0.1.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     8255 2024-03-04 14:22:02.462774 salgorithm-0.1.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7614 2024-03-04 14:21:46.000000 salgorithm-0.1.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-04 14:22:02.458774 salgorithm-0.1.1/salgorithm/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      639 2024-03-04 14:05:05.000000 salgorithm-0.1.1/salgorithm/BFS.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      289 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/BinarySearch.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      208 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Bubble.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      713 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Bucket.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      337 2024-03-03 14:20:48.000000 salgorithm-0.1.1/salgorithm/CaesarCipher.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      699 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Cocktail.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      246 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/DFS.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      712 2024-03-04 14:10:35.000000 salgorithm-0.1.1/salgorithm/Greedy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      551 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Heap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      237 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Insertion.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      413 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Interpolation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      431 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Jump.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      131 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Linear.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      511 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Merge.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      277 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Quick.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1317 2024-03-03 14:26:52.000000 salgorithm-0.1.1/salgorithm/RSA.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      848 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Radix.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      252 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Selection.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      349 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Shell.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1044 2024-03-03 14:16:26.000000 salgorithm-0.1.1/salgorithm/Tabu.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      485 2024-03-03 14:24:33.000000 salgorithm-0.1.1/salgorithm/TransposeCipher.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      518 2024-03-03 14:23:02.000000 salgorithm-0.1.1/salgorithm/VigenereCipher.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      796 2024-03-04 14:21:12.000000 salgorithm-0.1.1/salgorithm/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-04 14:22:02.458774 salgorithm-0.1.1/salgorithm.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     8255 2024-03-04 14:22:02.000000 salgorithm-0.1.1/salgorithm.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      672 2024-03-04 14:22:02.000000 salgorithm-0.1.1/salgorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-03-04 14:22:02.000000 salgorithm-0.1.1/salgorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2024-03-04 14:22:02.000000 salgorithm-0.1.1/salgorithm.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-03-04 14:22:02.462774 salgorithm-0.1.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1072 2024-03-04 14:21:53.000000 salgorithm-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 00:40:03.784008 salgorithm-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-19 00:38:30.000000 salgorithm-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 00:40:03.783008 salgorithm-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7614 2024-05-19 00:38:30.000000 salgorithm-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 00:40:03.765006 salgorithm-0.2.0/salgorithm/
+-rw-r--r--   0 root         (0) root         (0)      686 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/BFS.py
+-rw-r--r--   0 root         (0) root         (0)      338 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/BinarySearch.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Bubble.py
+-rw-r--r--   0 root         (0) root         (0)      764 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Bucket.py
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/CaesarCipher.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Cocktail.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/DFS.py
+-rw-r--r--   0 root         (0) root         (0)      761 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Greedy.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Heap.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Insertion.py
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Interpolation.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Jump.py
+-rw-r--r--   0 root         (0) root         (0)      182 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Linear.py
+-rw-r--r--   0 root         (0) root         (0)      559 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Merge.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Quick.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/RSA.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Radix.py
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Selection.py
+-rw-r--r--   0 root         (0) root         (0)      400 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Shell.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Tabu.py
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/TransposeCipher.py
+-rw-r--r--   0 root         (0) root         (0)      566 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/VigenereCipher.py
+-rw-r--r--   0 root         (0) root         (0)      796 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 00:40:03.780007 salgorithm-0.2.0/salgorithm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 00:40:03.000000 salgorithm-0.2.0/salgorithm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-19 00:40:03.000000 salgorithm-0.2.0/salgorithm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 00:40:03.000000 salgorithm-0.2.0/salgorithm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-19 00:40:03.000000 salgorithm-0.2.0/salgorithm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 00:40:03.784008 salgorithm-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-05-19 00:38:30.000000 salgorithm-0.2.0/setup.py
```

### Comparing `salgorithm-0.1.1/LICENSE` & `salgorithm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salgorithm-0.1.1/PKG-INFO` & `salgorithm-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salgorithm
-Version: 0.1.1
+Version: 0.2.0
 Summary: 让算法变得简单一点
 Home-page: https://github.com/SoulCodingYanhun/salgorithm
 Author: SoulCodingYanhun
 Author-email: souls2906@gmail.com
 Maintainer: SoulCodingYanhun
 Maintainer-email: souls2906@gmail.com
 License: Apache License
```

### Comparing `salgorithm-0.1.1/README.md` & `salgorithm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `salgorithm-0.1.1/salgorithm/Bucket.py` & `salgorithm-0.2.0/salgorithm/Bucket.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from .time import TimedFunction
+
+@TimedFunction
 def bucket_sort(arr):
     # 确定桶的数量，这里假设为10
     num_buckets = 10
 
     # 创建一个空的桶列表
     buckets = [[] for _ in range(num_buckets)]
```

### Comparing `salgorithm-0.1.1/salgorithm/Heap.py` & `salgorithm-0.2.0/salgorithm/Heap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from .time import TimedFunction
+
+@TimedFunction
 def heap_sort(arr):
     n = len(arr)
     for i in range(n // 2 - 1, -1, -1):
         heapify(arr, n, i)
     for i in range(n - 1, 0, -1):
         arr[i], arr[0] = arr[0], arr[i]
         heapify(arr, i, 0)
```

### Comparing `salgorithm-0.1.1/salgorithm/RSA.py` & `salgorithm-0.2.0/salgorithm/RSA.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+
 import random
+import .time from TimedFunction
 
 def is_prime(n):
     if n <= 1:
         return False
     for i in range(2, int(n**0.5) + 1):
         if n % i == 0:
             return False
@@ -40,17 +42,19 @@
         e = random.randrange(1, phi)
         g = gcd(e, phi)
 
     d = multiplicative_inverse(e, phi)
 
     return ((e, n), (d, n))
 
+@TimedFunction
 def encrypt(message, public_key):
     e, n = public_key
     encrypted_message = [pow(ord(char), e, n) for char in message]
     return encrypted_message
 
+@TimedFunction
 def decrypt(encrypted_message, private_key):
     d, n = private_key
     decrypted_message = [chr(pow(char, d, n)) for char in encrypted_message]
     return "".join(decrypted_message)
```

### Comparing `salgorithm-0.1.1/salgorithm/Radix.py` & `salgorithm-0.2.0/salgorithm/Radix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import .time from TimedFunction
+
+@TimedFunction
 def counting_sort(arr, exp):
     n = len(arr)
     output = [0] * n
     count = [0] * 10
 
     # 统计每个数字出现的次数
     for i in range(n):
@@ -29,8 +32,8 @@
     max_value = max(arr)
     exp = 1
 
     while max_value // exp > 0:
         counting_sort(arr, exp)
         exp *= 10
 
-    return arr
+    return arr
```

### Comparing `salgorithm-0.1.1/salgorithm/Tabu.py` & `salgorithm-0.2.0/salgorithm/Tabu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import .time from TimedFunction
+
+@TimedFunction
 def tabu_search(initial_solution, neighborhood_func, objective_func, tabu_list_size, max_iterations):
     current_solution = initial_solution
     best_solution = current_solution
     tabu_list = []
 
     for _ in range(max_iterations):
         neighborhood = neighborhood_func(current_solution)
```

### Comparing `salgorithm-0.1.1/salgorithm/__init__.py` & `salgorithm-0.2.0/salgorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.1.1/salgorithm.egg-info/PKG-INFO` & `salgorithm-0.2.0/salgorithm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salgorithm
-Version: 0.1.1
+Version: 0.2.0
 Summary: 让算法变得简单一点
 Home-page: https://github.com/SoulCodingYanhun/salgorithm
 Author: SoulCodingYanhun
 Author-email: souls2906@gmail.com
 Maintainer: SoulCodingYanhun
 Maintainer-email: souls2906@gmail.com
 License: Apache License
```

### Comparing `salgorithm-0.1.1/salgorithm.egg-info/SOURCES.txt` & `salgorithm-0.2.0/salgorithm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 salgorithm/Radix.py
 salgorithm/Selection.py
 salgorithm/Shell.py
 salgorithm/Tabu.py
 salgorithm/TransposeCipher.py
 salgorithm/VigenereCipher.py
 salgorithm/__init__.py
+salgorithm/time.py
 salgorithm.egg-info/PKG-INFO
 salgorithm.egg-info/SOURCES.txt
 salgorithm.egg-info/dependency_links.txt
 salgorithm.egg-info/top_level.txt
```

### Comparing `salgorithm-0.1.1/setup.py` & `salgorithm-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Load the README.md file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='salgorithm',
-    version='0.1.1',
+    version='0.2.0',
     description="让算法变得简单一点",
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type as Markdown
     include_package_data=True,
     author='SoulCodingYanhun',
     author_email='souls2906@gmail.com',
     maintainer='SoulCodingYanhun',
```

