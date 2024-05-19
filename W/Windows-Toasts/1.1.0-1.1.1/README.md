# Comparing `tmp/Windows-Toasts-1.1.0.tar.gz` & `tmp/windows_toasts-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Windows-Toasts-1.1.0.tar", last modified: Mon Feb 12 23:02:17 2024, max compression
+gzip compressed data, was "windows_toasts-1.1.1.tar", last modified: Sun May 19 11:32:36 2024, max compression
```

## Comparing `Windows-Toasts-1.1.0.tar` & `windows_toasts-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-02-12 23:02:17.195196 Windows-Toasts-1.1.0/
--rw-rw-rw-   0        0        0    11556 2022-02-19 10:55:53.000000 Windows-Toasts-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       69 2023-03-18 13:54:37.000000 Windows-Toasts-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3656 2024-02-12 23:02:17.194197 Windows-Toasts-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2407 2023-08-16 15:26:29.000000 Windows-Toasts-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-12 23:02:17.193200 Windows-Toasts-1.1.0/Windows_Toasts.egg-info/
--rw-rw-rw-   0        0        0     3656 2024-02-12 23:02:16.000000 Windows-Toasts-1.1.0/Windows_Toasts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      746 2024-02-12 23:02:16.000000 Windows-Toasts-1.1.0/Windows_Toasts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-12 23:02:16.000000 Windows-Toasts-1.1.0/Windows_Toasts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-02-12 23:02:16.000000 Windows-Toasts-1.1.0/Windows_Toasts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-24 23:36:24.000000 Windows-Toasts-1.1.0/Windows_Toasts.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      179 2024-02-12 23:02:16.000000 Windows-Toasts-1.1.0/Windows_Toasts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-02-12 23:02:16.000000 Windows-Toasts-1.1.0/Windows_Toasts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      362 2023-03-18 13:17:33.000000 Windows-Toasts-1.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-02-12 23:02:16.871724 Windows-Toasts-1.1.0/scripts/
--rw-rw-rw-   0        0        0        0 2023-03-11 02:56:42.000000 Windows-Toasts-1.1.0/scripts/__init__.py
--rw-rw-rw-   0        0        0     1622 2023-08-13 20:01:00.000000 Windows-Toasts-1.1.0/scripts/register_hkey_aumid.py
--rw-rw-rw-   0        0        0       42 2024-02-12 23:02:17.195196 Windows-Toasts-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1877 2024-01-30 14:02:30.000000 Windows-Toasts-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-12 23:02:16.858725 Windows-Toasts-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-12 23:02:17.106722 Windows-Toasts-1.1.0/src/windows_toasts/
--rw-rw-rw-   0        0        0     2117 2024-02-12 23:00:18.000000 Windows-Toasts-1.1.0/src/windows_toasts/__init__.py
--rw-rw-rw-   0        0        0      248 2024-02-12 23:01:23.000000 Windows-Toasts-1.1.0/src/windows_toasts/_version.py
--rw-rw-rw-   0        0        0     1307 2024-01-30 14:02:30.000000 Windows-Toasts-1.1.0/src/windows_toasts/events.py
--rw-rw-rw-   0        0        0      277 2024-02-12 23:00:18.000000 Windows-Toasts-1.1.0/src/windows_toasts/exceptions.py
--rw-rw-rw-   0        0        0        0 2022-02-26 17:24:59.000000 Windows-Toasts-1.1.0/src/windows_toasts/py.typed
--rw-rw-rw-   0        0        0     7774 2024-01-30 14:02:30.000000 Windows-Toasts-1.1.0/src/windows_toasts/toast.py
--rw-rw-rw-   0        0        0     1640 2023-03-17 22:03:36.000000 Windows-Toasts-1.1.0/src/windows_toasts/toast_audio.py
--rw-rw-rw-   0        0        0    15737 2024-01-30 14:02:30.000000 Windows-Toasts-1.1.0/src/windows_toasts/toast_document.py
--rw-rw-rw-   0        0        0    12063 2024-01-30 14:02:30.000000 Windows-Toasts-1.1.0/src/windows_toasts/toasters.py
--rw-rw-rw-   0        0        0     9062 2024-01-30 14:02:31.000000 Windows-Toasts-1.1.0/src/windows_toasts/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-02-12 23:02:17.192199 Windows-Toasts-1.1.0/tests/
--rw-rw-rw-   0        0        0     2680 2023-08-13 20:01:00.000000 Windows-Toasts-1.1.0/tests/test_aumid.py
--rw-rw-rw-   0        0        0      449 2024-02-12 23:00:18.000000 Windows-Toasts-1.1.0/tests/test_import.py
--rw-rw-rw-   0        0        0    10824 2024-02-12 23:00:18.000000 Windows-Toasts-1.1.0/tests/test_toasts.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:32:36.164857 windows_toasts-1.1.1/
+-rw-rw-rw-   0        0        0    11556 2022-02-19 10:55:53.000000 windows_toasts-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       69 2023-03-18 13:54:37.000000 windows_toasts-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3646 2024-05-19 11:32:36.163859 windows_toasts-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2407 2023-08-16 15:26:29.000000 windows_toasts-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 11:32:36.162857 windows_toasts-1.1.1/Windows_Toasts.egg-info/
+-rw-rw-rw-   0        0        0     3646 2024-05-19 11:32:35.000000 windows_toasts-1.1.1/Windows_Toasts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2024-05-19 11:32:36.000000 windows_toasts-1.1.1/Windows_Toasts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:32:35.000000 windows_toasts-1.1.1/Windows_Toasts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-19 11:32:35.000000 windows_toasts-1.1.1/Windows_Toasts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-24 23:36:24.000000 windows_toasts-1.1.1/Windows_Toasts.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      169 2024-05-19 11:32:35.000000 windows_toasts-1.1.1/Windows_Toasts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-19 11:32:35.000000 windows_toasts-1.1.1/Windows_Toasts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      362 2023-03-18 13:17:33.000000 windows_toasts-1.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-19 11:32:36.139748 windows_toasts-1.1.1/scripts/
+-rw-rw-rw-   0        0        0        0 2023-03-11 02:56:42.000000 windows_toasts-1.1.1/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1622 2023-08-13 20:01:00.000000 windows_toasts-1.1.1/scripts/register_hkey_aumid.py
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:32:36.164857 windows_toasts-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1867 2024-05-19 11:27:48.000000 windows_toasts-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:32:36.127725 windows_toasts-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 11:32:36.159858 windows_toasts-1.1.1/src/windows_toasts/
+-rw-rw-rw-   0        0        0     2117 2024-02-12 23:00:18.000000 windows_toasts-1.1.1/src/windows_toasts/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-05-19 11:28:39.000000 windows_toasts-1.1.1/src/windows_toasts/_version.py
+-rw-rw-rw-   0        0        0     1307 2024-05-19 10:21:34.000000 windows_toasts-1.1.1/src/windows_toasts/events.py
+-rw-rw-rw-   0        0        0      277 2024-02-12 23:00:18.000000 windows_toasts-1.1.1/src/windows_toasts/exceptions.py
+-rw-rw-rw-   0        0        0        0 2022-02-26 17:24:59.000000 windows_toasts-1.1.1/src/windows_toasts/py.typed
+-rw-rw-rw-   0        0        0     7985 2024-05-19 11:27:53.000000 windows_toasts-1.1.1/src/windows_toasts/toast.py
+-rw-rw-rw-   0        0        0     1640 2023-03-17 22:03:36.000000 windows_toasts-1.1.1/src/windows_toasts/toast_audio.py
+-rw-rw-rw-   0        0        0    15737 2024-01-30 14:02:30.000000 windows_toasts-1.1.1/src/windows_toasts/toast_document.py
+-rw-rw-rw-   0        0        0    12217 2024-05-19 11:27:53.000000 windows_toasts-1.1.1/src/windows_toasts/toasters.py
+-rw-rw-rw-   0        0        0     9062 2024-01-30 14:02:31.000000 windows_toasts-1.1.1/src/windows_toasts/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:32:36.161860 windows_toasts-1.1.1/tests/
+-rw-rw-rw-   0        0        0     2680 2023-08-13 20:01:00.000000 windows_toasts-1.1.1/tests/test_aumid.py
+-rw-rw-rw-   0        0        0      449 2024-02-12 23:00:18.000000 windows_toasts-1.1.1/tests/test_import.py
+-rw-rw-rw-   0        0        0    10620 2024-05-19 11:27:53.000000 windows_toasts-1.1.1/tests/test_toasts.py
```

### Comparing `Windows-Toasts-1.1.0/LICENSE` & `windows_toasts-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/PKG-INFO` & `windows_toasts-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Windows-Toasts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library used to send toast notifications on Windows machines
 Home-page: https://github.com/DatGuy1/Windows-Toasts
 Author: DatGuy
 Author-email: datguysteam@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://windows-toasts.readthedocs.io
 Project-URL: Source, https://github.com/DatGuy1/Windows-Toasts
