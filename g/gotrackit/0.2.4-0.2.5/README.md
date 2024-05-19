# Comparing `tmp/gotrackit-0.2.4.tar.gz` & `tmp/gotrackit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrackit-0.2.4.tar", last modified: Wed May  8 07:31:42 2024, max compression
+gzip compressed data, was "gotrackit-0.2.5.tar", last modified: Sun May 19 13:48:06 2024, max compression
```

## Comparing `gotrackit-0.2.4.tar` & `gotrackit-0.2.5.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.077210 gotrackit-0.2.4/
--rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     7990 2024-05-08 07:31:42.076213 gotrackit-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     7244 2024-05-08 07:07:22.000000 gotrackit-0.2.4/README.md
--rw-rw-rw-   0        0        0      795 2024-05-08 07:22:19.000000 gotrackit-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 07:31:42.077210 gotrackit-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.000415 gotrackit-0.2.4/src/
--rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.004404 gotrackit-0.2.4/src/gotrackit/
--rw-rw-rw-   0        0        0    15805 2024-04-29 14:02:05.000000 gotrackit-0.2.4/src/gotrackit/GlobalVal.py
--rw-rw-rw-   0        0        0    17874 2024-05-07 03:22:33.000000 gotrackit-0.2.4/src/gotrackit/MapMatch.py
--rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.4/src/gotrackit/WrapsFunc.py
--rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.4/src/gotrackit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.012383 gotrackit-0.2.4/src/gotrackit/generation/
--rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.4/src/gotrackit/generation/GpsGen.py
--rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.4/src/gotrackit/generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.016373 gotrackit-0.2.4/src/gotrackit/gps/
--rw-rw-rw-   0        0        0     4275 2024-04-30 05:17:12.000000 gotrackit-0.2.4/src/gotrackit/gps/GpsArray.py
--rw-rw-rw-   0        0        0     8333 2024-05-07 13:58:22.000000 gotrackit-0.2.4/src/gotrackit/gps/GpsTrip.py
--rw-rw-rw-   0        0        0     3896 2024-04-30 05:17:12.000000 gotrackit-0.2.4/src/gotrackit/gps/GpsXfer.py
--rw-rw-rw-   0        0        0    22763 2024-05-07 03:27:27.000000 gotrackit-0.2.4/src/gotrackit/gps/LocGps.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.4/src/gotrackit/gps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.019364 gotrackit-0.2.4/src/gotrackit/map/
--rw-rw-rw-   0        0        0    19826 2024-05-08 05:02:02.000000 gotrackit-0.2.4/src/gotrackit/map/Link.py
--rw-rw-rw-   0        0        0    38784 2024-05-08 07:13:14.000000 gotrackit-0.2.4/src/gotrackit/map/Net.py
--rw-rw-rw-   0        0        0     4848 2024-05-07 05:58:17.000000 gotrackit-0.2.4/src/gotrackit/map/Node.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.4/src/gotrackit/map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.023353 gotrackit-0.2.4/src/gotrackit/model/
--rw-rw-rw-   0        0        0    53479 2024-05-08 07:15:53.000000 gotrackit-0.2.4/src/gotrackit/model/Markov.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.4/src/gotrackit/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.027343 gotrackit-0.2.4/src/gotrackit/netreverse/
--rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.4/src/gotrackit/netreverse/GlobalVal.py
--rw-rw-rw-   0        0        0    27388 2024-05-07 03:33:38.000000 gotrackit-0.2.4/src/gotrackit/netreverse/NetGen.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.029338 gotrackit-0.2.4/src/gotrackit/netreverse/Parse/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Parse/__init__.py
--rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Parse/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.033327 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/
--rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/GeoProcess.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/GraphAna.py
--rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/IndexAna.py
--rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/MapProcess.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/od.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.035322 gotrackit-0.2.4/src/gotrackit/netreverse/Request/
--rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.036319 gotrackit-0.2.4/src/gotrackit/netreverse/Request/api/
--rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/api/WebApi.py
--rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/api/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/request_path.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.042305 gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/
--rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/__init__.py
--rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/bd_ts.py
--rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.047290 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.048287 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/DupProcess/
--rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.051279 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/
--rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
--rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.056266 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
--rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.058261 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
--rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.062250 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.063248 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/SaveStreets/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
--rw-rw-rw-   0        0        0    21421 2024-04-30 12:21:10.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.065242 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Split/
--rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Split/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.066239 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Tools/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
--rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Tools/process.py
--rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/__init__.py
--rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/conn.py
--rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/increment.py
--rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/net_reverse.py
--rw-rw-rw-   0        0        0     5758 2024-04-20 03:45:37.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/optimize_net.py
--rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/save_file.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.4/src/gotrackit/netreverse/__init__.py
--rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.4/src/gotrackit/netreverse/book_mark.py
--rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.4/src/gotrackit/netreverse/format_od.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.067237 gotrackit-0.2.4/src/gotrackit/netxfer/
--rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.4/src/gotrackit/netxfer/SumoConvert.py
--rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.4/src/gotrackit/netxfer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.071225 gotrackit-0.2.4/src/gotrackit/solver/
--rw-rw-rw-   0        0        0     9156 2024-05-07 23:25:32.000000 gotrackit-0.2.4/src/gotrackit/solver/Viterbi.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.4/src/gotrackit/solver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.075216 gotrackit-0.2.4/src/gotrackit/tools/
--rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.4/src/gotrackit/tools/__init__.py
--rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.4/src/gotrackit/tools/coord_trans.py
--rw-rw-rw-   0        0        0    12123 2024-05-06 03:34:25.000000 gotrackit-0.2.4/src/gotrackit/tools/geo_process.py
--rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.4/src/gotrackit/tools/group.py
--rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.4/src/gotrackit/tools/save_file.py
--rw-rw-rw-   0        0        0    10550 2024-05-07 01:39:06.000000 gotrackit-0.2.4/src/gotrackit/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:31:42.076213 gotrackit-0.2.4/src/gotrackit.egg-info/
--rw-rw-rw-   0        0        0     7990 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3695 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-08 07:31:41.000000 gotrackit-0.2.4/src/gotrackit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.978852 gotrackit-0.2.5/
+-rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     7735 2024-05-19 13:48:06.978852 gotrackit-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6989 2024-05-19 09:06:23.000000 gotrackit-0.2.5/README.md
+-rw-rw-rw-   0        0        0      795 2024-05-18 04:37:45.000000 gotrackit-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 13:48:06.978852 gotrackit-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.888421 gotrackit-0.2.5/src/
+-rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.896423 gotrackit-0.2.5/src/gotrackit/
+-rw-rw-rw-   0        0        0    16059 2024-05-17 07:53:49.000000 gotrackit-0.2.5/src/gotrackit/GlobalVal.py
+-rw-rw-rw-   0        0        0    17442 2024-05-19 09:31:55.000000 gotrackit-0.2.5/src/gotrackit/MapMatch.py
+-rw-rw-rw-   0        0        0      624 2024-05-18 04:36:05.000000 gotrackit-0.2.5/src/gotrackit/WrapsFunc.py
+-rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.5/src/gotrackit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.900422 gotrackit-0.2.5/src/gotrackit/generation/
+-rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.5/src/gotrackit/generation/GpsGen.py
+-rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.5/src/gotrackit/generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.904421 gotrackit-0.2.5/src/gotrackit/gps/
+-rw-rw-rw-   0        0        0     4241 2024-05-19 13:01:14.000000 gotrackit-0.2.5/src/gotrackit/gps/GpsArray.py
+-rw-rw-rw-   0        0        0     8021 2024-05-19 13:01:14.000000 gotrackit-0.2.5/src/gotrackit/gps/GpsTrip.py
+-rw-rw-rw-   0        0        0     3896 2024-04-30 05:17:12.000000 gotrackit-0.2.5/src/gotrackit/gps/GpsXfer.py
+-rw-rw-rw-   0        0        0    21654 2024-05-19 13:34:52.000000 gotrackit-0.2.5/src/gotrackit/gps/LocGps.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.5/src/gotrackit/gps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.913588 gotrackit-0.2.5/src/gotrackit/map/
+-rw-rw-rw-   0        0        0    20406 2024-05-17 07:59:43.000000 gotrackit-0.2.5/src/gotrackit/map/Link.py
+-rw-rw-rw-   0        0        0    40402 2024-05-17 08:31:42.000000 gotrackit-0.2.5/src/gotrackit/map/Net.py
+-rw-rw-rw-   0        0        0     4848 2024-05-18 04:12:21.000000 gotrackit-0.2.5/src/gotrackit/map/Node.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.5/src/gotrackit/map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.917016 gotrackit-0.2.5/src/gotrackit/model/
+-rw-rw-rw-   0        0        0    59444 2024-05-19 10:05:45.000000 gotrackit-0.2.5/src/gotrackit/model/Markov.py
+-rw-rw-rw-   0        0        0     2441 2024-05-19 12:17:01.000000 gotrackit-0.2.5/src/gotrackit/model/Para.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.5/src/gotrackit/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.921018 gotrackit-0.2.5/src/gotrackit/netreverse/
+-rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.5/src/gotrackit/netreverse/GlobalVal.py
+-rw-rw-rw-   0        0        0    27460 2024-05-08 15:05:30.000000 gotrackit-0.2.5/src/gotrackit/netreverse/NetGen.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.921018 gotrackit-0.2.5/src/gotrackit/netreverse/Parse/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Parse/__init__.py
+-rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Parse/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.929018 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/
+-rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/GeoProcess.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/GraphAna.py
+-rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/IndexAna.py
+-rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/MapProcess.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/od.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.929018 gotrackit-0.2.5/src/gotrackit/netreverse/Request/
+-rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.933019 gotrackit-0.2.5/src/gotrackit/netreverse/Request/api/
+-rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/api/WebApi.py
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/api/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/request_path.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.937018 gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/__init__.py
+-rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/bd_ts.py
+-rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.941018 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.945019 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/DupProcess/
+-rw-rw-rw-   0        0        0    21741 2024-05-08 08:28:07.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.949019 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/
+-rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
+-rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.953022 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    12237 2024-05-08 09:22:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
+-rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.953022 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
+-rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.962696 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    21567 2024-05-08 09:34:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.964854 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/SaveStreets/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
+-rw-rw-rw-   0        0        0    22373 2024-05-18 04:15:30.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.964854 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Split/
+-rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Split/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.968885 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Tools/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
+-rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Tools/process.py
+-rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/__init__.py
+-rw-rw-rw-   0        0        0     9629 2024-05-10 08:28:49.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/conn.py
+-rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/increment.py
+-rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/net_reverse.py
+-rw-rw-rw-   0        0        0     5790 2024-05-08 09:34:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/optimize_net.py
+-rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/save_file.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.5/src/gotrackit/netreverse/book_mark.py
+-rw-rw-rw-   0        0        0     1872 2024-05-08 09:34:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/format_od.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.968885 gotrackit-0.2.5/src/gotrackit/netxfer/
+-rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.5/src/gotrackit/netxfer/SumoConvert.py
+-rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.5/src/gotrackit/netxfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.973405 gotrackit-0.2.5/src/gotrackit/solver/
+-rw-rw-rw-   0        0        0     9156 2024-05-07 23:25:32.000000 gotrackit-0.2.5/src/gotrackit/solver/Viterbi.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.5/src/gotrackit/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.978852 gotrackit-0.2.5/src/gotrackit/tools/
+-rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.5/src/gotrackit/tools/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.5/src/gotrackit/tools/coord_trans.py
+-rw-rw-rw-   0        0        0    12569 2024-05-17 05:28:38.000000 gotrackit-0.2.5/src/gotrackit/tools/geo_process.py
+-rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.5/src/gotrackit/tools/group.py
+-rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.5/src/gotrackit/tools/save_file.py
+-rw-rw-rw-   0        0        0    10550 2024-05-07 01:39:06.000000 gotrackit-0.2.5/src/gotrackit/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.978852 gotrackit-0.2.5/src/gotrackit.egg-info/
+-rw-rw-rw-   0        0        0     7735 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3723 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/top_level.txt
```

### Comparing `gotrackit-0.2.4/LICENSE` & `gotrackit-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/PKG-INFO` & `gotrackit-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,64 +39,56 @@
 ~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
 
 Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
 </div>
 <br>
 
 
-
-**版本状态：05.07已经更新: v0.2.3**
+**版本状态：05.19即将更新: v0.2.5**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
+- 地图匹配接口效率优化, 相较于v0.2.4小幅度提升
 
-- 地图匹配接口效率优化, 相较于v0.2.2小幅度提升
-
-- 地图匹配接口报错机制优化
-
-- 地图匹配接口移除html_fldr参数, 使用out_fldr替代
-
-- 地图匹配接口增加即时输出开关instant_output, 打开后, 每匹配完一条轨迹马上进行结果存储
-
-- 路网构建: crs判断BUG修复、境外路网构建失败BUG修复
+- 新增网格参数搜索，帮助用户确定合理的匹配参数
 
-- 增加 环路 处理功能
+- BUG修复
 
 
 **不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
 
 
 <br>
 
 <div align=center>
-~ v0.2.4(相较于0.2.1)效率将大幅度提升, 最高可以提升10倍的性能 !~
+~ v0.2.5(相较于0.2.1)效率将大幅度提升, 最高可以提升15倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.4版解算时间 |
+| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.5版解算时间 |
 |----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
-| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.87秒**   |
-| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.89秒**   |
+| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.35秒**   |
+| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.60秒**   |
 
 
-v0.2.4多核效率对比:
+v0.2.5多核效率对比:
 
-基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快89s解算完150条轨迹，平均每条轨迹0.59s，相较于0.89s再次提升了30%，在车辆数较多时，多核的效率提升很明显。
+基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快71s解算完150条轨迹，平均每条轨迹0.47s，相较于0.60s再次提升了20%，在车辆数较多时，多核的效率提升很明显。
 
 | 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.4解算时间 |
 |-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
-| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 290.0秒     | 
-| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 130.6秒     |
-| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 113.3秒     |
-| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 97.3秒      | 
-| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 89.4秒      | 
-| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 91.5秒      | 
+| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 226.0秒     | 
+| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 101.6秒     |
+| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 88.3秒      |
+| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 75.3秒      | 
+| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 72.1秒      | 
+| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 71.5秒      | 
 
 
 <br>
 
 <div align=center>
 ~ 稀疏轨迹匹配与路径补全 ~
 </div>
```

### Comparing `gotrackit-0.2.4/README.md` & `gotrackit-0.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,64 +17,56 @@
 ~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
 
 Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
 </div>
 <br>
 
 
-
-**版本状态：05.07已经更新: v0.2.3**
+**版本状态：05.19即将更新: v0.2.5**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
+- 地图匹配接口效率优化, 相较于v0.2.4小幅度提升
 
-- 地图匹配接口效率优化, 相较于v0.2.2小幅度提升
-
-- 地图匹配接口报错机制优化
-
-- 地图匹配接口移除html_fldr参数, 使用out_fldr替代
-
-- 地图匹配接口增加即时输出开关instant_output, 打开后, 每匹配完一条轨迹马上进行结果存储
-
-- 路网构建: crs判断BUG修复、境外路网构建失败BUG修复
+- 新增网格参数搜索，帮助用户确定合理的匹配参数
 
-- 增加 环路 处理功能
+- BUG修复
 
 
 **不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
 
 
 <br>
 
 <div align=center>
-~ v0.2.4(相较于0.2.1)效率将大幅度提升, 最高可以提升10倍的性能 !~
+~ v0.2.5(相较于0.2.1)效率将大幅度提升, 最高可以提升15倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.4版解算时间 |
+| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.5版解算时间 |
 |----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
-| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.87秒**   |
-| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.89秒**   |
+| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.35秒**   |
+| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.60秒**   |
 
 
-v0.2.4多核效率对比:
+v0.2.5多核效率对比:
 
-基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快89s解算完150条轨迹，平均每条轨迹0.59s，相较于0.89s再次提升了30%，在车辆数较多时，多核的效率提升很明显。
+基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快71s解算完150条轨迹，平均每条轨迹0.47s，相较于0.60s再次提升了20%，在车辆数较多时，多核的效率提升很明显。
 
 | 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.4解算时间 |
 |-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
-| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 290.0秒     | 
-| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 130.6秒     |
-| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 113.3秒     |
-| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 97.3秒      | 
-| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 89.4秒      | 
-| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 91.5秒      | 
+| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 226.0秒     | 
+| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 101.6秒     |
+| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 88.3秒      |
+| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 75.3秒      | 
+| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 72.1秒      | 
+| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 71.5秒      | 
 
 
 <br>
 
 <div align=center>
 ~ 稀疏轨迹匹配与路径补全 ~
 </div>
```

### Comparing `gotrackit-0.2.4/pyproject.toml` & `gotrackit-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotrackit"
-version = "0.2.4"
+version = "0.2.5"
 dependencies = ["geopandas>=0.14.1", "shapely", "networkx", "pandas", "numpy", "keplergl", "geopy"]
 requires-python = ">=3.8"
 authors = [
   { name="Kai Tang", email="794568794@qq.com" },
 ]
 description = "A Python Package for Map Matching Algorithm Based on Hidden Markov Model"
 readme = "README.md"
```

### Comparing `gotrackit-0.2.4/src/gotrackit/GlobalVal.py` & `gotrackit-0.2.5/src/gotrackit/GlobalVal.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,17 @@
         self.GEOMETRY_FIELD = 'geometry'
         self.NODE_ID_FIELD = 'node_id'
         self.S_NODE = 'o_node'
         self.T_NODE = 'd_node'
         self.NODE_PATH_FIELD = 'path'
         self.COST_FIELD = 'cost'
         self.LINK_VEC_FIELD = 'dir_vec'
+        self.X_DIFF = 'lv_dx'
+        self.Y_DIFF = 'lv_dy'
+        self.VEC_LEN = 'lvl'
         self.SEG_COUNT = 'seg_count'
         self.SEG_ACCU_LENGTH = 'seg_accu_length'
 
 class GpsField(object):
     """gps数据字段"""
     def __init__(self):
         self.POINT_SEQ_FIELD = 'seq'
@@ -52,15 +55,20 @@
         self.ADJ_TIME_GAP = 'time_gap'
         self.ADJ_DIS = 'gps_adj_dis'
         self.ADJ_SPEED = 'adj_speed'
 
         self.DENSE_GEO = '__dens_geo__'
         self.N_SEGMENTS = '__n__'
 
-        self.DIFF_VEC = 'diff_vec'
+        self.X_DIFF = 'gv_dx'
+        self.Y_DIFF = 'gv_dy'
+        self.VEC_LEN = 'gvl'
+
+        self.PLAIN_X = 'prj_x'
+        self.PLAIN_Y = 'prj_y'
 
 
 class RouteField(object):
     """"""
     def __init__(self):
         self.PATH_ID_FIELD = 'path_id'
         self.TIME_COST_FIELD = 'time_cost'
