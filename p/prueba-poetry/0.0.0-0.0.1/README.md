# Comparing `tmp/prueba_poetry-0.0.0.tar.gz` & `tmp/prueba_poetry-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prueba_poetry-0.0.0.tar", max compression
+gzip compressed data, was "prueba_poetry-0.0.1.tar", max compression
```

## Comparing `prueba_poetry-0.0.0.tar` & `prueba_poetry-0.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-05-19 00:21:36.326416 prueba_poetry-0.0.0/prueba_poetry/__init__.py
--rw-r--r--   0        0        0      298 2024-05-19 00:21:43.057565 prueba_poetry-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 00:21:36.326416 prueba_poetry-0.0.0/README.md
--rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 prueba_poetry-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-19 00:21:36.326416 prueba_poetry-0.0.1/prueba_poetry/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-19 00:36:07.281773 prueba_poetry-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 00:21:36.326416 prueba_poetry-0.0.1/README.md
+-rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 prueba_poetry-0.0.1/PKG-INFO
```

