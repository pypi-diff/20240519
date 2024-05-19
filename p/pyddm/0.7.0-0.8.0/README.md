# Comparing `tmp/pyddm-0.7.0.tar.gz` & `tmp/pyddm-0.8.0-cp310-cp310-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyddm-0.7.0.tar", last modified: Sun Jul  2 15:02:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

