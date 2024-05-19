# Comparing `tmp/gruel-4.0.0.tar.gz` & `tmp/gruel-4.1.0.tar.gz`

## Comparing `gruel-4.0.0.tar` & `gruel-4.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/__init__.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/brewer.py
--rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/core.py
--rw-r--r--   0        0        0    17593 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/crawler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/py.typed
--rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/requests.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/subgruel.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/template.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gruel-4.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gruel-4.0.0/LICENSE.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gruel-4.0.0/README.md
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 gruel-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 gruel-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/__init__.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/brewer.py
+-rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/core.py
+-rw-r--r--   0        0        0    18595 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/crawler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/py.typed
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/requests.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/subgruel.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/template.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gruel-4.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gruel-4.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gruel-4.1.0/README.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 gruel-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 gruel-4.1.0/PKG-INFO
```

### Comparing `gruel-4.0.0/src/gruel/brewer.py` & `gruel-4.1.0/src/gruel/brewer.py`

 * *Files identical despite different names*

### Comparing `gruel-4.0.0/src/gruel/core.py` & `gruel-4.1.0/src/gruel/core.py`

 * *Files identical despite different names*

### Comparing `gruel-4.0.0/src/gruel/crawler.py` & `gruel-4.1.0/src/gruel/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from functools import lru_cache
 
 import loggi
 import scrapetools
 from noiftimer import Timer
 from pathier import Pathier, Pathish
 from printbuddies import ColorMap, Progress, TimerColumn
-from rich import print
 from rich.console import Console
 from rich.progress import ProgressColumn
+from seleniumuser.seleniumuser import User
 from typing_extensions import Any, Callable, Sequence, override
 
 from .core import ChoresMixin, ParserMixin, ScraperMetricsMixin
-from .requests import Response, request
+from .requests import Response, SeleniumResponse, request
 
 root = Pathier(__file__).parent
 color_map = ColorMap()
 console = Console(style="pink1")
 
 
 class ThreadManager:
@@ -304,15 +304,15 @@
 
 
 class Crawler(loggi.LoggerMixin, ChoresMixin, LimitCheckerMixin):
     """A mutli-threaded web crawler framework."""
 
     def __init__(
         self,
-        scraper: CrawlScraper | None = None,
+        scrapers: Sequence[CrawlScraper] = [],
         max_depth: int | None = None,
         max_time: float | None = None,
         log_name: str | int | loggi.LogName = loggi.LogName.CLASSNAME,
         log_dir: Pathish = "logs",
         max_threads: int = 5,
         same_site_only: bool = True,
         custom_url_manager: UrlManager | None = None,
@@ -334,17 +334,17 @@
         self.init_logger(log_name, log_dir)
         self.url_manager = custom_url_manager or UrlManager()
         self.thread_manager = ThreadManager(max_threads)
         self.timer = Timer()
         self.max_time = MaxTimeLimit(max_time, self.timer)
         self.max_depth = MaxDepthLimit(max_depth, self.thread_manager)
         self.same_site_only = same_site_only
-        self._scraper = None
-        if scraper:
-            self.scraper = scraper
+        self._scrapers: list[CrawlScraper] = []
+        for scraper in scrapers:
+            self.register_scraper(scraper)
 
     @property
     def display_columns(self) -> list[ProgressColumn]:
         """The display columns to be used by the progress bar."""
         columns = list(Progress.get_default_columns())
         columns[3] = TimerColumn(True)
         return columns
@@ -356,28 +356,33 @@
             self.url_manager.uncrawled or self.thread_manager.unfinished_workers
         )
 
     @property
     @override
     def limits(self) -> list[CrawlLimit]:
         limits = super().limits
-        if self.scraper:
-            limits.extend(self.get_limits(self.scraper))
+        # ? Should scraper limits only halt that particular scraper or the whole crawl
+        # ? Separate class or flag to have both options
+        for scraper in self.scrapers:
+            limits.extend(self.get_limits(scraper))
         return limits
 
     @property
-    def scraper(self) -> CrawlScraper | None:
+    def scrapers(self) -> list[CrawlScraper]:
         """The scraper being used by this crawler."""
-        return self._scraper
+        return self._scrapers
 
-    @scraper.setter
-    def scraper(self, scraper: CrawlScraper):
-        """Set this scraper as the scraper to use and set this crawler's logger to be the scraper's logger."""
-        self._scraper = scraper
-        self._scraper.logger = self.logger
+    def register_scraper(self, scraper: CrawlScraper):
+        """
+        Add this `scraper` instance to the list of scrapers.
+
+        This `Crawler` instance's logger will be passed to the logger attribute of `scraper`.
+        """
+        scraper.logger = self.logger
+        self._scrapers.append(scraper)
 
     @property
     def starting_url(self) -> str:
         """The starting url of the last crawl."""
         return self._starting_url
 
     def _dispatch_workers(self, executor: ThreadPoolExecutor):
@@ -392,16 +397,16 @@
     def _handle_page(self, url: str):
         self.logger.info(f"Scraping `{url}`.")
         response = self.request_page(url)
         urls = self.extract_crawlable_urls(response.get_linkscraper())
         new_urls = self.url_manager.filter_urls(urls)
         self.logger.info(f"Found {len(new_urls)} new urls on `{url}`.")
         self.url_manager.add_urls(new_urls)
-        if self.scraper:
-            self.scraper.scrape(response)
+        for scraper in self.scrapers:
+            scraper.scrape(response)
 
     def print_exceeded_limits(self):
         for limit in self.exceeded_limits:
             self.logger.info(str(limit))
             console.print(limit)
 
     def crawl(self, starting_url: str):