@@ -81,14 +89,15 @@
         self.ROUTE_ITEM = 'route_item'
         self.STRAIGHT_LENGTH = 'straight_l'
         self.DIS_GAP = 'dis_gap'
         self.PRJ_L = 'prj_dis'
         self.PRJ_GEO = 'prj_p'
         self.DIS_TO_NEXT = 'dis_to_next'
         self.HEADING_GAP = 'heading_gap'
+        self.EMISSION_P = 'emission_p'
 
 
 class KeplerConfig(object):
     def __init__(self):
         self.__BASE_CONFIG = {
             'version': 'v1',
             'config': {
```

### Comparing `gotrackit-0.2.4/src/gotrackit/MapMatch.py` & `gotrackit-0.2.5/src/gotrackit/MapMatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -- coding: utf-8 --
 # @Time    : 2024/3/25 14:13
 # @Author  : TangKai
 # @Team    : ZheChengData
 import os
-
 import numpy as np
 import pandas as pd
 import multiprocessing
 from .map.Net import Net
+from .model.Para import ParaGrid
 from .tools.group import cut_group
 from .gps.LocGps import GpsPointsGdf
 from .model.Markov import HiddenMarkov
 from .GlobalVal import NetField, GpsField
 from .visualization import export_visualization
 
 
@@ -30,19 +30,19 @@
                  is_lower_f: bool = False, lower_n: int = 2,
                  use_heading_inf: bool = False, heading_para_array: np.ndarray = None,
                  dense_gps: bool = True, dense_interval: float = 80.0,
                  dwell_l_length: float = 10.0, dwell_n: int = 2, del_dwell: bool = True,
                  dup_threshold: float = 10.0,
                  is_rolling_average: bool = False, window: int = 2,
                  export_html: bool = False, use_gps_source: bool = False, out_fldr: str = None,
-                 export_geo_res: bool = False,
-                 node_num_threshold: int = 2000, top_k: int = 20, omitted_l: float = 6.0,
+                 export_geo_res: bool = False, top_k: int = 20, omitted_l: float = 6.0,
                  link_width: float = 1.5, node_radius: float = 1.5,
                  match_link_width: float = 5.0, gps_radius: float = 6.0, export_all_agents: bool = False,
-                 visualization_cache_times: int = 50, multi_core_save: bool = False, instant_output: bool = False):
+                 visualization_cache_times: int = 50, multi_core_save: bool = False, instant_output: bool = False,
+                 use_para_grid: bool = False, para_grid: ParaGrid = None):
         """
         :param flag_name: 标记字符名称, 会用于标记输出的可视化文件, 默认"test"
         :param net: gotrackit路网对象, 必须指定
         :param use_sub_net: 是否在子网络上进行计算, 默认True
         :param gps_df: GPS数据, 必须指定
         :param time_format: GPS数据中时间列的格式, 默认"%Y-%m-%d %H:%M:%S"
         :param time_unit: GPS数据中时间列的单位, 如果时间列是数值(秒或者毫秒), 默认's'
@@ -62,29 +62,27 @@
         :param dup_threshold: 利用GPS轨迹计算sub_net时, 先对GPS点原始轨迹做简化, 重复点检测阈值, 默认5m
         :param is_rolling_average: 是否启用滑动窗口平均对GPS数据进行降噪, 默认False
         :param window: 滑动窗口大小, 默认2
         :param export_html: 是否输出网页可视化结果html文件, 默认True
         :param use_gps_source: 是否在可视化结果中使用GPS源数据进行展示, 默认False
         :param out_fldr: 保存匹配结果的文件目录, 默认当前目录
         :param export_geo_res: 是否输出匹配结果的几何可视化文件, 默认False
-        :param node_num_threshold: 默认2000
         :param omitted_l: 当某GPS点与前后GPS点的平均距离小于该距离(m)时, 该GPS点的方向限制作用被取消
         :param gps_radius: HTML可视化中GPS点的半径大小，单位米，默认8米
         :param export_all_agents: 是否将所有agent的可视化存储于一个html文件中
         :param visualization_cache_times: 每匹配完几辆车再进行(html or geojson文件)结果的统一存储, 默认50
         :param multi_core_save: 是否启用多进程进行结果存储
         :param instant_output: 是否每匹配完一条轨迹就存储csv匹配结果
+        :param use_para_grid: 是否启用网格参数搜索
+        :param para_grid: 网格参数对象
         """
         # 坐标系投影
         self.plain_crs = net.planar_crs
         self.geo_crs = net.geo_crs
 
-        # 用于自动确定是否使用全局路网的指标
-        self.node_num_threshold = node_num_threshold
-
         # gps参数
         self.gps_df = gps_df
         self.time_format = time_format  # 时间列格式
         self.time_unit = time_unit  # 时间列单位
         self.is_lower_f = is_lower_f  # 是否降频率
         self.lower_n = lower_n  # 降频倍数
         self.del_dwell = del_dwell
@@ -133,19 +131,20 @@
 
         self.export_all_agents = export_all_agents
         self.visualization_cache_times = visualization_cache_times
         self.multi_core_save = multi_core_save
         self.sub_net_buffer = self.gps_buffer + self.gps_route_buffer_gap + max_increment_times * increment_buffer
         self.instant_output = instant_output
 
+        self.use_para_grid = use_para_grid
+        self.para_grid = para_grid
+
     def execute(self) -> tuple[pd.DataFrame, dict, list]:
         match_res_df = pd.DataFrame()
         hmm_res_list = []  # save hmm_res
-        if len(self.my_net.get_node_data()[node_id_field].unique()) <= self.node_num_threshold:
-            self.use_sub_net = False
         self.gps_df.dropna(subset=[agent_id_field], inplace=True)
         agent_num = len(self.gps_df[gps_field.AGENT_ID_FIELD].unique())
         if agent_num == 0:
             print('去除agent_id列空值行后, gps数据为空...')
             return match_res_df, self.may_error_list, self.error_list
 
         # 对每辆车的轨迹进行匹配
@@ -214,51 +213,35 @@
                 used_net = self.my_net
                 print(rf'using whole net')
 
             # 初始化一个隐马尔可夫模型
             hmm_obj = HiddenMarkov(net=used_net, gps_points=gps_obj, beta=self.beta, gps_sigma=self.gps_sigma,
                                    not_conn_cost=self.not_conn_cost, use_heading_inf=self.use_heading_inf,
                                    heading_para_array=self.heading_para_array, dis_para=self.dis_para,
-                                   top_k=self.top_k, omitted_l=self.omitted_l)
+                                   top_k=self.top_k, omitted_l=self.omitted_l, para_grid=self.para_grid)
+            if not self.use_para_grid:
+                is_success, _match_res_df = hmm_obj.hmm_execute(add_single_ft=add_single_ft)
+            else:
+                is_success, _match_res_df = hmm_obj.hmm_para_grid_execute(add_single_ft=add_single_ft,
+                                                                          agent_id=agent_id)
+                self.para_grid.init_para_grid()
 
-            # 求解参数
-            try:
-                is_success = hmm_obj.generate_markov_para(add_single_ft)
-            except Exception as e:
-                print(rf'解算HMM参数出错:{repr(e)}')
-                is_success = False
             if not is_success:
                 self.error_list.append(agent_id)
                 continue
 
-            # 求解模型
-            try:
-                hmm_obj.solve()
-            except Exception as e:
-                print(rf'求解HMM模型出错:{repr(e)}')
-                self.error_list.append(agent_id)
-                continue
+            if hmm_obj.is_warn:
+                self.may_error_list[agent_id] = hmm_obj.format_warn_info
 
-            # 获取结果
-            try:
-                _match_res_df = hmm_obj.acquire_res()
-            except Exception as e:
-                print(rf'获取匹配结果出错:{repr(e)}')
-                self.error_list.append(agent_id)
-                continue
             if self.instant_output:
                 _match_res_df.to_csv(os.path.join(self.out_fldr, rf'{agent_id}_match_res.csv'),
                                      encoding='utf_8_sig', index=False)
             else:
                 match_res_df = pd.concat([match_res_df, _match_res_df])
 
-            hmm_obj.format_war_info()
-            if hmm_obj.is_warn:
-                self.may_error_list[agent_id] = hmm_obj.format_warn_info
-
             # if export files
             if self.export_html or self.export_geo_res:
                 hmm_res_list.append(hmm_obj)
                 if len(hmm_res_list) >= self.visualization_cache_times or agent_count == agent_num:
                     export_visualization(hmm_obj_list=hmm_res_list, use_gps_source=self.use_gps_source,
                                          export_geo=self.export_geo_res, export_html=self.export_html,
                                          gps_radius=self.gps_radius, export_all_agents=self.export_all_agents,
@@ -299,21 +282,21 @@
                            dense_interval=self.dense_interval, dwell_l_length=self.dwell_l_length, dwell_n=self.dwell_n,
                            del_dwell=self.del_dwell,
                            dup_threshold=self.dup_threshold, is_rolling_average=self.is_rolling_average,
                            window=self.rolling_window,
                            export_html=self.export_html,
                            use_gps_source=self.use_gps_source, out_fldr=core_out_fldr,
                            export_geo_res=self.export_geo_res,
-                           node_num_threshold=self.node_num_threshold,
                            top_k=self.top_k, omitted_l=self.omitted_l, link_width=self.link_width,
                            node_radius=self.node_radius,
                            match_link_width=self.match_link_width, gps_radius=self.gps_radius,
                            export_all_agents=self.export_all_agents,
                            visualization_cache_times=self.visualization_cache_times,
-                           multi_core_save=False, instant_output=self.instant_output)
+                           multi_core_save=False, instant_output=self.instant_output, use_para_grid=self.use_para_grid,
+                           para_grid=self.para_grid)
             result = pool.apply_async(mmp.execute,
                                       args=())
             result_list.append(result)
         pool.close()
         pool.join()
 
         match_res, may_error, error = pd.DataFrame(), dict(), list()
