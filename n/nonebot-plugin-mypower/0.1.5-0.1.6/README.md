# Comparing `tmp/nonebot_plugin_mypower-0.1.5.tar.gz` & `tmp/nonebot_plugin_mypower-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mypower-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_mypower-0.1.6.tar", max compression
```

## Comparing `nonebot_plugin_mypower-0.1.5.tar` & `nonebot_plugin_mypower-0.1.6.tar`

### file list

```diff
@@ -1,115 +1,139 @@
--rw-r--r--   0        0        0     2806 2024-01-15 01:41:26.996249 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/__init__.py
--rw-r--r--   0        0        0     8851 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/1.png
--rw-r--r--   0        0        0     8688 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/10.png
--rw-r--r--   0        0        0     9675 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/11.png
--rw-r--r--   0        0        0     8679 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/12.png
--rw-r--r--   0        0        0     9492 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/13.png
--rw-r--r--   0        0        0     8030 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/14.png
--rw-r--r--   0        0        0    10570 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/15.png
--rw-r--r--   0        0        0     8845 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/2.png
--rw-r--r--   0        0        0     9160 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/3.png
--rw-r--r--   0        0        0     9641 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/4.png
--rw-r--r--   0        0        0     8595 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/5.png
--rw-r--r--   0        0        0     8889 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/6.png
--rw-r--r--   0        0        0     9898 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/7.png
--rw-r--r--   0        0        0     8177 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/8.png
--rw-r--r--   0        0        0     8747 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/9.png
--rw-r--r--   0        0        0    64169 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/1.png
--rw-r--r--   0        0        0    94913 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/10.png
--rw-r--r--   0        0        0    88794 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/11.png
--rw-r--r--   0        0        0    85178 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/12.png
--rw-r--r--   0        0        0   108125 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/13.png
--rw-r--r--   0        0        0   107557 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/14.png
--rw-r--r--   0        0        0    78325 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/15.png
--rw-r--r--   0        0        0   103295 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/16.png
--rw-r--r--   0        0        0   125428 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/17.png
--rw-r--r--   0        0        0    87658 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/18.png
--rw-r--r--   0        0        0    56332 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/19.png
--rw-r--r--   0        0        0   110907 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/2.png
--rw-r--r--   0        0        0    87303 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/20.png
--rw-r--r--   0        0        0   123028 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/21.png
--rw-r--r--   0        0        0    76915 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/22.png
--rw-r--r--   0        0        0    62607 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/23.png
--rw-r--r--   0        0        0    49090 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/3.png
--rw-r--r--   0        0        0    82797 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/4.png
--rw-r--r--   0        0        0    99560 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/5.png
--rw-r--r--   0        0        0   110384 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/6.png
--rw-r--r--   0        0        0    74445 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/7.png
--rw-r--r--   0        0        0   110444 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/8.png
--rw-r--r--   0        0        0    86291 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/9.png
--rw-r--r--   0        0        0    20066 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/1.png
--rw-r--r--   0        0        0    12483 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/10.png
--rw-r--r--   0        0        0    14184 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/11.png
--rw-r--r--   0        0        0    12512 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/12.png
--rw-r--r--   0        0        0    23140 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/13.png
--rw-r--r--   0        0        0    14826 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/14.png
--rw-r--r--   0        0        0    13337 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/15.png
--rw-r--r--   0        0        0    31074 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/16.png
--rw-r--r--   0        0        0    10643 2024-01-15 13:40:43.473515 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/17.png
--rw-r--r--   0        0        0     8211 2024-01-15 13:42:00.324118 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/18.png
--rw-r--r--   0        0        0     7781 2024-01-15 13:42:48.623416 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/19.png
--rw-r--r--   0        0        0    24340 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/2.png
--rw-r--r--   0        0        0     8655 2024-01-15 13:48:33.173155 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/20.png
--rw-r--r--   0        0        0     8712 2024-01-15 13:49:00.824863 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/21.png
--rw-r--r--   0        0        0    12723 2024-01-15 13:49:51.826151 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/22.png
--rw-r--r--   0        0        0     9378 2024-01-15 13:50:39.432552 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/23.png
--rw-r--r--   0        0        0     8664 2024-01-15 13:52:40.458189 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/24.png
--rw-r--r--   0        0        0     8338 2024-01-15 13:53:21.514374 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/25.png
--rw-r--r--   0        0        0     8607 2024-01-15 13:53:54.508266 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/26.png
--rw-r--r--   0        0        0    11415 2024-01-15 13:55:44.092972 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/27.png
--rw-r--r--   0        0        0    12125 2024-01-15 13:57:50.643228 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/28.png
--rw-r--r--   0        0        0    16156 2024-01-15 13:58:54.597772 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/29.png
--rw-r--r--   0        0        0    20174 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/3.png
--rw-r--r--   0        0        0    11942 2024-01-15 13:59:42.905989 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/30.png
--rw-r--r--   0        0        0    13254 2024-01-15 14:00:39.324416 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/31.png
--rw-r--r--   0        0        0     7865 2024-01-15 14:02:06.702564 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/32.png
--rw-r--r--   0        0        0     8633 2024-01-15 14:02:46.199622 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/33.png
--rw-r--r--   0        0        0    19669 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/4.png
--rw-r--r--   0        0        0    13775 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/5.png
--rw-r--r--   0        0        0    16514 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/6.png
--rw-r--r--   0        0        0    20812 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/7.png
--rw-r--r--   0        0        0    15365 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/8.png
--rw-r--r--   0        0        0    11635 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/9.png
--rw-r--r--   0        0        0    14620 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/1.png
--rw-r--r--   0        0        0    20156 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/10.png
--rw-r--r--   0        0        0    21646 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/11.png
--rw-r--r--   0        0        0    22305 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/12.png
--rw-r--r--   0        0        0    16265 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/13.png
--rw-r--r--   0        0        0    17460 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/14.png
--rw-r--r--   0        0        0    15607 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/15.png
--rw-r--r--   0        0        0    22806 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/16.png
--rw-r--r--   0        0        0    22501 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/17.png
--rw-r--r--   0        0        0    16388 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/18.png
--rw-r--r--   0        0        0    22004 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/19.png
--rw-r--r--   0        0        0    21515 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/2.png
--rw-r--r--   0        0        0    20894 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/20.png
--rw-r--r--   0        0        0    17034 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/21.png
--rw-r--r--   0        0        0    20214 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/22.png
--rw-r--r--   0        0        0    17960 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/23.png
--rw-r--r--   0        0        0    11409 2024-01-15 13:06:32.656674 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/24.png
--rw-r--r--   0        0        0    12112 2024-01-15 13:07:47.393356 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/25.png
--rw-r--r--   0        0        0    11160 2024-01-15 13:08:53.049656 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/26.png
--rw-r--r--   0        0        0    13617 2024-01-15 13:11:20.330765 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/27.png
--rw-r--r--   0        0        0    11529 2024-01-15 13:12:25.426092 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/28.png
--rw-r--r--   0        0        0    10649 2024-01-15 13:13:18.064166 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/29.png
--rw-r--r--   0        0        0    28491 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/3.png
--rw-r--r--   0        0        0    14421 2024-01-15 13:14:02.638150 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/30.png
--rw-r--r--   0        0        0    14815 2024-01-15 13:15:29.721522 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/31.png
--rw-r--r--   0        0        0    17430 2024-01-15 13:16:31.894425 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/32.png
--rw-r--r--   0        0        0    16039 2024-01-15 13:22:04.774265 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/33.png
--rw-r--r--   0        0        0    16759 2024-01-15 13:23:39.126855 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/34.png
--rw-r--r--   0        0        0    14763 2024-01-15 13:26:54.506339 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/35.png
--rw-r--r--   0        0        0    16908 2024-01-15 13:28:24.869451 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/36.png
--rw-r--r--   0        0        0    14034 2024-01-15 13:29:52.905374 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/37.png
--rw-r--r--   0        0        0    15458 2024-01-15 13:31:37.229365 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/38.png
--rw-r--r--   0        0        0    10355 2024-01-15 13:35:07.743013 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/39.png
--rw-r--r--   0        0        0    29406 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/4.png
--rw-r--r--   0        0        0    12351 2024-01-15 13:38:25.202767 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/40.png
--rw-r--r--   0        0        0    19007 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/5.png
--rw-r--r--   0        0        0    17415 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/6.png
--rw-r--r--   0        0        0    18470 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/7.png
--rw-r--r--   0        0        0    15485 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/8.png
--rw-r--r--   0        0        0    19568 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/9.png
--rw-r--r--   0        0        0      625 2024-01-15 16:28:37.099716 nonebot_plugin_mypower-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1954 2024-01-15 16:16:07.517849 nonebot_plugin_mypower-0.1.5/README.md
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 nonebot_plugin_mypower-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-22 00:47:21.000000 nonebot_plugin_mypower-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2894 2024-05-19 11:22:34.732337 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/__init__.py
+-rw-r--r--   0        0        0     8851 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/1.png
+-rw-r--r--   0        0        0     8688 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/10.png
+-rw-r--r--   0        0        0     9675 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/11.png
+-rw-r--r--   0        0        0     8679 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/12.png
+-rw-r--r--   0        0        0     9492 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/13.png
+-rw-r--r--   0        0        0     8030 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/14.png
+-rw-r--r--   0        0        0    10570 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/15.png
+-rw-r--r--   0        0        0     8845 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/2.png
+-rw-r--r--   0        0        0     9160 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/3.png
+-rw-r--r--   0        0        0     9641 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/4.png
+-rw-r--r--   0        0        0     8595 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/5.png
+-rw-r--r--   0        0        0     8889 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/6.png
+-rw-r--r--   0        0        0     9898 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/7.png
+-rw-r--r--   0        0        0     8177 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/8.png
+-rw-r--r--   0        0        0     8747 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/9.png
+-rw-r--r--   0        0        0    64169 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/1.png
+-rw-r--r--   0        0        0    94913 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/10.png
+-rw-r--r--   0        0        0    88794 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/11.png
+-rw-r--r--   0        0        0    85178 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/12.png
+-rw-r--r--   0        0        0   108125 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/13.png
+-rw-r--r--   0        0        0   107557 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/14.png
+-rw-r--r--   0        0        0    78325 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/15.png
+-rw-r--r--   0        0        0   103295 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/16.png
+-rw-r--r--   0        0        0   125428 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/17.png
+-rw-r--r--   0        0        0    87658 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/18.png
+-rw-r--r--   0        0        0    56332 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/19.png
+-rw-r--r--   0        0        0   110907 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/2.png
+-rw-r--r--   0        0        0    87303 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/20.png
+-rw-r--r--   0        0        0   123028 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/21.png
+-rw-r--r--   0        0        0    76915 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/22.png
+-rw-r--r--   0        0        0    62607 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/23.png
+-rw-r--r--   0        0        0    49090 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/3.png
+-rw-r--r--   0        0        0    82797 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/4.png
+-rw-r--r--   0        0        0    99560 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/5.png
+-rw-r--r--   0        0        0   110384 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/6.png
+-rw-r--r--   0        0        0    74445 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/7.png
+-rw-r--r--   0        0        0   110444 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/8.png
+-rw-r--r--   0        0        0    86291 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/9.png
+-rw-r--r--   0        0        0    20066 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/1.png
+-rw-r--r--   0        0        0    12483 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/10.png
+-rw-r--r--   0        0        0    14184 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/11.png
+-rw-r--r--   0        0        0    12512 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/12.png
+-rw-r--r--   0        0        0    23140 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/13.png
+-rw-r--r--   0        0        0    14826 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/14.png
+-rw-r--r--   0        0        0    13337 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/15.png
+-rw-r--r--   0        0        0    31074 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/16.png
+-rw-r--r--   0        0        0    10643 2024-01-15 13:40:43.473515 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/17.png
+-rw-r--r--   0        0        0     8211 2024-01-15 13:42:00.324118 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/18.png
+-rw-r--r--   0        0        0     7781 2024-01-15 13:42:48.623416 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/19.png
+-rw-r--r--   0        0        0    24340 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/2.png
+-rw-r--r--   0        0        0     8655 2024-01-15 13:48:33.173155 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/20.png
+-rw-r--r--   0        0        0     8712 2024-01-15 13:49:00.824863 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/21.png
+-rw-r--r--   0        0        0    12723 2024-01-15 13:49:51.826151 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/22.png
+-rw-r--r--   0        0        0     9378 2024-01-15 13:50:39.432552 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/23.png
+-rw-r--r--   0        0        0     8664 2024-01-15 13:52:40.458189 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/24.png
+-rw-r--r--   0        0        0     8338 2024-01-15 13:53:21.514374 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/25.png
+-rw-r--r--   0        0        0     8607 2024-01-15 13:53:54.508266 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/26.png
+-rw-r--r--   0        0        0    11415 2024-01-15 13:55:44.092972 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/27.png
+-rw-r--r--   0        0        0    12125 2024-01-15 13:57:50.643228 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/28.png
+-rw-r--r--   0        0        0    16156 2024-01-15 13:58:54.597772 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/29.png
+-rw-r--r--   0        0        0    20174 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/3.png
+-rw-r--r--   0        0        0    11942 2024-01-15 13:59:42.905989 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/30.png
+-rw-r--r--   0        0        0    13254 2024-01-15 14:00:39.324416 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/31.png
+-rw-r--r--   0        0        0     7865 2024-01-15 14:02:06.702564 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/32.png
+-rw-r--r--   0        0        0     8633 2024-01-15 14:02:46.199622 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/33.png
+-rw-r--r--   0        0        0     9390 2024-03-12 15:33:36.909011 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/34.png
+-rw-r--r--   0        0        0     8070 2024-03-12 15:34:07.317669 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/35.png
+-rw-r--r--   0        0        0     7587 2024-03-12 15:34:27.673095 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/36.png
+-rw-r--r--   0        0        0    14574 2024-03-12 15:36:35.595642 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/37.png
+-rw-r--r--   0        0        0    15852 2024-03-12 15:41:54.849923 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/38.png
+-rw-r--r--   0        0        0    13507 2024-03-12 15:42:21.840791 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/39.png
+-rw-r--r--   0        0        0    19669 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/4.png
+-rw-r--r--   0        0        0    13754 2024-03-12 15:42:45.484715 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/40.png
+-rw-r--r--   0        0        0    13806 2024-03-12 15:43:36.567672 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/41.png
+-rw-r--r--   0        0        0    13775 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/5.png
+-rw-r--r--   0        0        0    16514 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/6.png
+-rw-r--r--   0        0        0    20812 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/7.png
+-rw-r--r--   0        0        0    15365 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/8.png
+-rw-r--r--   0        0        0    11635 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/9.png
+-rw-r--r--   0        0        0    14620 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/1.png
+-rw-r--r--   0        0        0    20156 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/10.png
+-rw-r--r--   0        0        0    21646 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/11.png
+-rw-r--r--   0        0        0    22305 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/12.png
+-rw-r--r--   0        0        0    16265 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/13.png
+-rw-r--r--   0        0        0    17460 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/14.png
+-rw-r--r--   0        0        0    15607 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/15.png
+-rw-r--r--   0        0        0    22806 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/16.png
+-rw-r--r--   0        0        0    22501 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/17.png
+-rw-r--r--   0        0        0    16388 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/18.png
+-rw-r--r--   0        0        0    22004 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/19.png
+-rw-r--r--   0        0        0    21515 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/2.png
+-rw-r--r--   0        0        0    20894 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/20.png
+-rw-r--r--   0        0        0    17034 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/21.png
+-rw-r--r--   0        0        0    20214 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/22.png
+-rw-r--r--   0        0        0    17960 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/23.png
+-rw-r--r--   0        0        0    11409 2024-01-15 13:06:32.656674 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/24.png
+-rw-r--r--   0        0        0    12112 2024-01-15 13:07:47.393356 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/25.png
+-rw-r--r--   0        0        0    11160 2024-01-15 13:08:53.049656 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/26.png
+-rw-r--r--   0        0        0    13617 2024-01-15 13:11:20.330765 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/27.png
+-rw-r--r--   0        0        0    11529 2024-01-15 13:12:25.426092 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/28.png
+-rw-r--r--   0        0        0    10649 2024-01-15 13:13:18.064166 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/29.png
+-rw-r--r--   0        0        0    28491 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/3.png
+-rw-r--r--   0        0        0    14421 2024-01-15 13:14:02.638150 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/30.png
+-rw-r--r--   0        0        0    14815 2024-01-15 13:15:29.721522 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/31.png
+-rw-r--r--   0        0        0    17430 2024-01-15 13:16:31.894425 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/32.png
+-rw-r--r--   0        0        0    16039 2024-01-15 13:22:04.774265 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/33.png
+-rw-r--r--   0        0        0    16759 2024-01-15 13:23:39.126855 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/34.png
+-rw-r--r--   0        0        0    14763 2024-01-15 13:26:54.506339 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/35.png
+-rw-r--r--   0        0        0    16908 2024-01-15 13:28:24.869451 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/36.png
+-rw-r--r--   0        0        0    14034 2024-01-15 13:29:52.905374 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/37.png
+-rw-r--r--   0        0        0    15458 2024-01-15 13:31:37.229365 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/38.png
+-rw-r--r--   0        0        0    10355 2024-01-15 13:35:07.743013 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/39.png
+-rw-r--r--   0        0        0    29406 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/4.png
+-rw-r--r--   0        0        0    12351 2024-01-15 13:38:25.202767 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/40.png
+-rw-r--r--   0        0        0    13723 2024-03-12 15:37:44.358823 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/41.png
+-rw-r--r--   0        0        0    12951 2024-03-12 15:37:59.130558 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/42.png
+-rw-r--r--   0        0        0    11938 2024-03-12 15:38:49.610215 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/43.png
+-rw-r--r--   0        0        0    14514 2024-03-12 15:45:07.228709 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/44.png
+-rw-r--r--   0        0        0    11443 2024-03-12 15:45:59.103719 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/45.png
+-rw-r--r--   0        0        0    11147 2024-03-12 15:46:29.872620 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/46.png
+-rw-r--r--   0        0        0    11406 2024-03-12 15:46:54.055952 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/47.png
+-rw-r--r--   0        0        0    12370 2024-03-12 15:56:20.613819 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/48.png
+-rw-r--r--   0        0        0     8748 2024-03-12 15:59:14.246162 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/49.png
+-rw-r--r--   0        0        0    19007 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/5.png
+-rw-r--r--   0        0        0    10281 2024-03-13 10:51:45.416816 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/50.png
+-rw-r--r--   0        0        0    12290 2024-03-14 08:13:57.864355 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/51.png
+-rw-r--r--   0        0        0    11941 2024-03-14 08:14:31.423179 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/52.png
+-rw-r--r--   0        0        0    10528 2024-03-14 08:15:17.010306 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/53.png
+-rw-r--r--   0        0        0     8811 2024-03-14 08:15:35.559546 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/54.png
+-rw-r--r--   0        0        0    15042 2024-03-14 08:16:37.966484 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/55.png
+-rw-r--r--   0        0        0    17415 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/6.png
+-rw-r--r--   0        0        0    18470 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/7.png
+-rw-r--r--   0        0        0    15485 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/8.png
+-rw-r--r--   0        0        0    19568 2023-11-10 21:04:52.000000 nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/9.png
+-rw-r--r--   0        0        0      596 2024-05-19 11:19:43.160483 nonebot_plugin_mypower-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1954 2024-01-15 16:16:07.517849 nonebot_plugin_mypower-0.1.6/README.md
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 nonebot_plugin_mypower-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/__init__.py` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import random
 from io import BytesIO  # 导入BytesIO
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import MessageSegment
+from nonebot.adapters.onebot.v11 import Bot, MessageSegment, Event
+from nonebot.adapters.onebot.v11.message import Message
 from nonebot.plugin import PluginMetadata
 
 # 元数据
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-mypower",
     description="随机生成超能力",
     usage="我的超能力",
@@ -21,16 +22,15 @@
     pillow_available = True
 except ImportError:
     pillow_available = False
 
 # 命令触发
 my_superpower = on_command('我的超能力', priority=10, block=True)
 
-# 命令触发
-my_superpower = on_command('我的超能力', priority=10, block=True)
+
 
 def create_image(selected_images):
     # 读取第一张图片以确定宽度
     first_image = Image.open(selected_images[0])
     total_width = first_image.width
 
     # 计算总高度并调整图片大小
@@ -50,15 +50,15 @@
     for img in images_to_join:
         new_image.paste(img, (0, current_height))
         current_height += img.height
 
     return new_image
 
 @my_superpower.handle()
-async def _():
+async def _(bot: Bot, event: Event):
     if not pillow_available:
         await my_superpower.send("图片处理功能无法使用，因为Pillow库没有安装。")
         return
 
     folders = ['超能力', '但是', '主义', '万圣节']
     selected_images = []
 
@@ -77,10 +77,11 @@
         # 创建图片并转换为字节流
         new_image = create_image(selected_images)
         img_byte_arr = BytesIO()
         new_image.save(img_byte_arr, format='PNG')
         img_byte_arr.seek(0)
 
         # 发送图片
-        await my_superpower.send(MessageSegment.image(img_byte_arr))
+        await my_superpower.send(MessageSegment.reply(event.message_id) + MessageSegment.image(img_byte_arr))
     except Exception as e:
-        await my_superpower.send(f"图片发送失败: {e}")
+        await my_superpower.send(MessageSegment.reply(event.message_id) + f"图片发送失败: {e}")
+
```

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/1.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/1.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/10.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/10.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/11.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/11.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/12.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/12.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/13.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/13.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/14.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/14.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/15.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/15.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/2.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/2.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/3.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/3.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/4.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/4.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/5.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/5.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/6.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/6.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/7.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/7.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/8.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/8.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/万圣节/9.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/万圣节/9.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/1.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/1.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/10.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/10.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/11.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/11.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/12.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/12.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/13.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/13.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/14.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/14.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/15.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/15.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/16.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/16.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/17.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/17.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/18.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/18.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/19.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/19.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/2.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/2.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/20.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/20.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/21.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/21.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/22.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/22.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/23.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/23.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/3.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/3.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/4.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/4.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/5.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/5.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/6.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/6.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/7.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/7.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/8.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/8.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/主义/9.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/主义/9.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/1.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/1.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/10.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/10.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/11.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/11.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/12.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/12.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/13.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/13.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/14.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/14.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/15.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/15.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/16.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/16.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/17.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/17.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/18.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/18.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/19.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/19.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/2.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/2.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/20.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/20.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/21.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/21.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/22.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/22.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/23.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/23.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/24.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/24.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/25.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/25.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/26.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/26.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/27.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/27.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/28.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/28.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/29.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/29.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/3.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/3.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/30.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/30.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/31.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/31.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/32.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/32.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/33.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/33.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/4.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/4.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/5.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/5.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/6.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/6.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/7.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/7.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/8.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/8.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/但是/9.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/但是/9.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/1.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/1.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/10.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/10.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/11.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/11.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/12.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/12.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/13.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/13.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/14.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/14.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/15.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/15.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/16.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/16.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/17.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/17.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/18.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/18.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/19.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/19.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/2.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/2.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/20.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/20.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/21.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/21.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/22.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/22.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/23.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/23.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/24.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/24.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/25.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/25.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/26.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/26.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/27.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/27.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/28.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/28.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/29.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/29.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/3.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/3.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/30.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/30.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/31.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/31.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/32.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/32.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/33.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/33.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/34.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/34.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/35.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/35.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/36.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/36.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/37.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/37.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/38.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/38.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/39.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/39.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/4.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/4.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/40.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/40.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/5.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/5.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/6.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/6.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/7.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/7.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/8.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/8.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/nonebot_plugin_mypower/超能力/9.png` & `nonebot_plugin_mypower-0.1.6/nonebot_plugin_mypower/超能力/9.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/pyproject.toml` & `nonebot_plugin_mypower-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "nonebot-plugin-mypower"
-version = "0.1.5"
+version = "0.1.6"
 description = "一款随机生成超能力的插件（适用于Onebot V11）"
