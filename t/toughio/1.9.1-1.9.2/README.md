# Comparing `tmp/toughio-1.9.1.tar.gz` & `tmp/toughio-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toughio-1.9.1.tar", last modified: Mon May  2 18:53:59 2022, max compression
+gzip compressed data, was "toughio-1.9.2.tar", last modified: Fri May  6 18:46:22 2022, max compression
```

## Comparing `toughio-1.9.1.tar` & `toughio-1.9.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.436082 toughio-1.9.1/
--rw-rw-rw-   0        0        0     2460 2021-12-06 20:12:26.000000 toughio-1.9.1/LICENSE
--rw-rw-rw-   0        0        0    11097 2022-05-02 18:53:59.435082 toughio-1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0    10034 2022-04-27 15:33:43.000000 toughio-1.9.1/README.rst
--rw-rw-rw-   0        0        0       42 2022-05-02 18:53:59.436082 toughio-1.9.1/setup.cfg
--rw-rw-rw-   0        0        0     2981 2022-04-27 15:26:33.000000 toughio-1.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.290392 toughio-1.9.1/test/
--rw-rw-rw-   0        0        0     1301 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_capillarity.py
--rw-rw-rw-   0        0        0     8951 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_cli.py
--rw-rw-rw-   0        0        0    30342 2022-05-02 18:39:26.000000 toughio-1.9.1/test/test_input.py
--rw-rw-rw-   0        0        0     8668 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_mesh_methods.py
--rw-rw-rw-   0        0        0      967 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_mesh_properties.py
--rw-rw-rw-   0        0        0     1473 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_meshio.py
--rw-rw-rw-   0        0        0     4479 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_meshmaker.py
--rw-rw-rw-   0        0        0     5109 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_output.py
--rw-rw-rw-   0        0        0     1282 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_relative_permeability.py
--rw-rw-rw-   0        0        0     1567 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_time_series.py
--rw-rw-rw-   0        0        0     5661 2022-04-27 15:26:33.000000 toughio-1.9.1/test/test_tough.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.299085 toughio-1.9.1/toughio/
--rw-rw-rw-   0        0        0      185 2022-05-02 18:51:57.000000 toughio-1.9.1/toughio/__about__.py
--rw-rw-rw-   0        0        0     1231 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.335084 toughio-1.9.1/toughio/_cli/
--rw-rw-rw-   0        0        0      250 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_cli/__init__.py
--rw-rw-rw-   0        0        0      920 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_cli/_co2tab.py
--rw-rw-rw-   0        0        0     9805 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_cli/_export.py
--rw-rw-rw-   0        0        0     4393 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_cli/_extract.py
--rw-rw-rw-   0        0        0     2465 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_cli/_merge.py
--rw-rw-rw-   0        0        0     1541 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_cli/_save2incon.py
--rw-rw-rw-   0        0        0     5512 2022-04-27 15:33:43.000000 toughio-1.9.1/toughio/_common.py
--rw-rw-rw-   0        0        0       39 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_exceptions.py
--rw-rw-rw-   0        0        0     1735 2022-04-27 15:33:43.000000 toughio-1.9.1/toughio/_helpers.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.336085 toughio-1.9.1/toughio/_io/
--rw-rw-rw-   0        0        0      503 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_io/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.339086 toughio-1.9.1/toughio/_io/input/
--rw-rw-rw-   0        0        0      134 2022-04-27 15:33:43.000000 toughio-1.9.1/toughio/_io/input/__init__.py
--rw-rw-rw-   0        0        0     3544 2022-04-27 15:33:43.000000 toughio-1.9.1/toughio/_io/input/_helpers.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.342085 toughio-1.9.1/toughio/_io/input/json/
--rw-rw-rw-   0        0        0      156 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_io/input/json/__init__.py
--rw-rw-rw-   0        0        0     1911 2022-04-27 15:33:43.000000 toughio-1.9.1/toughio/_io/input/json/_json.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.350083 toughio-1.9.1/toughio/_io/input/tough/
--rw-rw-rw-   0        0        0      170 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_io/input/tough/__init__.py
--rw-rw-rw-   0        0        0     5494 2022-04-27 15:33:43.000000 toughio-1.9.1/toughio/_io/input/tough/_common.py
--rw-rw-rw-   0        0        0    12088 2022-04-27 15:33:43.000000 toughio-1.9.1/toughio/_io/input/tough/_helpers.py
--rw-rw-rw-   0        0        0    30010 2022-05-02 18:51:57.000000 toughio-1.9.1/toughio/_io/input/tough/_read.py
--rw-rw-rw-   0        0        0    39883 2022-04-27 15:33:43.000000 toughio-1.9.1/toughio/_io/input/tough/_write.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.355086 toughio-1.9.1/toughio/_io/output/
--rw-rw-rw-   0        0        0      237 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_io/output/__init__.py
--rw-rw-rw-   0        0        0     1172 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_io/output/_common.py
--rw-rw-rw-   0        0        0     5562 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_io/output/_helpers.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.358086 toughio-1.9.1/toughio/_io/output/csv/
--rw-rw-rw-   0        0        0      153 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_io/output/csv/__init__.py
--rw-rw-rw-   0        0        0     4228 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_io/output/csv/_csv.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.361119 toughio-1.9.1/toughio/_io/output/petrasim/
--rw-rw-rw-   0        0        0      157 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_io/output/petrasim/__init__.py
--rw-rw-rw-   0        0        0     2399 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_io/output/petrasim/_petrasim.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.364084 toughio-1.9.1/toughio/_io/output/save/
--rw-rw-rw-   0        0        0      121 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_io/output/save/__init__.py
--rw-rw-rw-   0        0        0     1070 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_io/output/save/_save.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.367110 toughio-1.9.1/toughio/_io/output/tecplot/
--rw-rw-rw-   0        0        0      147 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_io/output/tecplot/__init__.py
--rw-rw-rw-   0        0        0     2781 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_io/output/tecplot/_tecplot.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.370086 toughio-1.9.1/toughio/_io/output/tough/
--rw-rw-rw-   0        0        0      123 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_io/output/tough/__init__.py
--rw-rw-rw-   0        0        0     4818 2022-04-27 15:33:43.000000 toughio-1.9.1/toughio/_io/output/tough/_tough.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.379119 toughio-1.9.1/toughio/_mesh/
--rw-rw-rw-   0        0        0      401 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_mesh/__init__.py
--rw-rw-rw-   0        0        0     6150 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/_common.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.381083 toughio-1.9.1/toughio/_mesh/_filter/
--rw-rw-rw-   0        0        0       90 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_mesh/_filter/__init__.py
--rw-rw-rw-   0        0        0     1722 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_mesh/_filter/_helpers.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.384119 toughio-1.9.1/toughio/_mesh/_filter/box/
--rw-rw-rw-   0        0        0       61 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_mesh/_filter/box/__init__.py
--rw-rw-rw-   0        0        0      776 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/_filter/box/_box.py
--rw-rw-rw-   0        0        0    10485 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/_helpers.py
--rw-rw-rw-   0        0        0    31814 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/_mesh.py
--rw-rw-rw-   0        0        0     8384 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/_properties.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.386206 toughio-1.9.1/toughio/_mesh/avsucd/
--rw-rw-rw-   0        0        0      172 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_mesh/avsucd/__init__.py
--rw-rw-rw-   0        0        0     7782 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/avsucd/_avsucd.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.390084 toughio-1.9.1/toughio/_mesh/flac3d/
--rw-rw-rw-   0        0        0      178 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_mesh/flac3d/__init__.py
--rw-rw-rw-   0        0        0    15624 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/flac3d/_flac3d.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.393087 toughio-1.9.1/toughio/_mesh/pickle/
--rw-rw-rw-   0        0        0      170 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_mesh/pickle/__init__.py
--rw-rw-rw-   0        0        0      979 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/pickle/_pickle.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.396083 toughio-1.9.1/toughio/_mesh/tecplot/
--rw-rw-rw-   0        0        0      155 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_mesh/tecplot/__init__.py
--rw-rw-rw-   0        0        0    14166 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/tecplot/_tecplot.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.400085 toughio-1.9.1/toughio/_mesh/tough/
--rw-rw-rw-   0        0        0      151 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/_mesh/tough/__init__.py
--rw-rw-rw-   0        0        0     5576 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/tough/_helpers.py
--rw-rw-rw-   0        0        0    13278 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/_mesh/tough/_tough.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.410085 toughio-1.9.1/toughio/capillarity/
--rw-rw-rw-   0        0        0      254 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/capillarity/__init__.py
--rw-rw-rw-   0        0        0     4011 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/capillarity/_base.py
--rw-rw-rw-   0        0        0     1236 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/capillarity/_linear.py
--rw-rw-rw-   0        0        0     1000 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/capillarity/_milly.py
--rw-rw-rw-   0        0        0     1606 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/capillarity/_pickens.py
--rw-rw-rw-   0        0        0     1616 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/capillarity/_trust.py
--rw-rw-rw-   0        0        0     1783 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/capillarity/_van_genuchten.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.412084 toughio-1.9.1/toughio/data/
--rw-rw-rw-   0        0        0   624121 2021-12-06 20:12:30.000000 toughio-1.9.1/toughio/data/CO2TAB
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.421085 toughio-1.9.1/toughio/meshmaker/
--rw-rw-rw-   0        0        0      327 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/meshmaker/__init__.py
--rw-rw-rw-   0        0        0     3778 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/meshmaker/_cylindric_grid.py
--rw-rw-rw-   0        0        0     7561 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/meshmaker/_helpers.py
--rw-rw-rw-   0        0        0     4592 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/meshmaker/_structured_grid.py
--rw-rw-rw-   0        0        0     1289 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/meshmaker/_triangulate.py
--rw-rw-rw-   0        0        0     1930 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/meshmaker/_voxelize.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.434083 toughio-1.9.1/toughio/relative_permeability/
--rw-rw-rw-   0        0        0      374 2021-12-06 20:12:28.000000 toughio-1.9.1/toughio/relative_permeability/__init__.py
--rw-rw-rw-   0        0        0     4213 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/relative_permeability/_base.py
--rw-rw-rw-   0        0        0     1291 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/relative_permeability/_corey.py
--rw-rw-rw-   0        0        0     1025 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/relative_permeability/_fatt_klikoff.py
--rw-rw-rw-   0        0        0     1264 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/relative_permeability/_grant.py
--rw-rw-rw-   0        0        0     1705 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/relative_permeability/_linear.py
--rw-rw-rw-   0        0        0      758 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/relative_permeability/_pickens.py
--rw-rw-rw-   0        0        0     1767 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/relative_permeability/_van_genuchten_mualem.py
--rw-rw-rw-   0        0        0     1452 2022-04-27 15:26:33.000000 toughio-1.9.1/toughio/relative_permeability/_verma.py
-drwxrwxrwx   0        0        0        0 2022-05-02 18:53:59.326085 toughio-1.9.1/toughio.egg-info/
--rw-rw-rw-   0        0        0    11097 2022-05-02 18:53:58.000000 toughio-1.9.1/toughio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2962 2022-05-02 18:53:59.000000 toughio-1.9.1/toughio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-02 18:53:58.000000 toughio-1.9.1/toughio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      211 2022-05-02 18:53:58.000000 toughio-1.9.1/toughio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2022-05-02 18:53:59.000000 toughio-1.9.1/toughio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-05-02 18:53:59.000000 toughio-1.9.1/toughio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:22.045568 toughio-1.9.2/
+-rw-rw-rw-   0        0        0     2460 2021-12-06 20:12:26.000000 toughio-1.9.2/LICENSE
+-rw-rw-rw-   0        0        0    11097 2022-05-06 18:46:22.044546 toughio-1.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10034 2022-04-27 15:33:43.000000 toughio-1.9.2/README.rst
+-rw-rw-rw-   0        0        0       42 2022-05-06 18:46:22.045568 toughio-1.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     2981 2022-04-27 15:26:33.000000 toughio-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.898283 toughio-1.9.2/test/
+-rw-rw-rw-   0        0        0     1301 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_capillarity.py
+-rw-rw-rw-   0        0        0     8951 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_cli.py
+-rw-rw-rw-   0        0        0    31581 2022-05-06 18:38:14.000000 toughio-1.9.2/test/test_input.py
+-rw-rw-rw-   0        0        0     8668 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_mesh_methods.py
+-rw-rw-rw-   0        0        0      967 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_mesh_properties.py
+-rw-rw-rw-   0        0        0     1473 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_meshio.py
+-rw-rw-rw-   0        0        0     4479 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_meshmaker.py
+-rw-rw-rw-   0        0        0     5109 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_output.py
+-rw-rw-rw-   0        0        0     1282 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_relative_permeability.py
+-rw-rw-rw-   0        0        0     1567 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_time_series.py
+-rw-rw-rw-   0        0        0     5661 2022-04-27 15:26:33.000000 toughio-1.9.2/test/test_tough.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.906746 toughio-1.9.2/toughio/
+-rw-rw-rw-   0        0        0      185 2022-05-03 18:05:48.000000 toughio-1.9.2/toughio/__about__.py
+-rw-rw-rw-   0        0        0     1231 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.940448 toughio-1.9.2/toughio/_cli/
+-rw-rw-rw-   0        0        0      250 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_cli/__init__.py
+-rw-rw-rw-   0        0        0      920 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_cli/_co2tab.py
+-rw-rw-rw-   0        0        0     9805 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_cli/_export.py
+-rw-rw-rw-   0        0        0     4393 2022-05-03 18:20:15.000000 toughio-1.9.2/toughio/_cli/_extract.py
+-rw-rw-rw-   0        0        0     2465 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_cli/_merge.py
+-rw-rw-rw-   0        0        0     1541 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_cli/_save2incon.py
+-rw-rw-rw-   0        0        0     5512 2022-04-27 15:33:43.000000 toughio-1.9.2/toughio/_common.py
+-rw-rw-rw-   0        0        0       39 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_exceptions.py
+-rw-rw-rw-   0        0        0     1735 2022-04-27 15:33:43.000000 toughio-1.9.2/toughio/_helpers.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.944967 toughio-1.9.2/toughio/_io/
+-rw-rw-rw-   0        0        0      503 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_io/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.947563 toughio-1.9.2/toughio/_io/input/
+-rw-rw-rw-   0        0        0      134 2022-04-27 15:33:43.000000 toughio-1.9.2/toughio/_io/input/__init__.py
+-rw-rw-rw-   0        0        0     3544 2022-04-27 15:33:43.000000 toughio-1.9.2/toughio/_io/input/_helpers.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.950257 toughio-1.9.2/toughio/_io/input/json/
+-rw-rw-rw-   0        0        0      156 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_io/input/json/__init__.py
+-rw-rw-rw-   0        0        0     1911 2022-04-27 15:33:43.000000 toughio-1.9.2/toughio/_io/input/json/_json.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.958114 toughio-1.9.2/toughio/_io/input/tough/
+-rw-rw-rw-   0        0        0      170 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_io/input/tough/__init__.py
+-rw-rw-rw-   0        0        0     5516 2022-05-06 18:20:15.000000 toughio-1.9.2/toughio/_io/input/tough/_common.py
+-rw-rw-rw-   0        0        0    12115 2022-05-06 18:19:51.000000 toughio-1.9.2/toughio/_io/input/tough/_helpers.py
+-rw-rw-rw-   0        0        0    30125 2022-05-06 18:18:18.000000 toughio-1.9.2/toughio/_io/input/tough/_read.py
+-rw-rw-rw-   0        0        0    40073 2022-05-06 18:31:00.000000 toughio-1.9.2/toughio/_io/input/tough/_write.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.962740 toughio-1.9.2/toughio/_io/output/
+-rw-rw-rw-   0        0        0      237 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_io/output/__init__.py
+-rw-rw-rw-   0        0        0     1172 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_io/output/_common.py
+-rw-rw-rw-   0        0        0     5562 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_io/output/_helpers.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.965564 toughio-1.9.2/toughio/_io/output/csv/
+-rw-rw-rw-   0        0        0      153 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_io/output/csv/__init__.py
+-rw-rw-rw-   0        0        0     4228 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_io/output/csv/_csv.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.968657 toughio-1.9.2/toughio/_io/output/petrasim/
+-rw-rw-rw-   0        0        0      157 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_io/output/petrasim/__init__.py
+-rw-rw-rw-   0        0        0     2399 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_io/output/petrasim/_petrasim.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.972228 toughio-1.9.2/toughio/_io/output/save/
+-rw-rw-rw-   0        0        0      121 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_io/output/save/__init__.py
+-rw-rw-rw-   0        0        0     1070 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_io/output/save/_save.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.975453 toughio-1.9.2/toughio/_io/output/tecplot/
+-rw-rw-rw-   0        0        0      147 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_io/output/tecplot/__init__.py
+-rw-rw-rw-   0        0        0     2781 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_io/output/tecplot/_tecplot.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.977826 toughio-1.9.2/toughio/_io/output/tough/
+-rw-rw-rw-   0        0        0      123 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_io/output/tough/__init__.py
+-rw-rw-rw-   0        0        0     4853 2022-05-03 18:27:11.000000 toughio-1.9.2/toughio/_io/output/tough/_tough.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.984688 toughio-1.9.2/toughio/_mesh/
+-rw-rw-rw-   0        0        0      401 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_mesh/__init__.py
+-rw-rw-rw-   0        0        0     6150 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/_common.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.988845 toughio-1.9.2/toughio/_mesh/_filter/
+-rw-rw-rw-   0        0        0       90 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_mesh/_filter/__init__.py
+-rw-rw-rw-   0        0        0     1722 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_mesh/_filter/_helpers.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.991607 toughio-1.9.2/toughio/_mesh/_filter/box/
+-rw-rw-rw-   0        0        0       61 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_mesh/_filter/box/__init__.py
+-rw-rw-rw-   0        0        0      776 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/_filter/box/_box.py
+-rw-rw-rw-   0        0        0    10485 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/_helpers.py
+-rw-rw-rw-   0        0        0    31814 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/_mesh.py
+-rw-rw-rw-   0        0        0     8384 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/_properties.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.994696 toughio-1.9.2/toughio/_mesh/avsucd/
+-rw-rw-rw-   0        0        0      172 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_mesh/avsucd/__init__.py
+-rw-rw-rw-   0        0        0     7782 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/avsucd/_avsucd.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.997060 toughio-1.9.2/toughio/_mesh/flac3d/
+-rw-rw-rw-   0        0        0      178 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_mesh/flac3d/__init__.py
+-rw-rw-rw-   0        0        0    15624 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/flac3d/_flac3d.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.999644 toughio-1.9.2/toughio/_mesh/pickle/
+-rw-rw-rw-   0        0        0      170 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_mesh/pickle/__init__.py
+-rw-rw-rw-   0        0        0      979 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/pickle/_pickle.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:22.002811 toughio-1.9.2/toughio/_mesh/tecplot/
+-rw-rw-rw-   0        0        0      155 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_mesh/tecplot/__init__.py
+-rw-rw-rw-   0        0        0    14166 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/tecplot/_tecplot.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:22.008481 toughio-1.9.2/toughio/_mesh/tough/
+-rw-rw-rw-   0        0        0      151 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/_mesh/tough/__init__.py
+-rw-rw-rw-   0        0        0     5576 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/tough/_helpers.py
+-rw-rw-rw-   0        0        0    13278 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/_mesh/tough/_tough.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:22.018472 toughio-1.9.2/toughio/capillarity/
+-rw-rw-rw-   0        0        0      254 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/capillarity/__init__.py
+-rw-rw-rw-   0        0        0     4011 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/capillarity/_base.py
+-rw-rw-rw-   0        0        0     1236 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/capillarity/_linear.py
+-rw-rw-rw-   0        0        0     1000 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/capillarity/_milly.py
+-rw-rw-rw-   0        0        0     1606 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/capillarity/_pickens.py
+-rw-rw-rw-   0        0        0     1616 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/capillarity/_trust.py
+-rw-rw-rw-   0        0        0     1783 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/capillarity/_van_genuchten.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:22.020478 toughio-1.9.2/toughio/data/
+-rw-rw-rw-   0        0        0   624121 2021-12-06 20:12:30.000000 toughio-1.9.2/toughio/data/CO2TAB
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:22.030135 toughio-1.9.2/toughio/meshmaker/
+-rw-rw-rw-   0        0        0      327 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/meshmaker/__init__.py
+-rw-rw-rw-   0        0        0     3778 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/meshmaker/_cylindric_grid.py
+-rw-rw-rw-   0        0        0     7561 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/meshmaker/_helpers.py
+-rw-rw-rw-   0        0        0     4592 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/meshmaker/_structured_grid.py
+-rw-rw-rw-   0        0        0     1289 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/meshmaker/_triangulate.py
+-rw-rw-rw-   0        0        0     1930 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/meshmaker/_voxelize.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:22.043296 toughio-1.9.2/toughio/relative_permeability/
+-rw-rw-rw-   0        0        0      374 2021-12-06 20:12:28.000000 toughio-1.9.2/toughio/relative_permeability/__init__.py
+-rw-rw-rw-   0        0        0     4213 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/relative_permeability/_base.py
+-rw-rw-rw-   0        0        0     1291 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/relative_permeability/_corey.py
+-rw-rw-rw-   0        0        0     1025 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/relative_permeability/_fatt_klikoff.py
+-rw-rw-rw-   0        0        0     1264 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/relative_permeability/_grant.py
+-rw-rw-rw-   0        0        0     1705 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/relative_permeability/_linear.py
+-rw-rw-rw-   0        0        0      758 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/relative_permeability/_pickens.py
+-rw-rw-rw-   0        0        0     1767 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/relative_permeability/_van_genuchten_mualem.py
+-rw-rw-rw-   0        0        0     1452 2022-04-27 15:26:33.000000 toughio-1.9.2/toughio/relative_permeability/_verma.py
+drwxrwxrwx   0        0        0        0 2022-05-06 18:46:21.930550 toughio-1.9.2/toughio.egg-info/
+-rw-rw-rw-   0        0        0    11097 2022-05-06 18:46:21.000000 toughio-1.9.2/toughio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2962 2022-05-06 18:46:21.000000 toughio-1.9.2/toughio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-06 18:46:21.000000 toughio-1.9.2/toughio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      211 2022-05-06 18:46:21.000000 toughio-1.9.2/toughio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2022-05-06 18:46:21.000000 toughio-1.9.2/toughio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-05-06 18:46:21.000000 toughio-1.9.2/toughio.egg-info/top_level.txt
```

### Comparing `toughio-1.9.1/LICENSE` & `toughio-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/PKG-INFO` & `toughio-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toughio
-Version: 1.9.1
+Version: 1.9.2
 Summary: Pre- and post-processing Python library for TOUGH
 Home-page: https://github.com/keurfonluu/toughio
 Author: Keurfon Luu
 Author-email: keurfonluu@lbl.gov
 License: 3-Clause BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `toughio-1.9.1/README.rst` & `toughio-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/setup.py` & `toughio-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_capillarity.py` & `toughio-1.9.2/test/test_capillarity.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_cli.py` & `toughio-1.9.2/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_input.py` & `toughio-1.9.2/test/test_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,14 +524,49 @@
                 assert v == generator[k]
 
             else:
                 assert np.allclose(v, generator[k], atol=1.0e-4)
 
 
 @pytest.mark.parametrize("write_read", [write_read_tough, write_read_json])
+def test_gener_delv(write_read):
+    n_rnd = np.random.randint(10) + 2
+    parameters_ref = {
+        "generators": [
+            {
+                "label": helpers.random_label(5),
+                "name": helpers.random_string(5),
+                "nseq": np.random.randint(10),
+                "nadd": np.random.randint(10),
+                "nads": np.random.randint(10),
+                "type": "DELV",
+                "rates": np.random.rand(),
+                "specific_enthalpy": np.random.rand(),
+                "layer_thickness": np.random.rand(),
+            }
+            for _ in range(n_rnd)
+        ],
+    }
+    parameters_ref["generators"][0]["n_layer"] = n_rnd
+    parameters = write_read(parameters_ref)
+
+    assert len(parameters_ref["generators"]) == len(parameters["generators"])
+
+    for generator_ref, generator in zip(
+        parameters_ref["generators"], parameters["generators"]
+    ):
+        for k, v in generator_ref.items():
+            if k in {"label", "name", "type"}:
+                assert v == generator[k]
+
+            else:
+                assert np.allclose(v, generator[k], atol=1.0e-4)
+
+
+@pytest.mark.parametrize("write_read", [write_read_tough, write_read_json])
 def test_diffu(write_read):
     n_phase = np.random.randint(8) + 1
     parameters_ref = {
         "n_phase": n_phase,
         "diffusion": np.random.rand(np.random.randint(5) + 1, n_phase),
     }
     parameters = write_read(parameters_ref)
```

