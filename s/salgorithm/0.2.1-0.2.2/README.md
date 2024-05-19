# Comparing `tmp/salgorithm-0.2.1.tar.gz` & `tmp/salgorithm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salgorithm-0.2.1.tar", last modified: Sun May 19 01:00:02 2024, max compression
+gzip compressed data, was "salgorithm-0.2.2.tar", last modified: Sun May 19 01:10:33 2024, max compression
```

## Comparing `salgorithm-0.2.1.tar` & `salgorithm-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:00:02.840861 salgorithm-0.2.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-19 00:38:30.000000 salgorithm-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 01:00:02.839861 salgorithm-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7614 2024-05-19 00:38:30.000000 salgorithm-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:00:02.825860 salgorithm-0.2.1/salgorithm/
--rw-r--r--   0 root         (0) root         (0)      686 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/BFS.py
--rw-r--r--   0 root         (0) root         (0)      338 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/BinarySearch.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Bubble.py
--rw-r--r--   0 root         (0) root         (0)      764 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Bucket.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/CaesarCipher.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Cocktail.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/DFS.py
--rw-r--r--   0 root         (0) root         (0)      761 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Greedy.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Heap.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Insertion.py
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Interpolation.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Jump.py
--rw-r--r--   0 root         (0) root         (0)      182 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Linear.py
--rw-r--r--   0 root         (0) root         (0)      559 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Merge.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Quick.py
--rw-r--r--   0 root         (0) root         (0)     1380 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/RSA.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Radix.py
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Selection.py
--rw-r--r--   0 root         (0) root         (0)      400 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Shell.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Tabu.py
--rw-r--r--   0 root         (0) root         (0)      533 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/TransposeCipher.py
--rw-r--r--   0 root         (0) root         (0)      566 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/VigenereCipher.py
--rw-r--r--   0 root         (0) root         (0)      796 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-19 00:59:41.000000 salgorithm-0.2.1/salgorithm/time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:00:02.837860 salgorithm-0.2.1/salgorithm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 01:00:02.000000 salgorithm-0.2.1/salgorithm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-19 01:00:02.000000 salgorithm-0.2.1/salgorithm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 01:00:02.000000 salgorithm-0.2.1/salgorithm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-19 01:00:02.000000 salgorithm-0.2.1/salgorithm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 01:00:02.841861 salgorithm-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1072 2024-05-19 00:59:58.000000 salgorithm-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:10:33.585652 salgorithm-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-19 00:38:30.000000 salgorithm-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 01:10:33.584652 salgorithm-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7614 2024-05-19 00:38:30.000000 salgorithm-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:10:33.542650 salgorithm-0.2.2/salgorithm/
+-rw-r--r--   0 root         (0) root         (0)      685 2024-05-19 01:06:53.000000 salgorithm-0.2.2/salgorithm/BFS.py
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-19 01:06:55.000000 salgorithm-0.2.2/salgorithm/BinarySearch.py
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-19 01:06:58.000000 salgorithm-0.2.2/salgorithm/Bubble.py
+-rw-r--r--   0 root         (0) root         (0)      734 2024-05-19 01:07:00.000000 salgorithm-0.2.2/salgorithm/Bucket.py
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-19 01:07:03.000000 salgorithm-0.2.2/salgorithm/CaesarCipher.py
+-rw-r--r--   0 root         (0) root         (0)      716 2024-05-19 01:07:08.000000 salgorithm-0.2.2/salgorithm/Cocktail.py
+-rw-r--r--   0 root         (0) root         (0)      293 2024-05-19 01:07:11.000000 salgorithm-0.2.2/salgorithm/DFS.py
+-rw-r--r--   0 root         (0) root         (0)      760 2024-05-19 01:07:14.000000 salgorithm-0.2.2/salgorithm/Greedy.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-19 01:07:17.000000 salgorithm-0.2.2/salgorithm/Heap.py
+-rw-r--r--   0 root         (0) root         (0)      284 2024-05-19 01:07:19.000000 salgorithm-0.2.2/salgorithm/Insertion.py
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-19 01:07:21.000000 salgorithm-0.2.2/salgorithm/Interpolation.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-19 01:07:24.000000 salgorithm-0.2.2/salgorithm/Jump.py
+-rw-r--r--   0 root         (0) root         (0)      173 2024-05-19 01:07:29.000000 salgorithm-0.2.2/salgorithm/Linear.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-19 01:07:32.000000 salgorithm-0.2.2/salgorithm/Merge.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-19 01:07:39.000000 salgorithm-0.2.2/salgorithm/Quick.py
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-05-19 01:07:37.000000 salgorithm-0.2.2/salgorithm/RSA.py
+-rw-r--r--   0 root         (0) root         (0)      861 2024-05-19 01:07:49.000000 salgorithm-0.2.2/salgorithm/Radix.py
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-19 01:07:51.000000 salgorithm-0.2.2/salgorithm/Selection.py
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-19 01:08:19.000000 salgorithm-0.2.2/salgorithm/Shell.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-19 01:08:27.000000 salgorithm-0.2.2/salgorithm/Tabu.py
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-19 01:08:22.000000 salgorithm-0.2.2/salgorithm/TransposeCipher.py
+-rw-r--r--   0 root         (0) root         (0)      565 2024-05-19 01:08:34.000000 salgorithm-0.2.2/salgorithm/VigenereCipher.py
+-rw-r--r--   0 root         (0) root         (0)      796 2024-05-19 00:38:30.000000 salgorithm-0.2.2/salgorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-19 00:59:41.000000 salgorithm-0.2.2/salgorithm/time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:10:33.583652 salgorithm-0.2.2/salgorithm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 01:10:33.000000 salgorithm-0.2.2/salgorithm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-19 01:10:33.000000 salgorithm-0.2.2/salgorithm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 01:10:33.000000 salgorithm-0.2.2/salgorithm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-19 01:10:33.000000 salgorithm-0.2.2/salgorithm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 01:10:33.586652 salgorithm-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-05-19 01:10:28.000000 salgorithm-0.2.2/setup.py
```

### Comparing `salgorithm-0.2.1/LICENSE` & `salgorithm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.1/PKG-INFO` & `salgorithm-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salgorithm
-Version: 0.2.1
+Version: 0.2.2
 Summary: 让算法变得简单一点
 Home-page: https://github.com/SoulCodingYanhun/salgorithm
 Author: SoulCodingYanhun
 Author-email: souls2906@gmail.com
 Maintainer: SoulCodingYanhun
 Maintainer-email: souls2906@gmail.com
 License: Apache License
