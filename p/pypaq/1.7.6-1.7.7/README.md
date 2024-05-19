# Comparing `tmp/pypaq-1.7.6.tar.gz` & `tmp/pypaq-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaq-1.7.6.tar", last modified: Tue Apr 23 11:27:37 2024, max compression
+gzip compressed data, was "pypaq-1.7.7.tar", last modified: Sun May 19 18:33:21 2024, max compression
```

## Comparing `pypaq-1.7.6.tar` & `pypaq-1.7.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.587747 pypaq-1.7.6/
--rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-04-23 11:27:37.587747 pypaq-1.7.6/PKG-INFO
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      470 2024-04-06 17:44:30.000000 pypaq-1.7.6/README.md
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.579747 pypaq-1.7.6/pypaq/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/__init__.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       41 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/exception.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq/lipytools/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/__init__.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     4111 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/decorators.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      826 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/double_hinge.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     3930 2024-04-06 21:52:22.000000 pypaq-1.7.6/pypaq/lipytools/files.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     1531 2024-04-07 18:56:30.000000 pypaq-1.7.6/pypaq/lipytools/moving_average.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     4908 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/plots.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     6044 2024-04-22 18:29:22.000000 pypaq-1.7.6/pypaq/lipytools/printout.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     2361 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/pylogger.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       73 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/softmax.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)      977 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/stats.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     1941 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/time_reporter.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq/mpython/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/mpython/__init__.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1570 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/mpython/mpdecor.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     5528 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/mpython/mptools.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq/pms/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/__init__.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     4582 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/base.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     3651 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/config_manager.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     8354 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/para.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)    13853 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/parasave.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)    18707 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/paspa.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     6863 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/points_cloud.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      211 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pytypes.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq/textools/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/textools/__init__.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1210 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/textools/text_metrics.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      668 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/textools/text_processing.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq.egg-info/
--rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/PKG-INFO
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      852 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/SOURCES.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        1 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/dependency_links.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       63 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/requires.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        6 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/top_level.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       38 2024-04-23 11:27:37.587747 pypaq-1.7.6/setup.cfg
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      491 2024-04-23 11:27:35.000000 pypaq-1.7.6/setup.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-05-19 18:33:21.211969 pypaq-1.7.7/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-05-19 18:33:21.211969 pypaq-1.7.7/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      470 2024-04-06 17:44:30.000000 pypaq-1.7.7/README.md
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-05-19 18:33:21.207969 pypaq-1.7.7/pypaq/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       41 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/exception.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-05-19 18:33:21.207969 pypaq-1.7.7/pypaq/lipytools/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/lipytools/__init__.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     4111 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/lipytools/decorators.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      826 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/lipytools/double_hinge.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3930 2024-04-06 21:52:22.000000 pypaq-1.7.7/pypaq/lipytools/files.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     1531 2024-04-07 18:56:30.000000 pypaq-1.7.7/pypaq/lipytools/moving_average.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     5011 2024-05-19 17:22:28.000000 pypaq-1.7.7/pypaq/lipytools/plots.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     6044 2024-04-22 18:29:22.000000 pypaq-1.7.7/pypaq/lipytools/printout.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2361 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/lipytools/pylogger.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       73 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/lipytools/softmax.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)      977 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/lipytools/stats.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     1941 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/lipytools/time_reporter.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-05-19 18:33:21.207969 pypaq-1.7.7/pypaq/mpython/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/mpython/__init__.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1570 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/mpython/mpdecor.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     5528 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/mpython/mptools.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-05-19 18:33:21.211969 pypaq-1.7.7/pypaq/pms/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/pms/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     4582 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/pms/base.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3358 2024-05-07 09:00:32.000000 pypaq-1.7.7/pypaq/pms/config_manager.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     8354 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/pms/para.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)    13853 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/pms/parasave.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)    18707 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/pms/paspa.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     6863 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/pms/points_cloud.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      211 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/pytypes.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-05-19 18:33:21.211969 pypaq-1.7.7/pypaq/textools/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/textools/__init__.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1210 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/textools/text_metrics.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      668 2024-04-06 17:44:30.000000 pypaq-1.7.7/pypaq/textools/text_processing.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-05-19 18:33:21.211969 pypaq-1.7.7/pypaq.egg-info/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-05-19 18:33:21.000000 pypaq-1.7.7/pypaq.egg-info/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      852 2024-05-19 18:33:21.000000 pypaq-1.7.7/pypaq.egg-info/SOURCES.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        1 2024-05-19 18:33:21.000000 pypaq-1.7.7/pypaq.egg-info/dependency_links.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       63 2024-05-19 18:33:21.000000 pypaq-1.7.7/pypaq.egg-info/requires.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        6 2024-05-19 18:33:21.000000 pypaq-1.7.7/pypaq.egg-info/top_level.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       38 2024-05-19 18:33:21.211969 pypaq-1.7.7/setup.cfg
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      491 2024-05-19 18:33:18.000000 pypaq-1.7.7/setup.py
```

### Comparing `pypaq-1.7.6/pypaq/lipytools/decorators.py` & `pypaq-1.7.7/pypaq/lipytools/decorators.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/lipytools/double_hinge.py` & `pypaq-1.7.7/pypaq/lipytools/double_hinge.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/lipytools/files.py` & `pypaq-1.7.7/pypaq/lipytools/files.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/lipytools/moving_average.py` & `pypaq-1.7.7/pypaq/lipytools/moving_average.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/lipytools/plots.py` & `pypaq-1.7.7/pypaq/lipytools/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,27 +60,29 @@
 
 
 def two_dim(
         y: Union[List,np.ndarray],                  # two(yx) or one(y) dim list or np.array
         x: Optional[Union[List,np.ndarray]]=    None,
         name=                                   'values',
         save_FD: str =                          None,
+        scatter=                                False,
         xlogscale=                              False,
         ylogscale=                              False,
         legend_loc=                             'upper left'):
 
     if type(y) is list: y = np.asarray(y)
     if x is None:
         if len(y.shape) < 2: x = np.arange(len(y))
         else:
             x = y[:, 1]
             y = y[:, 0]
 
     plt.clf()
