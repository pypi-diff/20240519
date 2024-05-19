# Comparing `tmp/gotrackit-0.2.5.tar.gz` & `tmp/gotrackit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrackit-0.2.5.tar", last modified: Sun May 19 13:48:06 2024, max compression
+gzip compressed data, was "gotrackit-0.2.6.tar", last modified: Sun May 19 15:17:35 2024, max compression
```

## Comparing `gotrackit-0.2.5.tar` & `gotrackit-0.2.6.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.978852 gotrackit-0.2.5/
--rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     7735 2024-05-19 13:48:06.978852 gotrackit-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     6989 2024-05-19 09:06:23.000000 gotrackit-0.2.5/README.md
--rw-rw-rw-   0        0        0      795 2024-05-18 04:37:45.000000 gotrackit-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-19 13:48:06.978852 gotrackit-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.888421 gotrackit-0.2.5/src/
--rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.896423 gotrackit-0.2.5/src/gotrackit/
--rw-rw-rw-   0        0        0    16059 2024-05-17 07:53:49.000000 gotrackit-0.2.5/src/gotrackit/GlobalVal.py
--rw-rw-rw-   0        0        0    17442 2024-05-19 09:31:55.000000 gotrackit-0.2.5/src/gotrackit/MapMatch.py
--rw-rw-rw-   0        0        0      624 2024-05-18 04:36:05.000000 gotrackit-0.2.5/src/gotrackit/WrapsFunc.py
--rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.5/src/gotrackit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.900422 gotrackit-0.2.5/src/gotrackit/generation/
--rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.5/src/gotrackit/generation/GpsGen.py
--rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.5/src/gotrackit/generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.904421 gotrackit-0.2.5/src/gotrackit/gps/
--rw-rw-rw-   0        0        0     4241 2024-05-19 13:01:14.000000 gotrackit-0.2.5/src/gotrackit/gps/GpsArray.py
--rw-rw-rw-   0        0        0     8021 2024-05-19 13:01:14.000000 gotrackit-0.2.5/src/gotrackit/gps/GpsTrip.py
--rw-rw-rw-   0        0        0     3896 2024-04-30 05:17:12.000000 gotrackit-0.2.5/src/gotrackit/gps/GpsXfer.py
--rw-rw-rw-   0        0        0    21654 2024-05-19 13:34:52.000000 gotrackit-0.2.5/src/gotrackit/gps/LocGps.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.5/src/gotrackit/gps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.913588 gotrackit-0.2.5/src/gotrackit/map/
--rw-rw-rw-   0        0        0    20406 2024-05-17 07:59:43.000000 gotrackit-0.2.5/src/gotrackit/map/Link.py
--rw-rw-rw-   0        0        0    40402 2024-05-17 08:31:42.000000 gotrackit-0.2.5/src/gotrackit/map/Net.py
--rw-rw-rw-   0        0        0     4848 2024-05-18 04:12:21.000000 gotrackit-0.2.5/src/gotrackit/map/Node.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.5/src/gotrackit/map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.917016 gotrackit-0.2.5/src/gotrackit/model/
--rw-rw-rw-   0        0        0    59444 2024-05-19 10:05:45.000000 gotrackit-0.2.5/src/gotrackit/model/Markov.py
--rw-rw-rw-   0        0        0     2441 2024-05-19 12:17:01.000000 gotrackit-0.2.5/src/gotrackit/model/Para.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.5/src/gotrackit/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.921018 gotrackit-0.2.5/src/gotrackit/netreverse/
--rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.5/src/gotrackit/netreverse/GlobalVal.py
--rw-rw-rw-   0        0        0    27460 2024-05-08 15:05:30.000000 gotrackit-0.2.5/src/gotrackit/netreverse/NetGen.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.921018 gotrackit-0.2.5/src/gotrackit/netreverse/Parse/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Parse/__init__.py
--rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Parse/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.929018 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/
--rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/GeoProcess.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/GraphAna.py
--rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/IndexAna.py
--rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/MapProcess.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/od.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.929018 gotrackit-0.2.5/src/gotrackit/netreverse/Request/
--rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.933019 gotrackit-0.2.5/src/gotrackit/netreverse/Request/api/
--rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/api/WebApi.py
--rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/api/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/request_path.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.937018 gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/
--rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/__init__.py
--rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/bd_ts.py
--rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.941018 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.945019 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/DupProcess/
--rw-rw-rw-   0        0        0    21741 2024-05-08 08:28:07.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.949019 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/
--rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
--rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.953022 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    12237 2024-05-08 09:22:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
--rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.953022 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
--rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.962696 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    21567 2024-05-08 09:34:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.964854 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/SaveStreets/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
--rw-rw-rw-   0        0        0    22373 2024-05-18 04:15:30.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.964854 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Split/
--rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Split/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.968885 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Tools/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
--rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Tools/process.py
--rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/__init__.py
--rw-rw-rw-   0        0        0     9629 2024-05-10 08:28:49.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/conn.py
--rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/increment.py
--rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/net_reverse.py
--rw-rw-rw-   0        0        0     5790 2024-05-08 09:34:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/optimize_net.py
--rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/save_file.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.5/src/gotrackit/netreverse/__init__.py
--rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.5/src/gotrackit/netreverse/book_mark.py
--rw-rw-rw-   0        0        0     1872 2024-05-08 09:34:18.000000 gotrackit-0.2.5/src/gotrackit/netreverse/format_od.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.968885 gotrackit-0.2.5/src/gotrackit/netxfer/
--rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.5/src/gotrackit/netxfer/SumoConvert.py
--rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.5/src/gotrackit/netxfer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.973405 gotrackit-0.2.5/src/gotrackit/solver/
--rw-rw-rw-   0        0        0     9156 2024-05-07 23:25:32.000000 gotrackit-0.2.5/src/gotrackit/solver/Viterbi.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.5/src/gotrackit/solver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.978852 gotrackit-0.2.5/src/gotrackit/tools/
--rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.5/src/gotrackit/tools/__init__.py
--rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.5/src/gotrackit/tools/coord_trans.py
--rw-rw-rw-   0        0        0    12569 2024-05-17 05:28:38.000000 gotrackit-0.2.5/src/gotrackit/tools/geo_process.py
--rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.5/src/gotrackit/tools/group.py
--rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.5/src/gotrackit/tools/save_file.py
--rw-rw-rw-   0        0        0    10550 2024-05-07 01:39:06.000000 gotrackit-0.2.5/src/gotrackit/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:48:06.978852 gotrackit-0.2.5/src/gotrackit.egg-info/
--rw-rw-rw-   0        0        0     7735 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3723 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-19 13:48:06.000000 gotrackit-0.2.5/src/gotrackit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.869109 gotrackit-0.2.6/
+-rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     7732 2024-05-19 15:17:35.869109 gotrackit-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6986 2024-05-19 15:13:23.000000 gotrackit-0.2.6/README.md
+-rw-rw-rw-   0        0        0      795 2024-05-19 15:13:23.000000 gotrackit-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 15:17:35.873109 gotrackit-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.794503 gotrackit-0.2.6/src/
+-rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.802309 gotrackit-0.2.6/src/gotrackit/
+-rw-rw-rw-   0        0        0    16111 2024-05-19 14:54:43.000000 gotrackit-0.2.6/src/gotrackit/GlobalVal.py
+-rw-rw-rw-   0        0        0    17442 2024-05-19 09:31:55.000000 gotrackit-0.2.6/src/gotrackit/MapMatch.py
+-rw-rw-rw-   0        0        0      624 2024-05-18 04:36:05.000000 gotrackit-0.2.6/src/gotrackit/WrapsFunc.py
+-rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.6/src/gotrackit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.807295 gotrackit-0.2.6/src/gotrackit/generation/
+-rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.6/src/gotrackit/generation/GpsGen.py
+-rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.6/src/gotrackit/generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.811284 gotrackit-0.2.6/src/gotrackit/gps/
+-rw-rw-rw-   0        0        0     4241 2024-05-19 13:01:14.000000 gotrackit-0.2.6/src/gotrackit/gps/GpsArray.py
+-rw-rw-rw-   0        0        0     8021 2024-05-19 13:01:14.000000 gotrackit-0.2.6/src/gotrackit/gps/GpsTrip.py
+-rw-rw-rw-   0        0        0     3896 2024-04-30 05:17:12.000000 gotrackit-0.2.6/src/gotrackit/gps/GpsXfer.py
+-rw-rw-rw-   0        0        0    21654 2024-05-19 13:34:52.000000 gotrackit-0.2.6/src/gotrackit/gps/LocGps.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.6/src/gotrackit/gps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.816271 gotrackit-0.2.6/src/gotrackit/map/
+-rw-rw-rw-   0        0        0    20406 2024-05-17 07:59:43.000000 gotrackit-0.2.6/src/gotrackit/map/Link.py
+-rw-rw-rw-   0        0        0    40402 2024-05-17 08:31:42.000000 gotrackit-0.2.6/src/gotrackit/map/Net.py
+-rw-rw-rw-   0        0        0     4848 2024-05-18 04:12:21.000000 gotrackit-0.2.6/src/gotrackit/map/Node.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.6/src/gotrackit/map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.818266 gotrackit-0.2.6/src/gotrackit/model/
+-rw-rw-rw-   0        0        0    59696 2024-05-19 15:12:13.000000 gotrackit-0.2.6/src/gotrackit/model/Markov.py
+-rw-rw-rw-   0        0        0     2441 2024-05-19 15:08:25.000000 gotrackit-0.2.6/src/gotrackit/model/Para.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.6/src/gotrackit/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.822701 gotrackit-0.2.6/src/gotrackit/netreverse/
+-rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.6/src/gotrackit/netreverse/GlobalVal.py
+-rw-rw-rw-   0        0        0    27460 2024-05-08 15:05:30.000000 gotrackit-0.2.6/src/gotrackit/netreverse/NetGen.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.823698 gotrackit-0.2.6/src/gotrackit/netreverse/Parse/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/Parse/__init__.py
+-rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.6/src/gotrackit/netreverse/Parse/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.828717 gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/
+-rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/GeoProcess.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/GraphAna.py
+-rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/IndexAna.py
+-rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/MapProcess.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/od.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.828717 gotrackit-0.2.6/src/gotrackit/netreverse/Request/
+-rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.6/src/gotrackit/netreverse/Request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.828717 gotrackit-0.2.6/src/gotrackit/netreverse/Request/api/
+-rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.6/src/gotrackit/netreverse/Request/api/WebApi.py
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.6/src/gotrackit/netreverse/Request/api/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.6/src/gotrackit/netreverse/Request/request_path.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.832716 gotrackit-0.2.6/src/gotrackit/netreverse/Request/usage/
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.6/src/gotrackit/netreverse/Request/usage/__init__.py
+-rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.6/src/gotrackit/netreverse/Request/usage/bd_ts.py
+-rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.6/src/gotrackit/netreverse/Request/usage/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.837107 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.841109 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/DupProcess/
+-rw-rw-rw-   0        0        0    21741 2024-05-08 08:28:07.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.845109 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/
+-rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
+-rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.849109 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    12237 2024-05-08 09:22:18.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
+-rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.849109 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
+-rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.853109 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    21567 2024-05-08 09:34:18.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.857109 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/SaveStreets/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
+-rw-rw-rw-   0        0        0    22373 2024-05-18 04:15:30.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.857109 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Split/
+-rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Split/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.861109 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Tools/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
+-rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Tools/process.py
+-rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/__init__.py
+-rw-rw-rw-   0        0        0     9629 2024-05-10 08:28:49.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/conn.py
+-rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/increment.py
+-rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/net_reverse.py
+-rw-rw-rw-   0        0        0     5790 2024-05-08 09:34:18.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/optimize_net.py
+-rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/save_file.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.6/src/gotrackit/netreverse/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.6/src/gotrackit/netreverse/book_mark.py
+-rw-rw-rw-   0        0        0     1872 2024-05-08 09:34:18.000000 gotrackit-0.2.6/src/gotrackit/netreverse/format_od.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.861109 gotrackit-0.2.6/src/gotrackit/netxfer/
+-rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.6/src/gotrackit/netxfer/SumoConvert.py
+-rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.6/src/gotrackit/netxfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.861109 gotrackit-0.2.6/src/gotrackit/solver/
+-rw-rw-rw-   0        0        0     9156 2024-05-07 23:25:32.000000 gotrackit-0.2.6/src/gotrackit/solver/Viterbi.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.6/src/gotrackit/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.869109 gotrackit-0.2.6/src/gotrackit/tools/
+-rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.6/src/gotrackit/tools/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.6/src/gotrackit/tools/coord_trans.py
+-rw-rw-rw-   0        0        0    12569 2024-05-17 05:28:38.000000 gotrackit-0.2.6/src/gotrackit/tools/geo_process.py
+-rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.6/src/gotrackit/tools/group.py
+-rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.6/src/gotrackit/tools/save_file.py
+-rw-rw-rw-   0        0        0    10550 2024-05-07 01:39:06.000000 gotrackit-0.2.6/src/gotrackit/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:17:35.869109 gotrackit-0.2.6/src/gotrackit.egg-info/
+-rw-rw-rw-   0        0        0     7732 2024-05-19 15:17:35.000000 gotrackit-0.2.6/src/gotrackit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3723 2024-05-19 15:17:35.000000 gotrackit-0.2.6/src/gotrackit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 15:17:35.000000 gotrackit-0.2.6/src/gotrackit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-19 15:17:35.000000 gotrackit-0.2.6/src/gotrackit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-19 15:17:35.000000 gotrackit-0.2.6/src/gotrackit.egg-info/top_level.txt
```

### Comparing `gotrackit-0.2.5/LICENSE` & `gotrackit-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/PKG-INFO` & `gotrackit-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 ~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
 
 Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
 </div>
 <br>
 
 
