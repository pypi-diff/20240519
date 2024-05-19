# Comparing `tmp/conf-mat-1.0.5.tar.gz` & `tmp/conf_mat-1.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf-mat-1.0.5.tar", last modified: Sat May 18 23:45:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

