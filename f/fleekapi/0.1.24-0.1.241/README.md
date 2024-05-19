# Comparing `tmp/fleekapi-0.1.24.tar.gz` & `tmp/fleekapi-0.1.241-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.1.24.tar", last modified: Sun May 19 14:23:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

