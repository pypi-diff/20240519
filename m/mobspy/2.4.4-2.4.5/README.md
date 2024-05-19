# Comparing `tmp/mobspy-2.4.4.tar.gz` & `tmp/mobspy-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobspy-2.4.4.tar", last modified: Fri May 17 16:16:21 2024, max compression
+gzip compressed data, was "mobspy-2.4.5.tar", last modified: Sun May 19 21:28:40 2024, max compression
```

## Comparing `mobspy-2.4.4.tar` & `mobspy-2.4.5.tar`

### file list

```diff
@@ -1,432 +1,437 @@
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:21.041458 mobspy-2.4.4/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.839733 mobspy-2.4.4/.github/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.864715 mobspy-2.4.4/.github/workflows/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-06-15 12:59:57.000000 mobspy-2.4.4/.github/workflows/python-app.yml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      415 2024-04-09 17:41:00.000000 mobspy-2.4.4/.gitignore
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1034 2024-02-26 16:22:21.000000 mobspy-2.4.4/.readthedocs.yaml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-06-15 12:59:57.000000 mobspy-2.4.4/LICENSE
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-17 16:16:21.040623 mobspy-2.4.4/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6331 2024-03-08 01:34:03.000000 mobspy-2.4.4/README.md
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.891450 mobspy-2.4.4/docs/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      634 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Makefile
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.924018 mobspy-2.4.4/docs/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.926663 mobspy-2.4.4/docs/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_autosummary/mobspy.rst
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.841544 mobspy-2.4.4/docs/_build/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.982218 mobspy-2.4.4/docs/_build/doctrees/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.008719 mobspy-2.4.4/docs/_build/doctrees/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    95114 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23601 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30820 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/03_Characteristics.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7466 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    24161 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/05_For_Loops.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21599 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    50076 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18699 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/08_Units.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41471 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/09_Result_Data.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    28500 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15272 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17080 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/12_Born_Species.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    39545 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/13_Events.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15325 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.011128 mobspy-2.4.4/docs/_build/doctrees/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2971 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/_autosummary/mobspy.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4285 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/api.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)  1736636 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2754 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/for_local_use.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4048 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/index.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    26568 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.data_handler.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67412 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   490595 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.modules.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16088 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.parameter_scripts.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8486 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.parameters.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8077 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.plot_params.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    86993 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.plot_scripts.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    33712 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.sbml_simulator.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9059 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/mobspy.simulation_logging.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2767 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/modules.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.044739 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.073824 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2407 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/setup.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2439 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/doctrees/test_script.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.131235 mobspy-2.4.4/docs/_build/html/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      230 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/.buildinfo
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.184126 mobspy-2.4.4/docs/_build/html/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41132 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/01_Basic_Intro.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16265 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17425 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/03_Characteristics.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10225 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/04_Characteristic_restriction.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15743 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/05_For_Loops.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14878 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/06_Order_Matters.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23518 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/07_Initial_Condition.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15642 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/08_Units.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23686 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/09_Result_Data.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23178 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/10_Reaction_Rates.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14337 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/11_Looping_Through_Species.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14032 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/12_Born_Species.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    28370 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/13_Events.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18015 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.185203 mobspy-2.4.4/docs/_build/html/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7201 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_autosummary/mobspy.html
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.217450 mobspy-2.4.4/docs/_build/html/_images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_11_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_1_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_4_3.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_8_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.235859 mobspy-2.4.4/docs/_build/html/_sources/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.262880 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.265286 mobspy-2.4.4/docs/_build/html/_sources/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/_autosummary/mobspy.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/api.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/for_local_use.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.data_handler.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.modules.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.parameters.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.plot_params.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/mobspy.simulation_logging.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/setup.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_sources/test_script.rst.txt
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.289483 mobspy-2.4.4/docs/_build/html/_static/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4289 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15094 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.292769 mobspy-2.4.4/docs/_build/html/_static/css/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3229 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.365023 mobspy-2.4.4/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    87624 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67312 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    86288 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    66444 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   165742 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   444379 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   165548 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    98024 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    77160 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   323344 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   193308 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   309728 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   184912 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   328412 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   195704 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   309192 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   182708 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   135314 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4472 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/doctools.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/file.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    89501 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.372284 mobspy-2.4.4/docs/_build/html/_static/js/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      934 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4370 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2734 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5023 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4758 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/language_data.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/minus.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4467 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6861 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/nbsphinx-code-cells.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      584 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/nbsphinx-gallery.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2871 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/plus.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4902 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/pygments.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18732 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7627 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/api.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6551 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/for_local_use.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67727 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/genindex.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10018 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/index.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14863 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.data_handler.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    91437 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   178543 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.modules.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11761 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.parameter_scripts.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8867 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.parameters.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8736 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.plot_params.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    36208 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.plot_scripts.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16526 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.sbml_simulator.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9250 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/mobspy.simulation_logging.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23199 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/modules.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8450 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/objects.inv
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17062 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/py-modindex.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6595 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/search.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    96699 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/searchindex.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6464 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/setup.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6500 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/_build/html/test_script.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/api.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1220 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/conf.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/for_local_use.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/index.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      800 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/make.bat
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.data_handler.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.modules.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.parameter_scripts.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.parameters.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.plot_params.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.plot_scripts.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.sbml_simulator.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/mobspy.simulation_logging.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/modules.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/setup.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.4/docs/test_script.rst
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:19.847299 mobspy-2.4.4/example_models/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.409247 mobspy-2.4.4/example_models/Tutorial Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   132826 2024-05-05 13:25:04.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7029 2024-05-14 12:30:35.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8153 2024-05-05 20:46:30.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3725 2024-05-06 09:21:49.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5464 2024-05-06 12:26:05.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8168 2024-05-06 13:31:40.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8662 2024-05-11 12:56:11.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    90412 2024-05-11 13:19:54.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30172 2024-05-14 13:24:55.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4201 2024-05-14 14:17:52.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4862 2024-05-14 14:54:54.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    47437 2024-05-14 20:07:50.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    31117 2024-05-15 13:19:46.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.413718 mobspy-2.4.4/example_models/Tutorial Notebooks/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12324 2023-04-19 14:32:18.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/images/Matching_Meta.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   141303 2023-04-09 17:03:35.000000 mobspy-2.4.4/example_models/Tutorial Notebooks/images/vectorial_space.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.655806 mobspy-2.4.4/example_models/application_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      572 2024-01-28 20:43:25.000000 mobspy-2.4.4/example_models/application_models/AB_2CD.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1448 2024-01-28 20:44:42.000000 mobspy-2.4.4/example_models/application_models/AND_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2357 2024-01-28 20:43:25.000000 mobspy-2.4.4/example_models/application_models/CRISPR_Oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1447 2024-05-07 17:47:59.000000 mobspy-2.4.4/example_models/application_models/For_The_Trees.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1291 2024-01-28 20:48:26.000000 mobspy-2.4.4/example_models/application_models/NOR_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1237 2024-01-28 20:47:24.000000 mobspy-2.4.4/example_models/application_models/donor_receptor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1371 2024-01-28 20:48:41.000000 mobspy-2.4.4/example_models/application_models/oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      994 2023-07-07 11:50:03.000000 mobspy-2.4.4/example_models/application_models/positive_phage_feedback_loop.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2917 2024-01-28 20:49:35.000000 mobspy-2.4.4/example_models/application_models/random_walk.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      637 2023-07-05 11:46:34.000000 mobspy-2.4.4/example_models/application_models/simple_infection.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      564 2024-01-28 20:50:18.000000 mobspy-2.4.4/example_models/application_models/simple_repressor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      828 2023-07-05 12:49:47.000000 mobspy-2.4.4/example_models/application_models/simple_rule_based_and_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      100 2024-05-17 12:39:17.000000 mobspy-2.4.4/for_local_use.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.657243 mobspy-2.4.4/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-06-15 12:59:57.000000 mobspy-2.4.4/images/img.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.664164 mobspy-2.4.4/mobspy/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2024-05-17 12:41:21.000000 mobspy-2.4.4/mobspy/_version.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.687986 mobspy-2.4.4/mobspy/data_handler/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/data_handler/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5759 2024-05-07 13:05:25.000000 mobspy-2.4.4/mobspy/data_handler/process_result_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8430 2024-05-15 10:39:35.000000 mobspy-2.4.4/mobspy/data_handler/time_series_object.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.694889 mobspy-2.4.4/mobspy/import_manager/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 12:02:22.000000 mobspy-2.4.4/mobspy/import_manager/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      639 2024-05-09 20:32:27.000000 mobspy-2.4.4/mobspy/import_manager/lazy_import_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      266 2024-05-11 12:43:21.000000 mobspy-2.4.4/mobspy/import_manager/profiler_import_time_test.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.781509 mobspy-2.4.4/mobspy/modules/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/modules/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8797 2024-05-13 18:03:50.000000 mobspy-2.4.4/mobspy/modules/assignments_implementation.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5229 2024-05-09 12:06:51.000000 mobspy-2.4.4/mobspy/modules/class_of_meta_specie_named_any.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21459 2024-05-09 17:30:19.000000 mobspy-2.4.4/mobspy/modules/compiler.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1573 2024-05-09 17:30:55.000000 mobspy-2.4.4/mobspy/modules/context_related_scripts.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5331 2024-05-09 18:27:27.000000 mobspy-2.4.4/mobspy/modules/event_functions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12949 2024-05-13 20:43:47.000000 mobspy-2.4.4/mobspy/modules/function_rate_code.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13174 2024-05-09 09:50:51.000000 mobspy-2.4.4/mobspy/modules/logic_operator_objects.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    54494 2024-05-13 16:54:50.000000 mobspy-2.4.4/mobspy/modules/meta_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5620 2024-05-09 17:15:14.000000 mobspy-2.4.4/mobspy/modules/meta_class_utils.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    39955 2024-05-13 20:43:12.000000 mobspy-2.4.4/mobspy/modules/mobspy_expressions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5117 2024-05-09 12:41:41.000000 mobspy-2.4.4/mobspy/modules/mobspy_parameters.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15249 2024-05-09 18:17:38.000000 mobspy-2.4.4/mobspy/modules/order_operators.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17391 2024-05-13 20:43:02.000000 mobspy-2.4.4/mobspy/modules/reaction_construction_nb.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4504 2024-05-09 16:53:50.000000 mobspy-2.4.4/mobspy/modules/set_counts_module.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4175 2024-05-09 18:27:27.000000 mobspy-2.4.4/mobspy/modules/species_string_generator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7715 2024-05-09 16:53:50.000000 mobspy-2.4.4/mobspy/modules/unit_handler.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      428 2024-05-09 16:53:50.000000 mobspy-2.4.4/mobspy/modules/user_functions.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.788755 mobspy-2.4.4/mobspy/parameter_estimation_data_loader/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-02-28 22:21:33.000000 mobspy-2.4.4/mobspy/parameter_estimation_data_loader/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      912 2024-01-31 10:55:41.000000 mobspy-2.4.4/mobspy/parameter_estimation_data_loader/data_loader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7845 2024-05-09 20:49:27.000000 mobspy-2.4.4/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.793781 mobspy-2.4.4/mobspy/parameter_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/parameter_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8408 2024-05-09 17:27:54.000000 mobspy-2.4.4/mobspy/parameter_scripts/parameter_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1957 2024-02-01 12:50:35.000000 mobspy-2.4.4/mobspy/parameter_scripts/parametric_sweeps.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.799802 mobspy-2.4.4/mobspy/parameters/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/parameters/README.md
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/parameters/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1188 2024-01-30 18:15:37.000000 mobspy-2.4.4/mobspy/parameters/default_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1285 2024-01-30 17:59:16.000000 mobspy-2.4.4/mobspy/parameters/example_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.802453 mobspy-2.4.4/mobspy/patch_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-04-09 18:34:07.000000 mobspy-2.4.4/mobspy/patch_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    71233 2024-05-05 13:14:45.000000 mobspy-2.4.4/mobspy/patch_scripts/basico_task_parametrization.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.814070 mobspy-2.4.4/mobspy/plot_params/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/plot_params/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2024-05-06 14:50:24.000000 mobspy-2.4.4/mobspy/plot_params/default_plot_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1907 2024-05-17 12:30:55.000000 mobspy-2.4.4/mobspy/plot_params/example_plot_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.823408 mobspy-2.4.4/mobspy/plot_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-03-28 14:29:54.000000 mobspy-2.4.4/mobspy/plot_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10975 2024-05-07 17:42:50.000000 mobspy-2.4.4/mobspy/plot_scripts/default_plots.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    20277 2024-05-17 12:33:10.000000 mobspy-2.4.4/mobspy/plot_scripts/hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2852 2024-05-16 20:39:29.000000 mobspy-2.4.4/mobspy/plot_scripts/process_plot_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3885 2024-03-28 14:34:48.000000 mobspy-2.4.4/mobspy/plot_scripts/statistics_calculations.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.829666 mobspy-2.4.4/mobspy/sbml_simulator/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8702 2024-03-20 17:46:34.000000 mobspy-2.4.4/mobspy/sbml_simulator/SBMLWriter.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/sbml_simulator/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.855762 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5705 2024-04-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      146 2024-04-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1040 2024-04-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8808 2024-04-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1070 2024-05-09 18:33:16.000000 mobspy-2.4.4/mobspy/sbml_simulator/builder.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12116 2024-05-09 20:34:41.000000 mobspy-2.4.4/mobspy/sbml_simulator/run.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    43371 2024-05-16 09:23:48.000000 mobspy-2.4.4/mobspy/simulation.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.858034 mobspy-2.4.4/mobspy/simulation_logging/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.4/mobspy/simulation_logging/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1099 2024-05-14 16:05:30.000000 mobspy-2.4.4/mobspy/simulation_logging/log_scripts.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       16 2024-05-13 10:44:36.000000 mobspy-2.4.4/mobspy/variables_and_operators.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.681692 mobspy-2.4.4/mobspy.egg-info/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-05-17 16:16:18.000000 mobspy-2.4.4/mobspy.egg-info/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16772 2024-05-17 16:16:19.000000 mobspy-2.4.4/mobspy.egg-info/SOURCES.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2024-05-17 16:16:18.000000 mobspy-2.4.4/mobspy.egg-info/dependency_links.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2024-05-17 16:16:18.000000 mobspy-2.4.4/mobspy.egg-info/requires.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2024-05-17 16:16:18.000000 mobspy-2.4.4/mobspy.egg-info/top_level.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-06-15 12:59:57.000000 mobspy-2.4.4/requirements.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2024-05-17 16:16:21.041791 mobspy-2.4.4/setup.cfg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-06-15 12:59:57.000000 mobspy-2.4.4/setup.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:20.864382 mobspy-2.4.4/test_plot_images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10767 2024-05-16 18:23:19.000000 mobspy-2.4.4/test_plot_images/constant_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    44355 2024-05-16 18:23:19.000000 mobspy-2.4.4/test_plot_images/deterministic_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    53864 2024-05-16 18:23:18.000000 mobspy-2.4.4/test_plot_images/stochastic_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    44218 2024-05-16 18:24:17.000000 mobspy-2.4.4/test_script.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-17 16:16:21.038268 mobspy-2.4.4/test_tools/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_1.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      241 2023-06-26 11:54:08.000000 mobspy-2.4.4/test_tools/model_10.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_11.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_12.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_13.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_14.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_15.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_16.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_17.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_18.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_19.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_2.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_20.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_21.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      471 2023-07-03 11:25:39.000000 mobspy-2.4.4/test_tools/model_22.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_23.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_24.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_25.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      518 2023-07-03 11:30:10.000000 mobspy-2.4.4/test_tools/model_26.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_27.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_28.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_29.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_3.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_30.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    55662 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_31.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      129 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_32.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      831 2023-07-03 15:00:26.000000 mobspy-2.4.4/test_tools/model_33.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2023-07-03 23:04:22.000000 mobspy-2.4.4/test_tools/model_34.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       61 2023-07-30 20:48:11.000000 mobspy-2.4.4/test_tools/model_35.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      175 2023-08-01 18:04:20.000000 mobspy-2.4.4/test_tools/model_36.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      391 2023-08-03 14:43:06.000000 mobspy-2.4.4/test_tools/model_37.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1427 2023-08-19 22:03:11.000000 mobspy-2.4.4/test_tools/model_38.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2853 2023-08-19 22:23:06.000000 mobspy-2.4.4/test_tools/model_39.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_4.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-11-15 12:57:45.000000 mobspy-2.4.4/test_tools/model_40.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1412 2023-11-15 12:57:45.000000 mobspy-2.4.4/test_tools/model_41.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      178 2023-11-15 12:57:45.000000 mobspy-2.4.4/test_tools/model_42.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      419 2023-11-17 12:18:00.000000 mobspy-2.4.4/test_tools/model_43.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      197 2024-01-31 16:54:44.000000 mobspy-2.4.4/test_tools/model_44.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8874 2024-02-22 02:44:14.000000 mobspy-2.4.4/test_tools/model_45.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      317 2024-02-24 00:21:58.000000 mobspy-2.4.4/test_tools/model_46.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      243 2024-02-24 13:50:27.000000 mobspy-2.4.4/test_tools/model_47.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      119 2024-05-02 10:01:49.000000 mobspy-2.4.4/test_tools/model_48.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      171 2024-05-07 20:34:12.000000 mobspy-2.4.4/test_tools/model_49.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_5.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      271 2024-05-13 15:07:53.000000 mobspy-2.4.4/test_tools/model_50.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      452 2024-05-13 19:52:51.000000 mobspy-2.4.4/test_tools/model_51.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-05-13 19:55:06.000000 mobspy-2.4.4/test_tools/model_52.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      417 2024-05-16 18:22:27.000000 mobspy-2.4.4/test_tools/model_53.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      389 2023-07-03 10:56:19.000000 mobspy-2.4.4/test_tools/model_6.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1362 2023-07-03 11:02:54.000000 mobspy-2.4.4/test_tools/model_7.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      433 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_8.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-06-15 12:59:57.000000 mobspy-2.4.4/test_tools/model_9.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-06-15 12:59:57.000000 mobspy-2.4.4/useful_parameters.json
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:40.207810 mobspy-2.4.5/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:38.856266 mobspy-2.4.5/.github/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:38.877761 mobspy-2.4.5/.github/workflows/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-06-15 12:59:57.000000 mobspy-2.4.5/.github/workflows/python-app.yml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      415 2024-04-09 17:41:00.000000 mobspy-2.4.5/.gitignore
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1034 2024-02-26 16:22:21.000000 mobspy-2.4.5/.readthedocs.yaml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-06-15 12:59:57.000000 mobspy-2.4.5/LICENSE
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7656 2024-05-19 21:28:40.206075 mobspy-2.4.5/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6394 2024-05-18 12:18:27.000000 mobspy-2.4.5/README.md
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:38.901762 mobspy-2.4.5/docs/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      634 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Makefile
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:38.933807 mobspy-2.4.5/docs/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:38.935320 mobspy-2.4.5/docs/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_autosummary/mobspy.rst
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:38.858571 mobspy-2.4.5/docs/_build/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:38.982921 mobspy-2.4.5/docs/_build/doctrees/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.040387 mobspy-2.4.5/docs/_build/doctrees/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    95114 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23601 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30820 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/03_Characteristics.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7466 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    24161 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/05_For_Loops.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21599 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    50076 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18699 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/08_Units.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    41471 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/09_Result_Data.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    28500 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15272 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17080 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/12_Born_Species.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    39545 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/13_Events.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15325 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.044765 mobspy-2.4.5/docs/_build/doctrees/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2971 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/_autosummary/mobspy.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4285 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/api.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)  1736636 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2754 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/for_local_use.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4048 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26568 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/mobspy.data_handler.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67412 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/mobspy.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   490595 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/mobspy.modules.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16088 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/mobspy.parameter_scripts.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8486 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/mobspy.parameters.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8077 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/mobspy.plot_params.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    86993 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/mobspy.plot_scripts.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    33712 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/mobspy.sbml_simulator.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9059 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/mobspy.simulation_logging.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2767 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/modules.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.127490 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.171714 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2407 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/setup.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2439 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/doctrees/test_script.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.236884 mobspy-2.4.5/docs/_build/html/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      230 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/.buildinfo
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.314923 mobspy-2.4.5/docs/_build/html/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    41132 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/01_Basic_Intro.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16265 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/02_Reaction_Inheritance.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17425 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/03_Characteristics.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10225 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/04_Characteristic_restriction.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15743 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/05_For_Loops.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14878 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/06_Order_Matters.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23518 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/07_Initial_Condition.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15642 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/08_Units.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23686 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/09_Result_Data.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23178 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/10_Reaction_Rates.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14337 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/11_Looping_Through_Species.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14032 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/12_Born_Species.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    28370 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/13_Events.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18015 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/14_Concatenating_Simulations.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.317247 mobspy-2.4.5/docs/_build/html/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7201 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_autosummary/mobspy.html
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.367165 mobspy-2.4.5/docs/_build/html/_images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_13_Events_11_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_13_Events_1_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_13_Events_4_3.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_13_Events_8_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.392289 mobspy-2.4.5/docs/_build/html/_sources/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.446021 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.448016 mobspy-2.4.5/docs/_build/html/_sources/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/_autosummary/mobspy.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/api.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/for_local_use.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/mobspy.data_handler.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/mobspy.modules.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/mobspy.parameters.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/mobspy.plot_params.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/mobspy.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/mobspy.simulation_logging.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/setup.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_sources/test_script.rst.txt
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.482012 mobspy-2.4.5/docs/_build/html/_static/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4289 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15094 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.489780 mobspy-2.4.5/docs/_build/html/_static/css/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3229 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.633864 mobspy-2.4.5/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    87624 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67312 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    86288 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    66444 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   165742 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   444379 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   165548 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    98024 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    77160 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   323344 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   193308 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   309728 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   184912 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   328412 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   195704 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   309192 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   182708 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   135314 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4472 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/file.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    89501 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.646322 mobspy-2.4.5/docs/_build/html/_static/js/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      934 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4370 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2734 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5023 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4758 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4467 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6861 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/nbsphinx-code-cells.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      584 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/nbsphinx-gallery.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2871 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4902 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18732 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5123 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7627 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/api.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6551 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/for_local_use.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67727 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/genindex.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10018 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/index.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14863 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/mobspy.data_handler.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    91437 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/mobspy.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   178543 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/mobspy.modules.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11761 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/mobspy.parameter_scripts.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8867 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/mobspy.parameters.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8736 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/mobspy.plot_params.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    36208 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/mobspy.plot_scripts.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16526 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/mobspy.sbml_simulator.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9250 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/mobspy.simulation_logging.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23199 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/modules.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8450 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/objects.inv
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17062 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/py-modindex.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6595 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/search.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    96699 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/searchindex.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6464 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/setup.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6500 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/_build/html/test_script.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/api.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1220 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/conf.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/for_local_use.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/index.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      800 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/make.bat
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/mobspy.data_handler.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/mobspy.modules.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/mobspy.parameter_scripts.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/mobspy.parameters.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/mobspy.plot_params.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/mobspy.plot_scripts.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/mobspy.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/mobspy.sbml_simulator.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/mobspy.simulation_logging.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/modules.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/setup.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.4.5/docs/test_script.rst
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:38.862279 mobspy-2.4.5/example_models/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.686294 mobspy-2.4.5/example_models/Tutorial Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   132880 2024-05-18 12:16:26.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6611 2024-05-18 12:16:23.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8153 2024-05-18 12:16:55.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3725 2024-05-18 12:17:07.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5464 2024-05-18 12:17:48.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8168 2024-05-06 13:31:40.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8662 2024-05-18 12:18:51.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11716 2024-05-18 12:19:35.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/08_Units_and_Output.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    85486 2024-05-18 12:20:08.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30270 2024-05-18 12:20:32.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4201 2024-05-18 12:21:02.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4862 2024-05-18 12:21:55.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    58353 2024-05-18 12:21:53.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30603 2024-05-18 12:22:37.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18512 2024-05-18 12:23:29.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/15_Assignments.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9875 2024-05-16 10:03:05.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/16_Rev_All_Any.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.693421 mobspy-2.4.5/example_models/Tutorial Notebooks/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12324 2023-04-19 14:32:18.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/images/Matching_Meta.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   141303 2023-04-09 17:03:35.000000 mobspy-2.4.5/example_models/Tutorial Notebooks/images/vectorial_space.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.737633 mobspy-2.4.5/example_models/application_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      572 2024-01-28 20:43:25.000000 mobspy-2.4.5/example_models/application_models/AB_2CD.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1448 2024-01-28 20:44:42.000000 mobspy-2.4.5/example_models/application_models/AND_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2357 2024-01-28 20:43:25.000000 mobspy-2.4.5/example_models/application_models/CRISPR_Oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1447 2024-05-07 17:47:59.000000 mobspy-2.4.5/example_models/application_models/For_The_Trees.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1291 2024-01-28 20:48:26.000000 mobspy-2.4.5/example_models/application_models/NOR_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1237 2024-01-28 20:47:24.000000 mobspy-2.4.5/example_models/application_models/donor_receptor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1371 2024-01-28 20:48:41.000000 mobspy-2.4.5/example_models/application_models/oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      994 2023-07-07 11:50:03.000000 mobspy-2.4.5/example_models/application_models/positive_phage_feedback_loop.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2917 2024-01-28 20:49:35.000000 mobspy-2.4.5/example_models/application_models/random_walk.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      637 2023-07-05 11:46:34.000000 mobspy-2.4.5/example_models/application_models/simple_infection.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      564 2024-01-28 20:50:18.000000 mobspy-2.4.5/example_models/application_models/simple_repressor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      828 2023-07-05 12:49:47.000000 mobspy-2.4.5/example_models/application_models/simple_rule_based_and_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      105 2024-05-19 19:38:35.000000 mobspy-2.4.5/for_local_use.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.741758 mobspy-2.4.5/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-06-15 12:59:57.000000 mobspy-2.4.5/images/img.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.753806 mobspy-2.4.5/mobspy/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-06-15 12:59:57.000000 mobspy-2.4.5/mobspy/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2024-05-19 21:25:16.000000 mobspy-2.4.5/mobspy/_version.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.769376 mobspy-2.4.5/mobspy/data_handler/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.5/mobspy/data_handler/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5421 2024-05-17 19:35:10.000000 mobspy-2.4.5/mobspy/data_handler/process_result_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8430 2024-05-15 10:39:35.000000 mobspy-2.4.5/mobspy/data_handler/time_series_object.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.778454 mobspy-2.4.5/mobspy/import_manager/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-05-13 12:02:22.000000 mobspy-2.4.5/mobspy/import_manager/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      639 2024-05-09 20:32:27.000000 mobspy-2.4.5/mobspy/import_manager/lazy_import_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      266 2024-05-11 12:43:21.000000 mobspy-2.4.5/mobspy/import_manager/profiler_import_time_test.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.823573 mobspy-2.4.5/mobspy/modules/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.5/mobspy/modules/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9099 2024-05-19 19:34:07.000000 mobspy-2.4.5/mobspy/modules/assignments_implementation.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5229 2024-05-09 12:06:51.000000 mobspy-2.4.5/mobspy/modules/class_of_meta_specie_named_any.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21459 2024-05-09 17:30:19.000000 mobspy-2.4.5/mobspy/modules/compiler.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1573 2024-05-09 17:30:55.000000 mobspy-2.4.5/mobspy/modules/context_related_scripts.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5331 2024-05-09 18:27:27.000000 mobspy-2.4.5/mobspy/modules/event_functions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12949 2024-05-13 20:43:47.000000 mobspy-2.4.5/mobspy/modules/function_rate_code.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13174 2024-05-09 09:50:51.000000 mobspy-2.4.5/mobspy/modules/logic_operator_objects.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    54494 2024-05-13 16:54:50.000000 mobspy-2.4.5/mobspy/modules/meta_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5620 2024-05-09 17:15:14.000000 mobspy-2.4.5/mobspy/modules/meta_class_utils.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    39955 2024-05-13 20:43:12.000000 mobspy-2.4.5/mobspy/modules/mobspy_expressions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5117 2024-05-09 12:41:41.000000 mobspy-2.4.5/mobspy/modules/mobspy_parameters.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15249 2024-05-09 18:17:38.000000 mobspy-2.4.5/mobspy/modules/order_operators.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17391 2024-05-13 20:43:02.000000 mobspy-2.4.5/mobspy/modules/reaction_construction_nb.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4504 2024-05-09 16:53:50.000000 mobspy-2.4.5/mobspy/modules/set_counts_module.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4175 2024-05-09 18:27:27.000000 mobspy-2.4.5/mobspy/modules/species_string_generator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7870 2024-05-17 18:36:55.000000 mobspy-2.4.5/mobspy/modules/unit_handler.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      428 2024-05-09 16:53:50.000000 mobspy-2.4.5/mobspy/modules/user_functions.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.827263 mobspy-2.4.5/mobspy/parameter_estimation_data_loader/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-02-28 22:21:33.000000 mobspy-2.4.5/mobspy/parameter_estimation_data_loader/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      912 2024-01-31 10:55:41.000000 mobspy-2.4.5/mobspy/parameter_estimation_data_loader/data_loader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7845 2024-05-09 20:49:27.000000 mobspy-2.4.5/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.835169 mobspy-2.4.5/mobspy/parameter_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.5/mobspy/parameter_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8408 2024-05-09 17:27:54.000000 mobspy-2.4.5/mobspy/parameter_scripts/parameter_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1957 2024-02-01 12:50:35.000000 mobspy-2.4.5/mobspy/parameter_scripts/parametric_sweeps.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.843128 mobspy-2.4.5/mobspy/parameters/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-06-15 12:59:57.000000 mobspy-2.4.5/mobspy/parameters/README.md
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.5/mobspy/parameters/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1188 2024-01-30 18:15:37.000000 mobspy-2.4.5/mobspy/parameters/default_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1285 2024-01-30 17:59:16.000000 mobspy-2.4.5/mobspy/parameters/example_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.845938 mobspy-2.4.5/mobspy/patch_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-04-09 18:34:07.000000 mobspy-2.4.5/mobspy/patch_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    71233 2024-05-05 13:14:45.000000 mobspy-2.4.5/mobspy/patch_scripts/basico_task_parametrization.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.860567 mobspy-2.4.5/mobspy/plot_params/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.5/mobspy/plot_params/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2024-05-06 14:50:24.000000 mobspy-2.4.5/mobspy/plot_params/default_plot_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1907 2024-05-17 12:30:55.000000 mobspy-2.4.5/mobspy/plot_params/example_plot_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.877046 mobspy-2.4.5/mobspy/plot_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-03-28 14:29:54.000000 mobspy-2.4.5/mobspy/plot_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10977 2024-05-17 23:07:18.000000 mobspy-2.4.5/mobspy/plot_scripts/default_plots.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    20265 2024-05-17 22:57:17.000000 mobspy-2.4.5/mobspy/plot_scripts/hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2852 2024-05-16 20:39:29.000000 mobspy-2.4.5/mobspy/plot_scripts/process_plot_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3885 2024-03-28 14:34:48.000000 mobspy-2.4.5/mobspy/plot_scripts/statistics_calculations.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.882910 mobspy-2.4.5/mobspy/sbml_simulator/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8702 2024-03-20 17:46:34.000000 mobspy-2.4.5/mobspy/sbml_simulator/SBMLWriter.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.5/mobspy/sbml_simulator/__init__.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.895788 mobspy-2.4.5/mobspy/sbml_simulator/__pycache__/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5705 2024-04-09 18:33:16.000000 mobspy-2.4.5/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      146 2024-04-09 18:33:16.000000 mobspy-2.4.5/mobspy/sbml_simulator/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1040 2024-04-09 18:33:16.000000 mobspy-2.4.5/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8808 2024-04-09 18:33:16.000000 mobspy-2.4.5/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1070 2024-05-09 18:33:16.000000 mobspy-2.4.5/mobspy/sbml_simulator/builder.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12116 2024-05-09 20:34:41.000000 mobspy-2.4.5/mobspy/sbml_simulator/run.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    43371 2024-05-17 19:42:26.000000 mobspy-2.4.5/mobspy/simulation.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.898888 mobspy-2.4.5/mobspy/simulation_logging/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.4.5/mobspy/simulation_logging/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1099 2024-05-17 18:23:52.000000 mobspy-2.4.5/mobspy/simulation_logging/log_scripts.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       16 2024-05-13 10:44:36.000000 mobspy-2.4.5/mobspy/variables_and_operators.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.763659 mobspy-2.4.5/mobspy.egg-info/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7656 2024-05-19 21:28:37.000000 mobspy-2.4.5/mobspy.egg-info/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16990 2024-05-19 21:28:38.000000 mobspy-2.4.5/mobspy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2024-05-19 21:28:37.000000 mobspy-2.4.5/mobspy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2024-05-19 21:28:37.000000 mobspy-2.4.5/mobspy.egg-info/requires.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2024-05-19 21:28:37.000000 mobspy-2.4.5/mobspy.egg-info/top_level.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-06-15 12:59:57.000000 mobspy-2.4.5/requirements.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2024-05-19 21:28:40.209440 mobspy-2.4.5/setup.cfg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-06-15 12:59:57.000000 mobspy-2.4.5/setup.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:39.925560 mobspy-2.4.5/test_plot_images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10767 2024-05-19 19:39:16.000000 mobspy-2.4.5/test_plot_images/constant_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    44758 2024-05-19 19:39:16.000000 mobspy-2.4.5/test_plot_images/deterministic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    54301 2024-05-19 19:39:16.000000 mobspy-2.4.5/test_plot_images/stochastic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    44758 2024-05-19 19:40:31.000000 mobspy-2.4.5/test_script.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-05-19 21:28:40.200881 mobspy-2.4.5/test_tools/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_1.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      241 2023-06-26 11:54:08.000000 mobspy-2.4.5/test_tools/model_10.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_11.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_12.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_13.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_14.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_15.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_16.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_17.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_18.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_19.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_2.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_20.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_21.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      471 2023-07-03 11:25:39.000000 mobspy-2.4.5/test_tools/model_22.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_23.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_24.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_25.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      518 2023-07-03 11:30:10.000000 mobspy-2.4.5/test_tools/model_26.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_27.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_28.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_29.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_3.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_30.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    55662 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_31.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      129 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_32.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      831 2023-07-03 15:00:26.000000 mobspy-2.4.5/test_tools/model_33.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2023-07-03 23:04:22.000000 mobspy-2.4.5/test_tools/model_34.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       61 2023-07-30 20:48:11.000000 mobspy-2.4.5/test_tools/model_35.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      175 2023-08-01 18:04:20.000000 mobspy-2.4.5/test_tools/model_36.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      391 2023-08-03 14:43:06.000000 mobspy-2.4.5/test_tools/model_37.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1427 2023-08-19 22:03:11.000000 mobspy-2.4.5/test_tools/model_38.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2853 2023-08-19 22:23:06.000000 mobspy-2.4.5/test_tools/model_39.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_4.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-11-15 12:57:45.000000 mobspy-2.4.5/test_tools/model_40.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1412 2023-11-15 12:57:45.000000 mobspy-2.4.5/test_tools/model_41.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      178 2023-11-15 12:57:45.000000 mobspy-2.4.5/test_tools/model_42.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      419 2023-11-17 12:18:00.000000 mobspy-2.4.5/test_tools/model_43.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      197 2024-01-31 16:54:44.000000 mobspy-2.4.5/test_tools/model_44.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8874 2024-02-22 02:44:14.000000 mobspy-2.4.5/test_tools/model_45.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      317 2024-02-24 00:21:58.000000 mobspy-2.4.5/test_tools/model_46.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      243 2024-02-24 13:50:27.000000 mobspy-2.4.5/test_tools/model_47.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      119 2024-05-02 10:01:49.000000 mobspy-2.4.5/test_tools/model_48.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      171 2024-05-07 20:34:12.000000 mobspy-2.4.5/test_tools/model_49.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_5.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      271 2024-05-13 15:07:53.000000 mobspy-2.4.5/test_tools/model_50.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      452 2024-05-13 19:52:51.000000 mobspy-2.4.5/test_tools/model_51.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-05-13 19:55:06.000000 mobspy-2.4.5/test_tools/model_52.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      417 2024-05-16 18:22:27.000000 mobspy-2.4.5/test_tools/model_53.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      122 2024-05-19 19:38:35.000000 mobspy-2.4.5/test_tools/model_54.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      160 2024-05-19 19:35:09.000000 mobspy-2.4.5/test_tools/model_55.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      389 2023-07-03 10:56:19.000000 mobspy-2.4.5/test_tools/model_6.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1362 2023-07-03 11:02:54.000000 mobspy-2.4.5/test_tools/model_7.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      433 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_8.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-06-15 12:59:57.000000 mobspy-2.4.5/test_tools/model_9.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-06-15 12:59:57.000000 mobspy-2.4.5/useful_parameters.json
```

### Comparing `mobspy-2.4.4/.github/workflows/python-app.yml` & `mobspy-2.4.5/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/.readthedocs.yaml` & `mobspy-2.4.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/LICENSE` & `mobspy-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/PKG-INFO` & `mobspy-2.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.4.4
+Version: 2.4.5
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
         
