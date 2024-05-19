# Comparing `tmp/ten_drops-1.0.1.tar.gz` & `tmp/ten_drops-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ten_drops-1.0.1.tar", last modified: Sat May 18 08:47:52 2024, max compression
+gzip compressed data, was "ten_drops-1.0.2.tar", last modified: Sun May 19 12:50:41 2024, max compression
```

## Comparing `ten_drops-1.0.1.tar` & `ten_drops-1.0.2.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 08:47:52.795453 ten_drops-1.0.1/
--rw-rw-rw-   0        0        0     1083 2024-04-14 12:44:53.000000 ten_drops-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       42 2024-05-17 14:40:25.000000 ten_drops-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1994 2024-05-18 08:47:52.795453 ten_drops-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2024-05-18 03:54:20.000000 ten_drops-1.0.1/README.md
--rw-rw-rw-   0        0        0      444 2024-05-18 08:46:33.000000 ten_drops-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 08:47:52.795453 ten_drops-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2909 2024-05-18 08:46:33.000000 ten_drops-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:47:52.709494 ten_drops-1.0.1/ten_drops/
--rw-rw-rw-   0        0        0     4240 2024-05-18 08:45:40.000000 ten_drops-1.0.1/ten_drops/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:47:52.701495 ten_drops-1.0.1/ten_drops/asset/
-drwxrwxrwx   0        0        0        0 2024-05-18 08:47:52.717495 ten_drops-1.0.1/ten_drops/asset/audio/
--rw-rw-rw-   0        0        0     1144 2024-05-17 10:26:33.000000 ten_drops-1.0.1/ten_drops/asset/audio/break.mp3
--rw-rw-rw-   0        0        0     1040 2024-05-17 10:25:47.000000 ten_drops-1.0.1/ten_drops/asset/audio/grow.mp3
--rw-rw-rw-   0        0        0     1976 2024-05-17 10:26:07.000000 ten_drops-1.0.1/ten_drops/asset/audio/hp.mp3
-drwxrwxrwx   0        0        0        0 2024-05-18 08:47:52.717495 ten_drops-1.0.1/ten_drops/asset/font/
--rw-rw-rw-   0        0        0   289624 2021-12-06 12:57:14.000000 ten_drops-1.0.1/ten_drops/asset/font/FiraCode-Regular.ttf
--rw-rw-rw-   0        0        0   124732 2016-01-30 05:05:18.000000 ten_drops-1.0.1/ten_drops/asset/font/kust.ttf
-drwxrwxrwx   0        0        0        0 2024-05-18 08:47:52.717495 ten_drops-1.0.1/ten_drops/asset/img/
--rw-rw-rw-   0        0        0   688855 2024-05-13 12:44:57.000000 ten_drops-1.0.1/ten_drops/asset/img/background.png
--rw-rw-rw-   0        0        0      390 2024-05-17 10:11:11.000000 ten_drops-1.0.1/ten_drops/asset/img/cursor.png
-drwxrwxrwx   0        0        0        0 2024-05-18 08:47:52.795453 ten_drops-1.0.1/ten_drops/asset/img/drop/
--rw-rw-rw-   0        0        0      834 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/0.png
--rw-rw-rw-   0        0        0      628 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/1.png
--rw-rw-rw-   0        0        0      918 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/10.png
--rw-rw-rw-   0        0        0     3497 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/100.png
--rw-rw-rw-   0        0        0     3565 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/101.png
--rw-rw-rw-   0        0        0     3256 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/102.png
--rw-rw-rw-   0        0        0     3180 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/103.png
--rw-rw-rw-   0        0        0     3483 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/104.png
--rw-rw-rw-   0        0        0     3505 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/105.png
--rw-rw-rw-   0        0        0     3247 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/106.png
--rw-rw-rw-   0        0        0     3311 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/107.png
--rw-rw-rw-   0        0        0     3165 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/108.png
--rw-rw-rw-   0        0        0     3205 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/109.png
--rw-rw-rw-   0        0        0      929 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/11.png
--rw-rw-rw-   0        0        0     3194 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/110.png
--rw-rw-rw-   0        0        0     3237 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/111.png
--rw-rw-rw-   0        0        0     3322 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/112.png
--rw-rw-rw-   0        0        0     3393 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/113.png
--rw-rw-rw-   0        0        0     3139 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/114.png
--rw-rw-rw-   0        0        0     3387 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/115.png
--rw-rw-rw-   0        0        0     3241 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/116.png
--rw-rw-rw-   0        0        0     3688 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/117.png
--rw-rw-rw-   0        0        0     3718 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/118.png
--rw-rw-rw-   0        0        0     3490 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/119.png
--rw-rw-rw-   0        0        0     1015 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/12.png
--rw-rw-rw-   0        0        0     3658 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/120.png
--rw-rw-rw-   0        0        0     3436 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/121.png
--rw-rw-rw-   0        0        0     3254 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/122.png
--rw-rw-rw-   0        0        0     3484 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/123.png
--rw-rw-rw-   0        0        0     3733 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/124.png
--rw-rw-rw-   0        0        0     3249 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/125.png
--rw-rw-rw-   0        0        0     4041 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/126.png
--rw-rw-rw-   0        0        0     3588 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/127.png
--rw-rw-rw-   0        0        0     3622 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/128.png
--rw-rw-rw-   0        0        0     3129 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/129.png
--rw-rw-rw-   0        0        0     1049 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/13.png
--rw-rw-rw-   0        0        0     3596 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/130.png
--rw-rw-rw-   0        0        0     4609 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/131.png
--rw-rw-rw-   0        0        0     4289 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/132.png
--rw-rw-rw-   0        0        0     2789 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/133.png
--rw-rw-rw-   0        0        0     1498 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/134.png
--rw-rw-rw-   0        0        0     1012 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/14.png
--rw-rw-rw-   0        0        0      955 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/15.png
--rw-rw-rw-   0        0        0      897 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/16.png
--rw-rw-rw-   0        0        0      843 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/17.png
--rw-rw-rw-   0        0        0      883 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/18.png
--rw-rw-rw-   0        0        0      936 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/19.png
--rw-rw-rw-   0        0        0      713 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/2.png
--rw-rw-rw-   0        0        0      994 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/20.png
--rw-rw-rw-   0        0        0     1020 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/21.png
--rw-rw-rw-   0        0        0     1025 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/22.png
--rw-rw-rw-   0        0        0      930 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/23.png
--rw-rw-rw-   0        0        0      939 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/24.png
--rw-rw-rw-   0        0        0      929 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/25.png
--rw-rw-rw-   0        0        0      989 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/26.png
--rw-rw-rw-   0        0        0      955 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/27.png
--rw-rw-rw-   0        0        0      929 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/28.png
--rw-rw-rw-   0        0        0     1251 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/29.png
--rw-rw-rw-   0        0        0      955 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/3.png
--rw-rw-rw-   0        0        0     1569 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/30.png
--rw-rw-rw-   0        0        0     1718 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/31.png
--rw-rw-rw-   0        0        0     1978 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/32.png
--rw-rw-rw-   0        0        0     1824 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/33.png
--rw-rw-rw-   0        0        0     1740 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/34.png
--rw-rw-rw-   0        0        0     1708 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/35.png
--rw-rw-rw-   0        0        0     1969 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/36.png
--rw-rw-rw-   0        0        0     2167 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/37.png
--rw-rw-rw-   0        0        0     2180 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/38.png
--rw-rw-rw-   0        0        0     2200 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/39.png
--rw-rw-rw-   0        0        0     1071 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/4.png
--rw-rw-rw-   0        0        0     1768 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/40.png
--rw-rw-rw-   0        0        0     1730 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/41.png
--rw-rw-rw-   0        0        0     2128 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/42.png
--rw-rw-rw-   0        0        0     2202 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/43.png
--rw-rw-rw-   0        0        0     1831 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/44.png
--rw-rw-rw-   0        0        0     1773 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/45.png
--rw-rw-rw-   0        0        0     2115 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/46.png
--rw-rw-rw-   0        0        0     1824 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/47.png
--rw-rw-rw-   0        0        0     2105 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/48.png
--rw-rw-rw-   0        0        0     1942 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/49.png
--rw-rw-rw-   0        0        0     1158 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/5.png
--rw-rw-rw-   0        0        0     1858 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/50.png
--rw-rw-rw-   0        0        0     1981 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/51.png
--rw-rw-rw-   0        0        0     2147 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/52.png
--rw-rw-rw-   0        0        0     2214 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/53.png
--rw-rw-rw-   0        0        0     2176 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/54.png
--rw-rw-rw-   0        0        0     2276 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/55.png
--rw-rw-rw-   0        0        0     2018 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/56.png
--rw-rw-rw-   0        0        0     1924 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/57.png
--rw-rw-rw-   0        0        0     1918 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/58.png
--rw-rw-rw-   0        0        0     2138 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/59.png
--rw-rw-rw-   0        0        0     1077 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/6.png
--rw-rw-rw-   0        0        0     2244 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/60.png
--rw-rw-rw-   0        0        0     2170 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/61.png
--rw-rw-rw-   0        0        0     2040 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/62.png
--rw-rw-rw-   0        0        0     1959 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/63.png
--rw-rw-rw-   0        0        0     2005 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/64.png
--rw-rw-rw-   0        0        0     2108 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/65.png
--rw-rw-rw-   0        0        0     2186 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/66.png
--rw-rw-rw-   0        0        0     2006 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/67.png
--rw-rw-rw-   0        0        0     1941 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/68.png
--rw-rw-rw-   0        0        0     2552 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/69.png
--rw-rw-rw-   0        0        0      935 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/7.png
--rw-rw-rw-   0        0        0     3138 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/70.png
--rw-rw-rw-   0        0        0     3280 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/71.png
--rw-rw-rw-   0        0        0     3443 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/72.png
--rw-rw-rw-   0        0        0     3000 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/73.png
--rw-rw-rw-   0        0        0     3009 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/74.png
--rw-rw-rw-   0        0        0     3069 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/75.png
--rw-rw-rw-   0        0        0     3340 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/76.png
--rw-rw-rw-   0        0        0     3591 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/77.png
--rw-rw-rw-   0        0        0     3661 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/78.png
--rw-rw-rw-   0        0        0     3602 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/79.png
--rw-rw-rw-   0        0        0      839 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/8.png
--rw-rw-rw-   0        0        0     3399 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/80.png
--rw-rw-rw-   0        0        0     3230 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/81.png
--rw-rw-rw-   0        0        0     3069 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/82.png
--rw-rw-rw-   0        0        0     3208 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/83.png
--rw-rw-rw-   0        0        0     3542 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/84.png
--rw-rw-rw-   0        0        0     3556 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/85.png
--rw-rw-rw-   0        0        0     3312 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/86.png
--rw-rw-rw-   0        0        0     3202 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/87.png
--rw-rw-rw-   0        0        0     3547 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/88.png
--rw-rw-rw-   0        0        0     3535 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/89.png
--rw-rw-rw-   0        0        0      736 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/9.png
--rw-rw-rw-   0        0        0     3542 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/90.png
--rw-rw-rw-   0        0        0     3362 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/91.png
--rw-rw-rw-   0        0        0     3356 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/92.png
--rw-rw-rw-   0        0        0     2835 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/93.png
--rw-rw-rw-   0        0        0     2935 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/94.png
--rw-rw-rw-   0        0        0     3035 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/95.png
--rw-rw-rw-   0        0        0     3548 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/96.png
--rw-rw-rw-   0        0        0     3663 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/97.png
--rw-rw-rw-   0        0        0     3185 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/98.png
--rw-rw-rw-   0        0        0     3036 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/drop/99.png
-drwxrwxrwx   0        0        0        0 2024-05-18 08:47:52.795453 ten_drops-1.0.1/ten_drops/asset/img/droplet/
--rw-rw-rw-   0        0        0      880 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/droplet/0.png
--rw-rw-rw-   0        0        0      846 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/droplet/1.png
--rw-rw-rw-   0        0        0      800 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/droplet/2.png
--rw-rw-rw-   0        0        0      937 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/droplet/3.png
--rw-rw-rw-   0        0        0      749 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/droplet/4.png
--rw-rw-rw-   0        0        0      579 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/droplet/5.png
--rw-rw-rw-   0        0        0      291 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/droplet/6.png
--rw-rw-rw-   0        0        0      169 2024-04-24 13:33:17.000000 ten_drops-1.0.1/ten_drops/asset/img/droplet/7.png
--rw-rw-rw-   0        0        0     5430 2024-05-17 09:03:24.000000 ten_drops-1.0.1/ten_drops/asset/img/game.ico
--rw-rw-rw-   0        0        0   573151 2024-05-16 14:18:21.000000 ten_drops-1.0.1/ten_drops/asset/img/notification.png
--rw-rw-rw-   0        0        0     1470 2024-05-17 08:38:54.000000 ten_drops-1.0.1/ten_drops/button.py
--rw-rw-rw-   0        0        0       69 2024-05-17 15:08:45.000000 ten_drops-1.0.1/ten_drops/cli.py
--rw-rw-rw-   0        0        0      996 2024-05-14 15:49:03.000000 ten_drops-1.0.1/ten_drops/cover.py
--rw-rw-rw-   0        0        0     3594 2024-05-17 11:21:07.000000 ten_drops-1.0.1/ten_drops/drop.py
--rw-rw-rw-   0        0        0     2038 2024-05-17 14:13:31.000000 ten_drops-1.0.1/ten_drops/droplet.py
--rw-rw-rw-   0        0        0     8919 2024-05-17 13:18:01.000000 ten_drops-1.0.1/ten_drops/game.py
--rw-rw-rw-   0        0        0     1591 2024-05-17 14:13:31.000000 ten_drops-1.0.1/ten_drops/notification.py
--rw-rw-rw-   0        0        0     2753 2024-05-17 08:38:54.000000 ten_drops-1.0.1/ten_drops/panel.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:47:52.795453 ten_drops-1.0.1/ten_drops.egg-info/
--rw-rw-rw-   0        0        0     1994 2024-05-18 08:47:52.000000 ten_drops-1.0.1/ten_drops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5310 2024-05-18 08:47:52.000000 ten_drops-1.0.1/ten_drops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 08:47:52.000000 ten_drops-1.0.1/ten_drops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 08:47:52.000000 ten_drops-1.0.1/ten_drops.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 08:47:52.000000 ten_drops-1.0.1/ten_drops.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 12:50:41.109132 ten_drops-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2024-04-14 12:44:53.000000 ten_drops-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       42 2024-05-17 14:40:25.000000 ten_drops-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1991 2024-05-19 12:50:41.109132 ten_drops-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1111 2024-05-19 09:06:33.000000 ten_drops-1.0.2/README.md
+-rw-rw-rw-   0        0        0      444 2024-05-19 12:49:58.000000 ten_drops-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 12:50:41.110132 ten_drops-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2909 2024-05-19 12:49:58.000000 ten_drops-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:50:41.017885 ten_drops-1.0.2/ten_drops/
+-rw-rw-rw-   0        0        0     4240 2024-05-18 08:45:40.000000 ten_drops-1.0.2/ten_drops/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:50:41.008804 ten_drops-1.0.2/ten_drops/asset/
+drwxrwxrwx   0        0        0        0 2024-05-19 12:50:41.023391 ten_drops-1.0.2/ten_drops/asset/audio/
+-rw-rw-rw-   0        0        0     1144 2024-05-17 10:26:33.000000 ten_drops-1.0.2/ten_drops/asset/audio/break.mp3
+-rw-rw-rw-   0        0        0     1040 2024-05-17 10:25:47.000000 ten_drops-1.0.2/ten_drops/asset/audio/grow.mp3
+-rw-rw-rw-   0        0        0     1976 2024-05-17 10:26:07.000000 ten_drops-1.0.2/ten_drops/asset/audio/hp.mp3
+drwxrwxrwx   0        0        0        0 2024-05-19 12:50:41.024890 ten_drops-1.0.2/ten_drops/asset/font/
+-rw-rw-rw-   0        0        0   289624 2021-12-06 12:57:14.000000 ten_drops-1.0.2/ten_drops/asset/font/FiraCode-Regular.ttf
+-rw-rw-rw-   0        0        0   124732 2016-01-30 05:05:18.000000 ten_drops-1.0.2/ten_drops/asset/font/kust.ttf
+drwxrwxrwx   0        0        0        0 2024-05-19 12:50:41.027895 ten_drops-1.0.2/ten_drops/asset/img/
+-rw-rw-rw-   0        0        0   688855 2024-05-13 12:44:57.000000 ten_drops-1.0.2/ten_drops/asset/img/background.png
+-rw-rw-rw-   0        0        0      390 2024-05-17 10:11:11.000000 ten_drops-1.0.2/ten_drops/asset/img/cursor.png
+drwxrwxrwx   0        0        0        0 2024-05-19 12:50:41.103614 ten_drops-1.0.2/ten_drops/asset/img/drop/
+-rw-rw-rw-   0        0        0      834 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/0.png
+-rw-rw-rw-   0        0        0      628 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/1.png
+-rw-rw-rw-   0        0        0      918 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/10.png
+-rw-rw-rw-   0        0        0     3497 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/100.png
+-rw-rw-rw-   0        0        0     3565 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/101.png
+-rw-rw-rw-   0        0        0     3256 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/102.png
+-rw-rw-rw-   0        0        0     3180 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/103.png
+-rw-rw-rw-   0        0        0     3483 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/104.png
+-rw-rw-rw-   0        0        0     3505 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/105.png
+-rw-rw-rw-   0        0        0     3247 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/106.png
+-rw-rw-rw-   0        0        0     3311 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/107.png
+-rw-rw-rw-   0        0        0     3165 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/108.png
+-rw-rw-rw-   0        0        0     3205 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/109.png
+-rw-rw-rw-   0        0        0      929 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/11.png
+-rw-rw-rw-   0        0        0     3194 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/110.png
+-rw-rw-rw-   0        0        0     3237 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/111.png
+-rw-rw-rw-   0        0        0     3322 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/112.png
+-rw-rw-rw-   0        0        0     3393 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/113.png
+-rw-rw-rw-   0        0        0     3139 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/114.png
+-rw-rw-rw-   0        0        0     3387 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/115.png
+-rw-rw-rw-   0        0        0     3241 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/116.png
+-rw-rw-rw-   0        0        0     3688 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/117.png
+-rw-rw-rw-   0        0        0     3718 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/118.png
+-rw-rw-rw-   0        0        0     3490 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/119.png
+-rw-rw-rw-   0        0        0     1015 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/12.png
+-rw-rw-rw-   0        0        0     3658 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/120.png
+-rw-rw-rw-   0        0        0     3436 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/121.png
+-rw-rw-rw-   0        0        0     3254 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/122.png
+-rw-rw-rw-   0        0        0     3484 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/123.png
+-rw-rw-rw-   0        0        0     3733 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/124.png
+-rw-rw-rw-   0        0        0     3249 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/125.png
+-rw-rw-rw-   0        0        0     4041 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/126.png
+-rw-rw-rw-   0        0        0     3588 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/127.png
+-rw-rw-rw-   0        0        0     3622 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/128.png
+-rw-rw-rw-   0        0        0     3129 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/129.png
+-rw-rw-rw-   0        0        0     1049 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/13.png
+-rw-rw-rw-   0        0        0     3596 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/130.png
+-rw-rw-rw-   0        0        0     4609 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/131.png
+-rw-rw-rw-   0        0        0     4289 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/132.png
+-rw-rw-rw-   0        0        0     2789 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/133.png
+-rw-rw-rw-   0        0        0     1498 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/134.png
+-rw-rw-rw-   0        0        0     1012 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/14.png
+-rw-rw-rw-   0        0        0      955 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/15.png
+-rw-rw-rw-   0        0        0      897 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/16.png
+-rw-rw-rw-   0        0        0      843 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/17.png
+-rw-rw-rw-   0        0        0      883 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/18.png
+-rw-rw-rw-   0        0        0      936 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/19.png
+-rw-rw-rw-   0        0        0      713 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/2.png
+-rw-rw-rw-   0        0        0      994 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/20.png
+-rw-rw-rw-   0        0        0     1020 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/21.png
+-rw-rw-rw-   0        0        0     1025 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/22.png
+-rw-rw-rw-   0        0        0      930 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/23.png
+-rw-rw-rw-   0        0        0      939 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/24.png
+-rw-rw-rw-   0        0        0      929 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/25.png
+-rw-rw-rw-   0        0        0      989 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/26.png
+-rw-rw-rw-   0        0        0      955 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/27.png
+-rw-rw-rw-   0        0        0      929 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/28.png
+-rw-rw-rw-   0        0        0     1251 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/29.png
+-rw-rw-rw-   0        0        0      955 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/3.png
+-rw-rw-rw-   0        0        0     1569 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/30.png
+-rw-rw-rw-   0        0        0     1718 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/31.png
+-rw-rw-rw-   0        0        0     1978 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/32.png
+-rw-rw-rw-   0        0        0     1824 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/33.png
+-rw-rw-rw-   0        0        0     1740 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/34.png
+-rw-rw-rw-   0        0        0     1708 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/35.png
+-rw-rw-rw-   0        0        0     1969 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/36.png
+-rw-rw-rw-   0        0        0     2167 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/37.png
+-rw-rw-rw-   0        0        0     2180 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/38.png
+-rw-rw-rw-   0        0        0     2200 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/39.png
+-rw-rw-rw-   0        0        0     1071 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/4.png
+-rw-rw-rw-   0        0        0     1768 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/40.png
+-rw-rw-rw-   0        0        0     1730 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/41.png
+-rw-rw-rw-   0        0        0     2128 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/42.png
+-rw-rw-rw-   0        0        0     2202 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/43.png
+-rw-rw-rw-   0        0        0     1831 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/44.png
+-rw-rw-rw-   0        0        0     1773 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/45.png
+-rw-rw-rw-   0        0        0     2115 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/46.png
+-rw-rw-rw-   0        0        0     1824 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/47.png
+-rw-rw-rw-   0        0        0     2105 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/48.png
+-rw-rw-rw-   0        0        0     1942 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/49.png
+-rw-rw-rw-   0        0        0     1158 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/5.png
+-rw-rw-rw-   0        0        0     1858 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/50.png
+-rw-rw-rw-   0        0        0     1981 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/51.png
+-rw-rw-rw-   0        0        0     2147 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/52.png
+-rw-rw-rw-   0        0        0     2214 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/53.png
+-rw-rw-rw-   0        0        0     2176 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/54.png
+-rw-rw-rw-   0        0        0     2276 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/55.png
+-rw-rw-rw-   0        0        0     2018 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/56.png
+-rw-rw-rw-   0        0        0     1924 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/57.png
+-rw-rw-rw-   0        0        0     1918 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/58.png
+-rw-rw-rw-   0        0        0     2138 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/59.png
+-rw-rw-rw-   0        0        0     1077 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/6.png
+-rw-rw-rw-   0        0        0     2244 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/60.png
+-rw-rw-rw-   0        0        0     2170 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/61.png
+-rw-rw-rw-   0        0        0     2040 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/62.png
+-rw-rw-rw-   0        0        0     1959 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/63.png
+-rw-rw-rw-   0        0        0     2005 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/64.png
+-rw-rw-rw-   0        0        0     2108 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/65.png
+-rw-rw-rw-   0        0        0     2186 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/66.png
+-rw-rw-rw-   0        0        0     2006 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/67.png
+-rw-rw-rw-   0        0        0     1941 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/68.png
+-rw-rw-rw-   0        0        0     2552 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/69.png
+-rw-rw-rw-   0        0        0      935 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/7.png
+-rw-rw-rw-   0        0        0     3138 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/70.png
+-rw-rw-rw-   0        0        0     3280 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/71.png
+-rw-rw-rw-   0        0        0     3443 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/72.png
+-rw-rw-rw-   0        0        0     3000 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/73.png
+-rw-rw-rw-   0        0        0     3009 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/74.png
+-rw-rw-rw-   0        0        0     3069 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/75.png
+-rw-rw-rw-   0        0        0     3340 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/76.png
+-rw-rw-rw-   0        0        0     3591 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/77.png
+-rw-rw-rw-   0        0        0     3661 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/78.png
+-rw-rw-rw-   0        0        0     3602 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/79.png
+-rw-rw-rw-   0        0        0      839 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/8.png
+-rw-rw-rw-   0        0        0     3399 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/80.png
+-rw-rw-rw-   0        0        0     3230 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/81.png
+-rw-rw-rw-   0        0        0     3069 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/82.png
+-rw-rw-rw-   0        0        0     3208 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/83.png
+-rw-rw-rw-   0        0        0     3542 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/84.png
+-rw-rw-rw-   0        0        0     3556 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/85.png
+-rw-rw-rw-   0        0        0     3312 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/86.png
+-rw-rw-rw-   0        0        0     3202 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/87.png
+-rw-rw-rw-   0        0        0     3547 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/88.png
+-rw-rw-rw-   0        0        0     3535 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/89.png
+-rw-rw-rw-   0        0        0      736 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/9.png
+-rw-rw-rw-   0        0        0     3542 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/90.png
+-rw-rw-rw-   0        0        0     3362 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/91.png
+-rw-rw-rw-   0        0        0     3356 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/92.png
+-rw-rw-rw-   0        0        0     2835 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/93.png
+-rw-rw-rw-   0        0        0     2935 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/94.png
+-rw-rw-rw-   0        0        0     3035 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/95.png
+-rw-rw-rw-   0        0        0     3548 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/96.png
+-rw-rw-rw-   0        0        0     3663 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/97.png
+-rw-rw-rw-   0        0        0     3185 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/98.png
+-rw-rw-rw-   0        0        0     3036 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/drop/99.png
+drwxrwxrwx   0        0        0        0 2024-05-19 12:50:41.108130 ten_drops-1.0.2/ten_drops/asset/img/droplet/
+-rw-rw-rw-   0        0        0      880 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/droplet/0.png
+-rw-rw-rw-   0        0        0      846 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/droplet/1.png
+-rw-rw-rw-   0        0        0      800 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/droplet/2.png
+-rw-rw-rw-   0        0        0      937 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/droplet/3.png
+-rw-rw-rw-   0        0        0      749 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/droplet/4.png
+-rw-rw-rw-   0        0        0      579 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/droplet/5.png
+-rw-rw-rw-   0        0        0      291 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/droplet/6.png
+-rw-rw-rw-   0        0        0      169 2024-04-24 13:33:17.000000 ten_drops-1.0.2/ten_drops/asset/img/droplet/7.png
+-rw-rw-rw-   0        0        0     5430 2024-05-17 09:03:24.000000 ten_drops-1.0.2/ten_drops/asset/img/game.ico
+-rw-rw-rw-   0        0        0   573151 2024-05-16 14:18:21.000000 ten_drops-1.0.2/ten_drops/asset/img/notification.png
+-rw-rw-rw-   0        0        0     1470 2024-05-17 08:38:54.000000 ten_drops-1.0.2/ten_drops/button.py
+-rw-rw-rw-   0        0        0       69 2024-05-17 15:08:45.000000 ten_drops-1.0.2/ten_drops/cli.py
+-rw-rw-rw-   0        0        0      996 2024-05-14 15:49:03.000000 ten_drops-1.0.2/ten_drops/cover.py
+-rw-rw-rw-   0        0        0     3594 2024-05-17 11:21:07.000000 ten_drops-1.0.2/ten_drops/drop.py
+-rw-rw-rw-   0        0        0     2038 2024-05-17 14:13:31.000000 ten_drops-1.0.2/ten_drops/droplet.py
+-rw-rw-rw-   0        0        0     8918 2024-05-19 09:07:04.000000 ten_drops-1.0.2/ten_drops/game.py
+-rw-rw-rw-   0        0        0     1591 2024-05-17 14:13:31.000000 ten_drops-1.0.2/ten_drops/notification.py
+-rw-rw-rw-   0        0        0     2753 2024-05-17 08:38:54.000000 ten_drops-1.0.2/ten_drops/panel.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:50:41.108130 ten_drops-1.0.2/ten_drops.egg-info/
+-rw-rw-rw-   0        0        0     1991 2024-05-19 12:50:40.000000 ten_drops-1.0.2/ten_drops.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5310 2024-05-19 12:50:40.000000 ten_drops-1.0.2/ten_drops.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 12:50:40.000000 ten_drops-1.0.2/ten_drops.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 12:50:40.000000 ten_drops-1.0.2/ten_drops.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 12:50:40.000000 ten_drops-1.0.2/ten_drops.egg-info/top_level.txt
```

### Comparing `ten_drops-1.0.1/LICENSE` & `ten_drops-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/PKG-INFO` & `ten_drops-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ten-drops
-Version: 1.0.1
+Version: 1.0.2
 Summary: A ten drops game written in pygame-ce.
 Home-page: https://github.com/chyok/ten-drops
 Author: chyok
 Author-email: chyok@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -27,15 +27,15 @@
 ![GitHub License](https://img.shields.io/github/license/chyok/ten-drops)
 ![PyPI - Version](https://img.shields.io/pypi/v/ten-drops)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ten-drops)
 
 A ten drops game written in pygame-ce.  
 Click on these water droplets to make them explode until the screen is cleared.
 
-The inspiration and assets all come from the Flash game of the same name.
+The inspiration and assets all come from the Flash game "Splash Back".
 
 ![example](https://github.com/chyok/ten-drops/assets/32629225/b8409169-dd31-4912-a91e-5fed288a833c)
 
 ## Installation
 
 ### use pip
```

### Comparing `ten_drops-1.0.1/README.md` & `ten_drops-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![GitHub License](https://img.shields.io/github/license/chyok/ten-drops)
 ![PyPI - Version](https://img.shields.io/pypi/v/ten-drops)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ten-drops)
 
 A ten drops game written in pygame-ce.  
 Click on these water droplets to make them explode until the screen is cleared.
 
-The inspiration and assets all come from the Flash game of the same name.
+The inspiration and assets all come from the Flash game "Splash Back".
 
 ![example](https://github.com/chyok/ten-drops/assets/32629225/b8409169-dd31-4912-a91e-5fed288a833c)
 
 ## Installation
 
 ### use pip
```

### Comparing `ten_drops-1.0.1/setup.py` & `ten_drops-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 NAME = 'ten-drops'
 DESCRIPTION = 'A ten drops game written in pygame-ce.'
 URL = 'https://github.com/chyok/ten-drops'
 EMAIL = 'chyok@hotmail.com'
 AUTHOR = 'chyok'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 
 REQUIRED = [
     'pygame-ce'
 ]
 
 EXTRAS = {}
```

### Comparing `ten_drops-1.0.1/ten_drops/__init__.py` & `ten_drops-1.0.2/ten_drops/__init__.py`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/audio/break.mp3` & `ten_drops-1.0.2/ten_drops/asset/audio/break.mp3`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/audio/grow.mp3` & `ten_drops-1.0.2/ten_drops/asset/audio/grow.mp3`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/audio/hp.mp3` & `ten_drops-1.0.2/ten_drops/asset/audio/hp.mp3`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/font/FiraCode-Regular.ttf` & `ten_drops-1.0.2/ten_drops/asset/font/FiraCode-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/font/kust.ttf` & `ten_drops-1.0.2/ten_drops/asset/font/kust.ttf`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/background.png` & `ten_drops-1.0.2/ten_drops/asset/img/background.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/0.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/0.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/1.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/1.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/10.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/10.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/100.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/100.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/101.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/101.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/102.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/102.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/103.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/103.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/104.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/104.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/105.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/105.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/106.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/106.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/107.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/107.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/108.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/108.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/109.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/109.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/11.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/11.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/110.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/110.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/111.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/111.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/112.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/112.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/113.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/113.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/114.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/114.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/115.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/115.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/116.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/116.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/117.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/117.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/118.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/118.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/119.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/119.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/12.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/12.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/120.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/120.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/121.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/121.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/122.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/122.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/123.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/123.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/124.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/124.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/125.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/125.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/126.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/126.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/127.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/127.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/128.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/128.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/129.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/129.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/13.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/13.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/130.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/130.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/131.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/131.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/132.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/132.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/133.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/133.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/134.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/134.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/14.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/14.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/15.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/15.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/16.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/16.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/17.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/17.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/18.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/18.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/19.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/19.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/2.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/2.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/20.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/20.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/21.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/21.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/22.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/22.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/23.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/23.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/24.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/24.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/25.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/25.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/26.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/26.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/27.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/27.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/28.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/28.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/29.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/29.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/3.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/3.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/30.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/30.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/31.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/31.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/32.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/32.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/33.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/33.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/34.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/34.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/35.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/35.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/36.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/36.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/37.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/37.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/38.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/38.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/39.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/39.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/4.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/4.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/40.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/40.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/41.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/41.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/42.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/42.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/43.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/43.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/44.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/44.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/45.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/45.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/46.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/46.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/47.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/47.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/48.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/48.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/49.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/49.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/5.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/5.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/50.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/50.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/51.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/51.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/52.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/52.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/53.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/53.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/54.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/54.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/55.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/55.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/56.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/56.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/57.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/57.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/58.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/58.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/59.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/59.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/6.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/6.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/60.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/60.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/61.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/61.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/62.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/62.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/63.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/63.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/64.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/64.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/65.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/65.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/66.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/66.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/67.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/67.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/68.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/68.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/69.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/69.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/7.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/7.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/70.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/70.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/71.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/71.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/72.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/72.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/73.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/73.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/74.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/74.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/75.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/75.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/76.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/76.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/77.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/77.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/78.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/78.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/79.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/79.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/8.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/8.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/80.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/80.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/81.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/81.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/82.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/82.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/83.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/83.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/84.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/84.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/85.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/85.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/86.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/86.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/87.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/87.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/88.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/88.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/89.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/89.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/9.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/9.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/90.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/90.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/91.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/91.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/92.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/92.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/93.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/93.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/94.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/94.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/95.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/95.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/96.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/96.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/97.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/97.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/98.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/98.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/drop/99.png` & `ten_drops-1.0.2/ten_drops/asset/img/drop/99.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/droplet/0.png` & `ten_drops-1.0.2/ten_drops/asset/img/droplet/0.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/droplet/1.png` & `ten_drops-1.0.2/ten_drops/asset/img/droplet/1.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/droplet/2.png` & `ten_drops-1.0.2/ten_drops/asset/img/droplet/2.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/droplet/3.png` & `ten_drops-1.0.2/ten_drops/asset/img/droplet/3.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/droplet/4.png` & `ten_drops-1.0.2/ten_drops/asset/img/droplet/4.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/droplet/5.png` & `ten_drops-1.0.2/ten_drops/asset/img/droplet/5.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/game.ico` & `ten_drops-1.0.2/ten_drops/asset/img/game.ico`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/asset/img/notification.png` & `ten_drops-1.0.2/ten_drops/asset/img/notification.png`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/button.py` & `ten_drops-1.0.2/ten_drops/button.py`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/cover.py` & `ten_drops-1.0.2/ten_drops/cover.py`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/drop.py` & `ten_drops-1.0.2/ten_drops/drop.py`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/droplet.py` & `ten_drops-1.0.2/ten_drops/droplet.py`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/game.py` & `ten_drops-1.0.2/ten_drops/game.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     def notify(self, _type):
         if _type == NoticeType.success:
             text = "     Well Done!\n     + 2 drops\n\n     Next Level"
         elif _type == NoticeType.failed:
             text = f"You Lost\nYour Score: {self.score}"
         else:
             text = ("The game and water drop assets are \n"
-                    "from the Flash game of the same name.\n"
+                    "from the Flash game \"Splash Back\".\n"
                     "\n\n\nAuthor: chyok\n"
                     "Email : chyok@hotmail.com\nGithub: https://github.com/chyok\n"
                     "\nImplemented using pygame-ce.")
 
         Notice(_type, text, self.notifications)
 
     def start(self):
```

### Comparing `ten_drops-1.0.1/ten_drops/notification.py` & `ten_drops-1.0.2/ten_drops/notification.py`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops/panel.py` & `ten_drops-1.0.2/ten_drops/panel.py`

 * *Files identical despite different names*

### Comparing `ten_drops-1.0.1/ten_drops.egg-info/PKG-INFO` & `ten_drops-1.0.2/ten_drops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ten-drops
-Version: 1.0.1
+Version: 1.0.2
 Summary: A ten drops game written in pygame-ce.
 Home-page: https://github.com/chyok/ten-drops
 Author: chyok
 Author-email: chyok@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -27,15 +27,15 @@
 ![GitHub License](https://img.shields.io/github/license/chyok/ten-drops)
 ![PyPI - Version](https://img.shields.io/pypi/v/ten-drops)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ten-drops)
 
 A ten drops game written in pygame-ce.  
 Click on these water droplets to make them explode until the screen is cleared.
 
-The inspiration and assets all come from the Flash game of the same name.
+The inspiration and assets all come from the Flash game "Splash Back".
 
 ![example](https://github.com/chyok/ten-drops/assets/32629225/b8409169-dd31-4912-a91e-5fed288a833c)
 
 ## Installation
 
 ### use pip
```

### Comparing `ten_drops-1.0.1/ten_drops.egg-info/SOURCES.txt` & `ten_drops-1.0.2/ten_drops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

