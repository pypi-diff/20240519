# Comparing `tmp/pyrodigal-3.3.0.tar.gz` & `tmp/pyrodigal-3.4.0-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrodigal-3.3.0.tar", last modified: Wed Jan 24 19:43:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