@@ -16,19 +16,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: winrt-runtime<=2.0.0b2
-Requires-Dist: winrt-Windows.Data.Xml.Dom<=2.0.0b2
-Requires-Dist: winrt-Windows.Foundation<=2.0.0b2
-Requires-Dist: winrt-Windows.Foundation.Collections<=2.0.0b2
-Requires-Dist: winrt-Windows.UI.Notifications<=2.0.0b2
+Requires-Dist: winrt-runtime<=2.0.1
+Requires-Dist: winrt-Windows.Data.Xml.Dom<=2.0.1
+Requires-Dist: winrt-Windows.Foundation<=2.0.1
+Requires-Dist: winrt-Windows.Foundation.Collections<=2.0.1
+Requires-Dist: winrt-Windows.UI.Notifications<=2.0.1
 
 # Windows-Toasts 
 
 ---
 [![PyPI version](https://img.shields.io/pypi/v/windows-toasts)](https://pypi.org/project/windows-toasts/) [![readthedocs.io](https://readthedocs.org/projects/windows-toasts/badge/?version=latest)](https://windows-toasts.readthedocs.io/en/latest/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/windows-toasts)](https://pypi.org/project/windows-toasts/) [![Downloads](https://static.pepy.tech/badge/windows-toasts/month)](https://pepy.tech/project/windows-toasts) [![codecov](https://codecov.io/gh/DatGuy1/Windows-Toasts/branch/master/graph/badge.svg?token=ZD8OF2SF61)](https://codecov.io/gh/DatGuy1/Windows-Toasts) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **Windows-Toasts** is a Python library used to send [toast notifications](https://docs.microsoft.com/windows/apps/design/shell/tiles-and-notifications/adaptive-interactive-toasts) on Windows machines. Check out the [documentation](https://windows-toasts.readthedocs.io/en/latest/).
```

### Comparing `Windows-Toasts-1.1.0/README.md` & `windows_toasts-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/Windows_Toasts.egg-info/PKG-INFO` & `windows_toasts-1.1.1/Windows_Toasts.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Windows-Toasts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library used to send toast notifications on Windows machines
 Home-page: https://github.com/DatGuy1/Windows-Toasts
 Author: DatGuy
 Author-email: datguysteam@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://windows-toasts.readthedocs.io
 Project-URL: Source, https://github.com/DatGuy1/Windows-Toasts
@@ -16,19 +16,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: winrt-runtime<=2.0.0b2
-Requires-Dist: winrt-Windows.Data.Xml.Dom<=2.0.0b2
-Requires-Dist: winrt-Windows.Foundation<=2.0.0b2
-Requires-Dist: winrt-Windows.Foundation.Collections<=2.0.0b2
-Requires-Dist: winrt-Windows.UI.Notifications<=2.0.0b2
+Requires-Dist: winrt-runtime<=2.0.1
+Requires-Dist: winrt-Windows.Data.Xml.Dom<=2.0.1
+Requires-Dist: winrt-Windows.Foundation<=2.0.1
+Requires-Dist: winrt-Windows.Foundation.Collections<=2.0.1
+Requires-Dist: winrt-Windows.UI.Notifications<=2.0.1
 
 # Windows-Toasts 
 
 ---
 [![PyPI version](https://img.shields.io/pypi/v/windows-toasts)](https://pypi.org/project/windows-toasts/) [![readthedocs.io](https://readthedocs.org/projects/windows-toasts/badge/?version=latest)](https://windows-toasts.readthedocs.io/en/latest/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/windows-toasts)](https://pypi.org/project/windows-toasts/) [![Downloads](https://static.pepy.tech/badge/windows-toasts/month)](https://pepy.tech/project/windows-toasts) [![codecov](https://codecov.io/gh/DatGuy1/Windows-Toasts/branch/master/graph/badge.svg?token=ZD8OF2SF61)](https://codecov.io/gh/DatGuy1/Windows-Toasts) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **Windows-Toasts** is a Python library used to send [toast notifications](https://docs.microsoft.com/windows/apps/design/shell/tiles-and-notifications/adaptive-interactive-toasts) on Windows machines. Check out the [documentation](https://windows-toasts.readthedocs.io/en/latest/).
```

### Comparing `Windows-Toasts-1.1.0/Windows_Toasts.egg-info/SOURCES.txt` & `windows_toasts-1.1.1/Windows_Toasts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/scripts/register_hkey_aumid.py` & `windows_toasts-1.1.1/scripts/register_hkey_aumid.py`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/setup.py` & `windows_toasts-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 packages = ["windows_toasts", "scripts"]
 
 requires = [
-    "winrt-runtime<=2.0.0b2",
-    "winrt-Windows.Data.Xml.Dom<=2.0.0b2",
-    "winrt-Windows.Foundation<=2.0.0b2",
-    "winrt-Windows.Foundation.Collections<=2.0.0b2",
-    "winrt-Windows.UI.Notifications<=2.0.0b2",
+    "winrt-runtime<=2.0.1",
+    "winrt-Windows.Data.Xml.Dom<=2.0.1",
+    "winrt-Windows.Foundation<=2.0.1",
+    "winrt-Windows.Foundation.Collections<=2.0.1",
+    "winrt-Windows.UI.Notifications<=2.0.1",
 ]
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 about = {}
 with open("src/windows_toasts/_version.py", "r") as f:
```

### Comparing `Windows-Toasts-1.1.0/src/windows_toasts/__init__.py` & `windows_toasts-1.1.1/src/windows_toasts/__init__.py`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/src/windows_toasts/events.py` & `windows_toasts-1.1.1/src/windows_toasts/events.py`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/src/windows_toasts/toast.py` & `windows_toasts-1.1.1/src/windows_toasts/toast.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     """Scenario for the toast"""
     suppress_popup: bool
     """Whether to suppress the toast popup and relegate it immediately to the action center"""
     timestamp: Optional[datetime.datetime]
     """A custom timestamp. If you don't provide one, Windows uses the time that your notification was sent"""
     progress_bar: Optional[ToastProgressBar]
     """An adjustable progress bar for the toast"""
+    attribution_text: Optional[str]
+    """Text displayed below any text elements, but above inline images"""
     on_activated: Optional[Callable[[ToastActivatedEventArgs], None]]
     """Callable to execute when the toast is clicked if basic, or a button is clicked if interactable"""
     on_dismissed: Optional[Callable[[ToastDismissedEventArgs], None]]
     """Callable to execute when the toast is dismissed (X is clicked or times out) if interactable"""
     on_failed: Optional[Callable[[ToastFailedEventArgs], None]]
     """Callable to execute when the toast fails to display"""
     actions: list[Union[ToastButton, ToastSystemButton]]
@@ -69,14 +71,15 @@
         text_fields: Union[list[Optional[str]], tuple[Optional[str]], set[Optional[str]]] = None,
         audio: Optional[ToastAudio] = None,
         duration: ToastDuration = ToastDuration.Default,
         expiration_time: Optional[datetime.datetime] = None,
         group: Optional[str] = None,
         launch_action: Optional[str] = None,
         progress_bar: Optional[ToastProgressBar] = None,
+        attribution_text: Optional[str] = None,
         scenario: ToastScenario = ToastScenario.Default,
         suppress_popup: bool = False,
         timestamp: Optional[datetime.datetime] = None,
         on_activated: Optional[Callable[[ToastActivatedEventArgs], None]] = None,
         on_dismissed: Optional[Callable[[ToastDismissedEventArgs], None]] = None,
         on_failed: Optional[Callable[[ToastFailedEventArgs], None]] = None,
         actions: Iterable[Union[ToastButton, ToastSystemButton]] = (),
@@ -93,14 +96,15 @@
         :param inputs: See :meth:`AddInput`
         :type inputs: Iterable[ToastInput]
         """
         self.audio = audio
         self.duration = duration
         self.scenario = scenario
         self.progress_bar = progress_bar
+        self.attribution_text = attribution_text
         self.timestamp = timestamp
         self.group = group
         self.expiration_time = expiration_time
         self.suppress_popup = suppress_popup
         self.launch_action = launch_action
 
         self.actions = []
```

### Comparing `Windows-Toasts-1.1.0/src/windows_toasts/toast_audio.py` & `windows_toasts-1.1.1/src/windows_toasts/toast_audio.py`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/src/windows_toasts/toast_document.py` & `windows_toasts-1.1.1/src/windows_toasts/toast_document.py`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/src/windows_toasts/toasters.py` & `windows_toasts-1.1.1/src/windows_toasts/toasters.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,17 @@
 
         if toast.timestamp is not None:
             toastContent.SetCustomTimestamp(toast.timestamp)
 
         if toast.audio is not None:
             toastContent.SetAudioAttributes(toast.audio)
 
+        if toast.attribution_text is not None:
+            toastContent.SetAttributionText(toast.attribution_text)
+
         if toast.scenario != ToastScenario.Default:
             toastContent.SetScenario(toast.scenario)
 
         if toast.launch_action is not None:
             toastContent.SetAttribute(toastContent.GetElementByTagName("toast"), "launch", toast.launch_action)
             toastContent.SetAttribute(toastContent.GetElementByTagName("toast"), "activationType", "protocol")
         else:
@@ -292,15 +295,15 @@
                 toastContent.SetTextFieldStatic(i, fieldContent)
 
         toastContent.SetAttribute(toastContent.bindingNode, "template", "ToastGeneric")
         toastNode = toastContent.GetElementByTagName("toast")
         toastContent.SetAttribute(toastNode, "useButtonStyle", "true")
 
         # If we haven't set up our own AUMID, put our application text in the attribution field
-        if self.defaultAUMID:
+        if self.defaultAUMID and toast.attribution_text is None:
             toastContent.SetAttributionText(self.applicationText)
 
         for toastInput in toast.inputs:
             toastContent.AddInput(toastInput)
 
         for customAction in toast.actions:
             toastContent.AddAction(customAction)
```

### Comparing `Windows-Toasts-1.1.0/src/windows_toasts/wrappers.py` & `windows_toasts-1.1.1/src/windows_toasts/wrappers.py`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/tests/test_aumid.py` & `windows_toasts-1.1.1/tests/test_aumid.py`

 * *Files identical despite different names*

### Comparing `Windows-Toasts-1.1.0/tests/test_toasts.py` & `windows_toasts-1.1.1/tests/test_toasts.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,24 +178,18 @@
     from src.windows_toasts import ToastDuration
 
     newToast = Toast(["A short toast"], duration=ToastDuration.Short)
     WindowsToaster("Python").show_toast(newToast)
 
 
 def test_attribution_text_toast():
-    from winrt.windows.ui.notifications import ToastNotification
+    newToast = Toast(["Incoming Message", "How are you?"])
+    newToast.attribution_text = "Via FakeMessenger"
 
-    newToast = Toast()
-    newToast.text_fields = ["Hello, World!", "Foobar"]
-
-    toaster = WindowsToaster("Python")
-    toastContent = toaster._setup_toast(newToast, False)
-    toastContent.SetAttributionText("Windows-Toasts")
-
-    toaster.toastNotifier.show(ToastNotification(toastContent.xmlDocument))
+    InteractableWindowsToaster("Python").show_toast(newToast)
 
 
 def test_scenario_toast():
     from src.windows_toasts import ToastScenario
 
     newToast = Toast(["Very important toast!", "Are you ready?", "Here it comes!"])
     newToast.scenario = ToastScenario.Important
```

