# Comparing `tmp/webflask-0.5.6.tar.gz` & `tmp/webflask-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webflask-0.5.6.tar", last modified: Mon May 13 01:35:26 2024, max compression
+gzip compressed data, was "webflask-0.6.tar", last modified: Sun May 19 16:18:19 2024, max compression
```

## Comparing `webflask-0.5.6.tar` & `webflask-0.6.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 01:35:26.492260 webflask-0.5.6/
--rw-rw-rw-   0        0        0       55 2024-05-13 01:35:26.490261 webflask-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.5.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 01:35:26.492260 webflask-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      413 2024-05-13 01:34:33.000000 webflask-0.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:35:26.464972 webflask-0.5.6/webflask/
--rw-rw-rw-   0        0        0        0 2024-05-12 15:16:13.000000 webflask-0.5.6/webflask/__init__.py
--rw-rw-rw-   0        0        0     3966 2024-05-06 15:34:58.000000 webflask-0.5.6/webflask/ajax.zip
--rw-rw-rw-   0        0        0  7982659 2024-05-12 16:34:09.000000 webflask-0.5.6/webflask/authorization.zip
--rw-rw-rw-   0        0        0     1282 2024-05-06 16:27:21.000000 webflask-0.5.6/webflask/cal.zip
--rw-rw-rw-   0        0        0      758 2024-05-12 15:45:15.000000 webflask-0.5.6/webflask/cssnbox.zip
--rw-rw-rw-   0        0        0      834 2024-05-12 15:16:24.000000 webflask-0.5.6/webflask/functions.py
--rw-rw-rw-   0        0        0     4236 2024-05-12 15:27:40.000000 webflask-0.5.6/webflask/one.html
--rw-rw-rw-   0        0        0      606 2024-05-13 01:35:20.000000 webflask-0.5.6/webflask/resume.txt
--rw-rw-rw-   0        0        0     1657 2024-05-12 15:27:51.000000 webflask-0.5.6/webflask/three.rb
--rw-rw-rw-   0        0        0      531 2024-05-13 01:35:10.000000 webflask-0.5.6/webflask/todo.txt
--rw-rw-rw-   0        0        0     2567 2024-05-13 00:46:42.000000 webflask-0.5.6/webflask/two.html
--rw-rw-rw-   0        0        0     1070 2024-05-13 00:35:12.000000 webflask-0.5.6/webflask/uploads.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 01:35:26.487982 webflask-0.5.6/webflask.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-13 01:35:26.000000 webflask-0.5.6/webflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-05-13 01:35:26.000000 webflask-0.5.6/webflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 01:35:26.000000 webflask-0.5.6/webflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 01:35:26.000000 webflask-0.5.6/webflask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 16:18:19.230009 webflask-0.6/
+-rw-rw-rw-   0        0        0       53 2024-05-19 16:18:19.229002 webflask-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 16:18:19.231064 webflask-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-05-19 16:17:50.000000 webflask-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:18:19.201486 webflask-0.6/webflask/
+-rw-rw-rw-   0        0        0        0 2024-05-12 15:16:13.000000 webflask-0.6/webflask/__init__.py
+-rw-rw-rw-   0        0        0     3966 2024-05-06 15:34:58.000000 webflask-0.6/webflask/ajax.zip
+-rw-rw-rw-   0        0        0  7982659 2024-05-12 16:34:09.000000 webflask-0.6/webflask/authorization.zip
+-rw-rw-rw-   0        0        0     5239 2024-05-19 14:39:53.000000 webflask-0.6/webflask/bulb.html
+-rw-rw-rw-   0        0        0     1282 2024-05-06 16:27:21.000000 webflask-0.6/webflask/cal.zip
+-rw-rw-rw-   0        0        0      758 2024-05-12 15:45:15.000000 webflask-0.6/webflask/cssnbox.zip
+-rw-rw-rw-   0        0        0      834 2024-05-12 15:16:24.000000 webflask-0.6/webflask/functions.py
+-rw-rw-rw-   0        0        0     4236 2024-05-12 15:27:40.000000 webflask-0.6/webflask/one.html
+-rw-rw-rw-   0        0        0      606 2024-05-13 01:35:20.000000 webflask-0.6/webflask/resume.txt
+-rw-rw-rw-   0        0        0     1865 2024-05-19 15:40:27.000000 webflask-0.6/webflask/telephone.zip
+-rw-rw-rw-   0        0        0     1654 2024-05-13 16:28:12.000000 webflask-0.6/webflask/three.rb
+-rw-rw-rw-   0        0        0      531 2024-05-13 01:35:10.000000 webflask-0.6/webflask/todo.txt
+-rw-rw-rw-   0        0        0     2567 2024-05-13 00:46:42.000000 webflask-0.6/webflask/two.html
+-rw-rw-rw-   0        0        0     1070 2024-05-13 00:35:12.000000 webflask-0.6/webflask/uploads.txt
+-rw-rw-rw-   0        0        0     2719 2024-05-19 15:35:11.000000 webflask-0.6/webflask/userjson.zip
+-rw-rw-rw-   0        0        0     1517 2024-05-19 14:22:06.000000 webflask-0.6/webflask/usn.zip
+drwxrwxrwx   0        0        0        0 2024-05-19 16:18:19.227923 webflask-0.6/webflask.egg-info/
+-rw-rw-rw-   0        0        0       53 2024-05-19 16:18:18.000000 webflask-0.6/webflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-05-19 16:18:18.000000 webflask-0.6/webflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 16:18:18.000000 webflask-0.6/webflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 16:18:18.000000 webflask-0.6/webflask.egg-info/top_level.txt
```

### Comparing `webflask-0.5.6/webflask/ajax.zip` & `webflask-0.6/webflask/ajax.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.5.6/webflask/authorization.zip` & `webflask-0.6/webflask/authorization.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.5.6/webflask/cal.zip` & `webflask-0.6/webflask/cal.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.5.6/webflask/cssnbox.zip` & `webflask-0.6/webflask/cssnbox.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.5.6/webflask/functions.py` & `webflask-0.6/webflask/functions.py`

 * *Files identical despite different names*

### Comparing `webflask-0.5.6/webflask/one.html` & `webflask-0.6/webflask/one.html`

 * *Files identical despite different names*

### Comparing `webflask-0.5.6/webflask/resume.txt` & `webflask-0.6/webflask/resume.txt`

 * *Files identical despite different names*

### Comparing `webflask-0.5.6/webflask/three.rb` & `webflask-0.6/webflask/three.rb`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   puts get_file_extension("example.txt")  # Output: .txt
   puts "\n"
   
   puts "3. Print the user's first and last name in reverse order"
   puts reverse_name("John", "Doe")  # Output: Doe John
   puts "\n"
   
-  puts "4. Retrieve the total marks from a hash containing subject names and marks"
+  puts "Retrieve the total marks from a hash containing subject names and marks"
   student_marks = { "Maths" => 90, "Science" => 85, "English" => 88 }
   puts total_marks(student_marks)  # Output: 263
   puts "\n"
   
   puts "5. Check if two temperatures are out of bounds"
   puts out_of_bounds?(10, 105)  # Output: true
   puts out_of_bounds?(-5, 90)   # Output: false
```

### Comparing `webflask-0.5.6/webflask/todo.txt` & `webflask-0.6/webflask/todo.txt`

 * *Files identical despite different names*

### Comparing `webflask-0.5.6/webflask/two.html` & `webflask-0.6/webflask/two.html`

 * *Files identical despite different names*

### Comparing `webflask-0.5.6/webflask/uploads.txt` & `webflask-0.6/webflask/uploads.txt`

 * *Files identical despite different names*

