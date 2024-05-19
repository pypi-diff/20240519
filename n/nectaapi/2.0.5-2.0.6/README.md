# Comparing `tmp/nectaapi-2.0.5.tar.gz` & `tmp/nectaapi-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nectaapi-2.0.5.tar", last modified: Sun Oct 23 15:10:16 2022, max compression
+gzip compressed data, was "nectaapi-2.0.6.tar", last modified: Sun May 19 13:16:58 2024, max compression
```

## Comparing `nectaapi-2.0.5.tar` & `nectaapi-2.0.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2022-10-23 15:10:16.131938 nectaapi-2.0.5/
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     2945 2022-07-06 20:44:54.000000 nectaapi-2.0.5/.gitignore
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     1092 2022-01-16 21:36:27.000000 nectaapi-2.0.5/LICENSE
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6732 2022-10-23 15:10:16.131938 nectaapi-2.0.5/PKG-INFO
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     6213 2022-10-23 15:08:30.000000 nectaapi-2.0.5/README.md
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2022-10-23 15:10:16.131938 nectaapi-2.0.5/nectaapi/
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)        0 2022-01-16 21:36:27.000000 nectaapi-2.0.5/nectaapi/__init__.py
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     1516 2022-01-16 21:36:27.000000 nectaapi-2.0.5/nectaapi/comparison.py
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     3215 2022-10-23 14:53:46.000000 nectaapi-2.0.5/nectaapi/schools.py
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     3367 2022-10-23 14:52:53.000000 nectaapi-2.0.5/nectaapi/student.py
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     4018 2022-10-23 14:54:31.000000 nectaapi-2.0.5/nectaapi/students.py
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     9969 2022-10-23 14:55:40.000000 nectaapi-2.0.5/nectaapi/summary.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2022-10-23 15:10:16.131938 nectaapi-2.0.5/nectaapi.egg-info/
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     6732 2022-10-23 15:10:16.000000 nectaapi-2.0.5/nectaapi.egg-info/PKG-INFO
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)      290 2022-10-23 15:10:16.000000 nectaapi-2.0.5/nectaapi.egg-info/SOURCES.txt
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)        1 2022-10-23 15:10:16.000000 nectaapi-2.0.5/nectaapi.egg-info/dependency_links.txt
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)        9 2022-10-23 15:10:16.000000 nectaapi-2.0.5/nectaapi.egg-info/top_level.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2022-10-23 15:10:16.131938 nectaapi-2.0.5/setup.cfg
--rwxrwxrwx   0 vincent   (1000) vincent   (1000)     1033 2022-10-23 15:08:07.000000 nectaapi-2.0.5/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-19 13:16:58.675889 nectaapi-2.0.6/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1092 2023-07-13 11:25:01.000000 nectaapi-2.0.6/LICENSE
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     7121 2024-05-19 13:16:58.675889 nectaapi-2.0.6/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6606 2024-05-19 13:02:55.000000 nectaapi-2.0.6/README.md
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-19 13:16:58.671877 nectaapi-2.0.6/nectaapi/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-07-13 11:25:01.000000 nectaapi-2.0.6/nectaapi/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2298 2024-05-19 06:09:22.000000 nectaapi-2.0.6/nectaapi/comparison.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3602 2024-05-19 11:38:40.000000 nectaapi-2.0.6/nectaapi/schools.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4176 2024-05-19 12:41:02.000000 nectaapi-2.0.6/nectaapi/student.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1045 2023-08-19 21:55:37.000000 nectaapi-2.0.6/nectaapi/student_name.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4448 2024-05-19 12:01:43.000000 nectaapi-2.0.6/nectaapi/students.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10669 2024-05-19 12:54:14.000000 nectaapi-2.0.6/nectaapi/summary.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-05-19 13:16:58.675889 nectaapi-2.0.6/nectaapi.egg-info/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     7121 2024-05-19 13:16:58.000000 nectaapi-2.0.6/nectaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      335 2024-05-19 13:16:58.000000 nectaapi-2.0.6/nectaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-05-19 13:16:58.000000 nectaapi-2.0.6/nectaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       24 2024-05-19 13:16:58.000000 nectaapi-2.0.6/nectaapi.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        9 2024-05-19 13:16:58.000000 nectaapi-2.0.6/nectaapi.egg-info/top_level.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2024-05-19 13:16:58.675889 nectaapi-2.0.6/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1086 2024-05-19 13:14:00.000000 nectaapi-2.0.6/setup.py
```

### Comparing `nectaapi-2.0.5/LICENSE` & `nectaapi-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nectaapi-2.0.5/PKG-INFO` & `nectaapi-2.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,94 @@
 Metadata-Version: 2.1
 Name: nectaapi
-Version: 2.0.5
+Version: 2.0.6
 Summary: Fetch results of various national examinations done in Tanzania
 Home-page: https://github.com/vincent-laizer/NECTA-API
 Author: Tanzania Programmers (Vincent Laizer)
 Author-email: <laizercorp@gmail.com>
-License: UNKNOWN
 Keywords: python,necta,api,necta api,necta tanzania,tanzania programmers
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: beautifulsoup4
 
 # Necta-API