```

### Comparing `salgorithm-0.2.1/README.md` & `salgorithm-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.1/salgorithm/BFS.py` & `salgorithm-0.2.2/salgorithm/BFS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import deque
-from .time import TimedFunction
+from time import TimedFunction
 
 @TimedFunction
 def bfs(graph, start):
     visited = set()  # 用于记录已访问的节点
     queue = deque([start])  # 使用队列来进行广度优先搜索
     visited.add(start)  # 将起始节点标记为已访问
```

### Comparing `salgorithm-0.2.1/salgorithm/Cocktail.py` & `salgorithm-0.2.2/salgorithm/Cocktail.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from .time import TimedFunction
-
-@TimedFunction
-def cocktail_sort(arr):
-    n = len(arr)
-    start = 0
-    end = n - 1
-    swapped = True
-
-    while swapped:
-        swapped = False
-
-        # 从左到右进行冒泡排序
-        for i in range(start, end):
-            if arr[i] > arr[i + 1]:
-                arr[i], arr[i + 1] = arr[i + 1], arr[i]
-                swapped = True
-
-        if not swapped:
-            break
-
-        swapped = False
-
-        # 从右到左进行冒泡排序
-        end -= 1
-        for i in range(end - 1, start - 1, -1):
-            if arr[i] > arr[i + 1]:
-                arr[i], arr[i + 1] = arr[i + 1], arr[i]
-                swapped = True
-
-        start += 1
-
-    return arr
+from time import TimedFunction
+
+@TimedFunction
+def cocktail_sort(arr):
+    n = len(arr)
+    start = 0
+    end = n - 1
+    swapped = True
+
+    while swapped:
+        swapped = False
+
+        # 从左到右进行冒泡排序
+        for i in range(start, end):
+            if arr[i] > arr[i + 1]:
+                arr[i], arr[i + 1] = arr[i + 1], arr[i]
+                swapped = True
+
+        if not swapped:
+            break
+
+        swapped = False
+
+        # 从右到左进行冒泡排序
+        end -= 1
+        for i in range(end - 1, start - 1, -1):
+            if arr[i] > arr[i + 1]:
+                arr[i], arr[i + 1] = arr[i + 1], arr[i]
+                swapped = True
+
+        start += 1
+
+    return arr
```

### Comparing `salgorithm-0.2.1/salgorithm/Greedy.py` & `salgorithm-0.2.2/salgorithm/Greedy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .time import TimedFunction
+from time import TimedFunction
 
 @TimedFunction
 def greedy_set_cover(universe, subsets):
     selected_subsets = []  # 存储被选择的子集
 
     while universe:  # 当宇宙集合非空时
         best_subset = None  # 当前最优子集
