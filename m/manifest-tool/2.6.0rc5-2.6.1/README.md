# Comparing `tmp/manifest-tool-2.6.0rc5.tar.gz` & `tmp/manifest_tool-2.6.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifest-tool-2.6.0rc5.tar", last modified: Wed Nov 15 10:16:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

