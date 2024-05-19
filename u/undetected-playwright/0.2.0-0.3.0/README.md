# Comparing `tmp/undetected_playwright-0.2.0.tar.gz` & `tmp/undetected_playwright-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undetected_playwright-0.2.0.tar", max compression
+gzip compressed data, was "undetected_playwright-0.3.0.tar", max compression
```

## Comparing `undetected_playwright-0.2.0.tar` & `undetected_playwright-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0    11558 2022-10-24 04:51:51.125169 undetected_playwright-0.2.0/LICENSE
--rw-r--r--   0        0        0     1417 2023-08-24 12:40:15.749728 undetected_playwright-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1373 2022-10-24 08:12:45.471968 undetected_playwright-0.2.0/README.md
--rw-r--r--   0        0        0      259 2023-08-24 12:37:45.643266 undetected_playwright-0.2.0/undetected_playwright/__init__.py
--rw-r--r--   0        0        0     1421 2023-08-24 12:37:45.618498 undetected_playwright-0.2.0/undetected_playwright/ninja.py
--rw-r--r--   0        0        0      619 2023-08-20 17:25:47.319637 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_template/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.319637 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_template/package.json
--rw-r--r--   0        0        0    22272 2023-08-20 17:25:47.320635 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_utils/index.js
--rw-r--r--   0        0        0     1706 2023-08-20 17:25:47.321635 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_utils/withUtils.js
--rw-r--r--   0        0        0     2720 2023-08-20 17:25:47.321635 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.app/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.322662 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.app/package.json
--rw-r--r--   0        0        0     2536 2023-08-20 17:25:47.323664 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.csi/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.323664 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.csi/package.json
--rw-r--r--   0        0        0     6164 2023-08-20 17:25:47.324763 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.loadTimes/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.325773 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.loadTimes/package.json
--rw-r--r--   0        0        0     9669 2023-08-20 17:25:47.326776 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.326776 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/package.json
--rw-r--r--   0        0        0      924 2023-08-20 17:25:47.327788 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/staticData.json
--rw-r--r--   0        0        0     1262 2023-08-20 17:25:47.328787 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/defaultArgs/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.328787 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/defaultArgs/package.json
--rw-r--r--   0        0        0     4679 2023-08-20 17:25:47.329790 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/iframe.contentWindow/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.330802 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/iframe.contentWindow/package.json
--rw-r--r--   0        0        0     2621 2023-08-20 17:25:47.331779 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/media.codecs/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.332776 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/media.codecs/package.json
--rw-r--r--   0        0        0     1213 2023-08-20 17:25:47.332776 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.hardwareConcurrency/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.334299 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.hardwareConcurrency/package.json
--rw-r--r--   0        0        0     1229 2023-08-20 17:25:47.334299 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.languages/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.335315 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.languages/package.json
--rw-r--r--   0        0        0     1994 2023-08-20 17:25:47.336336 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.permissions/index.js
--rw-r--r--   0        0        0       46 2023-08-20 17:25:47.336336 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.permissions/package.json
--rw-r--r--   0        0        0     1274 2023-08-20 17:25:47.337323 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/data.json
--rw-r--r--   0        0        0     1845 2023-08-20 17:25:47.337323 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/functionMocks.js
--rw-r--r--   0        0        0     3630 2023-08-20 17:25:47.338309 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/index.js
--rw-r--r--   0        0        0     5669 2023-08-20 17:25:47.339319 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/magicArray.js
--rw-r--r--   0        0        0      579 2023-08-20 17:25:47.340332 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/mimeTypes.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.340332 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/package.json
--rw-r--r--   0        0        0      556 2023-08-20 17:25:47.341323 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/plugins.js
--rw-r--r--   0        0        0     1823 2023-08-20 17:25:47.342323 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.vendor/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.342323 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.vendor/package.json
--rw-r--r--   0        0        0     1629 2023-08-20 17:25:47.343335 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.webdriver/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.343335 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.webdriver/package.json
--rw-r--r--   0        0        0      967 2023-08-20 17:25:47.344335 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/_fixtures/test.html
--rw-r--r--   0        0        0     2703 2023-08-20 17:25:47.345315 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.346511 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/package.json
--rw-r--r--   0        0        0     7050 2023-08-20 17:25:47.347514 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/user-agent-override/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.347514 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/user-agent-override/package.json
--rw-r--r--   0        0        0     2248 2023-08-20 17:25:47.348513 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/webgl.vendor/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.349514 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/webgl.vendor/package.json
--rw-r--r--   0        0        0     1237 2023-08-20 17:25:47.350515 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/window.outerdimensions/index.js
--rw-r--r--   0        0        0       48 2023-08-20 17:25:47.350515 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/window.outerdimensions/package.json
--rw-r--r--   0        0        0     1118 2023-08-20 17:25:47.318637 undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/LICENSE
--rw-r--r--   0        0        0     2555 1970-01-01 00:00:00.000000 undetected_playwright-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2022-10-24 04:51:51.125169 undetected_playwright-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1417 2024-05-19 02:08:58.179619 undetected_playwright-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5920 2024-05-19 02:08:58.173614 undetected_playwright-0.3.0/README.md
+-rw-r--r--   0        0        0      326 2024-05-19 02:08:58.181619 undetected_playwright-0.3.0/undetected_playwright/__init__.py
+-rw-r--r--   0        0        0     1421 2023-08-24 12:37:45.618498 undetected_playwright-0.3.0/undetected_playwright/ninja.py
+-rw-r--r--   0        0        0      619 2023-08-20 17:25:47.319637 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_template/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.319637 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_template/package.json
+-rw-r--r--   0        0        0    22272 2023-08-20 17:25:47.320635 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_utils/index.js
+-rw-r--r--   0        0        0     1706 2023-08-20 17:25:47.321635 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_utils/withUtils.js
+-rw-r--r--   0        0        0     2720 2023-08-20 17:25:47.321635 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.app/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.322662 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.app/package.json
+-rw-r--r--   0        0        0     2536 2023-08-20 17:25:47.323664 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.csi/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.323664 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.csi/package.json
+-rw-r--r--   0        0        0     6164 2023-08-20 17:25:47.324763 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.loadTimes/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.325773 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.loadTimes/package.json
+-rw-r--r--   0        0        0     9669 2023-08-20 17:25:47.326776 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.326776 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/package.json
+-rw-r--r--   0        0        0      924 2023-08-20 17:25:47.327788 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/staticData.json
+-rw-r--r--   0        0        0     1262 2023-08-20 17:25:47.328787 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/defaultArgs/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.328787 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/defaultArgs/package.json
+-rw-r--r--   0        0        0     4679 2023-08-20 17:25:47.329790 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/iframe.contentWindow/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.330802 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/iframe.contentWindow/package.json
+-rw-r--r--   0        0        0     2621 2023-08-20 17:25:47.331779 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/media.codecs/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.332776 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/media.codecs/package.json
+-rw-r--r--   0        0        0     1213 2023-08-20 17:25:47.332776 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.hardwareConcurrency/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.334299 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.hardwareConcurrency/package.json
+-rw-r--r--   0        0        0     1229 2023-08-20 17:25:47.334299 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.languages/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.335315 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.languages/package.json
+-rw-r--r--   0        0        0     1994 2023-08-20 17:25:47.336336 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.permissions/index.js
+-rw-r--r--   0        0        0       46 2023-08-20 17:25:47.336336 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.permissions/package.json
+-rw-r--r--   0        0        0     1274 2023-08-20 17:25:47.337323 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/data.json
+-rw-r--r--   0        0        0     1845 2023-08-20 17:25:47.337323 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/functionMocks.js
+-rw-r--r--   0        0        0     3630 2023-08-20 17:25:47.338309 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/index.js
+-rw-r--r--   0        0        0     5669 2023-08-20 17:25:47.339319 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/magicArray.js
+-rw-r--r--   0        0        0      579 2023-08-20 17:25:47.340332 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/mimeTypes.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.340332 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/package.json
+-rw-r--r--   0        0        0      556 2023-08-20 17:25:47.341323 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/plugins.js
+-rw-r--r--   0        0        0     1823 2023-08-20 17:25:47.342323 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.vendor/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.342323 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.vendor/package.json
+-rw-r--r--   0        0        0     1629 2023-08-20 17:25:47.343335 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.webdriver/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.343335 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.webdriver/package.json
+-rw-r--r--   0        0        0      967 2023-08-20 17:25:47.344335 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/_fixtures/test.html
+-rw-r--r--   0        0        0     2703 2023-08-20 17:25:47.345315 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.346511 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/package.json
+-rw-r--r--   0        0        0     7050 2023-08-20 17:25:47.347514 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/user-agent-override/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.347514 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/user-agent-override/package.json
+-rw-r--r--   0        0        0     2248 2023-08-20 17:25:47.348513 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/webgl.vendor/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.349514 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/webgl.vendor/package.json
+-rw-r--r--   0        0        0     1237 2023-08-20 17:25:47.350515 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/window.outerdimensions/index.js
+-rw-r--r--   0        0        0       48 2023-08-20 17:25:47.350515 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/window.outerdimensions/package.json
+-rw-r--r--   0        0        0     1118 2023-08-20 17:25:47.318637 undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/LICENSE
+-rw-r--r--   0        0        0     5412 2024-05-19 02:08:58.182621 undetected_playwright-0.3.0/undetected_playwright/tarnished.py
+-rw-r--r--   0        0        0     6977 1970-01-01 00:00:00.000000 undetected_playwright-0.3.0/PKG-INFO
```

### Comparing `undetected_playwright-0.2.0/LICENSE` & `undetected_playwright-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/pyproject.toml` & `undetected_playwright-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://python-poetry.org/docs/libraries/#versioning
 
 [tool.poetry]
 name = "undetected-playwright"