### Comparing `toughio-1.9.1/test/test_mesh_methods.py` & `toughio-1.9.2/test/test_mesh_methods.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_mesh_properties.py` & `toughio-1.9.2/test/test_mesh_properties.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_meshio.py` & `toughio-1.9.2/test/test_meshio.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_meshmaker.py` & `toughio-1.9.2/test/test_meshmaker.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_output.py` & `toughio-1.9.2/test/test_output.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_relative_permeability.py` & `toughio-1.9.2/test/test_relative_permeability.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_time_series.py` & `toughio-1.9.2/test/test_time_series.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/test/test_tough.py` & `toughio-1.9.2/test/test_tough.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/__init__.py` & `toughio-1.9.2/toughio/__init__.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_cli/_co2tab.py` & `toughio-1.9.2/toughio/_cli/_co2tab.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_cli/_export.py` & `toughio-1.9.2/toughio/_cli/_export.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_cli/_extract.py` & `toughio-1.9.2/toughio/_cli/_extract.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_cli/_merge.py` & `toughio-1.9.2/toughio/_cli/_merge.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_cli/_save2incon.py` & `toughio-1.9.2/toughio/_cli/_save2incon.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_common.py` & `toughio-1.9.2/toughio/_common.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_helpers.py` & `toughio-1.9.2/toughio/_helpers.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_io/input/_helpers.py` & `toughio-1.9.2/toughio/_io/input/_helpers.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_io/input/json/_json.py` & `toughio-1.9.2/toughio/_io/input/json/_json.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_io/input/tough/_common.py` & `toughio-1.9.2/toughio/_io/input/tough/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
     "nadd": None,
     "nads": None,
     "type": None,
     "times": None,
     "rates": None,
     "specific_enthalpy": None,
     "layer_thickness": None,
