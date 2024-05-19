# Comparing `tmp/mpl_ascii-0.6.1.tar.gz` & `tmp/mpl_ascii-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_ascii-0.6.1.tar", last modified: Sat May 11 09:39:42 2024, max compression
+gzip compressed data, was "mpl_ascii-0.6.2.tar", last modified: Sun May 19 13:36:22 2024, max compression
```

## Comparing `mpl_ascii-0.6.1.tar` & `mpl_ascii-0.6.2.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:39:42.330773 mpl_ascii-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:39:42.314773 mpl_ascii-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:39:42.314773 mpl_ascii-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-11 09:39:42.330773 mpl_ascii-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:39:42.326773 mpl_ascii-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_chart.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_label_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/bar_stacked.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/barh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/barh.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/box_plot_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/box_plot_basic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/categorical_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/categorical_variables.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/cohere.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/csd_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/csd_demo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/double_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/double_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/errorbars.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/errorbars.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/errorbars_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/errorbars_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/errorbars_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/errorbars_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/errorbars_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/errorbars_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/hist_best_fit_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/hist_best_fit_line.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/hist_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/hist_simple.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/hist_simple_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/hist_simple_colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/line_markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/line_markers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/lines_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/lines_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/scatter_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/scatter_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/simple_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/simple_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/violin_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/examples/violin_plot.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:39:42.326773 mpl_ascii-0.6.1/mpl_ascii/
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/mpl_ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/mpl_ascii/ascii_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/mpl_ascii/color_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    15664 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/mpl_ascii/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/mpl_ascii/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/mpl_ascii/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:39:42.330773 mpl_ascii-0.6.1/mpl_ascii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-11 09:39:42.000000 mpl_ascii-0.6.1/mpl_ascii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-11 09:39:42.000000 mpl_ascii-0.6.1/mpl_ascii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 09:39:42.000000 mpl_ascii-0.6.1/mpl_ascii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-11 09:39:42.000000 mpl_ascii-0.6.1/mpl_ascii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 09:39:42.000000 mpl_ascii-0.6.1/mpl_ascii.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 09:39:42.330773 mpl_ascii-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:39:42.330773 mpl_ascii-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-11 09:39:36.000000 mpl_ascii-0.6.1/tests/test_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.713123 mpl_ascii-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.697123 mpl_ascii-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.697123 mpl_ascii-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-19 13:36:22.713123 mpl_ascii-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.709123 mpl_ascii-0.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_chart.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_label_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/bar_stacked.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/barh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/barh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/box_plot_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/box_plot_basic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/categorical_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/categorical_variables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/cohere.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/color_bar_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/color_bar_scatter.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/csd_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/csd_demo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/double_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/double_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/errorbars_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_best_fit_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_best_fit_line.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_simple_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/hist_simple_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/line_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/line_markers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/lines_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/lines_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/scatter_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/scatter_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/simple_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/simple_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/violin_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/examples/violin_plot.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.709123 mpl_ascii-0.6.2/mpl_ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/ascii_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20303 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/mpl_ascii/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.709123 mpl_ascii-0.6.2/mpl_ascii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 13:36:22.000000 mpl_ascii-0.6.2/mpl_ascii.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:36:22.713123 mpl_ascii-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:22.709123 mpl_ascii-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-19 13:36:18.000000 mpl_ascii-0.6.2/tests/test_overlay.py
```

### Comparing `mpl_ascii-0.6.1/.github/workflows/python-package.yml` & `mpl_ascii-0.6.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/.gitignore` & `mpl_ascii-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/CHANGELOG.md` & `mpl_ascii-0.6.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,24 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
 ### Added
 
+- Add support for colour bars on scatter plots.
 - Add support for contour plots without colors.
 - Add support for text objects in plot.
 
+## [0.6.2] 2024-05-19
+
+## Fixed
+
+- `mpl_ascii` is now compatible with matplotlib 3.9.
+
 ## [0.6.1] 2024-05-11
 
 ### Fixed
 
 - Contour plots will return empty frame instead of raising an error.
 
 ## [0.6.0] 2024-05-10
```

### Comparing `mpl_ascii-0.6.1/LICENSE` & `mpl_ascii-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/Makefile` & `mpl_ascii-0.6.2/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 accept: $(addprefix $(ACCEPTANCE_DIR)/,$(ALL_PLOTS_TXT))
 	@true
 
 all.png: $(addprefix $(LOCATION)/,$(ALL_PLOTS_PNG))
 	@true
 
+clear:
+	-rm -rf $(DATA_DIR)
 
 %.txt: $(LOCATION)/%.txt
 	@true
 
 %.png: $(LOCATION)/%.png
 	@true
