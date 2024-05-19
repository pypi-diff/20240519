# Comparing `tmp/sabctools-8.2.1.tar.gz` & `tmp/sabctools-8.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabctools-8.2.1.tar", last modified: Sat May 18 18:34:19 2024, max compression
+gzip compressed data, was "sabctools-8.2.2.tar", last modified: Sun May 19 11:09:48 2024, max compression
```

## Comparing `sabctools-8.2.1.tar` & `sabctools-8.2.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-18 18:34:19.732585 sabctools-8.2.1/
--rw-r--r--   0 runner     (501) staff       (20)    17990 2024-05-18 18:31:21.000000 sabctools-8.2.1/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)       24 2024-05-18 18:31:21.000000 sabctools-8.2.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3122 2024-05-18 18:34:19.732427 sabctools-8.2.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2348 2024-05-18 18:31:21.000000 sabctools-8.2.1/README.md
--rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-18 18:31:21.000000 sabctools-8.2.1/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-18 18:34:19.711375 sabctools-8.2.1/sabctools.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3122 2024-05-18 18:34:19.000000 sabctools-8.2.1/sabctools.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3095 2024-05-18 18:34:19.000000 sabctools-8.2.1/sabctools.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-18 18:34:19.000000 sabctools-8.2.1/sabctools.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2024-05-18 18:34:19.000000 sabctools-8.2.1/sabctools.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-18 18:34:19.732623 sabctools-8.2.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)    17185 2024-05-18 18:31:21.000000 sabctools-8.2.1/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-18 18:34:19.713068 sabctools-8.2.1/src/
--rw-r--r--   0 runner     (501) staff       (20)      108 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2284 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crc32.cc
--rw-r--r--   0 runner     (501) staff       (20)     1127 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crc32.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-18 18:34:19.720732 sabctools-8.2.1/src/crcutil-1.0/
--rw-r--r--   0 runner     (501) staff       (20)       54 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/AUTHORS
--rw-r--r--   0 runner     (501) staff       (20)    11358 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/COPYING
--rw-r--r--   0 runner     (501) staff       (20)       58 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/ChangeLog
--rw-r--r--   0 runner     (501) staff       (20)     1700 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/INSTALL
--rw-r--r--   0 runner     (501) staff       (20)    11358 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    50573 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/Makefile
--rw-r--r--   0 runner     (501) staff       (20)     1210 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/Makefile.am
--rw-r--r--   0 runner     (501) staff       (20)    56163 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/Makefile.in
--rw-r--r--   0 runner     (501) staff       (20)     2076 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/Makefile.win
--rw-r--r--   0 runner     (501) staff       (20)       60 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/NEWS
--rw-r--r--   0 runner     (501) staff       (20)     6669 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/README
--rw-r--r--   0 runner     (501) staff       (20)    34611 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/aclocal.m4
--rw-r--r--   0 runner     (501) staff       (20)     2785 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/autogen.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-18 18:34:19.723511 sabctools-8.2.1/src/crcutil-1.0/code/
--rw-r--r--   0 runner     (501) staff       (20)     2368 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/base_types.h
--rw-r--r--   0 runner     (501) staff       (20)    12545 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/crc32c_sse4.cc
--rw-r--r--   0 runner     (501) staff       (20)     7511 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/crc32c_sse4.h
--rw-r--r--   0 runner     (501) staff       (20)     3336 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/crc32c_sse4_intrin.h
--rw-r--r--   0 runner     (501) staff       (20)     2223 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/crc_casts.h
--rw-r--r--   0 runner     (501) staff       (20)    21506 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/generic_crc.h
--rw-r--r--   0 runner     (501) staff       (20)     8663 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/gf_util.h
--rw-r--r--   0 runner     (501) staff       (20)     8211 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc
--rw-r--r--   0 runner     (501) staff       (20)     7459 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc
--rw-r--r--   0 runner     (501) staff       (20)     8601 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc
--rw-r--r--   0 runner     (501) staff       (20)     7945 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc
--rw-r--r--   0 runner     (501) staff       (20)     7379 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc
--rw-r--r--   0 runner     (501) staff       (20)     7264 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/platform.h
--rw-r--r--   0 runner     (501) staff       (20)     2266 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/protected_crc.h
--rw-r--r--   0 runner     (501) staff       (20)     3417 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/rolling_crc.h
--rw-r--r--   0 runner     (501) staff       (20)     1629 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/std_headers.h
--rw-r--r--   0 runner     (501) staff       (20)     8422 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/code/uint128_sse2.h
--rw-r--r--   0 runner     (501) staff       (20)     2231 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/config.h.in
--rw-r--r--   0 runner     (501) staff       (20)   212367 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/configure
--rw-r--r--   0 runner     (501) staff       (20)      744 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/configure.ac
--rw-r--r--   0 runner     (501) staff       (20)    18615 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/depcomp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-18 18:34:19.723875 sabctools-8.2.1/src/crcutil-1.0/examples/
--rw-r--r--   0 runner     (501) staff       (20)    10449 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/examples/interface.cc
--rw-r--r--   0 runner     (501) staff       (20)     8820 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/examples/interface.h
--rw-r--r--   0 runner     (501) staff       (20)     6390 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/examples/usage.cc
--rw-r--r--   0 runner     (501) staff       (20)    13663 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/install-sh
--rw-r--r--   0 runner     (501) staff       (20)    11419 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/missing
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-18 18:34:19.725549 sabctools-8.2.1/src/crcutil-1.0/tests/
--rw-r--r--   0 runner     (501) staff       (20)     2227 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/tests/aligned_alloc.h
--rw-r--r--   0 runner     (501) staff       (20)     2538 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/tests/bob_jenkins_rng.h
--rw-r--r--   0 runner     (501) staff       (20)     1915 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/tests/rdtsc.h
--rw-r--r--   0 runner     (501) staff       (20)     1803 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/tests/set_hi_pri.c
--rw-r--r--   0 runner     (501) staff       (20)     7593 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/tests/unittest.cc
--rw-r--r--   0 runner     (501) staff       (20)    33870 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/tests/unittest.h
--rw-r--r--   0 runner     (501) staff       (20)     1290 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/crcutil-1.0/tests/unittest_helper.h
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/py.typed
--rw-r--r--   0 runner     (501) staff       (20)     3961 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/sabctools.cc
--rw-r--r--   0 runner     (501) staff       (20)      963 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/sabctools.h
--rw-r--r--   0 runner     (501) staff       (20)      703 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/sabctools.pyi
--rw-r--r--   0 runner     (501) staff       (20)     3243 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/sparse.cc
--rw-r--r--   0 runner     (501) staff       (20)     1023 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/sparse.h
--rw-r--r--   0 runner     (501) staff       (20)     8637 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/unlocked_ssl.cc
--rw-r--r--   0 runner     (501) staff       (20)     1484 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/unlocked_ssl.h
--rw-r--r--   0 runner     (501) staff       (20)     1089 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/utils.cc
--rw-r--r--   0 runner     (501) staff       (20)      937 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/utils.h
--rw-r--r--   0 runner     (501) staff       (20)    10285 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yenc.cc
--rw-r--r--   0 runner     (501) staff       (20)     1388 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yenc.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-18 18:34:19.730235 sabctools-8.2.1/src/yencode/
--rw-r--r--   0 runner     (501) staff       (20)    10960 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/common.h
--rw-r--r--   0 runner     (501) staff       (20)     9326 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/crc.cc
--rw-r--r--   0 runner     (501) staff       (20)     2353 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/crc.h
--rw-r--r--   0 runner     (501) staff       (20)     6911 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/crc_arm.cc
--rw-r--r--   0 runner     (501) staff       (20)     6864 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/crc_arm_pmull.cc
--rw-r--r--   0 runner     (501) staff       (20)      589 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/crc_common.h
--rw-r--r--   0 runner     (501) staff       (20)    17801 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/crc_folding.cc
--rw-r--r--   0 runner     (501) staff       (20)     7011 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/crc_folding_256.cc
--rw-r--r--   0 runner     (501) staff       (20)     7289 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/crc_riscv.cc
--rw-r--r--   0 runner     (501) staff       (20)    10917 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder.cc
--rw-r--r--   0 runner     (501) staff       (20)     1878 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder.h
--rw-r--r--   0 runner     (501) staff       (20)      704 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_avx.cc
--rw-r--r--   0 runner     (501) staff       (20)      760 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_avx2.cc
--rw-r--r--   0 runner     (501) staff       (20)    23461 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_avx2_base.h
--rw-r--r--   0 runner     (501) staff       (20)     7641 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_common.h
--rw-r--r--   0 runner     (501) staff       (20)    17142 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_neon.cc
--rw-r--r--   0 runner     (501) staff       (20)    17359 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_neon64.cc
--rw-r--r--   0 runner     (501) staff       (20)    10838 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_rvv.cc
--rw-r--r--   0 runner     (501) staff       (20)     1382 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_sse2.cc
--rw-r--r--   0 runner     (501) staff       (20)    25288 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_sse_base.h
--rw-r--r--   0 runner     (501) staff       (20)      664 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_ssse3.cc
--rw-r--r--   0 runner     (501) staff       (20)     1426 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/decoder_vbmi2.cc
--rw-r--r--   0 runner     (501) staff       (20)     5395 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder.cc
--rw-r--r--   0 runner     (501) staff       (20)      608 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder.h
--rw-r--r--   0 runner     (501) staff       (20)      383 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_avx.cc
--rw-r--r--   0 runner     (501) staff       (20)      383 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_avx2.cc
--rw-r--r--   0 runner     (501) staff       (20)    21399 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_avx_base.h
--rw-r--r--   0 runner     (501) staff       (20)     2907 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_common.h
--rw-r--r--   0 runner     (501) staff       (20)    19077 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_neon.cc
--rw-r--r--   0 runner     (501) staff       (20)     6214 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_rvv.cc
--rw-r--r--   0 runner     (501) staff       (20)      320 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_sse2.cc
--rw-r--r--   0 runner     (501) staff       (20)    24611 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_sse_base.h
--rw-r--r--   0 runner     (501) staff       (20)      719 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_ssse3.cc
--rw-r--r--   0 runner     (501) staff       (20)      930 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/encoder_vbmi2.cc
--rw-r--r--   0 runner     (501) staff       (20)    77413 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/hedley.h
--rw-r--r--   0 runner     (501) staff       (20)     6465 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/platform.cc
--rw-r--r--   0 runner     (501) staff       (20)     7722 2024-05-18 18:31:21.000000 sabctools-8.2.1/src/yencode/stdint.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-18 18:34:19.732118 sabctools-8.2.1/tests/
--rw-r--r--   0 runner     (501) staff       (20)      550 2024-05-18 18:31:21.000000 sabctools-8.2.1/tests/test.py
--rw-r--r--   0 runner     (501) staff       (20)     2033 2024-05-18 18:31:21.000000 sabctools-8.2.1/tests/test_crc32.py
--rw-r--r--   0 runner     (501) staff       (20)     4092 2024-05-18 18:31:21.000000 sabctools-8.2.1/tests/test_decoder.py
--rw-r--r--   0 runner     (501) staff       (20)      204 2024-05-18 18:31:21.000000 sabctools-8.2.1/tests/test_encoder.py
--rw-r--r--   0 runner     (501) staff       (20)     1123 2024-05-18 18:31:21.000000 sabctools-8.2.1/tests/test_sparse.py
--rw-r--r--   0 runner     (501) staff       (20)    12761 2024-05-18 18:31:21.000000 sabctools-8.2.1/tests/test_unlocked_ssl.py
--rw-r--r--   0 runner     (501) staff       (20)      402 2024-05-18 18:31:21.000000 sabctools-8.2.1/tests/test_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     5879 2024-05-18 18:31:21.000000 sabctools-8.2.1/tests/testsupport.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.899271 sabctools-8.2.2/
+-rw-r--r--   0 runner     (501) staff       (20)    17990 2024-05-19 11:06:14.000000 sabctools-8.2.2/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)       24 2024-05-19 11:06:14.000000 sabctools-8.2.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3122 2024-05-19 11:09:48.899075 sabctools-8.2.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2348 2024-05-19 11:06:14.000000 sabctools-8.2.2/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-19 11:06:14.000000 sabctools-8.2.2/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.870139 sabctools-8.2.2/sabctools.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3122 2024-05-19 11:09:48.000000 sabctools-8.2.2/sabctools.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3095 2024-05-19 11:09:48.000000 sabctools-8.2.2/sabctools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-19 11:09:48.000000 sabctools-8.2.2/sabctools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-05-19 11:09:48.000000 sabctools-8.2.2/sabctools.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-19 11:09:48.899316 sabctools-8.2.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)    17185 2024-05-19 11:06:14.000000 sabctools-8.2.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.872348 sabctools-8.2.2/src/
+-rw-r--r--   0 runner     (501) staff       (20)      108 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2284 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crc32.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1127 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crc32.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.882966 sabctools-8.2.2/src/crcutil-1.0/
+-rw-r--r--   0 runner     (501) staff       (20)       54 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/AUTHORS
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/COPYING
+-rw-r--r--   0 runner     (501) staff       (20)       58 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/ChangeLog
+-rw-r--r--   0 runner     (501) staff       (20)     1700 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/INSTALL
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    50573 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)     1210 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/Makefile.am
+-rw-r--r--   0 runner     (501) staff       (20)    56163 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/Makefile.in
+-rw-r--r--   0 runner     (501) staff       (20)     2076 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/Makefile.win
+-rw-r--r--   0 runner     (501) staff       (20)       60 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/NEWS
+-rw-r--r--   0 runner     (501) staff       (20)     6669 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/README
+-rw-r--r--   0 runner     (501) staff       (20)    34611 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/aclocal.m4
+-rw-r--r--   0 runner     (501) staff       (20)     2785 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/autogen.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.886583 sabctools-8.2.2/src/crcutil-1.0/code/
+-rw-r--r--   0 runner     (501) staff       (20)     2368 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/base_types.h
+-rw-r--r--   0 runner     (501) staff       (20)    12545 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7511 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4.h
+-rw-r--r--   0 runner     (501) staff       (20)     3336 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4_intrin.h
+-rw-r--r--   0 runner     (501) staff       (20)     2223 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/crc_casts.h
+-rw-r--r--   0 runner     (501) staff       (20)    21506 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/generic_crc.h
+-rw-r--r--   0 runner     (501) staff       (20)     8663 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/gf_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     8211 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7459 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8601 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7945 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7379 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7264 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/platform.h
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/protected_crc.h
+-rw-r--r--   0 runner     (501) staff       (20)     3417 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/rolling_crc.h
+-rw-r--r--   0 runner     (501) staff       (20)     1629 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/std_headers.h
+-rw-r--r--   0 runner     (501) staff       (20)     8422 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/uint128_sse2.h
+-rw-r--r--   0 runner     (501) staff       (20)     2231 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/config.h.in
+-rw-r--r--   0 runner     (501) staff       (20)   212367 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/configure
+-rw-r--r--   0 runner     (501) staff       (20)      744 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/configure.ac
+-rw-r--r--   0 runner     (501) staff       (20)    18615 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/depcomp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.887005 sabctools-8.2.2/src/crcutil-1.0/examples/
+-rw-r--r--   0 runner     (501) staff       (20)    10449 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/examples/interface.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8820 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/examples/interface.h
+-rw-r--r--   0 runner     (501) staff       (20)     6390 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/examples/usage.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13663 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/install-sh
+-rw-r--r--   0 runner     (501) staff       (20)    11419 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/missing
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.889545 sabctools-8.2.2/src/crcutil-1.0/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     2227 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/aligned_alloc.h
+-rw-r--r--   0 runner     (501) staff       (20)     2538 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/bob_jenkins_rng.h
+-rw-r--r--   0 runner     (501) staff       (20)     1915 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/rdtsc.h
+-rw-r--r--   0 runner     (501) staff       (20)     1803 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/set_hi_pri.c
+-rw-r--r--   0 runner     (501) staff       (20)     7593 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/unittest.cc
+-rw-r--r--   0 runner     (501) staff       (20)    33870 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/unittest.h
+-rw-r--r--   0 runner     (501) staff       (20)     1290 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/unittest_helper.h
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/py.typed
+-rw-r--r--   0 runner     (501) staff       (20)     3961 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sabctools.cc
+-rw-r--r--   0 runner     (501) staff       (20)      963 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sabctools.h
+-rw-r--r--   0 runner     (501) staff       (20)      703 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sabctools.pyi
+-rw-r--r--   0 runner     (501) staff       (20)     3243 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sparse.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1023 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sparse.h
+-rw-r--r--   0 runner     (501) staff       (20)     8637 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/unlocked_ssl.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1484 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/unlocked_ssl.h
+-rw-r--r--   0 runner     (501) staff       (20)     1089 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/utils.cc
+-rw-r--r--   0 runner     (501) staff       (20)      937 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/utils.h
+-rw-r--r--   0 runner     (501) staff       (20)    10285 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yenc.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1388 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yenc.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.896058 sabctools-8.2.2/src/yencode/
+-rw-r--r--   0 runner     (501) staff       (20)    10960 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     9326 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2476 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc.h
+-rw-r--r--   0 runner     (501) staff       (20)     6911 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_arm.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6864 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_arm_pmull.cc
+-rw-r--r--   0 runner     (501) staff       (20)      589 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_common.h
+-rw-r--r--   0 runner     (501) staff       (20)    17801 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_folding.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7011 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_folding_256.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7289 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_riscv.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10917 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1878 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder.h
+-rw-r--r--   0 runner     (501) staff       (20)      704 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_avx.cc
+-rw-r--r--   0 runner     (501) staff       (20)      760 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_avx2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    23461 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_avx2_base.h
+-rw-r--r--   0 runner     (501) staff       (20)     7641 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_common.h
+-rw-r--r--   0 runner     (501) staff       (20)    17142 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_neon.cc
+-rw-r--r--   0 runner     (501) staff       (20)    17359 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_neon64.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10838 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_rvv.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1382 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_sse2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    25288 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_sse_base.h
+-rw-r--r--   0 runner     (501) staff       (20)      664 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_ssse3.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1426 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_vbmi2.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5395 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder.cc
+-rw-r--r--   0 runner     (501) staff       (20)      608 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder.h
+-rw-r--r--   0 runner     (501) staff       (20)      383 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_avx.cc
+-rw-r--r--   0 runner     (501) staff       (20)      383 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_avx2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    21399 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_avx_base.h
+-rw-r--r--   0 runner     (501) staff       (20)     2907 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_common.h
+-rw-r--r--   0 runner     (501) staff       (20)    19077 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_neon.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6214 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_rvv.cc
+-rw-r--r--   0 runner     (501) staff       (20)      320 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_sse2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    24611 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_sse_base.h
+-rw-r--r--   0 runner     (501) staff       (20)      719 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_ssse3.cc
+-rw-r--r--   0 runner     (501) staff       (20)      930 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_vbmi2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    77413 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/hedley.h
+-rw-r--r--   0 runner     (501) staff       (20)     6465 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/platform.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7722 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/stdint.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.898753 sabctools-8.2.2/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      550 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test.py
+-rw-r--r--   0 runner     (501) staff       (20)     2033 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_crc32.py
+-rw-r--r--   0 runner     (501) staff       (20)     4092 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_decoder.py
+-rw-r--r--   0 runner     (501) staff       (20)      204 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_encoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     1123 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_sparse.py
+-rw-r--r--   0 runner     (501) staff       (20)    12761 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_unlocked_ssl.py
+-rw-r--r--   0 runner     (501) staff       (20)      402 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     5879 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/testsupport.py
```

### Comparing `sabctools-8.2.1/LICENSE.md` & `sabctools-8.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/PKG-INFO` & `sabctools-8.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabctools
-Version: 8.2.1
+Version: 8.2.2
 Summary: C implementations of functions for use within SABnzbd
 Home-page: https://github.com/sabnzbd/sabctools/
 Author: Safihre
 Author-email: safihre@sabnzbd.org
 License: GPLv2+
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sabctools-8.2.1/README.md` & `sabctools-8.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/sabctools.egg-info/PKG-INFO` & `sabctools-8.2.2/sabctools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabctools
-Version: 8.2.1
+Version: 8.2.2
 Summary: C implementations of functions for use within SABnzbd
 Home-page: https://github.com/sabnzbd/sabctools/
 Author: Safihre
 Author-email: safihre@sabnzbd.org
 License: GPLv2+
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sabctools-8.2.1/sabctools.egg-info/SOURCES.txt` & `sabctools-8.2.2/sabctools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/setup.py` & `sabctools-8.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crc32.cc` & `sabctools-8.2.2/src/crc32.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crc32.h` & `sabctools-8.2.2/src/crc32.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/COPYING` & `sabctools-8.2.2/src/crcutil-1.0/COPYING`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/INSTALL` & `sabctools-8.2.2/src/crcutil-1.0/INSTALL`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/LICENSE` & `sabctools-8.2.2/src/crcutil-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/Makefile` & `sabctools-8.2.2/src/crcutil-1.0/Makefile`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/Makefile.am` & `sabctools-8.2.2/src/crcutil-1.0/Makefile.am`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/Makefile.in` & `sabctools-8.2.2/src/crcutil-1.0/Makefile.in`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/Makefile.win` & `sabctools-8.2.2/src/crcutil-1.0/Makefile.win`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/README` & `sabctools-8.2.2/src/crcutil-1.0/README`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/aclocal.m4` & `sabctools-8.2.2/src/crcutil-1.0/aclocal.m4`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/autogen.sh` & `sabctools-8.2.2/src/crcutil-1.0/autogen.sh`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/base_types.h` & `sabctools-8.2.2/src/crcutil-1.0/code/base_types.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/crc32c_sse4.cc` & `sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/crc32c_sse4.h` & `sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/crc32c_sse4_intrin.h` & `sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4_intrin.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/crc_casts.h` & `sabctools-8.2.2/src/crcutil-1.0/code/crc_casts.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/generic_crc.h` & `sabctools-8.2.2/src/crcutil-1.0/code/generic_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/gf_util.h` & `sabctools-8.2.2/src/crcutil-1.0/code/gf_util.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc` & `sabctools-8.2.2/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc` & `sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc` & `sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc` & `sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc` & `sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/platform.h` & `sabctools-8.2.2/src/crcutil-1.0/code/platform.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/protected_crc.h` & `sabctools-8.2.2/src/crcutil-1.0/code/protected_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/rolling_crc.h` & `sabctools-8.2.2/src/crcutil-1.0/code/rolling_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/std_headers.h` & `sabctools-8.2.2/src/crcutil-1.0/code/std_headers.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/code/uint128_sse2.h` & `sabctools-8.2.2/src/crcutil-1.0/code/uint128_sse2.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/config.h.in` & `sabctools-8.2.2/src/crcutil-1.0/config.h.in`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/configure` & `sabctools-8.2.2/src/crcutil-1.0/configure`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/configure.ac` & `sabctools-8.2.2/src/crcutil-1.0/configure.ac`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/depcomp` & `sabctools-8.2.2/src/crcutil-1.0/depcomp`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/examples/interface.cc` & `sabctools-8.2.2/src/crcutil-1.0/examples/interface.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/examples/interface.h` & `sabctools-8.2.2/src/crcutil-1.0/examples/interface.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/examples/usage.cc` & `sabctools-8.2.2/src/crcutil-1.0/examples/usage.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/install-sh` & `sabctools-8.2.2/src/crcutil-1.0/install-sh`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/missing` & `sabctools-8.2.2/src/crcutil-1.0/missing`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/tests/aligned_alloc.h` & `sabctools-8.2.2/src/crcutil-1.0/tests/aligned_alloc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/tests/bob_jenkins_rng.h` & `sabctools-8.2.2/src/crcutil-1.0/tests/bob_jenkins_rng.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/tests/rdtsc.h` & `sabctools-8.2.2/src/crcutil-1.0/tests/rdtsc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/tests/set_hi_pri.c` & `sabctools-8.2.2/src/crcutil-1.0/tests/set_hi_pri.c`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/tests/unittest.cc` & `sabctools-8.2.2/src/crcutil-1.0/tests/unittest.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/tests/unittest.h` & `sabctools-8.2.2/src/crcutil-1.0/tests/unittest.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/crcutil-1.0/tests/unittest_helper.h` & `sabctools-8.2.2/src/crcutil-1.0/tests/unittest_helper.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/sabctools.cc` & `sabctools-8.2.2/src/sabctools.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/sabctools.h` & `sabctools-8.2.2/src/sabctools.h`

 * *Files 14% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 
 #include <Python.h>
 #include <stdio.h>
 #include <fcntl.h>
 #include <string.h>
 
 /* Version information */
-#define SABCTOOLS_VERSION "8.2.1"
+#define SABCTOOLS_VERSION "8.2.2"
 
 PyMODINIT_FUNC PyInit_sabctools(void);
```