```

### Comparing `gotrackit-0.2.4/src/gotrackit/WrapsFunc.py` & `gotrackit-0.2.5/src/gotrackit/WrapsFunc.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/generation/GpsGen.py` & `gotrackit-0.2.5/src/gotrackit/generation/GpsGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/gps/GpsArray.py` & `gotrackit-0.2.5/src/gotrackit/gps/GpsArray.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,26 +33,26 @@
         """
         self.geo_crs = geo_crs
         self.__crs = self.geo_crs
         self.plane_crs = plane_crs
         self.gps_point_dis_dict = dict()
         self.gps_points_gdf = gps_points_df
         self.check()
-        if gps_field.HEADING_FIELD not in self.gps_points_gdf.columns:
-            self.gps_points_gdf[gps_field.HEADING_FIELD] = 0.0
-        self.gps_points_gdf[gps_field.GEOMETRY_FIELD] = self.gps_points_gdf.apply(
-            lambda item: Point(item[gps_field.LNG_FIELD], item[gps_field.LAT_FIELD]), axis=1)
+        self.gps_points_gdf[gps_field.GEOMETRY_FIELD] = \
+            self.gps_points_gdf[[gps_field.LNG_FIELD, gps_field.LAT_FIELD]].apply(lambda p: Point(p), axis=1)
         self.gps_points_gdf = gpd.GeoDataFrame(self.gps_points_gdf, geometry=gps_field.GEOMETRY_FIELD,
                                                crs=self.geo_crs)
         try:
             self.gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.gps_points_gdf[gps_field.TIME_FIELD], format=time_format)
         except ValueError:
+            print(rf'time column does not match format {time_format}, try using time-unit: {time_unit}')
             self.gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.gps_points_gdf[gps_field.TIME_FIELD], unit=time_unit)
+
         self.gps_points_gdf.sort_values(by=[gps_field.TIME_FIELD], ascending=[True], inplace=True)
         self.gps_points_gdf.reset_index(inplace=True, drop=True)
         self.to_plane_prj()
 
         # 存储最原始的GPS信息
         self.__source_gps_points_gdf = self.gps_points_gdf.copy()
         self.check()
@@ -96,13 +96,13 @@
     def _get_prj_inf(gps_point: Point = None, line: LineString = None) -> tuple[Point, float, float, float]:
         """
         # 返回 (GPS投影点坐标, GPS点到投影点的直线距离, GPS投影点到line拓扑起点的路径距离, line的长度)
         :param gps_point:
         :param line:
         :return: (GPS投影点坐标, GPS点到投影点的直线距离, GPS投影点到line拓扑起点的路径距离, line的长度)
         """
-        prj_p, p_prj_l, prj_route_l, line_length, _, _ = prj_inf(p=gps_point, line=line)
+        prj_p, p_prj_l, prj_route_l, line_length, _, _, _ = prj_inf(p=gps_point, line=line)
         return prj_p, p_prj_l, prj_route_l, line_length
 
     @property
     def gps_list_length(self) -> int:
         return len(self.gps_points_gdf)
```

### Comparing `gotrackit-0.2.4/src/gotrackit/gps/GpsTrip.py` & `gotrackit-0.2.5/src/gotrackit/gps/GpsTrip.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,18 +56,14 @@
 
             # 时间差和距离差
             group_gps_gdf[next_time_field] = group_gps_gdf[time_field].shift(-1).fillna(group_gps_gdf[time_field])
             group_gps_gdf[next_p_field] = group_gps_gdf[geometry_field].shift(-1).fillna(group_gps_gdf[geometry_field])
             group_gps_gdf[time_gap_field] = group_gps_gdf[next_time_field] - group_gps_gdf[time_field]
             group_gps_gdf[time_gap_field] = group_gps_gdf[time_gap_field].apply(lambda t: t.seconds)
             group_gps_gdf[dis_gap_field] = group_gps_gdf[next_p_field].distance(group_gps_gdf[geometry_field])
-            # group_gps_gdf[time_gap_field] = group_gps_gdf.apply(
-            #     lambda row: (row[next_time_field] - row[time_field]).seconds, axis=1)
-            # group_gps_gdf[dis_gap_field] = group_gps_gdf.apply(
-            #     lambda row: row[next_p_field].distance(row[geometry_field]), axis=1)
 
             # 切分主行程
             group_gps_gdf['main_label'] = (group_gps_gdf[time_gap_field] > self.group_gap_threshold).astype(int)
             self.add_group(label_field='main_label', df=group_gps_gdf, agent_id=agent_id)
             group_gps_gdf.drop(columns=['main_label'], axis=1, inplace=True)
 
             for _, _gps_df in group_gps_gdf.groupby(group_field):
```

### Comparing `gotrackit-0.2.4/src/gotrackit/gps/GpsXfer.py` & `gotrackit-0.2.5/src/gotrackit/gps/GpsXfer.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/gps/LocGps.py` & `gotrackit-0.2.5/src/gotrackit/gps/LocGps.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -- coding: utf-8 --
 # @Time    : 2023/12/10 20:12
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 """车辆GPS数据的相关方法和属性"""
 
-import datetime
 import numpy as np
 import pandas as pd
 import geopandas as gpd
 from ..map.Net import Net
 from datetime import timedelta
 from ..tools.geo_process import prj_inf
 from ..tools.geo_process import segmentize
@@ -31,15 +30,14 @@
 agent_field = gps_field.AGENT_ID_FIELD
 geometry_field = gps_field.GEOMETRY_FIELD
 time_gap_field = gps_field.ADJ_TIME_GAP
 dis_gap_field = gps_field.ADJ_DIS
 adj_speed_field = gps_field.ADJ_SPEED
 dense_geo_field = gps_field.DENSE_GEO
 n_seg_field = gps_field.N_SEGMENTS
-diff_vec = gps_field.DIFF_VEC
 geo_crs = prj_const.PRJ_CRS
 sub_group_field = gps_field.SUB_GROUP_FIELD
 
 
 class GpsPointsGdf(object):
 
     def __init__(self, gps_points_df: pd.DataFrame = None,
@@ -71,236 +69,213 @@
         self.dwell_l_length = dwell_l_length
         self.dwell_n = dwell_n
         self.__gps_point_dis_dict = dict()
         gps_points_df.reset_index(inplace=True, drop=True)
         self.__gps_points_gdf = gps_points_df
         self.agent_id = self.__gps_points_gdf.at[0, gps_field.AGENT_ID_FIELD]
         self.check()
-        if gps_field.HEADING_FIELD not in self.__gps_points_gdf.columns:
-            self.__gps_points_gdf[gps_field.HEADING_FIELD] = 0.0
-        self.__gps_points_gdf[gps_field.GEOMETRY_FIELD] = self.__gps_points_gdf.apply(
-            lambda item: Point(item[gps_field.LNG_FIELD], item[gps_field.LAT_FIELD]), axis=1)
+        self.__gps_points_gdf[gps_field.GEOMETRY_FIELD] = \
+            self.__gps_points_gdf[[gps_field.LNG_FIELD, gps_field.LAT_FIELD]].apply(lambda p: Point(p), axis=1)
         self.__gps_points_gdf = gpd.GeoDataFrame(self.__gps_points_gdf, geometry=gps_field.GEOMETRY_FIELD,
                                                  crs=self.geo_crs)
         try:
             self.__gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD], format=time_format)
         except ValueError:
+            print(rf'time column does not match format {time_format}, try using time-unit: {time_unit}')
             self.__gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD], unit=time_unit)
 
         self.__gps_points_gdf.sort_values(by=[gps_field.TIME_FIELD], ascending=[True], inplace=True)
         self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
-        self.__gps_points_gdf[gps_field.ORIGIN_POINT_SEQ_FIELD] = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD]
         self.__gps_points_gdf.reset_index(inplace=True, drop=True)
         self.to_plane_prj()
-        # self.calc_gps_point_dis()
+        self.generate_plain_xy()
+        self.gps_adj_dis_map = dict()
+        self.gps_seq_time_map = dict()
+        self.gps_seq_geo_map = dict()
 
         # 存储最原始的GPS信息
         self.__source_gps_points_gdf = self.__gps_points_gdf.copy()
 
         self.done_diff_heading = False
 
     def check(self):
         assert {gps_field.LNG_FIELD, gps_field.LAT_FIELD,
                 gps_field.AGENT_ID_FIELD, gps_field.TIME_FIELD}.issubset(
             set(self.__gps_points_gdf.columns)), \
             rf'GPS数据字段有误, 请至少包含如下字段: {gps_field.AGENT_ID_FIELD, gps_field.LNG_FIELD, gps_field.LAT_FIELD, gps_field.TIME_FIELD}'
 
+    def generate_plain_xy(self):
+        self.__gps_points_gdf[gps_field.PLAIN_X] = self.__gps_points_gdf[net_field.GEOMETRY_FIELD].apply(
+            lambda geo: geo.x)
+        self.__gps_points_gdf[gps_field.PLAIN_Y] = self.__gps_points_gdf[net_field.GEOMETRY_FIELD].apply(
+            lambda geo: geo.y)
+
     def dense(self) -> None:
         if len(self.__gps_points_gdf) <= 1:
             return None
         # 时间差和距离差
         self.calc_adj_dis_gap()
         self.calc_adj_time_gap()
-
         should_be_dense_gdf = self.__gps_points_gdf[self.__gps_points_gdf[dis_gap_field] > self.dense_interval].copy()
-        if should_be_dense_gdf.empty:
-            return None
         self.__gps_points_gdf.drop(columns=[next_time_field, next_p_field, time_gap_field, dis_gap_field], axis=1,
                                    inplace=True)
+        if should_be_dense_gdf.empty:
+            return None
 
-        should_be_dense_gdf[n_seg_field] = should_be_dense_gdf.apply(
-            lambda row: int(0.001 + row[dis_gap_field] / self.dense_interval) + 1, axis=1)
+        should_be_dense_gdf[n_seg_field] = (0.001 + should_be_dense_gdf[dis_gap_field] / self.dense_interval).astype(
+            int) + 1
+
+        dense_geo, dense_time = list(), list()
+        _ = [[dense_geo.append(segmentize(s_loc=(p.x, p.y), e_loc=(next_p.x, next_p.y), n=n)),
+              dense_time.append([t + timedelta(seconds=i * t_gap / n) for i in range(1, n)])]
+             for p, next_p, n, t, t_gap in zip(should_be_dense_gdf[geometry_field],
+                                               should_be_dense_gdf[next_p_field],
+                                               should_be_dense_gdf[n_seg_field], should_be_dense_gdf[time_field],
+                                               should_be_dense_gdf[time_gap_field])]
+        del _
+        should_be_dense_gdf[dense_geo_field] = dense_geo
+        should_be_dense_gdf[time_field] = dense_time
 
-        should_be_dense_gdf[[dense_geo_field, time_field]] = \
-            should_be_dense_gdf.apply(
-                lambda row: [
-                    list(segmentize(LineString([row[geometry_field], row[next_p_field]]), n=row[n_seg_field]).coords[
-                         1:-1]),
-                    [row[time_field] + timedelta(seconds=i * row[time_gap_field] / row[n_seg_field]) for i in
-                     range(1, row[n_seg_field])]],
-                axis=1, result_type='expand')
         should_be_dense_gdf.drop(columns=[geometry_field], axis=1, inplace=True)
         should_be_dense_gdf = pd.DataFrame(should_be_dense_gdf).explode(column=[time_field, dense_geo_field],
                                                                         ignore_index=True)
         should_be_dense_gdf.rename(columns={dense_geo_field: geometry_field}, inplace=True)
-        should_be_dense_gdf[geometry_field] = should_be_dense_gdf.apply(lambda row: Point(row[geometry_field]), axis=1)
-        should_be_dense_gdf.drop(columns=[next_time_field, next_p_field, time_gap_field, dis_gap_field], axis=1,
-                                 inplace=True)
+        should_be_dense_gdf[geometry_field] = should_be_dense_gdf[geometry_field].apply(lambda x: Point(x))
+        should_be_dense_gdf.drop(columns=[next_time_field, next_p_field, time_gap_field, dis_gap_field, n_seg_field],
+                                 axis=1, inplace=True)
+        # must be plain
         should_be_dense_gdf = gpd.GeoDataFrame(should_be_dense_gdf, geometry=geometry_field, crs=self.crs)
-        should_be_dense_gdf = should_be_dense_gdf.to_crs(self.geo_crs)
-        should_be_dense_gdf[[lng_field, lat_field]] = should_be_dense_gdf.apply(
-            lambda row: (row[geometry_field].x, row[geometry_field].y), axis=1, result_type='expand')
-        should_be_dense_gdf = should_be_dense_gdf.to_crs(self.plane_crs)
-
+        should_be_dense_gdf[gps_field.PLAIN_X] = should_be_dense_gdf[geometry_field].apply(lambda geo: geo.x)
+        should_be_dense_gdf[gps_field.PLAIN_Y] = should_be_dense_gdf[geometry_field].apply(lambda geo: geo.y)
         self.__gps_points_gdf = pd.concat([self.__gps_points_gdf, should_be_dense_gdf])
         self.__gps_points_gdf.sort_values(by=time_field, ascending=True, inplace=True)
         self.__gps_points_gdf.reset_index(inplace=True, drop=True)
         self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
-        self.__gps_points_gdf[gps_field.ORIGIN_POINT_SEQ_FIELD] = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD]
 
     def calc_adj_dis_gap(self) -> None:
         # 距离差
         self.__gps_points_gdf[next_p_field] = self.__gps_points_gdf[geometry_field].shift(-1).fillna(
             self.__gps_points_gdf[geometry_field])
-        # self.__gps_points_gdf[dis_gap_field] = self.__gps_points_gdf.apply(
-        #     lambda row: row[next_p_field].distance(row[geometry_field]), axis=1)
         self.__gps_points_gdf[dis_gap_field] = self.__gps_points_gdf[next_p_field].distance(
             self.__gps_points_gdf[geometry_field])
 
     def calc_adj_time_gap(self) -> None:
         # 时间差
         self.__gps_points_gdf[next_time_field] = self.__gps_points_gdf[time_field].shift(-1).fillna(
             self.__gps_points_gdf[time_field])
-        # self.__gps_points_gdf[time_gap_field] = self.__gps_points_gdf.apply(
-        #     lambda row: (row[next_time_field] - row[time_field]).seconds, axis=1)
         self.__gps_points_gdf[time_gap_field] = self.__gps_points_gdf[next_time_field] - self.__gps_points_gdf[
             time_field]
         self.__gps_points_gdf[time_gap_field] = self.__gps_points_gdf[time_gap_field].apply(lambda x: x.seconds)
 
     def calc_pre_next_dis(self) -> pd.DataFrame():
         self.calc_adj_dis_gap()
         # next_seq
         res = self.__gps_points_gdf.copy()
-        res[next_seq_field] = res[gps_field.POINT_SEQ_FIELD].shift(-1)
-        res.dropna(subset=[next_seq_field], inplace=True)
-        res[next_seq_field] = res[next_seq_field].astype(int)
-        return res[[gps_field.POINT_SEQ_FIELD, next_seq_field, gps_field.ADJ_DIS]]
+        self.gps_adj_dis_map = {seq: adj_dis for seq, adj_dis in zip(res[gps_field.POINT_SEQ_FIELD],
+                                                                     res[gps_field.ADJ_DIS])}
 
     def lower_frequency(self, n: int = 5):
         """
         GPS数据降频
         :param n: 降频倍数
         :return:
         """
         self.__gps_points_gdf['label'] = pd.Series([i for i in range(len(self.__gps_points_gdf))]) % n
         self.__gps_points_gdf = self.__gps_points_gdf[self.__gps_points_gdf['label'].eq(0)].copy()
-        self.__gps_points_gdf.drop(columns=['label'], axis=1, inplace=True)
+        del self.__gps_points_gdf['label']
 
     def rolling_average(self, window: int = 2):
         """
         滑动窗口降噪
         :param window: 窗口大小
         :return:
         """
+        # 滑动窗口执行后会重置所有的gps的seq字段
         if len(self.__gps_points_gdf) <= window:
             return None
+
         self.__gps_points_gdf[gps_field.TIME_FIELD] = self.__gps_points_gdf[gps_field.TIME_FIELD].apply(
             lambda t: t.timestamp())
-        self.__gps_points_gdf[gps_field.LNG_FIELD] = self.__gps_points_gdf[net_field.GEOMETRY_FIELD].apply(
-            lambda geo: geo.x)
-        self.__gps_points_gdf[gps_field.LAT_FIELD] = self.__gps_points_gdf[net_field.GEOMETRY_FIELD].apply(
-            lambda geo: geo.y)
-
-        # 滑动窗口执行后会重置所有的gps的seq字段
         self.__gps_points_gdf.reset_index(inplace=True, drop=True)
+        rolling_average_df = self.__gps_points_gdf[
+            [gps_field.PLAIN_X, gps_field.PLAIN_Y, gps_field.TIME_FIELD]].rolling(window=window).mean()
 
-        rolling_num_df = self.__gps_points_gdf[
-            [gps_field.LNG_FIELD, gps_field.LAT_FIELD, gps_field.TIME_FIELD]].rolling(window=window).mean()
-        rolling_heading_df = self.__gps_points_gdf[[gps_field.HEADING_FIELD]].rolling(window=window).median()
-
-        rolling_heading_df.dropna(subset=[gps_field.HEADING_FIELD], inplace=True)
-        rolling_num_df.dropna(subset=[gps_field.LNG_FIELD, gps_field.LAT_FIELD, gps_field.TIME_FIELD], inplace=True,
-                              how='any')
-
-        rolling_average_df = pd.concat([rolling_num_df, rolling_heading_df], axis=1)
+        rolling_average_df.dropna(subset=[gps_field.PLAIN_X, gps_field.PLAIN_Y, gps_field.TIME_FIELD], inplace=True,
+                                  how='any')
         rolling_average_df[gps_field.AGENT_ID_FIELD] = self.__gps_points_gdf.at[0, gps_field.AGENT_ID_FIELD]
-        del rolling_heading_df, rolling_num_df
 
         self.__gps_points_gdf = pd.concat([self.__gps_points_gdf.loc[[0], :],
                                            rolling_average_df,
                                            self.__gps_points_gdf.loc[[len(self.__gps_points_gdf) - 1], :]])
         del rolling_average_df
         self.__gps_points_gdf.reset_index(inplace=True, drop=True)
         self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
-
-        self.__gps_points_gdf[net_field.GEOMETRY_FIELD] = self.__gps_points_gdf[
-            [gps_field.LNG_FIELD, gps_field.LAT_FIELD]].apply(
-            lambda item: Point(item), axis=1)
-        self.__gps_points_gdf[gps_field.TIME_FIELD] = pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD],
-                                                                     unit='s')
-        self.__gps_points_gdf[gps_field.TIME_FIELD] = pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD],
-                                                                     format='%Y-%m-%d %H:%M:%S')
-
-    def calc_gps_point_dis(self) -> None:
-        seq_list = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD].to_list()
-        # {(from_seq, to_seq): dis, ...}
-        self.__gps_point_dis_dict = {
-            (seq_list[i], seq_list[i + 1]): self.__gps_points_gdf.at[seq_list[i], gps_field.GEOMETRY_FIELD].distance(
-                self.__gps_points_gdf.at[seq_list[i + 1], gps_field.GEOMETRY_FIELD]) for i in
-            range(len(self.__gps_points_gdf) - 1)}
-
-    def get_gps_point_dis(self, adj_gps_seq: tuple = None) -> float:
-        try:
-            dis = self.__gps_point_dis_dict[adj_gps_seq]
-        # some gps points do not have any candidate links
-        except KeyError:
-            dis = self.__gps_points_gdf.at[adj_gps_seq[0], gps_field.GEOMETRY_FIELD].distance(
-                self.__gps_points_gdf.at[adj_gps_seq[1], gps_field.GEOMETRY_FIELD])
-            self.__gps_point_dis_dict[adj_gps_seq] = dis
-        return dis
-
-    def get_adj_gps_dis_df(self):
-        return self.__gps_point_dis_dict
-
-    def plot_point(self):
-        pass
-
-    def get_gps_buffer_gdf(self):
-        pass
+        self.__gps_points_gdf[net_field.GEOMETRY_FIELD] = \
+            self.__gps_points_gdf[[gps_field.PLAIN_X, gps_field.PLAIN_Y]].apply(lambda item: Point(item), axis=1)
+        self.__gps_points_gdf[gps_field.TIME_FIELD] = \
+            pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD], unit='s')
+        self.__gps_points_gdf = gpd.GeoDataFrame(self.__gps_points_gdf, geometry=gps_field.GEOMETRY_FIELD, crs=self.crs)
 
     def calc_diff_heading(self):
         if self.done_diff_heading:
             return None
+        self.__gps_points_gdf['next_x'] = self.__gps_points_gdf[gps_field.PLAIN_X].shift(-1).fillna(
+            self.__gps_points_gdf[gps_field.PLAIN_X])
+        self.__gps_points_gdf['next_y'] = self.__gps_points_gdf[gps_field.PLAIN_Y].shift(-1).fillna(
+            self.__gps_points_gdf[gps_field.PLAIN_Y])
+        self.__gps_points_gdf['pre_x'] = self.__gps_points_gdf[gps_field.PLAIN_X].shift(1).fillna(
+            self.__gps_points_gdf[gps_field.PLAIN_X])
+        self.__gps_points_gdf['pre_y'] = self.__gps_points_gdf[gps_field.PLAIN_Y].shift(1).fillna(
+            self.__gps_points_gdf[gps_field.PLAIN_Y])
+        self.__gps_points_gdf[gps_field.X_DIFF] = self.__gps_points_gdf['next_x'] - self.__gps_points_gdf['pre_x']
+        self.__gps_points_gdf[gps_field.Y_DIFF] = self.__gps_points_gdf['next_y'] - self.__gps_points_gdf['pre_y']
+        del self.__gps_points_gdf['next_x'], self.__gps_points_gdf['next_y'], \
+            self.__gps_points_gdf['pre_x'], self.__gps_points_gdf['pre_y']
 
-        self.__gps_points_gdf[next_p_field] = self.__gps_points_gdf[geometry_field].shift(-1).fillna(
-            self.__gps_points_gdf[geometry_field])
-        self.__gps_points_gdf[pre_p_field] = self.__gps_points_gdf[geometry_field].shift(1).fillna(
-            self.__gps_points_gdf[geometry_field])
-
-        self.__gps_points_gdf['next_loc'] = self.__gps_points_gdf.apply(
-            lambda row: np.array([row[next_p_field].x, row[next_p_field].y]), axis=1)
-        self.__gps_points_gdf['pre_loc'] = self.__gps_points_gdf.apply(
-            lambda row: np.array([row[pre_p_field].x, row[pre_p_field].y]), axis=1)
-
-        # self.__gps_points_gdf['loc'] = self.__gps_points_gdf.apply(
-        #     lambda row: np.array([row[geometry_field].x, row[geometry_field].y]), axis=1)
-        # self.__gps_points_gdf[diff_vec] = self.__gps_points_gdf.apply(
-        #     lambda row: (row['next_loc'] - row['loc'] + row['loc'] - row['pre_loc']) / 2,
-        #     axis=1)
-
-        self.__gps_points_gdf[diff_vec] = (self.__gps_points_gdf['next_loc'] - self.__gps_points_gdf['pre_loc']) / 2
-
-        self.__gps_points_gdf.drop(
-            columns=[next_p_field, pre_p_field, 'next_loc', 'pre_loc'], axis=1, inplace=True)
+        self.__gps_points_gdf[gps_field.VEC_LEN] = np.sqrt(
+            self.__gps_points_gdf[gps_field.X_DIFF] ** 2 + self.__gps_points_gdf[gps_field.Y_DIFF] ** 2)
         self.done_diff_heading = True
 
     @property
     def gps_gdf(self) -> gpd.GeoDataFrame:
         return self.__gps_points_gdf.copy()
 
     @property
+    def gps_seq_time(self) -> dict:
+        if self.gps_seq_time_map:
+            return self.gps_seq_time_map
+        else:
+            self.gps_seq_time_map = {seq: t for seq, t in
+                                     zip(self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD],
+                                         self.__gps_points_gdf[gps_field.TIME_FIELD])}
+            return self.gps_seq_time_map
+
+    @property
+    def gps_seq_geo(self) -> dict:
+        if self.gps_seq_geo_map:
+            return self.gps_seq_geo_map
+        else:
+            self.gps_seq_geo_map = {seq: t for seq, t in
+                                    zip(self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD],
+                                        self.__gps_points_gdf[gps_field.GEOMETRY_FIELD])}
+            return self.gps_seq_geo_map
+
+    @property
     def crs(self):
         return self.__crs
 
     def get_gps_array_buffer(self, buffer: float = 200.0, dup_threshold: float = 10.0) -> Polygon or None:
         """输出gps路径的buffer范围面域"""
         gps_route_l = gpd.GeoSeries(LineString(self.__gps_points_gdf[gps_field.GEOMETRY_FIELD].to_list()))
-        simplify_gps_route_l = gps_route_l.remove_repeated_points(dup_threshold)
+        try:
+            simplify_gps_route_l = gps_route_l.remove_repeated_points(dup_threshold)
+        except:
+            simplify_gps_route_l = gps_route_l.simplify(dup_threshold / 10.0)
         gps_array_buffer = simplify_gps_route_l[0].buffer(buffer)
         return gps_array_buffer
 
     def generate_candidate_link(self, net: Net = None) -> tuple[pd.DataFrame, list[int]]:
         """
         计算GPS观测点的候选路段
         :param net:
@@ -316,15 +291,15 @@
         single_link_gdf.reset_index(inplace=True, drop=True)
         candidate_link = pd.DataFrame()
         remain_gps_list = []
         for i in [i for i in range(0, self.max_increment_times)]:
             now_buffer = self.buffer + i * self.increment_buffer
             print(rf'buffer: {now_buffer}m...')
 
-            gps_buffer_gdf['gps_buffer'] = gps_buffer_gdf[net_field.GEOMETRY_FIELD].apply(lambda p: p.buffer(now_buffer))
+            gps_buffer_gdf['gps_buffer'] = gps_buffer_gdf[net_field.GEOMETRY_FIELD].buffer(now_buffer)
             gps_buffer_gdf.set_geometry('gps_buffer', inplace=True, crs=gps_buffer_gdf.crs)
             join_df = gpd.sjoin(gps_buffer_gdf, single_link_gdf, how='left')
 
             _candidate_link = join_df[~join_df[net_field.SINGLE_LINK_ID_FIELD].isna()]
             candidate_link = pd.concat([candidate_link, _candidate_link])
             del _candidate_link
             remain_gps_list = list(join_df[join_df[net_field.SINGLE_LINK_ID_FIELD].isna()][gps_field.POINT_SEQ_FIELD].unique())
@@ -344,23 +319,21 @@
                                       on=net_field.SINGLE_LINK_ID_FIELD, how='left')
             candidate_link.reset_index(inplace=True, drop=True)
         return candidate_link, remain_gps_list
 
     def to_plane_prj(self) -> None:
         if self.__gps_points_gdf.crs.srs.upper() == self.plane_crs:
             self.__crs = self.plane_crs
