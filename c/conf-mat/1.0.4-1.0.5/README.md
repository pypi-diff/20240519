# Comparing `tmp/conf-mat-1.0.4.tar.gz` & `tmp/conf-mat-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf-mat-1.0.4.tar", last modified: Sun Mar 10 14:55:07 2024, max compression
+gzip compressed data, was "conf-mat-1.0.5.tar", last modified: Sat May 18 23:45:57 2024, max compression
```

## Comparing `conf-mat-1.0.4.tar` & `conf-mat-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 khiat     (1000) khiat     (1000)        0 2024-03-10 14:55:07.955048 conf-mat-1.0.4/
--rw-rw-r--   0 khiat     (1000) khiat     (1000)    42134 2024-03-10 14:55:07.955048 conf-mat-1.0.4/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)    41688 2024-03-10 14:53:23.000000 conf-mat-1.0.4/README.md
-drwxrwxr-x   0 khiat     (1000) khiat     (1000)        0 2024-03-10 14:55:07.951048 conf-mat-1.0.4/conf_mat/
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      402 2024-03-10 13:36:55.000000 conf-mat-1.0.4/conf_mat/__init__.py
--rw-rw-r--   0 khiat     (1000) khiat     (1000)    68300 2024-03-10 14:40:22.000000 conf-mat-1.0.4/conf_mat/conf_mat.py
-drwxrwxr-x   0 khiat     (1000) khiat     (1000)        0 2024-03-10 14:55:07.951048 conf-mat-1.0.4/conf_mat.egg-info/
--rw-rw-r--   0 khiat     (1000) khiat     (1000)    42134 2024-03-10 14:55:07.000000 conf-mat-1.0.4/conf_mat.egg-info/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      219 2024-03-10 14:55:07.000000 conf-mat-1.0.4/conf_mat.egg-info/SOURCES.txt
--rw-rw-r--   0 khiat     (1000) khiat     (1000)        1 2024-03-10 14:55:07.000000 conf-mat-1.0.4/conf_mat.egg-info/dependency_links.txt
--rw-rw-r--   0 khiat     (1000) khiat     (1000)       34 2024-03-10 14:55:07.000000 conf-mat-1.0.4/conf_mat.egg-info/requires.txt
--rw-rw-r--   0 khiat     (1000) khiat     (1000)        9 2024-03-10 14:55:07.000000 conf-mat-1.0.4/conf_mat.egg-info/top_level.txt
--rw-rw-r--   0 khiat     (1000) khiat     (1000)       38 2024-03-10 14:55:07.955048 conf-mat-1.0.4/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      736 2024-03-10 14:50:35.000000 conf-mat-1.0.4/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-18 23:45:57.547754 conf-mat-1.0.5/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    43560 2024-05-18 23:45:57.547754 conf-mat-1.0.5/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)    43119 2024-05-18 23:40:45.000000 conf-mat-1.0.5/README.md
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-18 23:45:57.547754 conf-mat-1.0.5/conf_mat/
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      397 2024-05-18 21:55:02.000000 conf-mat-1.0.5/conf_mat/__init__.py
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    79949 2024-05-18 23:31:54.000000 conf-mat-1.0.5/conf_mat/conf_mat.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-18 23:45:57.547754 conf-mat-1.0.5/conf_mat.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    43560 2024-05-18 23:45:57.000000 conf-mat-1.0.5/conf_mat.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      219 2024-05-18 23:45:57.000000 conf-mat-1.0.5/conf_mat.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-18 23:45:57.000000 conf-mat-1.0.5/conf_mat.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       34 2024-05-18 23:45:57.000000 conf-mat-1.0.5/conf_mat.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-18 23:45:57.000000 conf-mat-1.0.5/conf_mat.egg-info/top_level.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-18 23:45:57.547754 conf-mat-1.0.5/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      731 2024-05-18 21:54:14.000000 conf-mat-1.0.5/setup.py
```

### Comparing `conf-mat-1.0.4/PKG-INFO` & `conf-mat-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: conf-mat
-Version: 1.0.4
-Summary: Sophisticate Open Confusion Matrix
+Version: 1.0.5
+Summary: Sophisticate Confusion Matrix
 Home-page: https://pypi.org/project/conf-mat/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: confusion matrix
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -62,70 +62,73 @@
 conf_mat_to_html(y_true, y_pred, classes_names=[False, True])
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═════════════════════╤═══════════════════════════╤═══════════════════════════╕
 │ Classes             │ Predicted Positive (PP)   │ Predicted Negative (PN)   │
 ╞═════════════════════╪═══════════════════════════╪═══════════════════════════╡
-│ Actual Positive (P) │ True Positive (TP) : 273  │ False Negative (FN) : 244 │
+│ Actual Positive (P) │ True Positive (TP) : 240  │ False Negative (FN) : 241 │
 │                     │                           │ Type II Error (Missed)    │
 ├─────────────────────┼───────────────────────────┼───────────────────────────┤
-│ Actual Negative (N) │ False Positive (FP) : 229 │ True Negative (TN) : 254  │
+│ Actual Negative (N) │ False Positive (FP) : 259 │ True Negative (TN) : 260  │
 │                     │ Type I Error (Wrong)      │                           │
 ╘═════════════════════╧═══════════════════════════╧═══════════════════════════╛
 
-╒══════════╤══════════════════════════════════════════════════════╕
-│          │ Rate (Score)                                         │
-╞══════════╪══════════════════════════════════════════════════════╡
-│ Accuracy │ Correct        TP + TN                               │
-│          │ _______ : _________________  OR  1 - Error  =  0.53  │
-│          │                                                      │
-│          │  Total    TP + FP + FN + TN                          │
-├──────────┼──────────────────────────────────────────────────────┤
-│ Error    │ Wrong        FP + FN                                 │
-│          │ _____ : _________________  OR  1 - Accuracy  =  0.47 │
-│          │                                                      │
-│          │ Total   TP + FP + FN + TN                            │
-╘══════════╧══════════════════════════════════════════════════════╛
+╒══════════╤═════════════════════════════════════════════════════╕
+│          │ Rate (Score)                                        │
+╞══════════╪═════════════════════════════════════════════════════╡
+│ Accuracy │ Correct        TP + TN                              │
+│          │ _______ : _________________  OR  1 - Error  =  0.5  │
+│          │                                                     │
+│          │  Total    TP + FP + FN + TN                         │
+├──────────┼─────────────────────────────────────────────────────┤
+│ Error    │ Wrong        FP + FN                                │
+│          │ _____ : _________________  OR  1 - Accuracy  =  0.5 │
+│          │                                                     │
+│          │ Total   TP + FP + FN + TN                           │
+╘══════════╧═════════════════════════════════════════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════════╤═════════════════╤════════════════════╤═════════════════════╤════════════════╕
 │                  │ Precision (P)   │ Recall (R)         │ F1-Score (F)        │ Support (S)    │
 ╞══════════════════╪═════════════════╪════════════════════╪═════════════════════╪════════════════╡
 │ Positive (True)  │ P1 (PPV):       │ R1 (Sensitivity):  │ F1 :                │ S1 :           │
 │                  │                 │                    │                     │                │
 │                  │   TP            │   TP               │ 2 x P1 x R1         │                │
-│                  │ _______  = 0.54 │ _______  = 0.53    │ ___________  = 0.54 │  TP + FN = 517 │
+│                  │ _______  = 0.48 │ _______  = 0.5     │ ___________  = 0.49 │  TP + FN = 481 │
 │                  │                 │                    │                     │                │
 │                  │ TP + FP         │ TP + FN            │   P1 + R1           │                │
 ├──────────────────┼─────────────────┼────────────────────┼─────────────────────┼────────────────┤
 │ Negative (False) │ P0 (NPV):       │ R0 (Specificity):  │ F0 :                │ S0 :           │
 │                  │                 │                    │                     │                │
 │                  │   TN            │   TN               │ 2 x P0 x R0         │                │
-│                  │ _______  = 0.51 │ _______  = 0.53    │ ___________  = 0.52 │  FP + TN = 483 │
+│                  │ _______  = 0.52 │ _______  = 0.5     │ ___________  = 0.51 │  FP + TN = 519 │
 │                  │                 │                    │                     │                │
 │                  │ TN + FN         │ TN + FP            │   P0 + R0           │                │
 ├──────────────────┼─────────────────┼────────────────────┼─────────────────────┼────────────────┤
 │ Macro Avg        │ P1 + P0         │ R1 + R0            │ F1 + F0             │ TS = 1000      │
-│                  │ _______  = 0.53 │ _______  = 0.53    │ _______  = 0.53     │                │
+│                  │ _______  = 0.5  │ _______  = 0.5     │ _______  = 0.5      │                │
 │                  │                 │                    │                     │                │
 │                  │    2            │    2               │    2                │                │
 ├──────────────────┼─────────────────┼────────────────────┼─────────────────────┼────────────────┤
 │ Weighted Avg     │ W1              │ W2                 │ W3                  │ TS = 1000      │
-│                  │ __  = 0.53      │ __  = 0.53         │ __  = 0.53          │                │
+│                  │ __  = 0.5       │ __  = 0.5          │ __  = 0.5           │                │
 │                  │                 │                    │                     │                │
 │                  │ TS              │ TS                 │ TS                  │                │
 ╘══════════════════╧═════════════════╧════════════════════╧═════════════════════╧════════════════╛
 
 PPV : Positive Predictive Value
 
 NPV : Negative Predictive Value
@@ -138,14 +141,29 @@
 
 TS : Total Support = S1 + S0
 
 Note : All Real Numbers Are Rounded With Two Digits After The Comma
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1IA3ke21FHXBx7hydamouMhS9zvjHcy9B/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0001/
+
+
 #### You Can Plot, Generate HTML Page For Confusion Matrix And Classification Report Directly From One Calculation 
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import print_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -195,52 +213,70 @@
 conf_mat_to_html(conf_mat=cm, classes_names=[False, True], detail=False)
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═════════════════════╤═══════════════════════════╤═══════════════════════════╕
 │ Classes             │   Predicted Positive (PP) │   Predicted Negative (PN) │
 ╞═════════════════════╪═══════════════════════════╪═══════════════════════════╡
-│ Actual Positive (P) │                       261 │                       271 │
+│ Actual Positive (P) │                       239 │                       246 │
 ├─────────────────────┼───────────────────────────┼───────────────────────────┤
-│ Actual Negative (N) │                       240 │                       228 │
+│ Actual Negative (N) │                       252 │                       263 │
 ╘═════════════════════╧═══════════════════════════╧═══════════════════════════╛
 
 ╒══════════╤════════════════╕
 │          │   Rate (Score) │
 ╞══════════╪════════════════╡
-│ Accuracy │           0.49 │
+│ Accuracy │            0.5 │
 ├──────────┼────────────────┤
-│ Error    │           0.51 │
+│ Error    │            0.5 │
 ╘══════════╧════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════════╤═════════════════╤══════════════╤════════════════╤═══════════════╕
 │                  │   Precision (P) │   Recall (R) │   F1-Score (F) │   Support (S) │
 ╞══════════════════╪═════════════════╪══════════════╪════════════════╪═══════════════╡
-│ Positive (True)  │            0.52 │         0.49 │           0.51 │           532 │
+│ Positive (True)  │            0.49 │         0.49 │           0.49 │           485 │
 ├──────────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Negative (False) │            0.46 │         0.49 │           0.47 │           468 │
+│ Negative (False) │            0.52 │         0.51 │           0.51 │           515 │
 ├──────────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Macro Avg        │            0.49 │         0.49 │           0.49 │          1000 │
+│ Macro Avg        │            0.5  │         0.5  │           0.5  │          1000 │
 ├──────────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Weighted Avg     │            0.49 │         0.49 │           0.49 │          1000 │
+│ Weighted Avg     │            0.5  │         0.5  │           0.5  │          1000 │
 ╘══════════════════╧═════════════════╧══════════════╧════════════════╧═══════════════╛
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1L42AslXk-JRHNYpzMLXoRhtuhVWkTibC/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0011/
+
+
 #### You Can Plot And Generate HTML Page For Confusion Matrix Directly From One Calculation And Without Print Confusion Matrix And Classification Report
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import calc_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -263,17 +299,35 @@
 conf_mat_to_html(conf_mat=cm, classes_names=[False, True], detail=False)
 ```
 
 
 ### Output
 
 
+#### calc_conf_mat Output
+
+
+```bash
+[[243, 242], [256, 259]]
+```
+
+
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1tLBhU1RIlIRFX5YR-nXJMljV_sOVm_SH/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
 ```bash
-[[236, 253], [255, 256]]
+HTML File Generated Successfully :)
 ```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0101/
 
 
 ### For Multi Classification
 
 
 ```python
 from numpy.random import randint
@@ -301,91 +355,94 @@
     'C1', 'C2', 'C3', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9', 'C10'])
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═══════════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤═══════╕
 │ Classes   │   C1 │   C2 │   C3 │   C4 │   C5 │   C6 │   C7 │   C8 │   C9 │   C10 │
 ╞═══════════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪═══════╡
-│ C1        │    5 │   17 │   12 │   11 │   12 │   13 │    6 │   13 │   10 │     7 │
+│ C1        │    8 │    9 │   10 │    7 │   13 │   10 │    9 │   12 │   15 │    11 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C2        │   10 │    6 │   10 │   11 │   13 │   11 │   13 │    8 │   11 │    11 │
+│ C2        │    9 │    6 │    5 │   15 │   10 │   15 │   13 │   10 │   12 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C3        │    6 │    6 │   12 │    8 │   10 │    5 │   11 │    8 │    7 │    11 │
+│ C3        │   14 │    5 │    8 │   10 │   17 │   10 │   10 │    6 │   17 │    12 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C4        │   14 │   13 │   10 │    8 │    9 │    5 │   12 │   14 │    9 │     7 │
+│ C4        │    8 │   10 │    3 │   11 │    7 │    7 │    9 │    8 │    7 │     7 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C5        │   12 │    9 │   15 │    5 │    8 │    9 │    6 │    8 │   10 │    10 │
+│ C5        │    5 │   13 │    7 │   11 │    8 │   13 │    7 │   10 │    6 │     8 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C6        │   12 │   16 │   15 │    9 │   10 │    8 │   10 │   11 │   11 │    12 │
+│ C6        │    9 │   12 │   13 │    9 │   14 │    9 │    8 │    8 │   13 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C7        │   12 │    9 │   12 │   14 │   12 │    6 │   13 │   13 │    7 │    14 │
+│ C7        │   14 │   11 │   11 │   20 │    6 │    6 │    9 │    9 │   10 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C8        │    6 │   11 │    7 │   10 │   10 │   12 │    8 │   10 │    8 │    11 │
+│ C8        │   10 │   13 │    8 │   12 │   12 │    6 │   10 │    5 │   12 │    14 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C9        │   15 │    7 │    8 │    6 │    8 │    6 │    5 │    4 │   14 │    12 │
+│ C9        │   12 │    9 │   13 │    9 │    9 │    8 │   11 │   11 │    9 │     9 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C10       │   10 │   11 │   11 │   13 │    8 │   11 │   12 │   12 │    6 │    15 │
+│ C10       │   12 │   13 │   11 │   12 │   10 │   14 │   11 │    4 │    6 │    11 │
 ╘═══════════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧═══════╛
 
 Yellow  : Not None Correct Values / True Positive (TP) OR True Negative (TN)
 Red     : Not None Wrong Values / False Positive (FP) OR False Negative (FN)
 Green   : None Correct Values
 Blue    : None Wrong Values
 
-╒══════════╤════════════════════════════════════════════════════════════════╕
-│          │ Rate (Score)                                                   │
-╞══════════╪════════════════════════════════════════════════════════════════╡
-│ Accuracy │ Correct      Sum Of Yellow Values                              │
-│          │ _______ : ____________________________  OR  1 - Error  =  0.1  │
-│          │                                                                │
-│          │  Total    Sum Of Yellow And Red Values                         │
-├──────────┼────────────────────────────────────────────────────────────────┤
-│ Error    │ Wrong        Sum Of Red Values                                 │
-│          │ _____ : ____________________________  OR  1 - Accuracy  =  0.9 │
-│          │                                                                │
-│          │ Total   Sum Of Yellow And Red Values                           │
-╘══════════╧════════════════════════════════════════════════════════════════╛
+╒══════════╤═════════════════════════════════════════════════════════════════╕
+│          │ Rate (Score)                                                    │
+╞══════════╪═════════════════════════════════════════════════════════════════╡
+│ Accuracy │ Correct      Sum Of Yellow Values                               │
+│          │ _______ : ____________________________  OR  1 - Error  =  0.08  │
+│          │                                                                 │
+│          │  Total    Sum Of Yellow And Red Values                          │
+├──────────┼─────────────────────────────────────────────────────────────────┤
+│ Error    │ Wrong        Sum Of Red Values                                  │
+│          │ _____ : ____________________________  OR  1 - Accuracy  =  0.92 │
+│          │                                                                 │
+│          │ Total   Sum Of Yellow And Red Values                            │
+╘══════════╧═════════════════════════════════════════════════════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════╤═════════════════╤══════════════╤════════════════╤═══════════════╕
 │              │   Precision (P) │   Recall (R) │   F1-Score (F) │   Support (S) │
 ╞══════════════╪═════════════════╪══════════════╪════════════════╪═══════════════╡
