# Comparing `tmp/django_relay_endpoint-1.2.0.tar.gz` & `tmp/django_relay_endpoint-2.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_relay_endpoint-1.2.0.tar", last modified: Fri Dec 15 12:40:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