+
 Get a formated data of examination results scrapped from necta results website.
 
 Note this is not an official [NECTA](https://necta.go.tz/) API and is still in development
 
-Current version is `Beta 2.0.4`
+Current version is `Beta 2.0.6`
 
 This Version comes with a more modular structure compared to the previsious ones 
 
-Developed by [**Tanzania Programmers**](https://www.youtube.com/channel/UCuMUw-djxHqOHrvnnFGYtZA), written *by Vincent Laizer.*
+Developed by [**Tanzania Programmers**](https://tanzaniaprogrammers.com/), written *by Vincent Laizer.*
+
 ---
 
 ---
 
 ## Usage
+
 - [x] Get the package via pip
 
-``` 
-    pip install nectaapi 
-```
+    ```bash
+        pip install nectaapi 
+    ```
 
-- In any return value **asterisc '*'** indicates that no data could be scrapped
+    - In any return value **None** indicates that no data could be scrapped
 
 - [x] Get a list of all schools in a given year and exam type.
 
-exam type can be **acsee** or **csee** (for now, more to be added)
+    exam type can be **acsee** or **csee** (for now, more to be added)
 
-```python
-    from nectaapi import schools
+    ```python
+        from nectaapi import schools
 
-    data = schools.schools(2017, 'csee') 
-```
-  the function returns a dictionary in the form
+        data = schools.schools(2017, 'csee') 
+    ```
 
-  ```python
-  {
-      "exam_type": "examamination type",
-      "year_of_exam": "year of examination",
-      "number_of_schools": "number of schools in this exam and year",
-      "schools": [
-          {
-              "school_name": "school name 1",
-              "registration_number":"registration number 1"
-          },
-          {
-              "school_name": "school name 2",
-              "registration_number":"registration number 2"
-          },
-           ...]
-  }
-  ```
+    The function returns a dictionary in the form
+
+    ```python
+    {
+        "exam_type": "examamination type",
+        "year_of_exam": "year of examination",
+        "number_of_schools": "number of schools in this exam and year",
+        "schools": [
+            {
+                "school_name": "school name 1",
+                "registration_number":"registration number 1"
+            },
+            {
+                "school_name": "school name 2",
+                "registration_number":"registration number 2"
+            },
+            ...]
+    }
+    ```
+
+- [x] Get a highlight of school overal results
 
-  - [x] Get a highlight of school overal results
   ```python
     from nectaapi import summary
 
     data = summary.summary(year, examType, schoolNumber)
 
     # schoolNumber is the schools registration number ie s3881 or s1268
   ```
-  the function returns a dictionary in the form
+
+  The function returns a dictionary in the form
+  
   ```python
     {
         "school_name": "name of school",
         "school_number": "school_number",
         "exam_type": "exam_type",
         "year_of_exam": "year",
         "school_category":"category based on number of students",
@@ -99,25 +106,27 @@
         "regional_position": "school's regional position",
         "total_national_schools":"number of schools national wise",
         "total_regional_schools":"number of schools regional wise",
         "gpa": "school's GPA"
     }
   ```
 
-  - [x] Get a single students results
+- [x] Get a single students results
+
   ```python
     from nectaapi import student
 
     results = student.student(year, examType, schoolNumber, studentNumber)
 
     # student number is the students part of their examination number eg 0040 or 0553
   ```
 
   The 'student' function returns a dictionary of this form
-  ```python
+  
+  ```python  
     {
     "examination_number":"students examination number",
     "year_of_exam":"year",
     "exam_type":"exam type",
     "school_name":"name of student's school",
     "gender":"student's gender",
     "division":"students division",
@@ -129,84 +138,94 @@
                 ...
             }
     }
   ```
 
 - [x] Compare schools performance over a range of years or of just a single school
 
-not present in perivious versions
-
-The parameters of the function are, the start year, end year of comparison, exam type and a list of schools to compare. start year is always less than end year, suppose they are equal a one year comparison is returned
+    _not present in perivious versions_
 
-```python
-    from nectaapi import comparison
-    data = comparison.comparison(start_year, end_year, exam_type,  ["school_number1", "school_number2", ...])
-```
+    The parameters of the function are, the start year, end year of comparison, exam type and a list of schools to compare. start year is always less than end year, suppose they are equal a one year comparison is returned
 
-It then returns a dictionary with school comparable data like, gpa, national_position and number_of_students in the form
-
-```python
-    {
-        "year1":{
-            "school_number1":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
-            },
-            "school_number2":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
-            },
-            ...
-        },
-        "year2":{
-            "school_number1":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
-            },
-            "school_number2":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
+    ```python
+        from nectaapi import comparison
+        data = comparison.comparison(startYear, endYear, examType,  ["school_number1", "school_number2", ...])
+    ```
+
+    It then returns a dictionary with school comparable data like, gpa, national_position and number_of_students in the form
+
+    ```python
+        {
+            "year1":{
+                "school_number1":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                "school_number2":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                ...
             },
+            "year2":{
+                "school_number1":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                "school_number2":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                ...
+            }
             ...
         }
-        ...
-    }
-```
+    ```
 
-As one of my teachers said, **"Academics is one of the 3 areas in life where competition is allowed"** *Mr. H. Masegense*, so don't mind comparing performance of schools over the years
+    As one of my teachers said, **"Academics is one of the 3 areas in life where competition is allowed"** *Mr. H. Masegense*, so don't mind comparing performance of schools over the years
 
-+ comparison module comes with a bonus function to check if a school participated in national examinations of a given type and year. Returns a boolean value
+    + Comparison module comes with a bonus function to check if a school participated in national examinations of a given type and year. Returns a boolean value
 
-```python
-    from nectaapi import comparison
-    isPresent = comparison.schoolPresent(year, exam_type, school_number)
-```
+    ```python
+        from nectaapi import comparison
+        isPresent = comparison.schoolPresent(year, exam_type, school_number)
+    ```
 
 ## What's New
 
+## Version 2.0.6
+
+- Compatibility with 2023 **CSEE** results format
+- Compatibility with 2023 **ACSEE** results format
+- Minor bug fixes
+
 ## Version 2.0.5
+
 - Minor bug fixes
 
 ## Version 2.0.4
+
 - Compatibility with 2022 **ACSEE** results format
+
 ## Version 2.0.3
+
 - Compatibility with 2021 **CSEE** results format
+
 ## Version 2.0.0
+
 - Bug fixes on the school summary function
 - proper handling of the year 2015 where GPA system was used.
     - note, in this year, distinction is counted as division one, merit as division two, credit as division three, pass as division four and fail as division zero.
 - school comparison function
 - code modularity improvement
 
 ---
 
   check out video tutorial on [YouTube](https://www.youtube.com/channel/UCuMUw-djxHqOHrvnnFGYtZA) for demos.
 
 ---
 
 ### contributions are awaited for **GitHub repo [NECTA-API](https://github.com/vincent-laizer/NECTA-API)**
-
-
```

### Comparing `nectaapi-2.0.5/README.md` & `nectaapi-2.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 # Necta-API
+
 Get a formated data of examination results scrapped from necta results website.
 
 Note this is not an official [NECTA](https://necta.go.tz/) API and is still in development
 
-Current version is `Beta 2.0.4`
+Current version is `Beta 2.0.6`
 
 This Version comes with a more modular structure compared to the previsious ones 
 
-Developed by [**Tanzania Programmers**](https://www.youtube.com/channel/UCuMUw-djxHqOHrvnnFGYtZA), written *by Vincent Laizer.*
+Developed by [**Tanzania Programmers**](https://tanzaniaprogrammers.com/), written *by Vincent Laizer.*
+
 ---
 
 ---
 
 ## Usage
+
 - [x] Get the package via pip
 
-``` 
-    pip install nectaapi 
-```
+    ```bash
+        pip install nectaapi 
+    ```
 
-- In any return value **asterisc '*'** indicates that no data could be scrapped
+    - In any return value **None** indicates that no data could be scrapped
 
 - [x] Get a list of all schools in a given year and exam type.
 
-exam type can be **acsee** or **csee** (for now, more to be added)
+    exam type can be **acsee** or **csee** (for now, more to be added)
 
-```python
-    from nectaapi import schools
+    ```python
+        from nectaapi import schools
 
-    data = schools.schools(2017, 'csee') 
-```
-  the function returns a dictionary in the form
+        data = schools.schools(2017, 'csee') 
+    ```
 
-  ```python
-  {
-      "exam_type": "examamination type",
-      "year_of_exam": "year of examination",
-      "number_of_schools": "number of schools in this exam and year",
-      "schools": [
-          {
-              "school_name": "school name 1",
-              "registration_number":"registration number 1"
-          },
-          {
-              "school_name": "school name 2",
-              "registration_number":"registration number 2"
-          },
-           ...]
-  }
-  ```
+    The function returns a dictionary in the form
+
+    ```python
+    {
+        "exam_type": "examamination type",
+        "year_of_exam": "year of examination",
+        "number_of_schools": "number of schools in this exam and year",
+        "schools": [
+            {
+                "school_name": "school name 1",
+                "registration_number":"registration number 1"
+            },
+            {
+                "school_name": "school name 2",
+                "registration_number":"registration number 2"
+            },
+            ...]
+    }
+    ```
+
+- [x] Get a highlight of school overal results
 
-  - [x] Get a highlight of school overal results
   ```python
     from nectaapi import summary
 
     data = summary.summary(year, examType, schoolNumber)
 
     # schoolNumber is the schools registration number ie s3881 or s1268
   ```
-  the function returns a dictionary in the form
+
+  The function returns a dictionary in the form
+  
   ```python
     {
         "school_name": "name of school",
         "school_number": "school_number",
         "exam_type": "exam_type",
         "year_of_exam": "year",
         "school_category":"category based on number of students",
@@ -80,25 +87,27 @@
         "regional_position": "school's regional position",
         "total_national_schools":"number of schools national wise",
         "total_regional_schools":"number of schools regional wise",
         "gpa": "school's GPA"
     }
   ```
 
-  - [x] Get a single students results
+- [x] Get a single students results
+
   ```python
     from nectaapi import student
 
     results = student.student(year, examType, schoolNumber, studentNumber)
 
     # student number is the students part of their examination number eg 0040 or 0553
   ```
 
   The 'student' function returns a dictionary of this form
-  ```python
+  
+  ```python  
     {
     "examination_number":"students examination number",
     "year_of_exam":"year",
     "exam_type":"exam type",
     "school_name":"name of student's school",
     "gender":"student's gender",
     "division":"students division",
@@ -110,76 +119,88 @@
                 ...
             }
     }
   ```
 
 - [x] Compare schools performance over a range of years or of just a single school
 
-not present in perivious versions
-
-The parameters of the function are, the start year, end year of comparison, exam type and a list of schools to compare. start year is always less than end year, suppose they are equal a one year comparison is returned
-
-```python
-    from nectaapi import comparison
-    data = comparison.comparison(start_year, end_year, exam_type,  ["school_number1", "school_number2", ...])
-```
+    _not present in perivious versions_
 
-It then returns a dictionary with school comparable data like, gpa, national_position and number_of_students in the form
+    The parameters of the function are, the start year, end year of comparison, exam type and a list of schools to compare. start year is always less than end year, suppose they are equal a one year comparison is returned
 
-```python
-    {
-        "year1":{
-            "school_number1":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
-            },
-            "school_number2":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
-            },
-            ...
-        },
-        "year2":{
-            "school_number1":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
-            },
-            "school_number2":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
+    ```python
+        from nectaapi import comparison
+        data = comparison.comparison(startYear, endYear, examType,  ["school_number1", "school_number2", ...])
+    ```
+
+    It then returns a dictionary with school comparable data like, gpa, national_position and number_of_students in the form
+
+    ```python
+        {
+            "year1":{
+                "school_number1":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                "school_number2":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                ...
             },
+            "year2":{
+                "school_number1":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                "school_number2":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                ...
+            }
             ...
         }
-        ...
-    }
-```
+    ```
 
-As one of my teachers said, **"Academics is one of the 3 areas in life where competition is allowed"** *Mr. H. Masegense*, so don't mind comparing performance of schools over the years
+    As one of my teachers said, **"Academics is one of the 3 areas in life where competition is allowed"** *Mr. H. Masegense*, so don't mind comparing performance of schools over the years
 
-+ comparison module comes with a bonus function to check if a school participated in national examinations of a given type and year. Returns a boolean value
+    + Comparison module comes with a bonus function to check if a school participated in national examinations of a given type and year. Returns a boolean value
 
-```python
-    from nectaapi import comparison
-    isPresent = comparison.schoolPresent(year, exam_type, school_number)
-```
+    ```python
+        from nectaapi import comparison
+        isPresent = comparison.schoolPresent(year, exam_type, school_number)
+    ```
 
 ## What's New
 
+## Version 2.0.6
+
+- Compatibility with 2023 **CSEE** results format
+- Compatibility with 2023 **ACSEE** results format
+- Minor bug fixes
+
 ## Version 2.0.5
+
 - Minor bug fixes
 
 ## Version 2.0.4
+
 - Compatibility with 2022 **ACSEE** results format
+
 ## Version 2.0.3
+
 - Compatibility with 2021 **CSEE** results format
+
 ## Version 2.0.0
+
 - Bug fixes on the school summary function
 - proper handling of the year 2015 where GPA system was used.
     - note, in this year, distinction is counted as division one, merit as division two, credit as division three, pass as division four and fail as division zero.
 - school comparison function
 - code modularity improvement
 
 ---
```

### Comparing `nectaapi-2.0.5/nectaapi/schools.py` & `nectaapi-2.0.6/nectaapi/schools.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,44 +12,56 @@
         {"school_name":"school name 2", "school_number":"school number 2"},
         ...
     ]
 }
 '''
 from bs4 import BeautifulSoup
 import requests
+from typing import Dict,Any
 
-def schools(year, exam_type):
+def schools(year:int, exam_type:str)->Dict[str,Any]:
+    """Gets all schools and their registration numbers in a given year and exam type
+
+    Args:
+        year(int),exam_type(str)
+    
+    Returns:
+        Dict
+    """
+    
     url = ""
 
     # the number of waste rows to skip (letters in the home page), if available
     skip = 0
 
     if exam_type.lower() == "csee":
-        if int(year) == 2021:
-            url = f"https://onlinesys.necta.go.tz/results/2021/csee/csee.htm"
-        elif int(year) == 2016:
+        if int(year) == 2023:
+            url = f"https://matokeo.necta.go.tz/results/2023/csee/CSEE 2023.htm"
+        elif int(year) == 2016 or int(year) == 2022:
             url = f"https://onlinesys.necta.go.tz/results/{year}/csee/index.htm" # f"http://127.0.0.1/necta/{year}/csee"
         else:
             url = f"https://onlinesys.necta.go.tz/results/{year}/csee/csee.htm" # f"http://127.0.0.1/necta/{year}/csee"
 
         if int(year) > 2014:
             skip = 28
 
     elif exam_type.lower() == "acsee":
-        if int(year) == 2022:
-            url = f"https://matokeo.necta.go.tz/acsee2022/index.htm"
-        elif int(year) > 2019:
-            url = f"https://onlinesys.necta.go.tz/results/{year}/acsee/index.htm" # f"http://127.0.0.1/necta/{year}/acsee"
+        if int(year) == 2023:
+            url = f"https://matokeo.necta.go.tz/results/2023/acsee/index.htm"
+        elif int(year) <= 2022 and int(year) >= 2020:
+            url = f"https://onlinesys.necta.go.tz/results/{year}/acsee/index.htm"
+        elif int(year) <= 2019 and int(year) >= 2016:
+            url = f"https://onlinesys.necta.go.tz/results/{year}/acsee/acsee.htm"
         elif int(year) == 2014:
             url = f"https://onlinesys.necta.go.tz/results/2014/acsee/" # f"http://127.0.0.1/necta/{year}/acsee"
         else:
             url = f"https://onlinesys.necta.go.tz/results/{year}/acsee/acsee.htm" # f"http://127.0.0.1/necta/{year}/acsee"
 
         if int(year) > 2015:
-            skip = 27
+            skip = 28
     else:
         # invalid exam type
         raise Exception(f"Invalid Exam Type {exam_type}")
 
     data = requests.get(url)
     if data.status_code == 200:
         soup = BeautifulSoup(data.text, 'html.parser')
```

### Comparing `nectaapi-2.0.5/nectaapi/student.py` & `nectaapi-2.0.6/nectaapi/students.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,145 @@
 '''
