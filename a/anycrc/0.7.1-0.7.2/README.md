# Comparing `tmp/anycrc-0.7.1.tar.gz` & `tmp/anycrc-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.7.1.tar", last modified: Sat May 18 14:26:30 2024, max compression
+gzip compressed data, was "anycrc-0.7.2.tar", last modified: Sun May 19 13:47:01 2024, max compression
```

## Comparing `anycrc-0.7.1.tar` & `anycrc-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.886639 anycrc-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-18 14:26:26.000000 anycrc-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-18 14:26:30.886639 anycrc-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-18 14:26:26.000000 anycrc-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.882639 anycrc-0.7.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.882639 anycrc-0.7.1/lib/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-18 14:26:26.000000 anycrc-0.7.1/lib/crcany/crc.c
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-18 14:26:26.000000 anycrc-0.7.1/lib/crcany/crcdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-05-18 14:26:26.000000 anycrc-0.7.1/lib/crcany/model.c
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-18 14:26:26.000000 anycrc-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:26:30.886639 anycrc-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-18 14:26:26.000000 anycrc-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.882639 anycrc-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.886639 anycrc-0.7.1/src/anycrc/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 14:26:26.000000 anycrc-0.7.1/src/anycrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-18 14:26:26.000000 anycrc-0.7.1/src/anycrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-18 14:26:26.000000 anycrc-0.7.1/src/anycrc/anycrc.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-18 14:26:26.000000 anycrc-0.7.1/src/anycrc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.886639 anycrc-0.7.1/src/anycrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-18 14:26:30.000000 anycrc-0.7.1/src/anycrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-18 14:26:30.000000 anycrc-0.7.1/src/anycrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:26:30.000000 anycrc-0.7.1/src/anycrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 14:26:30.000000 anycrc-0.7.1/src/anycrc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:47:01.475484 anycrc-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-19 13:46:56.000000 anycrc-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-19 13:47:01.475484 anycrc-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-19 13:46:56.000000 anycrc-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:47:01.471484 anycrc-0.7.2/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:47:01.471484 anycrc-0.7.2/lib/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-19 13:46:56.000000 anycrc-0.7.2/lib/crcany/crc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-19 13:46:56.000000 anycrc-0.7.2/lib/crcany/crcdbl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18969 2024-05-19 13:46:56.000000 anycrc-0.7.2/lib/crcany/model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-19 13:46:56.000000 anycrc-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:47:01.475484 anycrc-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-19 13:46:56.000000 anycrc-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:47:01.471484 anycrc-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:47:01.475484 anycrc-0.7.2/src/anycrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 13:46:56.000000 anycrc-0.7.2/src/anycrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-19 13:46:56.000000 anycrc-0.7.2/src/anycrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-19 13:46:56.000000 anycrc-0.7.2/src/anycrc/anycrc.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-19 13:46:56.000000 anycrc-0.7.2/src/anycrc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:47:01.475484 anycrc-0.7.2/src/anycrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-19 13:47:01.000000 anycrc-0.7.2/src/anycrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-19 13:47:01.000000 anycrc-0.7.2/src/anycrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:47:01.000000 anycrc-0.7.2/src/anycrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 13:47:01.000000 anycrc-0.7.2/src/anycrc.egg-info/top_level.txt
```

### Comparing `anycrc-0.7.1/LICENSE` & `anycrc-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.1/PKG-INFO` & `anycrc-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
```

### Comparing `anycrc-0.7.1/README.md` & `anycrc-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.1/lib/crcany/crc.c` & `anycrc-0.7.2/lib/crcany/crc.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.1/lib/crcany/crcdbl.c` & `anycrc-0.7.2/lib/crcany/crcdbl.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.1/lib/crcany/model.c` & `anycrc-0.7.2/lib/crcany/model.c`

 * *Files 1% similar despite different names*

```diff
@@ -521,14 +521,15 @@
     model->table_byte = NULL;
     model->table_word = NULL;
     model->table_slice16 = NULL;
 }
 
 // See model.h.
 void free_model(model_t *model) {
+    free(model->name);
     free(model->table_comb);
     free(model->table_byte);
     free(model->table_word);
     free(model->table_slice16);
 }
 
 // Like POSIX getline().
```

### Comparing `anycrc-0.7.1/setup.py` & `anycrc-0.7.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         
 else:
     compile_args = ['-fopenmp', '-O2']
     link_args = ['-fopenmp', '-O2']
     
 setup(
     name = 'anycrc',
-    version = '0.7.1',
+    version = '0.7.2',
     package_dir = {"": "src"},
     cmdclass={"build_ext": Build},
     ext_modules = [
         Extension(
             name='anycrc.anycrc',
             extra_compile_args=compile_args,
             extra_link_args=link_args,
```

### Comparing `anycrc-0.7.1/src/anycrc/anycrc.pyx` & `anycrc-0.7.2/src/anycrc/anycrc.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 cdef bint parallel = True
 word_bits = WORDBITS
 
 cdef class CRC:
     cdef model_t model
     cdef word_t reg, reg_hi
     
-    def __init__(self, width, poly, init, ref_in, ref_out, xor_out, check=0, residue=0):
+    def __cinit__(self, width, poly, init, ref_in, ref_out, xor_out, check=0, residue=0):
         cdef unsigned endian = 1 if sys.byteorder == 'little' else 0
         refin = 'true' if ref_in else 'false'
         refout = 'true' if ref_out else 'false'
         
         if width > WORDBITS * 2:
             raise ValueError('CRC width is larger than what is allowed')
             
@@ -94,15 +94,15 @@
             
             if error_code == 1:
                 raise MemoryError('Out of memory error')
                 
             self.reg = self.model.init
             self.reg_hi = self.model.init_hi
             
-    def __del__(self):
+    def __dealloc__(self):
         free_model(&self.model);
         
     def get(self):
         if self.model.width <= WORDBITS:
             return self.reg
             
         else:
```

### Comparing `anycrc-0.7.1/src/anycrc/models.py` & `anycrc-0.7.2/src/anycrc/models.py`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.1/src/anycrc.egg-info/PKG-INFO` & `anycrc-0.7.2/src/anycrc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
```

