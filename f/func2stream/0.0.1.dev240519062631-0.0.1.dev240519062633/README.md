# Comparing `tmp/func2stream-0.0.1.dev240519062631.tar.gz` & `tmp/func2stream-0.0.1.dev240519062633-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func2stream-0.0.1.dev240519062631.tar", last modified: Sun May 19 06:26:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