-            pass
         else:
             self.__gps_points_gdf = self.__gps_points_gdf.to_crs(self.plane_crs)
             self.__crs = self.plane_crs
 
     def to_geo_prj(self) -> None:
         if self.__gps_points_gdf.crs.srs.upper() == self.geo_crs:
             self.__crs = self.geo_crs
-            pass
         else:
             self.__gps_points_gdf = self.__gps_points_gdf.to_crs(self.geo_crs)
             self.__crs = self.geo_crs
 
     def get_point(self, seq: int = 0):
         return self.__gps_points_gdf.at[seq, gps_field.TIME_FIELD], \
             self.__gps_points_gdf.at[seq, gps_field.GEOMETRY_FIELD]
@@ -368,55 +341,58 @@
     @property
     def source_gps(self) -> gpd.GeoDataFrame:
         if self.__source_gps_points_gdf is None:
             return self.__gps_points_gdf.copy()
         else:
             return self.__source_gps_points_gdf.copy()
 
-    def get_prj_inf(self, line: LineString, seq: int = 0) -> tuple[Point, float, float, float, np.ndarray]:
+    def get_prj_inf(self, line: LineString, seq: int = 0) -> tuple[Point, float, float, float, float, float]:
         """
         计算当前gps点实例在指定线对象上的投影信息
         :param line:
         :param seq:
         :return:
         """
-        (prj_p, prj_dis, route_dis, l_length, p_vec) = self._get_prj_inf(self.get_point(seq)[1], line)
-        return prj_p, prj_dis, route_dis, l_length, p_vec
+        (prj_p, prj_dis, route_dis, l_length, dx, dy) = self._get_prj_inf(self.get_point(seq)[1], line)
+        return prj_p, prj_dis, route_dis, l_length, dx, dy
 
     def delete_target_gps(self, target_seq_list: list[int]) -> None:
         self.__gps_points_gdf.drop(
             index=self.__gps_points_gdf[self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD].isin(target_seq_list)].index,
             inplace=True, axis=0)
 
     @staticmethod
-    def _get_prj_inf(gps_point: Point = None, line: LineString = None) -> tuple[Point, float, float, float, np.ndarray]:
+    def _get_prj_inf(gps_point: Point = None, line: LineString = None) -> tuple[Point, float, float, float, float, float]:
         """
         # 返回 (GPS投影点坐标, GPS点到投影点的直线距离, GPS投影点到line拓扑起点的路径距离, line的长度)
         :param gps_point:
         :param line:
         :return: (GPS投影点坐标, GPS点到投影点的直线距离, GPS投影点到line拓扑起点的路径距离, line的长度)
         """
-        prj_p, p_prj_l, prj_route_l, line_length, _, prj_vec = prj_inf(p=gps_point, line=line)
-        return prj_p, p_prj_l, prj_route_l, line_length, prj_vec
+        prj_p, p_prj_l, prj_route_l, line_length, _, dx, dy = prj_inf(p=gps_point, line=line)
+        return prj_p, p_prj_l, prj_route_l, line_length, dx, dy
 
     @property
     def gps_list_length(self) -> int:
         return len(self.__gps_points_gdf)
 
     @property
     def used_observation_seq_list(self) -> list[int]:
         return self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD].to_list()
 
     def del_dwell_points(self) -> None:
         # add field = dis_gap_field
         self.calc_adj_dis_gap()
+        del self.__gps_points_gdf[next_p_field]
         self.__gps_points_gdf['dwell_label'] = \
             (self.__gps_points_gdf[dis_gap_field] > self.dwell_l_length).astype(int)
+        del self.__gps_points_gdf[dis_gap_field]
         self.__gps_points_gdf.loc[len(self.__gps_points_gdf) - 1, 'dwell_label'] = 1
         self.__gps_points_gdf = self.del_consecutive_zero(df=self.__gps_points_gdf, col='dwell_label', n=self.dwell_n)
+        del self.__gps_points_gdf['dwell_label']
         try:
             self.__gps_points_gdf.drop(columns=[sub_group_field], axis=1, inplace=True)
         except KeyError:
             pass
 
     @staticmethod
     def del_consecutive_zero(df: pd.DataFrame or gpd.GeoDataFrame = None,
```

### Comparing `gotrackit-0.2.4/src/gotrackit/map/Link.py` & `gotrackit-0.2.5/src/gotrackit/map/Link.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
         self.__graph = nx.DiGraph()
         self.__ud_graph = nx.Graph()
         self.__one_out_degree_nodes = None
         self.__link_ft_mapping: dict[int, tuple[int, int]] = dict()
         self.__link_f_mapping: dict[int, int] = dict()
         self.__link_t_mapping: dict[int, int] = dict()
+        self.__link_geo_mapping: dict[int, LineString] = dict()
         self.done_link_vec = False
 
     def check(self):
         assert self.link_gdf.crs.srs.upper() == self.geo_crs, \
             rf'Link层数据必须为WGS84 - EPSG:4326, 实际输入: {self.link_gdf.crs.srs}'
         gap_set = {net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                    net_field.TO_NODE_FIELD, net_field.DIRECTION_FIELD, self.weight_field,
@@ -93,24 +94,26 @@
 
     def renew_length(self):
         self.link_gdf[length_field] = self.link_gdf[geometry_field].length
 
     def init_link_from_existing_single_link(self, single_link_gdf: gpd.GeoDataFrame = None,
                                             ft_link_mapping: dict = None,
                                             double_single_mapping: dict = None, link_ft_mapping: dict = None,
-                                            link_t_mapping: dict = None, link_f_mapping: dict = None):
+                                            link_t_mapping: dict = None, link_f_mapping: dict = None,
+                                            link_geo_mapping: dict = None):
         """通过给定的single_link_gdf初始化link, 用在子net的初始化上"""
         self.__single_link_gdf = single_link_gdf.copy()
 
         self.__double_single_mapping = double_single_mapping
         self.__ft_link_mapping = ft_link_mapping
         # single_link: (f, t)
         self.__link_ft_mapping = link_ft_mapping
         self.__link_t_mapping = link_t_mapping
         self.__link_f_mapping = link_f_mapping
+        self.__link_geo_mapping = link_geo_mapping
 
     def create_single_link(self, link_gdf: gpd.GeoDataFrame):
         """
         基于原来路网创建单向路网, 并且建立映射表
         :return:
         """
         link_gdf[net_field.DIRECTION_FIELD] = link_gdf[net_field.DIRECTION_FIELD].astype(int)
@@ -138,14 +141,17 @@
                                             self.__single_link_gdf[net_field.TO_NODE_FIELD])}
         self.__ft_link_mapping = {(f, t): single_link for f, t, single_link in
                                   zip(self.__single_link_gdf[net_field.FROM_NODE_FIELD],
                                       self.__single_link_gdf[net_field.TO_NODE_FIELD],
                                       self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD])}
         self.__link_f_mapping = {v: k[0] for k, v in self.__ft_link_mapping.items()}
         self.__link_t_mapping = {v: k[1] for k, v in self.__ft_link_mapping.items()}