@@ -120,13 +120,15 @@
         
         Version 2.1 - Added model parameters. Now MySim.results returns a list of all resulting time series no matter the number of repetitions. However, now a MySim.fres attribute was released that returns only the first time series in each simulation (thus, it is equal to MySim results with only one repetition in the previous version).
         
         Version 2.2 - Added MobsPy expressions
         
         Version 2.3 - MobsPy standard output is now always concentration.
         
+        Version 2.4.4 - Assignments completely added (both notations)
+        
         
         
         
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `mobspy-2.4.4/README.md` & `mobspy-2.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -114,9 +114,11 @@
 
 Version 2.1 - Added model parameters. Now MySim.results returns a list of all resulting time series no matter the number of repetitions. However, now a MySim.fres attribute was released that returns only the first time series in each simulation (thus, it is equal to MySim results with only one repetition in the previous version).
 
 Version 2.2 - Added MobsPy expressions
 
 Version 2.3 - MobsPy standard output is now always concentration.
 
+Version 2.4.4 - Assignments completely added (both notations)
+
```

### Comparing `mobspy-2.4.4/docs/Makefile` & `mobspy-2.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.5/docs/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.5/docs/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.5/docs/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.5/docs/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.5/docs/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.5/docs/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.5/docs/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/08_Units.ipynb` & `mobspy-2.4.5/docs/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.5/docs/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.5/docs/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.5/docs/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.5/docs/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/13_Events.ipynb` & `mobspy-2.4.5/docs/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.5/docs/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/03_Characteristics.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/03_Characteristics.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/05_For_Loops.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/05_For_Loops.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/08_Units.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/08_Units.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/09_Result_Data.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/09_Result_Data.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/12_Born_Species.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/12_Born_Species.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/13_Events.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/13_Events.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree` & `mobspy-2.4.5/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/_autosummary/mobspy.doctree` & `mobspy-2.4.5/docs/_build/doctrees/_autosummary/mobspy.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/api.doctree` & `mobspy-2.4.5/docs/_build/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/environment.pickle` & `mobspy-2.4.5/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/for_local_use.doctree` & `mobspy-2.4.5/docs/_build/doctrees/for_local_use.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/index.doctree` & `mobspy-2.4.5/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/mobspy.data_handler.doctree` & `mobspy-2.4.5/docs/_build/doctrees/mobspy.data_handler.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/mobspy.doctree` & `mobspy-2.4.5/docs/_build/doctrees/mobspy.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/mobspy.modules.doctree` & `mobspy-2.4.5/docs/_build/doctrees/mobspy.modules.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/mobspy.parameter_scripts.doctree` & `mobspy-2.4.5/docs/_build/doctrees/mobspy.parameter_scripts.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/mobspy.parameters.doctree` & `mobspy-2.4.5/docs/_build/doctrees/mobspy.parameters.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/mobspy.plot_params.doctree` & `mobspy-2.4.5/docs/_build/doctrees/mobspy.plot_params.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/mobspy.plot_scripts.doctree` & `mobspy-2.4.5/docs/_build/doctrees/mobspy.plot_scripts.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/mobspy.sbml_simulator.doctree` & `mobspy-2.4.5/docs/_build/doctrees/mobspy.sbml_simulator.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/mobspy.simulation_logging.doctree` & `mobspy-2.4.5/docs/_build/doctrees/mobspy.simulation_logging.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/modules.doctree` & `mobspy-2.4.5/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png` & `mobspy-2.4.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/setup.doctree` & `mobspy-2.4.5/docs/_build/doctrees/setup.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/doctrees/test_script.doctree` & `mobspy-2.4.5/docs/_build/doctrees/test_script.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/01_Basic_Intro.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/01_Basic_Intro.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/02_Reaction_Inheritance.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/03_Characteristics.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/03_Characteristics.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/04_Characteristic_restriction.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/04_Characteristic_restriction.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/05_For_Loops.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/05_For_Loops.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/06_Order_Matters.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/06_Order_Matters.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/07_Initial_Condition.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/07_Initial_Condition.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/08_Units.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/08_Units.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/08_Units.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/09_Result_Data.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/09_Result_Data.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/10_Reaction_Rates.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/10_Reaction_Rates.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/11_Looping_Through_Species.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/11_Looping_Through_Species.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/12_Born_Species.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/12_Born_Species.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/13_Events.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/13_Events.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/13_Events.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.html` & `mobspy-2.4.5/docs/_build/html/Notebooks/14_Concatenating_Simulations.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.5/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_autosummary/mobspy.html` & `mobspy-2.4.5/docs/_build/html/_autosummary/mobspy.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_11_2.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_13_Events_11_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_1_2.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_13_Events_1_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_4_3.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_13_Events_4_3.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_13_Events_8_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_13_Events_8_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png` & `mobspy-2.4.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt` & `mobspy-2.4.5/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/index.rst.txt` & `mobspy-2.4.5/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/mobspy.data_handler.rst.txt` & `mobspy-2.4.5/docs/_build/html/_sources/mobspy.data_handler.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/mobspy.modules.rst.txt` & `mobspy-2.4.5/docs/_build/html/_sources/mobspy.modules.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt` & `mobspy-2.4.5/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/mobspy.parameters.rst.txt` & `mobspy-2.4.5/docs/_build/html/_sources/mobspy.parameters.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/mobspy.plot_params.rst.txt` & `mobspy-2.4.5/docs/_build/html/_sources/mobspy.plot_params.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt` & `mobspy-2.4.5/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/mobspy.rst.txt` & `mobspy-2.4.5/docs/_build/html/_sources/mobspy.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt` & `mobspy-2.4.5/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `mobspy-2.4.5/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/basic.css` & `mobspy-2.4.5/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/badge_only.css` & `mobspy-2.4.5/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold.woff` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal.woff` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `mobspy-2.4.5/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/css/theme.css` & `mobspy-2.4.5/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/doctools.js` & `mobspy-2.4.5/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/jquery.js` & `mobspy-2.4.5/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/js/badge_only.js` & `mobspy-2.4.5/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `mobspy-2.4.5/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/js/html5shiv.min.js` & `mobspy-2.4.5/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/js/theme.js` & `mobspy-2.4.5/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/language_data.js` & `mobspy-2.4.5/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg` & `mobspy-2.4.5/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/nbsphinx-code-cells.css` & `mobspy-2.4.5/docs/_build/html/_static/nbsphinx-code-cells.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/nbsphinx-gallery.css` & `mobspy-2.4.5/docs/_build/html/_static/nbsphinx-gallery.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/nbsphinx-no-thumbnail.svg` & `mobspy-2.4.5/docs/_build/html/_static/nbsphinx-no-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/pygments.css` & `mobspy-2.4.5/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/searchtools.js` & `mobspy-2.4.5/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/_static/sphinx_highlight.js` & `mobspy-2.4.5/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/api.html` & `mobspy-2.4.5/docs/_build/html/api.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/for_local_use.html` & `mobspy-2.4.5/docs/_build/html/for_local_use.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/genindex.html` & `mobspy-2.4.5/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/index.html` & `mobspy-2.4.5/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/mobspy.data_handler.html` & `mobspy-2.4.5/docs/_build/html/mobspy.data_handler.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/mobspy.html` & `mobspy-2.4.5/docs/_build/html/mobspy.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/mobspy.modules.html` & `mobspy-2.4.5/docs/_build/html/mobspy.modules.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/mobspy.parameter_scripts.html` & `mobspy-2.4.5/docs/_build/html/mobspy.parameter_scripts.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/mobspy.parameters.html` & `mobspy-2.4.5/docs/_build/html/mobspy.parameters.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/mobspy.plot_params.html` & `mobspy-2.4.5/docs/_build/html/mobspy.plot_params.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/mobspy.plot_scripts.html` & `mobspy-2.4.5/docs/_build/html/mobspy.plot_scripts.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/mobspy.sbml_simulator.html` & `mobspy-2.4.5/docs/_build/html/mobspy.sbml_simulator.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/mobspy.simulation_logging.html` & `mobspy-2.4.5/docs/_build/html/mobspy.simulation_logging.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/modules.html` & `mobspy-2.4.5/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/objects.inv` & `mobspy-2.4.5/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/py-modindex.html` & `mobspy-2.4.5/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/search.html` & `mobspy-2.4.5/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/searchindex.js` & `mobspy-2.4.5/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/setup.html` & `mobspy-2.4.5/docs/_build/html/setup.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/_build/html/test_script.html` & `mobspy-2.4.5/docs/_build/html/test_script.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/conf.py` & `mobspy-2.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/index.rst` & `mobspy-2.4.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/make.bat` & `mobspy-2.4.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/mobspy.data_handler.rst` & `mobspy-2.4.5/docs/mobspy.data_handler.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/mobspy.modules.rst` & `mobspy-2.4.5/docs/mobspy.modules.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/mobspy.parameter_scripts.rst` & `mobspy-2.4.5/docs/mobspy.parameter_scripts.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/mobspy.parameters.rst` & `mobspy-2.4.5/docs/mobspy.parameters.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/mobspy.plot_params.rst` & `mobspy-2.4.5/docs/mobspy.plot_params.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/mobspy.plot_scripts.rst` & `mobspy-2.4.5/docs/mobspy.plot_scripts.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/mobspy.rst` & `mobspy-2.4.5/docs/mobspy.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/docs/mobspy.sbml_simulator.rst` & `mobspy-2.4.5/docs/mobspy.sbml_simulator.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995801814649471%*

 * *Differences: {"'cells'": "{3: {'outputs': {insert: [(1, OrderedDict([('name', 'stdout'), ('output_type', "*

 * *            "'stream'), ('text', ['\\n'])]))]}}, 5: {'outputs': {0: {'data': {'text/plain': "*

 * *            "['<mobspy.modules.meta_class.Reactions at 0x7fc51cba9280>']}}}}, 7: {'outputs': {0: "*

 * *            "{'data': {'text/plain': ['(<mobspy.modules.meta_class.Reacting_Species at "*

 * *            "0x7fc51cba93d0>,\\n', ' <mobspy.modules.meta_class.Reacting_Species at "*

 * *            "0x7fc51cba9370>)']}}}}, 9: {'outputs' […]*

```diff
@@ -48,14 +48,21 @@
                     "text": [
                         "Compiling model\n",
                         "Starting Simulator\n",
                         "Simulation is Over\n"
                     ]
                 },
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
                         "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
@@ -94,15 +101,15 @@
             "execution_count": 3,
             "id": "4887dd2c-eeb7-4261-be2d-fc553d2a170b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fcc15406490>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7fc51cba9280>"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -129,16 +136,16 @@
             "execution_count": 4,
             "id": "ebff93da-b7a8-4633-947a-f0bebfc4015d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(<mobspy.modules.meta_class.Reacting_Species at 0x7fcc19d778b0>,\n",
-                            " <mobspy.modules.meta_class.Reacting_Species at 0x7fcc19d77070>)"
+                            "(<mobspy.modules.meta_class.Reacting_Species at 0x7fc51cba93d0>,\n",
+                            " <mobspy.modules.meta_class.Reacting_Species at 0x7fc51cba9370>)"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -165,15 +172,15 @@
             "execution_count": 5,
             "id": "9d7a0cab-1e8a-4599-9698-44298607668a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fcc19d773a0>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7fc52347d550>"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -227,15 +234,15 @@
             "execution_count": 7,
             "id": "edab6319-29ea-4de2-861d-090c8a9b5439",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<matplotlib.image.AxesImage at 0x7fcc19e16c10>"
+                            "<matplotlib.image.AxesImage at 0x7fc52352c070>"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
@@ -285,15 +292,15 @@
             "execution_count": 8,
             "id": "81e1b6aa-2040-49da-af8e-1e3c8a34ac3f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fcc19d6bd00>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7fc52353e460>"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -392,16 +399,25 @@
                     "text": [
                         "Compiling model\n",
                         "Starting Simulator\n",
                         "Simulation is Over\n"
                     ]
                 },
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "\n",
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAaAAAAEaCAYAAABXZ4NKAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjMuNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8QVMy6AAAACXBIWXMAAAsTAAALEwEAmpwYAABS/klEQVR4nO3deXxU1fn48c8zk31PSAKEHQxhB9lUFmVR2dRopdbtZ61tKW3dal3b2tr1283WWq3WWpeq3691Dy4gqCAqooCArGEXgUAWQkISskzm+f0xkzGESTKETCYhz/v1yiuZe8+c++RymSfn3HPPEVXFGGOMaWuOUAdgjDGmc7IEZIwxJiQsARljjAkJS0DGGGNCwhKQMcaYkLAEZIwxJiTCQh3AyUpNTdW+ffuGOgxjjDEBWLNmTaGqpvnbF7QEJCJPABcB+ao6zM9+Af4GzAYqgOtV9bPm6u3bty+rV69u7XCNMcYEgYh80di+YHbBPQXMbGL/LCDT+zUPeCSIsRhjjGlngpaAVHU5cLiJItnAf9RjJZAkIt2DFQ9AeXU5s56dxd9W/i2YhzHGGBOAUA5C6AF8We/1Pu+2E4jIPBFZLSKrCwoKWnzAvSV7WbRzEXe/ezc2BZExxoRWKBOQ+NnmNyuo6mOqOlZVx6al+b2XFZDBaYPpFteNSlclv13+2xbXY4wx5tSFMgHtA3rVe90TOBDsg/7i3F8A8Mvlv2R/6f5gH84YY0wjQpmAFgDXicfZQImq5gX7oNeOvBYHDlxuF995/TvWFWeMMSEStAQkIv8HfAxkicg+Efm2iMwXkfneIm8Bu4AdwL+AHwQrlvriIuKY2m8qAIt2LOKlzS+1xWGNMcY0ELTngFT1qmb2K/DDYB2/Kd8c+U3e3f0uDnEw/435jM0YS7/kfqEIxRhj2kRRURHTp08H4ODBgzidTuruqX/66adERES0eUwdbiaE1nBx1sU4xUmt1nLMdYxL/3spK25YQWxEbKhDM8aYoOjSpQvr1q0D4L777iMuLo7bb7/dt9/lchEW1rYpoVPOBZcUlcQFAy4g0hlJdHg0G/M38q2cb9n9IGNMp3L99ddz2223MXXqVO666y527tzJzJkzGTNmDJMnT2br1q0AFBQUcPnllzNu3DjGjRvHRx991CrH75QtIIDLB1/Ooh2LqKmsYXzGeF7c/CJnfngm90y+J9ShGWNOc7cuupV1B9e1ap2juo3igZkPnPT7tm3bxjvvvIPT6WT69Ok8+uijZGZm8sknn/CDH/yA9957j1tuuYUf/ehHTJo0ib179zJjxgy2bNlyyjF32gSUnZXN9974HuMyxrFy/0qm95vOT9/7KXOHzCWzS2aowzPGmDbx9a9/HafTSVlZGStWrODrX/+6b19VVRUA77zzDps3b/ZtLy0t5ejRo8THx5/SsTttAkqLTeO8PufxWd5npMaksvPwThTl9W2vc9s5t4U6PGPMaawlLZVgiY313Pt2u90kJSX57hPV53a7+fjjj4mOjm7VY3fKe0B1Hrv4MYalD6OwopA9JXtIjkrmze1vhjosY4xpcwkJCfTr148XX3wRAFVl/fr1AFx44YU89NBDvrL+klRLdOoEdEbKGSz/1nL+dfG/iHBGUFxZzLI9yyitKg11aMYY0+aee+45/v3vfzNy5EiGDh1KTk4OAA8++CCrV69mxIgRDBkyhEcffbRVjicdbeTX2LFjNRjrAW0v2s7ghwdTq7X8btrvbDCCMca0AhFZo6pj/e3r1C2g+jK7ZPLKFa8AcO/Sezlc0dRKEsYYY06VJaB6Lhl0CUPShlCrtYx5bAxutzvUIRljzGnLElADP5n0EwD2lOzhm699M8TRGGPM6SuoCUhEZopIrojsEJG7/exPFJHXRWS9iGwSkW8FM55AzDxjJg5xEOGM4LkNz7G7eHeoQzLGmNNSMGfDdgIPA7OAIcBVIjKkQbEfAptVdSQwBbhfRNp+Rrx6usR04eyeZ9MtrhuKcvkLl9sUPcYYEwTBbAGNB3ao6i5VrQaeB7IblFEgXkQEiAMOA64gxhSQOZlz2Fuyl5ToFNYeXMuznz8b6pCMMea0E8wE1AP4st7rfd5t9T0EDMazEuoG4BZVDfmd/zmZcwAYljYMgBsX3kh+eX4oQzLGmNNOMBOQ+NnWsC9rBrAOyABGAQ+JSMIJFYnME5HVIrK6oKCgteM8wYiuI/j2md9m+d7lOMRBaVUpt71t0/MYY0xralECEpH7Aii2D+hV73VPPC2d+r4FvKIeO4DdwKCGFanqY6o6VlXH1i2gFEwiwuOXPM7iaxeTHJUMwHMbnmPNgTVBP7YxxnQWLW0BBfJJvArIFJF+3oEFVwILGpTZC0wHEJGuQBaeZbrbhQsGXMCG72/AKU4AfvBmm6wabowxnUKLEpCqvh5AGRdwI/A2sAV4QVU3ich8EZnvLfZrYIKIbADeBe5S1cKWxBQs3eO7c+eEOwH49MCnLNm5JMQRGWPM6aHZueBE5Gk8gwOOeF8nA/er6g3BD+9EwZoLriludTP04aFsLdpKz/iefPGjL3CIPcNrjDHNOdW54EbUJR8AVS0Gzmyl2DoEhzhYdv0yHOJg39F9PPzpw6EOyRhjOrxAEpDD2+oBQERS6IQL2XWN68qvp/4agNsW38ahskMhjsgYYzq2QBLQ/cAKEfm1iPwaWAH8MbhhtU93TbyL9Nh0XG4XIx4ZYUnIGGNOQbMJSFX/A8wFDgH5wNdU9ZlgB9YeOR1OHrvoMQDyK/IZ/6/xfHHkixBHZYwxHVOgd9K3Aq8AOUCZiPQOXkjt28VZFzOwy0DP/aDSfUz49wS2FGwJdVjGGNPhNJuAROQmPK2fJcAbwJve752SQxzcPfFu3OrGjZuj1UeZ/ORkVh9o25F5xhjT0QXSAroFyFLVoao6QlWHq+qIYAfWnl09/Goy4jNIjUmlxl1DdFg0U5+eytLdS0MdmjHGdBiBJKAvgZJgB9KRRIZFcutZt1JYUUiYI4yEqAR6JfRi1nOzeH7j87Z8gzHGBCCQBLQLWCYi94jIbXVfwQ6svZs3Zh4JkQmM7jaarYVbGZQ6iDO7nclVL19F9vPZNjjBGGOaEUgC2ovn/k8EEF/vq1NLjEpk/pj5fPjlh9x61q28uvVVLhp4EX++4M+8u/tdhvxjCL9d/lv2luwNdajGGNMuNTsVj6+gSDygqloW3JCaFoqpeBpz4OgBBj88mFp3LZldMll3cB3/vuTfTOo9iTuX3ElObg4AZ3Y7k0sHXcr3x36ftNjgz+ZtjDHtRVNT8QQyF9ww4BkgxbupELhOVTe1apQBak8JCOCLI19w48IbeWPbG0SHRXPMdYwIZwRD0oZwZrcz6Z3Qm3d2v8OKL1eQHJ3MH8//I98681s2l5wxplM41bngHgNuU9U+qtoH+DHwrwAPPFNEckVkh4jc3UiZKSKyTkQ2icj7gdTbnvRJ6sOCKxfwyhWvkBLtydHVtdWsO7iOJ9c9ya+W/wqnw8mPz/kxqdGpfOf17zDooUEs2rEoxJEbY0xoBdICWq+qI5vb5ud9TmAbcAGexelWAVep6uZ6ZZLwTO0zU1X3iki6qja59nV7awHVV11bTWGFZzUJt9vN5S9czpq8NfRN6svO4p0nlL9m+DU8dvFjxITHtHWoxhjTJk61BbRLRO4Vkb7er5/hWbm0OeOBHaq6S1WrgeeB7AZlrsazIupegOaST3sX4YwgIz6DjPgMeib25K1r3qJ3Ym+OuY6x/nvr2XXzLnbdvIt3rnuH+Ih4ntvwHP3/1p+F2xeGOnRjjGlzgSSgG4A0PFPxvAKk4llKuzk98DxDVGefd1t9A4FkEVkmImtE5Dp/FYnIPBFZLSKrCwoKAjh0+9AlpguvXfkaRyqPMP/N+SRGJdIvuR/T+01n+03bOSPlDA6VH2L2/87moU8fCnW4xhjTphpNQCISJSJpqlqsqjer6mhVHQ38D3AsgLrFz7aG/X1hwBhgDjADuFdEBp7wJtXHVHWsqo5NS+tYo8hGdB3BU9lP8fG+j0n/UzpTn57KAysfQERY9d1VTOg1AYCbFt7EXUvusodYjTGdRlMtoAeByX62nw/8NYC69wG96r3uCRzwU2aRqpZ7l+JeDjR5b6kj+vrQr7P2e2u5e9LdFJQX8KO3f8SYx8ZwsOwg7173Lj+b/DMc4uCPK/7I9P9Mx+V2hTpkY4wJukYHIYjIZlUd0si+Tao6tMmKRcLwDEKYDuzHMwjh6vrDt0VkMPAQntZPBPApcKWqbmys3vY8CCFQq/av4uL/u5harWXRNYsYkzGGLQVbuPDZC9lXuo8e8T148+o3GdnttMvFxphOpqWDEPx1oQXyPgBU1QXcCLwNbAFeUNVNIjJfROZ7y2wBFgGf40k+jzeVfE4X43qM48MbPiQuIo6pT09l2Z5lDE4bzBe3fMHk3pPZf3Q/ox8bze2Lb2dt3lrWHVzHuoPrbAE8Y8xppakW0PvAHar6aYPt44D7VfXcNojvBKdDC6jO/tL9XPjshWwr2sZtZ9/Gz8/7OU6Hk4lPTOTzQ5+f0BUX4Yzg7ol3c8/ke4gKiwpR1MYYE7gWzYQgIuOBF4CngDXezWOB6/B0k33S+qE273RKQADFx4q5Y8kd/Hvtv+mT2IeHZj/E6O6jGfPYGMIcYfxu+u+Ij4hHVXl5y8s8t+E5MlMyeXj2w5zf/3xEmmqoGmNMaLV4Kh4RSQd+CAzzbtoEPBTK53VOtwRU58O9HzL/jflsKtjE3RPv5uKBFzP1P1MZ3X00b179pm+WhXd2vcMP3vwB2w9vZ0DyALKzsskelM3EXhNxOpwh/i2MMeZ4pzQXXHtzuiYg8MykcPPCm/nnmn8yb/Q8LhxwIVe/cjUDuwxk8bWL6R7fHYBKVyVPrnuS13Nf593d71JdW82Z3c7knxf9k3E9xoX4tzDGmK+c6kwIpo1EOCN4ZM4j3DPpHh777DFe2PwCOd/IYXfxbiY+MZG3d7zNfcvu4+zHz+bGt26kd2Jvtt+4naeyn+Jg2UHOevwsbnzrRkoqbf1AY0z7Zy2gdurPK/7MHUvuYFzGOG4afxO3vn0rh48dRhAm9p5I/+T+PPv5s6TGpPKXC//CnMw5/HzZz3no04eIjYhl1hmzyM7KZnbmbJKjk0P96xhjOqlW6YITkVhVLW/VyFqgsyQggJc2v8SNb91IQUUB14+8nsm9JzN74GzSY9MBWJu3lu+98T1WHVjF98d+n3/M+QdrDqzhsTWPsWDbAg6WHSTMEca5fc713CvKyqZPUp8Q/1bGmM7kVNcDmgA8DsSpam8RGQl8T1V/0PqhNq8zJSDwjJL7ybs/4Z9r/klydDIXDbyI7KxsZgyYQWxELLXuWu5ccid/WfkXHp3zKN8b+z0A3Opm1f5VvLb1NXJyc9hSuAWAUd1GkZ2VzaWDLmVk15E2is4YE1SnmoA+AeYCC1T1TO+2jao6rMk3BklnS0B1Ptn3CQ+vepg3tr1BcWUxDnEQ5ggDQBCSopIorChk2fXLmNR70gnv31603ZeMVny5AkUJd4T7ElBiZCK/OO8XzB8730bTGWNazSknIFU9S0TW1ktAza4HFCydNQHVcbldfPDFByzbs4zq2moAjlYf5Ym1T1DpqiQ2IpYN399A36S+jdaRX57PG9veYHvRdt+2T/Z/wtI9SxmXMY5HL3qU0d1H+31vWXUZb+94m5zcHJbuWcrQtKFkZ2VzSdYl9EhoONm5MaazO9UE9BLwFzxztp0N3AyMVdUrWzvQQHT2BNSY3cW7uf6161m+dznhjnCuHHYl3x/7fc7qeVZAy3+rKs9vfJ4fvf0jCioKSI7yP3ChtKqUGncNKdEpTO07lfWH1rPj8A4AxmWM8z2XNDRtqHXvGWNOOQGlAn/DMwu2AIuBW1S1qLUDDYQloMapKr9e/mt+98HvqKqtAqB7XHdeuuIl37IPzTlSeYQHP3mQ/HL/zxrHRcQx84yZTOo9iTBHGKrKlsItvu69T/d7Zm5KjUklwhkBQJgjjIm9JpKdlc2szFkkRCa0wm9rjOkIQvYgqojMxJO8nHgmGv19I+XGASuBb6jqS03VaQmoeaVVpdy15C7+ueafiAiqSte4rkSHRR9Xbmj6UO6/8H4GdjlhCaYWO3D0AG9se4PVB1b71jYqrynnnV3vUFBRQLgjnB+O+yH3z7g/oJaZMaZjO9UW0EDgEaCrqg4TkRHAJar6m2be58SzHMMFeNb9WQVcpaqb/ZRbAlQCT1gCaj1rDqzhryv/ylvb3+JI5REm9Z7kuzfkVjevb3udSlclP5n0E+6adFdQJzitddfy8b6PeWLtEzy57kmuHHYlT1/6tK+VZIw5PTWVgMICeP+/gDuAfwKo6uci8r9AkwkIGA/sUNVd3iCeB7KBzQ3K3QS8DNgcMq1sTMYYnv3as5RUlnDR/13Eh3s/pF9yPy4bdBkXDriQksoSblt8G/e9fx9Pr3+aa0dcy6WDLuXMbmdSUFHA67mvs2DbAvYc2eO3foc4OKfnOWRnZTO131Rcbhfv7HqHnK057D6ymwv6X0D2oGwGpw7G6XAyqfckJvWeRFaXLO5+925KKkt46YqXiAmPadsTY4xpFwJpAa1S1XENRsGtU9VRzbxvLjBTVb/jff3/gLNU9cZ6ZXoA/wtMA/4NvGEtoOCoqKngR4t+xH83/ZeSqhKiwqIYmjYUhzgoqSzhQNkByqrLAAh3hFPjrgGgd2Jvzux2pt8BBcdqjvHh3g8pryknPiIel9vFMdcxEiMT6ZvUl/WH1gPQL6kfqTGpvvcN7DKQ2PBY/vXZvxjRdQQ3nHmDPSRrzGnqVFtAhSIyAFBvZXOBvECO62dbw2z3AHCXqtY2NWJKROYB8wB69+4dwKFNQzHhMfzz4n/y0OyHWP7FcnJyc3yj11JjUhmQMoCq2ioKygv4ouQLXFUufnbuz/jllF82OZrtWM0x3t39Lq/nvk6EM4JLsi7hvL7nEeGMYH/pfhbkLuCd3e9wrOYY4On6W7RjEUXHighzhJFblMsti27hlkW3EBMe43u2CWB8xnhevuJlEqJs0IIxp6NAWkD9gceACUAxsBu4RlW/aOZ95wD3qeoM7+t7AFT1f+qV2c1XiSoVqADmqeprjdVrLaDgq6ipYO4Lc1m4YyF/OP8P3Dnxzlatv9Zdy4ovV/Da1tdYd2gdFTUVFFYUUnysGLe6Ac/M4OU15UQ4Ivif8/+H28657bg6CisKeWPbG7y1/S0OHzvs9zjJ0cn8+YI/W8vKmBA6lfWAnMDvVfUOEYkFHKp6NMCDhuEZhDAd2I9nEMLVqrqpkfJPYV1w7UZ1bTXffO2bPL/xea4efjXXDL+Gaf2mtelKrL9d/lvue/8+XG4XiZGJvgELbnVTXOlJVj3iezT60O2G/A0kRCaw+NrFDE4b3GZxG2O+0tIVUcNU1SUi76nqtBYeeDaebjYnnhFuvxWR+QCq+miDsk9hCahdqXXXcs+79/DI6kcoqy4jLiKOSb0nNZqE+if1J3tQNhN6TTiuK+1UHK44zKX/vZQ1eWt826pcVUSHRfP4JY9zxdArGu0iXH9wPTOenYHL7WLRtYsYm+H3/4AxJohamoA+U9XRInI/kAm8CPhmw1bVV4IRbHMsAbW9Slcl7+1+j5ytOXx64FNfN1l9qkpuUS7VtdV0ie7CuX3ODWiIdUp0CrMzZ3N+//MDbl1tyt/Ehc9eyLGaY7x1zVuc3fPsRsvuOLyDC565gMKKQmZnzkb83JqMDY/lwgEX2kOyxgTBqSagJ+ttVjz3bFRVb2j9UJtnCaj9Olp1lEU7FpGTm8OavDU0d38RPA+uHq0+Smx4LNP6TQto7aJIZyRD04bywMoHyK/I5/LBl/taQd1iu3Fx1sWc0/Mc36Sq+0v3862cb7G3ZK/f+gorCik6VkS4I5wpfaf4Vp5tKC0mjTsm3EHXuK7NxmiM8WhpAtqHZw444avEU0dV9S+tHWggLAGdXqprq1m2ZxmvbX2N93a/55tCqCkllSUUVxYT5gjztVjqRtDtL91PjbuGtJg0Lhp4EZcOupTz+5/f5LNGte5aVu5bSU5uDot2LOJotf/bnPtL9xMTHsPvz/8988bMs5kcjAlASxNQHp4ZEPwOp1bVX7VeiIGzBGTc6uaTfZ+Qk5vDa1tfI7coF4DR3Uczc8BMEqMSWZu3loU7FlJSVUJ0WDQXDriQXgm9fHX0SOjBJVmXMDh1cMCTpuYW5vL9N7/P0j1LGd9jPOMzxvv2DUgZwCVZl9A/uX/r/rLGdHCn1AUX1MhawBKQaSi3MNeXjFbuW4mi9E3qy0UDL6JPYh92Fe/i7Z1vc6TyCOC5X1VcWQzAGSlnMHfwXO6YeAcp0SnNHktVeW7Dc/xi2S989bnV7ft5ePpw34zgY7qPsRnBTafX0gTkm/mgPbEEZJpyqOwQr297nZzcHJbsXEJVbRXJUcnMGTjnuBbQ0aqjbD+8nW1F29hzZA8p0Sk8MPMBrhl+TYuSxs7DO8nJzSEnN4cP937oGyI+J3MOXWK6nHR9w9KHMTtzNklRSSf9XmPak5YmoBRV9f+EXwhZAjKBKqsuY/HOxby29TVPd1xlid9yNe4a3/RDU/pMYUrfKX7LxUfGM/OMmc1229U9JJuTm8O7u96l0lV5UnG71U2t1hLmCOO8PucxodcEnOIZUBEZFsm0ftMYmzHW7kGZDiFkyzEEgyUg09pWH1jN9974Hp/lfXbcPHiN6RLdhWHpw7hp/E1cOujSVl/C3K1uPt3/KTlbc3gt9zW2Fm49oUxGfAYXD7yYSwddytS+U4kMi2zVGIxpLZaAjGmGy+3iH6v+wb1L76W0qjTg98WGxzJ3yFwuG3QZFwy44LjRdrmFuby3+72TbgE1VP//aK3W4lY3qw6sYtGORb6JYGdlzmJ8xvhWbRX1TerLhQMuJDYittXqNJ2PJSBjAlTrrm22BQSwpXAL3875NmsPrsUhDtzqJjosmgsGXMCA5AG8tf0t3+i8YMhMyWRO5hyqXFWsz1/PhkMbGh0+fiqiwqI4v//5nlaW8+RaWeHOcCb3nsyg1EE2GKMTswRkTBCoKq9seYWbF91M3tE8hqUPo+hYEfnl+ZzX5zyys7KZM3AOXaJPfhBCYw4fO8xb298iJzeHpXuW4nK7AnpfTFgMP5n8E+aPnR/QNEmKsjZvrW+p9S9Kmpx7uEmZKZlkZ2WTlZrl25Yak8r0ftOJj4xvcb2mY7AEZEwQlVaV8vOlP+fvn/6d9Nh0fjXlV1w1/CriIuKCetyKmgrKq8ubLVdYUcid79zJG9veYGTXkfzxgj8yte9Uwp3hAR1HVSk6VhTQzBb1Ha3+amaM93a/d0KyjHBGcH7/85l1xiwSIxN924d3Hc7IriOt1XSasARkTBtYc2AN89+cz+oDq4l0RjK9/3Sys7K5JOsSusV1C2lsqsqrW1/l5oU3s//oft/Q9OysbGYMmBH0lkhZdZnvWSk4ftj6ruJdJ5Tvk9iH7Kxszu55tm+QR1xEHDMGzGj1QR8muEKWgERkJvA3PLNhP66qv2+w/xrgLu/LMuD7qrq+qTotAZn2rNZdy4d7P/Q9GLv7yG4E4ayeZ3Fp1qUMSh0UUD1D04dyRsoZrR5fRU0Fb+94m5zcHN7Y9gZFx4p8yfKSgYElSqfDyVk9ziItNu2U41FV9pXuo7q2GvAMBqk7f0t2LTlhAMfo7qP550X/tJnNO5CQJCDvWkLbgAuAfXjWA7pKVTfXKzMB2KKqxSIyC88Cdmc1Va8lINNRqCob8zf6klH9JSUCMSRtCNlZ2cc9B1SfiDCi6wgy4jNaFJ/L7eKjvR812RJpjEMcTOg1geysbC4ddGlQkmV5dflx957WHVzHjxf/mENlh/jhuB/yk8k/aXTiWNN+hCoBNbsiaoPyycBGVe3RVL2WgExHdeDoAQ6VHWq2nMvtYsWXK8jJzWH5F8up1domy4/vMZ7srGzG9/hqGHZMeAxjuo85qfs8Ow7voKy6rNmyFTUVLN65mJzcHNYf8nRY1CXL8/qcF/AxGzM0bWijM46XVJbws/d+xsOrHkZRzupxFtlZ2YzrMc7vEHRBGNVtVECzrJvgCFUCmgvMVNXveF//P+AsVb2xkfK3A4PqyjfYNw+YB9C7d+8xX3zR8hE5xnQkh48dZnvRdr/7atw1LP9iOTm5OXy6/9MT9idFJTE7czaXDLyEngk9Wy0mp8PJyK4jiQ6PZs+RPeRszQk4WQZCEM7pdc5X94D8tP6+OPIFS/cs5cMvP/T7oO5x8YqTUd1GMbn3ZDK7ZPrWhIoJj6F/cv+gzCgR7gxnVLdRAa2JdboLVQL6OjCjQQIar6o3+Sk7FfgHMElVi5qq11pAxpxof+l+dhbv9L2umw7o9W2vU1hR2OrHiwmPYcaAGWRnZTMkbQgiQkllyXExBCrcEU7fpL44Hc7j7gF9lvdZq8fdlhIiE5h1xiyys7LJ7JLpt0yEM4KhaUNP64EV7boLTkRGAK8Cs1R1W3P1WgIyJnC17lrW5K1pdB68liivKWfJziXk5Oaw/+j+VqkzNSaViwZeRHZWNgOSBwBwsOwgu4t3B/T+5OjkZidu3V+6n4PlB32vDx87zMp9K1l1YNVJzVYREx7D+B7jmdBzAuN6jCM2/MSZIkqrSlm0YxELti0gvzy/yfrSYtK4eODFZA/Kpl9SP9/29Nj002Lxw1AloDA8gxCmA/vxDEK4WlU31SvTG3gPuE5VVwRSryUgY9oHVWXtwbUcOHrglOo5UnmEhTsW8ua2NympalmiFISze55NdlY2Fw64sMkFCOvER8aTEZ9BpauSj7/8mPKa5p+pKq8uZ/HOxSzYtoDCikLCHeFM7TeVS7MuZXKfyYQ7jr//5VY3G/M34nQ4/XbHFR8r9vzu29/0OwVU3f29GQNmBPRcWWxEbKt2t7aGUA7Dng08gGcY9hOq+lsRmQ+gqo+KyOPA5UDdTR1XY4HWsQRkzOmppraGFV+uOOkuQ0XZXLC5Rd12w9KHkZ2VzcUDL260tREfEX/Ckhq17lo+3vexb8LYHYd3NHmc2PBYZpwxwzeqseFsFNW11aw5sOa4Z6XyyvJYuGMhqw+c3Ofd4NTBvufP6o8STI9NDygxtzZ7ENUY0ynsLdnLyn0rqXU3PxgiryyP17e9zvIvluNWd5Nl60bbXTTwIlJjUo/bp6psP7ydTfmb/L7XjZtV+1fx9s63OVTe/CjIOmGOMKb0ncJ5fc4jITIhoCmUCisKWbJrCR9/+fEJA0KiwqK4oP8FZGdlM63fNKLCovzWkRqTesojGeuzBGSMMY0oqijivd3vNdoFt690HwtyF7DqwKqgx5IQmcCobqM4s9uZuNXNwu0L2VHcdOuqKclRyYxIH8Gw9GEoypvb32x2Xr/EyERmZc7i0qxLmZU5i4TIhBYfHywBGWPMKdtfup93d7/LsZpjQam/xl3Dh3s/5K3tbwVlZnOHODi397nMzpxNmCPM78g7t7pZd3Adb25/k8KKQiKdkRy8/eAprcxrCcgYYzqIKlcVy/Ysa7XlPKpcVWwu3MwrW145qbWu6ugvTi1HWAIyxphOrtJVye8++B2///D3Aa15VSeYCaj5u1rGGGM6vKiwKH419VdcO+JaXtnySkADNYLNEpAxxnQiA7sM5O5Jd4c6DABafxIkY4wxJgCWgIwxxoREhxuEICIFfDVzQkulAq0/Q2Pr6ggxQseIsyPECB0jToux9XSEOFsjxj6q6nf1wg6XgFqDiKxubsqfUOsIMULHiLMjxAgdI06LsfV0hDiDHaN1wRljjAkJS0DGGGNCorMmoMdCHUAAOkKM0DHi7AgxQseI02JsPR0hzqDG2CnvARljjAm9ztoCMsYYE2KWgIwxxoTEaZuARGSmiOSKyA4ROWHeCfF40Lv/cxEZHYIYe4nIUhHZIiKbROQWP2WmiEiJiKzzfv08BHHuEZEN3uOfMBNsOzmXWfXO0ToRKRWRWxuUafNzKSJPiEi+iGysty1FRJaIyHbv9+RG3tvkNdwGcf5JRLZ6/01fFZGkRt7b5PUR5BjvE5H99f5NZzfy3lCfy//Wi3GPiKxr5L1tdS79fva0+bWpqqfdF54lwHcC/YEIYD0wpEGZ2cBCQICzgU9CEGd3YLT353hgm584pwBvhPh87gFSm9gf8nPp59//IJ4H4EJ6LoFzgdHAxnrb/gjc7f35buAPjfwOTV7DbRDnhUCY9+c/+IszkOsjyDHeB9wewPUQ0nPZYP/9wM9DfC79fva09bV5uraAxgM7VHWXqlYDzwPZDcpkA/9Rj5VAkoh0b1hRMKlqnqp+5v35KLAF6NGWMbSSkJ/LBqYDO1X1VGfMOGWquhw43GBzNvC09+engUv9vDWQaziocarqYlV1eV+uBHoG6/iBaORcBiLk57KOiAhwBfB/wTp+IJr47GnTa/N0TUA9gC/rvd7HiR/sgZRpMyLSFzgT+MTP7nNEZL2ILBSRoW0bGQAKLBaRNSIyz8/+dnUugStp/D94qM8lQFdVzQPPBwGQ7qdMezunN+Bp5frT3PURbDd6uwmfaKTLqD2dy8nAIVXd3sj+Nj+XDT572vTaPF0TkPjZ1nC8eSBl2oSIxAEvA7eqasMlCz/D05U0Evg78FobhwcwUVVHA7OAH4rIuQ32t6dzGQFcArzoZ3d7OJeBak/n9KeAC3iukSLNXR/B9AgwABgF5OHp3mqo3ZxL4Cqabv206bls5rOn0bf52dai83m6JqB9QK96r3sCB1pQJuhEJBzPBfCcqr7ScL+qlqpqmffnt4BwEUltyxhV9YD3ez7wKp4meH3t4lx6zQI+U9VDDXe0h3Ppdaiui9L7Pd9PmXZxTkXkm8BFwDXqvQHQUADXR9Co6iFVrVVVN/CvRo7dXs5lGPA14L+NlWnLc9nIZ0+bXpunawJaBWSKSD/vX8RXAgsalFkAXOcdwXU2UFLX9Gwr3v7gfwNbVPUvjZTp5i2HiIzH829W1IYxxopIfN3PeG5Mb2xQLOTnsp5G/8IM9bmsZwHwTe/P3wRy/JQJ5BoOKhGZCdwFXKKqFY2UCeT6CGaM9e81XtbIsUN+Lr3OB7aq6j5/O9vyXDbx2dO212awR1uE6gvPyKxteEZr/NS7bT4w3/uzAA97928AxoYgxkl4mq6fA+u8X7MbxHkjsAnPSJOVwIQ2jrG/99jrvXG0y3PpjSMGT0JJrLctpOcSTzLMA2rw/OX4baAL8C6w3fs9xVs2A3irqWu4jePcgaevv+7afLRhnI1dH20Y4zPea+5zPB+C3dvjufRuf6ruWqxXNlTnsrHPnja9Nm0qHmOMMSFxunbBGWOMaecsARljjAkJS0DGGGNCwhKQMcaYkLAEZIwxJiQsARnjh4h0qTd78cF6My6Xicg/gnTMW0XkumDUXe8YF4nIL4N5DGMCZcOwjWmGiNwHlKnqn4N4jDA8UwWN1q8mAA3GMWq9x5mojTxcakxbsRaQMSdBPGsKveH9+T4ReVpEFnvXcfmaiPzRu57LIu9UJ4jIGBF53zvB5NuNzBQ+Dc8UQi4RGSAin9U7ZqaIrGmqLhH5rois8k60+rKIxHi3PyUifxGRpXim1ldgGZ7pdYwJKUtAxpyaAcAcPNPRPwssVdXhwDFgjjcJ/R2Yq6pjgCeA3/qpZyKwBkBVdwIlIjLKu+9bwFPN1PWKqo5Tz0SrW/DMElBnIHC+qv7Y+3o1nlmZjQmpsFAHYEwHt1BVa0RkA56FuhZ5t28A+gJZwDBgiXcaOieeaVoa6o4ncdR5HPiWiNwGfAPPpJRN1TVMRH4DJAFxwNv16npRVWvrvc7HM7WKMSFlCciYU1MFoKpuEanRr26quvH8/xJgk6qe00w9x4Coeq9fBn4BvAesUdUiEclooq6ngEtVdb2IXI9n9dc65Q3KRnmPZ0xIWRecMcGVC6SJyDngmQJf/C+EtwU4o+6FqlbiacU8AjwZQF3xQJ63m+6aZmIaSBvOWG1MYywBGRNE6lmyeC7wBxFZj2fW4Ql+ii4EGi4+9hzeFTIDqOtePCtaLgG2NhPWVODNk/xVjGl1NgzbmHZCRF4F7lTvcs0icjuepSXubcVjdAX+V1Wnt1adxrSUJSBj2gkRyQK6qupybzIaAExT1cJWPMY4oEZV17VWnca0lCUgY4wxIWH3gIwxxoSEJSBjjDEhYQnIGGNMSHS4B1FTU1O1b9++oQ7DGGNMANasWVOoqmn+9gUtAYnIE3gmPMxX1WF+9gvwN2A2UAFcr6qfNSzXUN++fVm9enVrh2uMMSYIROSLxvYFswvuKWBmE/tnAZner3l4nvg2xhjTSQQtAanqcuBwE0Wygf+ox0ogqZFp6ls7Lmpqa4J9GGOMMc0I5SCEHsCX9V7v824LmuJjxQx7ZBgPf/pwMA9jjDEmAKFMQOJnm9+nYkVknoisFpHVBQUFLT5gcnQyCREJ3P/R/VTXVLe4HmOMMaculAloH9Cr3uuewAF/BVX1MVUdq6pj09L8DqYI2I/O+RH7yvfx9MqnT6keY4wxpyaUCWgBcJ14nA2UqKq/hbpa1dcGf40esT14dN2jVFRUBPtwxhhjGhG0BCQi/wd8DGSJyD4R+baIzBeR+d4ibwG7gB3Av4AfBCuW+sIcYfxg7A/47PBnLFy7EJsLzxhjQqPDTUY6duxYPdXngIqPFdPj/h5M6z6NJy95klPt1jPGGOOfiKxR1bH+9nXKqXiSo5O5MutK3t7/Nut2rKOmxoZlG2NMW+uUCQjgx5N+TK3W8sLuF9i5c6d1xRljTBvrtAloaPehTMuYxjM7n+HT/Z9y4IDfAXjGGBMye/bsYdCgQXznO99h2LBhXHPNNbzzzjtMnDiRzMxMPv30U8rLy7nhhhsYN24cZ555Jjk5Ob73Tp48mdGjRzN69GhWrFgBwLJly5gyZQpz585l0KBBXHPNNSH7A7xT3gOqs2HXBma9PIsKVwVPTnqSaaOmER8f3yp1G2NOL7cuupV1B9e1ap2juo3igZkPNLp/z549nHHGGaxdu5ahQ4cybtw4Ro4cyb///W8WLFjAk08+yZAhQxgyZAjXXnstR44cYfz48axduxYRweFwEBUVxfbt27nqqqtYvXo1y5YtIzs7m02bNpGRkcHEiRP505/+xKRJk1r1d6tj94AaMbDHQP5+1t9xq5ubP7mZ1ZtX2/0gY0y70q9fP4YPH47D4WDo0KFMnz4dEWH48OHs2bOHxYsX8/vf/55Ro0YxZcoUKisr2bt3LzU1NXz3u99l+PDhfP3rX2fz5s2+OsePH0/Pnj1xOByMGjWKPXv2hOR363DLMbSmyMhIRvUaxQNnPcD8FfO59ZNbeT75eQYPHBzq0Iwx7UxTLZVgioyM9P3scDh8rx0OBy6XC6fTycsvv0xWVtZx77vvvvvo2rUr69evx+12ExUV5bdOp9OJy+UK8m/hX6duAYFneYepZ0zlvjPv4/Piz/nPxv/YA6rGmA5jxowZ/P3vf/fdx1m7di0AJSUldO/eHYfDwTPPPENtbW0ow/Sr0ycgEaF3795cO+paRiaP5IntT7B993YbFWeM6RDuvfdeampqGDFiBMOGDePee+8F4Ac/+AFPP/00Z599Ntu2bSM2NjbEkZ6oUw9CaOj5T57nqkVXccewO/jp+T8lMTExKMcxxpjOwgYhBGjumLmM7TKWJ7Y/Qe6uXGsFGWNMEFkCqicsLIy7zrqLoqoint/xPIWFhaEOyRhjTluWgBrIHpXNWaln8dSOp9j+xfZ2eePOGGNOB0FNQCIyU0RyRWSHiNztZ3+iiLwuIutFZJOIfCuY8QQiPDycu8bfRXF1MU9se4KDBw+GOiRjjDktBXM5BifwMDALGAJcJSJDGhT7IbBZVUcCU4D7RSQiWDEFavaI2czpOYendjzFO1vfobraVk81xpjWFswW0Hhgh6ruUtVq4Hkgu0EZBeJFRIA44DAQmiei6omMjOQ3E35DWlQaP1/7c7bt3hbqkIwx5rQTzJkQegBf1nu9DzirQZmH8KyMegCIB76hqu6GFYnIPGAeQO/evYMSbEOD+g3il2f+ku+t+B6/Wvkrnur1FDExMW1ybGNM+7R+/fpWnTUgLCyMkSNHnvT7HnjgAebNm+f3M+mpp55i9erVPPTQQwHXd/3113PRRRcxd+7ck47lVASzBSR+tjUc1zwDWAdkAKOAh0Qk4YQ3qT6mqmNVdWxbLR4XFRXFVWdfxdX9rubFPS/y3CfP2bBsYzq51p6ypqX1PfDAA6fFjC0tSkAicl8AxfYBveq97omnpVPft4BX1GMHsBsY1JKYgiE+Pp4/zvwj/eP6c++n97K/YH+oQzLGdCLl5eXMmTOHkSNHMmzYMP773//y4IMPcuDAAaZOncrUqVMBePLJJxk4cCDnnXceH330UbP1qio33ngjQ4YMYc6cOeTn5/v2rVmzhvPOO48xY8YwY8YM8vLy2LJlC+PHj/eV2bNnDyNGjDjl36+lLaA1AZRZBWSKSD/vwIIr8XS31bcXmA4gIl2BLGBXC2MKih7pPXhg+gMcqjzEvUvuxe0+oYfQGGOCYtGiRWRkZLB+/Xo2btzIzJkzufnmm8nIyGDp0qUsXbqUvLw8fvGLX/DRRx+xZMmS42a9bsyrr75Kbm4uGzZs4F//+pdvraCamhpuuukmXnrpJdasWcMNN9zAT3/6UwYPHkx1dTW7dnk+nv/73/9yxRVXnPLv16IEpKqvB1DGBdwIvA1sAV5Q1U0iMl9E5nuL/RqYICIbgHeBu1S13T39efGoi7l8wOU8s/MZPtz6YajDMcZ0EsOHD+edd97hrrvu4oMPPvA7Pdgnn3zClClTSEtLIyIigm984xvN1rt8+XKuuuoqnE4nGRkZTJs2DYDc3Fw2btzIBRdcwKhRo/jNb37Dvn37ALjiiit44YUXAE8CCuQ4zWk2AYnI0yKSVO91sog8EUjlqvqWqg5U1QGq+lvvtkdV9VHvzwdU9UJVHa6qw1T12Rb+HkH34MUPEhMWw+3v3W7Dso0xbWLgwIGsWbOG4cOHc8899/CrX/3KbznPQOKT4+89qsrQoUNZt24d69atY8OGDSxevBiAb3zjG7zwwgts27YNESEzM/Okj9lQIC2gEap6pF6AxcCZp3zkDiYjMYN7J9zLqqJVPPLBI6EOxxjTCRw4cICYmBiuvfZabr/9dj777DPAc3/66NGjAJx11lksW7aMoqIiampqePHFF5ut99xzz+X555+ntraWvLw8li5dCkBWVhYFBQV8/PHHgKdLbtOmTQAMGDAAp9PJr3/961Zp/UBgw7AdIpLsTTyISEqA7zvt/Gjyj3j686f5zarfcMXoK+ie3D3UIRlj2lBYWFirD8NuyoYNG7jjjjtwOByEh4fzyCOeP37nzZvHrFmz6N69O0uXLuW+++7jnHPOoXv37owePdo3hdiCBQtYvXr1CS2nyy67jPfee4/hw4f7Bi8ARERE8NJLL3HzzTdTUlKCy+Xi1ltvZejQoYCnFXTHHXewe/fuVvn9m12OQUSuA+4BXvJu+jrwW1V9plUiOEnBXI4hECv2rGDy05O5rM9lPHfVc8etLGiMMeZ4p7Qcg6r+B5gLHALyga+FKvm0BxP6TuC7I77Ly1+8zLMfPmv3g4wxpoUCHQW3FXgFyAHKRKRtpiNop/4060/0iOnBr9b+inWb1lFTUxPqkIwxpsMJZBTcTXhaP0uAN4A3vd87rfioeO6fcj97y/fyyKZHyM3NbfUnpI0x5nQXyGCCW4AsVS0KdjAdydzRc7lkwyU8s+sZJnedjIgwaNAgnE5nqEMzxpgOIZAuuC+BkmAH0tE4nU7+Z+r/0C26Gzd9chMf7v+Q3NxcW8DOGGMCFEgC2gUsE5F7ROS2uq9gB9YRZPXO4olJT9Atphs3f3IzC3cvZPv27VRVVYU6NGOMafcC6YLb6/2K8H4ZL6fTydDeQ3lcHufmT27mztV3sr10OzPzZzK672gyMjKaHedvjDGdVbPPAfkKisQDqqplwQ2paaF+Dqght9vNnj17yCvK457V9/BB/gcA9I/rzwU9LuDG0TfSI60HCQkJdn/IGNPpNPUcUCAPog4DngFSvJsKgetUdVMAB54J/A1wAo+r6u/9lJkCPACEA4Wqel5Tdba3BASe+ZMOHTrEgQMH2F++n/cPvs/7h95nddFqukZ15c7hdzKl2xSio6NJTU0lJSXFkpExplM41QS0Avipqi71vp4C/E5VJzTzPiewDbgAz9pAq4CrVHVzvTJJwApgpqruFZF0Vc33V1+d9piA6hw5coQ9e/ZQW1uLiPB58ef8dv1v2XF0B5O7TuaaftcwOnU0TnGSmJhI7969CQ8PD3XYxhgTNE0loEBuUMTWJR8AVV0mIrEBvG88sENVd3mDeB7IBuovVnE1ngXp9nrrbjL5tHdJSUmMGjUKVaW2tpaBlQMZmjyU53Y8x2PbHuODQx+QGJ7IxPSJXNH3CkYeHcmAAQOIj48PdejGGNPmAklAu0TkXjzdcADX4lm5tDk98AzhrrMPOKtBmYFAuIgsA+KBv3mn/unQRISwsDDi4uIYPmQ41zuu5/I+l7OyYCXvH3qfDw59wOIDi7l7+N1c5r6Mrl27kpGR0aIp1Y0xpqMKJAHdAPwSz1Q8AMvxLKXdHH+fpg37+8KAMXhWRY0GPhaRlaq67biKROYB8wB69+5YswBFRUUxePBgtm7dyrTu05jWfRql1aX8ZO1P+M3nv2HX0V3c4r6FsrIyBgwYYKPmjDGdRqOfdiISBcSragFwc73tXYFjAdS9D+hV73VP4ICfMoWqWg6Ui8hyYCSee0c+qvoY8Bh47gEFcOx2JTIyksGDB1NYWEhJSQkiwoNnPchfN/2V/939v+wq28Wvz/w1VVVVZGZmEh0dHeqQjTEm6Jp6EPVBYLKf7ecDfw2g7lVApoj0E5EI4EpgQYMyOcBkEQkTkRg8XXRbAqi7w4mIiCAjI4PBgwczatQoenTvwe3DbudnI37GZ0WfceX7V/LBgQ/YunUrR44cCXW4xhgTdE0loEmq+krDjar6HHBucxWrqgu4EXgbT1J5QVU3ich8EZnvLbMFWAR8DnyKZ6j2xpP/NToWh8NBRkYGvXr14rI+l/GfSf8hMTyRGz+5kb9u/Cu5O3LJz+/Q4zGMMaZZTd1waOqOeEDLOKjqW8BbDbY92uD1n4A/BVLf6SYtLY2wsDBkj/Cfyf/hr5v/yjO7nmF32W7+oH+gqqqKnj172uAEY8xpqalEki8i4xtuFJFxQEHwQupckpOTGThwIIkxifxkxE+4Z/g9fJT/ETetvIndebvZvn07hw8ftoXvjDGnnaZaQHcAL4jIU8Aa77axwHV47ueYVhIbG8vQoUM5ePAgc5lLfHg89669l3kfzePBsx6kvLwcVcXpdJKcnEyXLl2IiYmxlpExpkNrNAGp6qfeFtAPgeu9mzcBZ3X0B0bbIxGhe/fuJCcn43Q6iQ2L5c7Vd/K1pV/jmv7XcHW/q4kLj6OgoICioiIcDgdpaWmkp6fb0G1jTIcU8GSk7UV7noqntVRVVbF161a2FW/jkdxHWHpwKYnhiVze53JGpYxiSNIQkiKSfC2g5ORkunfvTlRUVIgjN8aY453SXHDtTWdIQADV1dVs2bIFl8vFliNbeHTbo3yU/5Fvf8+YnkxIn8CUblMYnTKacGc4PXr0ID093brmjDHthiWgDqq6uprc3FxqampQVcpqythSsoXNRzazrngdnxZ8SpW7ivjweK4fcD3XZ15PXFwc/fv3t245Y0y70CoJSERivTMWhFRnSkAAtbW17N69m6NHj+J2u4/bV1lbycqCleTszeGD/A+YmTGTn438GbERsaSnp5OcnGyzKhhjQupUl2OYADwOxKlqbxEZCXxPVX/Q+qE2r7MlIPCsN3Tw4EHy8vJ83WuqSt2/nary1M6neHjrwwxJHML94+4nPTodgLCwMLp06eJLRtY9Z4xpS6eagD4B5gILVPVM77aNqjqs1SMNQGdMQHUqKyuprKyktrYWl8tFZWUlFRUVVFZWoqoszVvKvWvvxSEO5vScw9w+c+kf3x/wzL4gIiQlJZGQkEBcXBwREbbCujEmuE51PSBU9csGfznXtkZg5uRERUU1OtKtoKCAqUzl6dineXLHk7y691Ve2PMCo1NGc0XfK5jSbQphjjCKioooLi5GVXE4HERGRhIVFUV0dDRJSUk2ks4Y02YCaQG9BPwFeAg4G8/M2GNVNSQPo3bmFlBzDh8+zJ49e1BViquKyfkyh1e+eIUDxw7QJbILl/W+jHO7nktmQibhjhNXYhURkpOT6dmzZ5MrtVZXV1NWVua7L5WSkkJCQoJ17xljTnCqXXCpwN/wzIItwGLgFlUtau1AA2EJqGklJSXs2rXLN2ChVmv5OP9jXvriJT7K/whFCXeEkxmfydCkoQxJGsLgxMH0i++HU5yAJxHFx8f7uvpqa2t995zqrhcR8R3D4fDM6BQfH09UVBTh4eG+r8jISMLDwy05GdNJhWwYtojMxJO8nHhmuv59I+XGASuBb6jqS03VaQmoedXV1Rw4cIDDhw9T/983/1g+nxd/zqYjm9hcspmtJVspd3kGNsaGxTIhbQLndTuPiekTiQ9v+TLhInJcwnG73YSHhxMXF0d8fLwvURljTn+n2gIaCDwCdFXVYSIyArhEVX/TzPuceBaWuwDPwnOrgKtUdbOfckuASuAJS0Ctp7FEVMetbvaW72XTkU2sLVrLB/kfUFRVhFOcDEwYyJCkIQxJHMKA+AGkRaXRJbILYY4wjrmOUVBZwOHqw/SM6UlqVGrAMdUlpm7dutG9e3drGRlzmjvVBPQ+nolJ/3kyo+BE5BzgPlWd4X19D4Cq/k+DcrcCNcA44A1LQK2vurqa/fv3+wYfNMatbjYe2cgHhz5gY/FGNpds9rWQAAQh2hlNRW3Fce9Lj0pnSOIQ+sX3Iy0qjbTINM/3ekmrIYfDQUxMjC1Dbsxp7lRHwcV4Jyatv80VwPt6AF/We70Pz4qn9QPrAVwGTMOTgEwQRERE0K9fPzIyMigqKqKsrIxjx45RW1t7/L0ccTAieQQjkkcAX7WQviz/koLKAgoqCyhzldElsgtpUWkkRSSxt2yvr0vvg/wPqNXjB0gKQkpkii8hpUWmMSplFNO7T8dd5mbTpk2kpKQQHR1NZGTkcckoLCysycEQxpiOLZAEVCgiAwAFEJG5QF4A7/PXt9Lwz+8HgLtUtbaprhgRmQfMA+jdu3cAhzb+REZGkpGR4Xvtcrk4evQoR44cobS0FJfLdfz9Gzf0jetL37i+jdY5MX2i72e3uimuLvYlq7qv/Mp8CioLOFhxkPWH1/PK3le4f9P9ZPfO5pJel9Cnpo/vOaX6VJXu3bvTrVs366oz5jQUSBdcf+AxYAJQDOwGrlHVL5p5X7NdcCKym68SVSpQAcxT1dcaq9e64IJHVXG5XLhcLkpLS8nLy0NVT5gC6FS41c2qwlW89MVLvH/wfdy4SQxPZHDSYLISsoh2fjV10JCkIUzoOoGYaE9XnT04a0zH0+J7QN4BAr9X1TtEJBZwqOrRAA8ahmcQwnRgP55BCFer6qZGyj+F3QNqV9xuN4WFhRw8eNDXOmrNZHTo2CE+zP+QzUc2s6VkCzuP7jyhC69HTA/m9pnL1O5TiY7wJKdwRzhp0Wm+Lrr63XYigtPpJCwsjLCwMBISEqwbz5gQalECEpEwVXWJyHuqOq2FB56Np5vNiWeE229FZD6Aqj7aoOxTWAJqt2pqanwPn9bU1OB2u1HV454Vqrun5G++ukC41Y16e2ldbhfvH3qfl/a8xGeHPzuhbN+4vkzpOoXzup1HVkIWEc7jW0d1cYgIAwYMID6+5cPKjTEt19IE9JmqjhaR+4FM4EXANyRKVV8JRrDNsQTUftV14VVXV1NVVYXL5aKmpobq6uoTklP9xFVdXd1k62pH6Q42Hfmq4XzUdZQV+StYU7TG12JKDE8kLSqNnjE9GZw02POQbeIQEiI8MzRkZGTQtWtXu5dkTBs71VFwKUARnpFqiueejQIhSUCm/RIR3wwIsbGxAb+vtraWsrIyjhw5QmVlpW+7qlJdXU1mYiaZiZnHvee6M67jSOURVhauZG/5XgorC8mvzGdX2S6WHVoGgFOcXNLrEr6d+W0kTygqKsLpdPrqqOumq3tI1qYTMqZtNZWA0kXkNmAjXyWeOh1rFTvTrjmdThITE0lMTPS7v66rr35r/fDhw3AAZvSYcUI339Gao2wp2cLSvKW89uVrvLHvDb7W+2sMTx7uKxPljPINC0+JTCEiLAIRoUuXLiQmJjaaiGJiYo5LYsaYlmuqCy4PzwwIfodTq+qvghlYY6wLztSpra0lLy+PgoIC37aG3XgHjx3k8W2P8/q+108Y4FAnxhnDN/p9g//X//+REJHgd0g4eBJhXXdeWlqatZaMCcAp3QMKamQtYAnINFTXVVdeXs7Ro0d9Mz7UT0bFVcWU1pT6Xle4Kiio8jyjtKZwDUvylhAXFsc1/a9hUOIgv8eJCYthRPIIIsMicTqdpKenExER4evGi4qKsqRkTAMtTUBr66beaU8sAZnmqCplZWUUFhZSWlp6wowP/mwv3c6juY/y/qH3m6w7NiyWCekTmNJ1ChO7TiQhIsG3r245i5SUFOuqM8arpQkoRVUPBzWyFrAEZE5W3fpFx44d821TVd8KszU1Nb4h4/vK9x3XUqqvoLKA5YeW88GhDzhcfZgwCWNMlzFM6TaFqd2m+iZldTgcvu66sLAwnE6nr0UW6LB0h8NBdHQ0sbGxREdH+5a8AHxLXhjTEYRsOYZgsARkWpuqkpeXx8GDBwNKELVay4biDbx/8H3eP/Q+e8v34hQn07pPY26fuYxOGd2qXXEN70m53W6io6NJTU0lOTnZJnM17ZolIGMCcOzYMXbt2kV1dXVA5eu69HYd3UXOlzks+HIBR2uO0i26GxnRGaRHpX81Cav3KyYsJqC6u0Z1JTHC/6jAOvVbWpGRkURHR/u6/epadHUPCDudTpKTk0lISLCEZdqUJSBjAqSqVFVVNbq/7gFal8tFUVER5eXlvkRUWVvJ2/vfZmXhyuMmY612B5bQGuoZ05MhSUPoHdsb8Q5GDXOEcUb8GQxNGnpS6zDBVwkrIiKCqKgooqKiiIiIOG4ghdPp9LW2ROS4rj9jWsISkDFBUlZWxt69e6mqqvI7yEFVKa0p9SWjytpKP7Ucz42bL8u/9CxzcWQzhyoP+S1Xtw7TkCTPV8+Ynr7k4RQnKREpJ0xR1FDD1Wvrfx6oKuHh4cTHx58wp179+1thYWGWqEyjLAEZE0SqSklJCfv27fPNkxcslbWVbC3ZyuYjmz1fJZvZW7630fKJ4YmkR6UzIH6AL1ENiB9AXFjcSd2naizB1HX11bWW6regAMLDw0lMTCQ+Pp6YmBgbpt4JhSwBichM4G94JiN9XFV/32D/NcBd3pdlwPdVdX1TdVoCMu2VqlJcXMyBAwd83Xh1H9zBTEql1aVsKdlCQeVXD+TWuGsoqi6ioLKAQ8cOsa10G/mV+b79Uc6o41auTYtKIzUqlQjHVy2mGGeMb19yRLIveThwEB8eH3AyqWtlNTwHkZGRJCQkkJCQ4FtqQ1VxOp1ERkZasjpNhCQBeZdy2AZcgGc11FXAVaq6uV6ZCcAWVS0WkVl41g86y2+FXpaATEdQN+za5XJRWVnJ0aNHKS0tPW6uu+be73A4WjVxFVYWsunIJs8Kt1UFJywcWOVu/N5XQ10iuzA4cTBDkobQL66fL1ElhifiEE/SdYiDSEfzicRf68rhcJCSknLCKL+IiAjr7utgTnUy0pYaD+xQ1V3eIJ4HsgFfAlLVFfXKrwR6BjEeY9pM3bpEdX/NNzbPXWPcbrdvZoejR49SW1t73D632+2bHy/QdZpSo1I5r9t5fvepKmWuMlxul+c1Srmr3Lei7ZHqI76yLreLHUd3sPnIZj7K/8i3hIY/Uc4o0qPSSY1MJTrsq8UGIxwRpEamkh6dflxLLD0qnbjwONxuN/n5+RQWFh5Xn4jQtWtX0tPT7UHf00AwE1AP4Mt6r/cBTbVuvg0sDGI8xnQYDoeD+Pj4ZtcxqptJvLS0lKNHj/oSkapSU1ODiAS0LpOIEB9+/LFSIlPoFduryfeVu8rJq8jztKKqCiipLvkqNq3lcNVhCqoKKKwspLiq2LevsraS1UWrOVpz4vqWaZFpDE7ytK56xfTytajCHeGcEX8GtbW1HDx4kC5duhAfH09cXJw9mNtBBTMB+Z3E1G9Bkal4EtCkRvbPA+YB9O7du7XiM6bDa2omcVWloqLC14qqqqryDZKo3411sgsH1hcbFssZCWdwRsIZLXp/ZW2lr5VV93176XY2H9nM8kPL/b4nMTzRN+ovPTqd1KhUukV387WiYp2xx3X7iYhvVomYmJjjfvewsDAiIiIIDw9vtmuvrlvVhqe3nmAmoH1A/T+fegIHGhYSkRHA48AsVS3yV5GqPgY8Bp57QK0fqjGnHxEhNjaW2NhYunXr5tvudrupqak57quqqsqXoOpzOBy+r/qOHTvme2D3VO4jRzmj6BXby29Lq6ym7LiBE8dqj5FbksumI5vYUrKFTUc2+Z02KUzCcMpX3XNJEUmkRqX6uvfqH3tgwkCGJg+lf2x/wp2Nt6Ia/o5Op9P3PFVkZKTfJGYT1DYvmIMQwvAMQpgO7MczCOFqVd1Ur0xv4D3gugb3gxplgxCMaR+qqqo4fPgwxcXFvlVvm2oZNPysqf+6sZFyzalrQdUtSFhQVUBxVbHvvpSqcqT6iK+FVVFb4XtvWU0ZZa4ywJO0opxRfo8R7ggnNTL1hFkt6taTSotKIyUqhTDHiX/PqyoxMTHEx8f7HvgNCws7LinVPQx8ugrJIARVdYnIjcDbeIZhP6Gqm0Rkvnf/o8DPgS7AP7z/IK7GAjXGtC+RkZF0796d7t27A56WVVVV1QmJprFWVN0cdyKCy+WivLycsrIyysrKqKmpweVynTCBa133V90zR9ESTXJcMgMZSGVlZcD3vMCTHPZX7GfTkU1sK93W6IwVVbVVFFYVUlBZQG5pLoerDp8w8MIpThLCE3wzVogIKREpxw2uSItKIy06jaSIJN8NCgcOkiOS6RbTjS5JXXwrCdcNLomLizutn5+yB1GNMaeF+ve8GnYl1iWlhjM9lJeXU11dfVKtL5fbxeGqw+RX5vsSU35l/nHdgbXuWoqqi3wtM39Jq6GkiCRfskqNTKVnbE+GJg1lWMow+nTtQ0xMYPMIRkZGEhsb227uU4VqGLYxxrSZ+ve8TkZ1dTUlJSXHLddRX12iqmthhUs46dHppEenB3yMuqRVUFVw3Mg/l9tFUVXRVwMxvCMGt5Zspajqq1viXaO6NjutEnhaYnXdhd1iu9EzsSc94nuQEZ/BsPRh9Ejt0a66+ywBGWM6tYiICNLS0potV/dsVmVlJS6XyzeAo7q6mpqaGt9zWfXVdTE6nU7SHel0i+3WSO1fqWup1c1wsaVkC7uO7sKtzbfQarSGwspC1h9ezzt571Dj/qolGOWMYkaPGVydeTXnnnEukZGRfuuoS+RtMbTduuCMMaYN1I0+rK6u9ntfq64bsLy8nNLSUioqKnC5XCdMGHsyxyupKaGgsoCDxw7y/sH3Wbh/IZW1lfSJ7XPcg8H1xYbFeroCo9PpndSbu6ffTWzUybUq67PJSI0xpgOqe/aobtXeQNQlrLqpnOqG2JeWlrKvcB9vfPkGnxZ+6rc+xTMjRt30TG51U3hrIYkJJzeTR4N47B6QMcZ0NPWndGqpuq62tLQ0evToQc/UnlxVclWzrSpVpaSqBKcjeFMeWQIyxphOIioqigEDBvh96Li++sPdgzlowRKQMcZ0MpGRkY0OQmhL7WOguDHGmE7HEpAxxpiQ6HCj4ESkAPjiFKtJBQqbLRVaHSFG6BhxdoQYoWPEaTG2no4QZ2vE2EdV/T5o1eESUGsQkdXtfc65jhAjdIw4O0KM0DHitBhbT0eIM9gxWhecMcaYkLAEZIwxJiQ6awJ6LNQBBKAjxAgdI86OECN0jDgtxtbTEeIMaoyd8h6QMcaY0OusLSBjjDEhdtomIBGZKSK5IrJDRO72s19E5EHv/s9FZHQIYuwlIktFZIuIbBKRW/yUmSIiJSKyzvv18xDEuUdENniPf8JMsO3kXGbVO0frRKRURG5tUKbNz6WIPCEi+SKysd62FBFZIiLbvd+TG3lvk9dwG8T5JxHZ6v03fVVEkhp5b5PXR5BjvE9E9tf7N53dyHtDfS7/Wy/GPSKyrpH3ttW59PvZ0+bXZv2VAk+XLzxLgO8E+gMRwHpgSIMys4GFeBbHPRv4JARxdgdGe3+OB7b5iXMK8EaIz+ceILWJ/SE/l37+/Q/ief4gpOcSOBcYDWyst+2PwN3en+8G/tDI79DkNdwGcV4IhHl//oO/OAO5PoIc433A7QFcDyE9lw323w/8PMTn0u9nT1tfm6drC2g8sENVd6lqNfA8kN2gTDbwH/VYCSSJSPe2DFJV81T1M+/PR4EtQI+2jKGVhPxcNjAd2Kmqp/rA8ilT1eXA4Qabs4GnvT8/DVzq562BXMNBjVNVF6uqy/tyJdAzWMcPRCPnMhAhP5d1xDMF9RXA/wXr+IFo4rOnTa/N0zUB9QC+rPd6Hyd+sAdSps2ISF/gTOATP7vPEZH1IrJQRIa2bWQAKLBYRNaIyDw/+9vVuQSupPH/4KE+lwBdVTUPPB8EgL+1ndvbOb0BTyvXn+auj2C70dtN+EQjXUbt6VxOBg6p6vZG9rf5uWzw2dOm1+bpmoD8LXTRcLhfIGXahIjEAS8Dt6pqaYPdn+HpShoJ/B14rY3DA5ioqqOBWcAPReTcBvvb07mMAC4BXvSzuz2cy0C1p3P6U8AFPNdIkeauj2B6BBgAjALy8HRvNdRuziVwFU23ftr0XDbz2dPo2/xsa9H5PF0T0D6gV73XPYEDLSgTdCISjucCeE5VX2m4X1VLVbXM+/NbQLiIpLZljKp6wPs9H3gVTxO8vnZxLr1mAZ+p6qGGO9rDufQ6VNdF6f2e76dMuzinIvJN4CLgGvXeAGgogOsjaFT1kKrWqqob+Fcjx24v5zIM+Brw38bKtOW5bOSzp02vzdM1Aa0CMkWkn/cv4iuBBQ3KLACu847gOhsoqWt6thVvf/C/gS2q+pdGynTzlkNExuP5NytqwxhjRSS+7mc8N6Y3NigW8nNZT6N/YYb6XNazAPim9+dvAjl+ygRyDQeViMwE7gIuUdWKRsoEcn0EM8b69xova+TYIT+XXucDW1V1n7+dbXkum/jsadtrM9ijLUL1hWdk1jY8ozV+6t02H5jv/VmAh737NwBjQxDjJDxN18+Bdd6v2Q3ivBHYhGekyUpgQhvH2N977PXeONrlufTGEYMnoSTW2xbSc4knGeYBNXj+cvw20AV4F9ju/Z7iLZsBvNXUNdzGce7A09dfd20+2jDOxq6PNozxGe819zmeD8Hu7fFcerc/VXct1isbqnPZ2GdPm16bNhOCMcaYkDhdu+CMMca0c5aAjDHGhIQlIGOMMSFhCcgYY0xIWAIyxhgTEpaAjPFDRLrUm734YL0Zl8tE5B9BOuatInJdMOqud4yLROSXwTyGMYGyYdjGNENE7gPKVPXPQTxGGJ6pgkbrVxOABuMYtd7jTNRGHi41pq1YC8iYkyCeNYXe8P58n4g8LSKLveu4fE1E/uhdz2WRd6oTRGSMiLzvnWDy7UZmCp+GZwohl4gMEJHP6h0zU0TWNFWXiHxXRFZ5J1p9WURivNufEpG/iMhSPFPrK7AMz/Q6xoSUJSBjTs0AYA6e6eifBZaq6nDgGDDHm4T+DsxV1THAE8Bv/dQzEVgDoKo7gRIRGeXd9y3gqWbqekVVx6lnotUteGYJqDMQOF9Vf+x9vRrPrMzGhFRYqAMwpoNbqKo1IrIBz0Jdi7zbNwB9gSxgGLDEOw2dE880LQ11x5M46jwOfEtEbgO+gWdSyqbqGiYivwGSgDjg7Xp1vaiqtfVe5+OZWsWYkLIEZMypqQJQVbeI1OhXN1XdeP5/CbBJVc9ppp5jQFS91y8DvwDeA9aoapGIZDRR11PApaq6XkSux7P6a53yBmWjvMczJqSsC86Y4MoF0kTkHPBMgS/+F8LbApxR90JVK/G0Yh4Bngygrnggz9tNd00zMQ2kDWesNqYxloCMCSL1LFk8F/iDiKzHM+vwBD9FFwINFx97Du8KmQHUdS+eFS2XAFubCWsq8OZJ/irGtDobhm1MOyEirwJ3qne5ZhG5Hc/SEve24jG6Av+rqtNbq05jWsoSkDHthIhkAV1Vdbk3GQ0ApqlqYSseYxxQo6rrWqtOY1rKEpAxxpiQsHtAxhhjQsISkDHGmJCwBGSMMSYkLAEZY4wJCUtAxhhjQsISkDHGmJD4/wiL4s0VlNMIAAAAAElFTkSuQmCC\n",
+                        "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 432x288 with 2 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -435,15 +451,15 @@
             "id": "efa57176-8d9f-4df9-87dd-a3f818fd0578",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[1.0000000000000002, 0.9000000000000001, 0.8800000000000001, 0.8400000000000001, 0.7700000000000001, 0.7300000000000001, 0.7000000000000001, 0.67, 0.6500000000000001, 0.6400000000000001, 0.6200000000000001, 0.6000000000000001, 0.5700000000000001, 0.53, 0.5000000000000001, 0.5100000000000001, 0.49000000000000005, 0.45000000000000007, 0.44000000000000006, 0.41000000000000003, 0.4000000000000001, 0.4000000000000001, 0.4000000000000001, 0.41000000000000003, 0.41000000000000003, 0.41000000000000003, 0.4000000000000001, 0.41000000000000003, 0.4000000000000001, 0.4000000000000001, 0.39000000000000007, 0.39000000000000007, 0.39000000000000007, 0.37000000000000005, 0.37000000000000005, 0.34, 0.34, 0.33000000000000007, 0.32000000000000006, 0.32000000000000006, 0.31000000000000005, 0.29000000000000004, 0.29000000000000004, 0.29000000000000004, 0.28, 0.27, 0.26000000000000006, 0.27, 0.27, 0.27, 0.27, 0.27, 0.27, 0.27, 0.26000000000000006, 0.26000000000000006, 0.26000000000000006, 0.26000000000000006, 0.24000000000000005, 0.23000000000000004, 0.22000000000000003, 0.22000000000000003, 0.22000000000000003, 0.22000000000000003, 0.21000000000000002, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.17, 0.16000000000000003, 0.16000000000000003, 0.16000000000000003, 0.15000000000000002, 0.15000000000000002, 0.15000000000000002, 0.15000000000000002, 0.14, 0.14, 0.14, 0.14, 0.14, 0.13000000000000003, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002], [1.0000000000000002, 0.9300000000000002, 0.8800000000000001, 0.8400000000000001, 0.7900000000000001, 0.7300000000000001, 0.68, 0.6400000000000001, 0.6300000000000001, 0.6200000000000001, 0.6200000000000001, 0.5900000000000001, 0.5700000000000001, 0.55, 0.55, 0.53, 0.5200000000000001, 0.5000000000000001, 0.49000000000000005, 0.4800000000000001, 0.4700000000000001, 0.4700000000000001, 0.45000000000000007, 0.45000000000000007, 0.45000000000000007, 0.4600000000000001, 0.45000000000000007, 0.44000000000000006, 0.44000000000000006, 0.43000000000000005, 0.4000000000000001, 0.39000000000000007, 0.39000000000000007, 0.37000000000000005, 0.37000000000000005, 0.38000000000000006, 0.38000000000000006, 0.38000000000000006, 0.35000000000000003, 0.35000000000000003, 0.35000000000000003, 0.34, 0.34, 0.34, 0.32000000000000006, 0.32000000000000006, 0.31000000000000005, 0.30000000000000004, 0.30000000000000004, 0.30000000000000004, 0.30000000000000004, 0.30000000000000004, 0.29000000000000004, 0.29000000000000004, 0.28, 0.27, 0.27, 0.27, 0.27, 0.27, 0.27, 0.27, 0.26000000000000006, 0.26000000000000006, 0.26000000000000006, 0.26000000000000006, 0.26000000000000006, 0.25000000000000006, 0.25000000000000006, 0.24000000000000005, 0.24000000000000005, 0.23000000000000004, 0.23000000000000004, 0.21000000000000002, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.17, 0.17, 0.16000000000000003, 0.16000000000000003, 0.16000000000000003, 0.16000000000000003, 0.15000000000000002, 0.15000000000000002, 0.14, 0.14, 0.14, 0.13000000000000003], [1.0000000000000002, 0.9500000000000002, 0.9100000000000001, 0.8000000000000002, 0.7800000000000001, 0.7200000000000001, 0.6500000000000001, 0.6300000000000001, 0.6300000000000001, 0.5900000000000001, 0.5800000000000001, 0.55, 0.53, 0.5000000000000001, 0.4800000000000001, 0.4700000000000001, 0.4700000000000001, 0.45000000000000007, 0.43000000000000005, 0.43000000000000005, 0.43000000000000005, 0.41000000000000003, 0.4000000000000001, 0.37000000000000005, 0.36000000000000004, 0.36000000000000004, 0.36000000000000004, 0.35000000000000003, 0.35000000000000003, 0.35000000000000003, 0.35000000000000003, 0.34, 0.34, 0.34, 0.34, 0.33000000000000007, 0.32000000000000006, 0.31000000000000005, 0.30000000000000004, 0.30000000000000004, 0.30000000000000004, 0.28, 0.28, 0.28, 0.28, 0.26000000000000006, 0.24000000000000005, 0.23000000000000004, 0.22000000000000003, 0.22000000000000003, 0.22000000000000003, 0.22000000000000003, 0.21000000000000002, 0.21000000000000002, 0.21000000000000002, 0.20000000000000004, 0.20000000000000004, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.17, 0.17, 0.17, 0.17, 0.17, 0.16000000000000003, 0.16000000000000003, 0.16000000000000003, 0.16000000000000003, 0.15000000000000002, 0.15000000000000002, 0.15000000000000002, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.13000000000000003, 0.13000000000000003, 0.13000000000000003, 0.13000000000000003, 0.13000000000000003, 0.13000000000000003, 0.13000000000000003, 0.11000000000000001, 0.11000000000000001, 0.11000000000000001, 0.11000000000000001]]\n"
+                        "[[1.0000000000000002, 0.9800000000000001, 0.8900000000000001, 0.8200000000000001, 0.7800000000000001, 0.7300000000000001, 0.7100000000000001, 0.67, 0.6600000000000001, 0.6200000000000001, 0.6100000000000001, 0.5900000000000001, 0.5900000000000001, 0.5800000000000001, 0.5900000000000001, 0.54, 0.5000000000000001, 0.4700000000000001, 0.4600000000000001, 0.4600000000000001, 0.45000000000000007, 0.45000000000000007, 0.43000000000000005, 0.43000000000000005, 0.43000000000000005, 0.39000000000000007, 0.38000000000000006, 0.36000000000000004, 0.34, 0.34, 0.33000000000000007, 0.33000000000000007, 0.29000000000000004, 0.30000000000000004, 0.30000000000000004, 0.29000000000000004, 0.29000000000000004, 0.29000000000000004, 0.28, 0.29000000000000004, 0.26000000000000006, 0.26000000000000006, 0.26000000000000006, 0.26000000000000006, 0.25000000000000006, 0.25000000000000006, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.23000000000000004, 0.22000000000000003, 0.21000000000000002, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.20000000000000004, 0.19000000000000003, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.17, 0.16000000000000003, 0.15000000000000002, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.14, 0.13000000000000003, 0.13000000000000003, 0.13000000000000003, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002], [1.0000000000000002, 0.9700000000000001, 0.8700000000000001, 0.8400000000000001, 0.7700000000000001, 0.7500000000000001, 0.7000000000000001, 0.6400000000000001, 0.5900000000000001, 0.55, 0.53, 0.5200000000000001, 0.5200000000000001, 0.5000000000000001, 0.5000000000000001, 0.49000000000000005, 0.4700000000000001, 0.4600000000000001, 0.44000000000000006, 0.44000000000000006, 0.43000000000000005, 0.42000000000000004, 0.42000000000000004, 0.41000000000000003, 0.39000000000000007, 0.39000000000000007, 0.39000000000000007, 0.38000000000000006, 0.37000000000000005, 0.37000000000000005, 0.37000000000000005, 0.37000000000000005, 0.37000000000000005, 0.37000000000000005, 0.36000000000000004, 0.36000000000000004, 0.36000000000000004, 0.34, 0.32000000000000006, 0.31000000000000005, 0.29000000000000004, 0.29000000000000004, 0.29000000000000004, 0.29000000000000004, 0.29000000000000004, 0.29000000000000004, 0.28, 0.28, 0.27, 0.26000000000000006, 0.25000000000000006, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.23000000000000004, 0.23000000000000004, 0.23000000000000004, 0.23000000000000004, 0.22000000000000003, 0.22000000000000003, 0.22000000000000003, 0.21000000000000002, 0.21000000000000002, 0.21000000000000002, 0.21000000000000002, 0.21000000000000002, 0.21000000000000002, 0.21000000000000002, 0.20000000000000004, 0.19000000000000003, 0.19000000000000003, 0.19000000000000003, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.17, 0.17, 0.15000000000000002, 0.15000000000000002, 0.14, 0.15000000000000002, 0.15000000000000002, 0.15000000000000002, 0.15000000000000002, 0.15000000000000002, 0.14, 0.14, 0.14, 0.13000000000000003, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.11000000000000001, 0.10000000000000002, 0.10000000000000002, 0.09000000000000001, 0.09000000000000001], [1.0000000000000002, 0.9200000000000002, 0.8500000000000001, 0.8100000000000002, 0.7800000000000001, 0.7400000000000001, 0.6900000000000001, 0.6500000000000001, 0.5700000000000001, 0.56, 0.54, 0.5200000000000001, 0.5000000000000001, 0.4800000000000001, 0.4600000000000001, 0.4600000000000001, 0.44000000000000006, 0.43000000000000005, 0.41000000000000003, 0.41000000000000003, 0.4000000000000001, 0.39000000000000007, 0.38000000000000006, 0.37000000000000005, 0.37000000000000005, 0.37000000000000005, 0.35000000000000003, 0.35000000000000003, 0.35000000000000003, 0.34, 0.34, 0.32000000000000006, 0.31000000000000005, 0.31000000000000005, 0.31000000000000005, 0.29000000000000004, 0.29000000000000004, 0.29000000000000004, 0.27, 0.26000000000000006, 0.26000000000000006, 0.26000000000000006, 0.25000000000000006, 0.25000000000000006, 0.25000000000000006, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.25000000000000006, 0.24000000000000005, 0.24000000000000005, 0.24000000000000005, 0.23000000000000004, 0.23000000000000004, 0.22000000000000003, 0.22000000000000003, 0.23000000000000004, 0.21000000000000002, 0.20000000000000004, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.18000000000000002, 0.17, 0.17, 0.17, 0.18000000000000002, 0.18000000000000002, 0.17, 0.17, 0.17, 0.16000000000000003, 0.15000000000000002, 0.14, 0.14, 0.14, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.12000000000000002, 0.11000000000000001, 0.11000000000000001, 0.10000000000000002, 0.08000000000000002, 0.08000000000000002, 0.08000000000000002, 0.08000000000000002, 0.07, 0.07, 0.06000000000000001, 0.06000000000000001, 0.06000000000000001]]\n"
                     ]
                 }
             ],
             "source": [
                 "print(S.results[Tree])"
             ]
         },
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986532981248055%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'data': {'text/plain': ['<mobspy.modules.meta_class.Reactions at "*

 * *            "0x7fc0ef2a1610>']}}}}, 11: {'outputs': [], 'source': {insert: [(1, 'Ecoli(50), "*

 * *            "Strepto(25), Glucose(10), Amino(100)\\n'), (2, '\\n'), (3, 'S = Simulation(Ecoli | "*

 * *            "Strepto | Glucose | Amino)')], delete: [3, 1, 0]}}, 13: {'outputs': {1: {'text': "*

 * *            "{insert: [(2, 'Amino,100\\n'), (3, 'Ecoli,50\\n'), (4, 'Glucose,10\\n'), (5, "*

 * *            "'Strepto,25\\n')], […]*

```diff
@@ -39,15 +39,15 @@
             "execution_count": 2,
             "id": "f9687e7a-abc5-4fde-a61c-aa8b6a2e8181",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fec96aa6a90>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7fc0ef2a1610>"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -126,34 +126,20 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "5f0c9765-b7d0-4e26-98ed-8660fcd74f26",
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "(<mobspy.modules.meta_class.Species at 0x7fec96a7f760>,\n",
-                            " <mobspy.modules.meta_class.Species at 0x7fec96aa6370>,\n",
-                            " <mobspy.modules.meta_class.Species at 0x7fec96a7ffa0>,\n",
-                            " <mobspy.modules.meta_class.Species at 0x7fec96aa66a0>)"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "S = Simulation(Ecoli | Strepto | Glucose | Amino)\n",
-                "\n",
                 "# Adding some counts\n",
-                "Ecoli(50), Strepto(25), Glucose(10), Amino(100)"
+                "Ecoli(50), Strepto(25), Glucose(10), Amino(100)\n",
+                "\n",
+                "S = Simulation(Ecoli | Strepto | Glucose | Amino)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2709519d-a951-4995-a3a3-d048f2b4a6c8",
             "metadata": {},
             "source": [
@@ -176,18 +162,18 @@
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "Species\n",
-                        "Amino,0\n",
-                        "Ecoli,0\n",
-                        "Glucose,0\n",
-                        "Strepto,0\n",
+                        "Amino,100\n",
+                        "Ecoli,50\n",
+                        "Glucose,10\n",
+                        "Strepto,25\n",
                         "\n",
                         "Mappings\n",
                         "Amino :\n",
                         "Amino\n",
                         "Ecoli :\n",
                         "Ecoli\n",
                         "Glucose :\n",
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/03_Characteristics.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/03_Characteristics.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998372395833333%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'data': {'text/plain': ['<mobspy.modules.meta_class.Reactions at "*

 * *            "0x7ff51e2a9670>']}}}}, 5: {'outputs': {0: {'data': {'text/plain': "*

 * *            "['<mobspy.modules.meta_class.Reactions at 0x7ff51e280e50>']}}}}, 8: {'outputs': {0: "*

 * *            "{'data': {'text/plain': ['<mobspy.modules.meta_class.Reactions at "*

 * *            "0x7ff523a39ca0>']}}}}}"}*

```diff
@@ -19,15 +19,15 @@
             "execution_count": 1,
             "id": "8a97e372-3f01-40f2-b3fc-c2309ba74efa",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7f9367aa3580>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7ff51e2a9670>"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -85,15 +85,15 @@
             "execution_count": 3,
             "id": "21118e41-f9f2-478b-bd73-9cf6ce5d4646",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7f9367a42220>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7ff51e280e50>"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -130,15 +130,15 @@
             "execution_count": 4,
             "id": "96ceda1e-c397-4e01-a815-bc7a262d2619",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7f9367aae070>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7ff523a39ca0>"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998611111111111%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'text\': {insert: [(2, "Characteristics: {\'aaa\', \'ccc\'}, '*

 * *            '{\'aaa\', \'bbb\'} \\n")], delete: [2]}}}}}'}*

```diff
@@ -19,15 +19,15 @@
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "\u001b[91mERROR: The same characteristic can only be shared through inheritance. There are two characteristics directly added to two meta-species \n",
                         "Repetition in: C, A \n",
-                        "Characteristics: {'aaa', 'ccc'}, {'bbb', 'aaa'} \n",
+                        "Characteristics: {'aaa', 'ccc'}, {'aaa', 'bbb'} \n",
                         "\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "from mobspy import *\n",
                 "\n",
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/05_For_Loops.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/06_Order_Matters.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'cells'": '{5: {\'outputs\': {0: {\'text\': ["[{\'characteristics\': \'std$\', \'quantity\': '*

 * *            '100}, {\'characteristics\': {\'red\', \'big\'}, \'quantity\': 150}]\\n"]}}}, 7: '*

 * *            '{\'outputs\': {0: {\'text\': ["[{\'characteristics\': \'std$\', \'quantity\': 100}, '*

 * *            "{'characteristics': {'red', 'big'}, 'quantity': 150}, {'characteristics': {'all$'}, "*

 * *            '\'quantity\': 10}]\\n"]}}}, 9: {\'outputs\': {0: {\'text\': ["[{\'characteristics\': '*

 * *            "'std$', ' […]*

```diff
@@ -78,15 +78,15 @@
             "id": "35b65938-1178-4b77-b019-1382c710fe09",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[{'characteristics': 'std$', 'quantity': 100}, {'characteristics': {'big', 'red'}, 'quantity': 150}]\n"
+                        "[{'characteristics': 'std$', 'quantity': 100}, {'characteristics': {'red', 'big'}, 'quantity': 150}]\n"
                     ]
                 }
             ],
             "source": [
                 "Tree.red.big(150)\n",
                 "print(Tree._species_counts)"
             ]
@@ -105,15 +105,15 @@
             "id": "5415163b-60e3-465d-8ed2-fe9dc3e6e72c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[{'characteristics': 'std$', 'quantity': 100}, {'characteristics': {'big', 'red'}, 'quantity': 150}, {'characteristics': {'all$'}, 'quantity': 10}]\n"
+                        "[{'characteristics': 'std$', 'quantity': 100}, {'characteristics': {'red', 'big'}, 'quantity': 150}, {'characteristics': {'all$'}, 'quantity': 10}]\n"
                     ]
                 }
             ],
             "source": [
                 "All[Tree](10)\n",
                 "print(Tree._species_counts)"
             ]
@@ -134,15 +134,15 @@
             "id": "643199fe-a82a-4ce5-91e3-0154fcfdce47",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[{'characteristics': 'std$', 'quantity': 100}, {'characteristics': {'big', 'red'}, 'quantity': 150}, {'characteristics': {'all$'}, 'quantity': 10}, {'characteristics': {'big', 'all$'}, 'quantity': 100}]\n"
+                        "[{'characteristics': 'std$', 'quantity': 100}, {'characteristics': {'red', 'big'}, 'quantity': 150}, {'characteristics': {'all$'}, 'quantity': 10}, {'characteristics': {'all$', 'big'}, 'quantity': 100}]\n"
                     ]
                 }
             ],
             "source": [
                 "All[Tree.big](100)\n",
                 "print(Tree._species_counts)"
             ]
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/09_Result_Data.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/09_Result_Data.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985591593013468%*

 * *Differences: {"'cells'": "{1: {'outputs': {insert: [(1, OrderedDict([('name', 'stdout'), ('output_type', "*

 * *            "'stream'), ('text', ['\\n', '\\n', '\\n'])]))]}}, 3: {'outputs': {2: {'data': "*

 * *            "{'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAZ0AAAEcCAYAAAAcM2nfAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjMuNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8QVMy6AAAACXBIWXMAAAsTAAALEwEAmpwYAABs8klEQVR4nO2dd3hU1daH3zWT3gmhJPRA6L2pgCggih17w4bKVakiKKgo92JBP0RUFAQFUUFRbFzlqlQLChJ6J5RQQwglkATS1/fHmcSgIZlAJpNJ9v […]*

```diff
@@ -24,14 +24,23 @@
                     "text": [
                         "Compiling model\n",
                         "Starting Simulator\n",
                         "Simulation is Over\n"
                     ]
                 },
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "\n",
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
                         "image/png": "iVBORw0KGgoAAAANSUhEUgAAAZwAAAEaCAYAAAAlqOH8AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjMuNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8QVMy6AAAACXBIWXMAAAsTAAALEwEAmpwYAAAe6klEQVR4nO3de5AV5Z3/8feHQYIiigmoqEHUIBZ3YSDeBTGRaGrdJHgrs1HZFGWMF+JqqZt1xdyqkvgzaKzokoghWbLB68qaiIrCJvGCmdFBQJQYJUIAQRNRNFEGvr8/Tg+L41yameme6ebzqjrl6T59+nyfeoQPT5/nPK2IwMzMLGvdOrsAMzPbNThwzMwsFw4cMzPLhQPHzMxy4cAxM7NcOHDMzCwX3Tu7gDT69u0bAwcO7OwyzMwshdra2tcjol/j/YUInIEDB1JTU9PZZZiZWQqS/tTUfl9SMzOzXDhwzMwsFw4cMzPLhQPHzMxy4cAxM7NcOHDMzCwXDhwzM8tFIX6HY2ZmO++NN95g4sSJAKxfv56qqir69av8HvPpp5+mR48eudbjwDEzK6mPfexj1NXVATB9+nT23HNPrrjiiu2v19fX0717fjHgS2pmZruQ888/n8svv5wJEyZw1VVX8cc//pFJkyYxZswYjj/+eF544QUANm7cyBe+8AXGjh3L2LFjefzxx9v92R7hmJnlYNr8adStr+vQc47afxQzJs3Y6fetXLmSBQsWUFVVxcSJE7ntttsYNGgQixcv5qKLLuKxxx7jsssu42tf+xrHHXccr776KqeccgorVqxoV70OHDOzXcwZZ5xBVVUVmzdv5oknnuCMM87Y/tp7770HwIIFC3j++ee373/rrbd4++236d27d5s/14FjZpaDtoxEstKrVy8Atm3bRp8+fbZ/z7Ojbdu28eSTT7L77rt32Of6Oxwzs13UXnvtxSGHHMJdd90FQESwZMkSAD796U9zyy23bD+2qVDaWZkGjqQ+ku6W9IKkFZKOlvT9ZPs5SfdJ6pNlDWZm1rw5c+Zw++23M3LkSIYOHcr9998PwM0330xNTQ0jRoxgyJAh3Hbbbe3+LEVEu0/S7Mml2cBvI+InknoAewDjgMciol7SdwEi4qqWzlNdXR2+H46ZWTFIqo2I6sb7MxvhSNoLOAG4HSAi3o+INyPi4YioTw57CjgoqxrMzKzryPKS2qHARuAOSc9K+omkXo2OmQI8mGENZmbWRWQZON2B0cCtEXEk8A5wdcOLkr4O1ANzmnqzpKmSaiTVbNy4McMyzcwsD1kGzhpgTUQsTrbvphJASDoP+CxwbjTzJVJEzIyI6oioblj7x8zMiiuzwImI9cBqSYOTXROB5yVNAq4C/iEi3s3q883MrGvJ+oeflwBzkhlqLwMXAL8HPgI8IgngqYi4MOM6zMysk2UaOBFRBzSeGveJLD/TzMy6Jq80YGZmuWhT4Eia3sF1mJlZybV1hFPboVWYmVnptSlwIuJ/OroQMzMrt1YDR9LsHRfYlLSPpFmZVmVmZqWTZoQzIiLebNiIiL8CR2ZWkZmZlVKawOkmaZ+GDUkfxTduMzOznZQmOP4f8ISku5PtM4BvZ1eSmZmVUauBExE/k1QLTAAEfD4inm/lbWZmZh+Q9tLYC8BfG46XNCAiXs2sKjMzK51WA0fSJcB1wGvAViqjnABGZFuamZmVSZoRzmXA4Ih4I+tizMysvNLMUlsNbMq6EDMzK7c0I5yXgUWSfgW817AzIm7MrCozMyudNIHzavLokTzMzMx2Wppp0dcDSOpd2YzNmVdlZmalk2YttWGSngWWAcsl1Uoamn1pZmZWJmkmDcwELo+IgyPiYOBfgB9nW5aZmZVNmsDpFRELGzYiYhHQK7OKzMyslFLNUpN0LfDzZPuLwCvZlWRmZmWUZoQzBegH3Js8+gIXZFmUmZmVT7MjHEk9gd4RsRG4dIf9+wF/S3Py5MZtPwGGUVkOZwrwIjAXGAisAs5M7rFjZmYl1tII52bg+Cb2nwz8IOX5bwLmR8QRwEhgBXA18GhEDAIeTbbNzKzkWgqc4yLi3sY7I2IOcEJrJ5a0V3Lc7cn73k/uHHo6MDs5bDbwjztXspmZFVFLkwbUwmtpvvs5FNgI3CFpJFBLZSHQ/SJiHUBErJO0b9pi26rf9/vx17/5qp2ZWWv22X0fNl65MZNztxQcGySNa7xT0lgqQdKa7sBo4NaIOBJ4h524fCZpqqQaSTUbN2bTeDMzy09LI5wrgTsl/ZTK6ASgGvgScHaKc68B1kTE4mT7biqB85qk/snopj+woak3R8RMKj86pbq6OlJ8XrOySmszM0uv2RFORDwNjKNyae385CHgkzuESLMiYj2wWtLgZNdE4HlgHnBesu884P421m5mZgXS4g8/I2IDlbt9ttUlwBxJPajc5uACKiF3p6R/prIK9RntOL+ZmRVEmpUG2iwi6qhchmtsYpafa2ZmXU+a2WZmZmbtljpwJHnBTjMza7M098M5RtLzVFYJQNJIST/KvDIzMyuVNCOcHwCnAG8ARMQSUqw0YGZmtqNUl9QiYnWjXVszqMXMzEoszSy11ZKOASKZ3nwpyeU1MzOztNKMcC4EvgocSGX1gFHJtpmZWWqtjnAi4nXg3BxqMTOzEkszS+1wSY9KWpZsj5D0b9mXZmZmZZLmktqPgWuALQAR8RzpFu80MzPbLk3g7JEs5Lmj+iyKMTOz8koTOK9LOgwIAEmTgXWZVmVmZqWTZlr0V6ncl+YISX8GXsGTCMzMbCe1GDiSqoCvRMTJyVpq3SLi7XxKMzOzMmk2cCR1j4h6SWMAIuKd/MoyM7OyaWmE8zQwGnhW0jzgLmB76ETEvRnXZmZmJZLmO5yPUlm48yQqEweU/NeBY2ZmqbUUOPtKuhxYxv8FTYPItCozMyudlgKnCtiTDwZNAweOmZntlJYCZ11EfCO3SszMrNRa+uFnUyMbMzOzNmkpcCbmVoWZmZVes5fUIuIv7T25pFXA21TuEFofEdWSRgG3AT2prMl2URNrtZmZWcmkmRbdXhOSe+o0+B5wfUQ8KOnUZHt8DnWYmVknSrN4Z0cLYK/k+d7A2k6owczMcpb1CCeAhyUF8B8RMROYBjwk6QYqgXdMxjWYmVkXkHXgHBsRayXtCzwi6QVgMvC1iLhH0pnA7cDJjd8oaSowFWDAgAEZl2lmZllTRD6/4ZQ0HdgMXAv0iYiQJGBTROzV0nurq6ujpqYmhyrNzKy9JNVGRHXj/Zl9hyOpl6TeDc+BT1NZJmctcGJy2EnAH7KqwczMuo4sL6ntB9xXGcTQHfhFRMyXtBm4SVJ34O8kl83MzKzcMguciHgZGNnE/t8BY7L6XDMz65o6Y1q0mZntghw4ZmaWCweOmZnlwoFjZma5cOCYmVkuHDhmZpYLB46ZmeXCgWNmZrlw4JiZWS4cOGZmlgsHjpmZ5cKBY2ZmuXDgmJlZLhw4ZmaWi9zu+NkekjYCf2rnafoCr3dAOV2R21ZMZW4blLt9blvLDo6Ifo13FiJwOoKkmqZueVoGblsxlbltUO72uW1t40tqZmaWCweOmZnlYlcKnJmdXUCG3LZiKnPboNztc9vaYJf5DsfMzDrXrjTCMTOzTuTAMTOzXJQqcCRNkvSipJckXd3E65J0c/L6c5JGd0adbZGibeMlbZJUlzz+vTPqbAtJsyRtkLSsmdeL3G+tta3I/fZxSQslrZC0XNJlTRxT5L5L075C9p+knpKelrQkadv1TRzT8X0XEaV4AFXAH4FDgR7AEmBIo2NOBR4EBBwFLO7sujuwbeOBBzq71ja27wRgNLCsmdcL2W8p21bkfusPjE6e9wZWluXP3E60r5D9l/THnsnz3YDFwFFZ912ZRjjjgJci4uWIeB/4JXB6o2NOB34WFU8BfST1z7vQNkjTtsKKiN8Af2nhkKL2W5q2FVZErIuIZ5LnbwMrgAMbHVbkvkvTvkJK+mNzsrlb8mg8g6zD+65MgXMgsHqH7TV8+H+ONMd0RWnrPjoZIj8oaWg+peWiqP2WVuH7TdJA4Egq/1LeUSn6roX2QUH7T1KVpDpgA/BIRGTed93b8+YuRk3sa5zYaY7pitLU/QyV9Ys2SzoV+G9gUNaF5aSo/ZZG4ftN0p7APcC0iHir8ctNvKVQfddK+wrbfxGxFRglqQ9wn6RhEbHjd40d3ndlGuGsAT6+w/ZBwNo2HNMVtVp3RLzVMESOiF8Du0nqm1+JmSpqv7Wq6P0maTcqfxnPiYh7mzik0H3XWvuK3n8AEfEmsAiY1OilDu+7MgXO74FBkg6R1AM4G5jX6Jh5wJeS2RdHAZsiYl3ehbZBq22TtL8kJc/HUenbN3KvNBtF7bdWFbnfkrpvB1ZExI3NHFbYvkvTvqL2n6R+ycgGSbsDJwMvNDqsw/uuNJfUIqJe0sXAQ1Rmdc2KiOWSLkxevw34NZWZFy8B7wIXdFa9OyNl2yYDX5FUD/wNODuSqSZdnaT/ojLbp6+kNcB1VL7ELHS/Qaq2FbbfgGOBfwKWJt8FAPwrMACK33eka19R+68/MFtSFZWQvDMiHsj670svbWNmZrko0yU1MzPrwhw4ZmaWCweOmZnlwoFjZma5cOCYmVkuHDhmHUTSx3ZYNXi9pD8nzzdL+lFn12fW2Twt2iwDkqYDmyPihs6uxayr8AjHLGPJPVMeSJ5PlzRb0sOSVkn6vKTvSVoqaX6ylAqSxkj6X0m1kh4qygrLZi1x4Jjl7zDgNCrLv/8nsDAihlP5pfppSej8EJgcEWOAWcC3O6tYs45SmqVtzArkwYjYImkplaWK5if7lwIDgcHAMOCRZJmuKqAQ64+ZtcSBY5a/9wAiYpukLTusvbWNyp9JAcsj4ujOKtAsC76kZtb1vAj0k3Q0VJbIL9KNvcya48Ax62KS24hPBr4raQlQBxzTqUWZdQBPizYzs1x4hGNmZrlw4JiZWS4cOGZmlgsHjpmZ5cKBY2ZmuSjEDz/79u0bAwcO7OwyzMwshdra2tcjol/j/YUInIEDB1JTU9PZZZiZWQqS/tTUfl9SMzOzXDhwzMwsFw4cMzPLhQPHzMxy4cAxM7NcOHDMzCwXDhwzM8uFA8fMzHLhwDEzs1w4cMzMLBcOHDOzLmTVqlUcccQRfPnLX2bYsGGce+65LFiwgGOPPZZBgwbx9NNP88477zBlyhTGjh3LkUceyf3337/9vccffzyjR49m9OjRPPHEEwAsWrSI8ePHM3nyZI444gjOPfdcOuNuz4VYS83MLG/T5k+jbn1dh55z1P6jmDFpRqvHvfTSS9x1113MnDmTsWPH8otf/ILf/e53zJs3j+985zsMGTKEk046iVmzZvHmm28ybtw4Tj75ZPbdd18eeeQRevbsyR/+8AfOOeec7etQPvvssyxfvpwDDjiAY489lscff5zjjjuuQ9vXGgeOmVkXc8ghhzB8+HAAhg4dysSJE5HE8OHDWbVqFWvWrGHevHnccMMNAPz973/n1Vdf5YADDuDiiy+mrq6OqqoqVq5cuf2c48aN46CDDgJg1KhRrFq1yoFjZtYVpBmJZOUjH/nI9ufdunXbvt2tWzfq6+upqqrinnvuYfDgwR943/Tp09lvv/1YsmQJ27Zto2fPnk2es6qqivr6+oxb8WGZfocjqY+kuyW9IGmFpKMlfT/Zfk7SfZL6ZFmDmVnZnHLKKfzwhz/c/j3Ms88+C8CmTZvo378/3bp14+c//zlbt27tzDI/JOtJAzcB8yPiCGAksAJ4BBgWESOAlcA1GddgZlYq1157LVu2bGHEiBEMGzaMa6+9FoCLLrqI2bNnc9RRR7Fy5Up69erVyZV+kLKaqSBpL2AJcGg08yGSPgdMjohzWzpXdXV1+AZsZmbFIKk2Iqob789yhHMosBG4Q9Kzkn4iqXHcTgEezLAGMzPrIrIMnO7AaODWiDgSeAe4uuFFSV8H6oE5Tb1Z0lRJNZJqNm7cmGGZZmaWhywDZw2wJiIWJ9t3UwkgJJ0HfBY4t7nLbRExMyKqI6K6X79+GZZpZmZ5yCxwImI9sFpSw7y9icDzkiYBVwH/EBHvZvX5ZmbWtWT9O5xLgDmSegAvAxcAvwc+AjwiCeCpiLgw4zrMzKyTZRo4EVEHNJ6p8IksP9PMzLomrzRgZtaMJUuWdOgv8rt3787IkSN3+n0zZsxg6tSp7LHHHh967ac//Sk1NTXccsstqc93/vnn89nPfpbJkyfvdC3t4dWizcya0dHLv7T1fDNmzODdd4v/lXebAkfS9A6uw8xsl/fOO+9w2mmnMXLkSIYNG8bcuXO5+eabWbt2LRMmTGDChAkA3HHHHRx++OGceOKJPP74462eNyK4+OKLGTJkCKeddhobNmzY/lptbS0nnngiY8aM4ZRTTmHdunWsWLGCcePGbT9m1apVjBgxot3ta+sltdp2f7KZmX3A/PnzOeCAA/jVr34FVNZG23vvvbnxxhtZuHAhffv2Zd26dVx33XXU1tay9957M2HCBI488sgWz3vffffx4osvsnTpUl577TWGDBnClClT2LJlC5dccgn3338//fr1Y+7cuXz9619n1qxZvP/++7z88ssceuihzJ07lzPPPLPd7WvTCCci/qfdn2xmZh8wfPhwFixYwFVXXcVvf/tb9t577w8ds3jxYsaPH0+/fv3o0aMHZ511Vqvn/c1vfsM555xDVVUVBxxwACeddBIAL774IsuWLeNTn/oUo0aN4lvf+hZr1qwB4Mwzz+TOO+8EYO7cuak+pzWtBo6k2Tuu6CxpH0mz2v3JZmb2AYcffji1tbUMHz6ca665hm984xtNHpf8pGSnNPWeiGDo0KHU1dVRV1fH0qVLefjhhwE466yzuPPOO1m5ciWSGDRo0E5/ZmNpRjgjIuLNHQr8K9Dy+M3MzHba2rVr2WOPPfjiF7/IFVdcwTPPPANA7969efvttwH45Cc/yaJFi3jjjTfYsmULd911V6vnPeGEE/jlL3/J1q1bWbduHQsXLgRg8ODBbNy4kSeffBKALVu2sHz5cgAOO+wwqqqq+OY3v9khoxtI9x1ON0n7JEGDpI+mfJ+ZWaF17969w6dFt2Tp0qVceeWVdOvWjd12241bb70VgKlTp/KZz3yG/v37s3DhQqZPn87RRx9N//79GT169Pb73sybN4+ampoPjYw+97nP8dhjjzF8+PDtkw0AevTowd13382ll17Kpk2bqK+vZ9q0aQwdOhSojHKuvPJKXnnllQ5pf6u3J5D0JSr3rLk72XUG8O2I+HmHVJCCb09gZlYczd2eoNWRSkT8TFItMAEQ8PmIeD6DGs3MrMTSXhp7Afhrw/GSBkTEq5lVZWZmpdNq4Ei6BLgOeA3YSmWUE0D7fwVkZma7jDQjnMuAwRHxRtbFmJlZeaWZFr0a2JR1IWZmVm5pRjgvA4sk/Qp4r2FnRNyYWVVmZlY6aQLn1eTRI3mYmZnttDTToq8HkNS7shmbM6/KzMxKJ81aasMkPQssA5ZLqpU0NPvSzMysTNJMGpgJXB4RB0fEwcC/AD/OtiwzMyubNIHTKyIWNmxExCKgV2YVmZlZKaWapSbpWqBh7bQvAh2zkpuZme0y0oxwpgD9gHuTR1/ggiyLMjOz8ml2hCOpJ9A7IjYCl+6wfz/gb2lOnty47SfAMCrL4UwBXgTmAgOBVcCZDbc+MDOz8mpphHMzcHwT+08GfpDy/DcB8yPiCGAksAK4Gng0IgYBjybbZmZWci0FznERcW/jnRExBzihtRNL2is57vbkfe8ndw49HZidHDYb+MedK9nMzIqopUkDLd00O813P4cCG4E7JI0EaqksBLpfRKwDiIh1kvZNW2xbTZs/jbr1dVl/jJlZ4Y3afxQzJs3I5NwtBc4GSeMi4ukdd0oaSyVI0px7NHBJRCyWdBM7cflM0lRgKsCAAQPSvq1ZDfcDNzOz5m3otiGzczd7i2lJ44A7gZ9SGZ0AVANfAs6OiMUtnljaH3gqIgYm28dTCZxPAOOT0U1/YFFEDG7pXL7FtJlZcTR3i+lmL40lI5txVC6tnZ88BHyytbBJ3r8eWC2pIUwmAs8D84Dzkn3nAfenboWZmRVWiz/8jIgNVO722VaXAHMk9aBym4MLqITcnZL+mcoq1Ge04/xmZlYQaVYaaLOIqKNyGa6xiVl+rpmZdT1pZpuZmZm1W+rAkeQFO83MrM3S3A/nGEnPU1klAEkjJf0o88rMzKxU0oxwfgCcArwBEBFLSLHSgJmZ2Y5SXVKLiNWNdm3NoBYzMyuxNLPUVks6BohkevOlJJfXzMzM0kozwrkQ+CpwILAGGJVsm5mZpdbqCCciXgfOzaEWMzMrsTSz1A6X9KikZcn2CEn/ln1pZmZWJmkuqf0YuAbYAhARzwFnZ1mUmZmVT5rA2aPxLQqA+iyKMTOz8koTOK9LOgwIAEmTgXWZVmVmZqWTZlr0V4GZwBGS/gy8gicRmJnZTmoxcCRVAV+JiJOTtdS6RYRvnWlmZjut2cCR1D0i6iWNAYiId/Iry8zMyqalEc7TwGjgWUnzgLuA7aETEfdmXJuZmZVImu9wPkpl4c6TqEwcUPJfB46ZmaXWUuDsK+lyYBn/FzQNItOqzMysdFoKnCpgTz4YNA0cOGZmtlNaCpx1EfGN3CoxM7NSa+mHn02NbMzMzNqkpRHOxPaeXNIq4G0qN2yrj4hqSaOA24CeVJbIuaiJpXPMzKxkmg2ciPhLB33GhOQWBw2+B1wfEQ9KOjXZHt9Bn2VmZl1UqltMd7AA9kqe7w2s7YQazMwsZ2l+h9MeATwsKYD/iIiZwDTgIUk3UAm8YzKuwczMuoCsA+fYiFgraV/gEUkvAJOBr0XEPZLOBG4HTm78RklTgakAAwYMyLhMMzPLmiLy+UmNpOnAZuBaoE9EhCQBmyJir5beW11dHTU1NTlUaWZm7SWpNiKqG+/P7DscSb0k9W54DnyayqoFa4ETk8NOAv6QVQ1mZtZ1ZHlJbT/gvsoghu7ALyJivqTNwE2SugN/J7lsZmZm5ZZZ4ETEy8DIJvb/DhiT1eeamVnX1BnTos3MbBfkwDEzs1w4cMzMLBcOHDMzy4UDx8zMcuHAMTOzXDhwzMwsFw4cMzPLhQPHzMxy4cAxM7NcOHDMzCwXDhwzM8uFA8fMzHLhwDEzs1w4cMzMLBe53WK6PSRtBP7UztP0BV7vgHK6IretmMrcNih3+9y2lh0cEf0a7yxE4HQESTVN3WO7DNy2Yipz26Dc7XPb2saX1MzMLBcOHDMzy8WuFDgzO7uADLltxVTmtkG52+e2tcEu8x2OmZl1rl1phGNmZp2oVIEjaZKkFyW9JOnqJl6XpJuT15+TNLoz6myLFG0bL2mTpLrk8e+dUWdbSJolaYOkZc28XuR+a61tRe63j0taKGmFpOWSLmvimCL3XZr2FbL/JPWU9LSkJUnbrm/imI7vu4goxQOoAv4IHAr0AJYAQxodcyrwICDgKGBxZ9fdgW0bDzzQ2bW2sX0nAKOBZc28Xsh+S9m2Ivdbf2B08rw3sLIsf+Z2on2F7L+kP/ZMnu8GLAaOyrrvyjTCGQe8FBEvR8T7wC+B0xsdczrws6h4CugjqX/ehbZBmrYVVkT8BvhLC4cUtd/StK2wImJdRDyTPH8bWAEc2OiwIvddmvYVUtIfm5PN3ZJH4y/0O7zvyhQ4BwKrd9hew4f/50hzTFeUtu6jkyHyg5KG5lNaLorab2kVvt8kDQSOpPIv5R2Vou9aaB8UtP8kVUmqAzYAj0RE5n3XvT1v7mLUxL7GiZ3mmK4oTd3PUFlOYrOkU4H/BgZlXVhOitpvaRS+3yTtCdwDTIuItxq/3MRbCtV3rbSvsP0XEVuBUZL6APdJGhYRO37X2OF9V6YRzhrg4ztsHwSsbcMxXVGrdUfEWw1D5Ij4NbCbpL75lZipovZbq4reb5J2o/KX8ZyIuLeJQwrdd621r+j9BxARbwKLgEmNXurwvitT4PweGCTpEEk9gLOBeY2OmQd8KZl9cRSwKSLW5V1oG7TaNkn7S1LyfByVvn0j90qzUdR+a1WR+y2p+3ZgRUTc2Mxhhe27NO0rav9J6peMbJC0O3Ay8EKjwzq870pzSS0i6iVdDDxEZVbXrIhYLunC5PXbgF9TmXnxEvAucEFn1bszUrZtMvAVSfXA34CzI5lq0tVJ+i8qs336SloDXEflS8xC9xukalth+w04FvgnYGnyXQDAvwIDoPh9R7r2FbX/+gOzJVVRCck7I+KBrP++9EoDZmaWizJdUjMzsy7MgWNmZrlw4JiZWS4cOGZmlgsHjpmZ5cKBY9ZBJH1sh1WD10v6c/J8s6QfdXZ9Zp3N06LNMiBpOrA5Im7o7FrMugqPcMwyltwz5YHk+XRJsyU9LGmVpM9L+p6kpZLmJ0upIGmMpP+VVCvpoaKssGzWEgeOWf4OA06jsvz7fwILI2I4lV+qn5aEzg+ByRExBpgFfLuzijXrKKVZ2sasQB6MiC2SllJZqmh+sn8pMBAYDAwDHkmW6aoCCrH+mFlLHDhm+XsPICK2Sdqyw9pb26j8mRSwPCKO7qwCzbLgS2pmXc+LQD9JR0Nlifwi3djLrDkOHLMuJrmN+GTgu5KWAHXAMZ1alFkH8LRoMzPLhUc4ZmaWCweOmZnlwoFjZma5cOCYmVkuHDhmZpYLB46ZmeXCgWNmZrlw4JiZWS7+PziByuR7vAU4AAAAAElFTkSuQmCC\n",
                         "text/plain": [
                             "<Figure size 432x288 with 2 Axes>"
                         ]
                     },
                     "metadata": {
@@ -88,16 +97,28 @@
                         "\u001b[91mWARNING: Time Series length is different. \n",
                         "MobsPy disregards time-series that have already finished during calculations\u001b[0m\n",
                         "\u001b[91mWARNING: Time Series length is different. \n",
                         "MobsPy disregards time-series that have already finished during calculations\u001b[0m\n"
                     ]
                 },
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "\n",
+                        "\n",
+                        "\n",
+                        "\n",
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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JE6fPl2qWjyIL4C1WIUPRxbYDGVIVlYW+/fvZ/369ezduxfv+fNpduedBG7aRPyYMex57TUCatc2uRpdSHHuteuAaYUcfxO4tvTluA673U61atUQES6udjEvtX+JTSc2MXL1SDJzMsnJyTHzO6VEWloa1157LW3atKFly5bMnTuXt956i0OHDtGjRw969OgBwMyZM2ncuDGXXXYZy5cvL7ZdVWXQoEE0b96ca6+9liNHjuSfW716NZdddhkdOnTgqquuIiEhga1bt9K5c+f8a+Lj42ndunXpf2HnyFbVKar6p6quztvcJaYykpqayubNm62/m9RU6vz73zR8+mkyatdm6+zZHO/bl6DgYBo1amQMjgspzuioquYWcjAXK9O0R1GzZs38970ie/Fcm+dYkbSC59Y+R3ZutpnfKSV++OEHoqKiWL9+PZs2baJPnz4MGTKEqKgoli5dytKlS0lISOCFF15g+fLlLFy4kC1bthTb7tdff8327dvZuHEj06dP5/fffwesp9fBgwczb948Vq9eTf/+/Xn22Wdp1qwZmZmZ7N5tBY7MnTuX22+/3aXfvQj+KyKPi0ikiITnbe4SU5lQVY4cOcKOHTvIyckhYPNmmvXrR9X580l48EG2zZhBZr16BAYGGoNTBhRndE6LSMzfDzqOnXGNJNfh5eVFRERE/h/VDXVuYHjz4Sw5vISXNr5Edk42R44c4dSpU25W6tm0atWKRYsW8fTTT/Prr78WOle2cuVKLr/8cqpVq4aPjw933HFHse3+8ssv3HXXXdjtdqKioujZ05oO2b59O5s2baJ37960bduWF198kQMHrHXLt99+O59//jlgGR1nPsdF3I/lTvsdK1R6NWDy0riY3Nxc4uPjOXjwIJqTQ82ZM2navz+2jAx2TJ3KoYEDEW9vAgICiImJMSHQZUBxgQTPA/8TkRf5a01BR2A0MMyFulxGZGQkycnJZGdno6rcHX03KVkpTI+bTpBXEMObD2f37t0mP9sF0LhxY1avXs2CBQsYPXo0V155Jc8///w/rjufJ8rC7lFVWrRowR9//PGPc3fccQe33XYbN998MyJCTMw/nqHKBFVtcL73iogdy0AdVNXrHCOkuVhBCfHA7ap6ojR0ViQyMzOJi4sjIyMDSUmh4ZgxhP36K8d792bf6NHkhIQgIvj7+9O4cWNjcMqIIn/KjmqhfYEewIeO7XLgFlVd4FpprsHb25sWLVoQHByc/w9sQOMB3Fn/Tj7d8ynvx71PTk4Ou3btMvM758mhQ4cICAigX79+jBgxgjVrrOz9wcHB+TXfL7roIpYtW8axY8fIysriiy++KLbd7t2789lnn5GTk0NCQgJLly4FoEmTJiQlJeUbnaysLDZv3gxAw4YNsdvtjBs3zp2jHETEW0SGiMg8xzZIRJx9qhkKFCwtMgpYrKoxwGLHvqEAqampbNmyhfT0dHz27KHZ/fcT+vvv7Bs5kj0vv5xvcPz8/IzBKWOKDZlW1U1YroEKg91up1GjRiQkJHD48GEAhrcYTmp2Ku/teI9g72Dubng3CQkJREVFuVnthePl5VXqIdNFsXHjRkaOHInNZsPb25spU6YAMGDAAK6++moiIyNZunQpY8eO5ZJLLrEW77Zvn183Z/78+cTGxvKf//znrHZvuukmlixZQqtWrfIDEAB8fHyYN28eQ4YM4eTJk2RnZzNs2DBatGgBWKOdkSNHsmfPnlL7GZwHUwBv4F3H/r2OYw8XdZMj7+G1wEvAcMfhG7Ee/gBmAcuAp0tVrQeTlJTE/v37UVVCf/6ZBs8/T66PDzumTCG1ffv863x9fWnSpIlJxlnGOFXa4II/pBTcA65KzZ6cnMyePXvIzc0lOzebUatHsSxxGWPbjOX6utcTExNDcHBwqX+uoXxT2qUNRGS9qrYp7lgh980DXgGCgRGO/pOsqmEFrjmhqlUKuXcAMACgbt26Hfbu3VsK36T8kpuby969e0lOTiY3O5vI6dOJmj6dtGbN2PV//0dWgUAiX19fmjZtWuwDlOH8KKr/lNWYsty6B8LCwmjevDk+Pj542715qf1LdI7ozH/W/4clh5awa9cuUxLZUBrkiEjDvB0RiQaKLIkqItcBR843tFpVpzkyIHTMy8pRUcnKymLbtm2cOHECTp2i4YgRRE2fzrFrr2X79OlnGRwfHx9jcNyIs6UNwlX1+N+ONVDVYv0VnuAe8PX1pXnz5uzZswdJESZ0nMDjKx7nmbXPEOAVkD8MN35fwwUwElgqIruxlhvUA4qrU9UVuEFErgH8gBAR+QRIFJFIVU0QkUjgSJGtVHBSU1PZuXMnOTk5+MbH03DECPz272ffiBEk3XEHOOZubTYbAQEBNGzY0BgcN+Lsf9H/ikhI3o6INAf+6+S9k4CngILrfWqoagKA47V6YTeKyAARiRWR2KSkJCc/7vyw2+00bNiQmjVrEugdyJud36RuYF1GxI7g9wO/ExcXR27uP5YsGQxOoaqLgRhgiGNroqpLi7lntKrWVtX6wJ1YReD6AfP5a571fuBblwkv55w6dSp//U3oL7/Q7P778UpOZsc775B05535BkdEiIiIoHHjxsbguBlnjc7LWIYnSEQ6YKX06FfcTZ7mHsirv9OoUSOq+FXhnYveobpfdQauGMhPu38yGQsMJcaRnf1eAFXNUNUNqroeuE9E7j7PZscDvUUkDqum1fhSkutRZGVlsXv3bmv9zfvv02j4cDJq12bbxx+T2vGv6QSbzUb9+vWpU6eOWfhZDnA24ef3jvDOn7AmNPuqapwTt3qkeyAkJITmzZvjHefN+13fZ9CKQTyx6glezHmRW223mrxMhpLwJNC9kONzgaVYxRGLRVWXYbmhUdVjQK/SkeeZqKplcE6dIvqFF6iybBnHrr6avc8+i/r55V/n5eVFTExMoUlmDe6hSKMjIm9jlafOIwTYDQwWEVR1SFH3q+porIWkiMjlWNE3/UTk/7DcAuMpp+6BvHmegPgApnWdxtCVQ3lm9TOkZqXS39bfZKA1OItdVVP+flBVT5VgnY7hbxw+fJj0gwdpOmAAfvHx7B8+nCN33XXW/I2/vz+NGjUy7rRyRnG/jb/HKJdWgsLxwOci8hCwj7/KYJcrbDYbDRo0wN/fn8lM5qnYp3hpw0ukZqUyzDaMevXqGcNjKA5vEQn8e+0cEQkGfNykyaNJS0vj8O7dxAwbhu/+/cS9+SYpF1+cfz5v/qZ27dqmf5ZDijQ6qjoLQEQCgXRVzXHs2wHfknyQp7oH8uZ5/P39ecP+Bs+tfo43t75JSnYKYxhjDI+hOD4A5onIY6oaDyAi9YF3HOcMJSAnJ4ed27bRYPRoAjdtYverr55lcGw2G3Xr1qVq1apuVGkoCmfHnYuBK4BUx74/1vxOF1eIKo+EhYXRqnkrxtvHE7Q2iBlxM0jJSmFCzwnUrVPX3fIM5RRVnSAiqcDPIhKE5a5OA8ar6hT3qvMsVJU9u3dTa9w4wn79lb2jRpHc868aeGb+xjNw1uj4qWqewUFVU0Wk0v1m/f39ad2yNS/6vEiwdzAf7fqI1B9TmdJnCvVq13O3PEM5RVWnAlMdRkcKm+MxFM+xY8cI/L//I+Lbb0l46CGOOirGiggBAQFm/sZDcDZkOk1E8pMWOcKmPa60QWng5eVF06ZNef6S5xnUbBD/O/g/7vvuPvYccGteL4MHoKqpxuCcH+np6ZyZOJHI6dM5esMNHHrUKmhss9moWrUqTZo0MQbHQ3D2tzQM+EJEDjn2IwH3pex1MzabjejoaJ4NfJYgryBe3fgqt31zG5/3/Zzo2tHulmcwVChyc3NJnDKFuuPHk3zppex95hkQQUSoVasW1asXurbcUE5xdp3OKhFpCjTBSuGxTVWzXKqsnCMi1KxZk6d7Pk2QdxAvrH2B6+ddz1e3fEWTOk3cLc/gAYiIr6pmuFtHeSdx3jzqjBpFWsuW7H7lFfDyyo8sDQsLc7c8Qwkp0r0mIj0drzcD1wONsVJ5XO84VukJCwtj+BXDmXjRRHam7OSaz69h676txd9oqFSIyIy/7QcBHlmTqiw5uXw51R5+mMzISHa+8Qbq54fdbqdJkybG4Hgoxc3pXOZ4vb6Q7ToX6vIo/P39ebzX40zrPo2Dpw9y61e3sn3PdpMyx1CQgyIyBUBEqmBFf37iXknlm8xdu/C/+WZyfX2Je/ttcqtU+WvRtolQ81iKW6fzguO1uGy4lR4vLy/u634fWZLFo8se5cH/PciM3jNo3NBUJTSAqo4RkVdFZCrQAStk+kt36yqv6LFj6JVX4pWWZpUmqFWLwMBAGjVqZIqueThO/TcUkaEiEiIW74vIGhG50tXiPA0RoX+3/jzf/nn+SPqDEb+MYNu2baYeTyVGRG7O24A/gYuBtYAaF/U5OHOGzKuvxnv/fna+/joZTZsSHh5O48aNjcGpADgbvdZfVd8UkauwyhA8CMzEchEYCmCz2Xi699MkpiXy7rZ3iVgTwfDs4TRp0gRf3xIlcTBUDK7/2/5arLLV12MtFP2qzBWVZ7KzybrtNnxiY9nz8sukdepEVGQkNWrUMJk/KgjOGp283/Y1wExVXS/mL+Cc+Pr68u9e/yYpPYlZu2YR4RvBPTn3EBMTQ1BQkLvlGcoQ45ouAbm5ZA8YgPf337NvxAhOXnUVDerXp0qVf1TiNngwzhqd1SLyE9AAGO1IVmgqmhVBREQEL3V9iWPpx5i4ZSJV/aqiqtSvX5/w8HB3yzOUMSIyCxiqqsmO/SrA66ra363CygtZWWTecw8+X3xBQv/+HL/nHhrHxBAYGOhuZYZSxlmj8xDQFtitqqdFpCoFSu2KSAtV3ewCfR5NdINoxncez79++xcvrHuBKj7WE1t6ejqRkZHGXVC5aJ1ncABU9YSItHOjnvLDmTNk3HgjvgsXcmDQII4/8gjNjDu6wuJUIIGq5qrqmrxOo6rHVHVDgUs+doU4T8dut9OiSQsmdppIncA6jIgdwbbkbSQmJhIfH29CqisXNsfoBgARCcf5h74Ki548SXqPHvgsWsTeUaM4/sgjNG3a1BicCkxpxfKaR/ZzEBAQQPPo5rxz8TsEeQUx5M8hHEg9wIkTJ9i+fTs5OTnulmgoG14HfheRcSIyDvgdeM3NmtxK9uHDpHfrhm9sLHvGjSP5zjtp0qQJPj6mzFBFprSMjnlkL4Jq1aoRHRHN2xe9TVZuFoNWDuJExglOnz7Nli1byMgwmVAqOqr6EXALkIhVnv1mVa20HoL0XbvI7toV37g4dk2YwKlrrzURnpUEs2qxDBARoqOjaVylMRM7TSTxTCLD/hzG6azTZGZmsmXLFk6dOuVumQYXICIhjtdw4DAwB5gNHHYcq3SkrFuHdO+O9+HDxL35JqmXX06TJk3w8/NztzRDGVBaRiezlNqpsHh5eREdHU27qu14qf1LbEnewug1o8nOzSY3N5edO3dy+PBhM89T8ZjjeF2NVf49b8vbrzSoKkeXLsXviiuwp6WxY+pUTnfuTOPGjfH393e3PEMZ4WxGgsVFHVPVi/9+3vBPgoODqVmzJj2jevJ0q6f57chvvLThJbJzs1FVEhIS2L17N7m5Jhq9oqCq1zleG6hqdIGtgapWmjoYqkrC118T1rcvarOxffp00lu2pHHjxiaPWiWjuCzTfg4XQISIVBGRcMdWH4gqE4UVjMjISPz8/Lil3i38q/G/+O+B/zLkzyEkZyaTm5vLyZMnzTxPBUREuopIoON9PxGZKCKVos55dnY2+2bOpEa/fmSHhLD9/ffJbNSIGLMOp1JS3EjnX1hugKbAGsf71cC3wDuulVYxEREaNmyIzWbjkcaP8Fzr51h7fC33/3Y/O07tQFXJyMhgy5YtpKSYIpMViCnAaRFpAzwF7KWYpQYiUkdElorIVhHZLCJDHcfDRWShiMQ5Xsvtkv0zZ86w/+23qfPoo2RGRbH9/ffJql2bhg0bmuwclZQijY6qvqmqDYARDndA3tZGVSeXkcYKh4+PDw0aNEBE6Fu3L9MvmU5mTib9l/dn4aGFgFUtMS4uzszzVByy1fpF3gi8qapvAsHF3QM8qarNsBKFDhSR5sAoYLGqxgCLHfvljmPHjpE4cSL1R47kdJMmbJ82jZxq1YiOjiYkJMTd8gxuwtlAgvdEZIiIzHNsg0TE26XKKjhhYWFUrVoVEaFllZZ8fOnHNA5pzOg1o3lr61vkaE7+PM+ePXvMPI/nkyIio4F+wPciYsdK/HlOVDVBVdc43qcAW4FaWIZrluOyWUBfV4k+H1SVffv2kfzhh9R74QVS27Yl7t13yQ0LM9U+DU4bnXexaoC8W+D9lOJuqgjuAVdSp04dfH19EREi/CJ475L3uKXeLXy06yOG/jmUk5knyc3NJTk5mS1btpCZaYIEPZg7gAzgIVU9jGU8/s/Zmx3zqO2AlUANVU0AyzBhZX4v7J4BIhIrIrFJSUkXKN85srOz2b59OxkLFtBg9GjSmjVj58SJaGAg9erVM8k7DYgzrhsRWa+qbYo7Vsh9kUCkqq5xJAldjfVU9gBwXFXHi8gooIqqPl1UWx07dtTY2IoXYZqTk8OuXbtIS0vLH818vfdrXt30KjX8a/B6x9dpFNIIsNLqNGzYkODg4rwyhgtFRFarakd364D80tY/Ay+p6lcikqyqYQXOn1DVIv+bl0X/OX36NHFxcfisW0fjxx6z5nCmTSM3LIy6desSERHh0s83lB+K6j/OjnRyRKRhgQajgWLzt3iqe6AssdvtxMTEnFUv5KZ6NzGtyzQycjJ4cPmDLDq0CLAMVFxcHMePH3enZEMpISLTnLjGG/gSmK2qebV3Eh0PdHkPdkdcp9I5jh49yrZt2/Dato2YIUPIqlqVHe+8Q25YGNWqVTMGx5CPs0ZnJLBURJaJyM/AEuDJknyQp7gH3IGIEBUVRXR0dH5p69ZVWvPJpZ8QExLDqDWjmLx1cv48T3x8PCdOnHCzakMp8F5RJx01qz4AtqrqxAKn5gP3O97fjxVN6hZUlb1797J//3689++n8cCB5Pr6EvfOO2RHRODr60vt2rXdJc9QDnHKvQYgIr5AE6zknttU1emFJJ7iHigPpKens2PHDrKzrQWjmTmZ/N/m/+PrfV/TpVoXXmz3IiE+IfmpdcykrGtwlXtNRAJVNc3Ja7sBvwIb+at+1TNYD26fA3WBfcBtqlrk8NcV/ScrK4u4uDjS09PxSkykycMPY09LsxZ+Oh6gmjdvbvKpVUKK6j8lSa3eAajvuKeNiOQlMSzuw8/pHlDVhPLiHigv+Pn50aJFi/x5Hh98eLb1szQLbcZrm17j3t/uZVy7cbSu0prdu3fTsGFDQkND3S3bUAwi0gV4HwgC6jrW6/xLVR8/1z2q+hvnzuDeq/RVOk9aWhpxcXHk5ORgT04mZtAgvE6eZMeUKaRHRyMi1K9f3/MNzrBhsG5d6bbZti1MmlTkJfHx8fTp04du3bqxYsUK2rRpw4MPPsgLL7zAkSNHmD17Ni1atGDw4MFs3LiR7Oxsxo4dy4033kh8fDz33nsvaWnWs83kyZPp0qULy5YtY+zYsURERLBp0yY6dOjAJ598UuZ1vZxNg/MxMAHoBnRybMU+BXqCe6A8kjfPU7169fw/iJvr3cz0LtNRVR75/RGm75hOVk4Wu3fvNotIPYM3gKuAYwCquh7o7lZF58mxY8fyy3LYUlOJGTIE3wMH2Pn665xu3hwRoWrVqiZS7QLZuXMnQ4cOZcOGDWzbto05c+bw22+/MWHCBF5++WVeeuklevbsyapVq1i6dCkjR44kLS2N6tWrs3DhQtasWcPcuXMZMmRIfptr165l0qRJbNmyhd27d7N8+fIy/17OjnQ6As215KsUuwL3AhtFZJ3j2DPAeOBzEXkIh3ughO1WeESEWrVqERAQQHx8PLm5ubSq0oo53efw6qZXeW/He/yR9Afj2o2DnRATE2NWeJdzVHX/354qPa6YUnZ2Nvv27UNVkfR0Gg0fTsD27eyaMIHUjtZzqK+vL3Xq1HGz0lKimBGJK2nQoAGtWrUCoEWLFvTq1QsRoVWrVsTHx3PgwAHmz5/PhAkTAMs1v2/fPqKiohg0aBDr1q3DbrezY8eO/DY7d+6cP8fWtm1b4uPj6datW5l+L2eNziagJpBQksbLs3vAU6hSpQr+/v758zxB3kGMazeOrtW78srGV7j7l7sZ1XIU13ItjRs3Nrmsyi/7HS42FREfYAhWNKdHceTIEStDRnY20aNHE7R2LXvGjePkpZcCYLPZaNSoUX5AjOH8KeiatNls+fs2m43s7GzsdjtffvklTZo0Oeu+sWPHUqNGDdavX09ubu5ZJSMKtmm328nOznbxt/gnzv5lRABbRORHEZmft7lSmOEv8uZ5goKC8jtzn1p9+LT7p8SExDBm3RieiX2G1ZtXc/r0aTerNZyDR4GBWEsGDgBtHfseQ05ODomJiWhODvXHjiXs11/Z9/TTnOjTB7D+GdarV8/z53E8hKuuuoq33347P03W2rVrATh58iSRkZHYbDY+/vjjcled2NmRzlhXijAUT948T1JSEocPHyYnJ4eogCimXjyVD3d+yPS46aw/sZ4XT73IXV3vMvVJyhmqehS4x906LoSkpCQ0N5c6r71G1R9+4ODAgRy99VbAcgdXqVKF8PBKWZfOLYwZM4Zhw4bRunVrVJX69evz3Xff8fjjj3PLLbfwxRdf0KNHj3Ln/XA6ZNrdVJaQaWdQVdLS0khMTOTkyZMAbDi+gefWPkfC6QQeavwQE2+cSFCAmeM5X0o7ZFpEGmOljqqhqi1FpDVwg6q+WFqfURQX2n9yc3PZsGEDVT/+mDoTJ3L4vvs4OHgwOOaofH19ad68uXGrGYDSyUhQWKPFrqY2uAYRISgoiIYNG9K6dWtq1apFhxod+Ozyz7im9jVM3zGdLu93YUvCFndLNfzFdGA0kAWgqhuAO92qqAQcO3YMr8OHiZoyheRu3c4yOGYex1ASLuSvpMjV1IaywcvLixo1atCyZUvaNmvLmz3e5JX2r7AnZQ+dPujEc4ueY8WBFWTnlv2EoeEsAlT1z78d84hfiqpy6NAhak2YgOTmsn/kyLMMTt26dc+arDYYiqJERiev8iGAqq4ufTmG8yVv9BMdHc2Iq0fw850/0zq8NS8vf5lLPriE8PHh3DjnRt5d9S47ju0wNXrKnqOO/IUKICK3UsJoUHdx/PhxApcvp8rixSQ8+CCZtWoB1t9cXokOg8FZnAokOJ/V1Ab34eXlRfuG7fn9sd/ZeWgn36z/hj8S/2DlgZXMj7OCDqMCo7iq0VX0btibXtG9qB5YaPo7Q+kxEJgGNBWRg8AePCCwQFVJ2LOHRuPHk163Lon33Zd/ztvbm3r16rlRncETcTZ6LW819XywVlOLiEeupq5MiAgxtWIYWWskYC3s+3Pnn/x3y3/5M+lPvtzyJTPXzwSgRdUWXBVzFVc2vJJL611KgHeAO6VXKBwF2x5T1Ssc3gKbI+t6uefkyZOEz5iB3/797Jg8GfXxAcw8juH8cTr3WkVYTV3Z8fLyokvTLnRp2gWA02dO89Omn1i0exErk1by9p9vM3HFRLxt3lwUeRFXRF/BlY2upHPtzthtdjer90xExEtVs0WkA4CzyT7LA6pK4ooVxMyYwfErriDl4osB62GmTp06JizfcF44a3QqxGpqw9kE+AfQt1Nf+nbqC0Di8US+2/AdP+//mZVHVzL217GM/XUswd7BXFzjYrrX7k7vhr1pVr0Z/v7+eHl5lXmyQA/kT6A9sNaxoPoLIN/wFEiCW+5IOXWKmi+9hNpsHHjiCYD8vGqVqT7O+vXrS3XlvpeXF23aFFn/slAmTZrEgAEDCAj4pxfiww8/JDY2lsmTJzvd3gMPPMB1113HrY61VmWFs0bnUeBN/lpN/RMetpraUDw1wmvw0OUP8RAPcfr0abbu28rCnQtZcWQFK5JWsPDAQsasGEOkfyQXVbuIi6pdRIdqHagZUBMRyTdAee8L2wICAggNDSUgIKCyGaxwrGSfPbGCCcTxWm6NTvLHH1P3t9/YP2wYWY4igwEBAdStW9fd0sqU0k4Vc77tTZo0iX79+hVqdDwJp4xORVhNbSgZAQEBdGjagXaN23Hq1CkSExPZmriVFUdX8GfSnyw6tIhv9n0DQA2/GrSu0ppWVVrRukprmoQ2wdvmXWi7J0+eJDExEYCgoCDCwsIIDQ3FxzFXUAGpLiLDsfIX5hmbPMptCGFqYiI1Xn6ZM9HRHLnTWk7k5eVFo0aNKtvDQpmTlpbG7bffzoEDB8jJyWHMmDEkJiZy6NAhevToQUREBEuXLmXmzJm88sorREZG0rhx42LTD6kqgwcPZsmSJTRo0OCsCNbVq1czfPhwUlNTiYiI4MMPPyQ5OZn777+fP/+0Iv3j4+O54YYb2LBhwwV9P2ej19y6mtrgPmw2G2FhYYSFhREdHc3Fxy4mKSmJ9Mx0tiZvZcPxDWxI3sDGExtZmLAQAB+bD01Dm55liKr5VctvMzfXqkd26tQpUlNT2b9/P15eXoSGhhIWFkZQUBB2e4WZQ7JjRX0W9p+63BqdjOefJyghge3Tp4OXFzabjcaNG+PlVZISXIbz4YcffiAqKorvv/8esB7UQkNDmThxIkuXLiUiIoKEhAReeOEFVq9eTWhoKD169KBdu3ZFtvv111+zfft2Nm7cSGJiIs2bN6d///5kZWUxePBgvv32W6pVq8bcuXN59tlnmTFjBpmZmezevZvo6Gjmzp3L7bfffsHfz9m/oOlYJavfA2s1tYjMAYzRqUR4e3tTs2ZNatSowZkzZ6ieVJ1Wx1txD/eQm5tLUnoSG05YBmjDiQ18Hv85n+z+BICa/jVpFdaKxqGNaRTciJiQGGr41cg3QFlZWRw9epTjx4+jqvj7++ePgvz9/T356TpBVf/jbhEl4czatVSZMYNj115Lart2+VVqzQLQsqFVq1aMGDGCp59+muuuu45LHRm8C7Jy5Uouv/xyqlWzHubuuOOOs0oYFMYvv/zCXXfdhd1uJyoqip49ewKwfft2Nm3aRO/evQErsWtkZCQAt99+O59//jmjRo1i7ty5zJ0794K/n7NGJ0BV//xbx/eI1dSG0ifPt1+vXj1q167NsWPHOHz4MDVsNejl14tekVbVisycTHac2pFviDYnb84fDQEEeQXRKKQRjYIb0SikETHBMTQMbkiQdxCnT5/mzJkzHD58GIDg4GDCwsIICQnxNFecZ1lLVXTgQHL9/TkwZAg2m42oqChTnbYMady4MatXr2bBggWMHj2aK6+8kueff/4f153Pg1hh96gqLVq04I8//vjHuTvuuIPbbruNm2++2VqCERNT4s/8O84aHY9dTW1wLXa7nerVq1OtWjVSUlI4fPgwqampqCo+dh9aVmlJyyot869PzUplV8ou4lLi2HXKev3fwf+RtvevSOIo/ygahjQkJjgm3xjVya5DSkoKqprvigsNDSU4OLi8u+I8qm5U5scfE/DHH+x7+mlyIiIIr1KF6tXNwuGy5NChQ4SHh9OvXz+CgoL48MMPAevBKyUlhYiICC666CKGDh3KsWPHCAkJ4Ysvvig2Iq579+6899573HfffRw5coSlS5dy991306RJE5KSkvjjjz+45JJLyMrKYseOHbRo0YKGDRtit9sZN24cd9xxR6l8P2eNjkeupjaUHSJCSEgIISEhZGRkkJiYyLFjx4C/5nAAgryDaBPehjbhf3UQVSUxPZG4U3HsTNmZ//r7kd/JUWs5mI/Nh+jg6LNGRY1DGxPuG46fn1++EQoMDCxXrjhVPe5uDU5z6hS2kSNJa9aMpJtvJsDfn3r16pWrn6c78PLyKvWQ6aLYuHEjI0eOxGaz4e3tzZQpUwAYMGAAV199NZGRkSxdupSxY8dyySWXEBkZSfv27fPr5syfP5/Y2Fj+85+zvbo33XQTS5YsoVWrVjRu3JjLLrsMAB8fH+bNm8eQIUM4efIk2dnZDBs2jBYtWgDWaGfkyJHs2bOnVL5/saUNHKupx6vqSHeupjalDTyPnJwcjh07RmJiItnZ2WcZH2fIzMlkT+oedqbsZOepncSlxLHz1E6OZhzNvybcJzzfRdc0zApeiKkaQ2hoKCEhIQQGBp7XqvnSLm3gbpzpP9lDh2J/+222zZxJZtu2tGjRwgQOGM6LovpPkX9Rnrya2uB+CnO9nTlzhpycHFT1rLU9YI14Cj4E+dh9aBLahCahZ5fjTc5MtozQqbh8Q/Tl3i/J2JMBQBWfKrSs0pI24W1oFdaKdjXaUTO8JsHBwQQFBZl/pIWxYQP2d97h6E03kd66NU1NpJrBRRT3V+Wxq6kN5YeCrrc8cnNzyc7OJjs7m6ysrLPeZ2Zm5h/LyckhOzsbVc0fsYT7hdPZrzMdI/56kMrRHPak7Dkreu7XxF8BsIudRsGNaB3emlZhrWhfvT3NazanatWqZ2nyNESkD9aibTvwvqqOP6+GcnPJffRRcoKDOThwIA0aNDApbgwuw9lHGY9bTW0o39hsNnx8fJyORDuXkcozUJmZmTT3bU5MaAy3NrgVVSU5I5mNJzayMXkjG09s5Pv93/NF/BeANRq6pf4tTL9ruiu/pstwuL3fAXpjZQlZJSLzVbXklftmzcL2xx/se/55ajRrRlhYWOmKNRgKUJzR8cjV1IaKh7NGKjc3lzNnzpCWlkZYahjVgqrRrUY3bDYb2bnZ7Dq1K380VMWnShmpdwmdgZ2quhtARD4DbgRKZnSOH0efeoq0Nm3IvfdeatasWfpKDYYCFGd0PHI1taHyYrPZCAwMJDAwMD/UNycnh9OnT5OWlkaV0Co0C2/GLdm3ePqcRS1gf4H9A8BFBS8QkQHAAODc+dJ++QVSUzkydiz1o6MrfaSawfUU1+tctpq61PzRBkMx2O12goODCQ4Ozj+WN1/kwRT7IKiq07CWOtCxY8fCHxL79iVnzx7qVatmauMYyoTi/spc8thTwB99NdAcuEtEmrviswyGwvDy8io2QWI55wBQp8B+beDQ+TTkVbNmeV9ga6hAFGd0XLWaOt8fraqZQJ4/2mAwOMcqIEZEGjhqXN2Jo7KvwVCeKdLouHA1dWH+6Fp/v0hEBohIrIjEJiUluUiKweB5qGo2MAj4Eaug4uequtm9qgyG4nHXTKpTgQkFfdIikiQie8/RXgRw9BznyjuerB08W39R2uuVpZDzQVUXAAucuXb16tVHK2j/Ac/WX1G1n7P/uMvolNgfrarVznVORGI9NWWJJ2sHz9bvydpLSkXtP+DZ+iujdneFqxh/tMFgMFRC3DLSceRzy/NH24EZxh9tMBgMFR+3rY4riT/aCaaVUjvuwJO1g2fr92TtpYmn/xw8WX+l015saQODwWAwGEoLswTZYDAYDGWGMToGg8FgKDM82uiISB8R2S4iO0VklLv1lAQRmSEiR0Rkk7u1lBQRqSMiS0Vkq4hsFpGh7tbkLCLiJyJ/ish6h/Z/u1uTOzF9yD1U5j7ksXM6jvxtOyhQTwS467zqibgBEekOpAIfqWpLd+spCSISCUSq6hoRCQZWA3094WcvVhrlQFVNFRFv4DdgqKqucLO0Msf0IfdRmfuQJ490PDp/m6r+ArgqzZBLUdUEVV3jeJ+ClYblH2mMyiNqkerY9XZsnvnkdeGYPuQmKnMf8mSj41T+NoNrEZH6QDtgpZulOI2I2EVkHXAEWKiqHqO9lDF9qBxQ2fqQJxsdU1jOzYhIEPAlMExVT7lbj7Ooao6qtsVKv9RZRDzKNVOKmD7kZipjH/Jko1Nq9UQMJcfhy/0SmK2qX7lbz/mgqsnAMqCPe5W4DdOH3Ehl7UOebHRM/jY34ZhI/ADYqqoT3a2nJIhINREJc7z3B64AtrlVlPswfchNVOY+5LFGx9PriYjIp8AfQBMROSAiD7lbUwnoCtwL9BSRdY7tGneLcpJIYKmIbMD6p7tQVb9zsya3YPqQW6m0fchjQ6YNBoPB4Hl47EjHYDAYDJ6HMToGg8FgKDOM0TEYDAZDmWGMjsFgMBjKDGN0DAaDwVBmGKPjYYhI1QIhlodF5KDjfaqIvOtufQZDecb0H/djQqY9GBEZC6Sq6gR3azEYPA3Tf9yDGelUEETkchH5zvF+rIjMEpGfRCReRG4WkddEZKOI/OBIv4GIdBCRn0VktYj86Ei3bjBUOkz/KTuM0am4NASuxUpV/wmwVFVbAWeAax0d523gVlXtAMwAXnKXWIOhnGH6j4vwcrcAg8v4n6pmichGwA784Di+EagPNAFaAgutNFDYgQQ36DQYyiOm/7gIY3QqLhkAqporIln61+RdLtbvXYDNqnqJuwQaDOUY039chHGvVV62A9VE5BKw0qyLSAs3azIYPAXTf84TY3QqKY7yxLcCr4rIemAd0MWtogwGD8H0n/PHhEwbDAaDocwwIx2DwWAwlBnG6BgMBoOhzDBGx2AwGAxlhjE6BoPBYCgzjNExGAwGQ5lhjI7BYDAYygxjdAwGg8FQZvw/JqgHJ4JmDHoAAAAASUVORK5CYII=\n",
                         "text/plain": [
                             "<Figure size 432x288 with 4 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -119,16 +140,23 @@
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "0f198b63-0238-4c20-b5e1-6cdfb81f17bb",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -157,19 +185,19 @@
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Tree: \n",
                         " [[60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0], [60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0], [60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0]]\n",
                         "Tree.not_sick: \n",
-                        " [[60.0, 42.0, 31.0, 27.0, 24.0, 19.0, 13.0, 11.0, 9.0, 5.0, 4.0, 2.0, 2.0], [60.0, 52.0, 43.0, 34.0, 26.0, 21.0, 12.0, 11.0, 10.0, 9.0, 4.0, 4.0, 2.0], [60.0, 43.0, 34.0, 23.0, 18.0, 11.0, 10.0, 8.0, 7.0, 5.0, 4.0, 4.0, 4.0]]\n",
+                        " [[60.0, 44.0, 41.0, 33.0, 26.0, 20.0, 13.0, 11.0, 10.0, 9.0, 6.0, 4.0, 4.0], [60.0, 52.0, 40.0, 32.0, 26.0, 20.0, 13.0, 11.0, 8.0, 4.0, 4.0, 4.0, 3.0], [60.0, 47.0, 38.0, 33.0, 21.0, 15.0, 13.0, 11.0, 9.0, 9.0, 8.0, 6.0, 2.0]]\n",
                         "Tree.sick: \n",
-                        " [[0.0, 18.0, 29.0, 33.0, 36.0, 41.0, 47.0, 49.0, 51.0, 55.0, 56.0, 58.0, 58.0], [0.0, 8.0, 17.0, 26.0, 34.0, 39.0, 48.0, 49.0, 50.0, 51.0, 56.0, 56.0, 58.0], [0.0, 17.0, 26.0, 37.0, 42.0, 49.0, 50.0, 52.0, 53.0, 55.0, 56.0, 56.0, 56.0]]\n",
+                        " [[0.0, 16.0, 19.0, 27.0, 34.0, 40.0, 47.0, 49.0, 50.0, 51.0, 54.0, 56.0, 56.0], [0.0, 8.0, 20.0, 28.0, 34.0, 40.0, 47.0, 49.0, 52.0, 56.0, 56.0, 56.0, 57.0], [0.0, 13.0, 22.0, 27.0, 39.0, 45.0, 47.0, 49.0, 51.0, 51.0, 52.0, 54.0, 58.0]]\n",
                         "Tree.sick.blue: \n",
-                        " [[0.0, 6.0, 10.0, 13.0, 14.0, 15.0, 16.0, 16.0, 18.0, 20.0, 20.0, 20.0, 20.0], [0.0, 1.0, 6.0, 7.0, 10.0, 12.0, 16.0, 16.0, 17.0, 18.0, 19.0, 19.0, 19.0], [0.0, 3.0, 5.0, 10.0, 14.0, 18.0, 18.0, 18.0, 18.0, 19.0, 20.0, 20.0, 20.0]]\n"
+                        " [[0.0, 6.0, 7.0, 8.0, 11.0, 12.0, 15.0, 16.0, 17.0, 17.0, 19.0, 19.0, 19.0], [0.0, 4.0, 7.0, 9.0, 12.0, 15.0, 17.0, 19.0, 19.0, 20.0, 20.0, 20.0, 20.0], [0.0, 2.0, 5.0, 9.0, 13.0, 17.0, 17.0, 17.0, 17.0, 17.0, 17.0, 17.0, 20.0]]\n"
                     ]
                 }
             ],
             "source": [
                 "R = S.results\n",
                 "print('Tree: \\n', R[Tree])\n",
                 "print('Tree.not_sick: \\n', R[Tree.not_sick])\n",
@@ -195,19 +223,19 @@
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Tree: \n",
                         " [60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0]\n",
                         "Tree.not_sick: \n",
-                        " [60.0, 42.0, 31.0, 27.0, 24.0, 19.0, 13.0, 11.0, 9.0, 5.0, 4.0, 2.0, 2.0]\n",
+                        " [60.0, 44.0, 41.0, 33.0, 26.0, 20.0, 13.0, 11.0, 10.0, 9.0, 6.0, 4.0, 4.0]\n",
                         "Tree.sick: \n",
-                        " [0.0, 18.0, 29.0, 33.0, 36.0, 41.0, 47.0, 49.0, 51.0, 55.0, 56.0, 58.0, 58.0]\n",
+                        " [0.0, 16.0, 19.0, 27.0, 34.0, 40.0, 47.0, 49.0, 50.0, 51.0, 54.0, 56.0, 56.0]\n",
                         "Tree.sick.blue: \n",
-                        " [0.0, 6.0, 10.0, 13.0, 14.0, 15.0, 16.0, 16.0, 18.0, 20.0, 20.0, 20.0, 20.0]\n"
+                        " [0.0, 6.0, 7.0, 8.0, 11.0, 12.0, 15.0, 16.0, 17.0, 17.0, 19.0, 19.0, 19.0]\n"
                     ]
                 }
             ],
             "source": [
                 "R = S.fres\n",
                 "print('Tree: \\n', R[Tree])\n",
                 "print('Tree.not_sick: \\n', R[Tree.not_sick])\n",
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990247140522875%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'data': {'text/plain': ['<mobspy.modules.meta_class.Reactions at "*

 * *            "0x7f887ca82dc0>']}}}}, 3: {'outputs': {0: {'data': {'text/plain': "*

 * *            "['<mobspy.modules.meta_class.Reactions at 0x7f887cab6fd0>']}}}}, 7: {'outputs': {1: "*

 * *            "{'text': {insert: [(2, 'The reactants C1.not_infect.old and V2 yield a rate constant "*

 * *            "of: 1.2100000000000002\\n'), (3, 'The reactants C1.not_infect.young and V2 yield a "*

 * *            "rate constant of: 1. […]*

```diff
@@ -16,15 +16,15 @@
             "execution_count": 1,
             "id": "98a8ca7b-c908-494b-86d8-c2fac76dcd7f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fd9c8281790>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7f887ca82dc0>"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -58,15 +58,15 @@
             "execution_count": 2,
             "id": "da60cebb-cd22-4ccc-8e43-5639175caf60",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<mobspy.modules.meta_class.Reactions at 0x7fd9c82a8940>"
+                            "<mobspy.modules.meta_class.Reactions at 0x7f887cab6fd0>"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -118,26 +118,26 @@
                         "Compiling model\n"
                     ]
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "The reactants C1.not_infect.old and V2 yield a rate constant of: 1.2100000000000002\n",
-                        "The reactants C1.not_infect.young and V2 yield a rate constant of: 1.2100000000000002\n",
                         "The reactants C1.not_infect.old and V1 yield a rate constant of: 0.8800000000000001\n",
                         "The reactants C1.not_infect.young and V1 yield a rate constant of: 0.8800000000000001\n",
-                        "The reactants C2.not_infect.old and V2 yield a rate constant of: 1.32\n",
-                        "The reactants C2.not_infect.young and V2 yield a rate constant of: 1.32\n",
-                        "The reactants C2.not_infect.old and V1 yield a rate constant of: 0.96\n",
-                        "The reactants C2.not_infect.young and V1 yield a rate constant of: 0.96\n",
+                        "The reactants C1.not_infect.old and V2 yield a rate constant of: 1.2100000000000002\n",
+                        "The reactants C1.not_infect.young and V2 yield a rate constant of: 1.2100000000000002\n",
+                        "The reactants C3.not_infect.old and V1 yield a rate constant of: 0.96\n",
+                        "The reactants C3.not_infect.young and V1 yield a rate constant of: 0.96\n",
                         "The reactants C3.not_infect.old and V2 yield a rate constant of: 1.32\n",
                         "The reactants C3.not_infect.young and V2 yield a rate constant of: 1.32\n",
-                        "The reactants C3.not_infect.old and V1 yield a rate constant of: 0.96\n",
-                        "The reactants C3.not_infect.young and V1 yield a rate constant of: 0.96\n"
+                        "The reactants C2.not_infect.old and V1 yield a rate constant of: 0.96\n",
+                        "The reactants C2.not_infect.young and V1 yield a rate constant of: 0.96\n",
+                        "The reactants C2.not_infect.old and V2 yield a rate constant of: 1.32\n",
+                        "The reactants C2.not_infect.young and V2 yield a rate constant of: 1.32\n"
                     ]
                 }
             ],
             "source": [
                 "\n",
                 "def infection_rate_1(r1, r2): \n",
                 "    factor = 1\n",
@@ -185,26 +185,26 @@
                         "Compiling model\n"
                     ]
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "The reactants C1.not_infect.old and V2 yield a rate constant of: 1.2100000000000002\n",
-                        "The reactants C1.not_infect.young and V2 yield a rate constant of: 1.2100000000000002\n",
                         "The reactants C1.not_infect.old and V1 yield a rate constant of: 0.8800000000000001\n",
                         "The reactants C1.not_infect.young and V1 yield a rate constant of: 0.8800000000000001\n",
-                        "The reactants C2.not_infect.old and V2 yield a rate constant of: 1.32\n",
-                        "The reactants C2.not_infect.young and V2 yield a rate constant of: 1.32\n",
-                        "The reactants C2.not_infect.old and V1 yield a rate constant of: 0.96\n",
-                        "The reactants C2.not_infect.young and V1 yield a rate constant of: 0.96\n",
+                        "The reactants C1.not_infect.old and V2 yield a rate constant of: 1.2100000000000002\n",
+                        "The reactants C1.not_infect.young and V2 yield a rate constant of: 1.2100000000000002\n",
+                        "The reactants C3.not_infect.old and V1 yield a rate constant of: 0.96\n",
+                        "The reactants C3.not_infect.young and V1 yield a rate constant of: 0.96\n",
                         "The reactants C3.not_infect.old and V2 yield a rate constant of: 1.32\n",
                         "The reactants C3.not_infect.young and V2 yield a rate constant of: 1.32\n",
-                        "The reactants C3.not_infect.old and V1 yield a rate constant of: 0.96\n",
-                        "The reactants C3.not_infect.young and V1 yield a rate constant of: 0.96\n"
+                        "The reactants C2.not_infect.old and V1 yield a rate constant of: 0.96\n",
+                        "The reactants C2.not_infect.young and V1 yield a rate constant of: 0.96\n",
+                        "The reactants C2.not_infect.old and V2 yield a rate constant of: 1.32\n",
+                        "The reactants C2.not_infect.young and V2 yield a rate constant of: 1.32\n"
                     ]
                 }
             ],
             "source": [
                 "\n",
                 "infection_dict = {'C1':{'V1':1.1 , 'V2':1.3 , 'V3':1.7}, \n",
                 "                  'C2':{'V1':1.4 , 'V2':1.1 , 'V3':1.9},\n",
@@ -246,14 +246,21 @@
                     "text": [
                         "Compiling model\n",
                         "Starting Simulator\n",
                         "Simulation is Over\n"
                     ]
                 },
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
                         "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
@@ -349,15 +356,15 @@
                 "Otherwise, if it is  1/([Time]), then the reactants are considered to represent the total amount. \u00a0\n",
                 "\n",
                 "Below, we show an example:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 8,
             "id": "728a8fd4-d6bf-4168-814f-cd8901dbce4c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999944885361552%*

 * *Differences: {"'cells'": '{4: {\'outputs\': {0: {\'text\': {insert: [(0, "{\'a3\', \'a1\', \'a2\'}\\n")], '*

 * *            'delete: [0]}}}}}'}*

```diff
@@ -64,15 +64,15 @@
             "id": "5391b29f-5a1d-42c7-94f5-90d83a53d75c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "{'a1', 'a2', 'a3'}\n",
+                        "{'a3', 'a1', 'a2'}\n",
                         "{'b1', 'b2', 'b3'}\n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/12_Born_Species.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/13_Events.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/13_Events.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990448915796137%*

 * *Differences: {"'cells'": "{1: {'outputs': {2: {'text': {delete: [1]}}, 4: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAYUAAAEGCAYAAACKB4k+AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjMuNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8QVMy6AAAACXBIWXMAAAsTAAALEwEAmpwYAAAzBklEQVR4nO3deXjU1fn//+edhbCEJYSsLNkJBAyLQakoikgDaqEKVfz4U6xWrdVaavut9mu1Xv1+1NZaldpqa+vWaqlKUXFDURBFBQHZd2QLeyCsAWKW+/dHJnQMASJkck4y9+O65srMe94zeWlI7jnL+xxRVYwxxhiACNcBjDHG+MOKgjHGmKOsKBhjjDnKioIxxpijrCgYY4w5Ksp1gNPRqVMnTU9Pdx3DGGOalPnz5+9S1YS6 […]*

```diff
@@ -51,21 +51,27 @@
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "Starting Simulator\n",
-                        "Running simulation in parallel\n",
                         "Simulation is Over\n"
                     ]
                 },
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -141,14 +147,15 @@
                         "\n",
                         "Reactions\n",
                         "reaction_0,{'re': [(1, 'A.a1'), (1, 'B.b1')], 'pr': [], 'kin': 'A.a1 * B.b1 * 0.01 * volume^-1'}\n",
                         "reaction_1,{'re': [(1, 'A.a2'), (1, 'B.b2')], 'pr': [], 'kin': 'A.a2 * B.b2 * 0.02 * volume^-1'}\n",
                         "\n",
                         "Events\n",
                         "event_0,{'trigger': '( ( (A.a1 + A.a2) <= 50 ) && ( (B.b1 + B.b2) <= 50 ) ) ', 'delay': '0', 'assignments': [('A.a1', '100'), ('A.a2', '100'), ('B.b1', '120'), ('B.b2', '120')]}\n",
+                        "\n",
                         "\n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -240,36 +247,35 @@
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "Compiling model\n",
                         "Starting Simulator\n",
-                        "Simulation is Over\n",
-                        "\u001b[91mERROR: At:             copier = getattr(x, \"__deepcopy__\", None) \n",
-                        "Line number: 151 \n",
-                        "Characteristic name __deepcopy__ in object A is not allowed. Please pick another name\u001b[0m\n"
-                    ]
-                },
-                {
-                    "ename": "SystemExit",
-                    "evalue": "1",
-                    "output_type": "error",
-                    "traceback": [
-                        "An exception has occurred, use %tb to see the full traceback.\n",
-                        "\u001b[0;31mSystemExit\u001b[0m\u001b[0;31m:\u001b[0m 1\n"
+                        "Simulation is Over\n"
                     ]
                 },
                 {
-                    "name": "stderr",
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "/Users/fabriciocravo/opt/anaconda3/lib/python3.8/site-packages/IPython/core/interactiveshell.py:3445: UserWarning: To exit: use 'exit', 'quit', or Ctrl-D.\n",
-                        "  warn(\"To exit: use 'exit', 'quit', or Ctrl-D.\", stacklevel=1)\n"
+                        "\n"
                     ]
+                },
+                {
+                    "data": {
+                        "image/png": "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\n",
+                        "text/plain": [
+                            "<Figure size 432x288 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "from mobspy import *\n",
                 "\n",
                 "A, B = BaseSpecies()\n",
                 "\n",
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.4.5/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987943672839505%*

 * *Differences: {"'cells'": "{1: {'outputs': {2: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAYUAAAEGCAYAAACKB4k+AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjMuNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8QVMy6AAAACXBIWXMAAAsTAAALEwEAmpwYAAAl50lEQVR4nO3deXhU9d3+8fcnCSSsErbIKqAsgghiVLa6YKkoKKCiiApWq9baKra/KrTW+rS19amt21PxUksLImBFRVGQVUTc0IAIIlsQkAiEENaQsCT5/P6YIQ0KJECGk5m5X9eVa2bOnDO5j5K553zPMubuiIiIACQEHUBERCoPlYKIiJRQKYiISAmVgoiIlFApiIhIiaSgA5yI+vXre4sWLYKOISISVRYuXLjV3Rsc7rmoLoUWLVqQkZERdAwRkahiZuuP9JyGj0RE […]*

```diff
@@ -27,16 +27,23 @@
                         "Compiling model\n",
                         "Compiling model\n",
                         "Starting Simulator\n",
                         "Simulation is Over\n"
                     ]
                 },
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -90,16 +97,23 @@
                         "Compiling model\n",
                         "Compiling model\n",
                         "Starting Simulator\n",
                         "Simulation is Over\n"
                     ]
                 },
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
```

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/images/Matching_Meta.png` & `mobspy-2.4.5/example_models/Tutorial Notebooks/images/Matching_Meta.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/Tutorial Notebooks/images/vectorial_space.png` & `mobspy-2.4.5/example_models/Tutorial Notebooks/images/vectorial_space.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/AB_2CD.py` & `mobspy-2.4.5/example_models/application_models/AB_2CD.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/AND_gate.py` & `mobspy-2.4.5/example_models/application_models/AND_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/CRISPR_Oscillator.py` & `mobspy-2.4.5/example_models/application_models/CRISPR_Oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/For_The_Trees.py` & `mobspy-2.4.5/example_models/application_models/For_The_Trees.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/NOR_gate.py` & `mobspy-2.4.5/example_models/application_models/NOR_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/donor_receptor.py` & `mobspy-2.4.5/example_models/application_models/donor_receptor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/oscillator.py` & `mobspy-2.4.5/example_models/application_models/oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/positive_phage_feedback_loop.py` & `mobspy-2.4.5/example_models/application_models/positive_phage_feedback_loop.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/random_walk.py` & `mobspy-2.4.5/example_models/application_models/random_walk.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/simple_infection.py` & `mobspy-2.4.5/example_models/application_models/simple_infection.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/simple_repressor.py` & `mobspy-2.4.5/example_models/application_models/simple_repressor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/example_models/application_models/simple_rule_based_and_gate.py` & `mobspy-2.4.5/example_models/application_models/simple_rule_based_and_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/images/img.png` & `mobspy-2.4.5/images/img.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/data_handler/process_result_data.py` & `mobspy-2.4.5/mobspy/data_handler/process_result_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,22 +82,14 @@
     def multiply_data_by_factor(data, factor):
         for key in data:
             if key == 'Time':
                 continue
 
             converted_data[key] = [count * factor for count in data[key]]
 
-    # Old function - remove if not need in future. Removed because it is to slow to do this with pint
-    #def convert_data(data, from_unit, to_unit):
-    #    for key in data:
-    #        if key == 'Time':
-    #            continue
-
-    #        converted_data[key] = [(count * from_unit).to(to_unit).magnitude for count in data[key]]
-
     if output_concentration:
         converted_data = convert_to_concentration(data, converted_data, volume_list, time_list)
 
     # Fix here - forgot concentration conversion
     if unit_y is not None:
         if 'mol' in str(unit_y):
             multiply_data_by_factor(converted_data, N_A ** -1)
```

