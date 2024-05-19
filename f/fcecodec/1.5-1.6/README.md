# Comparing `tmp/fcecodec-1.5.tar.gz` & `tmp/fcecodec-1.6-cp310-cp310-musllinux_1_2_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcecodec-1.5.tar", last modified: Sun Apr 28 13:40:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