+    "n_layer": None,
 }
 
 output = {
     "format": None,
     "variables": None,
 }
```

### Comparing `toughio-1.9.1/toughio/_io/input/tough/_helpers.py` & `toughio-1.9.2/toughio/_io/input/tough/_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         "nadd": "scalar",
         "nads": "scalar",
         "type": "str",
         "times": "scalar_array_like",
         "rates": "scalar_array_like",
         "specific_enthalpy": "scalar_array_like",
         "layer_thickness": "scalar",
+        "n_layer": "int",
     },
     "OUTPU": {"format": "str", "variables": "array_like"},
     "ELEME": {
         "nseq": "int",
         "nadd": "int",
         "material": "str_int",
         "volume": "scalar",
```

### Comparing `toughio-1.9.1/toughio/_io/input/tough/_read.py` & `toughio-1.9.2/toughio/_io/input/tough/_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -664,15 +664,15 @@
                 "nadd": data[3],
                 "nads": data[4],
                 "type": data[7],
                 "layer_thickness": data[11],
             }
 
             ltab = data[5]
-            if ltab and ltab > 1:
+            if ltab and ltab > 1 and tmp["type"] != "DELV":
                 itab = data[8]
                 keys = ["times", "rates"]
                 keys += ["specific_enthalpy"] if itab else []
                 for key in keys:
                     table = []
 
                     while len(table) < ltab:
@@ -687,14 +687,17 @@
                     {
                         "times": None,
                         "rates": data[9],
                         "specific_enthalpy": data[10],
                     }
                 )
 
+            if ltab and tmp["type"] == "DELV":
+                tmp["n_layer"] = ltab
+
             gener["generators"].append(tmp)
 
         else:
             break
 
         line = f.next()
```

### Comparing `toughio-1.9.1/toughio/_io/input/tough/_write.py` & `toughio-1.9.2/toughio/_io/input/tough/_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -976,14 +976,17 @@
                     else:
                         if np.ndim(data[key]) != 1:
                             raise TypeError()
 
                         if ltab != len(data[key]):
                             raise ValueError()
 
+        elif data["type"] == "DELV" and data["n_layer"]:
+            ltab = data["n_layer"]
+
         else:
             for key in ["rates", "specific_enthalpy"]:
                 if key in data and np.ndim(data[key]) > 0:
                     if len(data[key]) > 1:
                         raise ValueError()
 
                     data[key] = data[key][0]
@@ -1001,34 +1004,35 @@
             data["nseq"],
             data["nadd"],
             data["nads"],
             ltab if ltab > 1 else None,
             None,
             data["type"],
             itab,
-            None if ltab > 1 else data["rates"],
-            None if ltab > 1 else data["specific_enthalpy"],
+            None if ltab > 1 and data["type"] != "DELV" else data["rates"],
+            None if ltab > 1 and data["type"] != "DELV" else data["specific_enthalpy"],
             data["layer_thickness"],
         ]
         out += write_record(values, fmt1)
 