-│ C1           │            0.05 │         0.05 │           0.05 │           106 │
+│ C1           │            0.08 │         0.08 │           0.08 │           104 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C2           │            0.06 │         0.06 │           0.06 │           104 │
+│ C2           │            0.06 │         0.06 │           0.06 │           105 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C3           │            0.11 │         0.14 │           0.12 │            84 │
+│ C3           │            0.09 │         0.07 │           0.08 │           109 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C4           │            0.08 │         0.08 │           0.08 │           101 │
+│ C4           │            0.09 │         0.14 │           0.11 │            77 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C5           │            0.08 │         0.09 │           0.08 │            92 │
+│ C5           │            0.08 │         0.09 │           0.08 │            88 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C6           │            0.09 │         0.07 │           0.08 │           114 │
+│ C6           │            0.09 │         0.09 │           0.09 │           105 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C7           │            0.14 │         0.12 │           0.12 │           112 │
+│ C7           │            0.09 │         0.08 │           0.09 │           106 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C8           │            0.1  │         0.11 │           0.1  │            93 │
+│ C8           │            0.06 │         0.05 │           0.05 │           102 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C9           │            0.15 │         0.16 │           0.16 │            85 │
+│ C9           │            0.08 │         0.09 │           0.09 │           100 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C10          │            0.14 │         0.14 │           0.14 │           109 │
+│ C10          │            0.11 │         0.11 │           0.11 │           104 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Macro Avg    │            0.1  │         0.1  │           0.1  │          1000 │
+│ Macro Avg    │            0.08 │         0.09 │           0.08 │          1000 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Weighted Avg │            0.1  │         0.1  │           0.1  │          1000 │
+│ Weighted Avg │            0.08 │         0.08 │           0.08 │          1000 │
 ╘══════════════╧═════════════════╧══════════════╧════════════════╧═══════════════╛
 
 Precision    : Yellow Value / Sum Of Yellow Value Column
 
 Recall       : Yellow Value / Sum Of Yellow Value Row
 
 F1-Score     : (2 x Precision x Recall) / (Precision + Recall)
@@ -412,14 +469,29 @@
 
                Support   : Total (Sum Of All Matrix)
 
 Note : All Real Numbers Are Rounded With Two Digits After The Comma
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1Gp0CcqZwwZdb8ZTELzfKciJasFGNyqTc/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0111/
+
+
 #### You Can Plot, Generate HTML Page For Confusion Matrix And Classification Report Directly From One Calculation 
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import print_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -475,84 +547,102 @@
     'C1', 'C2', 'C3', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9', 'C10'], detail=False)
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═══════════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤═══════╕
 │ Classes   │   C1 │   C2 │   C3 │   C4 │   C5 │   C6 │   C7 │   C8 │   C9 │   C10 │
 ╞═══════════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪═══════╡
-│ C1        │   10 │    5 │    7 │    7 │    8 │   10 │    9 │   10 │   12 │     8 │
+│ C1        │   10 │    5 │   15 │    6 │    9 │   12 │   13 │    5 │   12 │    13 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C2        │    7 │   14 │   14 │    9 │    9 │   13 │   14 │   11 │   14 │     7 │
+│ C2        │   13 │    5 │    9 │    6 │   13 │   11 │   12 │    5 │    6 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C3        │   13 │   12 │    5 │    9 │    6 │    8 │    9 │   10 │   14 │     8 │
+│ C3        │   11 │   16 │    8 │   10 │   12 │   15 │    7 │   11 │   10 │    12 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C4        │    6 │   11 │    9 │   18 │   11 │    7 │   10 │   11 │    6 │     7 │
+│ C4        │   10 │    9 │   10 │    7 │   15 │   13 │   12 │   11 │   11 │    11 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C5        │    9 │    5 │   11 │    9 │    7 │    8 │    8 │   20 │    9 │    10 │
+│ C5        │   10 │    9 │   12 │    8 │   13 │    7 │    7 │    7 │    9 │     7 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C6        │   12 │    5 │    8 │   11 │   11 │   12 │   14 │   14 │   11 │     7 │
+│ C6        │   14 │   13 │   14 │   11 │    6 │   11 │    8 │   13 │   11 │    13 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C7        │   13 │    8 │   10 │    7 │   10 │   12 │   15 │   10 │    8 │     8 │
+│ C7        │    9 │   11 │   11 │    9 │    9 │   12 │    9 │   10 │    9 │     9 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C8        │   10 │    5 │    6 │   14 │   11 │    9 │    9 │   10 │    4 │    13 │
+│ C8        │   10 │   11 │   12 │   10 │    7 │   10 │   14 │   10 │   13 │    11 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C9        │   11 │   13 │   10 │   10 │   13 │   10 │    8 │   12 │    9 │    15 │
+│ C9        │    8 │   14 │    9 │    8 │    9 │    7 │    9 │   11 │    9 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C10       │   11 │   12 │   11 │   10 │    9 │    8 │    6 │   14 │   12 │    15 │
+│ C10       │    8 │   10 │    7 │    4 │    8 │   13 │    8 │    6 │    9 │    13 │
 ╘═══════════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧═══════╛
 
 ╒══════════╤════════════════╕
 │          │   Rate (Score) │
 ╞══════════╪════════════════╡
-│ Accuracy │           0.12 │
+│ Accuracy │           0.1  │
 ├──────────┼────────────────┤
-│ Error    │           0.89 │
+│ Error    │           0.91 │
 ╘══════════╧════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════╤═════════════════╤══════════════╤════════════════╤═══════════════╕
 │              │   Precision (P) │   Recall (R) │   F1-Score (F) │   Support (S) │
 ╞══════════════╪═════════════════╪══════════════╪════════════════╪═══════════════╡
-│ C1           │            0.1  │         0.12 │           0.11 │            86 │
+│ C1           │            0.1  │         0.1  │           0.1  │           100 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C2           │            0.16 │         0.12 │           0.14 │           112 │
+│ C2           │            0.05 │         0.06 │           0.05 │            90 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C3           │            0.05 │         0.05 │           0.05 │            94 │
+│ C3           │            0.07 │         0.07 │           0.07 │           112 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C4           │            0.17 │         0.19 │           0.18 │            96 │
+│ C4           │            0.09 │         0.06 │           0.07 │           109 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C5           │            0.07 │         0.07 │           0.07 │            96 │
+│ C5           │            0.13 │         0.15 │           0.14 │            89 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C6           │            0.12 │         0.11 │           0.12 │           105 │
+│ C6           │            0.1  │         0.1  │           0.1  │           114 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C7           │            0.15 │         0.15 │           0.15 │           101 │
+│ C7           │            0.09 │         0.09 │           0.09 │            98 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C8           │            0.08 │         0.11 │           0.09 │            91 │
+│ C8           │            0.11 │         0.09 │           0.1  │           108 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C9           │            0.09 │         0.08 │           0.09 │           111 │
+│ C9           │            0.09 │         0.1  │           0.09 │            94 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C10          │            0.15 │         0.14 │           0.15 │           108 │
+│ C10          │            0.12 │         0.15 │           0.13 │            86 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Macro Avg    │            0.12 │         0.11 │           0.11 │          1000 │
+│ Macro Avg    │            0.1  │         0.1  │           0.1  │          1000 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Weighted Avg │            0.12 │         0.12 │           0.12 │          1000 │
+│ Weighted Avg │            0.09 │         0.1  │           0.09 │          1000 │
 ╘══════════════╧═════════════════╧══════════════╧════════════════╧═══════════════╛
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1Card-dZs6sSjgqdiVPUMesXjy3u9nsuY/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/1001/
+
+
 #### You Can Plot And Generate HTML Page For Confusion Matrix Directly From One Calculation And Without Print Confusion Matrix And Classification Report
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import calc_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -577,25 +667,40 @@
     'C1', 'C2', 'C3', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9', 'C10'], detail=False)
 ```
 
 
 ### Output
 
 
+#### calc_conf_mat Output
+
+
 ```bash
-[[9, 12, 11, 8, 10, 10, 7, 6, 11, 9], [12, 9, 12, 9, 7, 3, 16, 7, 7, 11], [7, 10, 25, 14, 5, 14, 9, 11, 6, 12], [7, 15, 9, 11, 13, 13, 4, 7, 10, 10], [12, 10, 11, 3, 14, 6, 8, 19, 6, 15], [5, 14, 13, 17, 9, 8, 8, 7, 11, 17], [7, 10, 10, 10, 6, 9, 10, 4, 9, 11], [8, 9, 11, 7, 11, 11, 15, 9, 13, 12], [12, 12, 9, 6, 11, 7, 10, 13, 7, 10], [11, 5, 9, 13, 8, 14, 3, 9, 15, 13]]
+[[16, 11, 8, 6, 4, 11, 12, 9, 10, 6], [12, 15, 14, 7, 20, 7, 17, 8, 6, 10], [13, 13, 11, 12, 11, 10, 11, 9, 8, 9], [12, 11, 5, 15, 9, 10, 8, 10, 13, 9], [8, 13, 11, 8, 8, 8, 12, 15, 7, 12], [13, 8, 17, 14, 8, 7, 10, 6, 8, 6], [7, 21, 7, 7, 10, 11, 10, 12, 11, 8], [9, 10, 15, 11, 7, 6, 9, 6, 9, 9], [9, 13, 7, 14, 7, 10, 5, 11, 5, 7], [13, 9, 11, 8, 12, 12, 9, 7, 6, 13]]
 ```
 
 
-### Note
+#### plot_conf_mat Output
 
 
-These outputs are for the calc_conf_mat and print_conf_mat functions only, in both cases. I'll leave it to you to figure out the last two functions plot_conf_mat and conf_mat_to_html on your own.
+https://drive.google.com/file/d/1wmH3jQj8WZKtf2Vr-7LQgkI1udDFm0Zj/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/1011/
+
+
+### Note
 
 
-You can call all the functions with the camelCase format.
+You can call all functions with the camelCase format.
 
 
 ## License
 
 
 This project is licensed under the MIT LICENSE - see the [LICENSE](https://opensource.org/licenses/MIT) for more details.
```

### Comparing `conf-mat-1.0.4/README.md` & `conf-mat-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -48,70 +48,73 @@
 conf_mat_to_html(y_true, y_pred, classes_names=[False, True])
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═════════════════════╤═══════════════════════════╤═══════════════════════════╕
 │ Classes             │ Predicted Positive (PP)   │ Predicted Negative (PN)   │
 ╞═════════════════════╪═══════════════════════════╪═══════════════════════════╡
-│ Actual Positive (P) │ True Positive (TP) : 273  │ False Negative (FN) : 244 │
+│ Actual Positive (P) │ True Positive (TP) : 240  │ False Negative (FN) : 241 │
 │                     │                           │ Type II Error (Missed)    │
 ├─────────────────────┼───────────────────────────┼───────────────────────────┤
-│ Actual Negative (N) │ False Positive (FP) : 229 │ True Negative (TN) : 254  │
+│ Actual Negative (N) │ False Positive (FP) : 259 │ True Negative (TN) : 260  │
 │                     │ Type I Error (Wrong)      │                           │
 ╘═════════════════════╧═══════════════════════════╧═══════════════════════════╛
 
-╒══════════╤══════════════════════════════════════════════════════╕
-│          │ Rate (Score)                                         │
-╞══════════╪══════════════════════════════════════════════════════╡
-│ Accuracy │ Correct        TP + TN                               │
-│          │ _______ : _________________  OR  1 - Error  =  0.53  │
-│          │                                                      │
-│          │  Total    TP + FP + FN + TN                          │
-├──────────┼──────────────────────────────────────────────────────┤
-│ Error    │ Wrong        FP + FN                                 │
-│          │ _____ : _________________  OR  1 - Accuracy  =  0.47 │
-│          │                                                      │
-│          │ Total   TP + FP + FN + TN                            │
-╘══════════╧══════════════════════════════════════════════════════╛
+╒══════════╤═════════════════════════════════════════════════════╕
+│          │ Rate (Score)                                        │
+╞══════════╪═════════════════════════════════════════════════════╡
+│ Accuracy │ Correct        TP + TN                              │
+│          │ _______ : _________________  OR  1 - Error  =  0.5  │
+│          │                                                     │
+│          │  Total    TP + FP + FN + TN                         │
+├──────────┼─────────────────────────────────────────────────────┤
+│ Error    │ Wrong        FP + FN                                │
+│          │ _____ : _________________  OR  1 - Accuracy  =  0.5 │
+│          │                                                     │
+│          │ Total   TP + FP + FN + TN                           │
+╘══════════╧═════════════════════════════════════════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════════╤═════════════════╤════════════════════╤═════════════════════╤════════════════╕
 │                  │ Precision (P)   │ Recall (R)         │ F1-Score (F)        │ Support (S)    │
 ╞══════════════════╪═════════════════╪════════════════════╪═════════════════════╪════════════════╡
 │ Positive (True)  │ P1 (PPV):       │ R1 (Sensitivity):  │ F1 :                │ S1 :           │
 │                  │                 │                    │                     │                │
 │                  │   TP            │   TP               │ 2 x P1 x R1         │                │
-│                  │ _______  = 0.54 │ _______  = 0.53    │ ___________  = 0.54 │  TP + FN = 517 │
+│                  │ _______  = 0.48 │ _______  = 0.5     │ ___________  = 0.49 │  TP + FN = 481 │
 │                  │                 │                    │                     │                │
 │                  │ TP + FP         │ TP + FN            │   P1 + R1           │                │
 ├──────────────────┼─────────────────┼────────────────────┼─────────────────────┼────────────────┤
 │ Negative (False) │ P0 (NPV):       │ R0 (Specificity):  │ F0 :                │ S0 :           │
 │                  │                 │                    │                     │                │
 │                  │   TN            │   TN               │ 2 x P0 x R0         │                │
-│                  │ _______  = 0.51 │ _______  = 0.53    │ ___________  = 0.52 │  FP + TN = 483 │
+│                  │ _______  = 0.52 │ _______  = 0.5     │ ___________  = 0.51 │  FP + TN = 519 │
 │                  │                 │                    │                     │                │
 │                  │ TN + FN         │ TN + FP            │   P0 + R0           │                │
 ├──────────────────┼─────────────────┼────────────────────┼─────────────────────┼────────────────┤
 │ Macro Avg        │ P1 + P0         │ R1 + R0            │ F1 + F0             │ TS = 1000      │
-│                  │ _______  = 0.53 │ _______  = 0.53    │ _______  = 0.53     │                │
+│                  │ _______  = 0.5  │ _______  = 0.5     │ _______  = 0.5      │                │
 │                  │                 │                    │                     │                │
 │                  │    2            │    2               │    2                │                │
 ├──────────────────┼─────────────────┼────────────────────┼─────────────────────┼────────────────┤
 │ Weighted Avg     │ W1              │ W2                 │ W3                  │ TS = 1000      │
-│                  │ __  = 0.53      │ __  = 0.53         │ __  = 0.53          │                │
+│                  │ __  = 0.5       │ __  = 0.5          │ __  = 0.5           │                │
 │                  │                 │                    │                     │                │
 │                  │ TS              │ TS                 │ TS                  │                │
 ╘══════════════════╧═════════════════╧════════════════════╧═════════════════════╧════════════════╛
 
 PPV : Positive Predictive Value
 
 NPV : Negative Predictive Value
@@ -124,14 +127,29 @@
 
 TS : Total Support = S1 + S0
 
 Note : All Real Numbers Are Rounded With Two Digits After The Comma
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1IA3ke21FHXBx7hydamouMhS9zvjHcy9B/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0001/
+
+
 #### You Can Plot, Generate HTML Page For Confusion Matrix And Classification Report Directly From One Calculation 
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import print_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -181,52 +199,70 @@
 conf_mat_to_html(conf_mat=cm, classes_names=[False, True], detail=False)
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═════════════════════╤═══════════════════════════╤═══════════════════════════╕
 │ Classes             │   Predicted Positive (PP) │   Predicted Negative (PN) │
 ╞═════════════════════╪═══════════════════════════╪═══════════════════════════╡
-│ Actual Positive (P) │                       261 │                       271 │
+│ Actual Positive (P) │                       239 │                       246 │
 ├─────────────────────┼───────────────────────────┼───────────────────────────┤
-│ Actual Negative (N) │                       240 │                       228 │
+│ Actual Negative (N) │                       252 │                       263 │
 ╘═════════════════════╧═══════════════════════════╧═══════════════════════════╛
 
 ╒══════════╤════════════════╕
 │          │   Rate (Score) │
 ╞══════════╪════════════════╡
-│ Accuracy │           0.49 │
+│ Accuracy │            0.5 │
 ├──────────┼────────────────┤
-│ Error    │           0.51 │
+│ Error    │            0.5 │
 ╘══════════╧════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════════╤═════════════════╤══════════════╤════════════════╤═══════════════╕
 │                  │   Precision (P) │   Recall (R) │   F1-Score (F) │   Support (S) │
 ╞══════════════════╪═════════════════╪══════════════╪════════════════╪═══════════════╡
-│ Positive (True)  │            0.52 │         0.49 │           0.51 │           532 │
+│ Positive (True)  │            0.49 │         0.49 │           0.49 │           485 │
 ├──────────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Negative (False) │            0.46 │         0.49 │           0.47 │           468 │
+│ Negative (False) │            0.52 │         0.51 │           0.51 │           515 │
 ├──────────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Macro Avg        │            0.49 │         0.49 │           0.49 │          1000 │
+│ Macro Avg        │            0.5  │         0.5  │           0.5  │          1000 │
 ├──────────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Weighted Avg     │            0.49 │         0.49 │           0.49 │          1000 │
+│ Weighted Avg     │            0.5  │         0.5  │           0.5  │          1000 │
 ╘══════════════════╧═════════════════╧══════════════╧════════════════╧═══════════════╛
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1L42AslXk-JRHNYpzMLXoRhtuhVWkTibC/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0011/
+
+
 #### You Can Plot And Generate HTML Page For Confusion Matrix Directly From One Calculation And Without Print Confusion Matrix And Classification Report
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import calc_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -249,17 +285,35 @@
 conf_mat_to_html(conf_mat=cm, classes_names=[False, True], detail=False)
 ```
 
 
 ### Output
 
 
+#### calc_conf_mat Output
+
+
+```bash
+[[243, 242], [256, 259]]
+```
+
+
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1tLBhU1RIlIRFX5YR-nXJMljV_sOVm_SH/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
 ```bash