```

### Comparing `salgorithm-0.2.1/salgorithm/Heap.py` & `salgorithm-0.2.2/salgorithm/Heap.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .time import TimedFunction
+from time import TimedFunction
 
 @TimedFunction
 def heap_sort(arr):
     n = len(arr)
     for i in range(n // 2 - 1, -1, -1):
         heapify(arr, n, i)
     for i in range(n - 1, 0, -1):
```

### Comparing `salgorithm-0.2.1/salgorithm/Merge.py` & `salgorithm-0.2.2/salgorithm/Merge.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .time import TimedFunction
+from time import TimedFunction
 
 @TimedFunction
 def merge_sort(arr):
     if len(arr) <= 1:
         return arr
     mid = len(arr) // 2
     left = merge_sort(arr[:mid])
```

### Comparing `salgorithm-0.2.1/salgorithm/RSA.py` & `salgorithm-0.2.2/salgorithm/RSA.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import random
-import .time from TimedFunction
+import time from TimedFunction
 
 def is_prime(n):
     if n <= 1:
         return False
     for i in range(2, int(n**0.5) + 1):
         if n % i == 0:
             return False
```

### Comparing `salgorithm-0.2.1/salgorithm/Radix.py` & `salgorithm-0.2.2/salgorithm/Radix.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import .time from TimedFunction
-
-@TimedFunction
-def counting_sort(arr, exp):
-    n = len(arr)
-    output = [0] * n
-    count = [0] * 10
-
-    # 统计每个数字出现的次数
-    for i in range(n):
-        index = arr[i] // exp
-        count[index % 10] += 1
-
-    # 计算累计次数
-    for i in range(1, 10):
-        count[i] += count[i - 1]
-
-    # 根据次数将元素放入正确的位置
-    i = n - 1
-    while i >= 0:
-        index = arr[i] // exp
-        output[count[index % 10] - 1] = arr[i]
-        count[index % 10] -= 1
-        i -= 1
-
-    # 将排序后的结果复制回原数组
-    for i in range(n):
-        arr[i] = output[i]
-
-def radix_sort(arr):
-    # 找到数组中的最大值，确定迭代次数
-    max_value = max(arr)
-    exp = 1
-
-    while max_value // exp > 0:
-        counting_sort(arr, exp)
-        exp *= 10
-
-    return arr
+import time from TimedFunction
+
+@TimedFunction
+def counting_sort(arr, exp):
+    n = len(arr)
+    output = [0] * n
+    count = [0] * 10
+
+    # 统计每个数字出现的次数
+    for i in range(n):
+        index = arr[i] // exp
+        count[index % 10] += 1
+
+    # 计算累计次数
+    for i in range(1, 10):
+        count[i] += count[i - 1]
+
+    # 根据次数将元素放入正确的位置
+    i = n - 1
+    while i >= 0:
+        index = arr[i] // exp
+        output[count[index % 10] - 1] = arr[i]
+        count[index % 10] -= 1
+        i -= 1
+
+    # 将排序后的结果复制回原数组
+    for i in range(n):
+        arr[i] = output[i]
+
+def radix_sort(arr):
+    # 找到数组中的最大值，确定迭代次数
+    max_value = max(arr)
+    exp = 1
+
+    while max_value // exp > 0:
+        counting_sort(arr, exp)
+        exp *= 10
+
+    return arr
```

### Comparing `salgorithm-0.2.1/salgorithm/TransposeCipher.py` & `salgorithm-0.2.2/salgorithm/TransposeCipher.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import .time from TimedFunction
+import time from TimedFunction
 
 @TimedFunction
 def transpose_cipher(text, key):
     num_columns = len(key)
     num_rows = (len(text) + num_columns - 1) // num_columns
     num_padding = num_rows * num_columns - len(text)
     text += " " * num_padding
```

### Comparing `salgorithm-0.2.1/salgorithm/VigenereCipher.py` & `salgorithm-0.2.2/salgorithm/VigenereCipher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import .time from TimedFunction
+import time from TimedFunction
 
 @TimedFunction
 def vigenere_cipher(text, key):
     result = ""
     key_index = 0
     for char in text:
         if char.isalpha():
```

### Comparing `salgorithm-0.2.1/salgorithm/__init__.py` & `salgorithm-0.2.2/salgorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.1/salgorithm.egg-info/PKG-INFO` & `salgorithm-0.2.2/salgorithm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salgorithm
-Version: 0.2.1
+Version: 0.2.2
 Summary: 让算法变得简单一点
 Home-page: https://github.com/SoulCodingYanhun/salgorithm
 Author: SoulCodingYanhun
 Author-email: souls2906@gmail.com
 Maintainer: SoulCodingYanhun
 Maintainer-email: souls2906@gmail.com
 License: Apache License
```

### Comparing `salgorithm-0.2.1/salgorithm.egg-info/SOURCES.txt` & `salgorithm-0.2.2/salgorithm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.1/setup.py` & `salgorithm-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Load the README.md file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='salgorithm',
-    version='0.2.1',
+    version='0.2.2',
     description="让算法变得简单一点",
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type as Markdown
     include_package_data=True,
     author='SoulCodingYanhun',
     author_email='souls2906@gmail.com',
     maintainer='SoulCodingYanhun',
```