-Results of a single student
+A list of all students with their performance in a particular school or center
 returns a dictionary
-{
-    examination_number, year_of_exam, exam_type, school_name, gender,
-    division, points, subjects:
-            {
-                subject1:score1,
-                subject2:score2,
-                ...
-            }
-}
+school_name, school_number, number_of_students, year_of_exam, exam_type, students[
+    {
+        examination_number,
+        gender,
+        division,
+        points,
+        subjects:{
+            subject1:score1,
+            subject2:score2,
+            ...
+        }
+    }
+    ...
+]
 '''
 
 import requests
 from bs4 import BeautifulSoup
 from nectaapi import summary
-from nectaapi.students import splitAfter
+from typing import Dict,Any,List
+
+def students(year:int, exam_type:str, school_number:str)->Dict[str,Any]:
+    """Get all students with their performance in a particular school or center
 
-def student(year, exam_type, school_number, student_number):
+    Args:
+        year(int),exam_type(str), school_number(str)
+    
+    Returns:
+        Dict
+    """
     url = ""
     exam_type = exam_type.lower()
     school_number = school_number.lower()
     year = int(year)
     index = 0
 
     if exam_type == "acsee":
-        if year == 2022:
-            url = f"https://matokeo.necta.go.tz/acsee2022/results/{school_number}.htm"
+        if year == 2023:
+            url = f"https://matokeo.necta.go.tz/results/2023/acsee/results/{school_number}.htm"
         else:
             url = f"https://onlinesys.necta.go.tz/results/{year}/acsee/results/{school_number}.htm" 
-            # http://127.0.0.1/necta/{year}/acsee/s3881.php
         
         if school_number.startswith("p"):
-            if year > 2019:
-                index = 1
+            if year >= 2019:
+                index = 2
             else:
                 index = 0
         else:
-            if year > 2019:
+            if year >= 2019:
                 index = 2
             else:
                 index = 0
 
     elif exam_type == "csee":
-        if int(year) == 2021:
-            url = f"https://onlinesys.necta.go.tz/results/2021/csee/results/{school_number}.htm"
+        if int(year) == 2023:
+            url = f"https://matokeo.necta.go.tz/results/2023/csee/CSEE2023/results/{school_number}.htm"
+        elif int(year) > 2018:
+            url = f"https://onlinesys.necta.go.tz/results/{year}/csee/results/{school_number}.htm"
         elif int(year) > 2014:
             url = f"https://onlinesys.necta.go.tz/results/{year}/csee/results/{school_number}.htm" 
             # http://127.0.0.1/necta/{year}/csee/s3881.php
         else:
             url = f"https://onlinesys.necta.go.tz/results/{year}/csee/{school_number}.htm" 
             # http://127.0.0.1/necta/{year}/csee/s3881.php
 
         if school_number.startswith("p"):
             if year > 2018:
-                index = 1
+                index = 2
             else:
                 index = 0
         else:
             if year > 2018:
                 index = 2
             else:
                 index = 0
-
+    
     data = requests.get(url)
     soup = BeautifulSoup(data.text, 'html.parser')
 
     if data.status_code != 200:
         raise Exception(f"failed to connect to server\nError code {data.status_code}")
     else:
-        s = summary.summary(year, exam_type, school_number)
+        # get some data from summary function
+        school_summary = summary.summary(year, exam_type, school_number)
 
-        student_data = {
-            "examination_number":f"{school_number.upper()}/{student_number}",
+        students = {
+            "school_number":school_number,
+            "school_name":school_summary["school_name"],
             "year_of_exam":year,
             "exam_type":exam_type,
-            "gender":"*",
-            "school_name":s["school_name"],
-            "division":"*",
-            "points":"*",
-            "subjects":{}
+            "number_of_students":school_summary["number_of_students"],
+            "students":[]
         }
 
-        found = False
+        student_data = scrapStudents(soup, index)
+        students["students"] = student_data
 
-        studentsTable = soup.find_all("table")[index]
-        for tr in studentsTable.find_all("tr"):
-            row = []
-            for td in tr.find_all("td"):
-                row.append(td.text.strip('\n'))
-
-            # search for student number
-            if row[0] == student_data["examination_number"]:
-                student_data["gender"] = row[1]
-                student_data["division"] = row[3]
-                student_data["points"] = row[2]
-                student_data["subjects"] = splitAfter(row[4])
-                found = True
+        return students
 
-        if not found:
-            raise Exception(f"Wrong Examination Number {student_data['examination_number']}")
-        else:
-            return student_data
+def scrapStudents(soup, index)->List[Dict[str,Any]]:
+    studentsTable = soup.find_all("table")[index]
+    data = []
+
+    # [1:] -> eliminate the first row containing titles
+    for tr in studentsTable.find_all("tr")[1:]:
+        # row[reg_no, sex, points, division, subjects]
+        row = []
+        for td in tr.find_all("td"):
+            row.append(td.text.strip('\n'))
+
+        subjects = splitAfter(row[4])
+        student = {
+            "examination_number":row[0],
+            "gender":row[1],
+            "division":row[3],
+            "points":row[2],
+            "subjects":subjects
+        }
+
+        # print(student, end='\n')
+        data.append(student)
+
+    return data
+
+# assisting function in obtaining a dictionary of candidates subjects and grades
+def splitAfter(text)->Dict[str,str]:
+    subjects = {} # a dictionary of subject grade pair
+    values = []
+    temp = ""
+    for i in range(0, len(text)-1):
+        temp += text[i]
+        if text[i] == '\'' and text[i+1] == ' ':
+            values.append(temp)
+            temp = ""
+
+    for v in values:
+        q = v.split('-')
+        subject = q[0].strip()
+        grade = q[1].strip().strip('\'')
+        subjects.update({subject: grade})
+
+    return subjects
```

### Comparing `nectaapi-2.0.5/nectaapi/students.py` & `nectaapi-2.0.6/nectaapi/student.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,126 @@
 '''