-    plt.plot(x, y, label=name)
+    plot_f = plt.scatter if scatter else plt.plot
+    plot_f(x, y, label=name)
     if xlogscale: plt.xscale('log')
     if ylogscale: plt.yscale('log')
     plt.legend(loc=legend_loc)
     plt.grid(True)
     if save_FD:
         prep_folder(save_FD)
         plt.savefig(f'{save_FD}/{name}.png')
```

### Comparing `pypaq-1.7.6/pypaq/lipytools/printout.py` & `pypaq-1.7.7/pypaq/lipytools/printout.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/lipytools/pylogger.py` & `pypaq-1.7.7/pypaq/lipytools/pylogger.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/lipytools/stats.py` & `pypaq-1.7.7/pypaq/lipytools/stats.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/lipytools/time_reporter.py` & `pypaq-1.7.7/pypaq/lipytools/time_reporter.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/mpython/mpdecor.py` & `pypaq-1.7.7/pypaq/mpython/mpdecor.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/mpython/mptools.py` & `pypaq-1.7.7/pypaq/mpython/mptools.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/pms/base.py` & `pypaq-1.7.7/pypaq/pms/base.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/pms/para.py` & `pypaq-1.7.7/pypaq/pms/para.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/pms/parasave.py` & `pypaq-1.7.7/pypaq/pms/parasave.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/pms/paspa.py` & `pypaq-1.7.7/pypaq/pms/paspa.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/pms/points_cloud.py` & `pypaq-1.7.7/pypaq/pms/points_cloud.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/textools/text_metrics.py` & `pypaq-1.7.7/pypaq/textools/text_metrics.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq/textools/text_processing.py` & `pypaq-1.7.7/pypaq/textools/text_processing.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.6/pypaq.egg-info/SOURCES.txt` & `pypaq-1.7.7/pypaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

