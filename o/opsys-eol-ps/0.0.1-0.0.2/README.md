# Comparing `tmp/opsys-eol-ps-0.0.1.tar.gz` & `tmp/opsys-eol-ps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Z:\opt\atlassian\pipelines\agent\build\dist\.tmp-1rxzh74r\opsys-eol-ps-0.0.1.tar", last modified: Thu Feb 22 15:18:35 2024, max compression
+gzip compressed data, was "Z:\opt\atlassian\pipelines\agent\build\dist\.tmp-xyy952bz\opsys-eol-ps-0.0.2.tar", last modified: Sun May 19 15:19:12 2024, max compression
```

## Comparing `opsys-eol-ps-0.0.1.tar` & `opsys-eol-ps-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/
--rw-rw-rw-   0        0        0     1073 2024-02-22 15:17:59.000000 opsys-eol-ps-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      344 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      924 2024-02-22 15:17:59.000000 opsys-eol-ps-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/opsys_eol_ps/
--rw-rw-rw-   0        0        0       98 2024-02-22 15:17:59.000000 opsys-eol-ps-0.0.1/opsys_eol_ps/__init__.py
--rw-rw-rw-   0        0        0     7236 2024-02-22 15:17:59.000000 opsys-eol-ps-0.0.1/opsys_eol_ps/eol_ps.py
-drwxrwxrwx   0        0        0        0 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/opsys_eol_ps.egg-info/
--rw-rw-rw-   0        0        0      344 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/opsys_eol_ps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/opsys_eol_ps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/opsys_eol_ps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-22 15:18:34.000000 opsys-eol-ps-0.0.1/opsys_eol_ps.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/opsys_eol_ps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/opsys_eol_ps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-02-22 15:17:59.000000 opsys-eol-ps-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-22 15:18:35.000000 opsys-eol-ps-0.0.1/test/
--rw-rw-rw-   0        0        0       75 2024-02-22 15:17:59.000000 opsys-eol-ps-0.0.1/test/__init__.py
--rw-rw-rw-   0        0        0     4236 2024-02-22 15:17:59.000000 opsys-eol-ps-0.0.1/test/test_eol_ps.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/
+-rw-rw-rw-   0        0        0     1073 2024-05-19 15:18:53.000000 opsys-eol-ps-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      344 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      924 2024-05-19 15:18:53.000000 opsys-eol-ps-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/opsys_eol_ps/
+-rw-rw-rw-   0        0        0       98 2024-05-19 15:18:53.000000 opsys-eol-ps-0.0.2/opsys_eol_ps/__init__.py
+-rw-rw-rw-   0        0        0     7236 2024-05-19 15:18:53.000000 opsys-eol-ps-0.0.2/opsys_eol_ps/eol_ps.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/opsys_eol_ps.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/opsys_eol_ps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/opsys_eol_ps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/opsys_eol_ps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/opsys_eol_ps.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/opsys_eol_ps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/opsys_eol_ps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-19 15:18:53.000000 opsys-eol-ps-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:19:12.000000 opsys-eol-ps-0.0.2/test/
+-rw-rw-rw-   0        0        0       75 2024-05-19 15:18:53.000000 opsys-eol-ps-0.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     4236 2024-05-19 15:18:53.000000 opsys-eol-ps-0.0.2/test/test_eol_ps.py
```

### Comparing `opsys-eol-ps-0.0.1/LICENSE` & `opsys-eol-ps-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opsys-eol-ps-0.0.1/README.md` & `opsys-eol-ps-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `opsys-eol-ps-0.0.1/opsys_eol_ps/eol_ps.py` & `opsys-eol-ps-0.0.2/opsys_eol_ps/eol_ps.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,27 +128,27 @@
     def get_output_state(self, ):
         """
         Get the output state of the power supply device.
 
         Returns:
             bool: True if output is active, False otherwise.
         """
-        return self.read_holding_reg(5) != 0
+        return self.read_holding_reg(0) != 0
 
     def set_output_state(self, mode):
         """
         Set the output state of the power supply device.
 
         Args:
             mode (bool): Desired state of the output (True for ON, False for OFF).
         """
         value = 0
         if(mode):
             value = 1
-        self.write_holding_reg(5, value)
+        self.write_holding_reg(0, value)
 
 
     def get_volt(self, ):
         """
         Get the voltage output set on the power supply device.
 
         Returns:
```

### Comparing `opsys-eol-ps-0.0.1/setup.py` & `opsys-eol-ps-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     targets = []
     if fname.exists():
         with open(fname, 'r') as f:
             targets = f.read().splitlines()
     return targets
 
 setuptools.setup(name='opsys-eol-ps',
-                 version='0.0.1',
+                 version='0.0.2',
                  description='python package for the eol power supply',
                  url='https://bitbucket.org/opsys_tech/opsys_eol_ps/src/master/',
                  download_url='https://bitbucket.org/opsys_tech/opsys_eol_ps/src/master/',
                  author='nerya.lifshitz',
                  install_requires=get_install_requirements(),
                  author_email='nerya.lifshitz@opsys-tech.com',
                  packages=setuptools.find_packages(),
```

### Comparing `opsys-eol-ps-0.0.1/test/test_eol_ps.py` & `opsys-eol-ps-0.0.2/test/test_eol_ps.py`

 * *Files identical despite different names*