-        # Record 2
-        out += write_record(data["times"], fmt2, multi=True) if ltab > 1 else []
-
-        # Record 3
-        out += write_record(data["rates"], fmt2, multi=True) if ltab > 1 else []
-
-        # Record 4
-        if ltab > 1 and data["specific_enthalpy"] is not None:
-            if isinstance(data["specific_enthalpy"], (list, tuple, np.ndarray)):
-                specific_enthalpy = data["specific_enthalpy"]
-            else:
-                specific_enthalpy = np.full(ltab, data["specific_enthalpy"])
+        if ltab > 1 and data["type"] != "DELV":
+            # Record 2
+            out += write_record(data["times"], fmt2, multi=True)
+
+            # Record 3
+            out += write_record(data["rates"], fmt2, multi=True)
+
+            # Record 4
+            if data["specific_enthalpy"] is not None:
+                if isinstance(data["specific_enthalpy"], (list, tuple, np.ndarray)):
+                    specific_enthalpy = data["specific_enthalpy"]
+                else:
+                    specific_enthalpy = np.full(ltab, data["specific_enthalpy"])
 
-            out += write_record(specific_enthalpy, fmt2, multi=True)
+                out += write_record(specific_enthalpy, fmt2, multi=True)
 
     return out
 
 
 @block("DIFFU")
 def _write_diffu(parameters):
     """Write DIFFU block data."""