-authors = ["tianyisama <tianyisama99@gmail.com>"]
+authors = ["TianYi"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tianyisama/nonebot_plugin_mypower"
 repository = "https://github.com/tianyisama/nonebot_plugin_mypower"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_mypower-0.1.5/README.md` & `nonebot_plugin_mypower-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mypower-0.1.5/PKG-INFO` & `nonebot_plugin_mypower-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mypower
-Version: 0.1.5
+Version: 0.1.6
 Summary: 一款随机生成超能力的插件（适用于Onebot V11）
 Home-page: https://github.com/tianyisama/nonebot_plugin_mypower
 License: MIT
-Author: tianyisama
-Author-email: tianyisama99@gmail.com
+Author: TianYi
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mypower Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mypower Version: 0.1.6 Summary:
 ä¸æ¬¾éæºçæè¶è½åçæä»¶ï¼éç¨äºOnebot V11ï¼ Home-page: https:
-//github.com/tianyisama/nonebot_plugin_mypower License: MIT Author: tianyisama
-Author-email: tianyisama99@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Dist: nonebot-adapter-onebot
-(>=2.1.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Project-URL:
-Repository, https://github.com/tianyisama/nonebot_plugin_mypower Description-
-Content-Type: text/markdown
+//github.com/tianyisama/nonebot_plugin_mypower License: MIT Author: TianYi
+Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: nonebot-adapter-onebot (>=2.1.1,<3.0.0) Requires-Dist: nonebot2
+(>=2.0.0rc1,<3.0.0) Project-URL: Repository, https://github.com/tianyisama/
+nonebot_plugin_mypower Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                          # nonebot-plugin-mypower _â¨
   ä¸æ¬¾éæºçæè¶è½åçæä»¶ï¼éç¨äºOnebot V11ï¼â¨__[_l_i_c_e_n_s_e_]
                                [NoneBot][python]
 ## ð ä»ç» ä¸æ¬¾éæºçæè¶è½åçæä»¶ï¼éç¨äºNonebot2 V11ï¼
 ## ð¿ å®è£ å®è£pillow(å¿é¡») pip install pillow
```