+        # self.__link_geo_mapping = {single_link_id: geo for single_link_id, geo in
+        #                            zip(self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD],
+        #                                self.__single_link_gdf[net_field.GEOMETRY_FIELD])}
 
     def create_graph(self, weight_field: str = None):
         """
         创建有向图
         :return:
         """
         edge_list = [(f, t, {weight_field: l}) for f, t, l in
@@ -405,13 +411,17 @@
     def link_f_map(self) -> dict[int, int]:
         return self.__link_f_mapping
 
     @property
     def link_t_map(self) -> dict[int, int]:
         return self.__link_t_mapping
 
+    @property
+    def link_geo_map(self) -> dict[int, LineString]:
+        return self.__link_geo_mapping
+
     def vertex_degree(self, node: int = None) -> int:
         """无向图的节点度"""
         return self.__ud_graph.degree[node]
 
     def used_node(self) -> set[int]:
         return set(self.link_gdf[from_node_field]) | set(self.link_gdf[to_node_field])
```

### Comparing `gotrackit-0.2.4/src/gotrackit/map/Net.py` & `gotrackit-0.2.5/src/gotrackit/map/Net.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class Net(object):
 
     @function_time_cost
     def __init__(self, link_path: str = None, node_path: str = None, link_gdf: gpd.GeoDataFrame = None,
                  node_gdf: gpd.GeoDataFrame = None, weight_field: str = 'length', init_from_existing: bool = False,
                  is_check: bool = True, create_single: bool = True, search_method: str = 'dijkstra',
                  ft_link_mapping: dict = None, double_single_mapping: dict = None, link_ft_mapping: dict = None,
-                 link_t_mapping: dict = None, link_f_mapping: dict = None,
+                 link_t_mapping: dict = None, link_f_mapping: dict = None, link_geo_mapping: dict = None,
                  not_conn_cost: float = 999.0, cache_path: bool = True, cache_id: bool = True,
                  is_sub_net: bool = False, fmm_cache: bool = False, cache_cn: int = 2, cache_slice: int = None,
                  fmm_cache_fldr: str = None,
                  cache_name: str = 'cache', recalc_cache: bool = True,
                  cut_off: float = 1200.0, max_cut_off: float = 5000.0, delete_circle: bool = True):
         """
         创建Net类
@@ -63,14 +63,15 @@
         :param create_single: 是否在初始化的时候创建single层
         :param search_method: 路径搜索方法, 'dijkstra'
         :param init_from_existing: 是否直接从内存中的gdf创建single_link_gdf, 该参数用于类内部创建子net, 用户不用关心该参数, 使用默认值即可
         :param double_single_mapping:
         :param link_ft_mapping:
         :param link_f_mapping:
         :param link_t_mapping:
+        :param link_geo_mapping:
         :param ft_link_mapping:
         :param not_conn_cost: 不连通路径的阻抗(m), 默认999.0米
         :param is_sub_net: 是否是子网络, 默认False
         :param fmm_cache: 是否启用路径预存储, 默认False
         :param cache_cn: 使用几个核能进行路径预计算, 默认2
         :param fmm_cache_fldr: 存储路径预处理结果的文件目录, 默认./
         :param recalc_cache: 是否重新计算FMM路径缓存, 默认True
@@ -136,15 +137,16 @@
             if create_single:
                 # for sub net
                 self.__link.init_link_from_existing_single_link(single_link_gdf=link_gdf,
                                                                 double_single_mapping=double_single_mapping,
                                                                 ft_link_mapping=ft_link_mapping,
                                                                 link_ft_mapping=link_ft_mapping,
                                                                 link_t_mapping=link_t_mapping,
-                                                                link_f_mapping=link_f_mapping)
+                                                                link_f_mapping=link_f_mapping,
+                                                                link_geo_mapping=link_geo_mapping)
         if is_check:
             self.check()
 
     @property
     def planar_crs(self):
         return self.__planar_crs
 
@@ -321,14 +323,18 @@
         return self.__link.link_ft_map
 
     @property
     def link_t_map(self) -> dict[int, int]:
         return self.__link.link_t_map
 
     @property
+    def link_geo_map(self) -> dict[int, LineString]:
+        return self.__link.link_geo_map
+
+    @property
     def link_f_map(self) -> dict[int, int]:
         return self.__link.link_f_map
 
     @property
     def available_link_id(self) -> int:
         return self.__link.available_link_id
 
@@ -441,15 +447,15 @@
         if isinstance(p, Point):
             pass
         else:
             p = Point(p)
 
         # 获取打断点到target link的投影点信息
         target_link_geo = self.get_link_geo(target_link, _type='bilateral')
-        prj_p, p_prj_l, prj_route_l, target_l, split_link_geo_list, _ = prj_inf(p=p, line=target_link_geo)
+        prj_p, p_prj_l, prj_route_l, target_l, split_link_geo_list, _, _ = prj_inf(p=p, line=target_link_geo)
 
         if (target_l - prj_route_l) <= omitted_length_threshold:
             # this means that we should merge the to_node and p
             return False, Point(), [], 'tail_beyond'
         elif prj_route_l <= omitted_length_threshold:
             # this means that we should merge the from_node and p
             return False, Point(), [], 'head_beyond'
@@ -665,14 +671,25 @@
             columns={net_field.FROM_NODE_FIELD: o_node_field, net_field.TO_NODE_FIELD: d_node_field,
                      self.weight_field: cost_field})
         _[path_field] = _.apply(lambda row: [int(row[o_node_field]), int(row[d_node_field])], axis=1)
         done_stp_cost_df = pd.concat([_, done_stp_cost_df])
         del _
         done_stp_cost_df.drop_duplicates(subset=[o_node_field, d_node_field], keep='first', inplace=True)
         done_stp_cost_df.reset_index(inplace=True, drop=True)
+        done_stp_cost_df['2nd_node'], done_stp_cost_df['-2nd_node'] = -1, -1
+        normal_path_idx = done_stp_cost_df[cost_field] > 0
+        try:
+            done_stp_cost_df.loc[normal_path_idx, '2nd_node'] = done_stp_cost_df.loc[normal_path_idx, :][
+                path_field].apply(
+                lambda x: x[1])
+            done_stp_cost_df.loc[normal_path_idx, '-2nd_node'] = done_stp_cost_df.loc[normal_path_idx, :][
+                path_field].apply(
+                lambda x: x[-2])
+        except:
+            pass
         with open(os.path.join(self.fmm_cache_fldr, rf'{self.cache_name}_path_cache'), 'wb') as f:
             pickle.dump(done_stp_cost_df, f)
         self.set_path_cache(done_stp_cost_df)
 
     @staticmethod
     def slice_save(done_stp_cache: dict = None, done_cost_cache: dict = None, n: int = 3) -> pd.DataFrame:
         temp_stp_list = [{} for i in range(n)]
@@ -719,56 +736,70 @@
             [net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD, self.weight_field,
              'path']].copy()
 
     def cache_prj_info(self):
         if self.fmm_cache_fldr is None:
             self.fmm_cache_fldr = r'./'
         if not self.recalc_cache:
-            try:
-                with open(os.path.join(self.fmm_cache_fldr, rf'{self.cache_name}_prj'), 'rb') as f:
-                    cache_prj_inf = pickle.load(f)
-                self.set_prj_cache(cache_prj_inf)
-                return None
-            except Exception as e:
-                print(repr(e))
+            with open(os.path.join(self.fmm_cache_fldr, rf'{self.cache_name}_prj'), 'rb') as f:
+                cache_prj_inf = pickle.load(f)
+
+            if 1 in cache_prj_inf.keys():
+                if net_field.X_DIFF not in cache_prj_inf[1].columns:
+                    raise ValueError('检测到是0.2.4版本之前的缓存数据, 请在>=0.2.5版本下重新计算路径缓存')
+            if 2 in cache_prj_inf.keys():
+                if net_field.X_DIFF not in cache_prj_inf[2].columns:
+                    raise ValueError('检测到是0.2.4版本之前的缓存数据, 请在>=0.2.5版本下重新计算路径缓存')
+            self.set_prj_cache(cache_prj_inf)
+
+            return None
 
         single_link_gdf = self.__link.get_link_data()
         single_link_gdf = single_link_gdf[
             [net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD, net_field.GEOMETRY_FIELD, net_field.LENGTH_FIELD]].copy()
+
         cache_prj_gdf = self.split_segment(single_link_gdf)
-        cache_prj_gdf[['f_loc', 't_loc']] = cache_prj_gdf.apply(lambda row: list(row['geometry'].coords), axis=1,
-                                                                result_type='expand')
-        cache_prj_gdf[net_field.LINK_VEC_FIELD] = cache_prj_gdf.apply(
-            lambda row: np.array(row['t_loc']) - np.array(row['f_loc']), axis=1)
-        cache_prj_gdf.drop(columns=['f_loc', 't_loc', net_field.GEOMETRY_FIELD], axis=1, inplace=True)
+
+        # cache_prj_gdf.drop(columns=['f_loc', 't_loc', net_field.GEOMETRY_FIELD], axis=1, inplace=True)
         cache_prj_gdf[net_field.SEG_COUNT] = \
             cache_prj_gdf.groupby([net_field.FROM_NODE_FIELD,
-                                   net_field.TO_NODE_FIELD])[net_field.LINK_VEC_FIELD].transform('count')
+                                   net_field.TO_NODE_FIELD])[net_field.X_DIFF].transform('count')
         cache_prj_inf = {1: cache_prj_gdf[cache_prj_gdf[net_field.SEG_COUNT] == 1].copy().reset_index(drop=True),
                          2: cache_prj_gdf[cache_prj_gdf[net_field.SEG_COUNT] > 1].copy().reset_index(drop=True)}
         del cache_prj_gdf
         self.set_prj_cache(cache_prj_inf)
         with open(os.path.join(self.fmm_cache_fldr, rf'{self.cache_name}_prj'), 'wb') as f:
             pickle.dump(cache_prj_inf, f)
 
     @staticmethod
-    def split_segment(path_gdf: gpd.GeoDataFrame = None) -> gpd.GeoDataFrame:
+    def split_segment(path_gdf: gpd.GeoDataFrame = None) -> gpd.GeoDataFrame or pd.DataFrame:
         """
         拆解轨迹坐标, 并且粗去重(按照路段的起终点坐标)
         :param path_gdf: gpd.GeoDataFrame(), 必需参数, 必须字段: [geometry], crs要求EPSG:4326
         :return: gpd.GeoDataFrame(),
         """
         origin_crs = path_gdf.crs.srs
         path_gdf['point_list'] = path_gdf[net_field.GEOMETRY_FIELD].apply(lambda x: list(x.coords))
         path_gdf['line_list'] = path_gdf['point_list'].apply(
-            lambda x: [LineString((x[i], x[i + 1])) for i in range(0, len(x) - 1)])
+            lambda x: [(x[i], x[i + 1]) for i in range(0, len(x) - 1)])
         path_gdf['topo_seq'] = path_gdf['line_list'].apply(lambda x: [i for i in range(len(x))])
         path_gdf.drop(columns=[net_field.GEOMETRY_FIELD, 'point_list'], axis=1, inplace=True)
         path_gdf = pd.DataFrame(path_gdf)
         path_gdf = path_gdf.explode(column=['line_list', 'topo_seq'], ignore_index=True)
-        path_gdf.rename(columns={'line_list': net_field.GEOMETRY_FIELD}, inplace=True)
-        path_gdf = gpd.GeoDataFrame(path_gdf, crs=origin_crs, geometry=net_field.GEOMETRY_FIELD)
-        path_gdf['__l__'] = path_gdf[net_field.GEOMETRY_FIELD].length
+        path_gdf.rename(columns={'line_list': 'ft-loc'}, inplace=True)
+        # path_gdf = gpd.GeoDataFrame(path_gdf, crs=origin_crs, geometry=net_field.GEOMETRY_FIELD)
+        path_gdf['f_x'] = path_gdf['ft-loc'].apply(lambda x: x[0][0])
+        path_gdf['f_y'] = path_gdf['ft-loc'].apply(lambda x: x[0][1])
+        path_gdf['t_x'] = path_gdf['ft-loc'].apply(lambda x: x[1][0])
+        path_gdf['t_y'] = path_gdf['ft-loc'].apply(lambda x: x[1][1])
+        del path_gdf['ft-loc'], path_gdf[net_field.LENGTH_FIELD]
+        path_gdf[net_field.X_DIFF] = path_gdf['t_x'] - path_gdf['f_x']
+        path_gdf[net_field.Y_DIFF] = path_gdf['t_y'] - path_gdf['f_y']
+        del path_gdf['f_x'], path_gdf['f_y'], path_gdf['t_x'], path_gdf['t_y']
+        path_gdf[net_field.VEC_LEN] = np.sqrt(path_gdf[net_field.X_DIFF] ** 2 + path_gdf[net_field.Y_DIFF] ** 2)
+        # path_gdf['__l__'] = path_gdf[net_field.GEOMETRY_FIELD].length
         path_gdf[net_field.SEG_ACCU_LENGTH] = \
-            path_gdf.groupby([net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD])[['__l__']].cumsum()
-        del path_gdf['__l__']
+            path_gdf.groupby([net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD])[[net_field.VEC_LEN]].cumsum()
+        path_gdf['topo_seq'] = path_gdf['topo_seq'].astype(int)
+        # del path_gdf['__l__']
         return path_gdf
+
```

### Comparing `gotrackit-0.2.4/src/gotrackit/map/Node.py` & `gotrackit-0.2.5/src/gotrackit/map/Node.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/model/Markov.py` & `gotrackit-0.2.5/src/gotrackit/model/Markov.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 # @Time    : 2023/12/9 8:29
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 """Markov Model Class"""
 
 import os.path
-import time
 import warnings
 import numpy as np
 import pandas as pd
 import networkx as nx
 import geopandas as gpd
 from ..map.Net import Net
+from .Para import ParaGrid
 from datetime import timedelta
 from ..solver.Viterbi import Viterbi
 from ..gps.LocGps import GpsPointsGdf
 from ..tools.geo_process import prj_inf
 from ..WrapsFunc import function_time_cost
 from shapely.geometry import Point, LineString
 from ..GlobalVal import NetField, GpsField, MarkovField
-from ..tools.geo_process import n_equal_points, hmm_vector_angle
-
+from ..tools.geo_process import n_equal_points, vec_angle
 
 gps_field = GpsField()
 net_field = NetField()
 markov_field = MarkovField()
 
 from_link_f, to_link_f = markov_field.FROM_STATE, markov_field.TO_STATE
 from_link_n_f, to_link_n_f = markov_field.FROM_STATE_N, markov_field.TO_STATE_N
@@ -37,27 +36,29 @@
 
 
 class HiddenMarkov(object):
     """隐马尔可夫模型类"""
 
     def __init__(self, net: Net, gps_points: GpsPointsGdf, beta: float = 30.1, gps_sigma: float = 20.0,
                  not_conn_cost: float = 999.0, use_heading_inf: bool = True, heading_para_array: np.ndarray = None,
-                 dis_para: float = 0.1, top_k: int = 25, omitted_l: float = 6.0):
+                 dis_para: float = 0.1, top_k: int = 25, omitted_l: float = 6.0, para_grid: ParaGrid = None,
+                 use_para_grid: bool = False):
         self.gps_points = gps_points
         self.net = net
         # (gps_seq, single_link_id): (prj_p, prj_dis, route_dis)
         self.__done_prj_dict: dict[tuple[int, int]: tuple[Point, float, float, float, np.ndarray]] = dict()
         self.__done_prj_df: gpd.GeoDataFrame or pd.DataFrame = None
         self.__adj_seq_path_dict: dict[tuple[int, int], list[int, int]] = dict()
         self.__ft_transition_dict = dict()
         self.__ft_mapping_dict = dict()
         self.__ft_idx_map = pd.DataFrame()
         self.beta = beta
         self.gps_sigma = gps_sigma
         self.__emission_mat_dict = dict()
+        self.__seq2seq_len_dict = dict()
         self.__solver = None
         self.index_state_list = None
         self.gps_match_res_gdf = None
         # {(from_seq, to_seq): pd.DataFrame()}
         self.__s2s_route_l = pd.DataFrame()
         self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf, self.__may_error = None, None, None, None
         self.path_cost_df = pd.DataFrame()
@@ -71,52 +72,161 @@
         self.angle_slice = 180 / len(self.heading_para_array)
         self.dis_para = dis_para
         self.warn_info = {'from_ft': [], 'to_ft': []}
         self.format_warn_info = pd.DataFrame()
         self.top_k = top_k
         self.omitted_l = omitted_l
         self.gps_candidate_link = None
+        self.__transition_df = pd.DataFrame()
+        self.use_para_grid = use_para_grid
+        self.para_grid = para_grid
 
-    @function_time_cost
-    def generate_markov_para(self, add_single_ft: list[bool] = None) -> bool:
+    def init_warn_info(self):
+        self.warn_info = {'from_ft': [], 'to_ft': []}
+
+    def hmm_execute(self, add_single_ft: list[bool] = None) -> tuple[bool, pd.DataFrame]:
+        try:
+            is_success = self.__generate_st(add_single_ft=add_single_ft)
+        except Exception as e:
+            is_success = False
+            print(rf'构造矩阵结构出错:{repr(e)}')
+        if not is_success:
+            return False, pd.DataFrame()
+
+        try:
+            self.calc_transition_mat(beta=self.beta, dis_para=self.dis_para)
+        except Exception as e:
+            print(rf'计算转移矩阵出错:{repr(e)}')
+            return False, pd.DataFrame()
+
+        try:
+            self.__calc_emission(use_heading_inf=self.use_heading_inf, omitted_l=self.omitted_l,
+                                 gps_sigma=self.gps_sigma)
+        except Exception as e:
+            print(rf'计算发射矩阵出错:{repr(e)}')
+            return False, pd.DataFrame()
 
-        is_success = self.__generate_transition_mat_alpha_multi(add_single_ft)
-        if is_success:
-            self.__generate_emission_mat()
-        return is_success
+        try:
+            self.solve()
+        except Exception as e:
+            print(rf'回溯模型出错:{repr(e)}')
+            return False, pd.DataFrame()
 
-    def __generate_emission_mat(self):
+        try:
+            match_res = self.acquire_res()
+        except Exception as e:
+            print(rf'获取匹配结果出错:{repr(e)}')
+            return False, pd.DataFrame()
+        self.formatting_warn_info()
+        return True, match_res
 
+    def hmm_para_grid_execute(self, add_single_ft: list[bool] = None, agent_id=None) -> tuple[bool, pd.DataFrame]:
+        warnings.filterwarnings('ignore')
+        try:
+            is_success = self.__generate_st(add_single_ft=add_single_ft)
+        except Exception as e:
+            is_success = False
+            print(rf'构造矩阵结构出错:{repr(e)}')
+
+        if not is_success:
+            return False, pd.DataFrame()
+
+        match_res = pd.DataFrame()
+        transit_res = self.para_grid.transit_res
+        emission_res = self.para_grid.emission_res
+        all_num = len(transit_res) * len(emission_res)
+        c = 0
+        for k1 in transit_res.keys():
+            if not transit_res[k1]['res']:
+                try:
+                    beta = transit_res[k1]['parameter']['beta']
+                    self.calc_transition_mat(beta=beta, dis_para=self.dis_para)
+                    transit_res[k1]['res'] = self.__ft_transition_dict
+                except Exception as e:
+                    print(rf'计算转移矩阵出错:{repr(e)}')
+                    return False, pd.DataFrame()
+            else:
+                self.__ft_transition_dict = transit_res[k1]['res']
+
+            for k2 in emission_res.keys():
+                if not emission_res[k2]['res']:
+                    try:
+                        omitted_l, use_heading_inf, gps_sigma = \
+                            emission_res[k2]['parameter']['omitted_l'],\
+                            emission_res[k2]['parameter']['use_heading_inf'], \
+                            emission_res[k2]['parameter']['gps_sigma']
+                        self.__calc_emission(use_heading_inf=use_heading_inf, omitted_l=omitted_l,
+                                             gps_sigma=gps_sigma)
+                        emission_res[k2]['res'] = self.__emission_mat_dict
+                    except Exception as e:
+                        print(rf'计算发射矩阵出错:{repr(e)}')
+                        return False, pd.DataFrame()
+                else:
+                    self.__emission_mat_dict = emission_res[k2]['res']
+
+                try:
+                    self.solve()
+                except Exception as e:
+                    print(rf'回溯模型出错:{repr(e)}')
+                    return False, pd.DataFrame()
+
+                try:
+                    match_res = self.acquire_res()
+                except Exception as e:
+                    print(rf'获取匹配结果出错:{repr(e)}')
+                    return False, pd.DataFrame()
+
+                self.formatting_warn_info()
+                self.para_grid.update_res({'agent_id': agent_id, 'beta': transit_res[k1]['parameter']['beta'],
+                                           'gps_sigma': emission_res[k2]['parameter']['gps_sigma'],
+                                           'use_heading_inf': emission_res[k2]['parameter'][
+                                               'use_heading_inf'],
+                                           'omitted_l': emission_res[k2]['parameter']['omitted_l'],
+                                           'warn_num': len(self.format_warn_info)})
+                print(f'para - {c}:', transit_res[k1]['parameter'], emission_res[k2]['parameter'],
+                      rf'warning num: {len(self.format_warn_info)}')
+                if self.format_warn_info.empty:
+                    return True, match_res
+                c += 1
+                if c < all_num:
+                    self.init_warn_info()
+
+        return True, match_res
+
+    def __calc_emission(self, use_heading_inf: bool = True, omitted_l: float = 6.0, gps_sigma: float = 30.0):
         # 计算每个观测点的生成概率, 这是在计算状态转移概率之后, 已经将关联不到的GPS点删除了
-        # 这里的向量是候选路段的投影点的方向向量
-        emission_p_df = self.__done_prj_df.copy()
-        emission_p_df.rename(columns={'p_vec': net_field.LINK_VEC_FIELD}, inplace=True)
-        if self.use_heading_inf:
-            self.gps_points.calc_diff_heading()
-            emission_p_df = pd.merge(emission_p_df, self.gps_points.gps_gdf[[gps_field.POINT_SEQ_FIELD,
-                                                                             gps_field.DIFF_VEC]], how='left',
-                                     on=gps_field.POINT_SEQ_FIELD)
-            emission_p_df[markov_field.HEADING_GAP] = \
-                [hmm_vector_angle(gps_diff_vec=diff_vec,
-                                  link_dir_vec=link_vec,
-                                  omitted_l=self.omitted_l) for diff_vec, link_vec in
-                 zip(emission_p_df[gps_field.DIFF_VEC], emission_p_df[net_field.LINK_VEC_FIELD])]
+        if use_heading_inf:
+            if gps_field.X_DIFF not in self.__done_prj_df.columns:
+                self.gps_points.calc_diff_heading()
+                self.__done_prj_df = pd.merge(self.__done_prj_df, self.gps_points.gps_gdf[[gps_field.POINT_SEQ_FIELD,
+                                                                                           gps_field.X_DIFF,
+                                                                                           gps_field.Y_DIFF,
+                                                                                           gps_field.VEC_LEN]],
+                                              how='left',
+                                              on=gps_field.POINT_SEQ_FIELD)
+
+                vec_angle(df=self.__done_prj_df)
+                if markov_field.HEADING_GAP in self.__done_prj_df.columns:
+                    del self.__done_prj_df[markov_field.HEADING_GAP]
+                self.__done_prj_df.rename(columns={'theta': markov_field.HEADING_GAP}, inplace=True)
+
+            self.__done_prj_df.loc[self.__done_prj_df[gps_field.VEC_LEN] <= omitted_l, markov_field.HEADING_GAP] = 0
+
         else:
-            emission_p_df[markov_field.HEADING_GAP] = 0
-        emission_p_df[markov_field.HEADING_GAP] = emission_p_df[markov_field.HEADING_GAP].astype(object)
-        emission_p_df[markov_field.PRJ_L] = emission_p_df[markov_field.PRJ_L].astype(object)
-        emission_p_df.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD],
-                                  ascending=[True, True], inplace=True)
-        emission_p_df = emission_p_df.groupby([gps_field.POINT_SEQ_FIELD]).agg(
+            self.__done_prj_df[markov_field.HEADING_GAP] = 0
+
+        self.__done_prj_df[markov_field.HEADING_GAP] = self.__done_prj_df[markov_field.HEADING_GAP].astype(object)
+        self.__done_prj_df[markov_field.PRJ_L] = self.__done_prj_df[markov_field.PRJ_L].astype(object)
+
+        emission_p_df = self.__done_prj_df.groupby(gps_field.POINT_SEQ_FIELD).agg(
             {markov_field.PRJ_L: np.array, markov_field.HEADING_GAP: np.array}).reset_index(
             drop=False)
-
         self.__emission_mat_dict = {
             int(row[gps_field.POINT_SEQ_FIELD]): self.emission_probability(dis=row[markov_field.PRJ_L],
-                                                                           sigma=self.gps_sigma,
+                                                                           sigma=gps_sigma,
                                                                            heading_gap=row[markov_field.HEADING_GAP])
             for _, row in
             emission_p_df.iterrows()}
 
     def __generate_candidates(self) -> list[int]:
         # 初步依据gps点buffer得到候选路段, 关联不到的GPS点删除掉
         # seq, geometry, single_link_id, from_node, to_node, dir, length
@@ -158,15 +268,17 @@
         preliminary_candidate_link = preliminary_candidate_link.groupby(gps_field.POINT_SEQ_FIELD).head(
             top_k).reset_index(drop=True)
         if not using_cache:
             prj_info_list = [prj_inf(p=geo, line=single_link_geo) for geo, single_link_geo in
                              zip(preliminary_candidate_link[gps_field.GEOMETRY_FIELD],
                                  preliminary_candidate_link['single_link_geo'])]
             prj_df = pd.DataFrame(prj_info_list,
-                                  columns=['prj_p', 'prj_dis', 'route_dis', 'l_length', 'split_line', 'p_vec'])
+                                  columns=['prj_p', 'prj_dis', 'route_dis', 'l_length', 'split_line',
+                                           net_field.X_DIFF, net_field.Y_DIFF])
+            prj_df[net_field.VEC_LEN] = np.sqrt(prj_df[net_field.X_DIFF] ** 2 + prj_df[net_field.Y_DIFF] ** 2)
             del prj_df['split_line']
             del preliminary_candidate_link['quick_stl']
             preliminary_candidate_link = pd.merge(preliminary_candidate_link, prj_df, left_index=True, right_index=True)
             k_candidate_link = preliminary_candidate_link
             del prj_df
             return k_candidate_link
         else:
@@ -185,19 +297,21 @@
             cache_prj_gdf_a = cache_prj_inf[1]
             preliminary_candidate_link = pd.merge(preliminary_candidate_link, cache_prj_gdf_a, how='left',
                                                   on=[net_field.FROM_NODE_FIELD,
                                                       net_field.TO_NODE_FIELD])
             a_info = preliminary_candidate_link[~preliminary_candidate_link[net_field.SEG_ACCU_LENGTH].isna()].copy()
             preliminary_candidate_link = preliminary_candidate_link[
                 preliminary_candidate_link[net_field.SEG_ACCU_LENGTH].isna()].copy()
-            preliminary_candidate_link.drop(columns=[net_field.SEG_ACCU_LENGTH, 'topo_seq', net_field.LENGTH_FIELD,
-                                                     'dir_vec', net_field.SEG_COUNT], axis=1, inplace=True)
+            preliminary_candidate_link.drop(columns=[net_field.SEG_ACCU_LENGTH, 'topo_seq',
+                                                     net_field.X_DIFF, net_field.Y_DIFF, net_field.VEC_LEN,
+                                                     net_field.SEG_COUNT], axis=1,
+                                            inplace=True)
             del a_info[net_field.SEG_ACCU_LENGTH], a_info[net_field.SEG_COUNT], a_info['topo_seq']
             if preliminary_candidate_link.empty:
-                a_info.rename(columns={'quick_stl': 'prj_dis', 'dir_vec': 'p_vec'}, inplace=True)
+                a_info.rename(columns={'quick_stl': 'prj_dis'}, inplace=True)
                 return a_info
         else:
             a_info = pd.DataFrame()
 
         if 2 in cache_prj_inf.keys():
             cache_prj_gdf_b = cache_prj_inf[2]
             b_info = pd.merge(preliminary_candidate_link, cache_prj_gdf_b, how='inner', on=[net_field.FROM_NODE_FIELD,
@@ -220,15 +334,15 @@
 
                 d_info = d_info.groupby(
                     [gps_field.POINT_SEQ_FIELD, net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD]).head(n=1)
                 del d_info['ck'], d_info['topo_seq'], d_info['ratio'], d_info[net_field.SEG_ACCU_LENGTH]
 
             preliminary_candidate_link = pd.concat([a_info, c_info, d_info])
             preliminary_candidate_link.reset_index(inplace=True, drop=True)
-            preliminary_candidate_link.rename(columns={'quick_stl': 'prj_dis', 'dir_vec': 'p_vec'}, inplace=True)
+            preliminary_candidate_link.rename(columns={'quick_stl': 'prj_dis'}, inplace=True)
             return preliminary_candidate_link
         else:
             return a_info
 
     def solve(self, use_lop_p: bool = True):
         """
         :param use_lop_p: 是否使用对数概率, 避免浮点数精度下溢
@@ -238,79 +352,91 @@
         # 使用viterbi模型求解
         self.__solver = Viterbi(observation_list=self.gps_points.used_observation_seq_list,
                                 o_mat_dict=self.__emission_mat_dict,
                                 t_mat_dict=self.__ft_transition_dict, use_log_p=use_lop_p)
         self.__solver.init_model()
         self.index_state_list = self.__solver.iter_model()
 
-    def __generate_transition_mat_alpha_multi(self, add_single_ft: list[bool] = None) -> bool:
+    @function_time_cost
+    def __generate_st(self, add_single_ft: list[bool] = None) -> bool:
         # 计算 初步候选, 经过这一步, 实际匹配用到的GPS点已经完全确定
         # 得到self.gps_candidate_link
         seq_list = self.__generate_candidates()
         if not seq_list:
             return False
 
         # 已经删除了关联不到任何路段的GPS点, 基于新的序列计算相邻GPS点距离
         # gps_field.POINT_SEQ_FIELD, gps_field.NEXT_SEQ, gps_field.ADJ_DIS
-        gps_pre_next_dis_df = self.gps_points.calc_pre_next_dis()
-        gps_pre_next_dis_df.rename(columns={gps_field.POINT_SEQ_FIELD: gps_field.FROM_GPS_SEQ,
-                                            gps_field.NEXT_SEQ: gps_field.TO_GPS_SEQ}, inplace=True)
-
+        self.gps_points.calc_pre_next_dis()
         # 抽取单向信息
         single_link_ft_df = self.net.single_link_ft_cost()
         single_link_ft_df.reset_index(inplace=True, drop=True)
         g = self.net.graph
         is_sub_net = self.net.is_sub_net
         fmm_cache = self.net.fmm_cache
-        cut_off, max_cut_off = self.net.cut_off, self.net.max_cut_off
+        cut_off = self.net.cut_off
         # print(cut_off)
         if is_sub_net:
             if fmm_cache:
                 done_stp_cost_df = self.net.get_path_cache()
                 cache_prj_info = self.net.get_prj_cache()
             else:
                 done_stp_cost_df = pd.DataFrame()
                 cache_prj_info = dict()
         else:
             done_stp_cost_df = self.net.get_path_cache()
             cache_prj_info = self.net.get_prj_cache()
         single_link_f_map, single_link_t_map = self.net.link_f_map, self.net.link_t_map
-        adj_seq_path_dict, ft_transition_dict, ft_idx_map, s2s_route_l, prj_done_df, \
-            done_stp_cost_df = \
-            self.generate_transition_mat_beta(single_link_ft_df, self.gps_candidate_link,
-                                              gps_pre_next_dis_df, g, self.net.search_method,
-                                              self.net.weight_field, self.net.cache_path, self.net.not_conn_cost,
-                                              done_stp_cost_df, is_sub_net, fmm_cache,
-                                              cut_off, max_cut_off, cache_prj_info, add_single_ft, single_link_f_map,
-                                              single_link_t_map)
+        adj_seq_path_dict, ft_idx_map, s2s_route_l, prj_done_df, done_stp_cost_df, seq_len_dict, transition_df = \
+            self.generate_transition_st(single_link_ft_df, self.gps_candidate_link,
+                                        self.gps_points.gps_adj_dis_map, g, self.net.search_method,
+                                        self.net.weight_field, self.net.cache_path, self.net.not_conn_cost,
+                                        done_stp_cost_df, is_sub_net, fmm_cache,
+                                        cut_off, cache_prj_info, add_single_ft, single_link_f_map,
+                                        single_link_t_map)
         # print(len(done_stp_cost_df))
         ft_idx_map.reset_index(inplace=True, drop=True)
         s2s_route_l.reset_index(inplace=True, drop=True)
         self.__adj_seq_path_dict = adj_seq_path_dict
         self.__ft_idx_map = ft_idx_map
-        self.__ft_transition_dict = ft_transition_dict
         self.__s2s_route_l = s2s_route_l
         self.__done_prj_df = prj_done_df
+        self.__done_prj_df.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD],
+                                       ascending=[True, True], inplace=True)
+        self.__seq2seq_len_dict = seq_len_dict
+        self.__transition_df = transition_df
 
         if not is_sub_net and not fmm_cache:
             self.net.set_path_cache(stp_cost_df=done_stp_cost_df)
         return True
 