### Comparing `mobspy-2.4.4/mobspy/data_handler/time_series_object.py` & `mobspy-2.4.5/mobspy/data_handler/time_series_object.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/import_manager/lazy_import_class.py` & `mobspy-2.4.5/mobspy/import_manager/lazy_import_class.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/assignments_implementation.py` & `mobspy-2.4.5/mobspy/modules/assignments_implementation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from mobspy.modules.mobspy_expressions import MobsPyExpression as mbe_MobsPyExpression
 from mobspy.simulation_logging.log_scripts import error as simlog_error
 from mobspy.modules.species_string_generator import construct_all_combinations as ssg_construct_all_combinations, \
     construct_species_char_list as ssg_construct_species_char_list
+from re import compile as re_compile, escape as re_escape
 
 
 class Assignment_Operator:
     _asg_context = False
     regex_pattern = r'\(\$arg(?:\.[^\s().]+)?\)(?=[^\s()]|$)'
 
     @staticmethod
@@ -136,15 +137,15 @@
         for spe in spe_in_expression:
             replacement_dict[spe] = \
                 Assignment_Operator.generate_replacement_in_expression(spe, ortogonal_vector_structure,
                                                                        meta_species_in_model,
                                                                        for_error_tuple)
 
         for key, item in replacement_dict.items():
