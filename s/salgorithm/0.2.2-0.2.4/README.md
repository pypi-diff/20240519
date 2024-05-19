# Comparing `tmp/salgorithm-0.2.2.tar.gz` & `tmp/salgorithm-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salgorithm-0.2.2.tar", last modified: Sun May 19 01:10:33 2024, max compression
+gzip compressed data, was "salgorithm-0.2.4.tar", last modified: Sun May 19 04:11:39 2024, max compression
```

## Comparing `salgorithm-0.2.2.tar` & `salgorithm-0.2.4.tar`

### file list

```diff
@@ -1,36 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:10:33.585652 salgorithm-0.2.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-19 00:38:30.000000 salgorithm-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 01:10:33.584652 salgorithm-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7614 2024-05-19 00:38:30.000000 salgorithm-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:10:33.542650 salgorithm-0.2.2/salgorithm/
--rw-r--r--   0 root         (0) root         (0)      685 2024-05-19 01:06:53.000000 salgorithm-0.2.2/salgorithm/BFS.py
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-19 01:06:55.000000 salgorithm-0.2.2/salgorithm/BinarySearch.py
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-19 01:06:58.000000 salgorithm-0.2.2/salgorithm/Bubble.py
--rw-r--r--   0 root         (0) root         (0)      734 2024-05-19 01:07:00.000000 salgorithm-0.2.2/salgorithm/Bucket.py
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-19 01:07:03.000000 salgorithm-0.2.2/salgorithm/CaesarCipher.py
--rw-r--r--   0 root         (0) root         (0)      716 2024-05-19 01:07:08.000000 salgorithm-0.2.2/salgorithm/Cocktail.py
--rw-r--r--   0 root         (0) root         (0)      293 2024-05-19 01:07:11.000000 salgorithm-0.2.2/salgorithm/DFS.py
--rw-r--r--   0 root         (0) root         (0)      760 2024-05-19 01:07:14.000000 salgorithm-0.2.2/salgorithm/Greedy.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-05-19 01:07:17.000000 salgorithm-0.2.2/salgorithm/Heap.py
--rw-r--r--   0 root         (0) root         (0)      284 2024-05-19 01:07:19.000000 salgorithm-0.2.2/salgorithm/Insertion.py
--rw-r--r--   0 root         (0) root         (0)      444 2024-05-19 01:07:21.000000 salgorithm-0.2.2/salgorithm/Interpolation.py
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-19 01:07:24.000000 salgorithm-0.2.2/salgorithm/Jump.py
--rw-r--r--   0 root         (0) root         (0)      173 2024-05-19 01:07:29.000000 salgorithm-0.2.2/salgorithm/Linear.py
--rw-r--r--   0 root         (0) root         (0)      558 2024-05-19 01:07:32.000000 salgorithm-0.2.2/salgorithm/Merge.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-05-19 01:07:39.000000 salgorithm-0.2.2/salgorithm/Quick.py
--rw-r--r--   0 root         (0) root         (0)     1379 2024-05-19 01:07:37.000000 salgorithm-0.2.2/salgorithm/RSA.py
--rw-r--r--   0 root         (0) root         (0)      861 2024-05-19 01:07:49.000000 salgorithm-0.2.2/salgorithm/Radix.py
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-19 01:07:51.000000 salgorithm-0.2.2/salgorithm/Selection.py
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-19 01:08:19.000000 salgorithm-0.2.2/salgorithm/Shell.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-05-19 01:08:27.000000 salgorithm-0.2.2/salgorithm/Tabu.py
--rw-r--r--   0 root         (0) root         (0)      532 2024-05-19 01:08:22.000000 salgorithm-0.2.2/salgorithm/TransposeCipher.py
--rw-r--r--   0 root         (0) root         (0)      565 2024-05-19 01:08:34.000000 salgorithm-0.2.2/salgorithm/VigenereCipher.py
--rw-r--r--   0 root         (0) root         (0)      796 2024-05-19 00:38:30.000000 salgorithm-0.2.2/salgorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-19 00:59:41.000000 salgorithm-0.2.2/salgorithm/time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:10:33.583652 salgorithm-0.2.2/salgorithm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 01:10:33.000000 salgorithm-0.2.2/salgorithm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-19 01:10:33.000000 salgorithm-0.2.2/salgorithm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 01:10:33.000000 salgorithm-0.2.2/salgorithm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-19 01:10:33.000000 salgorithm-0.2.2/salgorithm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 01:10:33.586652 salgorithm-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1072 2024-05-19 01:10:28.000000 salgorithm-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 04:11:39.747372 salgorithm-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-19 00:38:30.000000 salgorithm-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2861 2024-05-19 04:11:39.746372 salgorithm-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-05-19 03:23:41.000000 salgorithm-0.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 04:11:39.701381 salgorithm-0.2.4/salgorithm/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-05-19 03:21:29.000000 salgorithm-0.2.4/salgorithm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 04:11:39.711379 salgorithm-0.2.4/salgorithm/cipher/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-19 03:15:10.000000 salgorithm-0.2.4/salgorithm/cipher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-19 03:13:58.000000 salgorithm-0.2.4/salgorithm/cipher/caesar_cipher.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2024-05-19 03:14:19.000000 salgorithm-0.2.4/salgorithm/cipher/rsa.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-19 03:14:12.000000 salgorithm-0.2.4/salgorithm/cipher/transpose_cipher.py
+-rw-r--r--   0 root         (0) root         (0)      544 2024-05-19 03:14:06.000000 salgorithm-0.2.4/salgorithm/cipher/vigenere_cipher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 04:11:39.715378 salgorithm-0.2.4/salgorithm/graph/
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-19 03:12:55.000000 salgorithm-0.2.4/salgorithm/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-19 03:11:59.000000 salgorithm-0.2.4/salgorithm/graph/bfs.py
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-19 03:12:06.000000 salgorithm-0.2.4/salgorithm/graph/dfs.py
+-rw-r--r--   0 root         (0) root         (0)      542 2024-05-19 03:12:12.000000 salgorithm-0.2.4/salgorithm/graph/greedy_set_cover.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 04:11:39.721377 salgorithm-0.2.4/salgorithm/searching/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-19 02:39:10.000000 salgorithm-0.2.4/salgorithm/searching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-19 02:38:22.000000 salgorithm-0.2.4/salgorithm/searching/binary_search.py
+-rw-r--r--   0 root         (0) root         (0)      733 2024-05-19 02:38:55.000000 salgorithm-0.2.4/salgorithm/searching/interpolation_search.py
+-rw-r--r--   0 root         (0) root         (0)      647 2024-05-19 02:39:02.000000 salgorithm-0.2.4/salgorithm/searching/jump_search.py
+-rw-r--r--   0 root         (0) root         (0)      361 2024-05-19 02:38:45.000000 salgorithm-0.2.4/salgorithm/searching/linear_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 04:11:39.734375 salgorithm-0.2.4/salgorithm/sorting/
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-19 03:20:27.000000 salgorithm-0.2.4/salgorithm/sorting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      276 2024-05-19 03:16:19.000000 salgorithm-0.2.4/salgorithm/sorting/bubble_sort.py
+-rw-r--r--   0 root         (0) root         (0)      773 2024-05-19 03:17:52.000000 salgorithm-0.2.4/salgorithm/sorting/bucket_sort.py
+-rw-r--r--   0 root         (0) root         (0)      648 2024-05-19 03:17:58.000000 salgorithm-0.2.4/salgorithm/sorting/cocktail_sort.py
+-rw-r--r--   0 root         (0) root         (0)      613 2024-05-19 03:16:27.000000 salgorithm-0.2.4/salgorithm/sorting/heap_sort.py
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-19 03:16:35.000000 salgorithm-0.2.4/salgorithm/sorting/insertion_sort.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-19 03:16:41.000000 salgorithm-0.2.4/salgorithm/sorting/merge_sort.py
+-rw-r--r--   0 root         (0) root         (0)      621 2024-05-19 03:19:30.000000 salgorithm-0.2.4/salgorithm/sorting/quick_sort.py
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-19 03:18:05.000000 salgorithm-0.2.4/salgorithm/sorting/radix_sort.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-19 03:17:45.000000 salgorithm-0.2.4/salgorithm/sorting/selection_sort.py
+-rw-r--r--   0 root         (0) root         (0)      392 2024-05-19 03:19:12.000000 salgorithm-0.2.4/salgorithm/sorting/shell_sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 04:11:39.736374 salgorithm-0.2.4/salgorithm/utils/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-19 03:22:13.000000 salgorithm-0.2.4/salgorithm/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      491 2024-05-19 03:09:11.000000 salgorithm-0.2.4/salgorithm/utils/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 04:11:39.744373 salgorithm-0.2.4/salgorithm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2861 2024-05-19 04:11:39.000000 salgorithm-0.2.4/salgorithm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-05-19 04:11:39.000000 salgorithm-0.2.4/salgorithm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 04:11:39.000000 salgorithm-0.2.4/salgorithm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-19 04:11:39.000000 salgorithm-0.2.4/salgorithm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 04:11:39.748372 salgorithm-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-05-19 03:26:47.000000 salgorithm-0.2.4/setup.py
```

### Comparing `salgorithm-0.2.2/LICENSE` & `salgorithm-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.2/salgorithm/Cocktail.py` & `salgorithm-0.2.4/salgorithm/sorting/cocktail_sort.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,24 @@
-from time import TimedFunction
+from algorithms.utils.timer import timer_decorator
 