### Comparing `sabctools-8.2.1/src/sabctools.pyi` & `sabctools-8.2.2/src/sabctools.pyi`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/sparse.cc` & `sabctools-8.2.2/src/sparse.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/sparse.h` & `sabctools-8.2.2/src/sparse.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/unlocked_ssl.cc` & `sabctools-8.2.2/src/unlocked_ssl.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/unlocked_ssl.h` & `sabctools-8.2.2/src/unlocked_ssl.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/utils.cc` & `sabctools-8.2.2/src/utils.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/utils.h` & `sabctools-8.2.2/src/utils.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yenc.cc` & `sabctools-8.2.2/src/yenc.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yenc.h` & `sabctools-8.2.2/src/yenc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/common.h` & `sabctools-8.2.2/src/yencode/common.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/crc.cc` & `sabctools-8.2.2/src/yencode/crc.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/crc.h` & `sabctools-8.2.2/src/yencode/crc.h`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 static inline int crc32_isa_level() {
 	return _crc32_isa;
 }
 
 
 // computes `n % 0xffffffff` (well, almost), using some bit-hacks
 static inline uint32_t crc32_powmod(uint64_t n) {
-#ifdef __GNUC__
+#if defined(__GNUC__) && (__GNUC__ >= 5 || (defined(__clang__) && (__clang_major__ > 3 || (__clang_major__ == 3 && __clang_minor__ > 3))))
 	unsigned res;
 	unsigned carry = __builtin_uadd_overflow(n >> 32, n, &res);
 	res += carry;
 	return res;
 #elif defined(_MSC_VER) && defined(PLATFORM_X86)
 	unsigned res;
 	unsigned char carry = _addcarry_u32(0, n >> 32, n, &res);
```

### Comparing `sabctools-8.2.1/src/yencode/crc_arm.cc` & `sabctools-8.2.2/src/yencode/crc_arm.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/crc_arm_pmull.cc` & `sabctools-8.2.2/src/yencode/crc_arm_pmull.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/crc_common.h` & `sabctools-8.2.2/src/yencode/crc_common.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/crc_folding.cc` & `sabctools-8.2.2/src/yencode/crc_folding.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/crc_folding_256.cc` & `sabctools-8.2.2/src/yencode/crc_folding_256.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/crc_riscv.cc` & `sabctools-8.2.2/src/yencode/crc_riscv.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder.cc` & `sabctools-8.2.2/src/yencode/decoder.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder.h` & `sabctools-8.2.2/src/yencode/decoder.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_avx.cc` & `sabctools-8.2.2/src/yencode/decoder_avx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_avx2.cc` & `sabctools-8.2.2/src/yencode/decoder_avx2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_avx2_base.h` & `sabctools-8.2.2/src/yencode/decoder_avx2_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_common.h` & `sabctools-8.2.2/src/yencode/decoder_common.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_neon.cc` & `sabctools-8.2.2/src/yencode/decoder_neon.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_neon64.cc` & `sabctools-8.2.2/src/yencode/decoder_neon64.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_rvv.cc` & `sabctools-8.2.2/src/yencode/decoder_rvv.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_sse2.cc` & `sabctools-8.2.2/src/yencode/decoder_sse2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_sse_base.h` & `sabctools-8.2.2/src/yencode/decoder_sse_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_ssse3.cc` & `sabctools-8.2.2/src/yencode/decoder_ssse3.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/decoder_vbmi2.cc` & `sabctools-8.2.2/src/yencode/decoder_vbmi2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/encoder.cc` & `sabctools-8.2.2/src/yencode/encoder.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/encoder.h` & `sabctools-8.2.2/src/yencode/encoder.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/encoder_avx_base.h` & `sabctools-8.2.2/src/yencode/encoder_avx_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/encoder_common.h` & `sabctools-8.2.2/src/yencode/encoder_common.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/encoder_neon.cc` & `sabctools-8.2.2/src/yencode/encoder_neon.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/encoder_rvv.cc` & `sabctools-8.2.2/src/yencode/encoder_rvv.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/encoder_sse_base.h` & `sabctools-8.2.2/src/yencode/encoder_sse_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/encoder_ssse3.cc` & `sabctools-8.2.2/src/yencode/encoder_ssse3.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/encoder_vbmi2.cc` & `sabctools-8.2.2/src/yencode/encoder_vbmi2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/hedley.h` & `sabctools-8.2.2/src/yencode/hedley.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/platform.cc` & `sabctools-8.2.2/src/yencode/platform.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/src/yencode/stdint.h` & `sabctools-8.2.2/src/yencode/stdint.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/tests/test.py` & `sabctools-8.2.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/tests/test_crc32.py` & `sabctools-8.2.2/tests/test_crc32.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/tests/test_decoder.py` & `sabctools-8.2.2/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/tests/test_sparse.py` & `sabctools-8.2.2/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/tests/test_unlocked_ssl.py` & `sabctools-8.2.2/tests/test_unlocked_ssl.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.1/tests/testsupport.py` & `sabctools-8.2.2/tests/testsupport.py`

 * *Files identical despite different names*