-**版本状态：05.19即将更新: v0.2.5**
+**版本状态：05.19已更新: v0.2.6**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
 - 地图匹配接口效率优化, 相较于v0.2.4小幅度提升
 
 - 新增网格参数搜索，帮助用户确定合理的匹配参数
 
@@ -56,32 +56,32 @@
 
 **不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
 
 
 <br>
 
 <div align=center>
-~ v0.2.5(相较于0.2.1)效率将大幅度提升, 最高可以提升15倍的性能 !~
+~ v0.2.6(相较于0.2.1)效率将大幅度提升, 最高可以提升20倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.5版解算时间 |
+| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.6版解算时间 |
 |----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
 | 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.35秒**   |
 | 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.60秒**   |
 
 
-v0.2.5多核效率对比:
+v0.2.6多核效率对比:
 
 基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快71s解算完150条轨迹，平均每条轨迹0.47s，相较于0.60s再次提升了20%，在车辆数较多时，多核的效率提升很明显。
 
-| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.4解算时间 |
+| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.6解算时间 |
 |-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
 | 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 226.0秒     | 
 | 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 101.6秒     |
 | 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 88.3秒      |
 | 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 75.3秒      | 
 | 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 72.1秒      | 
 | 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 71.5秒      |
```

### Comparing `gotrackit-0.2.5/README.md` & `gotrackit-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
 
 Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
 </div>
 <br>
 
 