-[[236, 253], [255, 256]]
+HTML File Generated Successfully :)
 ```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0101/
 
 
 ### For Multi Classification
 
 
 ```python
 from numpy.random import randint
@@ -287,91 +341,94 @@
     'C1', 'C2', 'C3', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9', 'C10'])
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═══════════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤═══════╕
 │ Classes   │   C1 │   C2 │   C3 │   C4 │   C5 │   C6 │   C7 │   C8 │   C9 │   C10 │
 ╞═══════════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪═══════╡
-│ C1        │    5 │   17 │   12 │   11 │   12 │   13 │    6 │   13 │   10 │     7 │
+│ C1        │    8 │    9 │   10 │    7 │   13 │   10 │    9 │   12 │   15 │    11 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C2        │   10 │    6 │   10 │   11 │   13 │   11 │   13 │    8 │   11 │    11 │
+│ C2        │    9 │    6 │    5 │   15 │   10 │   15 │   13 │   10 │   12 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C3        │    6 │    6 │   12 │    8 │   10 │    5 │   11 │    8 │    7 │    11 │
+│ C3        │   14 │    5 │    8 │   10 │   17 │   10 │   10 │    6 │   17 │    12 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C4        │   14 │   13 │   10 │    8 │    9 │    5 │   12 │   14 │    9 │     7 │
+│ C4        │    8 │   10 │    3 │   11 │    7 │    7 │    9 │    8 │    7 │     7 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C5        │   12 │    9 │   15 │    5 │    8 │    9 │    6 │    8 │   10 │    10 │
+│ C5        │    5 │   13 │    7 │   11 │    8 │   13 │    7 │   10 │    6 │     8 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C6        │   12 │   16 │   15 │    9 │   10 │    8 │   10 │   11 │   11 │    12 │
+│ C6        │    9 │   12 │   13 │    9 │   14 │    9 │    8 │    8 │   13 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C7        │   12 │    9 │   12 │   14 │   12 │    6 │   13 │   13 │    7 │    14 │
+│ C7        │   14 │   11 │   11 │   20 │    6 │    6 │    9 │    9 │   10 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C8        │    6 │   11 │    7 │   10 │   10 │   12 │    8 │   10 │    8 │    11 │
+│ C8        │   10 │   13 │    8 │   12 │   12 │    6 │   10 │    5 │   12 │    14 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C9        │   15 │    7 │    8 │    6 │    8 │    6 │    5 │    4 │   14 │    12 │
+│ C9        │   12 │    9 │   13 │    9 │    9 │    8 │   11 │   11 │    9 │     9 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C10       │   10 │   11 │   11 │   13 │    8 │   11 │   12 │   12 │    6 │    15 │
+│ C10       │   12 │   13 │   11 │   12 │   10 │   14 │   11 │    4 │    6 │    11 │
 ╘═══════════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧═══════╛
 
 Yellow  : Not None Correct Values / True Positive (TP) OR True Negative (TN)
 Red     : Not None Wrong Values / False Positive (FP) OR False Negative (FN)
 Green   : None Correct Values
 Blue    : None Wrong Values
 
-╒══════════╤════════════════════════════════════════════════════════════════╕
-│          │ Rate (Score)                                                   │
-╞══════════╪════════════════════════════════════════════════════════════════╡
-│ Accuracy │ Correct      Sum Of Yellow Values                              │
-│          │ _______ : ____________________________  OR  1 - Error  =  0.1  │
-│          │                                                                │
-│          │  Total    Sum Of Yellow And Red Values                         │
-├──────────┼────────────────────────────────────────────────────────────────┤
-│ Error    │ Wrong        Sum Of Red Values                                 │
-│          │ _____ : ____________________________  OR  1 - Accuracy  =  0.9 │
-│          │                                                                │
-│          │ Total   Sum Of Yellow And Red Values                           │
-╘══════════╧════════════════════════════════════════════════════════════════╛
+╒══════════╤═════════════════════════════════════════════════════════════════╕
+│          │ Rate (Score)                                                    │
+╞══════════╪═════════════════════════════════════════════════════════════════╡
+│ Accuracy │ Correct      Sum Of Yellow Values                               │
+│          │ _______ : ____________________________  OR  1 - Error  =  0.08  │
+│          │                                                                 │
+│          │  Total    Sum Of Yellow And Red Values                          │
+├──────────┼─────────────────────────────────────────────────────────────────┤
+│ Error    │ Wrong        Sum Of Red Values                                  │
+│          │ _____ : ____________________________  OR  1 - Accuracy  =  0.92 │
+│          │                                                                 │
+│          │ Total   Sum Of Yellow And Red Values                            │
+╘══════════╧═════════════════════════════════════════════════════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════╤═════════════════╤══════════════╤════════════════╤═══════════════╕
 │              │   Precision (P) │   Recall (R) │   F1-Score (F) │   Support (S) │
 ╞══════════════╪═════════════════╪══════════════╪════════════════╪═══════════════╡
-│ C1           │            0.05 │         0.05 │           0.05 │           106 │
+│ C1           │            0.08 │         0.08 │           0.08 │           104 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C2           │            0.06 │         0.06 │           0.06 │           104 │
+│ C2           │            0.06 │         0.06 │           0.06 │           105 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C3           │            0.11 │         0.14 │           0.12 │            84 │
+│ C3           │            0.09 │         0.07 │           0.08 │           109 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C4           │            0.08 │         0.08 │           0.08 │           101 │
+│ C4           │            0.09 │         0.14 │           0.11 │            77 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C5           │            0.08 │         0.09 │           0.08 │            92 │
+│ C5           │            0.08 │         0.09 │           0.08 │            88 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C6           │            0.09 │         0.07 │           0.08 │           114 │
+│ C6           │            0.09 │         0.09 │           0.09 │           105 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C7           │            0.14 │         0.12 │           0.12 │           112 │
+│ C7           │            0.09 │         0.08 │           0.09 │           106 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C8           │            0.1  │         0.11 │           0.1  │            93 │
+│ C8           │            0.06 │         0.05 │           0.05 │           102 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C9           │            0.15 │         0.16 │           0.16 │            85 │
+│ C9           │            0.08 │         0.09 │           0.09 │           100 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C10          │            0.14 │         0.14 │           0.14 │           109 │
+│ C10          │            0.11 │         0.11 │           0.11 │           104 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Macro Avg    │            0.1  │         0.1  │           0.1  │          1000 │
+│ Macro Avg    │            0.08 │         0.09 │           0.08 │          1000 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Weighted Avg │            0.1  │         0.1  │           0.1  │          1000 │
+│ Weighted Avg │            0.08 │         0.08 │           0.08 │          1000 │
 ╘══════════════╧═════════════════╧══════════════╧════════════════╧═══════════════╛
 
 Precision    : Yellow Value / Sum Of Yellow Value Column
 
 Recall       : Yellow Value / Sum Of Yellow Value Row
 
 F1-Score     : (2 x Precision x Recall) / (Precision + Recall)
@@ -398,14 +455,29 @@
 
                Support   : Total (Sum Of All Matrix)
 
 Note : All Real Numbers Are Rounded With Two Digits After The Comma
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1Gp0CcqZwwZdb8ZTELzfKciJasFGNyqTc/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0111/
+
+
 #### You Can Plot, Generate HTML Page For Confusion Matrix And Classification Report Directly From One Calculation 
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import print_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -461,84 +533,102 @@
     'C1', 'C2', 'C3', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9', 'C10'], detail=False)
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═══════════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤═══════╕
 │ Classes   │   C1 │   C2 │   C3 │   C4 │   C5 │   C6 │   C7 │   C8 │   C9 │   C10 │
 ╞═══════════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪═══════╡
-│ C1        │   10 │    5 │    7 │    7 │    8 │   10 │    9 │   10 │   12 │     8 │
+│ C1        │   10 │    5 │   15 │    6 │    9 │   12 │   13 │    5 │   12 │    13 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C2        │    7 │   14 │   14 │    9 │    9 │   13 │   14 │   11 │   14 │     7 │
+│ C2        │   13 │    5 │    9 │    6 │   13 │   11 │   12 │    5 │    6 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C3        │   13 │   12 │    5 │    9 │    6 │    8 │    9 │   10 │   14 │     8 │
+│ C3        │   11 │   16 │    8 │   10 │   12 │   15 │    7 │   11 │   10 │    12 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C4        │    6 │   11 │    9 │   18 │   11 │    7 │   10 │   11 │    6 │     7 │
+│ C4        │   10 │    9 │   10 │    7 │   15 │   13 │   12 │   11 │   11 │    11 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C5        │    9 │    5 │   11 │    9 │    7 │    8 │    8 │   20 │    9 │    10 │
+│ C5        │   10 │    9 │   12 │    8 │   13 │    7 │    7 │    7 │    9 │     7 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C6        │   12 │    5 │    8 │   11 │   11 │   12 │   14 │   14 │   11 │     7 │
+│ C6        │   14 │   13 │   14 │   11 │    6 │   11 │    8 │   13 │   11 │    13 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C7        │   13 │    8 │   10 │    7 │   10 │   12 │   15 │   10 │    8 │     8 │
+│ C7        │    9 │   11 │   11 │    9 │    9 │   12 │    9 │   10 │    9 │     9 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C8        │   10 │    5 │    6 │   14 │   11 │    9 │    9 │   10 │    4 │    13 │
+│ C8        │   10 │   11 │   12 │   10 │    7 │   10 │   14 │   10 │   13 │    11 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C9        │   11 │   13 │   10 │   10 │   13 │   10 │    8 │   12 │    9 │    15 │
+│ C9        │    8 │   14 │    9 │    8 │    9 │    7 │    9 │   11 │    9 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C10       │   11 │   12 │   11 │   10 │    9 │    8 │    6 │   14 │   12 │    15 │
+│ C10       │    8 │   10 │    7 │    4 │    8 │   13 │    8 │    6 │    9 │    13 │
 ╘═══════════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧═══════╛
 
 ╒══════════╤════════════════╕
 │          │   Rate (Score) │
 ╞══════════╪════════════════╡
-│ Accuracy │           0.12 │
+│ Accuracy │           0.1  │
 ├──────────┼────────────────┤
-│ Error    │           0.89 │
+│ Error    │           0.91 │
 ╘══════════╧════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════╤═════════════════╤══════════════╤════════════════╤═══════════════╕
 │              │   Precision (P) │   Recall (R) │   F1-Score (F) │   Support (S) │
 ╞══════════════╪═════════════════╪══════════════╪════════════════╪═══════════════╡
-│ C1           │            0.1  │         0.12 │           0.11 │            86 │
+│ C1           │            0.1  │         0.1  │           0.1  │           100 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C2           │            0.16 │         0.12 │           0.14 │           112 │
+│ C2           │            0.05 │         0.06 │           0.05 │            90 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C3           │            0.05 │         0.05 │           0.05 │            94 │
+│ C3           │            0.07 │         0.07 │           0.07 │           112 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C4           │            0.17 │         0.19 │           0.18 │            96 │
+│ C4           │            0.09 │         0.06 │           0.07 │           109 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C5           │            0.07 │         0.07 │           0.07 │            96 │
+│ C5           │            0.13 │         0.15 │           0.14 │            89 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C6           │            0.12 │         0.11 │           0.12 │           105 │
+│ C6           │            0.1  │         0.1  │           0.1  │           114 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C7           │            0.15 │         0.15 │           0.15 │           101 │
+│ C7           │            0.09 │         0.09 │           0.09 │            98 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C8           │            0.08 │         0.11 │           0.09 │            91 │
+│ C8           │            0.11 │         0.09 │           0.1  │           108 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C9           │            0.09 │         0.08 │           0.09 │           111 │
+│ C9           │            0.09 │         0.1  │           0.09 │            94 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C10          │            0.15 │         0.14 │           0.15 │           108 │
+│ C10          │            0.12 │         0.15 │           0.13 │            86 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Macro Avg    │            0.12 │         0.11 │           0.11 │          1000 │
+│ Macro Avg    │            0.1  │         0.1  │           0.1  │          1000 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Weighted Avg │            0.12 │         0.12 │           0.12 │          1000 │
+│ Weighted Avg │            0.09 │         0.1  │           0.09 │          1000 │
 ╘══════════════╧═════════════════╧══════════════╧════════════════╧═══════════════╛
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1Card-dZs6sSjgqdiVPUMesXjy3u9nsuY/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/1001/
+
+
 #### You Can Plot And Generate HTML Page For Confusion Matrix Directly From One Calculation And Without Print Confusion Matrix And Classification Report
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import calc_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -563,25 +653,40 @@
     'C1', 'C2', 'C3', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9', 'C10'], detail=False)
 ```
 
 
 ### Output
 
 
+#### calc_conf_mat Output
+
+
 ```bash
-[[9, 12, 11, 8, 10, 10, 7, 6, 11, 9], [12, 9, 12, 9, 7, 3, 16, 7, 7, 11], [7, 10, 25, 14, 5, 14, 9, 11, 6, 12], [7, 15, 9, 11, 13, 13, 4, 7, 10, 10], [12, 10, 11, 3, 14, 6, 8, 19, 6, 15], [5, 14, 13, 17, 9, 8, 8, 7, 11, 17], [7, 10, 10, 10, 6, 9, 10, 4, 9, 11], [8, 9, 11, 7, 11, 11, 15, 9, 13, 12], [12, 12, 9, 6, 11, 7, 10, 13, 7, 10], [11, 5, 9, 13, 8, 14, 3, 9, 15, 13]]
+[[16, 11, 8, 6, 4, 11, 12, 9, 10, 6], [12, 15, 14, 7, 20, 7, 17, 8, 6, 10], [13, 13, 11, 12, 11, 10, 11, 9, 8, 9], [12, 11, 5, 15, 9, 10, 8, 10, 13, 9], [8, 13, 11, 8, 8, 8, 12, 15, 7, 12], [13, 8, 17, 14, 8, 7, 10, 6, 8, 6], [7, 21, 7, 7, 10, 11, 10, 12, 11, 8], [9, 10, 15, 11, 7, 6, 9, 6, 9, 9], [9, 13, 7, 14, 7, 10, 5, 11, 5, 7], [13, 9, 11, 8, 12, 12, 9, 7, 6, 13]]
 ```
 
 
-### Note
+#### plot_conf_mat Output
 
 
-These outputs are for the calc_conf_mat and print_conf_mat functions only, in both cases. I'll leave it to you to figure out the last two functions plot_conf_mat and conf_mat_to_html on your own.
+https://drive.google.com/file/d/1wmH3jQj8WZKtf2Vr-7LQgkI1udDFm0Zj/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/1011/
+
+
+### Note
 
 
-You can call all the functions with the camelCase format.
+You can call all functions with the camelCase format.
 
 
 ## License
 
 
 This project is licensed under the MIT LICENSE - see the [LICENSE](https://opensource.org/licenses/MIT) for more details.
```

### Comparing `conf-mat-1.0.4/conf_mat/conf_mat.py` & `conf-mat-1.0.5/conf_mat/conf_mat.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Khiat Mohammed Abderrezzak <khiat.abderrezzak@gmail.com>
 
-"""Sophisticate Open Confusion Matrix"""
+"""Sophisticate Confusion Matrix"""
+
+# To Get The Img Path
+from os import path
 
 # To Draw Tables In The Console And The Web Page
 from tabulate import tabulate
 
 # Data Visualization
 from matplotlib.pyplot import (
     imshow,
@@ -114,23 +117,26 @@
             left=False,
             right=False,
             labelright=False,
             labelleft=True,
         )
         # Printing The Title And YLabel
         xlabel(
-            "\nConfusion Matrix (Unary Classification)"
-            if len(cm) == 1
-            else "\nConfusion Matrix (Binary Classification)"
-            if len(cm) == 2
-            else "\nConfusion Matrix (Multi Classification)",
+            (
+                "\nConfusion Matrix (Unary Classification)"
+                if len(cm) == 1
+                else (
+                    "\nConfusion Matrix (Binary Classification)"
+                    if len(cm) == 2
+                    else "\nConfusion Matrix (Multi Classification)"
+                )
+            ),
             loc="center",
         )
-        ylabel("Actual Classes" if len(cm) >
-               1 else "Actual class", loc="center")
+        ylabel("Actual Classes" if len(cm) > 1 else "Actual class", loc="center")
         # Deviding Imshow Squares With Black Bold Lines
         if len(cm) > 1:
             for i in range(1, len(val)):
                 # Horizontal Line
                 axhline(i - 0.5, color="black", linewidth=2)
                 # Vertical Line
                 axvline(i - 0.5, color="black", linewidth=2)
@@ -172,16 +178,15 @@
         # Fix The Difference Between The Two Lists
         if len(mining) > len(target):
             dif: int = len(mining) - len(target)
             for i in range(dif):
                 target.append(len(target) + i)
         # Label Encoding
         for i in range(len(y_or_predicted_y)):
-            y_or_predicted_y[i] = target[mining.index(
-                str(y_or_predicted_y[i]))]
+            y_or_predicted_y[i] = target[mining.index(str(y_or_predicted_y[i]))]
         # Preparing X Axis And Y Axis Real Values List
         final: list = []
         # Append The Real Values In X Axis And Y Axis List
         for i, j in zip(mining, target):
             final.append(i + "/" + j)
         # Return Encoded Data
         return y_or_predicted_y, list(map(str, predicted_y_or_y)), final
@@ -206,16 +211,15 @@
         # Fix The Difference Between The Two Lists
         if len(mining) > len(target):
             dif: int = len(mining) - len(target)
             for i in range(dif):
                 target.append(len(target) + i)
         # Label Encoding
         for i in range(len(predicted_y_or_y)):
