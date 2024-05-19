# Comparing `tmp/func2stream-0.0.1.dev240519060652.tar.gz` & `tmp/func2stream-0.0.1.dev240519060655-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func2stream-0.0.1.dev240519060652.tar", last modified: Sun May 19 06:06:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