-**版本状态：05.19即将更新: v0.2.5**
+**版本状态：05.19已更新: v0.2.6**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
 - 地图匹配接口效率优化, 相较于v0.2.4小幅度提升
 
 - 新增网格参数搜索，帮助用户确定合理的匹配参数
 
@@ -34,32 +34,32 @@
 
 **不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
 
 
 <br>
 
 <div align=center>
-~ v0.2.5(相较于0.2.1)效率将大幅度提升, 最高可以提升15倍的性能 !~
+~ v0.2.6(相较于0.2.1)效率将大幅度提升, 最高可以提升20倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.5版解算时间 |
+| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.6版解算时间 |
 |----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
 | 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.35秒**   |
 | 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.60秒**   |
 
 
-v0.2.5多核效率对比:
+v0.2.6多核效率对比:
 
 基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快71s解算完150条轨迹，平均每条轨迹0.47s，相较于0.60s再次提升了20%，在车辆数较多时，多核的效率提升很明显。
 
-| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.4解算时间 |
+| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.6解算时间 |
 |-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
 | 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 226.0秒     | 
 | 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 101.6秒     |
 | 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 88.3秒      |
 | 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 75.3秒      | 
 | 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 72.1秒      | 
 | 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 71.5秒      |
```

### Comparing `gotrackit-0.2.5/pyproject.toml` & `gotrackit-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotrackit"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = ["geopandas>=0.14.1", "shapely", "networkx", "pandas", "numpy", "keplergl", "geopy"]
 requires-python = ">=3.8"
 authors = [
   { name="Kai Tang", email="794568794@qq.com" },
 ]
 description = "A Python Package for Map Matching Algorithm Based on Hidden Markov Model"
 readme = "README.md"
