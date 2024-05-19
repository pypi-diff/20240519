# Comparing `tmp/anycrc-0.7.0.tar.gz` & `tmp/anycrc-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.7.0.tar", last modified: Tue May 14 20:56:05 2024, max compression
+gzip compressed data, was "anycrc-0.7.1.tar", last modified: Sat May 18 14:26:30 2024, max compression
```

## Comparing `anycrc-0.7.0.tar` & `anycrc-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:56:05.554912 anycrc-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-14 20:56:01.000000 anycrc-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 20:56:05.554912 anycrc-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-14 20:56:01.000000 anycrc-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:56:05.550912 anycrc-0.7.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:56:05.550912 anycrc-0.7.0/lib/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-14 20:56:01.000000 anycrc-0.7.0/lib/crcany/crc.c
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-14 20:56:01.000000 anycrc-0.7.0/lib/crcany/crcdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-05-14 20:56:01.000000 anycrc-0.7.0/lib/crcany/model.c
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-14 20:56:01.000000 anycrc-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:56:05.554912 anycrc-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-14 20:56:01.000000 anycrc-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:56:05.550912 anycrc-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:56:05.554912 anycrc-0.7.0/src/anycrc/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 20:56:01.000000 anycrc-0.7.0/src/anycrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-14 20:56:01.000000 anycrc-0.7.0/src/anycrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-14 20:56:01.000000 anycrc-0.7.0/src/anycrc/anycrc.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-14 20:56:01.000000 anycrc-0.7.0/src/anycrc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:56:05.554912 anycrc-0.7.0/src/anycrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 20:56:05.000000 anycrc-0.7.0/src/anycrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 20:56:05.000000 anycrc-0.7.0/src/anycrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:56:05.000000 anycrc-0.7.0/src/anycrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 20:56:05.000000 anycrc-0.7.0/src/anycrc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.886639 anycrc-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-18 14:26:26.000000 anycrc-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-18 14:26:30.886639 anycrc-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-18 14:26:26.000000 anycrc-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.882639 anycrc-0.7.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.882639 anycrc-0.7.1/lib/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-18 14:26:26.000000 anycrc-0.7.1/lib/crcany/crc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-18 14:26:26.000000 anycrc-0.7.1/lib/crcany/crcdbl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-05-18 14:26:26.000000 anycrc-0.7.1/lib/crcany/model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-18 14:26:26.000000 anycrc-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:26:30.886639 anycrc-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-18 14:26:26.000000 anycrc-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.882639 anycrc-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.886639 anycrc-0.7.1/src/anycrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 14:26:26.000000 anycrc-0.7.1/src/anycrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-18 14:26:26.000000 anycrc-0.7.1/src/anycrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-18 14:26:26.000000 anycrc-0.7.1/src/anycrc/anycrc.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-18 14:26:26.000000 anycrc-0.7.1/src/anycrc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:26:30.886639 anycrc-0.7.1/src/anycrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-18 14:26:30.000000 anycrc-0.7.1/src/anycrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-18 14:26:30.000000 anycrc-0.7.1/src/anycrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:26:30.000000 anycrc-0.7.1/src/anycrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 14:26:30.000000 anycrc-0.7.1/src/anycrc.egg-info/top_level.txt
```

### Comparing `anycrc-0.7.0/LICENSE` & `anycrc-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.0/PKG-INFO` & `anycrc-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
@@ -69,22 +69,14 @@
 >>> anycrc.set_parallel(False)
 ```
 
 For a list of pre-built models, check [models.py](https://github.com/marzooqy/anycrc/blob/main/src/anycrc/models.py). To get a list of the models at any time, use the following command:
 
 `python -m anycrc models`
 
-The algorithm used will depend on the length of the input and the CRC's width:
-
-| Data Length | Width ≤ 64 | Width > 64 |
-|:-:|:-:|:-:|
-| Length < 16 | byte-by-byte | byte-by-byte |
-| 16 ≤ Length < 20,000 | slice-by-16 | byte-by-byte |
-| Length ≥ 20,000 | parallel slice-by-16 | byte-by-byte |
-
 The maximum possible CRC width is 128 bits.
 
 ## Benchmarks
 
 Calculating the CRC32 for lorem ipsum 1 million times:
 
 | Module | Time Elapsed (s) | Speed (GiB/s) | Relative |
@@ -104,8 +96,10 @@
 | fastcrc | 0.67 | 0.62 | 39.75 |
 | crcmod-plus | 0.67 | 0.62 | 39.73 |
 
 Tested on a 10th generation Intel i7 processor. Parallel performance will depend on your system.
 
 #### Notes
 
-Parallelism is disabled when the length of the input data is under 20k, as the serial method is faster in that case.
+Parallelism is disabled when the length of the input data is under 200k, as the serial method is faster in that case.
+
+The input needs to be very large in order to notice the speed advantage of the parallel algorithm.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `anycrc-0.7.0/README.md` & `anycrc-0.7.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -60,22 +60,14 @@
 >>> anycrc.set_parallel(False)
 ```
 
 For a list of pre-built models, check [models.py](https://github.com/marzooqy/anycrc/blob/main/src/anycrc/models.py). To get a list of the models at any time, use the following command:
 
 `python -m anycrc models`
 
-The algorithm used will depend on the length of the input and the CRC's width:
-
-| Data Length | Width ≤ 64 | Width > 64 |
-|:-:|:-:|:-:|
-| Length < 16 | byte-by-byte | byte-by-byte |
-| 16 ≤ Length < 20,000 | slice-by-16 | byte-by-byte |
-| Length ≥ 20,000 | parallel slice-by-16 | byte-by-byte |
-
 The maximum possible CRC width is 128 bits.
 
 ## Benchmarks
 
 Calculating the CRC32 for lorem ipsum 1 million times:
 
 | Module | Time Elapsed (s) | Speed (GiB/s) | Relative |
@@ -95,8 +87,10 @@
 | fastcrc | 0.67 | 0.62 | 39.75 |
 | crcmod-plus | 0.67 | 0.62 | 39.73 |
 
 Tested on a 10th generation Intel i7 processor. Parallel performance will depend on your system.
 
 #### Notes
 
-Parallelism is disabled when the length of the input data is under 20k, as the serial method is faster in that case.
+Parallelism is disabled when the length of the input data is under 200k, as the serial method is faster in that case.
+
+The input needs to be very large in order to notice the speed advantage of the parallel algorithm.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `anycrc-0.7.0/lib/crcany/crc.c` & `anycrc-0.7.1/lib/crcany/crc.c`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -415,16 +415,16 @@
     // Process as many 16 byte block as are available.
     if (len >= 16) {
         crc <<= top;
         if (little) {
             if (!model->ref)
                 crc = swap(crc);
             do {
-                uint32_t crc_hi = (crc >> 32) ^ *(uint32_t const *)(buf + 4);
                 uint32_t crc_lo = (crc & 0xffffffff) ^ *(uint32_t const *)buf;
+                uint32_t crc_hi = (crc >> 32) ^ *(uint32_t const *)(buf + 4);
                 uint32_t i3 = *(uint32_t const *)(buf + 8);
                 uint32_t i4 = *(uint32_t const *)(buf + 12);
                 
                 crc = model->table_slice16[15 * 256 + (crc_lo & 0xff)]
                     ^ model->table_slice16[14 * 256 + ((crc_lo >> 8) & 0xff)]
                     ^ model->table_slice16[13 * 256 + ((crc_lo >> 16) & 0xff)]
                     ^ model->table_slice16[12 * 256 + (crc_lo >> 24)]
```