-            predicted_y_or_y[i] = target[mining.index(
-                str(predicted_y_or_y[i]))]
+            predicted_y_or_y[i] = target[mining.index(str(predicted_y_or_y[i]))]
         # Preparing X Axis And Y Axis Real Values List
         final: list = []
         # Append The Real Values In X Axis And Y Axis List
         for i, j in zip(target, mining):
             final.append(i + "/" + j)
         # Return Encoded Data
         return list(map(str, y_or_predicted_y)), predicted_y_or_y, final
@@ -301,34 +305,40 @@
             rcm[lines][columns] = rcm[1 - lines][1 - columns]
             rcm[1 - lines][1 - columns] = help
     return rcm
 
 
 def red(text: str) -> str:
     """Red Coloring Function"""
-    # Coloring The Input Text With Red Color
     return "\033[91;1m{}\033[00m".format(text)
 
 
 def green(text: str) -> str:
     """Green Coloring Function"""
-    # Coloring The Input Text With Green Color
     return "\033[92;1m{}\033[00m".format(text)
 
 
+def blue(text: str) -> str:
+    """Blue Coloring Function"""
+    return "\033[94;1m{}\033[00m".format(text)
+
+
 def yellow(text: str) -> str:
     """Yellow Coloring Function"""
-    # Coloring The Input Text With Yellow Color
     return "\033[93;1m{}\033[00m".format(text)
 
 
-def blue(text: str) -> str:
-    """Blue Coloring Function"""
-    # Coloring The Input Text With Blue Color
-    return "\033[94;1m{}\033[00m".format(text)
+def cyan(text: str) -> str:
+    """Cyan Coloring Function"""
+    return "\033[36;1m{}\033[00m".format(text)
+
+
+def white(text: str) -> str:
+    """White Coloring Function"""
+    return "\033[37;1m{}\033[00m".format(text)
 
 
 def classification_report_calculation(
     cm: list, val: list = [], html: bool = False
 ) -> float | list:
     """Classification Report Calculation"""
     if len(cm) == 2:
@@ -422,47 +432,83 @@
             # Increase In The Recall Sum
             rec_sum += class_repo[i][1]
             # F1-Score Calculation
             som2: int = class_repo[i][0] + class_repo[i][1]
             if som2 == 0:
                 class_repo[i][2] = float(0)
             else:
-                class_repo[i][2] = (2 * class_repo[i][0] *
-                                    class_repo[i][1]) / som2
+                class_repo[i][2] = (2 * class_repo[i][0] * class_repo[i][1]) / som2
             # Increase In The F1-Score Sum
             f1_sum += class_repo[i][2]
             # Support Calculation
             class_repo[i][3] = sum(cm[i])
             # Calculating Percesion For The Weighted Avg
             wa_per_sum += class_repo[i][0] * class_repo[i][3]
             # Calculating Recall For The Weighted Avg
             wa_rec_sum += class_repo[i][1] * class_repo[i][3]
             # Calculating F1-Score For The Weighted Avg
             wa_f1_sum += class_repo[i][2] * class_repo[i][3]
             # Round The Precision Value
-            class_repo[i][0] = round(class_repo[i][0], 2)
+            class_repo[i][0] = (
+                cyan(f"{round(class_repo[i][0], 2)}")
+                if not html
+                else round(class_repo[i][0], 2)
+            )
             # Round The Precision Value
-            class_repo[i][1] = round(class_repo[i][1], 2)
+            class_repo[i][1] = (
+                cyan(f"{round(class_repo[i][1], 2)}")
+                if not html
+                else round(class_repo[i][1], 2)
+            )
             # Round The F1-Score Value
-            class_repo[i][2] = round(class_repo[i][2], 2)
+            class_repo[i][2] = (
+                cyan(f"{round(class_repo[i][2], 2)}")
+                if not html
+                else round(class_repo[i][2], 2)
+            )
+            class_repo[i][3] = cyan(f"{sum(cm[i])}") if not html else class_repo[i][3]
         # Preparing The Macro Avg And Weighted Avg Matrix.
         class_repo_con = [
             [
-                "Macro Avg",
-                round(per_sum / len(val), 2),
-                round(rec_sum / len(val), 2),
-                round(f1_sum / len(val), 2),
-                total,
+                white("Macro Avg") if not html else "Macro Avg",
+                (
+                    cyan(round(per_sum / len(val), 2))
+                    if not html
+                    else round(per_sum / len(val), 2)
+                ),
+                (
+                    cyan(round(rec_sum / len(val), 2))
+                    if not html
+                    else round(rec_sum / len(val), 2)
+                ),
+                (
+                    cyan(round(f1_sum / len(val), 2))
+                    if not html
+                    else round(f1_sum / len(val), 2)
+                ),
+                cyan(total) if not html else total,
             ],
             [
-                "Weighted Avg",
-                round(wa_per_sum / total, 2),
-                round(wa_rec_sum / total, 2),
-                round(wa_f1_sum / total, 2),
-                total,
+                white("Weighted Avg") if not html else "Weighted Avg",
+                (
+                    cyan(round(wa_per_sum / total, 2))
+                    if not html
+                    else round(wa_per_sum / total, 2)
+                ),
+                (
+                    cyan(round(wa_rec_sum / total, 2))
+                    if not html
+                    else round(wa_rec_sum / total, 2)
+                ),
+                (
+                    cyan(round(wa_f1_sum / total, 2))
+                    if not html
+                    else round(wa_f1_sum / total, 2)
+                ),
+                cyan(total) if not html else total,
             ],
         ]
         # Correct Values Sum
         correct: int = 0
         # Wrong Values Sum
         wrong: int = 0
         # Colored The Values
@@ -494,22 +540,28 @@
         accuracy: float = correct / total
         # Calculating The Error Rate
         error: float = wrong / total
         # Insert The Column Of Classes
         val.insert(0, "Classes")
         # Insert Classes In Confusion Matrix
         for i in range(len(cm)):
-            cm[i].insert(0, val[i + 1])
+            if not html:
+                cm[i].insert(0, white(val[i + 1]))
+            else:
+                cm[i].insert(0, val[i + 1])
         # Insert Classes In Classification Report Matrix
         for i in range(len(class_repo)):
-            class_repo[i].insert(0, val[i + 1])
+            if not html:
+                class_repo[i].insert(0, white(val[i + 1]))
+            else:
+                class_repo[i].insert(0, val[i + 1])
         return accuracy, error, class_repo, class_repo_con
     else:
         # Printing Error Msg
-        print("This Function Work Just With Confusion Matrix of Length >= 2")
+        raise TypeError("This Function Work Just With Confusion Matrix of Length >= 2")
 
 
 def classes_check(classes_names: list, val: list, func: int) -> list:
     """Classes Names Check Function"""
     # Check The Type Of Classes Names variable
     if type(classes_names) == list:
         if len(classes_names) == 0:
@@ -517,30 +569,42 @@
             return val
         elif len(classes_names) != 0 and (
             len(classes_names) > len(val) or len(classes_names) < len(val)
         ):
             # Printing Error Msg
             print(
                 (
-                    "plot_conf_mat "
+                    cyan("plot_conf_mat ")
                     if func == 0
-                    else "print_conf_mat "
-                    if func == 1
-                    else "conf_mat_to_html "
-                    if func == 2
-                    else "plotConfMat "
-                    if func == 3
-                    else "printConfMat "
-                    if func == 4
-                    else "confMatToHtml "
-                    if func == 5
-                    else "lambda "
+                    else (
+                        cyan("print_conf_mat ")
+                        if func == 1
+                        else (
+                            cyan("conf_mat_to_html ")
+                            if func == 2
+                            else (
+                                cyan("plotConfMat ")
+                                if func == 3
+                                else (
+                                    cyan("printConfMat ")
+                                    if func == 4
+                                    else (
+                                        cyan("confMatToHtml ")
+                                        if func == 5
+                                        else cyan("lambda ")
+                                    )
+                                )
+                            )
+                        )
+                    )
                 )
                 + red("Warning")
-                + " : The Number Of Classes Names Is Different From The Number Of Classes"
+                + white(
+                    " : The Number Of Classes Names Is Different From The Number Of Classes"
+                )
             )
             return val
         else:
             # Update To The New List
             return classes_names
     elif type(classes_names) == dict:
         l: list = list(classes_names)
@@ -569,30 +633,42 @@
             classes_names: list = l
         if len(classes_names) == len(val):
             return classes_names
         else:
             # Printing Error Msg
             print(
                 (
-                    "plot_conf_mat "
+                    cyan("plot_conf_mat ")
                     if func == 0
-                    else "print_conf_mat "
-                    if func == 1
-                    else "conf_mat_to_html "
-                    if func == 2
-                    else "plotConfMat "
-                    if func == 3
-                    else "printConfMat "
-                    if func == 4
-                    else "confMatToHtml "
-                    if func == 5
-                    else "lambda "
+                    else (
+                        cyan("print_conf_mat ")
+                        if func == 1
+                        else (
+                            cyan("conf_mat_to_html ")
+                            if func == 2
+                            else (
+                                cyan("plotConfMat ")
+                                if func == 3
+                                else (
+                                    cyan("printConfMat ")
+                                    if func == 4
+                                    else (
+                                        cyan("confMatToHtml ")
+                                        if func == 5
+                                        else cyan("lambda ")
+                                    )
+                                )
+                            )
+                        )
+                    )
                 )
                 + red("Warning")
-                + " : The Number Of Classes Names Is Different From The Number Of Classes"
+                + white(
+                    " : The Number Of Classes Names Is Different From The Number Of Classes"
+                )
             )
             return val
     else:
         try:
             # Converting The Classes Names List Into List Type
             classes_names: list = list(classes_names)
         except:
@@ -601,30 +677,42 @@
         if len(classes_names) == len(val):
             # Update To The New List
             return classes_names
         else:
             # Printing Error Msg
             print(
                 (
-                    "plot_conf_mat "
+                    cyan("plot_conf_mat ")
                     if func == 0
-                    else "print_conf_mat "
-                    if func == 1
-                    else "conf_mat_to_html "
-                    if func == 2
-                    else "plotConfMat "
-                    if func == 3
-                    else "printConfMat "
-                    if func == 4
-                    else "confMatToHtml "
-                    if func == 5
-                    else "lambda "
+                    else (
+                        cyan("print_conf_mat ")
+                        if func == 1
+                        else (
+                            cyan("conf_mat_to_html ")
+                            if func == 2
+                            else (
+                                cyan("plotConfMat ")
+                                if func == 3
+                                else (
+                                    cyan("printConfMat ")
+                                    if func == 4
+                                    else (
+                                        cyan("confMatToHtml ")
+                                        if func == 5
+                                        else cyan("lambda ")
+                                    )
+                                )
+                            )
+                        )
+                    )
                 )
                 + red("Warning")
-                + " : The Number Of Classes Names Is Different From The Number Of Classes"
+                + white(
+                    " : The Number Of Classes Names Is Different From The Number Of Classes"
+                )
             )
             return val
 
 
 def control(
     y_or_predicted_y: list,
     predicted_y_or_y: list,
@@ -657,19 +745,19 @@
             val: list = classes_check(classes_names, val, func)
     return cm, val
 
 
 def calc_conf_mat(y_or_predicted_y: list, predicted_y_or_y: list) -> list:
     """Confusion Matrix Calculation Function"""
     if len(y_or_predicted_y) == len(predicted_y_or_y):
-        cm, val = control(y_or_predicted_y, predicted_y_or_y, spe=True)
+        cm, _ = control(y_or_predicted_y, predicted_y_or_y, spe=True)
         return cm
     else:
         # Printing Error Msg
-        print(
+        raise TypeError(
             "The List Of Original Values And The List Of Predicted Values Are Not Of The Same Length :("
         )
 
 
 def calcConfMat(y_or_predicted_y: list, predicted_y_or_y: list) -> list:
     cm: list = calc_conf_mat(y_or_predicted_y, predicted_y_or_y)
     return cm
@@ -692,31 +780,29 @@
                 pass
             else:
                 fn = 0
         except NameError as e1:
             fn = 0
         if len(conf_mat) == 0:
             # Calculating The Confusion Matrix
-            cm, val = control(y_or_predicted_y,
-                              predicted_y_or_y, classes_names, fn)
+            cm, val = control(y_or_predicted_y, predicted_y_or_y, classes_names, fn)
         else:
             # Puting The Confusion Matrix Directely
             cm: list = list(conf_mat)
             # Checking The Classes Names
             val: list = classes_check(classes_names, [*range(len(cm))], fn)
         fn = -1
         if len(cm) == 0:
             # Printing Msg
             print("There Is Nothing To See Here :)")
         elif len(cm) == 1:
             # Preparing Imshow
             imshow_config(cm)
             # Printing The Real Values In X Axis And Y Axis
-            xticks(ticks=[0], labels=[
-                   f"Positive If Pos OR Negative If Neg ({val[0]})"])
+            xticks(ticks=[0], labels=[f"Positive If Pos OR Negative If Neg ({val[0]})"])
             yticks(ticks=[0], labels=[f"Pos OR Neg ({val[0]})"], rotation=90)
             # Preparing The Data Of Square
             annot: list = (
                 [f"True Positive OR True Negative \n\nTP OR TN : \n\n{cm[0][0]}"]
                 if detail
                 else [cm[0][0]]
             )
@@ -785,15 +871,15 @@
                         horizontalalignment="center",
                         verticalalignment="center",
                         fontsize=10,
                         color="black",
                     )
     else:
         # Printing Error Msg
-        print(
+        raise TypeError(
             "The List Of Original Values And The List Of Predicted Values Are Not Of The Same Length :("
         )
 
 
 def plotConfMat(
     y_or_predicted_y: list = [],
     predicted_y_or_y: list = [],
@@ -827,89 +913,104 @@
         try:
             if fn == 4:
                 pass
             else:
                 fn = 1
         except NameError as e1:
             fn = 1
-        cm, val = control(y_or_predicted_y, predicted_y_or_y,
-                          classes_names, fn)
+        cm, val = control(y_or_predicted_y, predicted_y_or_y, classes_names, fn)
         fn = -1
-        cmc: list = [[cm[i][j]
-                      for j in range(len(cm[i]))] for i in range(len(cm))]
+        cmc: list = [[cm[i][j] for j in range(len(cm[i]))] for i in range(len(cm))]
         if len(cm) == 0:
             # Printing All Data
             print([])
         if len(cm) == 1:
             # Preparing Confusion Matrix
             data1: list = [
                 [
                     "",
-                    f"Positive If Positive OR Negative If Negative ({val[0]})",
+                    white("Positive If Positive OR Negative If Negative (")
+                    + cyan(f"{val[0]}")
+                    + white(")"),
                 ],
                 [
-                    f"Positive OR Negative ({val[0]})",
-                    f"True Positive OR True Negative \n\n           TP OR TN : \n\n              {cm[0][0]}"
-                    if detail
-                    else cm[0][0],
+                    white("Positive OR Negative (") + cyan(f"{val[0]}") + white(")"),
+                    (
+                        white("True Positive OR True Negative ")
+                        + "\n\n"
+                        + white("           TP OR TN : ")
+                        + "\n\n"
+                        + cyan(f"              {cm[0][0]}")
+                        if detail
+                        else cyan(f"{cm[0][0]}")
+                    ),
                 ],
             ]
             # Preparing The Rate/Score Table
             data2: list = [
                 [
                     "",
-                    "Rate (Score)",
+                    white("Rate (Score)"),
                 ],
                 [
-                    "Accuracy",
-                    "1",
+                    white("Accuracy"),
+                    cyan("1"),
                 ],
                 [
-                    "Error",
-                    "0",
+                    white("Error"),
+                    cyan("0"),
                 ],
             ]
             # Preparing Classification Report
             data3: list = [
                 [
-                    "Precision (P)",
-                    "Recall (R)",
-                    "F1-Score (F)",
-                    "Support (S)",
-                ],
-                [
-                    f"Positive OR Negative ({val[0]})",
-                    "1",
-                    "1",
-                    "1",
-                    f"{cm[0][0]}",
-                ],
-                [
-                    "Macro Avg",
-                    "1",
-                    "1",
-                    "1",
-                    f"{cm[0][0]}",
-                ],
-                [
-                    "Weighted Avg",
-                    "1",
-                    "1",
-                    "1",
-                    f"{cm[0][0]}",
+                    white("Precision (P)"),
+                    white("Recall (R)"),
+                    white("F1-Score (F)"),
+                    white("Support (S)"),
+                ],
+                [
+                    white("Positive OR Negative (") + cyan(f"{val[0]}") + white(")"),
+                    cyan("1"),
+                    cyan("1"),
+                    cyan("1"),
+                    cyan(f"{cm[0][0]}"),
+                ],
+                [
+                    white("Macro Avg"),
+                    cyan("1"),
+                    cyan("1"),
+                    cyan("1"),
+                    cyan(f"{cm[0][0]}"),
+                ],
+                [
+                    white("Weighted Avg"),
+                    cyan("1"),
+                    cyan("1"),
+                    cyan("1"),
+                    cyan(f"{cm[0][0]}"),
                 ],
             ]
             # Printing All Data
-            print("\nConfusion Matrix : \n" + "_" *
-                  len("Confusion Matrix") + "\n")
+            print(
+                white(
+                    "\n"
+                    + white("Confusion Matrix : ")
+                    + "\n"
+                    + white("_" * len("Confusion Matrix"))
+                    + "\n"
+                )
+            )
             print(tabulate(data1, headers="firstrow", tablefmt="fancy_grid") + "\n")
             print(tabulate(data2, headers="firstrow", tablefmt="fancy_grid") + "\n")
             print(
-                "\nClassification Report : \n"
-                + "_" * len("Classification Report")
+                "\n"
+                + white("Classification Report : ")
+                + "\n"
+                + white("_" * len("Classification Report"))
                 + "\n"
             )
             print(tabulate(data3, headers="firstrow", tablefmt="fancy_grid"))
         elif len(cm) == 2:
             (
                 accuracy,
                 error,
@@ -921,452 +1022,603 @@
                 support_0,
                 f_score_1,
                 f_score_0,
             ) = classification_report_calculation(cm)
             # Preparing Confusion Matrix
             data1: list = [
                 [
-                    "Classes",
-                    "Predicted Positive (PP)",
-                    "Predicted Negative (PN)",
+                    white("Classes"),
+                    white("Predicted Positive (PP)"),
+                    white("Predicted Negative (PN)"),
                     "",
                 ],
                 [
-                    "Actual Positive (P)",
-                    ("True Positive (" + yellow("TP") + f") : {cm[1][1]}")
-                    if detail
-                    else cm[1][1],
-                    (
-                        "False Negative ("
-                        + blue("FN")
-                        + f") : {cm[1][0]}\nType II Error (Missed)"
-                    )
-                    if detail
-                    else cm[1][0],
+                    white("Actual Positive (P)"),
+                    (
+                        (
+                            white("True Positive (")
+                            + yellow("TP")
+                            + white(") : ")
+                            + cyan(f"{cm[1][1]}")
+                        )
+                        if detail
+                        else cyan(f"{cm[1][1]}")
+                    ),
+                    (
+                        (
+                            white("False Negative (")
+                            + blue("FN")
+                            + white(") : ")
+                            + cyan(f"{cm[1][0]}")
+                            + "\n"
+                            + cyan("Type II Error (Missed)")
+                        )
+                        if detail
+                        else cyan(f"{cm[1][0]}")
+                    ),
                 ],
                 [
-                    "Actual Negative (N)",
+                    white("Actual Negative (N)"),
+                    (
+                        (
+                            white("False Positive (")
+                            + red("FP")
+                            + white(") : ")
+                            + cyan(f"{cm[0][1]}")
+                            + "\n"
+                            + cyan("Type I Error (Wrong)")
+                        )
+                        if detail
+                        else cyan(f"{cm[0][1]}")
+                    ),
                     (
-                        "False Positive ("
-                        + red("FP")
-                        + f") : {cm[0][1]}\nType I Error (Wrong)"
-                    )
-                    if detail
-                    else cm[0][1],
-                    ("True Negative (" + green("TN") + f") : {cm[0][0]}")
-                    if detail
-                    else cm[0][0],
+                        (
+                            white("True Negative (")
+                            + green("TN")
+                            + white(") : ")
+                            + cyan(f"{cm[0][0]}")
+                        )
+                        if detail
+                        else cyan(f"{cm[0][0]}")
+                    ),
                 ],
             ]
             # Preparing The Rate/Score Table
             data2: list = [
                 [
                     "",
-                    "Rate (Score)",
+                    white("Rate (Score)"),
                 ],
                 [
-                    "Accuracy",
+                    white("Accuracy"),
                     (
-                        "Correct        "
-                        + yellow("TP")
-                        + " + "
-                        + green("TN")
-                        + "\n"
-                        + "_" * len("Correct")
-                        + " : "
-                        + "_" * len("TP + FP + FN + TN")
-                        + "  OR  1 - Error "
-                        + " =  "
-                        + f"{round(accuracy, 2)}"
-                        + "\n\n Total    "
-                        + yellow("TP")
-                        + " + "
-                        + red("FP")
-                        + " + "
-                        + blue("FN")
-                        + " + "
-                        + green("TN")
-                    )
-                    if detail
-                    else round(accuracy, 2),
+                        (
+                            white("Correct        ")
+                            + yellow("TP")
+                            + white(" + ")
+                            + green("TN")
+                            + "\n"
+                            + white("_" * len("Correct"))
+                            + white(" : ")
+                            + white("_" * len("TP + FP + FN + TN"))
+                            + white("  OR  1 - Error ")
+                            + white(" =  ")
+                            + cyan(f"{round(accuracy, 2)}")
+                            + "\n\n"
+                            + white(" Total    ")
+                            + yellow("TP")
+                            + white(" + ")
+                            + red("FP")
+                            + white(" + ")
+                            + blue("FN")
+                            + white(" + ")
+                            + green("TN")
+                        )
+                        if detail
+                        else cyan(f"{round(accuracy, 2)}")
+                    ),
                 ],
                 [
-                    "Error",
+                    white("Error"),
                     (
-                        "Wrong        "
-                        + red("FP")
-                        + " + "
-                        + blue("FN")
-                        + "\n"
-                        + "_" * len("Wrong")
-                        + " : "
-                        + "_" * len("TP + FP + FN + TN")
-                        + "  OR  1 - Accuracy "
-                        + " =  "
-                        + f"{error}"
-                        + "\n\nTotal   "
-                        + yellow("TP")
-                        + " + "
-                        + red("FP")
-                        + " + "
-                        + blue("FN")
-                        + " + "
-                        + green("TN")
-                    )
-                    if detail
-                    else error,
+                        (
+                            white("Wrong        ")
+                            + red("FP")
+                            + white(" + ")
+                            + blue("FN")
+                            + "\n"
+                            + white("_" * len("Wrong"))
+                            + white(" : ")
+                            + white("_" * len("TP + FP + FN + TN"))
+                            + white("  OR  1 - Accuracy ")
+                            + white(" =  ")
+                            + cyan(f"{error}")
+                            + "\n\n"
+                            + white("Total   ")
+                            + yellow("TP")
+                            + white(" + ")
+                            + red("FP")
+                            + white(" + ")
+                            + blue("FN")
+                            + white(" + ")
+                            + green("TN")
+                        )
+                        if detail
+                        else cyan(f"{error}")
+                    ),
                 ],
             ]
             # Preparing Classification Report
             data3: list = [
                 [
-                    "Precision (P)",
-                    "Recall (R)",
-                    "F1-Score (F)",
-                    "Support (S)",
+                    white("Precision (P)"),
+                    white("Recall (R)"),
+                    white("F1-Score (F)"),
+                    white("Support (S)"),
                 ],
                 [
-                    f"Positive ({val[1]})",
+                    white("Positive (") + cyan(f"{val[1]}") + white(")"),
                     (
-                        "P1 (PPV): \n\n  "
-                        + yellow("TP")
-                        + "\n"
-                        + "_" * len("TP + FP")
-                        + "  = "
-                        + f"{round(precision, 2)}"
-                        + "\n\n"
-                        + yellow("TP")
-                        + " + "
-                        + red("FP")
-                    )
-                    if detail
-                    else round(precision, 2),
-                    (
-                        f"R1 (Sensitivity):\n\n  "
-                        + yellow("TP")
-                        + "\n"
-                        + "_" * len("TP + FN")
-                        + "  = "
-                        + f"{round(recall, 2)}"
-                        + "\n\n"
-                        + yellow("TP")
-                        + " + "
-                        + blue("FN")
-                    )
-                    if detail
-                    else round(recall, 2),
-                    (
-                        "F1 : \n\n"
-                        + "2 x P1 x R1\n"
-                        + "_" * len("2 x P1 x R1")
-                        + "  = "
-                        + f"{round(f_score_1, 2)}"
-                        + "\n\n  P1 + R1"
-                    )
-                    if detail
-                    else round(f_score_1, 2),
-                    (
-                        "S1 : \n\n\n "
-                        + yellow("TP")
-                        + " + "
-                        + blue("FN")
-                        + f" = {support_1}"
-                    )
-                    if detail
-                    else support_1,
+                        (
+                            white("P1 (PPV): ")
+                            + "\n\n  "
+                            + yellow("TP")
+                            + "\n"
+                            + white("_" * len("TP + FP"))
+                            + white("  = ")
+                            + cyan(f"{round(precision, 2)}")
+                            + "\n\n"
+                            + yellow("TP")
+                            + white(" + ")
+                            + red("FP")
+                        )
+                        if detail
+                        else cyan(f"{round(precision, 2)}")
+                    ),
+                    (
+                        (
+                            white("R1 (Sensitivity):")
+                            + "\n\n  "
+                            + yellow("TP")
+                            + "\n"
+                            + white("_" * len("TP + FN"))
+                            + white("  = ")
+                            + cyan(f"{round(recall, 2)}")
+                            + "\n\n"
+                            + yellow("TP")
+                            + white(" + ")
+                            + blue("FN")
+                        )
+                        if detail
+                        else cyan(f"{round(recall, 2)}")
+                    ),
+                    (
+                        (
+                            white("F1 : ")
+                            + "\n\n"
+                            + white("2 x P1 x R1")
+                            + "\n"
+                            + white("_" * len("2 x P1 x R1"))
+                            + white("  = ")
+                            + cyan(f"{round(f_score_1, 2)}")
+                            + "\n\n"
+                            + white("  P1 + R1")
+                        )
+                        if detail
+                        else cyan(f"{round(f_score_1, 2)}")
+                    ),
+                    (
+                        (
+                            white("S1 : ")
+                            + "\n\n\n "
+                            + yellow("TP")
+                            + white(" + ")
+                            + blue("FN")
+                            + cyan(f" = {support_1}")
+                        )
+                        if detail
+                        else cyan(f"{support_1}")
+                    ),
                 ],
                 [
-                    f"Negative ({val[0]})",
+                    white("Negative (") + cyan(f"{val[0]}") + white(")"),
                     (
-                        f"P0 (NPV): \n\n  "
-                        + green("TN")
-                        + "\n"
-                        + "_" * len("TN + FN")
-                        + "  = "
-                        + f"{round(negative_precision, 2)}"
-                        + "\n\n"
-                        + green("TN")
-                        + " + "
-                        + blue("FN")
-                    )
-                    if detail
-                    else round(negative_precision, 2),
-                    (
-                        f"R0 (Specificity): \n\n  "
-                        + green("TN")
-                        + "\n"
-                        + "_" * len("TN + FP")
-                        + "  = "
-                        + f"{round(specificity, 2)}"
-                        + "\n\n"
-                        + green("TN")
-                        + " + "
-                        + red("FP")
-                    )
-                    if detail
-                    else round(specificity, 2),
-                    (
-                        "F0 : \n\n"
-                        + "2 x P0 x R0\n"
-                        + "_" * len("2 x P0 x R0")
-                        + "  = "
-                        + f"{round(f_score_0, 2)}"
-                        + "\n\n  P0 + R0"
-                    )
-                    if detail
-                    else round(f_score_0, 2),
-                    (
-                        "S0 : \n\n\n "
-                        + red("FP")
-                        + " + "
-                        + green("TN")
-                        + f" = {support_0}"
-                    )
-                    if detail
-                    else support_0,
+                        (
+                            white("P0 (NPV): ")
+                            + "\n\n  "
+                            + green("TN")
+                            + "\n"
+                            + white("_" * len("TN + FN"))
+                            + white("  = ")
+                            + cyan(f"{round(negative_precision, 2)}")
+                            + "\n\n"
+                            + green("TN")
+                            + white(" + ")
+                            + blue("FN")
+                        )
+                        if detail
+                        else cyan(f"{round(negative_precision, 2)}")
+                    ),
+                    (
+                        (
+                            white("R0 (Specificity): ")
+                            + "\n\n  "
+                            + green("TN")
+                            + "\n"
+                            + white("_" * len("TN + FP"))
+                            + white("  = ")
+                            + cyan(f"{round(specificity, 2)}")
+                            + "\n\n"
+                            + green("TN")
+                            + white(" + ")
+                            + red("FP")
+                        )
+                        if detail
+                        else cyan(f"{round(specificity, 2)}")
+                    ),
+                    (
+                        (
+                            white("F0 : ")
+                            + "\n\n"
+                            + white("2 x P0 x R0")
+                            + "\n"
+                            + white("_" * len("2 x P0 x R0"))
+                            + white("  = ")
+                            + cyan(f"{round(f_score_0, 2)}")
+                            + "\n\n"
+                            + white("  P0 + R0")
+                        )
+                        if detail
+                        else cyan(f"{round(f_score_0, 2)}")
+                    ),
+                    (
+                        (
+                            white("S0 : ")
+                            + "\n\n\n "
+                            + red("FP")
+                            + white(" + ")
+                            + green("TN")
+                            + cyan(f" = {support_0}")
+                        )
+                        if detail
+                        else cyan(f"{support_0}")
+                    ),
                 ],
                 [
-                    "Macro Avg",
+                    white("Macro Avg"),
+                    (
+                        (
+                            white("P1 + P0")
+                            + "\n"
+                            + white("_" * len("P1 + P0"))
+                            + white("  = ")
+                            + cyan(f"{round((precision + negative_precision)/2, 2)}")
+                            + "\n\n"
+                            + white("   2")
+                        )
+                        if detail
+                        else cyan(f"{round((precision + negative_precision) / 2, 2)}")
+                    ),
+                    (
+                        (
+                            white("R1 + R0")
+                            + "\n"
+                            + white("_" * len("R1 + R0"))
+                            + white("  = ")
+                            + cyan(f"{round((recall + specificity)/2, 2)}")
+                            + "\n\n"
+                            + white("   2")
+                        )
+                        if detail
+                        else cyan(f"{round((recall + specificity) / 2, 2)}")
+                    ),
                     (
-                        "P1 + P0\n"
-                        + "_" * len("P1 + P0")
-                        + "  = "
-                        + f"{round((precision + negative_precision)/2, 2)}"
-                        + "\n\n   2"
-                    )
-                    if detail
-                    else round((precision + negative_precision) / 2, 2),
-                    (
-                        "R1 + R0\n"
-                        + "_" * len("R1 + R0")
-                        + "  = "
-                        + f"{round((recall + specificity)/2, 2)}"
-                        + "\n\n   2"
-                    )
-                    if detail
-                    else round((recall + specificity) / 2, 2),
-                    (
-                        "F1 + F0\n"
-                        + "_" * len("F1 + F0")
-                        + "  = "
-                        + f"{round((f_score_1 + f_score_0)/2, 2)}"
-                        + "\n\n   2"
-                    )
-                    if detail
-                    else round((f_score_1 + f_score_0) / 2, 2),
-                    (f"TS = {support_0 + support_1}")
-                    if detail
-                    else support_0 + support_1,
+                        (
+                            white("F1 + F0")
+                            + "\n"
+                            + white("_" * len("F1 + F0"))
+                            + white("  = ")
+                            + cyan(f"{round((f_score_1 + f_score_0)/2, 2)}")
+                            + "\n\n"
+                            + white("   2")
+                        )
+                        if detail
+                        else cyan(f"{round((f_score_1 + f_score_0) / 2, 2)}")
+                    ),
+                    (
+                        (white("TS = ") + cyan(f"{support_0 + support_1}"))
+                        if detail
+                        else cyan(f"{support_0 + support_1}")
+                    ),
                 ],
                 [
-                    "Weighted Avg",
+                    white("Weighted Avg"),
+                    (
+                        (
+                            white("W1")
+                            + "\n"
+                            + white("_" * len("TS"))
+                            + white("  = ")
+                            + cyan(
+                                f"{round(((precision * support_1) + (negative_precision * support_0))/(support_0 + support_1), 2)}"
+                            )
+                            + "\n\n"
+                            + white("TS")
+                        )
+                        if detail
+                        else cyan(
+                            f"{round(((precision * support_1) + (negative_precision * support_0))/ (support_0 + support_1),2)}"
+                        )
+                    ),
+                    (
+                        (
+                            white("W2")
+                            + "\n"
+                            + white("_" * len("TS"))
+                            + white("  = ")
+                            + cyan(
+                                f"{round(((recall * support_1) + (specificity * support_0))/(support_0 + support_1), 2)}"
+                            )
+                            + "\n\n"
+                            + white("TS")
+                        )
+                        if detail
+                        else cyan(
+                            f"{round(((recall * support_1) + (specificity * support_0))/ (support_0 + support_1),2)}"
+                        )
+                    ),
                     (
-                        "W1\n"
-                        + "_" * len("TS")
-                        + "  = "
-                        + f"{round(((precision * support_1) + (negative_precision * support_0))/(support_0 + support_1), 2)}"
-                        + "\n\nTS"
-                    )
-                    if detail
-                    else round(
-                        ((precision * support_1) + (negative_precision * support_0))
-                        / (support_0 + support_1),
-                        2,
-                    ),
-                    (
-                        "W2\n"
-                        + "_" * len("TS")
-                        + "  = "
-                        + f"{round(((recall * support_1) + (specificity * support_0))/(support_0 + support_1), 2)}"
-                        + "\n\nTS"
-                    )
-                    if detail
-                    else round(
-                        ((recall * support_1) + (specificity * support_0))
-                        / (support_0 + support_1),
-                        2,
-                    ),
-                    (
-                        "W3\n"
-                        + "_" * len("TS")
-                        + "  = "
-                        + f"{round(((f_score_1 * support_1) + (f_score_0 * support_0))/(support_1 + support_0),2)}"
-                        + "\n\nTS"
-                    )
-                    if detail
-                    else round(
-                        ((f_score_1 * support_1) + (f_score_0 * support_0))
-                        / (support_1 + support_0),
-                        2,
-                    ),
-                    (f"TS = {support_0 + support_1}")
-                    if detail
-                    else support_0 + support_1,
+                        (
+                            white("W3")
+                            + "\n"
+                            + white("_" * len("TS"))
+                            + white("  = ")
+                            + cyan(
+                                f"{round(((f_score_1 * support_1) + (f_score_0 * support_0))/(support_1 + support_0),2)}"
+                            )
+                            + "\n\n"
+                            + white("TS")
+                        )
+                        if detail
+                        else cyan(
+                            f"{round(((f_score_1 * support_1) + (f_score_0 * support_0))/ (support_1 + support_0),2)}"
+                        )
+                    ),
+                    (
+                        (white("TS = ") + cyan(f"{support_0 + support_1}"))
+                        if detail
+                        else cyan(f"{support_0 + support_1}")
+                    ),
                 ],
             ]
             # Printing All Data