-    def generate_transition_mat_beta(self, single_link_ft_df: pd.DataFrame = None,
-                                     pre_seq_candidate: pd.DataFrame = None,
-                                     gps_pre_next_dis_df: pd.DataFrame = None,
-                                     g: nx.DiGraph = None,
-                                     method: str = None, weight_field: str = 'length',
-                                     cache_path: bool = True, not_conn_cost: float = 999.0,
-                                     done_stp_cost_df: pd.DataFrame = None,
-                                     is_sub_net: bool = True, fmm_cache: bool = False, cut_off: float = 600.0,
-                                     max_cut_off: float = 2000.0, cache_prj_inf: dict = None,
-                                     add_single_ft: list[bool] = None, link_f_map: dict = None,
-                                     link_t_map: dict = None) -> \
-            tuple[dict, dict, pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
+    def calc_transition_mat(self, beta: float = 6.0, dis_para: float = 0.1):
+        seq_len_dict = self.__seq2seq_len_dict
+        self.__transition_df['trans_values'] = \
+            self.transition_probability(beta, self.__transition_df[markov_field.DIS_GAP].values, dis_para)
+
+        ft_transition_dict = {f_gps_seq: df['trans_values'].values.reshape(seq_len_dict[f_gps_seq],
+                                                                           int(len(df) / seq_len_dict[f_gps_seq])) for
+                              (f_gps_seq, t_gps_seq), df in
+                              self.__transition_df.groupby([gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ])}
+
+        self.__ft_transition_dict = ft_transition_dict
+
+    def generate_transition_st(self, single_link_ft_df: pd.DataFrame = None,
+                               pre_seq_candidate: pd.DataFrame = None,
+                               gps_adj_dis_map: dict = None,
+                               g: nx.DiGraph = None,
+                               method: str = None, weight_field: str = 'length',
+                               cache_path: bool = True, not_conn_cost: float = 999.0,
+                               done_stp_cost_df: pd.DataFrame = None,
+                               is_sub_net: bool = True, fmm_cache: bool = False, cut_off: float = 600.0,
+                               cache_prj_inf: dict = None,
+                               add_single_ft: list[bool] = None, link_f_map: dict = None,
+                               link_t_map: dict = None) -> \
+            tuple[dict, pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame, dict, pd.DataFrame]:
         # K候选
         seq_k_candidate_info = \
             self.filter_k_candidates(preliminary_candidate_link=pre_seq_candidate, using_cache=fmm_cache,
                                      top_k=self.top_k, cache_prj_inf=cache_prj_inf)
         # print(rf'{len(seq_k_candidate_info)}个候选路段...')
         seq_k_candidate_info.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD], inplace=True)
         now_source_node = set(seq_k_candidate_info[net_field.FROM_NODE_FIELD])
@@ -347,18 +473,27 @@
             ignore_index=True)
         from_state['from_route_dis'] = from_state['from_route_dis'].astype(float)
         to_state['to_route_dis'] = to_state['to_route_dis'].astype(float)
 
         transition_df = pd.merge(from_state, to_state, on='g', how='outer')
         transition_df.reset_index(inplace=True, drop=True)
         # print(rf'{len(transition_df)}次状态转移...')
-        transition_df['from_link_f'] = transition_df[markov_field.FROM_STATE].map(link_f_map)
-        transition_df['from_link_t'] = transition_df[markov_field.FROM_STATE].map(link_t_map)
-        transition_df['to_link_f'] = transition_df[markov_field.TO_STATE].map(link_f_map)
-        transition_df['to_link_t'] = transition_df[markov_field.TO_STATE].map(link_t_map)
+        if len(transition_df) >= 30000:
+            now_target_node = set(seq_k_candidate_info[net_field.TO_NODE_FIELD])
+            link_t_map = {k: v for k, v in link_t_map.items() if v in now_target_node}
+            link_f_map = {k: v for k, v in link_f_map.items() if v in now_source_node}
+            transition_df['from_link_f'] = transition_df[markov_field.FROM_STATE].map(link_f_map)
+            transition_df['from_link_t'] = transition_df[markov_field.FROM_STATE].map(link_t_map)
+            transition_df['to_link_f'] = transition_df[markov_field.TO_STATE].map(link_f_map)
+            transition_df['to_link_t'] = transition_df[markov_field.TO_STATE].map(link_t_map)
+        else:
+            transition_df['from_link_f'] = transition_df[markov_field.FROM_STATE].apply(lambda x: link_f_map[x])
+            transition_df['from_link_t'] = transition_df[markov_field.FROM_STATE].apply(lambda x: link_t_map[x])
+            transition_df['to_link_f'] = transition_df[markov_field.TO_STATE].apply(lambda x: link_f_map[x])
+            transition_df['to_link_t'] = transition_df[markov_field.TO_STATE].apply(lambda x: link_t_map[x])
 
         # now_source_node = set(transition_df['from_link_f'])
         if not fmm_cache:
             # 先计算所有要计算的path
             if o_node_field in done_stp_cost_df.columns:
                 already_cache_node = set(done_stp_cost_df[o_node_field])
             else:
@@ -373,14 +508,27 @@
                                                        single_link_ft_path_df=single_link_ft_df,
                                                        weight_field=weight_field, method=method, g=g,
                                                        add_single_ft=add_single_ft)
         del single_link_ft_df, g
 
         _done_stp_cost_df = done_stp_cost_df[done_stp_cost_df[o_node_field].isin(now_source_node) &
                                              done_stp_cost_df[d_node_field].isin(now_source_node)].copy()
+        if not fmm_cache:
+            _done_stp_cost_df['2nd_node'] = -1
+            _done_stp_cost_df['-2nd_node'] = -1
+            normal_path_idx = _done_stp_cost_df[cost_field] > 0
+            try:
+                _done_stp_cost_df.loc[normal_path_idx, '2nd_node'] = _done_stp_cost_df.loc[normal_path_idx, :][
+                    path_field].apply(
+                    lambda x: x[1])
+                _done_stp_cost_df.loc[normal_path_idx, '-2nd_node'] = _done_stp_cost_df.loc[normal_path_idx, :][
+                    path_field].apply(
+                    lambda x: x[-2])
+            except:
+                pass
         transition_df = pd.merge(transition_df, _done_stp_cost_df, left_on=['from_link_f', 'to_link_f'],
                                  right_on=[o_node_field, d_node_field], how='left')
         del _done_stp_cost_df
         del transition_df[o_node_field], transition_df[d_node_field]
         # sub_net do not share path within different agents
         if is_sub_net or fmm_cache or not cache_path:
             del done_stp_cost_df
@@ -393,57 +541,34 @@
         normal_path_idx_a = transition_df[cost_field] > 0
         _ = transition_df[normal_path_idx_a]
         adj_seq_path_dict = {(int(f_state), int(t_state)): node_path for f_state, t_state, node_path, c in
                              zip(_[markov_field.FROM_STATE],
                                  _[markov_field.TO_STATE],
                                  _[path_field],
                                  _[cost_field]) if c > 0}
+
         same_link_idx = transition_df[markov_field.FROM_STATE] == transition_df[markov_field.TO_STATE]
-        transition_df.loc[same_link_idx, markov_field.ROUTE_LENGTH] = \
-            np.abs(transition_df.loc[same_link_idx, :]['from_route_dis'] -
-                   transition_df.loc[same_link_idx, :]['to_route_dis'])
-        transition_df['2nd_node'] = -1
-        transition_df['-2nd_node'] = -1
-        # normal_path_idx_a = transition_df[cost_field] > 0, normal_path_idx_a可能全是False
-        try:
-            transition_df.loc[normal_path_idx_a, '2nd_node'] = transition_df.loc[normal_path_idx_a, :][
-                path_field].apply(
-                lambda x: x[1])
-            transition_df.loc[normal_path_idx_a, '-2nd_node'] = transition_df.loc[normal_path_idx_a, :][
-                path_field].apply(
-                lambda x: x[-2])
-        except:
-            pass
-        normal_path_idx_b = (normal_path_idx_a & \
-                             (transition_df['2nd_node'] == transition_df['from_link_t']) & \
-                             (transition_df['-2nd_node'] != transition_df['to_link_t'])) | \
+        normal_path_idx_b = (normal_path_idx_a & (transition_df['2nd_node'] == transition_df['from_link_t']) & (
+                    transition_df['-2nd_node'] != transition_df['to_link_t'])) | \
                             ((transition_df['from_link_f'] == transition_df['to_link_t']) &
                              (transition_df['from_link_t'] == transition_df['to_link_f']))
+        final_idx = normal_path_idx_b | same_link_idx
+        transition_df.loc[final_idx, markov_field.ROUTE_LENGTH] = \
+            np.abs(transition_df.loc[final_idx, :][cost_field] -
+                   transition_df.loc[final_idx, :]['from_route_dis'] +
+                   transition_df.loc[final_idx, :]['to_route_dis'])
+        transition_df[gps_field.ADJ_DIS] = transition_df[gps_field.FROM_GPS_SEQ].map(gps_adj_dis_map)
 
-        transition_df.loc[normal_path_idx_b, markov_field.ROUTE_LENGTH] = \
-            np.abs(transition_df.loc[normal_path_idx_b, :][cost_field] -
-                   transition_df.loc[normal_path_idx_b, :]['from_route_dis'] +
-                   transition_df.loc[normal_path_idx_b, :]['to_route_dis'])
-
-        transition_df = pd.merge(transition_df, gps_pre_next_dis_df, on=[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ],
-                                 how='left')
         transition_df[markov_field.DIS_GAP] = np.abs(
             -transition_df[markov_field.ROUTE_LENGTH] + transition_df[gps_field.ADJ_DIS])
 
         s2s_route_l = transition_df[[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ, markov_field.ROUTE_LENGTH,
                                      markov_field.FROM_STATE, markov_field.TO_STATE]].copy()
-        transition_df['trans_values'] = \
-            self.transition_probability(self.beta, transition_df[markov_field.DIS_GAP].values, self.dis_para)
-
-        ft_transition_dict = {f_gps_seq: df['trans_values'].values.reshape(seq_len_dict[f_gps_seq],
-                                                                           int(len(df) / seq_len_dict[f_gps_seq])) for
-                              (f_gps_seq, t_gps_seq), df in
-                              transition_df.groupby([gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ])}
-
-        return adj_seq_path_dict, ft_transition_dict, ft_idx_map, s2s_route_l, seq_k_candidate_info, done_stp_cost_df
+        return adj_seq_path_dict, ft_idx_map, s2s_route_l, seq_k_candidate_info, done_stp_cost_df, \
+            seq_len_dict, transition_df
 
     def add_path_cache(self, done_stp_cost_df: pd.DataFrame = None, source_node_list: list[int] or set[int] = None,
                        g: nx.DiGraph = None, method: str = 'dijkstra', single_link_ft_path_df: pd.DataFrame = None,
                        weight_field: str = None, cut_off: float = 600.0, add_single_ft: list[bool] = True) \
             -> pd.DataFrame:
         _done_stp_cost_df = self.single_source_path_cache(node_list=source_node_list, method=method, cut_off=cut_off,
                                                           weight_field=weight_field, g=g)
@@ -569,38 +694,36 @@
                                                                                     gps_field.SUB_SEQ_FIELD]]])
             gps_link_state_df.sort_values(by=[gps_field.POINT_SEQ_FIELD, gps_field.SUB_SEQ_FIELD],
                                           ascending=[True, True], inplace=True)
             gps_link_state_df.reset_index(inplace=True, drop=True)
 
         # 给每个gps点打上路网link标签, 存在GPS匹配不到路段的情况(比如buffer范围内无候选路段)
         gps_match_res_gdf = pd.merge(gps_match_res_gdf[[gps_field.POINT_SEQ_FIELD, gps_field.AGENT_ID_FIELD,
-                                                        gps_field.LNG_FIELD, gps_field.LAT_FIELD, gps_field.TIME_FIELD,
+                                                        gps_field.PLAIN_X, gps_field.PLAIN_Y, gps_field.TIME_FIELD,
                                                         gps_field.GEOMETRY_FIELD]],
                                      gps_link_state_df, on=gps_field.POINT_SEQ_FIELD, how='right')
         del gps_link_state_df
         gps_match_res_gdf.loc[gps_match_res_gdf[gps_field.NEXT_LINK_FIELD].isna(), net_field.GEOMETRY_FIELD] = \
             omitted_gps_state_df[net_field.GEOMETRY_FIELD].to_list()
         gps_match_res_gdf.loc[gps_match_res_gdf[gps_field.NEXT_LINK_FIELD].isna(), gps_field.TIME_FIELD] = \
             omitted_gps_state_df[gps_field.TIME_FIELD].to_list()
 
         gps_match_res_gdf.drop(columns=[gps_field.NEXT_LINK_FIELD], axis=1, inplace=True)
         gps_match_res_gdf = gpd.GeoDataFrame(gps_match_res_gdf, geometry=gps_field.GEOMETRY_FIELD,
                                              crs=self.gps_points.crs)
         gps_match_res_gdf = gps_match_res_gdf.to_crs(self.gps_points.geo_crs)
-        gps_match_res_gdf[[gps_field.LNG_FIELD, gps_field.LAT_FIELD]] = gps_match_res_gdf.apply(
-            lambda row: (row[gps_field.GEOMETRY_FIELD].x, row[gps_field.GEOMETRY_FIELD].y), axis=1,
-            result_type='expand')
+        gps_match_res_gdf[gps_field.LNG_FIELD] = gps_match_res_gdf[gps_field.GEOMETRY_FIELD].apply(lambda p: p.x)
+        gps_match_res_gdf[gps_field.LAT_FIELD] = gps_match_res_gdf[gps_field.GEOMETRY_FIELD].apply(lambda p: p.y)
         prj_gdf = gps_match_res_gdf[[markov_field.PRJ_GEO]].copy()
         del gps_match_res_gdf[markov_field.PRJ_GEO]
         prj_gdf.dropna(subset=[markov_field.PRJ_GEO], inplace=True)
         prj_gdf = gpd.GeoDataFrame(prj_gdf, geometry=markov_field.PRJ_GEO, crs=self.gps_points.plane_crs)
         prj_gdf = prj_gdf.to_crs(self.gps_points.geo_crs)
