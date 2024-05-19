# Comparing `tmp/txm_sandbox-0.3.1.post1.tar.gz` & `tmp/txm_sandbox-0.3.1.post2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txm_sandbox-0.3.1.post1.tar", last modified: Sat May 18 02:17:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

