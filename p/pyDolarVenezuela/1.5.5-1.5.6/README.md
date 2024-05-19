# Comparing `tmp/pydolarvenezuela-1.5.5.tar.gz` & `tmp/pydolarvenezuela-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.5.5.tar", last modified: Wed May  8 05:25:45 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.5.6.tar", last modified: Sun May 19 06:52:15 2024, max compression
```

## Comparing `pydolarvenezuela-1.5.5.tar` & `pydolarvenezuela-1.5.6.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.118536 pydolarvenezuela-1.5.5/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.5/LICENSE
--rw-rw-rw-   0        0        0     7221 2024-05-08 05:25:45.110580 pydolarvenezuela-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     4830 2024-05-08 05:23:24.000000 pydolarvenezuela-1.5.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 05:25:44.915627 pydolarvenezuela-1.5.5/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2879 2024-05-08 05:22:33.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:25:44.950502 pydolarvenezuela-1.5.5/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:25:44.950502 pydolarvenezuela-1.5.5/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/assets/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:25:44.998987 pydolarvenezuela-1.5.5/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.032525 pydolarvenezuela-1.5.5/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.082019 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     5345 2024-05-08 05:21:26.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2141 2024-04-28 15:44:15.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     1762 2024-04-29 16:09:28.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     2382 2024-05-04 07:56:14.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     1282 2024-05-04 08:02:51.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/italcambio.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.102583 pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     2236 2024-04-28 11:49:26.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.107586 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7221 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      897 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-05-08 05:22:42.000000 pydolarvenezuela-1.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 05:25:45.121532 pydolarvenezuela-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-05-08 05:22:38.000000 pydolarvenezuela-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 06:52:15.867858 pydolarvenezuela-1.5.6/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0     7221 2024-05-19 06:52:15.864869 pydolarvenezuela-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4830 2024-05-08 05:23:24.000000 pydolarvenezuela-1.5.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 06:52:15.754849 pydolarvenezuela-1.5.6/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2879 2024-05-19 06:51:29.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 06:52:15.793854 pydolarvenezuela-1.5.6/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-05-19 06:52:15.817853 pydolarvenezuela-1.5.6/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/models/images.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-05-19 06:52:15.838856 pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     5345 2024-05-19 04:56:54.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2328 2024-05-19 06:17:16.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2081 2024-05-19 06:50:07.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2627 2024-05-19 05:56:01.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1282 2024-05-04 08:02:51.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-05-19 06:52:15.854856 pydolarvenezuela-1.5.6/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0    12380 2024-05-19 06:16:03.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 06:52:15.859859 pydolarvenezuela-1.5.6/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7221 2024-05-19 06:52:15.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2024-05-19 06:52:15.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 06:52:15.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-19 06:52:15.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 06:52:15.000000 pydolarvenezuela-1.5.6/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-05-19 06:51:40.000000 pydolarvenezuela-1.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 06:52:15.868860 pydolarvenezuela-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-05-19 06:51:43.000000 pydolarvenezuela-1.5.6/setup.py
```

### Comparing `pydolarvenezuela-1.5.5/LICENSE` & `pydolarvenezuela-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.5/PKG-INFO` & `pydolarvenezuela-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.5
+Version: 1.5.6
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.5.5/README.md` & `pydolarvenezuela-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import network
 from .models.pages import Page
 from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-version = '1.5.5'