-            asg_expression = asg_expression.replace(key, item)
+            asg_expression = Assignment_Operator.replace_agn_expr(asg_expression, key, item)
 
         return asg_expression
 
     @staticmethod
     def compile_assignments_for_sbml(unprocessed_asgns, ortogonal_vector_structure, meta_species_in_model):
 
         assignments_for_sbml = {}
@@ -184,14 +185,19 @@
 
             assignments_for_sbml['assignment_' + str(assignment_counter)] = \
                 {'species': spe_to_asgn, 'expression': asgn_expression}
             assignment_counter += 1
 
         return assignments_for_sbml
 
+    @staticmethod
+    def replace_agn_expr(assignment_ex, to_replace, replacement):
+        pattern = re_compile(re_escape(to_replace) + r'(?![a-zA-Z0-9_])')
+        return pattern.sub(replacement, assignment_ex)
+
 
 Assign = Assignment_Operator()
 
 
 class Asg:
     assignments = {}
```

### Comparing `mobspy-2.4.4/mobspy/modules/class_of_meta_specie_named_any.py` & `mobspy-2.4.5/mobspy/modules/class_of_meta_specie_named_any.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/compiler.py` & `mobspy-2.4.5/mobspy/modules/compiler.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/context_related_scripts.py` & `mobspy-2.4.5/mobspy/modules/context_related_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/event_functions.py` & `mobspy-2.4.5/mobspy/modules/event_functions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/function_rate_code.py` & `mobspy-2.4.5/mobspy/modules/function_rate_code.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/logic_operator_objects.py` & `mobspy-2.4.5/mobspy/modules/logic_operator_objects.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/meta_class.py` & `mobspy-2.4.5/mobspy/modules/meta_class.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/meta_class_utils.py` & `mobspy-2.4.5/mobspy/modules/meta_class_utils.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/mobspy_expressions.py` & `mobspy-2.4.5/mobspy/modules/mobspy_expressions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/mobspy_parameters.py` & `mobspy-2.4.5/mobspy/modules/mobspy_parameters.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/order_operators.py` & `mobspy-2.4.5/mobspy/modules/order_operators.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/reaction_construction_nb.py` & `mobspy-2.4.5/mobspy/modules/reaction_construction_nb.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/set_counts_module.py` & `mobspy-2.4.5/mobspy/modules/set_counts_module.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/species_string_generator.py` & `mobspy-2.4.5/mobspy/modules/species_string_generator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/modules/unit_handler.py` & `mobspy-2.4.5/mobspy/modules/unit_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,20 @@
     """
     try:
         converted_quantity = deepcopy(quantity)
     except:
         converted_quantity = quantity
 
     if isinstance(quantity, Quantity):
-        if '[length]' not in str(quantity.dimensionality) and '[substance]' not in quantity.dimensionality:
+
+        if '[length]' not in str(quantity.dimensionality) and '[substance]' not in quantity.dimensionality\
+                and str(quantity.dimensionality) != "dimensionless":
             simlog.error(f'The assigned quantity {quantity} is neither a count or concentration')
+        elif str(quantity) == "dimensionless":
+            return quantity.magnitude
 
         try:
             if '[substance]' in quantity.dimensionality:
                 if '[length]' in str(quantity.dimensionality):
                     converted_quantity = converted_quantity.convert(f'moles/(decimeter ** {dimension})')
                     converted_quantity = converted_quantity * volume
```

### Comparing `mobspy-2.4.4/mobspy/parameter_estimation_data_loader/data_loader.py` & `mobspy-2.4.5/mobspy/parameter_estimation_data_loader/data_loader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py` & `mobspy-2.4.5/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/parameter_scripts/parameter_reader.py` & `mobspy-2.4.5/mobspy/parameter_scripts/parameter_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/parameter_scripts/parametric_sweeps.py` & `mobspy-2.4.5/mobspy/parameter_scripts/parametric_sweeps.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/parameters/README.md` & `mobspy-2.4.5/mobspy/parameters/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/parameters/default_reader.py` & `mobspy-2.4.5/mobspy/parameters/default_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/parameters/example_reader.py` & `mobspy-2.4.5/mobspy/parameters/example_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/patch_scripts/basico_task_parametrization.py` & `mobspy-2.4.5/mobspy/patch_scripts/basico_task_parametrization.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/plot_params/example_plot_reader.py` & `mobspy-2.4.5/mobspy/plot_params/example_plot_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/plot_scripts/default_plots.py` & `mobspy-2.4.5/mobspy/plot_scripts/default_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     """
     if 'xlabel' not in new_plot_params:
         new_plot_params['xlabel'] = 'Time'
 
         if new_plot_params['unit_x'] is not None and not ("ignore_unit_label_x" in new_plot_params and
                                                           new_plot_params["ignore_unit_label_x"]):
             if not isinstance(new_plot_params['unit_x'], Quantity):