```

### Comparing `mpl_ascii-0.6.1/PKG-INFO` & `mpl_ascii-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.6.1
+Version: 0.6.2
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
```

### Comparing `mpl_ascii-0.6.1/README.md` & `mpl_ascii-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_chart.py` & `mpl_ascii-0.6.2/examples/bar_chart.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_chart.txt` & `mpl_ascii-0.6.2/examples/bar_chart.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_color.py` & `mpl_ascii-0.6.2/examples/bar_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_color.txt` & `mpl_ascii-0.6.2/examples/bar_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_1.py` & `mpl_ascii-0.6.2/examples/bar_label_1.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_1.txt` & `mpl_ascii-0.6.2/examples/bar_label_1.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_2.py` & `mpl_ascii-0.6.2/examples/bar_label_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_2.txt` & `mpl_ascii-0.6.2/examples/bar_label_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_3.py` & `mpl_ascii-0.6.2/examples/bar_label_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_3.txt` & `mpl_ascii-0.6.2/examples/bar_label_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_4.py` & `mpl_ascii-0.6.2/examples/bar_label_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_4.txt` & `mpl_ascii-0.6.2/examples/bar_label_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_5.py` & `mpl_ascii-0.6.2/examples/bar_label_5.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_label_5.txt` & `mpl_ascii-0.6.2/examples/bar_label_5.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_stacked.py` & `mpl_ascii-0.6.2/examples/bar_stacked.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/bar_stacked.txt` & `mpl_ascii-0.6.2/examples/bar_stacked.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/barh.py` & `mpl_ascii-0.6.2/examples/barh.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/barh.txt` & `mpl_ascii-0.6.2/examples/barh.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/box_plot_basic.py` & `mpl_ascii-0.6.2/examples/box_plot_basic.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/box_plot_basic.txt` & `mpl_ascii-0.6.2/examples/box_plot_basic.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/categorical_variables.py` & `mpl_ascii-0.6.2/examples/categorical_variables.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/categorical_variables.txt` & `mpl_ascii-0.6.2/examples/categorical_variables.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/cohere.py` & `mpl_ascii-0.6.2/examples/cohere.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/cohere.txt` & `mpl_ascii-0.6.2/examples/cohere.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/csd_demo.py` & `mpl_ascii-0.6.2/examples/csd_demo.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/csd_demo.txt` & `mpl_ascii-0.6.2/examples/csd_demo.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/double_plot.py` & `mpl_ascii-0.6.2/examples/double_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/double_plot.txt` & `mpl_ascii-0.6.2/examples/double_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/errorbars.txt` & `mpl_ascii-0.6.2/examples/errorbars.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/errorbars_2.py` & `mpl_ascii-0.6.2/examples/errorbars_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/errorbars_2.txt` & `mpl_ascii-0.6.2/examples/errorbars_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/errorbars_3.py` & `mpl_ascii-0.6.2/examples/errorbars_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/errorbars_3.txt` & `mpl_ascii-0.6.2/examples/errorbars_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/errorbars_4.py` & `mpl_ascii-0.6.2/examples/errorbars_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/errorbars_4.txt` & `mpl_ascii-0.6.2/examples/errorbars_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/hist_best_fit_line.py` & `mpl_ascii-0.6.2/examples/hist_best_fit_line.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/hist_best_fit_line.txt` & `mpl_ascii-0.6.2/examples/hist_best_fit_line.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/hist_simple.py` & `mpl_ascii-0.6.2/examples/hist_simple.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/hist_simple.txt` & `mpl_ascii-0.6.2/examples/hist_simple.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/hist_simple_colors.py` & `mpl_ascii-0.6.2/examples/hist_simple_colors.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/hist_simple_colors.txt` & `mpl_ascii-0.6.2/examples/hist_simple_colors.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/line_markers.py` & `mpl_ascii-0.6.2/examples/line_markers.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/line_markers.txt` & `mpl_ascii-0.6.2/examples/line_markers.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/lines_multi_color.py` & `mpl_ascii-0.6.2/examples/lines_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/lines_multi_color.txt` & `mpl_ascii-0.6.2/examples/lines_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/scatter_multi_color.py` & `mpl_ascii-0.6.2/examples/scatter_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/scatter_multi_color.txt` & `mpl_ascii-0.6.2/examples/scatter_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/simple_plot.py` & `mpl_ascii-0.6.2/examples/simple_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/simple_plot.txt` & `mpl_ascii-0.6.2/examples/simple_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/violin_plot.py` & `mpl_ascii-0.6.2/examples/violin_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/examples/violin_plot.txt` & `mpl_ascii-0.6.2/examples/violin_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/mpl_ascii/ascii_canvas.py` & `mpl_ascii-0.6.2/mpl_ascii/ascii_canvas.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/mpl_ascii/draw.py` & `mpl_ascii-0.6.2/mpl_ascii/draw.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,303 +1,119 @@
-from matplotlib.collections import LineCollection, PathCollection, PolyCollection
+from itertools import zip_longest
+import matplotlib
+from matplotlib.axes import Axes
+from matplotlib.collections import LineCollection, PathCollection, PolyCollection, QuadMesh
+from matplotlib.colors import Colormap, ListedColormap, Normalize
 from matplotlib.container import BarContainer, ErrorbarContainer
 from matplotlib.contour import QuadContourSet
 from matplotlib.lines import Line2D
 from matplotlib.patches import Rectangle
 from matplotlib.text import Annotation, Text
 import numpy as np
 
 from mpl_ascii.ascii_canvas import AsciiCanvas