-            print("\nConfusion Matrix : \n" + "_" *
-                  len("Confusion Matrix") + "\n")
+            print(
+                "\n"
+                + white("Confusion Matrix : ")
+                + "\n"
+                + white("_" * len("Confusion Matrix"))
+                + "\n"
+            )
             print(tabulate(data1, headers="firstrow", tablefmt="fancy_grid") + "\n")
             print(tabulate(data2, headers="firstrow", tablefmt="fancy_grid") + "\n")
             print(
-                "\nClassification Report : \n"
-                + "_" * len("Classification Report")
+                "\n"
+                + white("Classification Report : ")
+                + "\n"
+                + white("_" * len("Classification Report"))
                 + "\n"
             )
             print(tabulate(data3, headers="firstrow", tablefmt="fancy_grid"))
             if detail:
-                print("\nPPV : Positive Predictive Value")
-                print("\nNPV : Negative Predictive Value")
-                print("\nW1 = (P1 x S1) + (P0 x S0)")
-                print("\nW2 = (R1 x S1) + (R0 x S0)")
-                print("\nW3 = (F1 x S1) + (F0 x S0)")
-                print("\nTS : Total Support = S1 + S0")
+                print("\n" + white("PPV : Positive Predictive Value"))
+                print("\n" + white("NPV : Negative Predictive Value"))
+                print("\n" + white("W1 = (P1 x S1) + (P0 x S0)"))
+                print("\n" + white("W2 = (R1 x S1) + (R0 x S0)"))
+                print("\n" + white("W3 = (F1 x S1) + (F0 x S0)"))
+                print("\n" + white("TS : Total Support = S1 + S0"))
                 print(
-                    "\nNote : All Real Numbers Are Rounded With Two Digits After The Comma"
+                    "\n"
+                    + white(
+                        "Note : All Real Numbers Are Rounded With Two Digits After The Comma"
+                    )
                 )
         else:
             (
                 accuracy,
                 error,
                 class_repo,
                 class_repo_con,
             ) = classification_report_calculation(cm, val)
+            for i in range(len(val)):
+                val[i] = white(val[i])
             # Concat The Classes with Confusion Matrix
             data1: list = [val] + cm
             # Preparing The Rate/Score Table
             data2: list = [
                 [
                     "",
-                    "Rate (Score)",
+                    white("Rate (Score)"),
                 ],
                 [
-                    "Accuracy",
+                    white("Accuracy"),
                     (
-                        "Correct      "
-                        + "Sum Of "
-                        + yellow("Yellow")
-                        + " Values\n"
-                        + "_" * len("Correct")
-                        + " : "
-                        + "_" * len("Sum Of Yellow And Red Values")
-                        + "  OR  1 - Error "
-                        + " =  "
-                        + f"{round(accuracy, 2)}"
-                        + "\n\n Total    Sum Of "
-                        + yellow("Yellow")
-                        + " And "
-                        + red("Red")
-                        + " Values"
-                    )
-                    if detail
-                    else round(accuracy, 2),
+                        (
+                            white("Correct      Sum Of ")
+                            + yellow("Yellow")
+                            + white(" Values")
+                            + "\n"
+                            + white("_" * len("Correct"))
+                            + white(" : ")
+                            + white("_" * len("Sum Of Yellow And Red Values"))
+                            + white("  OR  1 - Error ")
+                            + white(" =  ")
+                            + cyan(f"{round(accuracy, 2)}")
+                            + "\n\n"
+                            + white(" Total    Sum Of ")
+                            + yellow("Yellow")
+                            + white(" And ")
+                            + red("Red")
+                            + white(" Values")
+                        )
+                        if detail
+                        else cyan(f"{round(accuracy, 2)}")
+                    ),
                 ],
                 [
-                    "Error",
+                    white("Error"),
                     (
-                        "Wrong        "
-                        + "Sum Of "
-                        + red("Red")
-                        + " Values\n"
-                        + "_" * len("Wrong")
-                        + " : "
-                        + "_" * len("Sum Of Yellow And Red Values")
-                        + "  OR  1 - Accuracy "
-                        + " =  "
-                        + f"{round(error, 2)}"
-                        + "\n\nTotal   Sum Of "
-                        + yellow("Yellow")
-                        + " And "
-                        + red("Red")
-                        + " Values"
-                    )
-                    if detail
-                    else round(error, 2),
+                        (
+                            white("Wrong        Sum Of ")
+                            + red("Red")
+                            + white(" Values")
+                            + "\n"
+                            + white("_" * len("Wrong"))
+                            + white(" : ")
+                            + white("_" * len("Sum Of Yellow And Red Values"))
+                            + white("  OR  1 - Accuracy ")
+                            + white(" =  ")
+                            + cyan(f"{round(error, 2)}")
+                            + "\n\n"
+                            + white("Total   Sum Of ")
+                            + yellow("Yellow")
+                            + white(" And ")
+                            + red("Red")
+                            + white(" Values")
+                        )
+                        if detail
+                        else cyan(f"{round(error, 2)}")
+                    ),
                 ],
             ]
             # Concat The header Row With The Classification Report Matrix
             data3: list = (
-                [["", "Precision (P)", "Recall (R)",
-                  "F1-Score (F)", "Support (S)"]]
+                [
+                    [
+                        "",
+                        white("Precision (P)"),
+                        white("Recall (R)"),
+                        white("F1-Score (F)"),
+                        white("Support (S)"),
+                    ]
+                ]
                 + class_repo
                 + class_repo_con
             )
             # Printing All Data
-            print("\nConfusion Matrix : \n" + "_" *
-                  len("Confusion Matrix") + "\n")
+            print(
+                "\n"
+                + white("Confusion Matrix : ")
+                + "\n"
+                + white("_" * len("Confusion Matrix"))
+                + "\n"
+            )
             print(tabulate(data1, headers="firstrow", tablefmt="fancy_grid") + "\n")
             if detail:
                 print(yellow("Yellow"), end=" ")
                 print(
-                    " : Not None Correct Values / True Positive (TP) OR True Negative (TN)"
+                    white(
+                        " : Not None Correct Values / True Positive (TP) OR True Negative (TN)"
+                    )
                 )
                 print(red("Red"), end=" ")
                 print(
-                    "    : Not None Wrong Values / False Positive (FP) OR False Negative (FN)"
+                    white(
+                        "    : Not None Wrong Values / False Positive (FP) OR False Negative (FN)"
+                    )
                 )
                 print(green("Green"), end=" ")
-                print("  : None Correct Values")
+                print(white("  : None Correct Values"))
                 print(blue("Blue"), end=" ")
-                print("   : None Wrong Values\n")
+                print(white("   : None Wrong Values") + "\n")
             print(tabulate(data2, headers="firstrow", tablefmt="fancy_grid") + "\n")
             print(
-                "\nClassification Report : \n"
-                + "_" * len("Classification Report")
+                "\n"
+                + white("Classification Report : ")
+                + "\n"
+                + white("_" * len("Classification Report"))
                 + "\n"
             )
             print(tabulate(data3, headers="firstrow", tablefmt="fancy_grid") + "\n")
             if detail:
                 print(
-                    "Precision    : "
+                    white("Precision    : ")
                     + yellow("Yellow")
-                    + " Value / Sum Of "
+                    + white(" Value / Sum Of ")
                     + yellow("Yellow")
-                    + " Value Column\n"
+                    + white(" Value Column")
+                    + "\n"
                 )
                 print(
-                    "Recall       : "
+                    white("Recall       : ")
                     + yellow("Yellow")
-                    + " Value / Sum Of "
+                    + white(" Value / Sum Of ")
                     + yellow("Yellow")
-                    + " Value Row\n"
+                    + white(" Value Row")
+                    + "\n"
+                )
+                print(
+                    white(
+                        "F1-Score     : (2 x Precision x Recall) / (Precision + Recall)"
+                    )
+                    + "\n"
                 )
+                print(white("Support      : Sum Of Each Row") + "\n")
+                print(white("Macro Avg    :") + "\n")
                 print(
-                    "F1-Score     : (2 x Precision x Recall) / (Precision + Recall)\n"
+                    white(
+                        "               Precision : (Sum Of Precision Column) / Classes Count"
+                    )
+                    + "\n"
                 )
-                print("Support      : Sum Of Each Row\n")
-                print("Macro Avg    :\n")
                 print(
-                    "               Precision : (Sum Of Precision Column) / Classes Count\n"
+                    white(
+                        "               Recall    : (Sum Of Recall Column) / Classes Count"
+                    )
+                    + "\n"
+                )
+                print(
+                    white(
+                        "               F1-Score  : (Sum Of F1-Score Column) / Classes Count"
+                    )
+                    + "\n"
                 )
                 print(
-                    "               Recall    : (Sum Of Recall Column) / Classes Count\n"
+                    white("               Support   : Total (Sum Of All Matrix)") + "\n"
                 )
+                print(white("Weighted Avg :") + "\n")
                 print(
-                    "               F1-Score  : (Sum Of F1-Score Column) / Classes Count\n"
+                    white(
+                        "               Precision : (Sum Of (Precision x support)) / Total (Sum Of All Matrix)"
+                    )
+                    + "\n"
                 )
-                print("               Support   : Total (Sum Of All Matrix)\n")
-                print("Weighted Avg :\n")
                 print(
-                    "               Precision : (Sum Of (Precision x support)) / Total (Sum Of All Matrix)\n"
+                    white(
+                        "               Recall    : (Sum Of (Recall x Support)) / Total (Sum Of All Matrix)"
+                    )
+                    + "\n"
                 )
                 print(
-                    "               Recall    : (Sum Of (Recall x Support)) / Total (Sum Of All Matrix)\n"
+                    white(
+                        "               F1-Score  : (Sum Of (F1-Score x Support)) / Total (Sum Of All Matrix)"
+                    )
+                    + "\n"
                 )
                 print(
-                    "               F1-Score  : (Sum Of (F1-Score x Support)) / Total (Sum Of All Matrix)\n"
+                    white("               Support   : Total (Sum Of All Matrix)") + "\n"
                 )
-                print("               Support   : Total (Sum Of All Matrix)\n")
                 print(
-                    "Note : All Real Numbers Are Rounded With Two Digits After The Comma"
+                    white(
+                        "Note : All Real Numbers Are Rounded With Two Digits After The Comma"
+                    )
                 )
         return cmc
     else:
         # Printing Error Msg