-        prj_gdf[['prj_lng', 'ptj_lat']] = prj_gdf.apply(
-            lambda row: (row[markov_field.PRJ_GEO].x, row[markov_field.PRJ_GEO].y), axis=1,
-            result_type='expand')
+        prj_gdf['prj_lng'] = prj_gdf[markov_field.PRJ_GEO].apply(lambda p: p.x)
+        prj_gdf['prj_lat'] = prj_gdf[markov_field.PRJ_GEO].apply(lambda p: p.y)
         gps_match_res_gdf = pd.merge(gps_match_res_gdf, prj_gdf, how='left', left_index=True, right_index=True)
         del prj_gdf
         self.gps_match_res_gdf = gps_match_res_gdf
         return self.gps_match_res_gdf
 
     def acquire_omitted_match_item(self, gps_link_state_df: pd.DataFrame = None) -> pd.DataFrame:
         """
@@ -660,17 +783,17 @@
                         (pre_seq, _single_link, sub_seq) + bilateral_unidirectional_mapping[_single_link]
                         for _single_link, sub_seq in zip(_single_link_list,
                                                          range(1, len(_single_link_list) + 1))]
 
                     # 利用前后的GPS点信息来补全缺失的GPS点
                     pre_order_gps, next_order_gps = gps_match_res_gdf.at[pre_seq, net_field.GEOMETRY_FIELD], \
                         gps_match_res_gdf.at[next_seq, net_field.GEOMETRY_FIELD]
-                    omitted_gps_points.extend(n_equal_points(len(_single_link_list) + 1, from_point=pre_order_gps,
-                                                             to_point=next_order_gps, add_noise=True, noise_frac=0.3))
-
+                    omitted_gps_points.extend(n_equal_points(len(_single_link_list) + 1,
+                                                             from_loc=(pre_order_gps.x, pre_order_gps.y),
+                                                             to_loc=(next_order_gps.x, next_order_gps.y)))
                     # 一条补出来的路生成一个GPS点
                     pre_seq_time, next_seq_time = gps_match_res_gdf.at[pre_seq, gps_field.TIME_FIELD], \
                         gps_match_res_gdf.at[next_seq, gps_field.TIME_FIELD]
                     dt = (next_seq_time - pre_seq_time).total_seconds() / (len(omitted_gps_points) + 1)
                     omitted_gps_points_time.extend(
                         [pre_seq_time + timedelta(seconds=dt * n) for n in range(1, len(_single_link_list) + 1)])
                 else:
@@ -855,17 +978,16 @@
         match_link_gdf = gpd.GeoDataFrame(match_link_gdf, geometry=net_field.GEOMETRY_FIELD, crs=self.net.planar_crs)
         match_link_gdf = match_link_gdf.to_crs(self.net.geo_crs)
 
         for gdf, name in zip([gps_layer, prj_p_layer, prj_l_layer, match_link_gdf],
                              ['gps', 'prj_p', 'prj_l', 'match_link']):
             gdf.to_file(os.path.join(out_fldr, '-'.join([flag_name, name]) + '.geojson'), driver='GeoJSON')
 
-    def format_war_info(self):
-        if self.warn_info['from_ft']:
-            self.format_warn_info = pd.DataFrame(self.warn_info)
+    def formatting_warn_info(self):
+        self.format_warn_info = pd.DataFrame(self.warn_info)
         del self.warn_info
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/GlobalVal.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/NetGen.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/NetGen.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,41 +2,38 @@
 # @Time    : 2023/7/31 0031 9:52
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 
 """生产路网的相关方法"""
 
-import time
 import os.path
 import pandas as pd
 import geopandas as gpd
 from ..map.Net import Net
 from .RoadNet.conn import Conn
 from .GlobalVal import NetField
 from .format_od import FormatOD
 from .RoadNet import net_reverse
 from ..gps.GpsTrip import GpsTrip
 from .RoadNet.increment import increment
 from .RoadNet.save_file import save_file
 from .Request.request_path import CarPath
 from .RoadNet.optimize_net import optimize
-from ..WrapsFunc import function_time_cost
 from .Parse.gd_car_path import ParseGdPath
 from .RoadNet.Split.SplitPath import split_path
 from .PublicTools.GeoProcess import generate_region
 from .RoadNet.Split.SplitPath import split_path_main
 from ..tools.geo_process import clean_link_geo, remapping_id
 from .RoadNet.Tools.process import merge_double_link, create_single_link
 from .RoadNet.SaveStreets.streets import generate_node_from_link, modify_minimum
 
 
 net_field = NetField()
 
-
 class Reverse(object):
     def __init__(self, flag_name: str = '深圳市', plain_prj: str = None, net_out_fldr: str = None,
                  net_file_type: str = 'shp'):
         # overall
         self.flag_name = flag_name
         self.plain_prj = plain_prj
         self.net_out_fldr = net_out_fldr
@@ -299,15 +296,15 @@
                      od_num: int = 100, gap_n: int = 1000, min_od_length: float = 1200.0) -> tuple[bool, list[str]]:
         """构造OD -> 请求 -> 二进制存储"""
         assert binary_path_fldr is not None
 
         assert od_type in ['rand_od', 'region_od', 'diy_od', 'gps_based']
         fmod = FormatOD(plain_crs=self.plain_prj)
         if isinstance(region_gdf, gpd.GeoDataFrame) and not region_gdf.empty:
-            assert region_gdf.crs.srs == 'EPSG:4326', '面域文件必须是EPSG:4326"'
+            assert region_gdf.crs.srs.upper() == 'EPSG:4326', '面域文件必须是EPSG:4326"'
         if od_type == 'rand_od':
             if region_gdf is None or region_gdf.empty:
                 region_gdf = generate_region(min_lng=min_lng, min_lat=min_lat, w=w, h=h, plain_crs=self.plain_prj)
 
             od_df = fmod.format_region_rnd_od(region_gdf=region_gdf, flag_name=self.flag_name, od_num=od_num,
                                               gap_n=gap_n, length_limit=min_od_length,
                                               boundary_buffer=boundary_buffer)
@@ -375,15 +372,15 @@
         :param node_gdf:
         :param book_mark_name:
         :param link_name_field:
         :param generate_mark
         :return:
         """
         geo_crs = link_gdf.crs.srs
-        assert geo_crs == 'EPSG:4326'
+        assert geo_crs.upper() == 'EPSG:4326'
         link_gdf, node_gdf = self.fix_minimum_gap(node_gdf=node_gdf, link_gdf=link_gdf)
         net = Net(link_gdf=link_gdf, node_gdf=node_gdf, create_single=False)
         conn = Conn(net=net, check_buffer=self.conn_buffer)
         conn.execute(out_fldr=self.net_out_fldr, file_name=book_mark_name, generate_mark=generate_mark)
         net.export_net(export_crs=link_gdf.crs.srs, out_fldr=self.net_out_fldr, file_type=self.net_file_type,
                        flag_name='modifiedConn')
         net.to_geo_prj()
@@ -443,15 +440,18 @@
         :param link_gdf:
         :param node_gdf:
         :return:
         """
         my_net = Net(link_gdf=link_gdf,
                      node_gdf=node_gdf, create_single=False, delete_circle=False)
         my_net.process_circle()
-        return my_net.get_bilateral_link_data().reset_index(drop=True), my_net.get_node_data().reset_index(drop=True)
+        link, node = my_net.get_bilateral_link_data().reset_index(drop=True), my_net.get_node_data().reset_index(drop=True)
+        link = link.to_crs('EPSG:4326')
+        node = node.to_crs('EPSG:4326')
+        return link, node
 
     def redivide_link_node(self, link_gdf: gpd.GeoDataFrame = None):
         """
         对link进行线层和点层的重新划分
         :param link_gdf: gpd.GeoDataFrame, 要求至少有geometry字段
         """
         link_gdf = link_gdf.to_crs('EPSG:4326')
```

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/Parse/gd_car_path.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/Parse/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/GeoProcess.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/GraphAna.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/GraphAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/IndexAna.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/IndexAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/PublicTools/od.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/Request/api/WebApi.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/Request/api/WebApi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/Request/request_path.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/Request/request_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/bd_ts.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/bd_ts.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/Request/usage/gd_car_path.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         2     [(13, 14), (14, 15), (15, 16), (16, 17)]                       [0,0,0]      [XX路,XX路,XX路]
         3     [(1, 7), (7, 9), (3, 9), (3, 4), (4, 5), (5, 99)]               [0,1,0]      [XX路,XX路,XX路]
     """
 
     # 直接修改传入的link_gdf
     print(r'##########   Merge Road Sections')
     node_gdf.set_index(node_id_field, inplace=True)
-    origin_crs = link_gdf.crs
+    origin_crs = link_gdf.crs.srs
     link_gdf['sorted_ft'] = link_gdf[[from_node_id_field, to_node_id_field]].apply(lambda x: tuple(sorted(x)), axis=1)
 
     origin_sorted_ft_list = link_gdf['sorted_ft'].to_list()
 
     # 用于记录合并信息
     merge_info_dict = dict()
 
@@ -257,15 +257,15 @@
 def get_length_from_linestring(linestring_obj=None, crs='EPSG:4326'):
     """
     在epsg:4326下计算LineString的长度, km
     :param linestring_obj: LineString, 多段线对象
     :param crs:
     :return:
     """
-    if crs == 'EPSG:4326':
+    if crs.upper() == 'EPSG:4326':
         coord_list = list(linestring_obj.coords)
         try:
             length_list = [distance(tuple(coord_list[i][::-1]), tuple(coord_list[i + 1][::-1])).m for i in range(0, len(coord_list) - 1)]
             return sum(length_list)
         except ValueError as e:
             # print(r'是平面坐标')
             return linestring_obj.length
```

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,15 @@
 def get_length_from_linestring(linestring_obj=None, crs='EPSG:4326'):
     """
     在epsg:4326下计算LineString的长度, km
     :param linestring_obj: LineString, 多段线对象
     :param crs:
     :return:
     """
-    if crs == 'EPSG:4326':
+    if crs.upper() == 'EPSG:4326':
         coord_list = list(linestring_obj.coords)
         try:
             length_list = [distance(tuple(coord_list[i][::-1]), tuple(coord_list[i + 1][::-1])).m for i in
                            range(0, len(coord_list) - 1)]
             return sum(length_list)
         except ValueError as e:
             # print(r'是平面坐标')
```

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -- coding: utf-8 --
 # @Time    : 2024/1/25 14:37
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 
 """路网点层生产, 并且做一些空间优化"""
-
+import numpy as np
 import pandas as pd
 import networkx as nx
 import geopandas as gpd
 from ..save_file import save_file
 from ...GlobalVal import NetField
 from shapely.geometry import Point
 from shapely.geometry import LineString
@@ -67,17 +67,15 @@
             update_link_field_list.remove(net_field.TO_NODE_FIELD)
 
     # 3.更新线层数据
     link_gdf = update_link(link_gdf=link_gdf, node_gdf=node_gdf, update_link_field_list=update_link_field_list,
                            origin_crs=origin_crs, plain_prj=plain_prj, fill_dir=fill_dir)
 
     # 去除没有link连接的节点
-    used_node = set(link_gdf[net_field.FROM_NODE_FIELD]) | set(link_gdf[net_field.TO_NODE_FIELD])
-    node_gdf.drop(index=node_gdf[~node_gdf[net_field.NODE_ID_FIELD].isin(used_node)].index, inplace=True, axis=1)
-    node_gdf.reset_index(inplace=True, drop=True)
+    drop_no_use_nodes(link_gdf, node_gdf)
 
     if save_streets_before_modify_minimum:
         save_file(data_item=link_gdf, file_type=net_file_type, out_fldr=out_fldr, file_name='LinkBeforeModify')
         save_file(data_item=node_gdf, file_type=net_file_type, out_fldr=out_fldr, file_name='NodeBeforeModify')
 
     # 极小间隔点优化
     node_group_status_gdf = gpd.GeoDataFrame()
@@ -127,18 +125,16 @@
         node_gdf.reset_index(inplace=True, drop=True)
         node_gdf = gpd.GeoDataFrame(node_gdf, geometry=net_field.GEOMETRY_FIELD, crs=origin_crs)
     else:
         # 取出操作列
         used_link_geo = link_gdf[[net_field.GEOMETRY_FIELD]].copy()
 
         # 取出两端坐标
-        used_link_geo['f_coords'] = used_link_geo.apply(
-            lambda x: list(x[net_field.GEOMETRY_FIELD].coords)[0], axis=1)
-        used_link_geo['t_coords'] = used_link_geo.apply(
-            lambda x: list(x[net_field.GEOMETRY_FIELD].coords)[-1], axis=1)
+        used_link_geo['f_coords'] = used_link_geo[net_field.GEOMETRY_FIELD].apply(lambda geo: list(geo.coords)[0])
+        used_link_geo['t_coords'] = used_link_geo[net_field.GEOMETRY_FIELD].apply(lambda geo: list(geo.coords)[-1])
         non_dup_coords_list = used_link_geo['f_coords'].to_list() + used_link_geo['t_coords'].to_list()
         node_coords_list = list(set(non_dup_coords_list))
         node_gdf = gpd.GeoDataFrame({net_field.NODE_ID_FIELD: [x for x in range(1, len(node_coords_list) + 1)]},
                                     geometry=[Point(cor) for cor in node_coords_list], crs=origin_crs)
     return node_gdf
 
 
@@ -175,15 +171,15 @@
     link_gdf[net_field.TO_NODE_FIELD] = join_data[net_field.NODE_ID_FIELD]
     del join_data
     link_gdf.drop(['__TopologyFromCoord__', '__TopologyToCoord___'], inplace=True, axis=1)
 
     if net_field.LENGTH_FIELD in update_link_field_list:
         # 更新length
         link_gdf = link_gdf.to_crs(plain_prj)
-        link_gdf[net_field.LENGTH_FIELD] = link_gdf[net_field.GEOMETRY_FIELD].apply(lambda x: round(x.length, 2))
+        link_gdf[net_field.LENGTH_FIELD] = np.around(link_gdf[net_field.GEOMETRY_FIELD].length, 2)
         link_gdf = link_gdf.to_crs(origin_crs)
     else:
         assert net_field.LENGTH_FIELD in col_list, f'线层数据中缺少{net_field.LENGTH_FIELD}字段, 但是却没有指定更新!'
 
     if net_field.LINK_ID_FIELD in update_link_field_list:
         # 更新link_id
         link_gdf[net_field.LINK_ID_FIELD] = [x for x in range(1, len(link_gdf) + 1)]
@@ -229,16 +225,15 @@
     if origin_crs == plain_prj:
         pass
     else:
         node_gdf = node_gdf.to_crs(plain_prj)
 
     buffer_node_gdf = node_gdf.copy()
 