-from mpl_ascii.color_map import Char, ax_color_map, std_color
+from mpl_ascii.color_map import Char, std_color
 from mpl_ascii.tools import linear_transform, scale_factor
 
+from mpl_ascii import color_map
+
 import mpl_ascii
 
-def draw_ax(ax, axes_height, axes_width):
+mpl_version = matplotlib.__version__
+mpl_version = tuple(map(int, mpl_version.split(".")))
+
+
+def draw_ax(ax: Axes, axes_height, axes_width, color_to_ascii):
     frame_buffer_left = 1
     frame_buffer_right = 1
     frame_buffer_top = 1
     frame_buffer_bottom = 1
 
 
     frame_width = axes_width + frame_buffer_left + frame_buffer_right
     frame_height = axes_height + frame_buffer_top + frame_buffer_bottom
 
-    color_to_ascii = ax_color_map(ax)
-
     x_range = ax.get_xlim()
     if x_range[1] < x_range[0]:
         x_range = x_range[1], x_range[0]
 
     y_range = ax.get_ylim()
     if y_range[1] < y_range[0]:
         y_range = y_range[1], y_range[0]
 
-    x_min, x_max = x_range
-    y_min, y_max = y_range
-
     canvas = AsciiCanvas(np.full((axes_height, axes_width), fill_value=" "))
 
-    errorbar_caplines = []
-    error_barlinescols = []
-    for container in ax.containers:
-        if not isinstance(container, ErrorbarContainer):
-            continue
-        _, caplines, barlinescols = tuple(container)
-        errorbar_caplines += [*caplines]
-        error_barlinescols += [*barlinescols]
-
-
-    for container in ax.containers:
-        # Draw Bar chart
-        if not isinstance(container, BarContainer):
-            continue
-        for bar in container.patches:
-            if not isinstance(bar, Rectangle):
-                continue
-
-            char = color_to_ascii[std_color(bar.get_facecolor())]
-
-            canvas_bar = AsciiCanvas(
-                    draw_bar(
-                    bar.get_height(),
-                    bar.get_width(),
-                    axes_height,
-                    axes_width,
-                    x_range,
-                    y_range,
-                    char
-                )
-            )
-            ascii_x_bar = round(linear_transform(bar.xy[0], x_min, x_max, 0, axes_width-1))
-            ascii_y_bar = round(linear_transform(bar.xy[1], y_min, y_max, 1, axes_height))
-
-            canvas = canvas.update(canvas_bar, (axes_height - ascii_y_bar - canvas_bar.shape[0]+1, ascii_x_bar))
-
+    errorbar_caplines, error_barlinescols = get_errorbars(ax.containers)
 
+    canvas = add_bar_chart(canvas, ax.containers, axes_height, axes_width, x_range, y_range, color_to_ascii)
 
-    lines_with_markers = []
-    # Draw lines
-    for line in ax.get_lines():
-        if line in errorbar_caplines:
-            continue
-        if line.get_marker() != "None" and line.get_marker() != "":
-            lines_with_markers.append(line)
-
-        char = color_to_ascii[std_color(line.get_color())]
-        xy_data = line.get_xydata()
-        x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
-        line = AsciiCanvas(
-                draw_line(
-                width=axes_width,
-                height=axes_height,
-                x_data=x_data,
-                y_data=y_data,
-                x_range=x_range,
-                y_range=y_range,
-                char = char,
-                linestyle=line.get_linestyle()
-            )
-        )
-
-        canvas = canvas.update(line, (0,0))
+    if mpl_ascii.UNRELEASED:
 