-A list of all students with their performance in a particular school or center
+Results of a single student
 returns a dictionary
-school_name, school_number, number_of_students, year_of_exam, exam_type, students[
-    {
-        examination_number,
-        gender,
-        division,
-        points,
-        subjects:{
-            subject1:score1,
-            subject2:score2,
-            ...
-        }
-    }
-    ...
-]
+{
+    examination_number, year_of_exam, exam_type, school_name, gender,
+    division, points, subjects:
+            {
+                subject1:score1,
+                subject2:score2,
+                ...
+            }
+}
 '''
 
 import requests
 from bs4 import BeautifulSoup
 from nectaapi import summary
-
-def students(year, exam_type, school_number):
+from nectaapi.students import splitAfter
+from typing import Dict,Any
+from nectaapi.student_name import student_names
+
+def student(year:int, exam_type:str, school_number:str, student_number:int)->Dict[str,Any]:
+    """Results of a single student
+
+    Args:
+        year(int), exam_type(str), school_number(str), student_number(int)
+    
+    Returns:
+        Dict
+    
+    """
+    
     url = ""
     exam_type = exam_type.lower()
     school_number = school_number.lower()
     year = int(year)
     index = 0
 
     if exam_type == "acsee":
-        if year == 2022:
-            url = f"https://matokeo.necta.go.tz/acsee2022/results/{school_number}.htm"
+        if year == 2023:
+            url = f"https://matokeo.necta.go.tz/results/2023/acsee/results/{school_number}.htm"
         else:
             url = f"https://onlinesys.necta.go.tz/results/{year}/acsee/results/{school_number}.htm" 
-            # http://127.0.0.1/necta/{year}/acsee/s3881.php
         
         if school_number.startswith("p"):
             if year > 2019:
-                index = 1
+                index = 2
             else:
                 index = 0
         else:
-            if year > 2019:
+            if year >= 2019:
                 index = 2
             else:
                 index = 0
 
     elif exam_type == "csee":
-        if int(year) == 2021:
-            url = f"https://onlinesys.necta.go.tz/results/2021/csee/results/p0101.htm"
+        if int(year) == 2023:
+            url = f"https://matokeo.necta.go.tz/results/2023/csee/CSEE2023/results/{school_number}.htm"
+        elif int(year) == 2021:
+            url = f"https://onlinesys.necta.go.tz/results/2021/csee/results/{school_number}.htm"
         elif int(year) > 2014:
             url = f"https://onlinesys.necta.go.tz/results/{year}/csee/results/{school_number}.htm" 
             # http://127.0.0.1/necta/{year}/csee/s3881.php
         else:
             url = f"https://onlinesys.necta.go.tz/results/{year}/csee/{school_number}.htm" 
             # http://127.0.0.1/necta/{year}/csee/s3881.php
 
         if school_number.startswith("p"):
             if year > 2018:
-                index = 1
+                index = 2
             else:
                 index = 0
         else:
             if year > 2018:
                 index = 2
             else:
                 index = 0
 
     data = requests.get(url)
     soup = BeautifulSoup(data.text, 'html.parser')
 
     if data.status_code != 200:
         raise Exception(f"failed to connect to server\nError code {data.status_code}")
     else:
-        # get some data from summary function
         s = summary.summary(year, exam_type, school_number)
 
-        students = {
-            "school_number":school_number,
-            "school_name":s["school_name"],
+        student_data = {
+            "examination_number":f"{school_number.upper()}/{student_number}",
             "year_of_exam":year,
             "exam_type":exam_type,
-            "number_of_students":s["number_of_students"],
-            "students":[]
-        }
-
-        student_data = scrapStudents(soup, index)
-        students["students"] = student_data
-
-        return students
-
-def scrapStudents(soup, index):
-    studentsTable = soup.find_all("table")[index]
-    data = []
-
-    # [1:] -> eliminate the first row containing titles
-    for tr in studentsTable.find_all("tr")[1:]:
-        # row[reg_no, sex, points, division, subjects]
-        row = []
-        for td in tr.find_all("td"):
-            row.append(td.text.strip('\n'))
-
-        subjects = splitAfter(row[4])
-        student = {
-            "examination_number":row[0],
-            "gender":row[1],
-            "division":row[3],
-            "points":row[2],
-            "subjects":subjects
+            "gender":"*",
+            "school_name":s["school_name"],
+            "division":"*",
+            "points":"*",
+            "subjects":{}
         }
 
-        # print(student, end='\n')
-        data.append(student)
-
-    return data
+        found = False
 
-# assisting function in obtaining a dictionary of candidates subjects and grades
-def splitAfter(text):
-    subjects = {} # a dictionary of subject grade pair
-    values = []
-    temp = ""
-    for i in range(0, len(text)-1):
-        temp += text[i]
-        if text[i] == '\'' and text[i+1] == ' ':
-            values.append(temp)
-            temp = ""
-
-    for v in values:
-        q = v.split('-')
-        subject = q[0].strip()
-        grade = q[1].strip().strip('\'')
-        subjects.update({subject: grade})
+        studentsTable = soup.find_all("table")[index]
+        for tr in studentsTable.find_all("tr"):
+            row = []
+            for td in tr.find_all("td"):
+                row.append(td.text.strip('\n'))
+
+            # search for student number
+            print(row)
+            if row[0] == student_data["examination_number"]:
+                student_data["gender"] = row[1]
+                student_data["division"] = row[3]
+                student_data["points"] = row[2]
+                student_data["subjects"] = splitAfter(row[4])
+                found = True
 
-    return subjects
+        if not found:
+            raise Exception(f"Wrong Examination Number {student_data['examination_number']}")
+        else:
+            # get student names
+            names = student_names(student_number, school_number, year, exam_type)
+            if names != None:
+                student_data["firstname"] = names["firstname"]
+                student_data["middlename"] = names["middlename"]
+                student_data["lastname"] = names["lastname"]
+                student_data["sex"] = names["sex"]
+                
+            return student_data
```

### Comparing `nectaapi-2.0.5/nectaapi/summary.py` & `nectaapi-2.0.6/nectaapi/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,44 @@
 school_name, school_number, exam_type, year_of_exam, school_category, number_of_students, school_region,
 male_students, female_students, absentees, division_one, division_two, division_three, division_four,
 division_zero, national_position, regional_position, total_national_schools, total_regional_schools, gpa
 '''
 import requests
 from bs4 import BeautifulSoup
 