```

### Comparing `gotrackit-0.2.5/src/gotrackit/GlobalVal.py` & `gotrackit-0.2.6/src/gotrackit/GlobalVal.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         self.ROUTE_ITEM = 'route_item'
         self.STRAIGHT_LENGTH = 'straight_l'
         self.DIS_GAP = 'dis_gap'
         self.PRJ_L = 'prj_dis'
         self.PRJ_GEO = 'prj_p'
         self.DIS_TO_NEXT = 'dis_to_next'
         self.HEADING_GAP = 'heading_gap'
+        self.USED_HEADING_GAP = 'used_heading_gap'
         self.EMISSION_P = 'emission_p'
 
 
 class KeplerConfig(object):
     def __init__(self):
         self.__BASE_CONFIG = {
             'version': 'v1',
```

### Comparing `gotrackit-0.2.5/src/gotrackit/MapMatch.py` & `gotrackit-0.2.6/src/gotrackit/MapMatch.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/WrapsFunc.py` & `gotrackit-0.2.6/src/gotrackit/WrapsFunc.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/generation/GpsGen.py` & `gotrackit-0.2.6/src/gotrackit/generation/GpsGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/gps/GpsArray.py` & `gotrackit-0.2.6/src/gotrackit/gps/GpsArray.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/gps/GpsTrip.py` & `gotrackit-0.2.6/src/gotrackit/gps/GpsTrip.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/gps/GpsXfer.py` & `gotrackit-0.2.6/src/gotrackit/gps/GpsXfer.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/gps/LocGps.py` & `gotrackit-0.2.6/src/gotrackit/gps/LocGps.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/map/Link.py` & `gotrackit-0.2.6/src/gotrackit/map/Link.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/map/Net.py` & `gotrackit-0.2.6/src/gotrackit/map/Net.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/map/Node.py` & `gotrackit-0.2.6/src/gotrackit/map/Node.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/model/Markov.py` & `gotrackit-0.2.6/src/gotrackit/model/Markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,30 +204,33 @@
                                               how='left',
                                               on=gps_field.POINT_SEQ_FIELD)
 
                 vec_angle(df=self.__done_prj_df)
                 if markov_field.HEADING_GAP in self.__done_prj_df.columns:
                     del self.__done_prj_df[markov_field.HEADING_GAP]
                 self.__done_prj_df.rename(columns={'theta': markov_field.HEADING_GAP}, inplace=True)
