# Comparing `tmp/pyphy2D-1.0.tar.gz` & `tmp/pyphy2D-2.0.0-cp312-cp312-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphy2D-1.0.tar", last modified: Sat May 18 12:08:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