-def summary(year, exam_type, school_number):
+def summary(year:int, exam_type:str, school_number:str):
+
+    """Summary of a school's performance
+    
+    Args:
+        year(int), exam_type(str), school_number(str)
+    
+    Returns:
+        Dict
+
+    returns a dictionary with these keys and their values
+    school_name, school_number, exam_type, year_of_exam, school_category, number_of_students, school_region,
+    male_students, female_students, absentees, division_one, division_two, division_three, division_four,
+    division_zero, national_position, regional_position, total_national_schools, total_regional_schools, gpa
+    """
+    
     url = ""
     exam_type = exam_type.lower()
     school_number = school_number.lower()
 
     if exam_type == "acsee":
-        if year == 2022:
-            url = f"https://matokeo.necta.go.tz/acsee2022/results/{school_number}.htm"
+        if year == 2023:
+            url = f"https://matokeo.necta.go.tz/results/2023/acsee/results/{school_number}.htm"
         else:
-            url = f"https://onlinesys.necta.go.tz/results/{year}/{exam_type}/results/{school_number}.htm" 
-            # f"http://127.0.0.1/necta/{year}/acsee/s3881.php"
-            # https://onlinesys.necta.go.tz/results/2021/acsee/results/s3881.htm  
+            url = f"https://onlinesys.necta.go.tz/results/{year}/acsee/results/{school_number}.htm" 
+        
     elif exam_type == "csee":