### Comparing `anycrc-0.7.0/lib/crcany/crcdbl.c` & `anycrc-0.7.1/lib/crcany/crcdbl.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.0/lib/crcany/model.c` & `anycrc-0.7.1/lib/crcany/model.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.0/setup.py` & `anycrc-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,25 @@
                      '-lwinpthread',
                      '-Wl,--no-whole-archive',
                      '-fopenmp',
                      '-O2',
                      '-DMS_WIN64']
                      
     else:
-        #github actions and python make it difficult to compile with 32-bit mingw, so just use msvc
+        #github actions and python make it difficult to compile with 32-bit MinGW, so just use MSVC
         compile_args = ['/openmp']
         link_args = []
         
 else:
     compile_args = ['-fopenmp', '-O2']
     link_args = ['-fopenmp', '-O2']
     
 setup(
     name = 'anycrc',
-    version = '0.7.0',
+    version = '0.7.1',
     package_dir = {"": "src"},
     cmdclass={"build_ext": Build},
     ext_modules = [
         Extension(
             name='anycrc.anycrc',
             extra_compile_args=compile_args,
             extra_link_args=link_args,
```

### Comparing `anycrc-0.7.0/src/anycrc/anycrc.pyx` & `anycrc-0.7.1/src/anycrc/anycrc.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from libc.stdint cimport uintmax_t
 from .models import models, aliases
 import sys
 
 ctypedef uintmax_t word_t
 
 cdef extern from '../../lib/crcany/model.h':
-    cdef unsigned short WORDCHARS
-    cdef unsigned short WORDBITS = WORDCHARS << 3
+    cdef const unsigned short WORDCHARS
+    cdef const unsigned short WORDBITS
     
     ctypedef struct model_t:
         unsigned short width
         short cycle
         short back
         char ref
         char rev
@@ -40,15 +40,14 @@
     
     cdef word_t crc_parallel(model_t *model, word_t crc, const void *dat, size_t len, int *error)
     
     cdef int crc_table_combine(model_t *model)
     cdef word_t crc_combine(model_t *model, word_t crc1, word_t crc2, uintmax_t len2);
     
 cdef extern from '../../lib/crcany/crcdbl.h':
-    cdef void crc_bitwise_dbl(model_t *model, word_t *crc_hi, word_t *crc_lo, const unsigned char *buf, size_t len)
     cdef int crc_table_bytewise_dbl(model_t *model)
     cdef void crc_bytewise_dbl(model_t *model, word_t *crc_hi, word_t *crc_lo, const unsigned char *buf, size_t len)
     
 cdef bint parallel = True
 word_bits = WORDBITS
 
 cdef class CRC:
@@ -120,15 +119,15 @@
         self.reg = self.model.init
         self.reg_hi = self.model.init_hi
         
     cdef word_t _calc(self, const unsigned char *data, word_t length):
         cdef word_t crc
         cdef int error = 0
         
-        if parallel and length >= 20000:
+        if parallel and length >= 200000:
             crc = crc_parallel(&self.model, self.reg, data, length, &error)
             
             if error == 1:
                 raise MemoryError('Out of memory error')
                 
             return crc
```

### Comparing `anycrc-0.7.0/src/anycrc/models.py` & `anycrc-0.7.1/src/anycrc/models.py`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.0/src/anycrc.egg-info/PKG-INFO` & `anycrc-0.7.1/src/anycrc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
@@ -69,22 +69,14 @@
 >>> anycrc.set_parallel(False)
 ```
 
 For a list of pre-built models, check [models.py](https://github.com/marzooqy/anycrc/blob/main/src/anycrc/models.py). To get a list of the models at any time, use the following command:
 
 `python -m anycrc models`
 
-The algorithm used will depend on the length of the input and the CRC's width:
-
-| Data Length | Width ≤ 64 | Width > 64 |
-|:-:|:-:|:-:|
-| Length < 16 | byte-by-byte | byte-by-byte |
-| 16 ≤ Length < 20,000 | slice-by-16 | byte-by-byte |
-| Length ≥ 20,000 | parallel slice-by-16 | byte-by-byte |
-
 The maximum possible CRC width is 128 bits.
 
 ## Benchmarks
 
 Calculating the CRC32 for lorem ipsum 1 million times:
 
 | Module | Time Elapsed (s) | Speed (GiB/s) | Relative |
@@ -104,8 +96,10 @@
 | fastcrc | 0.67 | 0.62 | 39.75 |
 | crcmod-plus | 0.67 | 0.62 | 39.73 |
 
 Tested on a 10th generation Intel i7 processor. Parallel performance will depend on your system.
 
 #### Notes
 
-Parallelism is disabled when the length of the input data is under 20k, as the serial method is faster in that case.
+Parallelism is disabled when the length of the input data is under 200k, as the serial method is faster in that case.
+
+The input needs to be very large in order to notice the speed advantage of the parallel algorithm.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

