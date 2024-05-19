# Comparing `tmp/stockhero-0.4.8.tar.gz` & `tmp/stockhero-0.4.9.tar.gz`

## Comparing `stockhero-0.4.8.tar` & `stockhero-0.4.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 stockhero-0.4.8/requirements.txt
--rw-r--r--   0        0        0    27618 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/StockExchange.py
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/StockValuation.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/Ticker.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/__init__.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/__version__.py
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/Ticker_Sources/GuruFocusRequest.py
--rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/Ticker_Sources/MorningStarRequest.py
--rw-r--r--   0        0        0    24854 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/Ticker_Sources/NASDAQRequest.py
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/Ticker_Sources/StratosphereRequest.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/Ticker_Sources/TickerRequest.py
--rw-r--r--   0        0        0    42440 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/Ticker_Sources/TraderFoxRequest.py
--rw-r--r--   0        0        0    14446 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/Ticker_Sources/YahooRequest.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 stockhero-0.4.8/src/StockHero/Ticker_Sources/__init__.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 stockhero-0.4.8/tests/test_all_ticker_requests.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 stockhero-0.4.8/.gitignore
--rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 stockhero-0.4.8/LICENSE
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 stockhero-0.4.8/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 stockhero-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 stockhero-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 stockhero-0.4.9/requirements.txt
+-rw-r--r--   0        0        0     9222 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/StockExchange.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/Ticker.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/__init__.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/__version__.py
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/Ticker_Sources/GuruFocusRequest.py
+-rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/Ticker_Sources/MorningStarRequest.py
+-rw-r--r--   0        0        0    24854 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/Ticker_Sources/NASDAQRequest.py
+-rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/Ticker_Sources/StratosphereRequest.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/Ticker_Sources/TickerRequest.py
+-rw-r--r--   0        0        0    42440 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/Ticker_Sources/TraderFoxRequest.py
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/Ticker_Sources/YahooRequest.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 stockhero-0.4.9/src/StockHero/Ticker_Sources/__init__.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 stockhero-0.4.9/tests/test_all_ticker_requests.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 stockhero-0.4.9/.gitignore
+-rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 stockhero-0.4.9/LICENSE
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 stockhero-0.4.9/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 stockhero-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 stockhero-0.4.9/PKG-INFO
```

### Comparing `stockhero-0.4.8/src/StockHero/Ticker.py` & `stockhero-0.4.9/src/StockHero/Ticker.py`

 * *Files identical despite different names*

### Comparing `stockhero-0.4.8/src/StockHero/__version__.py` & `stockhero-0.4.9/src/StockHero/__version__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,29 @@
 #|  \__| $$  | $$|  \| $$__/ $$| $$_____ | $$$$$$\ | $$  | $$| $$$$$$$$| $$      | $$__/ $$
 # \$$    $$   \$$  $$ \$$    $$ \$$     \| $$  \$$\| $$  | $$ \$$     \| $$       \$$    $$
 #  \$$$$$$     \$$$$   \$$$$$$   \$$$$$$$ \$$   \$$ \$$   \$$  \$$$$$$$ \$$        \$$$$$$ 
 
 __title__ = 'StockHero'
 __description__ = 'stock market data downloader'
 __url__ = 'https://github.com/RobWen/StockHero'
