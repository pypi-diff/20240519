# Comparing `tmp/pyqn-1.3.2.tar.gz` & `tmp/pyqn-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqn-1.3.2.tar", last modified: Mon Aug  1 10:51:43 2022, max compression
+gzip compressed data, was "pyqn-1.4.tar", last modified: Mon Apr 22 12:05:48 2024, max compression
```

## Comparing `pyqn-1.3.2.tar` & `pyqn-1.4.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 10:51:43.827831 pyqn-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-08-01 10:51:24.000000 pyqn-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-08-01 10:51:43.827831 pyqn-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-01 10:51:24.000000 pyqn-1.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-01 10:51:24.000000 pyqn-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-08-01 10:51:43.827831 pyqn-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-08-01 10:51:24.000000 pyqn-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 10:51:43.823831 pyqn-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 10:51:43.823831 pyqn-1.3.2/src/pyqn/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5100 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/atom_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)    12372 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/base_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/list_base_units.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/qn_array.py
--rw-r--r--   0 runner    (1001) docker     (121)    11494 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/quantity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/si.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)    12163 2022-08-01 10:51:24.000000 pyqn-1.3.2/src/pyqn/units.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 10:51:43.827831 pyqn-1.3.2/src/pyqn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-08-01 10:51:43.000000 pyqn-1.3.2/src/pyqn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-08-01 10:51:43.000000 pyqn-1.3.2/src/pyqn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 10:51:43.000000 pyqn-1.3.2/src/pyqn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-01 10:51:43.000000 pyqn-1.3.2/src/pyqn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-01 10:51:43.000000 pyqn-1.3.2/src/pyqn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:05:48.875368 pyqn-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-22 12:05:38.000000 pyqn-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-22 12:05:48.875368 pyqn-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-22 12:05:38.000000 pyqn-1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 12:05:38.000000 pyqn-1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 12:05:48.875368 pyqn-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-22 12:05:38.000000 pyqn-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:05:48.871368 pyqn-1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:05:48.871368 pyqn-1.4/src/pyqn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/atom_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/base_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/list_base_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/qn_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11494 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/si.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-22 12:05:38.000000 pyqn-1.4/src/pyqn/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:05:48.875368 pyqn-1.4/src/pyqn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-22 12:05:48.000000 pyqn-1.4/src/pyqn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-22 12:05:48.000000 pyqn-1.4/src/pyqn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:05:48.000000 pyqn-1.4/src/pyqn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 12:05:48.000000 pyqn-1.4/src/pyqn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 12:05:48.000000 pyqn-1.4/src/pyqn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:05:48.875368 pyqn-1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-22 12:05:38.000000 pyqn-1.4/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-22 12:05:38.000000 pyqn-1.4/tests/test_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-22 12:05:38.000000 pyqn-1.4/tests/test_undef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-22 12:05:38.000000 pyqn-1.4/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-22 12:05:38.000000 pyqn-1.4/tests/test_units_collisions.py
```

### Comparing `pyqn-1.3.2/LICENSE` & `pyqn-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqn-1.3.2/PKG-INFO` & `pyqn-1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqn
-Version: 1.3.2
+Version: 1.4
 Summary: A package for managing physical units and quantities
 Home-page: https://github.com/xnx/pyqn
 Author: Christian Hill
 Author-email: xn.hill@gmail.com
 Project-URL: Bug Reports, https://github.com/xnx/pyqn/issues
 Keywords: chemistry,units,physical quantities,unit conversion
 Classifier: Development Status :: 4 - Beta
@@ -14,20 +14,28 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyparsing>=2.3
+Requires-Dist: importlib-resources>=1.0; python_version < "3.7.0"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: ipython; extra == "dev"
 
 ********************
 Introduction to PyQn
 ********************