@@ -446,24 +451,48 @@
     @override
     def postscrape_chores(self):
         self.timer.stop()
         self.logger.info(f"Crawl completed in {self.timer.elapsed_str}.")
         console.print(
             f"{color_map.sg3}Crawl completed in {color_map.go1}{self.timer.elapsed_str}[/]."
         )
-        if self.scraper:
-            self.scraper.postscrape_chores()
+        for scraper in self.scrapers:
+            scraper.postscrape_chores()
 
     @override
     def prescrape_chores(self):
         self.timer.start()
-        if self.scraper:
-            self.scraper.prescrape_chores()
+        for scraper in self.scrapers:
+            scraper.prescrape_chores()
         start_time = f"{datetime.now():%H:%M:%S}"
         self.logger.info(f"Starting crawl ({start_time}) at {self.starting_url}")
         console.print(
             f"Starting crawl ({color_map.go1}{start_time}[/]) at {color_map.or_}{self.starting_url}"
         )
 
     def request_page(self, url: str) -> Response:
         """Make a request to `url` and return the page."""
         return request(url, logger=self.logger)
+
+
+class SeleniumCrawler(Crawler):
+    """
+    Requires Firefox to be installed and for `geckodriver.exe` to be in system PATH.
+
+    Currently `max_threads` is hardcoded to `1`.
+    """
+
+    @override
+    def __init__(self, *args: Any, **kwargs: Any):
+        super().__init__(*args, **kwargs)
+        self.thread_manager = ThreadManager(1)
+        self.user = User(True)
+
+    @override
+    def request_page(self, url: str) -> SeleniumResponse:
+        self.user.get(url)
+        return SeleniumResponse.from_selenium_user(self.user)
+
+    @override
+    def crawl(self, starting_url: str):
+        super().crawl(starting_url)
+        self.user.close_browser()
```

### Comparing `gruel-4.0.0/src/gruel/requests.py` & `gruel-4.1.0/src/gruel/requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import requests
 import requests.adapters
 import requests.cookies
 import scrapetools
 import urllib3.util  # type: ignore
 from bs4 import BeautifulSoup
 from noiftimer import Timer
+from seleniumuser.seleniumuser import User
 from typing_extensions import Self, override
 from whosyouragent import whosyouragent
 
 
 class Response(requests.Response):
     """
     Override of `requests.Response` adding the following convenience methods:
@@ -35,14 +36,44 @@
     def from_base_response(cls, response: requests.Response) -> Self:
         """Convert a `requests.Response` object into a `gruel.Response` object."""
         self = cls()
         self.__dict__ = response.__dict__.copy()
         return self
 
 
+class SeleniumResponse(Response):
+    """
+    For mocking a `Response` type object from a `User` instance.
+
+    Only mocks `url` and `text` variables/properties.
+    """
+
+    def __init__(self, *args: Any, **kwargs: Any):
+        super().__init__(*args, **kwargs)
+        self._text = ""
+
+    @property
+    @override
+    def text(self) -> str:
+        return self._text
+
+    @classmethod
+    def from_selenium_user(cls, user: User) -> Self:
+        """
+        Construct a `Response` object from a `seleniumuser.User` instance.
+
+        Pass the `User` instance to this function after using the instance to request a page.
+        """
+        self = cls()
+        self.url = user.current_url()
+        assert user.browser
+        self._text = user.browser.page_source
+        return self
+
+
 retry_on_codes = [408, 413, 444, 499, 500, 502, 503, 504]
 
 
 class Session(requests.Session):
     @override
     def __init__(
         self,
```

### Comparing `gruel-4.0.0/src/gruel/subgruel.py` & `gruel-4.1.0/src/gruel/subgruel.py`

 * *Files identical despite different names*

### Comparing `gruel-4.0.0/src/gruel/template.py` & `gruel-4.1.0/src/gruel/template.py`

 * *Files identical despite different names*

### Comparing `gruel-4.0.0/LICENSE.txt` & `gruel-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gruel-4.0.0/pyproject.toml` & `gruel-4.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "gruel"
 description = "Another scraping framework"
-version = "4.0.0"
-dependencies = ["pathier", "printbuddies", "younotyou", "noiftimer", "requests", "whosyouragent", "quickpool", "loggi", "beautifulsoup4", "rich", "scrapetools", "typing_extensions", "urllib3"]
+version = "4.1.0"
+dependencies = ["pathier", "printbuddies", "younotyou", "noiftimer", "requests", "whosyouragent", "quickpool", "loggi", "beautifulsoup4", "rich", "scrapetools", "typing_extensions", "urllib3", "seleniumuser"]
 readme = "README.md"
 keywords = ["scrape", "scraping", "webscraping", "webscraper", "beautifulsoup", "framework"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 requires-python = ">=3.10, <=3.12"
 
 [[project.authors]]
 name = "Matt Manes"
```

### Comparing `gruel-4.0.0/PKG-INFO` & `gruel-4.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gruel
-Version: 4.0.0
+Version: 4.1.0
 Summary: Another scraping framework
 Project-URL: Homepage, https://github.com/matt-manes/gruel
 Project-URL: Documentation, https://github.com/matt-manes/gruel/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gruel/tree/main/src/gruel
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: beautifulsoup,framework,scrape,scraping,webscraper,webscraping
@@ -17,14 +17,15 @@
 Requires-Dist: noiftimer
 Requires-Dist: pathier
 Requires-Dist: printbuddies
 Requires-Dist: quickpool
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: scrapetools
+Requires-Dist: seleniumuser
 Requires-Dist: typing-extensions
 Requires-Dist: urllib3
 Requires-Dist: whosyouragent
 Requires-Dist: younotyou
 Description-Content-Type: text/markdown
 
 # gruel
```