-__version__ = '0.4.7'
+__version__ = '0.4.9'
 __author__ = 'RobWen'
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2022 - 2023'
 __thanks__ = 'Thanks to my colleagues @Fraunhofer IIS'
 
 '''
 Release History
+0.4.9 (02.09.2023)
+    - Readme überarbeitet
+    - Gurufocus PE Ratio überarbeitet (MMM, IFF, OTLY)
+    - Yahoo statistics_p rausgeworfen
+    - Suche bei Stratosphere eingeführt und der Name wird auch ausgegeben
+        - damit kann die GUI nochmal überarbeiten werden
+
 0.4.8 (28.08.2023)
     - added Dependencies
     - added Fear_and_Greed - API
     
 0.4.7 (24.08.2023)
     - changed Badge
     - Stratosphere Summary more features
```

### Comparing `stockhero-0.4.8/src/StockHero/Ticker_Sources/GuruFocusRequest.py` & `stockhero-0.4.9/src/StockHero/Ticker_Sources/GuruFocusRequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Aug 26 09:32:50 2022
 
 @author: RobWen
-Version: 0.4.5
+Version: 0.4.9
 """
 
 # Packages
 import requests
 from bs4 import BeautifulSoup
 import pandas as pd
 
@@ -59,18 +59,30 @@
             r = requests.get(f'https://www.gurufocus.com/term/pettm/{self.ticker}/PE-Ratio')
             page = BeautifulSoup(r.content, 'html.parser')
         
             table = page.find('div', {'class':'history_bar value'})
             
             try:
                 table = table.find('strong').text.split()
-                df = pd.DataFrame([table[1], table[3], table[5], table[7]]
-                                    ,  columns=[f"{self.ticker}'s PE Ratio Range Over the Past 10 Years"]
-                                    ,  index = [table[0], table[2], table[4], table[6]])
-                self.__PE_Ratio_Average = df
+                if len(table) == 8:
+                    df = pd.DataFrame([table[1], table[3], table[5], table[7]]
+                                        ,  columns=[f"{self.ticker}'s PE Ratio Range Over the Past 10 Years"]
+                                        ,  index = [table[0], table[2], table[4], table[6]])
+                    self.__PE_Ratio_Average = df
+                if table[1] == "At":
+                    df = pd.DataFrame([table[1] + " " + table[2], table[4], table[6], table[8] + " " + table[9]]
+                                        ,  columns=[f"{self.ticker}'s PE Ratio Range Over the Past 10 Years"]
+                                        ,  index = [table[0], table[3], table[5], table[7]])
+                    self.__PE_Ratio_Average = df
+                if len(table) == 12:
+                    df = pd.DataFrame([table[1] + " " + table[2], table[4] + " " + table[5], table[7] + " " + table[8], 
+                                       table[10] + " " + table[11]]
+                                        ,  columns=[f"{self.ticker}'s PE Ratio Range Over the Past 10 Years"]
+                                        ,  index = [table[0], table[3], table[6], table[9]])
+                    self.__PE_Ratio_Average = df
                 return self.__PE_Ratio_Average
             except:
                 return None
         #else:
         #    return None
         
     def __gurufocus_debt_to_ebitda(self):
```

### Comparing `stockhero-0.4.8/src/StockHero/Ticker_Sources/MorningStarRequest.py` & `stockhero-0.4.9/src/StockHero/Ticker_Sources/MorningStarRequest.py`

 * *Files identical despite different names*

### Comparing `stockhero-0.4.8/src/StockHero/Ticker_Sources/NASDAQRequest.py` & `stockhero-0.4.9/src/StockHero/Ticker_Sources/NASDAQRequest.py`

 * *Files identical despite different names*

### Comparing `stockhero-0.4.8/src/StockHero/Ticker_Sources/StratosphereRequest.py` & `stockhero-0.4.9/src/StockHero/Ticker_Sources/StratosphereRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Aug 17 10:53:30 2023
 
 @author: rwenzel
-Version: 0.4.7
+Version: 0.4.9
 """
 
 # Packages
 import pandas as pd
 import requests
+from urllib.parse import urlencode
 from bs4 import BeautifulSoup
 import numpy as np
 
 # Header
 from .TickerRequest import *
 
 class StratosphereRequest(TickerRequest):
     def __init__(self, ticker, headers_standard):
         super().__init__(ticker, headers_standard)
         self.__headers_standard = headers_standard
-        
-    ################################
-    ###                          ###
-    ###  Stratosphere Requests   ###
-    ###                          ###
-    ################################
+         
+    ###########################
+    ###                     ###
+    ###    Stratosphere     ###
+    ###      Requests       ###
+    ###                     ###
+    ###########################
     
     @property
     def basic(self):
         return self.__stratosphere_basic_abfrage()
     
     @property
     def margins(self):
@@ -60,15 +62,16 @@
     
     @property
     def summary(self):
         return self.__stratosphere_summary_abfrage()
     
     ###########################
     ###                     ###
-    ###  Stratosphere Data  ###
+    ###    Stratosphere     ###
+    ###        Dummy        ###
     ###                     ###
     ###########################
     
     # Dummy Abfragen, um Fehler im Vorfeld abzufangen
     def __stratosphere_basic_abfrage(self):
         
         if self.ticker is None or self.ticker == '':
@@ -137,23 +140,66 @@
         
         if self.ticker is None or self.ticker == '':
             self.ticker = 'None'
             return None
         
         return self.__stratosphere_summary_df()
     
+    ###########################
+    ###                     ###
+    ###     Stratosphere    ###
+    ###    Help functions   ###
+    ###                     ###
+    ###########################
+    
     # Hilfsfunktionen 
     def __initialize_dataframe(self, index):
         df = pd.DataFrame([''], columns=["Summary"], index=index)
         return df
+
+    ###########################
+    ###                     ###
+    ###     Stratosphere    ###
+    ###        Search       ###
+    ###                     ###
+    ###########################
+
+    # Suche bei https://www.stratosphere.io/
+    def __stratosphere_identifier(self):
+        
+        params = {
+            "x-algolia-agent": "Algolia for JavaScript (5.0.0-alpha.73); Search (5.0.0-alpha.73); Browser",
+            "x-algolia-api-key": "f490c20728b7866fc81c7b6e3d7e0e2b",
+            "x-algolia-application-id": "ZPBCEGHCCC",
+        }
+        
+        url = "https://zpbceghccc-dsn.algolia.net/1/indexes/*/queries?" + urlencode(params)
+
+        try:
+            data = {"requests":[{"indexName":"companies","query":f"{self.ticker}","hitsPerPage":1,"tagFilters":["Stratosphere"]}]}
+            page = requests.post(url, json=data)
+            json = page.json()
+            self.__identifier = json["results"][0]["hits"][0]["identifier"]
+            self.name = json["results"][0]["hits"][0]["name"]
+        except:
+            return None
+        
+        return self.__identifier
+
+    ###########################
+    ###                     ###
+    ###     Stratosphere    ###
+    ###         Data        ###
+    ###                     ###
+    ###########################
     
     # Eigentlichen Abfragen
     def __stratosphere_data_dict(self):
         
-        url = f'https://www.stratosphere.io/company/{self.ticker}/'
+        url = f'https://www.stratosphere.io/company/{self.__stratosphere_identifier()}/'
 
         page = requests.get(url)
         
         if page.status_code != 200:
             return None
         
         page = BeautifulSoup(page.content, 'html.parser')
```

### Comparing `stockhero-0.4.8/src/StockHero/Ticker_Sources/TraderFoxRequest.py` & `stockhero-0.4.9/src/StockHero/Ticker_Sources/TraderFoxRequest.py`

 * *Files identical despite different names*

### Comparing `stockhero-0.4.8/tests/test_all_ticker_requests.py` & `stockhero-0.4.9/tests/test_all_ticker_requests.py`

 * *Files identical despite different names*

### Comparing `stockhero-0.4.8/.gitignore` & `stockhero-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `stockhero-0.4.8/LICENSE` & `stockhero-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stockhero-0.4.8/README.md` & `stockhero-0.4.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # StockHero  
 ## Download market data from finance APIs and other sources
 > It's an open-source tool that uses publicly available APIs and other sources, and is intended for research and educational purposes only.<br>
 > If you find a bug, try fix it yourself first
   
 [![Downloads](https://static.pepy.tech/badge/StockHero)](https://pepy.tech/project/StockHero)
 
-## New Features in 0.4.8
+> [!IMPORTANT]
+> The library was crafted by a Large Language Model, no programmer was hurt during the process
+
+<br>
+
+## New Features in 0.4.9
 * Minor fixes
 
 ### New Features planned for the next release
 - fix more "features" (bugs)
 
 ## The Ticker module
 The ```Ticker``` module, gets the financial data from nasdaq.com, morningstar.com, yahoo.com as a pandas.DataFrame <br>
@@ -17,29 +22,23 @@
 ```python
 
 import StockHero as stock
 nvda = stock.Ticker('NVDA') # e.g. NVIDIA Corp
 #or
 nvda = stock.Ticker('US67066G1040') # e.g. NVIDIA Corp
 
-''' Morningstar '''
+''' Morningstar API '''
 nvda.morningstar.quote                  # Quote
 nvda.morningstar.key_statistics         # Key Statistics (combination of the ones below)
 nvda.morningstar.growth_rev             # Growth - Revenue %
 nvda.morningstar.growth_op_inc          # Growth - Operating Income %
 nvda.morningstar.growth_net_inc         # Growth - Net Income %
 nvda.morningstar.growth_eps             # Growth - EPS %
 
-''' Yahoo Finance '''
-## I would recommend to use yfinance instead of this library ##
-
-nvda.yahoo.statistics                   # Statistics
-nvda.yahoo.statistics_p                 # Statistics - PreProcessed
-
-''' NASDAQ '''
+''' NASDAQ API '''
 nvda.nasdaq.summ                        # Summary
 nvda.nasdaq.div_hist                    # Dividend History
 nvda.nasdaq.hist_quotes_stock           # Historical Quotes for Stocks
 nvda.nasdaq.hist_quotes_etf             # Historical Quotes for ETFs
 nvda.nasdaq.hist_nocp                   # Historical Nasdaq Official Closing Price (NOCP)
 nvda.nasdaq.fin_income_statement_y      # Financials - Income Statement - Yearly
 nvda.nasdaq.fin_balance_sheet_y         # Financials - Balance Sheet    - Yearly
@@ -51,32 +50,30 @@
 nvda.nasdaq.fin_fin_ratios_q            # Financials - Financial Ratios - Quarterly
 nvda.nasdaq.earn_date_eps               # Earnings Date - Earnings Per Share
 nvda.nasdaq.earn_date_surprise          # Earnings Date - Quarterly Earnings Surprise Amount
 nvda.nasdaq.yearly_earn_forecast        # Earnings Date - Yearly Earnings Forecast 
 nvda.nasdaq.quarterly_earn_forecast     # Earnings Date - Quarterly Earnings Forecast 
 nvda.nasdaq.pe_peg_forecast             # Price/Earnings, PEG Ratios, Growth Rates Forecast
 
-''' Gurufocus '''
-nvda.gurufocus.pe_ratio_av              # Historical Average Price/Earnings-Ratio
-nvda.gurufocus.debt_to_ebitda           # Debt-to-EBITDA Ratio
 ```
 
 ## The StockExchange module
 The ```StockExchange``` module, gets the financial data from the NASDAQ Stock Screener <br>
 Added CNN Fear and Greed Index
 
 ```python
 import StockHero as stock
 t = stock.StockExchange('something') # e.g. Nasdaq
 
-''' NASDAQ '''
+''' NASDAQ API '''
 t.nasdaq                              # Nasdaq Stock Market
 
-''' CNN '''
+''' CNN API '''
 t.cnn_fear_and_greed                  # CNN Fear and Greed Index
+t.cnn_fear_and_greed_graph_data       # CNN Fear and Greed Graph API
 ```
 
 ## Combining both modules
 You can combine both modules, for example
 ```python
 import StockHero as stock
 t = stock.StockExchange('something')
@@ -91,10 +88,10 @@
 <br>
 ### Any feedback or suggestions, let me know
 Or in the words of Peter Thiel:
 > We wanted flying cars, instead we got 140 characters
 <br>
 ### Versions
 
-0.4.8  Minor fixes <br>
+0.4.9  Minor fixes <br>
 ... <br>
 0.0.1  First Release
```

### Comparing `stockhero-0.4.8/pyproject.toml` & `stockhero-0.4.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "StockHero"
-version = "0.4.8"
+version = "0.4.9"
 authors = [{ name = "RobWen"}]
 maintainers = [{ name = "asti205"}]
 description = "market data from finance APIs and other publicy available sources"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `stockhero-0.4.8/PKG-INFO` & `stockhero-0.4.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StockHero
-Version: 0.4.8
+Version: 0.4.9
 Summary: market data from finance APIs and other publicy available sources
 Author: RobWen
 Maintainer: asti205
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,20 @@
 # StockHero  
 ## Download market data from finance APIs and other sources
 > It's an open-source tool that uses publicly available APIs and other sources, and is intended for research and educational purposes only.<br>
 > If you find a bug, try fix it yourself first
   
 [![Downloads](https://static.pepy.tech/badge/StockHero)](https://pepy.tech/project/StockHero)
 
-## New Features in 0.4.8
+> [!IMPORTANT]
+> The library was crafted by a Large Language Model, no programmer was hurt during the process
+
+<br>
+
+## New Features in 0.4.9
 * Minor fixes
 
 ### New Features planned for the next release
 - fix more "features" (bugs)
 
 ## The Ticker module
 The ```Ticker``` module, gets the financial data from nasdaq.com, morningstar.com, yahoo.com as a pandas.DataFrame <br>
@@ -34,29 +39,23 @@
 ```python
 
 import StockHero as stock
 nvda = stock.Ticker('NVDA') # e.g. NVIDIA Corp
 #or
 nvda = stock.Ticker('US67066G1040') # e.g. NVIDIA Corp
 
-''' Morningstar '''
+''' Morningstar API '''
 nvda.morningstar.quote                  # Quote
 nvda.morningstar.key_statistics         # Key Statistics (combination of the ones below)
 nvda.morningstar.growth_rev             # Growth - Revenue %
 nvda.morningstar.growth_op_inc          # Growth - Operating Income %
 nvda.morningstar.growth_net_inc         # Growth - Net Income %
 nvda.morningstar.growth_eps             # Growth - EPS %
 
-''' Yahoo Finance '''
-## I would recommend to use yfinance instead of this library ##
-
-nvda.yahoo.statistics                   # Statistics
-nvda.yahoo.statistics_p                 # Statistics - PreProcessed
-
-''' NASDAQ '''
+''' NASDAQ API '''
 nvda.nasdaq.summ                        # Summary
 nvda.nasdaq.div_hist                    # Dividend History
 nvda.nasdaq.hist_quotes_stock           # Historical Quotes for Stocks
 nvda.nasdaq.hist_quotes_etf             # Historical Quotes for ETFs
 nvda.nasdaq.hist_nocp                   # Historical Nasdaq Official Closing Price (NOCP)
 nvda.nasdaq.fin_income_statement_y      # Financials - Income Statement - Yearly
 nvda.nasdaq.fin_balance_sheet_y         # Financials - Balance Sheet    - Yearly
@@ -68,32 +67,30 @@
 nvda.nasdaq.fin_fin_ratios_q            # Financials - Financial Ratios - Quarterly
 nvda.nasdaq.earn_date_eps               # Earnings Date - Earnings Per Share
 nvda.nasdaq.earn_date_surprise          # Earnings Date - Quarterly Earnings Surprise Amount
 nvda.nasdaq.yearly_earn_forecast        # Earnings Date - Yearly Earnings Forecast 
 nvda.nasdaq.quarterly_earn_forecast     # Earnings Date - Quarterly Earnings Forecast 
 nvda.nasdaq.pe_peg_forecast             # Price/Earnings, PEG Ratios, Growth Rates Forecast
 
-''' Gurufocus '''
-nvda.gurufocus.pe_ratio_av              # Historical Average Price/Earnings-Ratio
-nvda.gurufocus.debt_to_ebitda           # Debt-to-EBITDA Ratio
 ```
 
 ## The StockExchange module
 The ```StockExchange``` module, gets the financial data from the NASDAQ Stock Screener <br>
 Added CNN Fear and Greed Index
 
 ```python
 import StockHero as stock
 t = stock.StockExchange('something') # e.g. Nasdaq
 
-''' NASDAQ '''
+''' NASDAQ API '''
 t.nasdaq                              # Nasdaq Stock Market
 
-''' CNN '''
+''' CNN API '''
 t.cnn_fear_and_greed                  # CNN Fear and Greed Index
+t.cnn_fear_and_greed_graph_data       # CNN Fear and Greed Graph API
 ```
 
 ## Combining both modules
 You can combine both modules, for example
 ```python
 import StockHero as stock
 t = stock.StockExchange('something')
@@ -108,10 +105,10 @@
 <br>
 ### Any feedback or suggestions, let me know
 Or in the words of Peter Thiel:
 > We wanted flying cars, instead we got 140 characters
 <br>
 ### Versions
 
-0.4.8  Minor fixes <br>
+0.4.9  Minor fixes <br>
 ... <br>
 0.0.1  First Release
```