-        print(
+        raise TypeError(
             "The List Of Original Values And The List Of Predicted Values Are Not Of The Same Length :("
         )
 
 
 def printConfMat(
     y_or_predicted_y: list,
     predicted_y_or_y: list,
@@ -1425,16 +1677,15 @@
                 pass
             else:
                 fn = 2
         except NameError as e1:
             fn = 2
         if len(conf_mat) == 0:
             # Calculating The Confusion Matrix
-            cm, val = control(y_or_predicted_y,
-                              predicted_y_or_y, classes_names, fn)
+            cm, val = control(y_or_predicted_y, predicted_y_or_y, classes_names, fn)
         else:
             if type(conf_mat) != list:
                 # Puting The Confusion Matrix Directely
                 cm: list = list(conf_mat)
                 # Converting The Rows Into A List Data Type
                 for i in range(len(cm)):
                     cm[i] = list(cm[i])
@@ -1446,27 +1697,29 @@
         # Creating The Confusion Matrix Heatmap (Png Format) In Working Direcory
         if detail:
             imshow_config(cm, val, True)
         else:
             imshow_config(cm, val, True, False)
         if len(cm) == 0:
             # Print Msg
-            print("No HTML File Generated :(")
+            print(cyan("No HTML File Generated :("))
         elif len(cm) == 1:
             # Preparing Confusion Matrix
             data1: list = [
                 [
                     "",
                     f"Positive If Positive OR Negative If Negative ({val[0]})",
                 ],
                 [
                     f"Positive OR Negative ({val[0]})",
-                    f"True Positive OR True Negative \n\n           TP OR TN : \n\n              {cm[0][0]}"
-                    if detail
-                    else cm[0][0],
+                    (
+                        f"True Positive OR True Negative \n\n           TP OR TN : \n\n              {cm[0][0]}"
+                        if detail
+                        else cm[0][0]
+                    ),
                 ],
             ]
             # Preparing The Rate/Score Table
             data2: list = [
                 [
                     "",
                     "Rate (Score)",
@@ -1517,27 +1770,25 @@
                     tabulate(data1, headers="firstrow", tablefmt="html")
                     + "\n<br>\n<br>\n"
                 )
                 file.write(
                     tabulate(data2, headers="firstrow", tablefmt="html")
                     + "\n<br>\n<br>\n"
                 )
-                file.write(
-                    "<u><b>Classification Report</b></u> :\n<br>\n<br>\n")
+                file.write("<u><b>Classification Report</b></u> :\n<br>\n<br>\n")
                 file.write(
                     tabulate(data3, headers="firstrow", tablefmt="html")
                     + "\n<br>\n<br>\n"
                 )
-                file.write(
-                    "<u><b>Confusion Matrix Display</b></u> : \n<br>\n<br>\n")
+                file.write("<u><b>Confusion Matrix Display</b></u> : \n<br>\n<br>\n")
                 file.write('<img src="conf_Mat.png" alt="Confusion Matrix">\n')
             # Update HTML Code
             update_html()
             # Print The Success Msg
-            print("HTML File Generated Successfully :)")
+            print(cyan("HTML File Generated Successfully :)"))
             # Opening HTML Page
             wb("conf_Mat.html")
         elif len(cm) == 2:
             (
                 accuracy,
                 error,
                 precision,
@@ -1556,165 +1807,196 @@
                     "Predicted Positive (PP)",
                     "Predicted Negative (PN)",
                     "",
                 ],
                 [
                     "Actual Positive (P)",
                     f"True Positive (TP) : {cm[1][1]}" if detail else cm[1][1],
-                    f"False Negative (FN) / Type II Error (Missed) : {cm[1][0]}"
-                    if detail
-                    else cm[1][0],
+                    (
+                        f"False Negative (FN) / Type II Error (Missed) : {cm[1][0]}"
+                        if detail
+                        else cm[1][0]
+                    ),
                 ],
                 [
                     "Actual Negative (N)",
-                    f"False Positive (FP) Type I Error (Wrong) : {cm[0][1]}"
-                    if detail
-                    else cm[0][1],
+                    (
+                        f"False Positive (FP) Type I Error (Wrong) : {cm[0][1]}"
+                        if detail
+                        else cm[0][1]
+                    ),
                     f"True Negative (TN) : {cm[0][0]}" if detail else cm[0][0],
                 ],
             ]
             # Preparing The Rate/Score Table
             data2: list = [
                 [
                     "",
                     "Rate (Score)",
                 ],
                 [
                     "Accuracy",
-                    f"Correct / Total : (TP + TN) / (TP + FP + FN + TN) = {round(accuracy, 2)}"
-                    if detail
-                    else round(accuracy, 2),
+                    (
+                        f"Correct / Total : (TP + TN) / (TP + FP + FN + TN) = {round(accuracy, 2)}"
+                        if detail
+                        else round(accuracy, 2)
+                    ),
                 ],
                 [
                     "Error",
-                    f"Wrong / Total : (FP + FN) / (TP + FP + FN + TN) = {error}"
-                    if detail
-                    else error,
+                    (
+                        f"Wrong / Total : (FP + FN) / (TP + FP + FN + TN) = {error}"
+                        if detail
+                        else error
+                    ),
                 ],
             ]
             # Preparing Classification Report
             data3: list = [
                 [
                     "Precision (P)",
                     "Recall (R)",
                     "F1-Score (F)",
                     "Support (S)",
                 ],
                 [
                     f"Positive ({val[1]})",
-                    f"P1 (PPV): TP / (TP + FP) = {round(precision, 2)}"
-                    if detail
-                    else round(precision, 2),
-                    f"R1 (Sensitivity): TP / (TP + FN) = {round(recall, 2)}"
-                    if detail
-                    else round(recall, 2),
-                    f"F1 : (2 x P1 x R1) / (P1 + R1) = {round(f_score_1, 2)}"
-                    if detail
-                    else round(f_score_1, 2),
+                    (
+                        f"P1 (PPV): TP / (TP + FP) = {round(precision, 2)}"
+                        if detail
+                        else round(precision, 2)
+                    ),
+                    (
+                        f"R1 (Sensitivity): TP / (TP + FN) = {round(recall, 2)}"
+                        if detail
+                        else round(recall, 2)
+                    ),
+                    (
+                        f"F1 : (2 x P1 x R1) / (P1 + R1) = {round(f_score_1, 2)}"
+                        if detail
+                        else round(f_score_1, 2)
+                    ),
                     f"S1 : TP + FN = {support_1}" if detail else support_1,
                 ],
                 [
                     f"Negative ({val[0]})",
-                    f"P0 (NPV): TN / (TN + FN) = {round(negative_precision, 2)}"
-                    if detail
-                    else round(negative_precision, 2),
-                    f"R0 (Specificity): TN / (TN + FP) = {round(specificity, 2)}"
-                    if detail
-                    else round(specificity, 2),
-                    f"F0 : (2 x P0 x R0) /  (P0 + R0) = {round(f_score_0, 2)}"
-                    if detail
-                    else round(f_score_0, 2),
+                    (
+                        f"P0 (NPV): TN / (TN + FN) = {round(negative_precision, 2)}"
+                        if detail
+                        else round(negative_precision, 2)
+                    ),
+                    (
+                        f"R0 (Specificity): TN / (TN + FP) = {round(specificity, 2)}"
+                        if detail
+                        else round(specificity, 2)
+                    ),
+                    (
+                        f"F0 : (2 x P0 x R0) /  (P0 + R0) = {round(f_score_0, 2)}"
+                        if detail
+                        else round(f_score_0, 2)
+                    ),
                     f"S0 : FP + TN = {support_0}" if detail else support_0,
                 ],
                 [
                     "Macro Avg",
-                    f"(P1 + P0) / 2 = {round((precision + negative_precision)/2, 2)}"
-                    if detail
-                    else round((precision + negative_precision) / 2, 2),
-                    f"(R1 + R0) / 2 = {round((recall + specificity)/2, 2)}"
-                    if detail
-                    else round((recall + specificity) / 2, 2),
-                    f"(F1 + F0) / 2 = {round((f_score_1 + f_score_0)/2, 2)}"
-                    if detail
-                    else round((f_score_1 + f_score_0) / 2, 2),
-                    f"TS = {support_0 + support_1}"
-                    if detail
-                    else support_0 + support_1,
+                    (
+                        f"(P1 + P0) / 2 = {round((precision + negative_precision)/2, 2)}"
+                        if detail
+                        else round((precision + negative_precision) / 2, 2)
+                    ),
+                    (
+                        f"(R1 + R0) / 2 = {round((recall + specificity)/2, 2)}"
+                        if detail
+                        else round((recall + specificity) / 2, 2)
+                    ),
+                    (
+                        f"(F1 + F0) / 2 = {round((f_score_1 + f_score_0)/2, 2)}"
+                        if detail
+                        else round((f_score_1 + f_score_0) / 2, 2)
+                    ),
+                    (
+                        f"TS = {support_0 + support_1}"
+                        if detail
+                        else support_0 + support_1
+                    ),
                 ],
                 [
                     "Weighted Avg",
-                    f"W1 / TS = {round(((precision * support_1) + (negative_precision * support_0))/(support_0 + support_1), 2)}"
-                    if detail
-                    else round(
-                        ((precision * support_1) + (negative_precision * support_0))
-                        / (support_0 + support_1),
-                        2,
-                    ),
-                    f"W2 / TS = {round(((recall * support_1) + (specificity * support_0))/(support_0 + support_1), 2)}"
-                    if detail
-                    else round(
-                        ((recall * support_1) + (specificity * support_0))
-                        / (support_0 + support_1),
-                        2,
-                    ),
-                    f"W3 / TS = {round(((f_score_1 * support_1) + (f_score_0 * support_0))/(support_1 + support_0),2)}"
-                    if detail
-                    else round(
-                        ((f_score_1 * support_1) + (f_score_0 * support_0))
-                        / (support_1 + support_0),
-                        2,
-                    ),
-                    f"TS = {support_0 + support_1}"
-                    if detail
-                    else support_0 + support_1,
+                    (
+                        f"W1 / TS = {round(((precision * support_1) + (negative_precision * support_0))/(support_0 + support_1), 2)}"
+                        if detail
+                        else round(
+                            ((precision * support_1) + (negative_precision * support_0))
+                            / (support_0 + support_1),
+                            2,
+                        )
+                    ),
+                    (
+                        f"W2 / TS = {round(((recall * support_1) + (specificity * support_0))/(support_0 + support_1), 2)}"
+                        if detail
+                        else round(
+                            ((recall * support_1) + (specificity * support_0))
+                            / (support_0 + support_1),
+                            2,
+                        )
+                    ),
+                    (
+                        f"W3 / TS = {round(((f_score_1 * support_1) + (f_score_0 * support_0))/(support_1 + support_0),2)}"
+                        if detail
+                        else round(
+                            ((f_score_1 * support_1) + (f_score_0 * support_0))
+                            / (support_1 + support_0),
+                            2,
+                        )
+                    ),
+                    (
+                        f"TS = {support_0 + support_1}"
+                        if detail
+                        else support_0 + support_1
+                    ),
                 ],
             ]
             # Writing All Data
             with open("conf_Mat.html", "w") as file:
                 file.write("<u><b>Confusion Matrix</b></u> : \n<br>\n<br>\n")
                 file.write(
                     tabulate(data1, headers="firstrow", tablefmt="html")
                     + "\n<br>\n<br>\n"
                 )
                 file.write(
                     tabulate(data2, headers="firstrow", tablefmt="html")
                     + "\n<br>\n<br>\n"
                 )
-                file.write(
-                    "<u><b>Classification Report</b></u> : \n<br>\n<br>\n")
+                file.write("<u><b>Classification Report</b></u> : \n<br>\n<br>\n")
                 file.write(
                     tabulate(data3, headers="firstrow", tablefmt="html")
                     + "\n<br>\n<br>\n"
                 )
                 if detail:
                     file.write(
                         "<u><b>PPV</b></u> : Positive Predictive Value\n<br>\n<br>\n"
                     )
                     file.write(
                         "<u><b>NPV</b></u> : Negative Predictive Value\n<br>\n<br>\n"
                     )
-                    file.write(
-                        "<b>W1</b> = (P1 x S1) + (P0 x S0)\n<br>\n<br>\n")
-                    file.write(
-                        "<b>W2</b> = (R1 x S1) + (R0 x S0)\n<br>\n<br>\n")
-                    file.write(
-                        "<b>W3</b> = (F1 x S1) + (F0 x S0)\n<br>\n<br>\n")
+                    file.write("<b>W1</b> = (P1 x S1) + (P0 x S0)\n<br>\n<br>\n")
+                    file.write("<b>W2</b> = (R1 x S1) + (R0 x S0)\n<br>\n<br>\n")
+                    file.write("<b>W3</b> = (F1 x S1) + (F0 x S0)\n<br>\n<br>\n")
                     file.write(
                         "<b>TS</b> : Total Support = S1 + S0\n<br>\n<br>\n<br>\n"
                     )
                     file.write(
                         "<u><b>Note</b></u> : All Real Numbers Are Rounded With Two Digits After The Comma\n<br>\n<br>\n<br>\n<br>"
                     )
-                file.write(
-                    "<u><b>Confusion Matrix Display</b></u> : \n<br>\n<br>\n")
+                file.write("<u><b>Confusion Matrix Display</b></u> : \n<br>\n<br>\n")
                 file.write('<img src="conf_Mat.png" alt="Confusion Matrix">\n')
             # Update HTML Code
             update_html()
             # Print The Success Msg
-            print("HTML File Generated Successfully :)")
+            print(cyan("HTML File Generated Successfully :)"))
             # Opening HTML Page
             wb("conf_Mat.html")
         else:
             (
                 accuracy,
                 error,
                 class_repo,
@@ -1726,45 +2008,47 @@
             data2: list = [
                 [
                     "",
                     "Rate (Score)",
                 ],
                 [
                     "Accuracy",
-                    f"Correct / Total : Sum Of Left Diagonal Values / Total (Sum Of All Matrix) OR  1 - Error = {round(accuracy, 2)}"
-                    if detail
-                    else round(accuracy, 2),
+                    (
+                        f"Correct / Total : Sum Of Left Diagonal Values / Total (Sum Of All Matrix) OR  1 - Error = {round(accuracy, 2)}"
+                        if detail
+                        else round(accuracy, 2)
+                    ),
                 ],
                 [
                     "Error",
-                    f"Wrong / Total : (Total (Sum Of All Matrix) - Sum Of Left Diagonal Values) / Total (Sum Of All Matrix) OR  1 - Accuracy = {round(error, 2)}"
-                    if detail
-                    else round(error, 2),
+                    (
+                        f"Wrong / Total : (Total (Sum Of All Matrix) - Sum Of Left Diagonal Values) / Total (Sum Of All Matrix) OR  1 - Accuracy = {round(error, 2)}"
+                        if detail
+                        else round(error, 2)
+                    ),
                 ],
             ]
             # Concat The header Row With The Classification Report Matrix
             data3: list = (
-                [["", "Precision (P)", "Recall (R)",
-                  "F1-Score (F)", "Support (S)"]]
+                [["", "Precision (P)", "Recall (R)", "F1-Score (F)", "Support (S)"]]
                 + class_repo
                 + class_repo_con
             )
             # Writing All Data
             with open("conf_Mat.html", "w") as file:
                 file.write("<u><b>Confusion Matrix</b></u> : \n<br>\n<br>\n")
                 file.write(
                     tabulate(data1, headers="firstrow", tablefmt="html")
                     + "\n<br>\n<br>\n"
                 )
                 file.write(
                     tabulate(data2, headers="firstrow", tablefmt="html")
                     + "\n<br>\n<br>\n"
                 )
-                file.write(
-                    "<u><b>Classification Report<b></u> :\n<br>\n<br>\n")
+                file.write("<u><b>Classification Report<b></u> :\n<br>\n<br>\n")
                 file.write(
                     tabulate(data3, headers="firstrow", tablefmt="html")
                     + "\n<br>\n<br>\n"
                 )
                 if detail:
                     file.write(
                         "<b><u>Precision</u></b> "
@@ -1773,15 +2057,15 @@
                     )
                     file.write(
                         "<u><b>Recall</b></u>    "
                         + "&nbsp;" * 8
                         + ": Sum Of True Prediction For Each Value (Left Diagonal) / Sum Of Value Row\n<br>\n<br>\n"
                     )
                     file.write(
-                        '<iframe src="https://drive.google.com/file/d/1DVa-k7XycuOyGY5nHwHhFKNCYBJ2qMEb/preview" width="538" height="477" allow="autoplay" frameborder="0"></iframe>\n<br>\n<br>\n'
+                        f'<img src="{path.dirname(path.abspath(__file__))}/conf_Mat_Ex.png" alt="conf_Mat_Ex">\n<br>\n<br>\n'
                     )
                     file.write(
                         "<u><b>F1-Score</b></u>  "
                         + "&nbsp;" * 3
                         + ": (2 x Precision x Recall) / (Precision + Recall)\n<br>\n<br>\n"
                     )
                     file.write(
@@ -1830,23 +2114,27 @@
                         + "Support   "
                         + "&nbsp;" * 2
                         + ": Total (Sum Of All Matrix)\n<br>\n<br>\n<br>\n"
                     )
                     file.write(
                         "<u><b>Note</b></u> : All Real Numbers Are Rounded With Two Digits After The Comma\n<br>\n<br>\n<br>\n<br>\n"
                     )
-                file.write(
-                    "<u><b>Confusion Matrix Display</b></u> : \n<br>\n<br>\n")
+                file.write("<u><b>Confusion Matrix Display</b></u> : \n<br>\n<br>\n")
                 file.write('<img src="conf_Mat.png" alt="Confusion Matrix">\n')
             # Update HTML Code
             update_html()
             # Print The Success Msg
-            print("HTML File Generated Successfully :)")
+            print(cyan("HTML File Generated Successfully :)"))
             # Opening HTML Page
             wb("conf_Mat.html")
+    else:
+        # Printing Error Msg
+        raise TypeError(
+            "The List Of Original Values And The List Of Predicted Values Are Not Of The Same Length :("
+        )
 
 
 def confMatToHtml(
     y_or_predicted_y: list = [],
     predicted_y_or_y: list = [],
     *,
     classes_names: list = [],
@@ -1858,7 +2146,15 @@
     conf_mat_to_html(
         y_or_predicted_y,
         predicted_y_or_y,
         classes_names=classes_names,
         conf_mat=conf_mat,
         detail=detail,
     )
+
+
+def main() -> None:
+    print("conf-mat")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `conf-mat-1.0.4/conf_mat.egg-info/PKG-INFO` & `conf-mat-1.0.5/conf_mat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: conf-mat
-Version: 1.0.4
-Summary: Sophisticate Open Confusion Matrix
+Version: 1.0.5
+Summary: Sophisticate Confusion Matrix
 Home-page: https://pypi.org/project/conf-mat/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: confusion matrix
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -62,70 +62,73 @@
 conf_mat_to_html(y_true, y_pred, classes_names=[False, True])
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═════════════════════╤═══════════════════════════╤═══════════════════════════╕
 │ Classes             │ Predicted Positive (PP)   │ Predicted Negative (PN)   │
 ╞═════════════════════╪═══════════════════════════╪═══════════════════════════╡
-│ Actual Positive (P) │ True Positive (TP) : 273  │ False Negative (FN) : 244 │
+│ Actual Positive (P) │ True Positive (TP) : 240  │ False Negative (FN) : 241 │
 │                     │                           │ Type II Error (Missed)    │
 ├─────────────────────┼───────────────────────────┼───────────────────────────┤
-│ Actual Negative (N) │ False Positive (FP) : 229 │ True Negative (TN) : 254  │
+│ Actual Negative (N) │ False Positive (FP) : 259 │ True Negative (TN) : 260  │
 │                     │ Type I Error (Wrong)      │                           │
 ╘═════════════════════╧═══════════════════════════╧═══════════════════════════╛
 
-╒══════════╤══════════════════════════════════════════════════════╕
-│          │ Rate (Score)                                         │
-╞══════════╪══════════════════════════════════════════════════════╡
-│ Accuracy │ Correct        TP + TN                               │
-│          │ _______ : _________________  OR  1 - Error  =  0.53  │
-│          │                                                      │
-│          │  Total    TP + FP + FN + TN                          │
-├──────────┼──────────────────────────────────────────────────────┤
-│ Error    │ Wrong        FP + FN                                 │
-│          │ _____ : _________________  OR  1 - Accuracy  =  0.47 │
-│          │                                                      │
-│          │ Total   TP + FP + FN + TN                            │
-╘══════════╧══════════════════════════════════════════════════════╛
+╒══════════╤═════════════════════════════════════════════════════╕
+│          │ Rate (Score)                                        │
+╞══════════╪═════════════════════════════════════════════════════╡
+│ Accuracy │ Correct        TP + TN                              │
+│          │ _______ : _________________  OR  1 - Error  =  0.5  │
+│          │                                                     │
+│          │  Total    TP + FP + FN + TN                         │
+├──────────┼─────────────────────────────────────────────────────┤
+│ Error    │ Wrong        FP + FN                                │
+│          │ _____ : _________________  OR  1 - Accuracy  =  0.5 │
+│          │                                                     │
+│          │ Total   TP + FP + FN + TN                           │
+╘══════════╧═════════════════════════════════════════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════════╤═════════════════╤════════════════════╤═════════════════════╤════════════════╕
 │                  │ Precision (P)   │ Recall (R)         │ F1-Score (F)        │ Support (S)    │
 ╞══════════════════╪═════════════════╪════════════════════╪═════════════════════╪════════════════╡
 │ Positive (True)  │ P1 (PPV):       │ R1 (Sensitivity):  │ F1 :                │ S1 :           │
 │                  │                 │                    │                     │                │
 │                  │   TP            │   TP               │ 2 x P1 x R1         │                │
-│                  │ _______  = 0.54 │ _______  = 0.53    │ ___________  = 0.54 │  TP + FN = 517 │
+│                  │ _______  = 0.48 │ _______  = 0.5     │ ___________  = 0.49 │  TP + FN = 481 │
 │                  │                 │                    │                     │                │
 │                  │ TP + FP         │ TP + FN            │   P1 + R1           │                │
 ├──────────────────┼─────────────────┼────────────────────┼─────────────────────┼────────────────┤
 │ Negative (False) │ P0 (NPV):       │ R0 (Specificity):  │ F0 :                │ S0 :           │
 │                  │                 │                    │                     │                │
 │                  │   TN            │   TN               │ 2 x P0 x R0         │                │
-│                  │ _______  = 0.51 │ _______  = 0.53    │ ___________  = 0.52 │  FP + TN = 483 │
+│                  │ _______  = 0.52 │ _______  = 0.5     │ ___________  = 0.51 │  FP + TN = 519 │
 │                  │                 │                    │                     │                │
 │                  │ TN + FN         │ TN + FP            │   P0 + R0           │                │
 ├──────────────────┼─────────────────┼────────────────────┼─────────────────────┼────────────────┤
 │ Macro Avg        │ P1 + P0         │ R1 + R0            │ F1 + F0             │ TS = 1000      │
-│                  │ _______  = 0.53 │ _______  = 0.53    │ _______  = 0.53     │                │
+│                  │ _______  = 0.5  │ _______  = 0.5     │ _______  = 0.5      │                │
 │                  │                 │                    │                     │                │
 │                  │    2            │    2               │    2                │                │
 ├──────────────────┼─────────────────┼────────────────────┼─────────────────────┼────────────────┤
 │ Weighted Avg     │ W1              │ W2                 │ W3                  │ TS = 1000      │
-│                  │ __  = 0.53      │ __  = 0.53         │ __  = 0.53          │                │
+│                  │ __  = 0.5       │ __  = 0.5          │ __  = 0.5           │                │
 │                  │                 │                    │                     │                │
 │                  │ TS              │ TS                 │ TS                  │                │
 ╘══════════════════╧═════════════════╧════════════════════╧═════════════════════╧════════════════╛
 
 PPV : Positive Predictive Value
 
 NPV : Negative Predictive Value
@@ -138,14 +141,29 @@
 
 TS : Total Support = S1 + S0
 
 Note : All Real Numbers Are Rounded With Two Digits After The Comma
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1IA3ke21FHXBx7hydamouMhS9zvjHcy9B/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0001/
+
+
 #### You Can Plot, Generate HTML Page For Confusion Matrix And Classification Report Directly From One Calculation 
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import print_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -195,52 +213,70 @@
 conf_mat_to_html(conf_mat=cm, classes_names=[False, True], detail=False)
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═════════════════════╤═══════════════════════════╤═══════════════════════════╕
 │ Classes             │   Predicted Positive (PP) │   Predicted Negative (PN) │
 ╞═════════════════════╪═══════════════════════════╪═══════════════════════════╡
-│ Actual Positive (P) │                       261 │                       271 │
+│ Actual Positive (P) │                       239 │                       246 │
 ├─────────────────────┼───────────────────────────┼───────────────────────────┤
-│ Actual Negative (N) │                       240 │                       228 │
+│ Actual Negative (N) │                       252 │                       263 │
 ╘═════════════════════╧═══════════════════════════╧═══════════════════════════╛
 
 ╒══════════╤════════════════╕
 │          │   Rate (Score) │
 ╞══════════╪════════════════╡
-│ Accuracy │           0.49 │
+│ Accuracy │            0.5 │
 ├──────────┼────────────────┤
-│ Error    │           0.51 │
+│ Error    │            0.5 │
 ╘══════════╧════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════════╤═════════════════╤══════════════╤════════════════╤═══════════════╕
 │                  │   Precision (P) │   Recall (R) │   F1-Score (F) │   Support (S) │
 ╞══════════════════╪═════════════════╪══════════════╪════════════════╪═══════════════╡
-│ Positive (True)  │            0.52 │         0.49 │           0.51 │           532 │
+│ Positive (True)  │            0.49 │         0.49 │           0.49 │           485 │
 ├──────────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Negative (False) │            0.46 │         0.49 │           0.47 │           468 │
+│ Negative (False) │            0.52 │         0.51 │           0.51 │           515 │
 ├──────────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Macro Avg        │            0.49 │         0.49 │           0.49 │          1000 │
+│ Macro Avg        │            0.5  │         0.5  │           0.5  │          1000 │
 ├──────────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Weighted Avg     │            0.49 │         0.49 │           0.49 │          1000 │
+│ Weighted Avg     │            0.5  │         0.5  │           0.5  │          1000 │
 ╘══════════════════╧═════════════════╧══════════════╧════════════════╧═══════════════╛
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1L42AslXk-JRHNYpzMLXoRhtuhVWkTibC/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0011/
+
+
 #### You Can Plot And Generate HTML Page For Confusion Matrix Directly From One Calculation And Without Print Confusion Matrix And Classification Report
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import calc_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -263,17 +299,35 @@
 conf_mat_to_html(conf_mat=cm, classes_names=[False, True], detail=False)
 ```
 
 
 ### Output
 
 
+#### calc_conf_mat Output
+
+
+```bash
+[[243, 242], [256, 259]]
+```
+
+
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1tLBhU1RIlIRFX5YR-nXJMljV_sOVm_SH/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
 ```bash
-[[236, 253], [255, 256]]
+HTML File Generated Successfully :)
 ```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0101/
 
 
 ### For Multi Classification
 
 
 ```python
 from numpy.random import randint
@@ -301,91 +355,94 @@
     'C1', 'C2', 'C3', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9', 'C10'])
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═══════════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤═══════╕
 │ Classes   │   C1 │   C2 │   C3 │   C4 │   C5 │   C6 │   C7 │   C8 │   C9 │   C10 │
 ╞═══════════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪═══════╡
-│ C1        │    5 │   17 │   12 │   11 │   12 │   13 │    6 │   13 │   10 │     7 │
+│ C1        │    8 │    9 │   10 │    7 │   13 │   10 │    9 │   12 │   15 │    11 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C2        │   10 │    6 │   10 │   11 │   13 │   11 │   13 │    8 │   11 │    11 │
+│ C2        │    9 │    6 │    5 │   15 │   10 │   15 │   13 │   10 │   12 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C3        │    6 │    6 │   12 │    8 │   10 │    5 │   11 │    8 │    7 │    11 │
+│ C3        │   14 │    5 │    8 │   10 │   17 │   10 │   10 │    6 │   17 │    12 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C4        │   14 │   13 │   10 │    8 │    9 │    5 │   12 │   14 │    9 │     7 │
+│ C4        │    8 │   10 │    3 │   11 │    7 │    7 │    9 │    8 │    7 │     7 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C5        │   12 │    9 │   15 │    5 │    8 │    9 │    6 │    8 │   10 │    10 │
+│ C5        │    5 │   13 │    7 │   11 │    8 │   13 │    7 │   10 │    6 │     8 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C6        │   12 │   16 │   15 │    9 │   10 │    8 │   10 │   11 │   11 │    12 │
+│ C6        │    9 │   12 │   13 │    9 │   14 │    9 │    8 │    8 │   13 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C7        │   12 │    9 │   12 │   14 │   12 │    6 │   13 │   13 │    7 │    14 │
+│ C7        │   14 │   11 │   11 │   20 │    6 │    6 │    9 │    9 │   10 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C8        │    6 │   11 │    7 │   10 │   10 │   12 │    8 │   10 │    8 │    11 │
+│ C8        │   10 │   13 │    8 │   12 │   12 │    6 │   10 │    5 │   12 │    14 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C9        │   15 │    7 │    8 │    6 │    8 │    6 │    5 │    4 │   14 │    12 │
+│ C9        │   12 │    9 │   13 │    9 │    9 │    8 │   11 │   11 │    9 │     9 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C10       │   10 │   11 │   11 │   13 │    8 │   11 │   12 │   12 │    6 │    15 │
+│ C10       │   12 │   13 │   11 │   12 │   10 │   14 │   11 │    4 │    6 │    11 │
 ╘═══════════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧═══════╛
 
 Yellow  : Not None Correct Values / True Positive (TP) OR True Negative (TN)
 Red     : Not None Wrong Values / False Positive (FP) OR False Negative (FN)
 Green   : None Correct Values
 Blue    : None Wrong Values
 
-╒══════════╤════════════════════════════════════════════════════════════════╕
-│          │ Rate (Score)                                                   │
-╞══════════╪════════════════════════════════════════════════════════════════╡
-│ Accuracy │ Correct      Sum Of Yellow Values                              │
-│          │ _______ : ____________________________  OR  1 - Error  =  0.1  │
-│          │                                                                │
-│          │  Total    Sum Of Yellow And Red Values                         │
-├──────────┼────────────────────────────────────────────────────────────────┤
-│ Error    │ Wrong        Sum Of Red Values                                 │
-│          │ _____ : ____________________________  OR  1 - Accuracy  =  0.9 │
-│          │                                                                │
-│          │ Total   Sum Of Yellow And Red Values                           │
-╘══════════╧════════════════════════════════════════════════════════════════╛
+╒══════════╤═════════════════════════════════════════════════════════════════╕
+│          │ Rate (Score)                                                    │
+╞══════════╪═════════════════════════════════════════════════════════════════╡
+│ Accuracy │ Correct      Sum Of Yellow Values                               │
+│          │ _______ : ____________________________  OR  1 - Error  =  0.08  │
+│          │                                                                 │
+│          │  Total    Sum Of Yellow And Red Values                          │
+├──────────┼─────────────────────────────────────────────────────────────────┤
+│ Error    │ Wrong        Sum Of Red Values                                  │
+│          │ _____ : ____________________________  OR  1 - Accuracy  =  0.92 │
+│          │                                                                 │
+│          │ Total   Sum Of Yellow And Red Values                            │
+╘══════════╧═════════════════════════════════════════════════════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════╤═════════════════╤══════════════╤════════════════╤═══════════════╕
 │              │   Precision (P) │   Recall (R) │   F1-Score (F) │   Support (S) │
 ╞══════════════╪═════════════════╪══════════════╪════════════════╪═══════════════╡
-│ C1           │            0.05 │         0.05 │           0.05 │           106 │
+│ C1           │            0.08 │         0.08 │           0.08 │           104 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C2           │            0.06 │         0.06 │           0.06 │           104 │
+│ C2           │            0.06 │         0.06 │           0.06 │           105 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C3           │            0.11 │         0.14 │           0.12 │            84 │
+│ C3           │            0.09 │         0.07 │           0.08 │           109 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C4           │            0.08 │         0.08 │           0.08 │           101 │
+│ C4           │            0.09 │         0.14 │           0.11 │            77 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C5           │            0.08 │         0.09 │           0.08 │            92 │
+│ C5           │            0.08 │         0.09 │           0.08 │            88 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C6           │            0.09 │         0.07 │           0.08 │           114 │
+│ C6           │            0.09 │         0.09 │           0.09 │           105 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C7           │            0.14 │         0.12 │           0.12 │           112 │
+│ C7           │            0.09 │         0.08 │           0.09 │           106 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C8           │            0.1  │         0.11 │           0.1  │            93 │
+│ C8           │            0.06 │         0.05 │           0.05 │           102 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C9           │            0.15 │         0.16 │           0.16 │            85 │
+│ C9           │            0.08 │         0.09 │           0.09 │           100 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C10          │            0.14 │         0.14 │           0.14 │           109 │
+│ C10          │            0.11 │         0.11 │           0.11 │           104 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Macro Avg    │            0.1  │         0.1  │           0.1  │          1000 │
+│ Macro Avg    │            0.08 │         0.09 │           0.08 │          1000 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Weighted Avg │            0.1  │         0.1  │           0.1  │          1000 │
+│ Weighted Avg │            0.08 │         0.08 │           0.08 │          1000 │
 ╘══════════════╧═════════════════╧══════════════╧════════════════╧═══════════════╛
 
 Precision    : Yellow Value / Sum Of Yellow Value Column
 
 Recall       : Yellow Value / Sum Of Yellow Value Row
 
 F1-Score     : (2 x Precision x Recall) / (Precision + Recall)
@@ -412,14 +469,29 @@
 
                Support   : Total (Sum Of All Matrix)
 
 Note : All Real Numbers Are Rounded With Two Digits After The Comma
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1Gp0CcqZwwZdb8ZTELzfKciJasFGNyqTc/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/0111/
+
+
 #### You Can Plot, Generate HTML Page For Confusion Matrix And Classification Report Directly From One Calculation 
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import print_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -475,84 +547,102 @@
     'C1', 'C2', 'C3', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9', 'C10'], detail=False)
 ```
 
 
 ### Output
 
 
+#### print_conf_mat Output
+
+
 ```bash
 Confusion Matrix : 
 ________________
 
 ╒═══════════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤══════╤═══════╕
 │ Classes   │   C1 │   C2 │   C3 │   C4 │   C5 │   C6 │   C7 │   C8 │   C9 │   C10 │
 ╞═══════════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪══════╪═══════╡
-│ C1        │   10 │    5 │    7 │    7 │    8 │   10 │    9 │   10 │   12 │     8 │
+│ C1        │   10 │    5 │   15 │    6 │    9 │   12 │   13 │    5 │   12 │    13 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C2        │    7 │   14 │   14 │    9 │    9 │   13 │   14 │   11 │   14 │     7 │
+│ C2        │   13 │    5 │    9 │    6 │   13 │   11 │   12 │    5 │    6 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C3        │   13 │   12 │    5 │    9 │    6 │    8 │    9 │   10 │   14 │     8 │
+│ C3        │   11 │   16 │    8 │   10 │   12 │   15 │    7 │   11 │   10 │    12 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C4        │    6 │   11 │    9 │   18 │   11 │    7 │   10 │   11 │    6 │     7 │
+│ C4        │   10 │    9 │   10 │    7 │   15 │   13 │   12 │   11 │   11 │    11 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C5        │    9 │    5 │   11 │    9 │    7 │    8 │    8 │   20 │    9 │    10 │
+│ C5        │   10 │    9 │   12 │    8 │   13 │    7 │    7 │    7 │    9 │     7 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C6        │   12 │    5 │    8 │   11 │   11 │   12 │   14 │   14 │   11 │     7 │
+│ C6        │   14 │   13 │   14 │   11 │    6 │   11 │    8 │   13 │   11 │    13 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C7        │   13 │    8 │   10 │    7 │   10 │   12 │   15 │   10 │    8 │     8 │
+│ C7        │    9 │   11 │   11 │    9 │    9 │   12 │    9 │   10 │    9 │     9 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C8        │   10 │    5 │    6 │   14 │   11 │    9 │    9 │   10 │    4 │    13 │
+│ C8        │   10 │   11 │   12 │   10 │    7 │   10 │   14 │   10 │   13 │    11 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C9        │   11 │   13 │   10 │   10 │   13 │   10 │    8 │   12 │    9 │    15 │
+│ C9        │    8 │   14 │    9 │    8 │    9 │    7 │    9 │   11 │    9 │    10 │
 ├───────────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼──────┼───────┤
-│ C10       │   11 │   12 │   11 │   10 │    9 │    8 │    6 │   14 │   12 │    15 │
+│ C10       │    8 │   10 │    7 │    4 │    8 │   13 │    8 │    6 │    9 │    13 │
 ╘═══════════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧══════╧═══════╛
 
 ╒══════════╤════════════════╕
 │          │   Rate (Score) │
 ╞══════════╪════════════════╡
-│ Accuracy │           0.12 │
+│ Accuracy │           0.1  │
 ├──────────┼────────────────┤
-│ Error    │           0.89 │
+│ Error    │           0.91 │
 ╘══════════╧════════════════╛
 
 
 Classification Report : 
 _____________________
 
 ╒══════════════╤═════════════════╤══════════════╤════════════════╤═══════════════╕
 │              │   Precision (P) │   Recall (R) │   F1-Score (F) │   Support (S) │
 ╞══════════════╪═════════════════╪══════════════╪════════════════╪═══════════════╡
-│ C1           │            0.1  │         0.12 │           0.11 │            86 │
+│ C1           │            0.1  │         0.1  │           0.1  │           100 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C2           │            0.16 │         0.12 │           0.14 │           112 │
+│ C2           │            0.05 │         0.06 │           0.05 │            90 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C3           │            0.05 │         0.05 │           0.05 │            94 │
+│ C3           │            0.07 │         0.07 │           0.07 │           112 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C4           │            0.17 │         0.19 │           0.18 │            96 │
+│ C4           │            0.09 │         0.06 │           0.07 │           109 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C5           │            0.07 │         0.07 │           0.07 │            96 │
+│ C5           │            0.13 │         0.15 │           0.14 │            89 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C6           │            0.12 │         0.11 │           0.12 │           105 │
+│ C6           │            0.1  │         0.1  │           0.1  │           114 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C7           │            0.15 │         0.15 │           0.15 │           101 │
+│ C7           │            0.09 │         0.09 │           0.09 │            98 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C8           │            0.08 │         0.11 │           0.09 │            91 │
+│ C8           │            0.11 │         0.09 │           0.1  │           108 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C9           │            0.09 │         0.08 │           0.09 │           111 │
+│ C9           │            0.09 │         0.1  │           0.09 │            94 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ C10          │            0.15 │         0.14 │           0.15 │           108 │
+│ C10          │            0.12 │         0.15 │           0.13 │            86 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Macro Avg    │            0.12 │         0.11 │           0.11 │          1000 │
+│ Macro Avg    │            0.1  │         0.1  │           0.1  │          1000 │
 ├──────────────┼─────────────────┼──────────────┼────────────────┼───────────────┤
-│ Weighted Avg │            0.12 │         0.12 │           0.12 │          1000 │
+│ Weighted Avg │            0.09 │         0.1  │           0.09 │          1000 │
 ╘══════════════╧═════════════════╧══════════════╧════════════════╧═══════════════╛
 ```
 
 
+#### plot_conf_mat Output
+
+
+https://drive.google.com/file/d/1Card-dZs6sSjgqdiVPUMesXjy3u9nsuY/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/1001/
+
+
 #### You Can Plot And Generate HTML Page For Confusion Matrix Directly From One Calculation And Without Print Confusion Matrix And Classification Report
 
 
 ```python
 from numpy.random import randint
 from matplotlib.pyplot import show
 from conf_mat import calc_conf_mat, plot_conf_mat, conf_mat_to_html
@@ -577,25 +667,40 @@
     'C1', 'C2', 'C3', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9', 'C10'], detail=False)
 ```
 
 
 ### Output
 
 
+#### calc_conf_mat Output
+
+
 ```bash
-[[9, 12, 11, 8, 10, 10, 7, 6, 11, 9], [12, 9, 12, 9, 7, 3, 16, 7, 7, 11], [7, 10, 25, 14, 5, 14, 9, 11, 6, 12], [7, 15, 9, 11, 13, 13, 4, 7, 10, 10], [12, 10, 11, 3, 14, 6, 8, 19, 6, 15], [5, 14, 13, 17, 9, 8, 8, 7, 11, 17], [7, 10, 10, 10, 6, 9, 10, 4, 9, 11], [8, 9, 11, 7, 11, 11, 15, 9, 13, 12], [12, 12, 9, 6, 11, 7, 10, 13, 7, 10], [11, 5, 9, 13, 8, 14, 3, 9, 15, 13]]
+[[16, 11, 8, 6, 4, 11, 12, 9, 10, 6], [12, 15, 14, 7, 20, 7, 17, 8, 6, 10], [13, 13, 11, 12, 11, 10, 11, 9, 8, 9], [12, 11, 5, 15, 9, 10, 8, 10, 13, 9], [8, 13, 11, 8, 8, 8, 12, 15, 7, 12], [13, 8, 17, 14, 8, 7, 10, 6, 8, 6], [7, 21, 7, 7, 10, 11, 10, 12, 11, 8], [9, 10, 15, 11, 7, 6, 9, 6, 9, 9], [9, 13, 7, 14, 7, 10, 5, 11, 5, 7], [13, 9, 11, 8, 12, 12, 9, 7, 6, 13]]
 ```
 
 
-### Note
+#### plot_conf_mat Output
 
 
-These outputs are for the calc_conf_mat and print_conf_mat functions only, in both cases. I'll leave it to you to figure out the last two functions plot_conf_mat and conf_mat_to_html on your own.
+https://drive.google.com/file/d/1wmH3jQj8WZKtf2Vr-7LQgkI1udDFm0Zj/view?usp=drive_link
+
+
+#### conf_mat_to_html Output
+
+
+```bash
+HTML File Generated Successfully :)
+```
+https://xswzbb4c3ixsgksk9qu6zw.on.drv.tw/1011/
+
+
+### Note
 
 
-You can call all the functions with the camelCase format.
+You can call all functions with the camelCase format.
 
 
 ## License
 
 
 This project is licensed under the MIT LICENSE - see the [LICENSE](https://opensource.org/licenses/MIT) for more details.
```

### Comparing `conf-mat-1.0.4/setup.py` & `conf-mat-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="conf-mat",
-    version="1.0.4",
+    version="1.0.5",
     author="khiat Mohammed Abderrezzak",
     author_email="khiat.abderrezzak@gmail.com",
     license="MIT",
-    description="Sophisticate Open Confusion Matrix",
+    description="Sophisticate Confusion Matrix",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/conf-mat/",
     packages=find_packages(),
     install_requires=[
         "tabulate>=0.9.0",
         "matplotlib>=3.8.3",
```