-                new_plot_params['xlabel'] += f' ({new_plot_params["unit_x"]})'
+                new_plot_params['xlabel'] += f' ({new_plot_params["unit_x"]}s)'
             else:
-                new_plot_params['xlabel'] += f' ({new_plot_params["unit_x"].units})'
+                new_plot_params['xlabel'] += f' ({new_plot_params["unit_x"].units}s)'
 
     if 'ylabel' not in new_plot_params:
         if new_plot_params['output_concentration']:
             new_plot_params['ylabel'] = 'Conc.'
         else:
             new_plot_params['ylabel'] = 'Counts'
```

### Comparing `mobspy-2.4.4/mobspy/plot_scripts/hierarchical_plot.py` & `mobspy-2.4.5/mobspy/plot_scripts/hierarchical_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,14 @@
                 try:
                     return params[key]
                 except (KeyError, IndexError):
                     return None
 
 
 def annotation_handling(axs, figure_index, plot_index, plot_params):
-    print()
 
     if find_parameter(plot_params, key='annotations', index=(figure_index, plot_index)) is not None:
         annotations = find_parameter(plot_params, key='annotations', index=(figure_index, plot_index))
 
         if type(annotations) != list:
             simlog.warning("On plotting annotations: Annotations must a be list with dictionaries as elements")
             return 0
