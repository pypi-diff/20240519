# Comparing `tmp/func2stream-0.0.1.dev240519063723.tar.gz` & `tmp/func2stream-0.0.1.dev240519063726-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func2stream-0.0.1.dev240519063723.tar", last modified: Sun May 19 06:37:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