-
-            self.__done_prj_df.loc[self.__done_prj_df[gps_field.VEC_LEN] <= omitted_l, markov_field.HEADING_GAP] = 0
+            self.__done_prj_df[markov_field.USED_HEADING_GAP] = self.__done_prj_df[markov_field.HEADING_GAP]
+            self.__done_prj_df.loc[
+                self.__done_prj_df[gps_field.VEC_LEN] <= omitted_l, markov_field.USED_HEADING_GAP] = 0
 
         else:
-            self.__done_prj_df[markov_field.HEADING_GAP] = 0
+            self.__done_prj_df[markov_field.USED_HEADING_GAP] = 0
 
-        self.__done_prj_df[markov_field.HEADING_GAP] = self.__done_prj_df[markov_field.HEADING_GAP].astype(object)
+        self.__done_prj_df[markov_field.USED_HEADING_GAP] = \
+            self.__done_prj_df[markov_field.USED_HEADING_GAP].astype(object)
         self.__done_prj_df[markov_field.PRJ_L] = self.__done_prj_df[markov_field.PRJ_L].astype(object)
 
         emission_p_df = self.__done_prj_df.groupby(gps_field.POINT_SEQ_FIELD).agg(
-            {markov_field.PRJ_L: np.array, markov_field.HEADING_GAP: np.array}).reset_index(
+            {markov_field.PRJ_L: np.array, markov_field.USED_HEADING_GAP: np.array}).reset_index(
             drop=False)
         self.__emission_mat_dict = {
             int(row[gps_field.POINT_SEQ_FIELD]): self.emission_probability(dis=row[markov_field.PRJ_L],
                                                                            sigma=gps_sigma,
-                                                                           heading_gap=row[markov_field.HEADING_GAP])
+                                                                           heading_gap=row[
+                                                                               markov_field.USED_HEADING_GAP])
             for _, row in
             emission_p_df.iterrows()}
 
     def __generate_candidates(self) -> list[int]:
         # 初步依据gps点buffer得到候选路段, 关联不到的GPS点删除掉
         # seq, geometry, single_link_id, from_node, to_node, dir, length
         gps_candidate_link, _gap = self.gps_points.generate_candidate_link(net=self.net)
