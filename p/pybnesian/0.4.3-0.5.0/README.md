# Comparing `tmp/pybnesian-0.4.3.tar.gz` & `tmp/pybnesian-0.5.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybnesian-0.4.3.tar", last modified: Sun Oct 23 11:52:16 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