-@TimedFunction
+@timer_decorator
 def cocktail_sort(arr):
     n = len(arr)
+    swapped = True
     start = 0
     end = n - 1
-    swapped = True
-
     while swapped:
         swapped = False
-
-        # 从左到右进行冒泡排序
         for i in range(start, end):
             if arr[i] > arr[i + 1]:
                 arr[i], arr[i + 1] = arr[i + 1], arr[i]
                 swapped = True
-
         if not swapped:
             break
-
         swapped = False
-
-        # 从右到左进行冒泡排序
         end -= 1
         for i in range(end - 1, start - 1, -1):
             if arr[i] > arr[i + 1]:
                 arr[i], arr[i + 1] = arr[i + 1], arr[i]
                 swapped = True
-
         start += 1
-
-    return arr
+    return arr
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `salgorithm-0.2.2/salgorithm/Heap.py` & `salgorithm-0.2.4/salgorithm/sorting/heap_sort.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from time import TimedFunction
-
-@TimedFunction
-def heap_sort(arr):
-    n = len(arr)
-    for i in range(n // 2 - 1, -1, -1):
-        heapify(arr, n, i)
-    for i in range(n - 1, 0, -1):
-        arr[i], arr[0] = arr[0], arr[i]
-        heapify(arr, i, 0)
-    return arr
+from algorithms.utils.timer import timer_decorator
 
 def heapify(arr, n, i):
     largest = i
     left = 2 * i + 1
     right = 2 * i + 2
-    if left < n and arr[left] > arr[largest]:
+    if left < n and arr[i] < arr[left]:
         largest = left
-    if right < n and arr[right] > arr[largest]:
+    if right < n and arr[largest] < arr[right]:
         largest = right
     if largest != i:
         arr[i], arr[largest] = arr[largest], arr[i]
         heapify(arr, n, largest)
+
+@timer_decorator
+def heap_sort(arr):
+    n = len(arr)
+    for i in range(n // 2 - 1, -1, -1):
+        heapify(arr, n, i)
+    for i in range(n - 1, 0, -1):
+        arr[i], arr[0] = arr[0], arr[i]
+        heapify(arr, i, 0)
+    return arr
```