```

### Comparing `mobspy-2.4.4/mobspy/plot_scripts/process_plot_data.py` & `mobspy-2.4.5/mobspy/plot_scripts/process_plot_data.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/plot_scripts/statistics_calculations.py` & `mobspy-2.4.5/mobspy/plot_scripts/statistics_calculations.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/sbml_simulator/SBMLWriter.py` & `mobspy-2.4.5/mobspy/sbml_simulator/SBMLWriter.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc` & `mobspy-2.4.5/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc` & `mobspy-2.4.5/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc` & `mobspy-2.4.5/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/sbml_simulator/builder.py` & `mobspy-2.4.5/mobspy/sbml_simulator/builder.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/sbml_simulator/run.py` & `mobspy-2.4.5/mobspy/sbml_simulator/run.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/simulation.py` & `mobspy-2.4.5/mobspy/simulation.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy/simulation_logging/log_scripts.py` & `mobspy-2.4.5/mobspy/simulation_logging/log_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/mobspy.egg-info/PKG-INFO` & `mobspy-2.4.5/mobspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.4.4
+Version: 2.4.5
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
         
@@ -120,13 +120,15 @@
         
         Version 2.1 - Added model parameters. Now MySim.results returns a list of all resulting time series no matter the number of repetitions. However, now a MySim.fres attribute was released that returns only the first time series in each simulation (thus, it is equal to MySim results with only one repetition in the previous version).
         
         Version 2.2 - Added MobsPy expressions
         
         Version 2.3 - MobsPy standard output is now always concentration.
         