```

### Comparing `gotrackit-0.2.5/src/gotrackit/model/Para.py` & `gotrackit-0.2.6/src/gotrackit/model/Para.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/GlobalVal.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/NetGen.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/NetGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/Parse/gd_car_path.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/Parse/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/GeoProcess.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/GraphAna.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/GraphAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/IndexAna.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/IndexAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/PublicTools/od.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/PublicTools/od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/Request/api/WebApi.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/Request/api/WebApi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/Request/request_path.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/Request/request_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/bd_ts.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/Request/usage/bd_ts.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/Request/usage/gd_car_path.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/Request/usage/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/Tools/process.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/Tools/process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/conn.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/conn.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/increment.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/increment.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/net_reverse.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/net_reverse.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/optimize_net.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/optimize_net.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/RoadNet/save_file.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/RoadNet/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/book_mark.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/book_mark.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netreverse/format_od.py` & `gotrackit-0.2.6/src/gotrackit/netreverse/format_od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/netxfer/SumoConvert.py` & `gotrackit-0.2.6/src/gotrackit/netxfer/SumoConvert.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/solver/Viterbi.py` & `gotrackit-0.2.6/src/gotrackit/solver/Viterbi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/tools/coord_trans.py` & `gotrackit-0.2.6/src/gotrackit/tools/coord_trans.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/tools/geo_process.py` & `gotrackit-0.2.6/src/gotrackit/tools/geo_process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/tools/group.py` & `gotrackit-0.2.6/src/gotrackit/tools/group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/tools/save_file.py` & `gotrackit-0.2.6/src/gotrackit/tools/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit/visualization.py` & `gotrackit-0.2.6/src/gotrackit/visualization.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.5/src/gotrackit.egg-info/PKG-INFO` & `gotrackit-0.2.6/src/gotrackit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 ~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
 
 Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
 </div>
 <br>
 
 
-**版本状态：05.19即将更新: v0.2.5**
+**版本状态：05.19已更新: v0.2.6**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
 - 地图匹配接口效率优化, 相较于v0.2.4小幅度提升
 
 - 新增网格参数搜索，帮助用户确定合理的匹配参数
 
@@ -56,32 +56,32 @@
 
 **不要下载GitHub仓库上的代码来使用!!!  直接pip安装gotrackit为第三方库即可使用**
 
 
 <br>
 
 <div align=center>
-~ v0.2.5(相较于0.2.1)效率将大幅度提升, 最高可以提升15倍的性能 !~
+~ v0.2.6(相较于0.2.1)效率将大幅度提升, 最高可以提升20倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
-| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.5版解算时间 |
+| 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.6版解算时间 |
 |----------------|----------|----------------|------------------|---------|------------|-------------|-------------|
 | 1辆车,深圳稀疏轨迹点样例1 | 190      | 60             | 500m             | 10615 | 629788次 | 28秒         | **1.35秒**   |
 | 1辆车,深圳稀疏轨迹点样例2 | 400      | 20             | 120m             | 5137 | 82006次  | 7.8秒        | **0.60秒**   |
 
 
-v0.2.5多核效率对比:
+v0.2.6多核效率对比:
 
 基于上表深圳稀疏轨迹点样例2，我们将他复制150份，进行多核测试，可以看到到6核时, 效率已经不再提升，最快71s解算完150条轨迹，平均每条轨迹0.47s，相较于0.60s再次提升了20%，在车辆数较多时，多核的效率提升很明显。
 
-| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.4解算时间 |
+| 样例数据                                      | 有效的GPS点数 | top_k | gps_buffer | 候选路段条数 | 状态转移次数 | v0.2.6解算时间 |
 |-------------------------------------------|----------|----------------|------------------|-----|--------|------------|
 | 150辆车的GPS轨迹(单核串行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 226.0秒     | 
 | 150辆车的GPS轨迹(3核并行,子图搜索,有构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 101.6秒     |
 | 150辆车的GPS轨迹(3核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 88.3秒      |
 | 150辆车的GPS轨迹(4核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 75.3秒      | 
 | 150辆车的GPS轨迹(5核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 72.1秒      | 
 | 150辆车的GPS轨迹(6核并行,全图搜索,无构建子图的额外开销,提前预计算路径) | 6w       | 20             | 120m             | 75W | 1200W次 | 71.5秒      |
```

### Comparing `gotrackit-0.2.5/src/gotrackit.egg-info/SOURCES.txt` & `gotrackit-0.2.6/src/gotrackit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