-version = "0.2.0"
+version = "0.3.0"
 description = "You know who I am"
 license = "Apache-2.0"
 authors = ["QIN2DIM <yaoqinse@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/QIN2DIM/undetected-playwright"
 repository = "https://github.com/QIN2DIM/undetected-playwright"
 documentation = "https://github.com/QIN2DIM/undetected-playwright"
```

### Comparing `undetected_playwright-0.2.0/undetected_playwright/ninja.py` & `undetected_playwright-0.3.0/undetected_playwright/ninja.py`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_template/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_template/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_utils/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_utils/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_utils/withUtils.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/_utils/withUtils.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.app/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.app/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.csi/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.csi/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.loadTimes/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.loadTimes/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/staticData.json` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/chrome.runtime/staticData.json`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/defaultArgs/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/defaultArgs/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/iframe.contentWindow/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/iframe.contentWindow/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/media.codecs/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/media.codecs/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.hardwareConcurrency/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.hardwareConcurrency/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.languages/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.languages/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.permissions/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.permissions/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/data.json` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/data.json`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/functionMocks.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/functionMocks.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/magicArray.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/magicArray.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/mimeTypes.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/mimeTypes.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/plugins.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.plugins/plugins.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.vendor/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.vendor/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.webdriver/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/navigator.webdriver/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/_fixtures/test.html` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/_fixtures/test.html`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/sourceurl/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/user-agent-override/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/user-agent-override/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/webgl.vendor/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/webgl.vendor/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/window.outerdimensions/index.js` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/evasions/window.outerdimensions/index.js`

 * *Files identical despite different names*

### Comparing `undetected_playwright-0.2.0/undetected_playwright/puppeteer-extra-plugin-stealth/LICENSE` & `undetected_playwright-0.3.0/undetected_playwright/puppeteer-extra-plugin-stealth/LICENSE`

 * *Files identical despite different names*