+        Version 2.4.4 - Assignments completely added (both notations)
+        
         
         
         
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `mobspy-2.4.4/mobspy.egg-info/SOURCES.txt` & `mobspy-2.4.5/mobspy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -240,20 +240,23 @@
 example_models/Tutorial Notebooks/01_Basic_Intro.ipynb
 example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb
 example_models/Tutorial Notebooks/03_Characteristics.ipynb
 example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb
 example_models/Tutorial Notebooks/05_For_Loops.ipynb
 example_models/Tutorial Notebooks/06_Order_Matters.ipynb
 example_models/Tutorial Notebooks/07_Initial_Condition.ipynb
+example_models/Tutorial Notebooks/08_Units_and_Output.ipynb
 example_models/Tutorial Notebooks/09_Result_Data.ipynb
 example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb
 example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb
 example_models/Tutorial Notebooks/12_Born_Species.ipynb
 example_models/Tutorial Notebooks/13_Events.ipynb
 example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb
+example_models/Tutorial Notebooks/15_Assignments.ipynb
+example_models/Tutorial Notebooks/16_Rev_All_Any.ipynb
 example_models/Tutorial Notebooks/images/Matching_Meta.png
 example_models/Tutorial Notebooks/images/vectorial_space.png
 example_models/application_models/AB_2CD.py
 example_models/application_models/AND_gate.py
 example_models/application_models/CRISPR_Oscillator.py
 example_models/application_models/For_The_Trees.py
 example_models/application_models/NOR_gate.py
@@ -376,11 +379,13 @@
 test_tools/model_48.txt
 test_tools/model_49.txt
 test_tools/model_5.txt
 test_tools/model_50.txt
 test_tools/model_51.txt
 test_tools/model_52.txt
 test_tools/model_53.txt
+test_tools/model_54.txt
+test_tools/model_55.txt
 test_tools/model_6.txt
 test_tools/model_7.txt
 test_tools/model_8.txt
 test_tools/model_9.txt
```