-        if int(year) == 2021:
+        if int(year) == 2023:
+            url = f"https://matokeo.necta.go.tz/results/2023/csee/CSEE2023/results/{school_number}.htm"
+        elif int(year) == 2021:
             url = f"https://onlinesys.necta.go.tz/results/2021/csee/results/{school_number}.htm"
         elif int(year) > 2014:
             url = f"https://onlinesys.necta.go.tz/results/{year}/{exam_type}/results/{school_number}.htm" 
             # f"http://127.0.0.1/necta/{year}/csee/s3881.php"
             # https://onlinesys.necta.go.tz/results/2015/csee/results/s3881.htm 
         else:
             url = f"https://onlinesys.necta.go.tz/results/{year}/{exam_type}/{school_number}.htm" 
@@ -80,15 +96,17 @@
         # centers dont have a bottom summary table and so should not provide these data
         
         if school_number.startswith("p"):
             # handle center
             summary = handleCenter(summary, soup)
         else:
             # handle a school
-            summary = handleSchool(summary, soup)
+            if year != 2015 or exam_type == "acsee":
+                # 2015 has no bottom performance analysis table in csee
+                summary = handleSchool(summary, soup)
     else:
         # failed to fetch data, raise exception
         raise Exception(f"Failed to access {url}\nResponse Code {data.status_code}")
 
     return summary
 
 # initialize numerical values to zero