+version = '1.5.6'
 """
 Versión actual de la biblioteca    
 """
 
 class CheckVersion:
     """
     Verificar actualización de la biblioteca
```

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/bcv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bs4 import BeautifulSoup
 
 from ..network import requests, get
-from ..utils import currencies
+from ..utils import currencies, list_monitors_images
 
 requests.packages.urllib3.disable_warnings()
 
 def _get_rate_by_id(tag_id: str, soup: BeautifulSoup):
     return float(soup.find(id=tag_id).find("strong").text.strip().replace(',', '.'))
 
 def _get_time(soup: BeautifulSoup):
@@ -36,16 +36,18 @@
                     'last_update': str(bank.find('td', 'views-field views-field-field-fecha-del-indicador').text).strip().replace('-', '/')
                 })
             self.rates['banks'] = banks
         
         self.rates['last_update'] = _get_time(section_tipo_de_cambio_oficial)
 
         for code, values in currencies.items():
+            image = next((image.image for image in list_monitors_images if image.provider == 'bcv' and image.title == code), None)
             self.rates[code] = {
                 "title": values['name'],
                 "price": round(_get_rate_by_id(values['id'], section_tipo_de_cambio_oficial), 2),
-                "price_old": _get_rate_by_id(values['id'], section_tipo_de_cambio_oficial)
+                "price_old": _get_rate_by_id(values['id'], section_tipo_de_cambio_oficial),
+                "image": image
             }
 
     def get_values(self):
         self._load()
         return self.rates
```

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/criptodolar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from .. import network
 from ..tools import time
+from ..utils import list_monitors_images
 
 def _convert_specific_format(text: str, character: str = '_') -> str:
     acentos = {'á': 'a', 'é': 'e', 'í': 'i', 'ó': 'o', 'ú': 'u'}
     for acento, sin_acento in acentos.items():
         text = text.lower().replace(acento, sin_acento).replace(' ', character)
     return text
 
@@ -24,19 +25,22 @@
         self.currency = currency
     
     def _load(self):
         self.data = {}
 
         for monitor in self.json_response:
             if monitor['type'] in ['bolivar', 'bancove']:
+                image = next((image.image for image in list_monitors_images if image.provider == 'criptodolar' and image.title == _convert_specific_format(
+                    _convert_dollar_name_to_monitor_name(monitor['name']))), None)
                 data = {
                     'title': _convert_dollar_name_to_monitor_name(monitor['name']),
                     'price': round(monitor['price'], 2),
                     'price_old': monitor['priceOld'],
                     'last_update': time.get_time_standard(monitor['updatedAt']),
+                    'image': image
                 }
 
                 self.data[_convert_specific_format(data['title'])] = data
     
     def get_values(self):
         self._load()
         return self.data
```

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from bs4 import BeautifulSoup
 from .. import network
 from ..tools import time
+from ..utils import list_monitors_images
 
 def _convert_specific_format(text: str, character: str = '_') -> str:
     acentos = {'á': 'a', 'é': 'e', 'í': 'i', 'ó': 'o', 'ú': 'u'}
     for acento, sin_acento in acentos.items():
         text = text.lower().replace(acento, sin_acento).replace(' ', character)
     return text
 
@@ -33,23 +34,25 @@
 
             price = float(price)
             last_update = time.get_formatted_time(' '.join(str(result.find('p', "fecha").text).split(' ')[1:]).capitalize())
             symbol = str(result.find('p', "cambio-por").text)[0] if not str(result.find('p', "cambio-por").text)[0] == ' ' else ''
             color  = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
             percent = float(str(result.find('p', "cambio-por").text)[1:].strip().replace(',', '.').replace('%', ''))
             change = float(str(result.find('p', "cambio-num").text).replace(',', '.'))
+            image = next((image.image for image in list_monitors_images if image.provider == 'exchangemonitor' and image.title == _convert_specific_format(name)), None)
 
             data = {
                 'title': name,
                 'price': price,
                 'last_update': last_update,
                 'percent': percent,
                 'change': change,
                 'color': color,
-                'symbol': symbol
+                'symbol': symbol,
+                'image': image
             }
 
             self.data[_convert_specific_format(name)] = data
     
     def get_values(self):
         self._load()
         return self.data
```

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/italcambio.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/provider/italcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.5.6/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.5.6/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.5
+Version: 1.5.6
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.5.6/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 pyDolarVenezuela/pages.py
 pyDolarVenezuela/utils.py
 pyDolarVenezuela.egg-info/PKG-INFO
 pyDolarVenezuela.egg-info/SOURCES.txt
 pyDolarVenezuela.egg-info/dependency_links.txt
 pyDolarVenezuela.egg-info/requires.txt
 pyDolarVenezuela.egg-info/top_level.txt
-pyDolarVenezuela/assets/__init__.py
-pyDolarVenezuela/assets/icons/__init__.py
 pyDolarVenezuela/data/__init__.py
 pyDolarVenezuela/data/redis.py
 pyDolarVenezuela/models/__init__.py
 pyDolarVenezuela/models/database.py
+pyDolarVenezuela/models/images.py
 pyDolarVenezuela/models/pages.py
 pyDolarVenezuela/provider/__init__.py
 pyDolarVenezuela/provider/bcv.py
 pyDolarVenezuela/provider/criptodolar.py
 pyDolarVenezuela/provider/exchangemonitor.py
 pyDolarVenezuela/provider/italcambio.py
 pyDolarVenezuela/tools/__init__.py
```

### Comparing `pydolarvenezuela-1.5.5/pyproject.toml` & `pydolarvenezuela-1.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.5.5"
+version = "1.5.6"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.5.5/setup.py` & `pydolarvenezuela-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.5.5'
+VERSION = '1.5.6'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