### Comparing `mobspy-2.4.4/setup.py` & `mobspy-2.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_plot_images/constant_tree.png` & `mobspy-2.4.5/test_plot_images/constant_tree.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_script.py` & `mobspy-2.4.5/test_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -1794,14 +1794,39 @@
     Rev[A + 4 * B >> C][lambda r1, r2: (100-r1)*(100-r2), lambda r: r**3]
 
     S = Simulation(A | B | C)
     S.level = -1
     assert compare_model(S.compile(), 'test_tools/model_53.txt')
 
 
+def test_dimensionless_count():
+    # model 54
+    a = 100*u.l/u.l
+    A = BaseSpecies()
+
+    A >> Zero [1]
+
+    A(a)
+    S = Simulation(A)
+    S.duration = 10
+    S.level = - 1
+    assert compare_model(S.compile(), 'test_tools/model_54.txt')
+
+
+def test_assignment_similar_species():
+    # model 55
+    A, R, Raa = BaseSpecies()
+
+    A.assign(R*Raa)
+
+    S = Simulation(A | R | Raa)
+    S.level = - 1
+    assert compare_model(S.compile(), 'test_tools/model_55.txt')
+
+
 # This is here because pytest is slow - but this script works fine with pytest. Just make sure that the
 # python version in terminal is above 3.10
 test_list = [test_model_1, test_model_2, test_model_3, test_model_4, test_model_5, test_model_6, test_model_7,
              test_orthogonal_spaces, test_average_value, test_hybrid_sim, test_concatenated_simulation,
              test_event_type, test_reacting_species_event, test_unit_event_test, test_reaction_deactivation,
              test_double_rate, test_single_rate, test_triple_rate, test_stochastic_event_duration,
              test_logic_operator_syntax, test_stack_position, test_empty_arguments,
@@ -1821,15 +1846,16 @@
              test_parameter_operation_in_rate, test_multi_parameter_with_expression, test_double_parameters_with_units,
              test_parameters_with_units, test_convert_back_parameter, test_parameter_fit_with_units,
              test_multiple_runs_fit, test_simple_fit, test_numpy_in_expression_function, test_numpy_in_rates,
              test_numpy_in_counts, test_numpy_in_set_counts, test_multi_methods_plot, test_unit_x_conversion,
              test_Silicon_valley, test_replacing_species_name_in_expression, test_basic_assignment,
              test_illegal_unit_op_in_assignment, test_all_asgn_ops, test_no_species_in_asg, text_complex_assignments,
              text_assign_context_exit, text_even_more_complex_assignments, test_assign_context_complex,
-             test_assign_context_constant, test_duration_with_run, test_rev]
+             test_assign_context_constant, test_duration_with_run, test_rev, test_dimensionless_count,
+             test_assignment_similar_species]
 
 sub_test = test_list
 
 
 def perform_tests():
     any_failed = False
     for test in sub_test:
```

### Comparing `mobspy-2.4.4/test_tools/model_15.txt` & `mobspy-2.4.5/test_tools/model_15.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_19.txt` & `mobspy-2.4.5/test_tools/model_19.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_21.txt` & `mobspy-2.4.5/test_tools/model_21.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_24.txt` & `mobspy-2.4.5/test_tools/model_24.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_26.txt` & `mobspy-2.4.5/test_tools/model_26.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_3.txt` & `mobspy-2.4.5/test_tools/model_3.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_31.txt` & `mobspy-2.4.5/test_tools/model_31.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_33.txt` & `mobspy-2.4.5/test_tools/model_33.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_38.txt` & `mobspy-2.4.5/test_tools/model_38.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_39.txt` & `mobspy-2.4.5/test_tools/model_39.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_4.txt` & `mobspy-2.4.5/test_tools/model_4.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_40.txt` & `mobspy-2.4.5/test_tools/model_40.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_41.txt` & `mobspy-2.4.5/test_tools/model_41.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_45.txt` & `mobspy-2.4.5/test_tools/model_45.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_5.txt` & `mobspy-2.4.5/test_tools/model_5.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_7.txt` & `mobspy-2.4.5/test_tools/model_7.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.4.4/test_tools/model_9.txt` & `mobspy-2.4.5/test_tools/model_9.txt`

 * *Files identical despite different names*