@@ -146,15 +164,15 @@
 
 # function to scrap school data accordingly
 def handleSchool(summary, soup):
     year = int(summary["year_of_exam"])
     exam_type = summary["exam_type"].lower()
 
     if exam_type == "acsee":
-        if year > 2019:
+        if year >= 2019:
             # has a top analysis table
             summary = scrapManual(soup, summary, 2) # just for absentees
             summary = set_zero(summary)
             summary = scrapTopTable(soup, summary)
             summary = scrapBottomPerformance(soup, summary, 4)
         else:
             # has no top analysis table get data manually
```

### Comparing `nectaapi-2.0.5/nectaapi.egg-info/PKG-INFO` & `nectaapi-2.0.6/nectaapi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,94 @@
 Metadata-Version: 2.1
 Name: nectaapi
-Version: 2.0.5
+Version: 2.0.6
 Summary: Fetch results of various national examinations done in Tanzania
 Home-page: https://github.com/vincent-laizer/NECTA-API
 Author: Tanzania Programmers (Vincent Laizer)
 Author-email: <laizercorp@gmail.com>
-License: UNKNOWN
 Keywords: python,necta,api,necta api,necta tanzania,tanzania programmers
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: beautifulsoup4
 
 # Necta-API
+
 Get a formated data of examination results scrapped from necta results website.
 
 Note this is not an official [NECTA](https://necta.go.tz/) API and is still in development
 
-Current version is `Beta 2.0.4`
+Current version is `Beta 2.0.6`
 
 This Version comes with a more modular structure compared to the previsious ones 
 
-Developed by [**Tanzania Programmers**](https://www.youtube.com/channel/UCuMUw-djxHqOHrvnnFGYtZA), written *by Vincent Laizer.*
+Developed by [**Tanzania Programmers**](https://tanzaniaprogrammers.com/), written *by Vincent Laizer.*
+
 ---
 
 ---
 
 ## Usage
+
 - [x] Get the package via pip
 
-``` 
-    pip install nectaapi 
-```
+    ```bash
+        pip install nectaapi 
+    ```
 
-- In any return value **asterisc '*'** indicates that no data could be scrapped
+    - In any return value **None** indicates that no data could be scrapped
 
 - [x] Get a list of all schools in a given year and exam type.
 
-exam type can be **acsee** or **csee** (for now, more to be added)
+    exam type can be **acsee** or **csee** (for now, more to be added)
 
-```python
-    from nectaapi import schools
+    ```python
+        from nectaapi import schools
 
-    data = schools.schools(2017, 'csee') 
-```
-  the function returns a dictionary in the form
+        data = schools.schools(2017, 'csee') 
+    ```
 
-  ```python
-  {
-      "exam_type": "examamination type",
-      "year_of_exam": "year of examination",
-      "number_of_schools": "number of schools in this exam and year",
-      "schools": [
-          {
-              "school_name": "school name 1",
-              "registration_number":"registration number 1"
-          },
-          {
-              "school_name": "school name 2",
-              "registration_number":"registration number 2"
-          },
-           ...]
-  }
-  ```
+    The function returns a dictionary in the form
+
+    ```python
+    {
+        "exam_type": "examamination type",
+        "year_of_exam": "year of examination",
+        "number_of_schools": "number of schools in this exam and year",
+        "schools": [
+            {
+                "school_name": "school name 1",
+                "registration_number":"registration number 1"
+            },
+            {
+                "school_name": "school name 2",
+                "registration_number":"registration number 2"
+            },
+            ...]
+    }
+    ```
+
+- [x] Get a highlight of school overal results
 
-  - [x] Get a highlight of school overal results
   ```python
     from nectaapi import summary
 
     data = summary.summary(year, examType, schoolNumber)
 
     # schoolNumber is the schools registration number ie s3881 or s1268
   ```
-  the function returns a dictionary in the form
+
+  The function returns a dictionary in the form
+  
   ```python
     {
         "school_name": "name of school",
         "school_number": "school_number",
         "exam_type": "exam_type",
         "year_of_exam": "year",
         "school_category":"category based on number of students",
@@ -99,25 +106,27 @@
         "regional_position": "school's regional position",
         "total_national_schools":"number of schools national wise",
         "total_regional_schools":"number of schools regional wise",
         "gpa": "school's GPA"
     }
   ```
 
-  - [x] Get a single students results
+- [x] Get a single students results
+
   ```python
     from nectaapi import student
 
     results = student.student(year, examType, schoolNumber, studentNumber)
 
     # student number is the students part of their examination number eg 0040 or 0553
   ```
 
   The 'student' function returns a dictionary of this form
-  ```python
+  
+  ```python  
     {
     "examination_number":"students examination number",
     "year_of_exam":"year",
     "exam_type":"exam type",
     "school_name":"name of student's school",
     "gender":"student's gender",
     "division":"students division",
@@ -129,84 +138,94 @@
                 ...
             }
     }
   ```
 
 - [x] Compare schools performance over a range of years or of just a single school
 
-not present in perivious versions
-
-The parameters of the function are, the start year, end year of comparison, exam type and a list of schools to compare. start year is always less than end year, suppose they are equal a one year comparison is returned
+    _not present in perivious versions_
 
-```python
-    from nectaapi import comparison
-    data = comparison.comparison(start_year, end_year, exam_type,  ["school_number1", "school_number2", ...])
-```
+    The parameters of the function are, the start year, end year of comparison, exam type and a list of schools to compare. start year is always less than end year, suppose they are equal a one year comparison is returned
 
-It then returns a dictionary with school comparable data like, gpa, national_position and number_of_students in the form
-
-```python
-    {
-        "year1":{
-            "school_number1":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
-            },
-            "school_number2":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
-            },
-            ...
-        },
-        "year2":{
-            "school_number1":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
-            },
-            "school_number2":{
-                "gpa":"",
-                "national_position":"",
-                "number_of_students":""
+    ```python
+        from nectaapi import comparison
+        data = comparison.comparison(startYear, endYear, examType,  ["school_number1", "school_number2", ...])
+    ```
+
+    It then returns a dictionary with school comparable data like, gpa, national_position and number_of_students in the form
+
+    ```python
+        {
+            "year1":{
+                "school_number1":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                "school_number2":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                ...
             },
+            "year2":{
+                "school_number1":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                "school_number2":{
+                    "gpa":"",
+                    "national_position":"",
+                    "number_of_students":""
+                },
+                ...
+            }
             ...
         }
-        ...
-    }
-```
+    ```
 
-As one of my teachers said, **"Academics is one of the 3 areas in life where competition is allowed"** *Mr. H. Masegense*, so don't mind comparing performance of schools over the years
+    As one of my teachers said, **"Academics is one of the 3 areas in life where competition is allowed"** *Mr. H. Masegense*, so don't mind comparing performance of schools over the years
 
-+ comparison module comes with a bonus function to check if a school participated in national examinations of a given type and year. Returns a boolean value
+    + Comparison module comes with a bonus function to check if a school participated in national examinations of a given type and year. Returns a boolean value
 
-```python
-    from nectaapi import comparison
-    isPresent = comparison.schoolPresent(year, exam_type, school_number)
-```
+    ```python
+        from nectaapi import comparison
+        isPresent = comparison.schoolPresent(year, exam_type, school_number)
+    ```
 
 ## What's New
 
+## Version 2.0.6
+
+- Compatibility with 2023 **CSEE** results format
+- Compatibility with 2023 **ACSEE** results format
+- Minor bug fixes
+
 ## Version 2.0.5
+
 - Minor bug fixes
 
 ## Version 2.0.4
+
 - Compatibility with 2022 **ACSEE** results format
+
 ## Version 2.0.3
+
 - Compatibility with 2021 **CSEE** results format
+
 ## Version 2.0.0
+
 - Bug fixes on the school summary function
 - proper handling of the year 2015 where GPA system was used.
     - note, in this year, distinction is counted as division one, merit as division two, credit as division three, pass as division four and fail as division zero.
 - school comparison function
 - code modularity improvement
 
 ---
 
   check out video tutorial on [YouTube](https://www.youtube.com/channel/UCuMUw-djxHqOHrvnnFGYtZA) for demos.
 
 ---
 
 ### contributions are awaited for **GitHub repo [NECTA-API](https://github.com/vincent-laizer/NECTA-API)**
-
-
```

### Comparing `nectaapi-2.0.5/setup.py` & `nectaapi-2.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.0.5'
+VERSION = '2.0.6'
 DESCRIPTION = 'Fetch results of various national examinations done in Tanzania'
 LONG_DESCRIPTION = ""
 with open('README.md') as rm:
     LONG_DESCRIPTION = rm.read()
 
 # Setting up
 setup(
@@ -13,15 +13,18 @@
     author="Tanzania Programmers (Vincent Laizer)",
     author_email="<laizercorp@gmail.com>",
     url="https://github.com/vincent-laizer/NECTA-API",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=[],
+    install_requires=[
+        'requests',
+        'beautifulsoup4'
+    ],
     keywords=['python', 'necta', 'api', 'necta api', 'necta tanzania', 'tanzania programmers'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