```

### Comparing `toughio-1.9.1/toughio/_io/output/_common.py` & `toughio-1.9.2/toughio/_io/output/_common.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_io/output/_helpers.py` & `toughio-1.9.2/toughio/_io/output/_helpers.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_io/output/csv/_csv.py` & `toughio-1.9.2/toughio/_io/output/csv/_csv.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_io/output/petrasim/_petrasim.py` & `toughio-1.9.2/toughio/_io/output/petrasim/_petrasim.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_io/output/save/_save.py` & `toughio-1.9.2/toughio/_io/output/save/_save.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_io/output/tecplot/_tecplot.py` & `toughio-1.9.2/toughio/_io/output/tecplot/_tecplot.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_io/output/tough/_tough.py` & `toughio-1.9.2/toughio/_io/output/tough/_tough.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 line = next(f)
                 if line.strip():
                     break
 
             # Loop until end of output block
             while True:
                 if line[:10].strip() and not line.strip().startswith("ELEM"):
-                    line = line.lstrip()
+                    line = line[1:] if file_type == "element" else line[5:]
 
                     if first and not label_length:
                         label_length = get_label_length(line[:9])
                         iend = (
                             label_length
                             if file_type == "element"
                             else 2 * label_length + 2
```

### Comparing `toughio-1.9.1/toughio/_mesh/_common.py` & `toughio-1.9.2/toughio/_mesh/_common.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/_filter/_helpers.py` & `toughio-1.9.2/toughio/_mesh/_filter/_helpers.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/_filter/box/_box.py` & `toughio-1.9.2/toughio/_mesh/_filter/box/_box.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/_helpers.py` & `toughio-1.9.2/toughio/_mesh/_helpers.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/_mesh.py` & `toughio-1.9.2/toughio/_mesh/_mesh.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/_properties.py` & `toughio-1.9.2/toughio/_mesh/_properties.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/avsucd/_avsucd.py` & `toughio-1.9.2/toughio/_mesh/avsucd/_avsucd.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/flac3d/_flac3d.py` & `toughio-1.9.2/toughio/_mesh/flac3d/_flac3d.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/pickle/_pickle.py` & `toughio-1.9.2/toughio/_mesh/pickle/_pickle.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/tecplot/_tecplot.py` & `toughio-1.9.2/toughio/_mesh/tecplot/_tecplot.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/tough/_helpers.py` & `toughio-1.9.2/toughio/_mesh/tough/_helpers.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/_mesh/tough/_tough.py` & `toughio-1.9.2/toughio/_mesh/tough/_tough.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/capillarity/_base.py` & `toughio-1.9.2/toughio/capillarity/_base.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/capillarity/_linear.py` & `toughio-1.9.2/toughio/capillarity/_linear.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/capillarity/_milly.py` & `toughio-1.9.2/toughio/capillarity/_milly.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/capillarity/_pickens.py` & `toughio-1.9.2/toughio/capillarity/_pickens.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/capillarity/_trust.py` & `toughio-1.9.2/toughio/capillarity/_trust.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/capillarity/_van_genuchten.py` & `toughio-1.9.2/toughio/capillarity/_van_genuchten.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/data/CO2TAB` & `toughio-1.9.2/toughio/data/CO2TAB`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/meshmaker/_cylindric_grid.py` & `toughio-1.9.2/toughio/meshmaker/_cylindric_grid.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/meshmaker/_helpers.py` & `toughio-1.9.2/toughio/meshmaker/_helpers.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/meshmaker/_structured_grid.py` & `toughio-1.9.2/toughio/meshmaker/_structured_grid.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/meshmaker/_triangulate.py` & `toughio-1.9.2/toughio/meshmaker/_triangulate.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/meshmaker/_voxelize.py` & `toughio-1.9.2/toughio/meshmaker/_voxelize.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/relative_permeability/_base.py` & `toughio-1.9.2/toughio/relative_permeability/_base.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/relative_permeability/_corey.py` & `toughio-1.9.2/toughio/relative_permeability/_corey.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/relative_permeability/_fatt_klikoff.py` & `toughio-1.9.2/toughio/relative_permeability/_fatt_klikoff.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/relative_permeability/_grant.py` & `toughio-1.9.2/toughio/relative_permeability/_grant.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/relative_permeability/_linear.py` & `toughio-1.9.2/toughio/relative_permeability/_linear.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/relative_permeability/_pickens.py` & `toughio-1.9.2/toughio/relative_permeability/_pickens.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/relative_permeability/_van_genuchten_mualem.py` & `toughio-1.9.2/toughio/relative_permeability/_van_genuchten_mualem.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio/relative_permeability/_verma.py` & `toughio-1.9.2/toughio/relative_permeability/_verma.py`

 * *Files identical despite different names*

### Comparing `toughio-1.9.1/toughio.egg-info/PKG-INFO` & `toughio-1.9.2/toughio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toughio
-Version: 1.9.1
+Version: 1.9.2
 Summary: Pre- and post-processing Python library for TOUGH
 Home-page: https://github.com/keurfonluu/toughio
 Author: Keurfon Luu
 Author-email: keurfonluu@lbl.gov
 License: 3-Clause BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `toughio-1.9.1/toughio.egg-info/SOURCES.txt` & `toughio-1.9.2/toughio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