```

### Comparing `pyqn-1.3.2/setup.py` & `pyqn-1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 root = Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (root / "README.rst").read_text(encoding="utf-8")
 
 setup(
     name="pyqn",
-    version="1.3.2",
+    version="1.4",
     description="A package for managing physical units and quantities",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/xnx/pyqn",
     author="Christian Hill",
     author_email="xn.hill@gmail.com",
     classifiers=[
@@ -23,14 +23,16 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Operating System :: OS Independent",
     ],
     keywords="chemistry, units, physical quantities, unit conversion",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.6",
```

### Comparing `pyqn-1.3.2/src/pyqn/atom_unit.py` & `pyqn-1.4/src/pyqn/atom_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,31 +19,33 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with PyQn.  If not, see <http://www.gnu.org/licenses/>
 
 import sys
+from fractions import Fraction
 from pyparsing import Word, Group, Literal, Suppress, ParseException, oneOf, Optional
 from .si import si_prefixes
 from .base_unit import BaseUnit, base_unit_stems
 from .dimensions import Dimensions
 
 # pyparsing stuff for parsing unit strings:
 caps = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 lowers = caps.lower()
 letters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz_0"
 digits = "123456789"
-exponent = Word(digits + "-")
+exponent = Word(digits + "-/")
 prefix = oneOf(list(si_prefixes.keys()))
 ustem = Word(letters + "Å" + "Ω")
 uatom = (Group("1" | (Optional(prefix) + ustem)) + Optional(exponent)) | (
     Group("1" | ustem) + Optional(exponent)
 )
 
+
 # floating point equality and its negation, to some suitable tolerance
 def feq(f1, f2, tol=1.0e-10):
     return abs(f1 - f2) <= tol
 
 
 def fneq(f1, f2, tol=1.0e-10):
     return not feq(f1, f2, tol)
@@ -121,15 +123,18 @@
             base_unit = base_unit_stems[stem]
         except:
             raise UnitsError("Unrecognised unit: %s" % s_unit_atom)
 
         # if there is an exponent, determine what it is (default is 1)
         exponent = 1
         if len(uatom_data) == 2:
-            exponent = int(uatom_data[1])
+            if "/" in uatom_data:
+                exponent = int(uatom_data[1])
+            else:
+                exponent = Fraction(uatom_data[1])
         return AtomUnit(prefix, base_unit, exponent)
 
     def __pow__(self, power):
         """Return the current AtomUnit raised to a specified power."""
         return AtomUnit(self.prefix, self.base_unit, self.exponent * power)
 
     def __str__(self):
```

### Comparing `pyqn-1.3.2/src/pyqn/base_unit.py` & `pyqn-1.4/src/pyqn/base_unit.py`

 * *Files identical despite different names*

### Comparing `pyqn-1.3.2/src/pyqn/dimensions.py` & `pyqn-1.4/src/pyqn/dimensions.py`

 * *Files identical despite different names*

### Comparing `pyqn-1.3.2/src/pyqn/list_base_units.py` & `pyqn-1.4/src/pyqn/list_base_units.py`

 * *Files identical despite different names*

### Comparing `pyqn-1.3.2/src/pyqn/qn_array.py` & `pyqn-1.4/src/pyqn/qn_array.py`

 * *Files identical despite different names*

### Comparing `pyqn-1.3.2/src/pyqn/quantity.py` & `pyqn-1.4/src/pyqn/quantity.py`

 * *Files identical despite different names*

### Comparing `pyqn-1.3.2/src/pyqn/si.py` & `pyqn-1.4/src/pyqn/si.py`

 * *Files identical despite different names*

### Comparing `pyqn-1.3.2/src/pyqn/symbol.py` & `pyqn-1.4/src/pyqn/symbol.py`

 * *Files identical despite different names*

### Comparing `pyqn-1.3.2/src/pyqn/units.py` & `pyqn-1.4/src/pyqn/units.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with PyQn.  If not, see <http://www.gnu.org/licenses/>
 
+import re
 import copy
 from .dimensions import Dimensions
 from .dimensions import d_dimensionless, d_length, d_energy, d_time, d_temperature
 from .atom_unit import AtomUnit, UnitsError, feq
 
 h, NA, c, kB = (6.62607015e-34, 6.02214076e23, 299792458.0, 1.380649e-23)
 
@@ -78,26 +79,43 @@
 
         dims = Dimensions()
         for atom_unit in self.atom_units:
             dims *= atom_unit.dims
         return dims
 
     @classmethod
-    def parse(self, s_compoundunit):
+    def parse(self, s_compoundunit, no_divided_units=False):
         """
         Parse the string s_compoundunit and return the corresponding
         Units object.
 
         """
 
+        if no_divided_units:
+            # s_compoundunit does not consist of any units separated by '/'
+            # so parse immediately as a sequence of multiplied units.
+            return Units.parse_mult_units(s_compoundunit)
+
+        # We need to temporarily identify rational exponents (e.g. "Pa-1/2")
+        # and replace the / with : so that we can split up the atomic units
+        # properly.
+        patt = r"\d+/\d+"
+        rational_exponents = re.findall(patt, s_compoundunit)
+        for e in rational_exponents:
+            es = e.replace("/", ":")
+            s_compoundunit = s_compoundunit.replace(e, es)
+
         div_fields = s_compoundunit.split("/")
-        ndiv_fields = len(div_fields)
-        compound_unit = Units.parse_mult_units(div_fields[0])
+        # don't forget to put back the "/" character in any rational exponents.
+        compound_unit = Units.parse_mult_units(div_fields[0].replace(":", "/"))
         for div_field in div_fields[1:]:
-            compound_unit = compound_unit / Units.parse(div_field)
+            div_field = div_field.replace(":", "/")
+            compound_unit = compound_unit / Units.parse(
+                div_field, no_divided_units=True
+            )
         return compound_unit
 
     @classmethod
     def parse_mult_units(self, munit):
         """
         Parse a string of units multiplied together (indicated by '.'),
         returning the corresponding Units object.
@@ -240,15 +258,15 @@
             return "undef"
 
         h = []
         n = len(self.atom_units)
         for i, atom_unit in enumerate(self.atom_units):
             h.extend([atom_unit.prefix or "", atom_unit.base_unit.stem])
             if atom_unit.exponent != 1:
-                h.append("<sup>{:d}</sup>".format(atom_unit.exponent))
+                h.append(f"<sup>{atom_unit.exponent}</sup>")
             if i < n - 1:
                 h.append(" ")
         return "".join(h)
 
     @property
     def latex(self):
         if self.undef:
```

### Comparing `pyqn-1.3.2/src/pyqn.egg-info/PKG-INFO` & `pyqn-1.4/src/pyqn.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqn
-Version: 1.3.2
+Version: 1.4
 Summary: A package for managing physical units and quantities
 Home-page: https://github.com/xnx/pyqn
 Author: Christian Hill
 Author-email: xn.hill@gmail.com
 Project-URL: Bug Reports, https://github.com/xnx/pyqn/issues
 Keywords: chemistry,units,physical quantities,unit conversion
 Classifier: Development Status :: 4 - Beta
@@ -14,20 +14,28 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyparsing>=2.3
+Requires-Dist: importlib-resources>=1.0; python_version < "3.7.0"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: ipython; extra == "dev"
 
 ********************
 Introduction to PyQn
 ********************
```