-    for container in ax.containers:
-        # Add errorbars
-        if isinstance(container, ErrorbarContainer):
-            _, _, barlinescols = tuple(container)
-
-            for collection in barlinescols:
-                for xy in collection.get_segments():
-                    x_data = [p[0] for p in xy]
-                    y_data = [p[1] for p in xy]
-                    char = Char("-", "white")
-
-                    if len(set(x_data)) == 1:
-                        char = Char("|", "white")
-
-                    errorbar = AsciiCanvas(draw_line(
-                        width=axes_width,
-                        height=axes_height,
-                        x_data=x_data,
-                        y_data=y_data,
-                        x_range=x_range,
-                        y_range=y_range,
-                        char = char
+        for container in ax.collections:
+            if isinstance(container, QuadMesh):
+                color_bar_width = 10
+                axes_width = color_bar_width
+                frame_width = axes_width + frame_buffer_left + frame_buffer_right
+
+
+                bar_chars = color_map.bar_chars
+                tick_data = [tick.get_loc() for tick in ax.yaxis.get_major_ticks()]
+                for char, i in zip(bar_chars, range(1, len(tick_data))):
+                    top_value = tick_data[i]
+                    bottom_value = tick_data[i-1]
+                    if tick_data[i] > y_range[1]:
+                        top_value = y_range[1]
+                    top = round(linear_transform(top_value, y_range[0], y_range[1], 1, axes_height))
+                    bottom = round(linear_transform(bottom_value, y_range[0], y_range[1], 1, axes_height))
+                    cmap, norm = container.cmap, container.norm
+                    char = color_to_ascii[std_color(cmap(norm(top_value)))]
+                    bar_height = top - bottom
+                    if i == 1:
+                        bar_height = top
+
+                    c = AsciiCanvas(draw_bar(
+                        bar_height,
+                        10,
+                        axes_height,
+                        10,
+                        (0,9),
+                        (1,axes_height),
+                        char
                     ))
-                    canvas = canvas.update(errorbar, (0,0))
 
-    # Add lines with markers
-    for line in lines_with_markers:
-        marker = get_ascii_marker(line.get_marker())
+                    canvas = canvas.update(c, (axes_height - top, 0))
 
-        color = color_to_ascii[std_color(line.get_color())].color
-        char = Char(marker.upper(), color)
-        xy_data = line.get_xydata()
-        x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
-        line = AsciiCanvas(
-                draw_line(
-                width=axes_width,
-                height=axes_height,
-                x_data=x_data,
-                y_data=y_data,
-                x_range=x_range,
-                y_range=y_range,
-                char = char,
-                linestyle="None"
-            )
-        )
-        canvas = canvas.update(line, (0,0))
+    canvas = add_line_plots(canvas, ax.get_lines(), axes_height, axes_width, x_range, y_range, color_to_ascii, errorbar_caplines)
 
-    for collection in ax.collections:
-        # Contour plot
-        if mpl_ascii.UNRELEASED:
-            if isinstance(collection, QuadContourSet):
-                for seg in collection.allsegs:
-                    for xy_data in seg:
-
-                        x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
-                        line = AsciiCanvas(
-                                draw_line(
-                                width=axes_width,
-                                height=axes_height,
-                                x_data=x_data,
-                                y_data=y_data,
-                                x_range=x_range,
-                                y_range=y_range,
-                                char = "-",
-                            )
-                        )
-                        canvas = canvas.update(line, (0,0))
+    canvas = add_errorbars(canvas, axes_height, axes_width, error_barlinescols, x_range, y_range)
 
-        # Violin Plots
-        if isinstance(collection, PolyCollection):
-            char = color_to_ascii[std_color(collection.get_facecolor())]
-            for path in collection.get_paths():
-                xy_data = path.vertices
-                x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
-                line = AsciiCanvas(
-                    draw_line(
-                    width=axes_width,
-                    height=axes_height,
-                    x_data=x_data,
-                    y_data=y_data,
-                    x_range=x_range,
-                    y_range=y_range,
-                    char = char,
-                    )
-                )
-                canvas = canvas.update(line, (0,0))
-
-        # Violin Plots
-        if isinstance(collection, LineCollection):
-            if collection in error_barlinescols:
-                continue
-
-            for xy in collection.get_segments():
-                x_data = [p[0] for p in xy]
-                y_data = [p[1] for p in xy]
-                char = color_to_ascii[std_color(collection.get_color())]
-                line = AsciiCanvas(
-                    draw_line(
-                    width=axes_width,
-                    height=axes_height,
-                    x_data=x_data,
-                    y_data=y_data,
-                    x_range=x_range,
-                    y_range=y_range,
-                    char = char,
-                    )
-                )
-                canvas = canvas.update(line, (0,0))
+    lines_with_markers = get_lines_with_markers(ax.get_lines(), errorbar_caplines)
 
-        # Add scatter plot
-        if isinstance(collection, PathCollection):
-            offsets = collection.get_offsets()
-
-            if len(collection.get_facecolor()) > 0:
-                color = collection.get_facecolor()[0]
-
-            if len(collection.get_edgecolor()) > 0:
-                color = collection.get_edgecolor()[0]
-
-            for point in offsets:
-                color = tuple(color)
-
-                x_new = round(linear_transform(point[0], x_min, x_max, 0, axes_width-1))
-                y_new = round(linear_transform(point[1], y_min, y_max, 1, axes_height))
-
-                char = color_to_ascii.get(std_color(color), Char("+", "white"))
-                canvas = canvas.update(AsciiCanvas(np.array([[char]])), (axes_height-y_new, x_new))
+    canvas = add_line_markers(canvas, axes_height, axes_width, x_range, y_range, color_to_ascii, lines_with_markers)
 
     if mpl_ascii.UNRELEASED:
-        for text in ax.texts:
-            if isinstance(text, Annotation):
-                continue
-            if isinstance(text, Text):
-                text_xy = text.get_position()
-                text_canvas = AsciiCanvas(np.array([list(text.get_text())]))
-                ascii_x = round(linear_transform(text_xy[0], x_min, x_max, 0, axes_width-1))
-                ascii_y = round(linear_transform(text_xy[1], y_min, y_max, 1, axes_height))
-                canvas = canvas.update(text_canvas, (axes_height - ascii_y, ascii_x))
+        canvas = add_contours(canvas, ax.collections, axes_height, axes_width, x_range, y_range, color_to_ascii)
 
-    # Add frame
-    canvas = canvas.update(AsciiCanvas(draw_frame(frame_height, frame_width)), (-frame_buffer_left,-frame_buffer_top))
-
-    # Add xticks and labels
-    tick_data = [tick.get_position()[0] for tick in ax.xaxis.get_ticklabels()]
-    label_data = [tick.get_text().replace("\n", "") for tick in ax.xaxis.get_ticklabels()]
-    xticks = AsciiCanvas(draw_x_ticks(axes_width, tick_data, label_data, x_range))
-
-    xlabel = AsciiCanvas(np.array([list(ax.get_xlabel())]))
-
-    xticks_and_label = xticks.update(xlabel, location=(xticks.shape[0],int(xticks.shape[1] / 2)))
-
-    canvas = canvas.update(xticks_and_label, location=(canvas.shape[0]-1, 1))
-
-    # Add yticks and labels
-    tick_data = [tick.get_loc() for tick in ax.yaxis.get_major_ticks()]
-    label_data = [tick.label1.get_text().replace("\n", "") for tick in ax.yaxis.get_major_ticks()]
-    yticks = AsciiCanvas(draw_y_ticks(axes_height, tick_data, label_data, y_range))
+    canvas = add_violin_plots(canvas, ax.collections, axes_height, axes_width, x_range, y_range, color_to_ascii, error_barlinescols)
 
-    ylabel = AsciiCanvas(np.array([list(ax.get_ylabel())]).T)
-    yticks_and_label = yticks.update(ylabel, location=(int(yticks.shape[0] / 2), -(ylabel.shape[1] + 1)))
+    canvas = add_scatter_plots(canvas, ax.collections, axes_height, axes_width, x_range, y_range, color_to_ascii)
 
-    canvas = canvas.update(yticks_and_label, location=(1, -yticks_and_label.shape[1]+1))
 
-    # Add ax title
-    ax_title = AsciiCanvas(np.array([list(ax.get_title())]))
-    canvas = canvas.update(ax_title, location=(-(ax_title.shape[0] + 1), int(canvas.shape[1] / 2)))
+    if mpl_ascii.UNRELEASED:
+        canvas = add_text(canvas, ax.texts, axes_height, axes_width, x_range, y_range)
 
-    # Add legend
-    legend = ax.get_legend()
-    if legend:
-        handles, text = legend.legendHandles, legend.texts
+    canvas = add_frame(canvas, frame_height, frame_width, frame_buffer_left, frame_buffer_top)
 
-        canvas_legend = AsciiCanvas()
-        for handle, text in zip(handles, text):
-            char = " "
-            if isinstance(handle, Rectangle):
-                char = color_to_ascii[std_color(handle.get_facecolor())]
-            if isinstance(handle, Line2D):
-                char = color_to_ascii[std_color(handle.get_color())]
-            if isinstance(handle, PathCollection):
-                color = tuple(handle.get_facecolor()[0])
-                char = color_to_ascii[std_color(color)]
+    canvas = add_xticks_and_labels(canvas, ax, axes_width, x_range)
 
-            arr = np.array([[char] * 3 + [" "] + list(text.get_text())])
-            canvas_legend = canvas_legend.update(AsciiCanvas(arr), (canvas_legend.shape[0], 0))
+    canvas = add_yticks_and_labels(canvas, ax, axes_height, y_range)
 
-        title = legend.get_title().get_text() or "Legend"
-        title = AsciiCanvas(np.array([list(title)]))
-        canvas_legend = canvas_legend.update(title, (-2,0))
-        legend_frame = AsciiCanvas(draw_frame(canvas_legend.shape[0]+2, canvas_legend.shape[1]+4))
-        canvas_legend = legend_frame.update(canvas_legend, (1,2))
+    canvas = add_ax_title(canvas, ax.get_title())
 
-        canvas = canvas.update(canvas_legend, (canvas.shape[0] + 1, round(canvas.shape[1] / 2) ))
+    canvas = add_legend(canvas, ax.get_legend(), color_to_ascii)
 
     return canvas
 
 
 def draw_frame(height, width):
     frame = np.full((height, width), fill_value=" ")
     frame[0,:] = "-"
@@ -453,9 +269,309 @@
     if marker == "<" or marker == "3":
         marker = chr(9664)
     if marker == ">" or marker == "4":
         marker = chr(9654)
 
     return marker
 
+def get_errorbars(containers):
+    errorbar_caplines = []
+    error_barlinescols = []
+    for container in containers:
+        if not isinstance(container, ErrorbarContainer):
+            continue
+        _, caplines, barlinescols = tuple(container)
+        errorbar_caplines += [*caplines]
+        error_barlinescols += [*barlinescols]
+
+    return errorbar_caplines, error_barlinescols
+
+def add_bar_chart(canvas, containers, axes_height, axes_width, x_range, y_range, color_to_ascii):
+    x_min, x_max = x_range
+    y_min, y_max = y_range
+
+    for container in containers:
+        # Draw Bar chart
+        if not isinstance(container, BarContainer):
+            continue
+        for bar in container.patches:
+            if not isinstance(bar, Rectangle):
+                continue
+
+            char = color_to_ascii[std_color(bar.get_facecolor())]
+
+            canvas_bar = AsciiCanvas(
+                    draw_bar(
+                    bar.get_height(),
+                    bar.get_width(),
+                    axes_height,
+                    axes_width,
+                    x_range,
+                    y_range,
+                    char
+                )
+            )
+            ascii_x_bar = round(linear_transform(bar.xy[0], x_min, x_max, 0, axes_width-1))
+            ascii_y_bar = round(linear_transform(bar.xy[1], y_min, y_max, 1, axes_height))
+
+            canvas = canvas.update(canvas_bar, (axes_height - ascii_y_bar - canvas_bar.shape[0]+1, ascii_x_bar))
+
+    return canvas
+
+def add_line_plots(canvas, lines, axes_height, axes_width, x_range, y_range, color_to_ascii, errorbar_caplines):
+    for line in lines:
+        if line in errorbar_caplines:
+            continue
+
+        char = color_to_ascii[std_color(line.get_color())]
+        xy_data = line.get_xydata()
+        x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
+        line = AsciiCanvas(
+                draw_line(
+                width=axes_width,
+                height=axes_height,
+                x_data=x_data,
+                y_data=y_data,
+                x_range=x_range,
+                y_range=y_range,
+                char = char,
+                linestyle=line.get_linestyle()
+            )
+        )
+
+        canvas = canvas.update(line, (0,0))
+    return canvas
+
+def get_lines_with_markers(lines, errorbar_caplines):
+    lines_with_markers = []
+    # Draw lines
+    for line in lines:
+        if line in errorbar_caplines:
+            continue
+        if line.get_marker() != "None" and line.get_marker() != "":
+            lines_with_markers.append(line)
+
+    return lines_with_markers
+
+def add_errorbars(canvas, axes_height, axes_width, error_barlinescols, x_range, y_range):
+    for collection in error_barlinescols:
+        for xy in collection.get_segments():
+            x_data = [p[0] for p in xy]
+            y_data = [p[1] for p in xy]
+            char = Char("-", "white")
+
+            if len(set(x_data)) == 1:
+                char = Char("|", "white")
 
+            errorbar = AsciiCanvas(draw_line(
+                width=axes_width,
+                height=axes_height,
+                x_data=x_data,
+                y_data=y_data,
+                x_range=x_range,
+                y_range=y_range,
+                char = char
+            ))
+
+            canvas = canvas.update(errorbar, (0,0))
+    return canvas
+
+def add_line_markers(canvas, axes_height, axes_width, x_range, y_range, color_to_ascii, lines_with_markers):
+    for line in lines_with_markers:
+        marker = get_ascii_marker(line.get_marker())
+
+        color = color_to_ascii[std_color(line.get_color())].color
+        char = Char(marker.upper(), color)
+        xy_data = line.get_xydata()
+        x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
+        line = AsciiCanvas(
+                draw_line(
+                width=axes_width,
+                height=axes_height,
+                x_data=x_data,
+                y_data=y_data,
+                x_range=x_range,
+                y_range=y_range,
+                char = char,
+                linestyle="None"
+            )
+        )
+        canvas = canvas.update(line, (0,0))
+    return canvas
+
+def add_contours(canvas, collections, axes_height, axes_width, x_range, y_range, color_to_ascii):
+    for collection in collections:
+        if isinstance(collection, QuadContourSet):
+            for seg in collection.allsegs:
+                for xy_data in seg:
+
+                    x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
+                    line = AsciiCanvas(
+                            draw_line(
+                            width=axes_width,
+                            height=axes_height,
+                            x_data=x_data,
+                            y_data=y_data,
+                            x_range=x_range,
+                            y_range=y_range,
+                            char = "-",
+                        )
+                    )
+                    canvas = canvas.update(line, (0,0))
+
+    return canvas
+
+def add_violin_plots(canvas, collections, axes_height, axes_width, x_range, y_range, color_to_ascii, error_barlinescols):
+    for collection in collections:
+        # Contour plot
+        if isinstance(collection, PolyCollection):
+            char = color_to_ascii[std_color(collection.get_facecolor())]
+            for path in collection.get_paths():
+                xy_data = path.vertices
+                x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
+                line = AsciiCanvas(
+                    draw_line(
+                    width=axes_width,
+                    height=axes_height,
+                    x_data=x_data,
+                    y_data=y_data,
+                    x_range=x_range,
+                    y_range=y_range,
+                    char = char,
+                    )
+                )
+                canvas = canvas.update(line, (0,0))
+
+        if isinstance(collection, LineCollection):
+            if collection in error_barlinescols:
+                continue
+
+            for xy in collection.get_segments():
+                x_data = [p[0] for p in xy]
+                y_data = [p[1] for p in xy]
+                char = color_to_ascii[std_color(collection.get_color())]
+                line = AsciiCanvas(
+                    draw_line(
+                    width=axes_width,
+                    height=axes_height,
+                    x_data=x_data,
+                    y_data=y_data,
+                    x_range=x_range,
+                    y_range=y_range,
+                    char = char,
+                    )
+                )
+                canvas = canvas.update(line, (0,0))
+    return canvas
+
+def add_scatter_plots(canvas, collections, axes_height, axes_width, x_range, y_range, color_to_ascii):
+    x_min, x_max = x_range
+    y_min, y_max = y_range
+
+    for collection in collections:
+        # Add scatter plot
+        if isinstance(collection, PathCollection):
+            offsets = collection.get_offsets()
+            if len(collection.get_facecolor()) > 0:
+                default_color = collection.get_facecolor()[0]
+                colors = collection.get_facecolor()
+
+            if len(collection.get_edgecolor()) > 0:
+                default_color = collection.get_edgecolor()[0]
+                colors = collection.get_edgecolor()
+
+
+            for point,color in zip_longest(offsets, colors, fillvalue=default_color):
+                color = tuple(color)
+
+                x_new = round(linear_transform(point[0], x_min, x_max, 0, axes_width-1))
+                y_new = round(linear_transform(point[1], y_min, y_max, 1, axes_height))
+
+                char = color_to_ascii.get(std_color(color), Char("+", "white"))
+                canvas = canvas.update(AsciiCanvas(np.array([[char]])), (axes_height-y_new, x_new))
+
+    return canvas
+
+def add_text(canvas, texts, axes_height, axes_width, x_range, y_range):
+    x_min, x_max = x_range
+    y_min, y_max = y_range
+
+    for text in texts:
+        if isinstance(text, Annotation):
+            continue
+        if isinstance(text, Text):
+            text_xy = text.get_position()
+            text_canvas = AsciiCanvas(np.array([list(text.get_text())]))
+            ascii_x = round(linear_transform(text_xy[0], x_min, x_max, 0, axes_width-1))
+            ascii_y = round(linear_transform(text_xy[1], y_min, y_max, 1, axes_height))
+            canvas = canvas.update(text_canvas, (axes_height - ascii_y, ascii_x))
+
+    return canvas
+
+def add_frame(canvas, frame_height, frame_width, frame_buffer_left, frame_buffer_top):
+    canvas = canvas.update(AsciiCanvas(draw_frame(frame_height, frame_width)), (-frame_buffer_left,-frame_buffer_top))
+    return canvas
+
+def add_xticks_and_labels(canvas, ax, axes_width, x_range):
+    tick_data = [tick.get_position()[0] for tick in ax.xaxis.get_ticklabels()]
+    label_data = [tick.get_text().replace("\n", "") for tick in ax.xaxis.get_ticklabels()]
+    xticks = AsciiCanvas(draw_x_ticks(axes_width, tick_data, label_data, x_range))
+
+    xlabel = AsciiCanvas(np.array([list(ax.get_xlabel())]))
+
+    xticks_and_label = xticks.update(xlabel, location=(xticks.shape[0],int(xticks.shape[1] / 2)))
+
+    canvas = canvas.update(xticks_and_label, location=(canvas.shape[0]-1, 1))
+    return canvas
+
+def add_yticks_and_labels(canvas, ax, axes_height, y_range):
+
+    # Add yticks and labels
+    tick_data = [tick.get_loc() for tick in ax.yaxis.get_major_ticks()]
+    label_data = [tick.label1.get_text().replace("\n", "") for tick in ax.yaxis.get_major_ticks()]
+    yticks = AsciiCanvas(draw_y_ticks(axes_height, tick_data, label_data, y_range))
+
+    ylabel = AsciiCanvas(np.array([list(ax.get_ylabel())]).T)
+    yticks_and_label = yticks.update(ylabel, location=(int(yticks.shape[0] / 2), -(ylabel.shape[1] + 1)))
+
+    canvas = canvas.update(yticks_and_label, location=(1, -yticks_and_label.shape[1]+1))
+    return canvas
+
+def add_ax_title(canvas, title):
+    ax_title = AsciiCanvas(np.array([list(title)]))
+    canvas = canvas.update(ax_title, location=(-(ax_title.shape[0] + 1), int(canvas.shape[1] / 2)))
+
+    return canvas
+
+def add_legend(canvas, legend, color_to_ascii):
+
+    # Add legend
+    if legend:
+        texts = legend.texts
+        if mpl_version >= (3,7,0):
+            handles = legend.legend_handles
+        else:
+            handles = legend.legendHandles
+
+        canvas_legend = AsciiCanvas()
+        for handle, text in zip(handles, texts):
+            char = " "
+            if isinstance(handle, Rectangle):
+                char = color_to_ascii[std_color(handle.get_facecolor())]
+            if isinstance(handle, Line2D):
+                char = color_to_ascii[std_color(handle.get_color())]
+            if isinstance(handle, PathCollection):
+                color = tuple(handle.get_facecolor()[0])
+                char = color_to_ascii[std_color(color)]
+
+            arr = np.array([[char] * 3 + [" "] + list(text.get_text())])
+            canvas_legend = canvas_legend.update(AsciiCanvas(arr), (canvas_legend.shape[0], 0))
+
+        title = legend.get_title().get_text() or "Legend"
+        title = AsciiCanvas(np.array([list(title)]))
+        canvas_legend = canvas_legend.update(title, (-2,0))
+        legend_frame = AsciiCanvas(draw_frame(canvas_legend.shape[0]+2, canvas_legend.shape[1]+4))
+        canvas_legend = legend_frame.update(canvas_legend, (1,2))
+
+        canvas = canvas.update(canvas_legend, (canvas.shape[0] + 1, round(canvas.shape[1] / 2) ))
 
+    return canvas
```

### Comparing `mpl_ascii-0.6.1/mpl_ascii/overlay.py` & `mpl_ascii-0.6.2/mpl_ascii/overlay.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/mpl_ascii.egg-info/PKG-INFO` & `mpl_ascii-0.6.2/mpl_ascii.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.6.1
+Version: 0.6.2
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
```

### Comparing `mpl_ascii-0.6.1/mpl_ascii.egg-info/SOURCES.txt` & `mpl_ascii-0.6.2/mpl_ascii.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 examples/barh.txt
 examples/box_plot_basic.py
 examples/box_plot_basic.txt
 examples/categorical_variables.py
 examples/categorical_variables.txt
 examples/cohere.py
 examples/cohere.txt
+examples/color_bar_scatter.py
+examples/color_bar_scatter.txt
 examples/csd_demo.py
 examples/csd_demo.txt
 examples/double_plot.py
 examples/double_plot.txt
 examples/errorbars.py
 examples/errorbars.txt
 examples/errorbars_2.py
```

### Comparing `mpl_ascii-0.6.1/pyproject.toml` & `mpl_ascii-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.1/tests/test_overlay.py` & `mpl_ascii-0.6.2/tests/test_overlay.py`

 * *Files identical despite different names*