### Comparing `salgorithm-0.2.2/salgorithm/RSA.py` & `salgorithm-0.2.4/salgorithm/cipher/rsa.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-
+from algorithms.utils.timer import timer_decorator
 import random
-import time from TimedFunction
 
-def is_prime(n):
-    if n <= 1:
+def is_prime(num):
+    if num < 2:
         return False
-    for i in range(2, int(n**0.5) + 1):
-        if n % i == 0:
+    for i in range(2, int(num ** 0.5) + 1):
+        if num % i == 0:
             return False
     return True
 
-def gcd(a, b):
-    while b != 0:
-        a, b = b, a % b
-    return a
-
-def multiplicative_inverse(e, phi):
-    def extended_gcd(a, b):
-        if a == 0:
-            return b, 0, 1
-        else:
-            gcd, x, y = extended_gcd(b % a, a)
-            return gcd, y - (b // a) * x, x
-
-    gcd, x, y = extended_gcd(e, phi)
-    if gcd == 1:
-        return x % phi
-
 def generate_keypair(p, q):
     if not (is_prime(p) and is_prime(q)):
         raise ValueError("Both numbers must be prime.")
-    elif p == q:
-        raise ValueError("p and q cannot be equal.")
-
     n = p * q
     phi = (p - 1) * (q - 1)
-
     e = random.randrange(1, phi)
     g = gcd(e, phi)
     while g != 1:
         e = random.randrange(1, phi)
         g = gcd(e, phi)
-
     d = multiplicative_inverse(e, phi)
-
     return ((e, n), (d, n))
 
-@TimedFunction
-def encrypt(message, public_key):
-    e, n = public_key
-    encrypted_message = [pow(ord(char), e, n) for char in message]
-    return encrypted_message
-
-@TimedFunction
-def decrypt(encrypted_message, private_key):
-    d, n = private_key
-    decrypted_message = [chr(pow(char, d, n)) for char in encrypted_message]
-    return "".join(decrypted_message)
+def gcd(a, b):
+    while b != 0:
+        a, b = b, a % b
+    return a
 
+def multiplicative_inverse(e, phi):
+    d = 0
+    x1 = 0
+    x2 = 1
+    y1 = 1
+    temp_phi = phi
+    while e > 0:
+        temp1 = temp_phi // e
+        temp2 = temp_phi - temp1 * e
+        temp_phi = e
+        e = temp2
+        x = x2 - temp1 * x1
+        y = d - temp1 * y1
+        x2 = x1
+        x1 = x
+        d = y1
+        y1 = y
+    if temp_phi == 1:
+        return d + phi
+
+@timer_decorator
+def encrypt(text, public_key):
+    key, n = public_key
+    cipher = [pow(ord(char), key, n) for char in text]
+    return cipher
+
+@timer_decorator
+def decrypt(cipher, private_key):
+    key, n = private_key
+    text = [chr(pow(char, key, n)) for char in cipher]
+    return "".join(text)
```

### Comparing `salgorithm-0.2.2/setup.py` & `salgorithm-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Load the README.md file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='salgorithm',
-    version='0.2.2',
+    version='0.2.4',
     description="让算法变得简单一点",
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type as Markdown
     include_package_data=True,
     author='SoulCodingYanhun',
     author_email='souls2906@gmail.com',
     maintainer='SoulCodingYanhun',
```