-    buffer_node_gdf[net_field.GEOMETRY_FIELD] = \
-        buffer_node_gdf[net_field.GEOMETRY_FIELD].apply(lambda x: x.buffer(buffer))
+    buffer_node_gdf[net_field.GEOMETRY_FIELD] = buffer_node_gdf[net_field.GEOMETRY_FIELD].buffer(buffer)
     join_df = gpd.sjoin(node_gdf, buffer_node_gdf)
 
     node_gdf = node_gdf.to_crs(origin_crs)
 
     join_df.reset_index(inplace=True, drop=True)
 
     join_df.drop(
@@ -306,32 +301,46 @@
         alter_link_gdf.drop_duplicates(subset=[net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD], inplace=True,
                                        keep='first')
         alter_link_gdf.drop(index=alter_link_gdf[alter_link_gdf[net_field.FROM_NODE_FIELD] ==
                                                  alter_link_gdf[net_field.TO_NODE_FIELD]].index, inplace=True, axis=0)
         link_gdf = link_gdf.drop(index=link_gdf[alter_index].index, axis=0)
 
         # 修改起终点坐标
-        alter_link_gdf[net_field.GEOMETRY_FIELD] = alter_link_gdf.apply(
-            lambda item: LineString([(node_gdf.at[item[net_field.FROM_NODE_FIELD], net_field.GEOMETRY_FIELD].x,
-                                      node_gdf.at[item[net_field.FROM_NODE_FIELD], net_field.GEOMETRY_FIELD].y)] +
-                                    list(item[net_field.GEOMETRY_FIELD].coords)[1:-1] +
-                                    [(node_gdf.at[item[net_field.TO_NODE_FIELD], net_field.GEOMETRY_FIELD].x,
-                                      node_gdf.at[item[net_field.TO_NODE_FIELD], net_field.GEOMETRY_FIELD].y)]), axis=1)
+        # 可能一条link退化为点
+        if not alter_link_gdf.empty:
+            # alter_link_gdf[net_field.GEOMETRY_FIELD] = alter_link_gdf.apply(
+            #     lambda item: LineString([(node_gdf.at[item[net_field.FROM_NODE_FIELD], net_field.GEOMETRY_FIELD].x,
+            #                               node_gdf.at[item[net_field.FROM_NODE_FIELD], net_field.GEOMETRY_FIELD].y)] +
+            #                             list(item[net_field.GEOMETRY_FIELD].coords)[1:-1] +
+            #                             [(node_gdf.at[item[net_field.TO_NODE_FIELD], net_field.GEOMETRY_FIELD].x,
+            #                               node_gdf.at[item[net_field.TO_NODE_FIELD], net_field.GEOMETRY_FIELD].y)]), axis=1)
+            alter_link_gdf[net_field.GEOMETRY_FIELD] = [
+                LineString([(node_gdf.at[fn, net_field.GEOMETRY_FIELD].x,
+                             node_gdf.at[fn, net_field.GEOMETRY_FIELD].y)] +
+                           list(geo.coords)[1:-1] +
+                           [(node_gdf.at[tn, net_field.GEOMETRY_FIELD].x,
+                             node_gdf.at[tn, net_field.GEOMETRY_FIELD].y)]) for fn, tn, geo in
+                zip(alter_link_gdf[net_field.FROM_NODE_FIELD],
+                    alter_link_gdf[net_field.TO_NODE_FIELD],
+                    alter_link_gdf[net_field.GEOMETRY_FIELD])]
 
-        link_gdf = pd.concat([link_gdf, alter_link_gdf])
+            link_gdf = pd.concat([link_gdf, alter_link_gdf])
 
         link_gdf = gpd.GeoDataFrame(link_gdf, geometry=net_field.GEOMETRY_FIELD, crs=origin_crs)
 
         link_gdf.reset_index(inplace=True, drop=True)
         node_gdf.reset_index(inplace=True, drop=False)
 
         link_gdf.drop_duplicates(subset=[net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD], keep='first',
                                  inplace=True)
         link_gdf.reset_index(inplace=True, drop=True)
 
+        # 去除没有link连接的节点
+        drop_no_use_nodes(link_gdf, node_gdf)
+
         node_group_status_df = pd.DataFrame(node_group_status_list, columns=[net_field.NODE_ID_FIELD, 'status'])
         node_group_status_df = pd.merge(node_group_status_df,
                                         node_gdf[[net_field.NODE_ID_FIELD, net_field.GEOMETRY_FIELD]],
                                         on=net_field.NODE_ID_FIELD,
                                         how='left')
         node_group_status_gdf = gpd.GeoDataFrame(node_group_status_df, geometry=net_field.GEOMETRY_FIELD,
                                                  crs=origin_crs)
@@ -424,7 +433,14 @@
 
         # delete_node: remain_node
         node_map_dict = {}
         for node_group in nx.connected_components(g):
             # 必然有 >= 2 个元素
             node_group_list = list(node_group)
             node_map_dict.update({origin_node: node_group_list[0] for origin_node in node_group_list[1:]})
+
+
+def drop_no_use_nodes(link_gdf: gpd.GeoDataFrame = None, node_gdf: gpd.GeoDataFrame = None):
+    # 去除没有link连接的节点
+    used_node = set(link_gdf[net_field.FROM_NODE_FIELD]) | set(link_gdf[net_field.TO_NODE_FIELD])
+    node_gdf.drop(index=node_gdf[~node_gdf[net_field.NODE_ID_FIELD].isin(used_node)].index, inplace=True, axis=1)
+    node_gdf.reset_index(inplace=True, drop=True)
```

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/Tools/process.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Tools/process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/conn.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/conn.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/increment.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/increment.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/net_reverse.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/net_reverse.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/optimize_net.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/optimize_net.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,25 +72,25 @@
         generate_book_mark(input_fldr=out_fldr, name_loc_dict=merge_info_dict, prj_name=out_fldr.split('/')[-1])
         new_link.to_file(os.path.join(out_fldr, 'AfterTPMergeLink.shp'), encoding='gbk')
         new_node.to_file(os.path.join(out_fldr, 'AfterTPMergeNode.shp'), encoding='gbk')
 
     # 是否处理重复link
     if is_process_dup_link:
         origin_crs = new_link.crs.srs
-        if new_link.crs.srs == plain_prj:
+        if new_link.crs.srs.upper() == plain_prj.upper():
             pass
         else:
             new_link = new_link.to_crs(plain_prj)
             new_node = new_node.to_crs(plain_prj)
         print(r'##########   Remove Overlapping Road Segments')
         final_link, final_node, dup_info_dict = process_dup_link(link_gdf=new_link, node_gdf=new_node,
                                                                  buffer=process_dup_link_buffer,
                                                                  dup_link_buffer_ratio=dup_link_buffer_ratio,
                                                                  modify_minimum_buffer=modify_minimum_buffer)
-        if final_link.crs.srs == origin_crs:
+        if final_link.crs.srs.upper() == origin_crs.upper():
             pass
         else:
             final_link = final_link.to_crs(origin_crs)
             final_node = final_node.to_crs(origin_crs)
         return final_link, final_node, dup_info_dict
     else:
         return new_link, new_node, dict()
```

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/RoadNet/save_file.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/book_mark.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/book_mark.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/netreverse/format_od.py` & `gotrackit-0.2.5/src/gotrackit/netreverse/format_od.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         :param flag_name:
         :param od_num:
         :param gap_n:
         :param length_limit:
         :param boundary_buffer:
         :return:
         """
-        origin_crs = region_gdf.crs
+        origin_crs = region_gdf.crs.srs
         region_gdf = region_gdf.to_crs(self.plain_crs)
         region_gdf[region_field.GEO_FIELD] = region_gdf[region_field.GEO_FIELD].apply(
             lambda geo: geo.buffer(boundary_buffer))
         region_gdf = region_gdf.to_crs(origin_crs)
         polygon_obj = unary_union(region_gdf[region_field.GEO_FIELD].to_list())
         rnd_od_df = region_rnd_od(polygon_obj=polygon_obj, flag_name=flag_name,
                                   od_num=od_num, gap_n=gap_n, length_limit=length_limit)
```

### Comparing `gotrackit-0.2.4/src/gotrackit/netxfer/SumoConvert.py` & `gotrackit-0.2.5/src/gotrackit/netxfer/SumoConvert.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/solver/Viterbi.py` & `gotrackit-0.2.5/src/gotrackit/solver/Viterbi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/tools/coord_trans.py` & `gotrackit-0.2.5/src/gotrackit/tools/coord_trans.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/tools/geo_process.py` & `gotrackit-0.2.5/src/gotrackit/tools/geo_process.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,57 +5,37 @@
 
 
 import numpy as np
 import pandas as pd
 import geopandas as gpd
 from ..GlobalVal import NetField
 from .coord_trans import LngLatTransfer
-from shapely.geometry import LineString, Point
 from shapely.geometry import Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon, LinearRing
-from ..WrapsFunc import function_time_cost
 
 net_field = NetField()
 geometry_field = net_field.GEOMETRY_FIELD
 node_id_field = net_field.NODE_ID_FIELD
 link_id_field = net_field.LINK_ID_FIELD
 from_node_field = net_field.FROM_NODE_FIELD
 to_node_field = net_field.TO_NODE_FIELD
 
 
-def n_equal_points(n, from_loc: tuple = None, to_loc=None,
-                   from_point: Point = None, to_point: Point = None, add_noise: bool = False,
-                   noise_frac: float = 0.3) -> list[list]:
+def n_equal_points(n, from_loc: tuple = None, to_loc: tuple = None) -> list[tuple]:
     """
 
     :param n:
     :param from_loc:
     :param to_loc:
-    :param from_point:
-    :param to_point:
-    :param add_noise:
-    :param noise_frac:
     :return:
     """
     assert n > 1
-    if from_point is None or to_point is None:
-        line = LineString([from_loc, to_loc])
-    else:
-        line = LineString([from_point, to_point])
-    line_length = line.length
-
     try:
-        dense_line = segmentize(line=line, n=n)
+        equal_points = segmentize(s_loc=from_loc, e_loc=to_loc, n=n)
     except AttributeError:
         raise AttributeError(r'请升级geopandas到最新版本0.14.1')
-
-    equal_points = list(dense_line.coords)[1:-1]
-    if add_noise:
-        base_noise = 0.707106 * noise_frac * line_length / n
-        equal_points = [[loc[0] + np.random.normal(loc=0, scale=base_noise),
-                         loc[1] + np.random.normal(loc=0, scale=base_noise)] for loc in equal_points]
     return equal_points
 
 
 def cut_line_in_nearest_point(line, point) -> list[LineString]:
     """
 
     :param line:
@@ -109,77 +89,83 @@
         return 180 * np.arccos(cos_res) / np.pi
     elif cos_res < 0:
         if cos_res < -1.0:
             cos_res = -0.99999
     return 180 * np.arccos(cos_res) / np.pi
 
 
-def segmentize(line: LineString = None, n: int = None) -> LineString:
+def segmentize(s_loc: list or tuple = None, e_loc: list or tuple = None, n: int = None) -> list[tuple]:
     """
-    将直线对象line进行n等分加密
-    :param line: 直线
+    将直线对象line进行n等分加密, 返回中间的加密点坐标
+    :param s_loc
+    :param e_loc
     :param n:
     :return:
     """
-    coord_list = list(line.coords)
-    s, e = coord_list[0], coord_list[-1]
+    # s, e = coord_list[0], coord_list[-1]
     try:
-        k = (e[1] - s[1]) / (e[0] - s[0])
+        k = (e_loc[1] - s_loc[1]) / (e_loc[0] - s_loc[0])
     except ZeroDivisionError:
-        gap = line.length / n
-        return LineString([s] + [(s[0], s[1] + (i + 1) * gap) for i in range(n - 1)] + [e])
+        gap = np.abs(e_loc[1] - s_loc[1]) / n
+        return [(s_loc[0], s_loc[1] + (i + 1) * gap) for i in range(n - 1)]
 
-    b = e[1] - k * e[0]
-    gap_x = (e[0] - s[0]) / n
-    sample_x_list = [s[0] + (i + 1) * gap_x for i in range(n - 1)]
-    return LineString([s] + [(sample_x, k * sample_x + b) for sample_x in sample_x_list] + [e])
+    b = e_loc[1] - k * e_loc[0]
+    gap_x = (e_loc[0] - s_loc[0]) / n
+    sample_x_list = [s_loc[0] + (i + 1) * gap_x for i in range(n - 1)]
+    return [(sample_x, k * sample_x + b) for sample_x in sample_x_list]
 
 
-def prj_inf(p: Point = None, line: LineString = None) -> tuple[Point, float, float, float, list[LineString], np.ndarray]:
+def prj_inf(p: Point = None, line: LineString = None) -> tuple[Point, float, float, float, list[LineString], float, float]:
     """
     # 返回 某point到line的(投影点坐标, 点到投影点的直线距离, 投影点到line拓扑起点的路径距离, line的长度, 投影点打断line后的geo list)
     :param p:
     :param line:
     :return: (投影点坐标, 点到投影点的直线距离, 投影点到line拓扑起点的路径距离, line的长度, 投影点打断line后的geo list, 投影点的方向向量)
     """
 
     distance = line.project(p)
 
     if distance <= 0.0:
         line_cor = list(line.coords)
         prj_p = Point(line_cor[0])
-        prj_vec = np.array(line_cor[1]) - np.array(line_cor[0])
-        return prj_p, prj_p.distance(p), distance, line.length, [LineString(line)], prj_vec
+        # prj_vec = np.array(line_cor[1]) - np.array(line_cor[0])
+        dx, dy = line_cor[1][0] - line_cor[0][0], line_cor[1][1] - line_cor[0][1]
+        return prj_p, prj_p.distance(p), distance, line.length, [LineString(line)], dx, dy
     elif distance >= line.length:
         line_cor = list(line.coords)
         prj_p = Point(line_cor[-1])
-        prj_vec = np.array(line_cor[-1]) - np.array(line_cor[-2])
-        return prj_p, prj_p.distance(p), distance, line.length, [LineString(line)], prj_vec
+        # prj_vec = np.array(line_cor[-1]) - np.array(line_cor[-2])
+        dx, dy = line_cor[-1][0] - line_cor[-2][0], line_cor[-1][1] - line_cor[-2][1]
+        return prj_p, prj_p.distance(p), distance, line.length, [LineString(line)], dx, dy
     else:
         coords = list(line.coords)
         for i, _p in enumerate(coords):
             xd = line.project(Point(_p))
             if xd == distance:
                 prj_p = Point(coords[i])
-                prj_vec = np.array(coords[i]) - np.array(coords[i - 1])
+                # prj_vec = np.array(coords[i]) - np.array(coords[i - 1])
+                dx, dy = coords[i][0] - coords[i - 1][0], coords[i][1] - coords[i - 1][1]
                 return prj_p, prj_p.distance(p), distance, line.length, \
-                    [LineString(coords[:i + 1]), LineString(coords[i:])], prj_vec
+                    [LineString(coords[:i + 1]), LineString(coords[i:])], dx, dy
             if xd > distance:
                 cp = line.interpolate(distance)
                 prj_p = Point((cp.x, cp.y))
-                prj_vec = np.array(coords[i]) - np.array(coords[i - 1])
+                # prj_vec = np.array(coords[i]) - np.array(coords[i - 1])
+                dx, dy = coords[i][0] - coords[i - 1][0], coords[i][1] - coords[i - 1][1]
                 return prj_p, prj_p.distance(p), distance, line.length, [LineString(coords[:i] + [(cp.x, cp.y)]),
                                                                          LineString(
-                                                                             [(cp.x, cp.y)] + coords[i:])], prj_vec
-
+                                                                             [(cp.x, cp.y)] + coords[i:])], dx, dy
+    # to here means error
+    raise ValueError(r'路段几何存在重叠环路线型, 请使用redivide_link_node函数处理')
 
 def clean_link_geo(gdf: gpd.GeoDataFrame = None, plain_crs: str = 'EPSG:32650', l_threshold: float = 0.5) -> gpd.GeoDataFrame:
     """
     将geometry列中的Multi对象处理为single对象
     :param gdf:
+    :param l_threshold:
     :param plain_crs
     :return:
     """
     assert geometry_field in gdf.columns
     origin_crs = gdf.crs.srs
     con = LngLatTransfer()
 
@@ -224,16 +210,16 @@
     node_gdf[node_id_field] = node_gdf[node_id_field].map(node_map)
     link_gdf[link_id_field] = [i for i in range(1, len(link_gdf) + 1)]
     link_gdf[[from_node_field, to_node_field]] = link_gdf.apply(lambda row: (node_map[row[from_node_field]],
                                                                              node_map[row[to_node_field]]), axis=1,
                                                                 result_type='expand')
 
 
-def divide_line_by_l(line_geo: LineString = None, divide_l: float = 50.0, l_min: float = 0.5) -> tuple[
-    list[LineString], list[Point], int]:
+def divide_line_by_l(line_geo: LineString = None, divide_l: float = 50.0, l_min: float = 0.5) -> \
+        tuple[list[LineString], list[Point], int]:
     """
 
     :param line_geo:
     :param divide_l:
     :param l_min:
     :return:
     """
@@ -249,15 +235,15 @@
     divide_point_list = []
 
     for i, p in enumerate(p_list):
         if i + 1 == len(p_list):
             if not is_remain:
                 divide_line_list.append(used_l)
                 break
-        prj_p, _, dis, _, split_line_list, _ = prj_inf(p, used_l)
+        prj_p, _, dis, _, split_line_list, _, _ = prj_inf(p, used_l)
         used_l = split_line_list[-1]
         if i + 1 == len(p_list):
             if is_remain:
                 divide_line_list.extend(split_line_list)
                 divide_point_list.append(p)
                 break
         divide_line_list.append(split_line_list[0])
@@ -298,33 +284,48 @@
     # 在GPS点密集处, gps_diff_vec不准确, 往往gps_diff_vec的模会很小, 为了不干扰匹配, 返回0
     if np.sqrt(gps_diff_vec[0] ** 2 + gps_diff_vec[1] ** 2) <= omitted_l:
         return 0.0
     else:
         return vector_angle(v1=gps_diff_vec, v2=link_dir_vec)
 
 
-def angle_base_north(v: np.ndarray = None):
-    angle = vector_angle(v, np.array([0, 1]))
-    if v[0] <= 0:
-        return angle
-    else:
-        return 360 - angle
-
-
 def judge_plain_crs(lng: float = None) -> str:
     six_df = pd.DataFrame([(i * 6, 32631 + i) for i in range(-30, 30)],
                           columns=['start_lng', 'plain_crs'])
     res = six_df[lng - six_df['start_lng'] >= 0]['plain_crs'].max()
     return rf'EPSG:{res}'
 
 def judge_plain_crs_based_on_node(node_gdf: gpd.GeoDataFrame = None) -> str:
     mean_x = np.array([geo.x for geo in node_gdf['geometry']]).mean()
     return judge_plain_crs(lng=mean_x)
 
 
+def vec_angle(df: pd.DataFrame or gpd.GeoDataFrame = None, va_dx_field: str = 'gv_dx', va_dy_field: str = 'gv_dy',
+              val_field: str = 'gvl',
+              vb_dx_field: str = 'lv_dx', vb_dy_field: str = 'lv_dy', vbl_field: str = 'lvl'):
+    """
+    change inplace
+    :param df:
+    :param va_dx_field:
+    :param va_dy_field:
+    :param val_field:
+    :param vb_dx_field:
+    :param vb_dy_field:
+    :param vbl_field:
+    :return:
+    """
+    df['cos'] = (df[va_dx_field] * df[vb_dx_field] + df[va_dy_field] * df[vb_dy_field]) / (
+                df[val_field] * df[vbl_field])
+    df.loc[df['cos'] == -np.inf, 'cos'] = np.inf
+    df.loc[df['cos'] <= -1, 'cos'] = -1
+    df.loc[df['cos'] >= 1, 'cos'] = 1
+    df['theta'] = 180 * np.arccos(df['cos']) / np.pi
+    df.loc[df['theta'] >= 179.9, 'theta'] = 179.9
+
+
 if __name__ == '__main__':
     pass
     # import geopandas as gpd
     # import matplotlib.pyplot as plt
     #
     # l = LineString([(0,0), (12, 90)])
     # p = gpd.GeoDataFrame({'geometry': [Point(item) for item in l.coords]}, geometry='geometry')
```

### Comparing `gotrackit-0.2.4/src/gotrackit/tools/group.py` & `gotrackit-0.2.5/src/gotrackit/tools/group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/tools/save_file.py` & `gotrackit-0.2.5/src/gotrackit/tools/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit/visualization.py` & `gotrackit-0.2.5/src/gotrackit/visualization.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.4/src/gotrackit.egg-info/PKG-INFO` & `gotrackit-0.2.5/src/gotrackit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,64 +39,56 @@
 ~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
 
 Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
 </div>
 <br>
 
 
-
-**版本状态：05.07已经更新: v0.2.3**
+**版本状态：05.19即将更新: v0.2.5**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
+- 地图匹配接口效率优化, 相较于v0.2.4小幅度提升
 
-- 地图匹配接口效率优化, 相较于v0.2.2小幅度提升
-
-- 地图匹配接口报错机制优化
-
-- 地图匹配接口移除html_fldr参数, 使用out_fldr替代
-
-- 地图匹配接口增加即时输出开关instant_output, 打开后, 每匹配完一条轨迹马上进行结果存储
-
-- 路网构建: crs判断BUG修复、境外路网构建失败BUG修复
+- 新增网格参数搜索，帮助用户确定合理的匹配参数
 
-- 增加 环路 处理功能
+- BUG修复
 
 
 **不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
 
 
 <br>
 
 <div align=center>
-~ v0.2.4(相较于0.2.1)效率将大幅度提升, 最高可以提升10倍的性能 !~
+~ v0.2.5(相较于0.2.1)效率将大幅度提升, 最高可以提升15倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.4版解算时间 |
+| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.5版解算时间 |
 |----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
-| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.87秒**   |
-| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.89秒**   |
+| 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.35秒**   |
+| 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.60秒**   |
 
 
-v0.2.4多核效率对比:
+v0.2.5多核效率对比:
 
-基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快89s解算完150条轨迹，平均每条轨迹0.59s，相较于0.89s再次提升了30%，在车辆数较多时，多核的效率提升很明显。
+基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快71s解算完150条轨迹，平均每条轨迹0.47s，相较于0.60s再次提升了20%，在车辆数较多时，多核的效率提升很明显。
 
 | 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.4解算时间 |
 |-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
-| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 290.0秒     | 
-| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 130.6秒     |
-| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 113.3秒     |
-| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 97.3秒      | 
-| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 89.4秒      | 
-| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 91.5秒      | 
+| 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 226.0秒     | 
+| 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 101.6秒     |
+| 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 88.3秒      |
+| 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 75.3秒      | 
+| 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 72.1秒      | 
+| 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 71.5秒      | 
 
 
 <br>
 
 <div align=center>
 ~ 稀疏轨迹匹配与路径补全 ~
 </div>
```

### Comparing `gotrackit-0.2.4/src/gotrackit.egg-info/SOURCES.txt` & `gotrackit-0.2.5/src/gotrackit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/gotrackit/gps/LocGps.py
 src/gotrackit/gps/__init__.py
 src/gotrackit/map/Link.py
 src/gotrackit/map/Net.py
 src/gotrackit/map/Node.py
 src/gotrackit/map/__init__.py
 src/gotrackit/model/Markov.py
+src/gotrackit/model/Para.py
 src/gotrackit/model/__init__.py
 src/gotrackit/netreverse/GlobalVal.py
 src/gotrackit/netreverse/NetGen.py
 src/gotrackit/netreverse/__init__.py
 src/gotrackit/netreverse/book_mark.py
 src/gotrackit/netreverse/format_od.py
 src/gotrackit/netreverse/Parse/__init__.py
```

