# Comparing `tmp/torspy-1.0.3.tar.gz` & `tmp/torspy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torspy-1.0.3.tar", last modified: Fri May 17 18:04:18 2024, max compression
+gzip compressed data, was "torspy-2.0.0.tar", last modified: Sun May 19 06:06:24 2024, max compression
```

## Comparing `torspy-1.0.3.tar` & `torspy-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 18:04:18.999239 torspy-1.0.3/
--rw-rw-rw-   0        0        0     1065 2024-05-17 18:01:10.000000 torspy-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     6954 2024-05-17 18:04:18.999239 torspy-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2024-05-17 18:01:11.000000 torspy-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 18:04:18.999239 torspy-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1304 2024-05-17 18:04:08.000000 torspy-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:04:18.952377 torspy-1.0.3/torspy/
--rw-rw-rw-   0        0        0       78 2024-05-17 18:01:10.000000 torspy-1.0.3/torspy/__init__.py
--rw-rw-rw-   0        0        0     1948 2024-05-17 18:01:10.000000 torspy-1.0.3/torspy/cli.py
--rw-rw-rw-   0        0        0     9432 2024-05-17 18:01:10.000000 torspy-1.0.3/torspy/scraper.py
--rw-rw-rw-   0        0        0      102 2024-05-17 18:01:10.000000 torspy-1.0.3/torspy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:04:18.983621 torspy-1.0.3/torspy.egg-info/
--rw-rw-rw-   0        0        0     6954 2024-05-17 18:04:18.000000 torspy-1.0.3/torspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-05-17 18:04:18.000000 torspy-1.0.3/torspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 18:04:18.000000 torspy-1.0.3/torspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-17 18:04:18.000000 torspy-1.0.3/torspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-05-17 18:04:18.000000 torspy-1.0.3/torspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 18:04:18.000000 torspy-1.0.3/torspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 06:06:24.692725 torspy-2.0.0/
+-rw-rw-rw-   0        0        0     1065 2024-05-19 06:03:36.000000 torspy-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0    12582 2024-05-19 06:06:24.677754 torspy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11543 2024-05-19 06:03:37.000000 torspy-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 06:06:24.692725 torspy-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2024-05-19 06:06:13.000000 torspy-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 06:06:24.520889 torspy-2.0.0/torspy/
+-rw-rw-rw-   0        0        0      103 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/__init__.py
+-rw-rw-rw-   0        0        0     2910 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-19 06:06:24.677754 torspy-2.0.0/torspy/scraper/
+-rw-rw-rw-   0        0        0      103 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/__init__.py
+-rw-rw-rw-   0        0        0     1488 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/analyze.py
+-rw-rw-rw-   0        0        0     3256 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/directories.py
+-rw-rw-rw-   0        0        0     1244 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/download.py
+-rw-rw-rw-   0        0        0     1405 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/html_extract.py
+-rw-rw-rw-   0        0        0     1247 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/links.py
+-rw-rw-rw-   0        0        0     2143 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/scrape.py
+-rw-rw-rw-   0        0        0     1265 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/services.py
+-rw-rw-rw-   0        0        0     3367 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/subdomains.py
+-rw-rw-rw-   0        0        0      716 2024-05-19 06:03:36.000000 torspy-2.0.0/torspy/scraper/tor_check.py
+drwxrwxrwx   0        0        0        0 2024-05-19 06:06:24.630262 torspy-2.0.0/torspy.egg-info/
+-rw-rw-rw-   0        0        0    12582 2024-05-19 06:06:23.000000 torspy-2.0.0/torspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2024-05-19 06:06:24.000000 torspy-2.0.0/torspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 06:06:23.000000 torspy-2.0.0/torspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-19 06:06:23.000000 torspy-2.0.0/torspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-05-19 06:06:24.000000 torspy-2.0.0/torspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 06:06:24.000000 torspy-2.0.0/torspy.egg-info/top_level.txt
```

### Comparing `torspy-1.0.3/LICENSE` & `torspy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torspy-1.0.3/setup.py` & `torspy-2.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='torspy',
-    version='1.0.3',
+    version='2.0.0',
     author='Fidal',
     author_email='mrfidal@proton.me',
     description='torspy is a Python package for exploring .onion sites via Tor. It scrapes HTML content, localizes text, and detects hidden directories. With subdomain scanning, torspy enables thorough reconnaissance.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mr-fidal/torspy',
     packages=find_packages(),
```

### Comparing `torspy-1.0.3/torspy/cli.py` & `torspy-2.0.0/torspy/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,52 @@
 #!/usr/bin/python3
 # copyright ©️ 2024 author Fidal
 
 import argparse
-from .scraper import scrape_onion_site, find_directories, find_subdomains
+from .scraper.scrape import scrape_onion_site
+from .scraper.directories import find_directories
+from .scraper.subdomains import find_subdomains
+from .scraper.html_extract import extract_html
+from .scraper.analyze import analyze_content
+from .scraper.download import download_content
+from .scraper.links import find_links
+from .scraper.services import get_service_info 
 
 def main():
     epilog_text = '''
 \ntorspy is a robust Python package fortified with powerful algorithms, designed for seamless exploration of .onion sites via the Tor network. Its arsenal includes adept scraping of HTML from .onion URLs, precise text localization within the acquired content, and proficient storage of findings. Moreover, torspy boasts formidable subdomain scanning capabilities, enabling thorough reconnaissance across diverse subdomains. Additionally, it excels at detecting hidden directories, further enhancing its efficacy in navigating and extracting valuable information from the depths of the dark web.\n\n
 Copyright (c) 2024 author: Fidal
 Report an Issue : https://github.com/mr-fidal/torspy/issues
-'''
+    '''
+
     parser = argparse.ArgumentParser(description='Scrape a .onion site.', epilog=epilog_text,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('url', type=str, help='The .onion site URL to scrape')
     parser.add_argument('--find', type=str, help='The text to search for within the site')
     parser.add_argument('-s', '--save', type=str, help='The file name to save the content')
     parser.add_argument('-d', '--directory', type=str, help='The directory to save the file')
-    parser.add_argument('--dir', type=str, help='File containing list of directories to check')
-    parser.add_argument('--sub', type=str, help='File containing list of subdomains to check')
+    parser.add_argument('--dir', type=str, help='The file containing directories to scan')
+    parser.add_argument('--sub', type=str, help='The file containing subdomains to scan')
+    parser.add_argument('--analyze', action='store_true', help='Analyze the content of the site')
+    parser.add_argument('--download', action='store_true', help='Download the content of the site')
+    parser.add_argument('--links', action='store_true', help='Find all links on the site')
+    parser.add_argument('--service', action='store_true', help='Get service info of the site')
+
     args = parser.parse_args()
 
     if args.dir:
         find_directories(args.url, args.dir, args.save, args.directory)
     elif args.sub:
         find_subdomains(args.url, args.sub, args.save, args.directory)
+    elif args.analyze:
+        analyze_content(args.url)
+    elif args.download:
+        download_content(args.url, args.save, args.directory)
+    elif args.links:
+        find_links(args.url, args.save, args.directory)  
+    elif args.service:
+        get_service_info(args.url, args.save) 
     else:
         scrape_onion_site(args.url, args.find, args.save, args.directory)
 
 if __name__ == "__main__":
     main()
-
```

