# Comparing `tmp/py_alpaca_daily_losers-0.1.1.tar.gz` & `tmp/py_alpaca_daily_losers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_daily_losers-0.1.1.tar", max compression
+gzip compressed data, was "py_alpaca_daily_losers-0.2.0.tar", max compression
```

## Comparing `py_alpaca_daily_losers-0.1.1.tar` & `py_alpaca_daily_losers-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2024-05-18 22:45:52.968768 py_alpaca_daily_losers-0.1.1/LICENSE
--rw-r--r--   0        0        0    13494 2024-05-18 22:35:14.428880 py_alpaca_daily_losers-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-18 17:16:27.292173 py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/__init__.py
--rw-r--r--   0        0        0    18043 2024-05-18 22:51:12.078715 py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/daily_losers.py
--rw-r--r--   0        0        0        0 2024-05-18 17:18:38.222152 py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/src/__init__.py
--rw-r--r--   0        0        0     1103 2024-05-18 21:16:37.509688 py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/src/article_extractor.py
--rw-r--r--   0        0        0      460 2024-05-18 20:41:18.600056 py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/src/global_fuctions.py
--rw-r--r--   0        0        0      736 2024-05-18 20:12:35.110354 py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/src/marketaux.py
--rw-r--r--   0        0        0     2082 2024-05-18 18:20:18.541515 py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/src/openai.py
--rw-r--r--   0        0        0     1877 2024-05-18 18:28:49.471426 py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/src/slack.py
--rw-r--r--   0        0        0      495 2024-05-18 22:51:51.188709 py_alpaca_daily_losers-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14156 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.0/LICENSE
+-rw-r--r--   0        0        0    13887 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/__init__.py
+-rw-r--r--   0        0        0    19580 2024-05-19 19:00:43.120319 py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/daily_losers.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/src/__init__.py
+-rw-r--r--   0        0        0     1407 2024-05-19 19:01:05.570313 py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/src/article_extractor.py
+-rw-r--r--   0        0        0      481 2024-05-19 15:45:30.783151 py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/src/global_fuctions.py
+-rw-r--r--   0        0        0      936 2024-05-19 19:01:28.900310 py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/src/marketaux.py
+-rw-r--r--   0        0        0     2183 2024-05-19 15:58:13.033135 py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/src/openai.py
+-rw-r--r--   0        0        0     1941 2024-05-19 15:58:22.013134 py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/src/slack.py
+-rw-r--r--   0        0        0      692 2024-05-19 19:04:44.310272 py_alpaca_daily_losers-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14549 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.2.0/PKG-INFO
```

### Comparing `py_alpaca_daily_losers-0.1.1/LICENSE` & `py_alpaca_daily_losers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.1.1/README.md` & `py_alpaca_daily_losers-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 </details>
 <hr>
 
 ##  Overview
 
 The py-alpaca-daily-losers project integrates Alpaca Markets for a daily losers strategy, offering market data extraction, AI analysis, and Slack notifications. The core functionality centers on retrieving and analyzing daily stock market data using indicators like Bollinger Bands and RSI. It provides insights through news extraction, sentiment analysis, and chat functions via OpenAI integration. This project equips users with robust data analysis tools for informed decision-making in the stock market.
 
+This project is in no way trading advice, or a vaild strategy. Any trading done using this package should only be on a paper account, until proven to work.
+
+Visit [PyAlpacaApi](https://github.com/TexasCoding/py-alpaca-api) to learn more about the core of this project.
+
+Visit [AlpacaApiStrategies](https://github.com/TexasCoding/alpaca-api-strategies) for an example app using this strategy.
+
 ---
 
 ##  Features
 
 |    |   Feature         | Description |
 |----|-------------------|---------------------------------------------------------------|
 | ⚙️  | **Architecture**  | The project has a modular architecture that integrates various components for market data extraction, AI analysis, and Slack notifications. It leverages external APIs effectively within its architecture. |
```

### Comparing `py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/daily_losers.py` & `py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/daily_losers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import os
 import pandas as pd
 from py_alpaca_api.alpaca import PyAlpacaApi
 
 from .src.marketaux import MarketAux
 from .src.article_extractor import ArticleExtractor
 from .src.openai import OpenAIAPI
-from .src.global_fuctions import *
+from .src.global_fuctions import send_message
 
 from ta.volatility import BollingerBands
 from ta.momentum import RSIIndicator
 
 from tqdm import tqdm
-
+from dotenv import load_dotenv
 from datetime import datetime
 from datetime import timedelta
 from pytz import timezone
 
-tz = timezone('US/Eastern')
+tz = timezone("US/Eastern")
 ctime = datetime.now(tz)
 today = ctime.strftime("%Y-%m-%d")
 previous_day = (ctime - timedelta(days=1)).strftime("%Y-%m-%d")
 year_ago = (ctime - timedelta(days=365)).strftime("%Y-%m-%d")
 
-from dotenv import load_dotenv
+
 load_dotenv()
 
-api_key=str(os.getenv('API_KEY'))
-api_secret=str(os.getenv('API_SECRET'))
-api_paper=True if os.getenv('API_PAPER') == 'True' else False
+api_key = str(os.getenv("API_KEY"))
+api_secret = str(os.getenv("API_SECRET"))
+api_paper = True if os.getenv("API_PAPER") == "True" else False
+
 
 class DailyLosers:
     def __init__(self):
-        self.alpaca = PyAlpacaApi(api_key=api_key, api_secret=api_secret, api_paper=api_paper)
-        self.production = True if os.getenv('PRODUCTION') == 'True' else False
+        self.alpaca = PyAlpacaApi(
+            api_key=api_key, api_secret=api_secret, api_paper=api_paper
+        )
+        self.production = True if os.getenv("PRODUCTION") == "True" else False
 
     def run(self):
         """
         Run the daily losers strategy
         """
         # Sell the positions based on the sell criteria
         self.sell_positions_from_criteria()
@@ -56,277 +59,368 @@
         return: False if market is closed or there are no stocks to sell
         """
         print("Selling positions based on sell criteria")
         # Get the sell opportunities
         sell_opportunities = self.get_sell_opportunities()
         # Get the current positions
         current_positions = self.alpaca.position.get_all()
-        sold_positions = [] 
+        sold_positions = []
         # Iterate through the sell opportunities and sell the stocks
         for symbol in sell_opportunities:
             # Try to sell the stock
             try:
                 # Get the quantity of the stock to sell
-                qty = current_positions[current_positions['symbol'] == symbol]['qty'].values[0]
+                qty = current_positions[current_positions["symbol"] == symbol][
+                    "qty"
+                ].values[0]
                 if self.alpaca.market.clock().is_open:
-                    self.alpaca.order.market(symbol=symbol, qty=qty, side='sell')
+                    self.alpaca.order.market(
+                        symbol=symbol, qty=qty, side="sell"
+                    )
             # If there is an error, print or send a slack message
             except Exception as e:
                 send_message(f"Error selling {symbol}: {e}")
                 continue
             # If the order was successful, append the sold position to the sold_positions list
             else:
-                sold_positions.append({'symbol': symbol, 'qty': qty})
+                sold_positions.append({"symbol": symbol, "qty": qty})
 
         # Print or send slack messages of the sold positions
         if not sold_positions:
             # If no positions were sold, create the message
             sold_message = "No positions to sell"
         else:
             # If positions were sold, create the message
-            sold_message = "Successfully{} sold the following positions:\n".format(" pretend" if not self.alpaca.market.clock().is_open else "")
+            sold_message = (
+                "Successfully{} sold the following positions:\n".format(
+                    " pretend"
+                    if not self.alpaca.market.clock().is_open
+                    else ""
+                )
+            )
             for position in sold_positions:
-                sold_message += "{qty} shares of {symbol}\n".format(qty=position['qty'], symbol=position['symbol'])
+                sold_message += "{qty} shares of {symbol}\n".format(
+                    qty=position["qty"], symbol=position["symbol"]
+                )
         # Print or send the message
         send_message(sold_message)
 
     ########################################################
     # Define the get_sell_opportunities function
     ########################################################
-    def get_sell_opportunities(self):
+    def get_sell_opportunities(self) -> list:
         """
         Get the sell assets opportunities based on the RSI and Bollinger Bands
         return: List of sell opportunities
         """
         # Get the current positions from the Alpaca API
         current_positions = self.alpaca.position.get_all()
-        if current_positions[current_positions['symbol'] != 'Cash'].empty:
+        if current_positions[current_positions["symbol"] != "Cash"].empty:
             return []
         # Get the symbols from the current positions that are not cash
-        current_positions_symbols   = current_positions[current_positions['symbol'] != 'Cash']['symbol'].tolist()
+        current_positions_symbols = current_positions[
+            current_positions["symbol"] != "Cash"
+        ]["symbol"].tolist()
         # Get the assets history from the Yahoo API
-        assets_history              = self.get_ticker_data(current_positions_symbols)
+        assets_history = self.get_ticker_data(current_positions_symbols)
         # Get the sell criteria
-        sell_criteria = ((assets_history[['rsi14', 'rsi30', 'rsi50', 'rsi200']] >= 70).any(axis=1)) | \
-                            ((assets_history[['bbhi14', 'bbhi30', 'bbhi50', 'bbhi200']] == 1).any(axis=1))
+        sell_criteria = (
+            (assets_history[["rsi14", "rsi30", "rsi50", "rsi200"]] >= 70).any(
+                axis=1
+            )
+        ) | (
+            (
+                assets_history[["bbhi14", "bbhi30", "bbhi50", "bbhi200"]] == 1
+            ).any(axis=1)
+        )
         # Get the filtered positions based on the sell criteria
         sell_filtered_df = assets_history[sell_criteria]
         # Get the symbol list from the filtered positions
-        return sell_filtered_df['symbol'].tolist()
-    
+        return sell_filtered_df["symbol"].tolist()
+
     ########################################################
     # Define the liquidate_positions_for_capital function
     ########################################################
     def liquidate_positions_for_capital(self):
         """
         Liquidate the positions to make cash 10% of the portfolio
         The strategy is to sell the top 25% of performing stocks evenly to make cash 10% of total portfolio
         return: True if the function is successful
         return: False if the market is closed or there are no stocks to sell
         """
-        print("Liquidating positions for capital to make cash 10% of the portfolio")
+        print(
+            "Liquidating positions for capital to make cash 10% of the portfolio"
+        )
         # Get the current positions from the Alpaca API
         current_positions = self.alpaca.position.get_all()
         if current_positions.empty:
             sold_message = "No positions available to liquidate for capital"
             send_message(sold_message)
             return
         # Get the cash available from the Alpaca API
-        #cash_available = float(self.alpaca.get_account().cash)
-        cash_row = current_positions[current_positions['symbol'] == 'Cash']
-   
+        # cash_available = float(self.alpaca.get_account().cash)
+        cash_row = current_positions[current_positions["symbol"] == "Cash"]
+
         # Get the total holdings from the current positions and cash available
-        total_holdings  = current_positions['market_value'].sum()
+        total_holdings = current_positions["market_value"].sum()
 
         sold_positions = []
         # If the cash is less than 10% of the total holdings, liquidate the top 25% of performing stocks to make cash 10% of the portfolio
-        if cash_row['market_value'][0] / total_holdings < 0.1:
+        if cash_row["market_value"][0] / total_holdings < 0.1:
             # Sort the positions by profit percentage
-            current_positions = current_positions[current_positions['symbol'] != 'Cash'].sort_values(by='profit_pct', ascending=False) 
+            current_positions = current_positions[
+                current_positions["symbol"] != "Cash"
+            ].sort_values(by="profit_pct", ascending=False)
             # Sell the top 25% of performing stocks evenly to make cash 10% of total portfolio
-            top_performers              = current_positions.iloc[:int(len(current_positions) // 2)]
-            top_performers_market_value = top_performers['market_value'].sum()
-            cash_needed                 = total_holdings * 0.1 - cash_row['market_value'][0]
+            top_performers = current_positions.iloc[
+                : int(len(current_positions) // 2)
+            ]
+            top_performers_market_value = top_performers["market_value"].sum()
+            cash_needed = total_holdings * 0.1 - cash_row["market_value"][0]
 
             # Sell the top performers to make cash 10% of the portfolio
             for index, row in top_performers.iterrows():
-                print(f"Selling {row['symbol']} to make cash 10% portfolio cash requirement")
+                print(
+                    f"Selling {row['symbol']} to make cash 10% portfolio cash requirement"
+                )
                 # Calculate the quantity to sell from the top performers
-                #amount_to_sell = float((row['market_value'] / top_performers_market_value) * cash_needed)
-                amount_to_sell = int((row['market_value'] / top_performers_market_value) * cash_needed)
+                # amount_to_sell = float((row['market_value'] / top_performers_market_value) * cash_needed)
+                amount_to_sell = int(
+                    (row["market_value"] / top_performers_market_value)
+                    * cash_needed
+                )
                 # If the amount to sell is 0, continue to the next stock
                 if amount_to_sell == 0:
                     continue
 
                 # Market sell the stock
                 try:
                     # Market sell the stock if the market is open
                     if self.alpaca.market.clock().is_open:
-                        self.alpaca.order.market(symbol=row['symbol'], notional=amount_to_sell, side='sell')
+                        self.alpaca.order.market(
+                            symbol=row["symbol"],
+                            notional=amount_to_sell,
+                            side="sell",
+                        )
                 # If there is an error, print or send a slack message
                 except Exception as e:
-                        send_message(f"Error selling {row['symbol']}: {e}")
-                        continue
+                    send_message(f"Error selling {row['symbol']}: {e}")
+                    continue
                 # If the order was successful, append the sold position to the sold_positions list
                 else:
-                    sold_positions.append({'symbol': row['symbol'], 'notional': round(amount_to_sell, 2)})
+                    sold_positions.append(
+                        {
+                            "symbol": row["symbol"],
+                            "notional": round(amount_to_sell, 2),
+                        }
+                    )
         # Print or send slack messages of the sold positions
         if not sold_positions:
             # If no positions were sold, create the message
             sold_message = "No positions liquidated for capital"
         else:
             # If positions were sold, create the message
             # Pretend trades if the market is closed
-            sold_message = "Successfully{} liquidated the following positions:\n".format(" pretend" if not self.alpaca.market.clock().is_open else "")
+            sold_message = (
+                "Successfully{} liquidated the following positions:\n".format(
+                    " pretend"
+                    if not self.alpaca.market.clock().is_open
+                    else ""
+                )
+            )
             for position in sold_positions:
-                sold_message += "Sold ${qty} of {symbol}\n".format(qty=position['notional'], symbol=position['symbol'])
+                sold_message += "Sold ${qty} of {symbol}\n".format(
+                    qty=position["notional"], symbol=position["symbol"]
+                )
         # Print or send the message
         send_message(sold_message)
 
     ########################################################
     # Define the check_for_buy_opportunities function
     ########################################################
     def check_for_buy_opportunities(self):
         losers = self.get_daily_losers()
         ticker_data = self.get_ticker_data(losers)
         filter_tickers = self.buy_criteria(ticker_data)
-        news_filtered_tickers = self.filter_tickers_with_news(filter_tickers)
-        self.open_posistions(news_filtered_tickers)
+        self.filter_tickers_with_news(filter_tickers)
+        self.open_posistions()
 
     ########################################################
     # Define the open_posistions function
     ########################################################
-    def open_posistions(self, limit: int=8):
+    def open_posistions(self, ticker_limit=8):
         """
         Buy the stocks based on the buy opportunities, limit to 8 stocks by default
         Should only be run at market open
         Send a slack message with the bought positions, or print the bought positions
         """
-        print("Buying orders based on buy opportunities and openai sentiment. Limit to 8 stocks by default")
+        print(
+            "Buying orders based on buy opportunities and openai sentiment. Limit to 8 stocks by default"
+        )
         # Get the tickers from the get_ticker_info function and convert symbols to a list
-        tickers = self.alpaca.watchlist.get_assets(watchlist_name="DailyLosers")
+        tickers = self.alpaca.watchlist.get_assets(
+            watchlist_name="DailyLosers"
+        )
+
         # Get the available cash from the Alpaca API
         available_cash = self.alpaca.account.get().cash
-        ticker_count = len(tickers)
+
         # This is the amount to buy for each stock
-        if ticker_count == 0:
+        if len(tickers) == 0:
             notional = 0
         else:
-            notional = (available_cash / ticker_count) - 1
-            
+            notional = (available_cash / len(tickers[:ticker_limit])) - 1
+
         bought_positions = []
         # Iterate through the tickers and buy the stocks
-        for ticker in tickers[:ticker_count]:
+        for ticker in tickers[:ticker_limit]:
             # Market buy the stock
             try:
                 if self.alpaca.market.clock().is_open:
-                    #print(f"Buying {ticker} with notional amount of {notional}")
+                    # print(f"Buying {ticker} with notional amount of {notional}")
                     self.alpaca.order.market(symbol=ticker, notional=notional)
             # If there is an error, print or send a slack message
             except Exception as e:
                 send_message(f"Error buying {ticker}: {e}")
                 continue
             else:
-                bought_positions.append({'symbol': ticker, 'notional': round(notional, 2)})
+                bought_positions.append(
+                    {"symbol": ticker, "notional": round(notional, 2)}
+                )
         # Print or send slack messages of the bought positions
         if not bought_positions:
             # If no positions were bought, create the message
             bought_message = "No positions bought"
         else:
             # If positions were bought, create the message
-            bought_message = "Successfully{} bought the following positions:\n".format(" pretend" if not self.alpaca.market.clock().is_open else "")
+            bought_message = (
+                "Successfully{} bought the following positions:\n".format(
+                    " pretend"
+                    if not self.alpaca.market.clock().is_open
+                    else ""
+                )
+            )
             for position in bought_positions:
-                bought_message += "${qty} of {symbol}\n".format(qty=position['notional'], symbol=position['symbol'])
+                bought_message += "${qty} of {symbol}\n".format(
+                    qty=position["notional"], symbol=position["symbol"]
+                )
         # Print or send the message
         send_message(bought_message)
 
     ########################################################
     # Define the filter_tickers_with_news function
     ########################################################
-    def filter_tickers_with_news(self, tickers) -> list[str]:
+    def filter_tickers_with_news(self, tickers) -> list:
         news = MarketAux()
         article = ArticleExtractor()
         openai = OpenAIAPI()
         filtered_tickers = []
-        
+
         for i, ticker in tqdm(
             enumerate(tickers),
             desc=f"• Analizing news for {len(tickers)} tickers, using OpenAI & MarketAux: ",
         ):
             m_news = news.get_symbol_news(symbol=ticker)
             articles = article.extract_articles(m_news)
 
             if len(articles) > 0:
-                bullish=0
-                bearish=0
+                bullish = 0
+                bearish = 0
                 for art in articles:
-                    sentiment = openai.get_sentiment_analysis(title=art['title'], symbol=ticker, article=art['content'])
+                    sentiment = openai.get_sentiment_analysis(
+                        title=art["title"],
+                        symbol=ticker,
+                        article=art["content"],
+                    )
                     if sentiment == "BULLISH":
-                        bullish+=1
+                        bullish += 1
                     else:
-                        bearish+=1
-            if bullish > bearish:
-                filtered_tickers.append(ticker)
+                        bearish += 1
+
+                if bullish > bearish:
+                    filtered_tickers.append(ticker)
 
         if len(filtered_tickers) == 0:
             print("No tickers with news found")
+            return []
 
         try:
-            self.alpaca.watchlist.update(watchlist_name="DailyLosers", symbols=','.join(filtered_tickers))
+            self.alpaca.watchlist.update(
+                watchlist_name="DailyLosers",
+                symbols=",".join(filtered_tickers),
+            )
         except Exception:
-            self.alpaca.watchlist.create(name=f"DailyLosers", symbols=','.join(filtered_tickers))
-
-        tickers = self.alpaca.watchlist.get_assets(watchlist_name="DailyLosers")
+            self.alpaca.watchlist.create(
+                name="DailyLosers", symbols=",".join(filtered_tickers)
+            )
+
+        tickers = self.alpaca.watchlist.get_assets(
+            watchlist_name="DailyLosers"
+        )
 
         return tickers
 
     ########################################################
     # Define the get_daily_losers function
     ########################################################
-    def get_daily_losers(self) -> list[str]:
-        losers = self.alpaca.screener.losers()['symbol'].to_list()
+    def get_daily_losers(self) -> list:
+        losers = self.alpaca.screener.losers()["symbol"].to_list()
         try:
             watchlist = self.alpaca.watchlist.get(watchlist_name="DailyLosers")
         except Exception:
-            watchlist = self.alpaca.watchlist.create(name=f"DailyLosers", symbols=','.join(losers))
+            watchlist = self.alpaca.watchlist.create(
+                name="DailyLosers", symbols=",".join(losers)
+            )
         else:
             if watchlist.updated_at.strftime("%Y-%m-%d") != today:
-                watchlist = self.alpaca.watchlist.update(watchlist_name=f"DailyLosers", symbols=','.join(losers))
+                watchlist = self.alpaca.watchlist.update(
+                    watchlist_name="DailyLosers", symbols=",".join(losers)
+                )
             else:
                 print(f"Watchlist already updated today: {today}")
 
-        return self.alpaca.watchlist.get_assets(watchlist_name="DailyLosers") 
-    
+        return self.alpaca.watchlist.get_assets(watchlist_name="DailyLosers")
+
     ########################################################
     # Define the buy_criteria function
     ########################################################
-    def buy_criteria(self, data) -> list[str]:
+    def buy_criteria(self, data) -> list:
         """
         Get the buy criteria for the stock
         :param data: DataFrame: stock data
         :return: list: tickers
         """
         # Filter the DataFrame based on the buy criteria
         buy_criteria = (
             (data[["bblo14", "bblo30", "bblo50", "bblo200"]] == 1).any(axis=1)
         ) | ((data[["rsi14", "rsi30", "rsi50", "rsi200"]] <= 30).any(axis=1))
         # Get the filtered data based on the buy criteria
         buy_filtered_data = data[buy_criteria]
 
         filtered_data = list(buy_filtered_data["symbol"])
 
+        if len(filtered_data) == 0:
+            print("No tickers meet the buy criteria")
+            return []
+
         try:
-            self.alpaca.watchlist.update(watchlist_name="DailyLosers", symbols=','.join(filtered_data))
+            self.alpaca.watchlist.update(
+                watchlist_name="DailyLosers", symbols=",".join(filtered_data)
+            )
         except Exception:
-            self.alpaca.watchlist.create(name=f"DailyLosers", symbols=','.join(filtered_data))
-
-        tickers = self.alpaca.watchlist.get_assets(watchlist_name="DailyLosers")
+            self.alpaca.watchlist.create(
+                name="DailyLosers", symbols=",".join(filtered_data)
+            )
+
+        tickers = self.alpaca.watchlist.get_assets(
+            watchlist_name="DailyLosers"
+        )
         # Return the list of tickers that meet the buy criteria
         return tickers
-    
+
     ########################################################
     # Define the get_ticker_data function
     ########################################################
     def get_ticker_data(self, tickers) -> pd.DataFrame:
         """
         Get the daily stock data, RSI, and Bollinger Bands
         this function is used for the daily stock data, RSI, and Bollinger Bands
@@ -339,15 +433,17 @@
         for i, ticker in tqdm(
             enumerate(tickers),
             desc="• Analizing ticker data for "
             + str(len(tickers))
             + " symbols from Alpaca API",
         ):
             try:
-                history = self.alpaca.history.get_stock_data(symbol=ticker, start=year_ago, end=previous_day) 
+                history = self.alpaca.history.get_stock_data(
+                    symbol=ticker, start=year_ago, end=previous_day
+                )
             except Exception:
                 continue
 
             try:
                 for n in [14, 30, 50, 200]:
                     # Initialize RSI Indicator
                     history["rsi" + str(n)] = RSIIndicator(
```

### Comparing `py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/src/article_extractor.py` & `py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/src/article_extractor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 import os
 import requests
 import json
 
 import textwrap
 
 from dotenv import load_dotenv
+
 load_dotenv()
 
+
 class ArticleExtractor:
     def __init__(self):
-        self.api_key = os.getenv('ARTICLE_EXTRACTOR_API_KEY')
+        self.api_key = os.getenv("ARTICLE_EXTRACTOR_API_KEY")
 
     @staticmethod
-    def truncate(s, l):
-        if (l >= len(s)):
-            return (s)
+    def truncate(string, length):
+        if length >= len(string):
+            return string
         else:
-            return textwrap.shorten(s,width=l,placeholder="")
+            return textwrap.shorten(string, width=length, placeholder="")
 
     def extract_articles(self, urls: list) -> list:
         return_data = []
         if len(urls) == 0:
             return return_data
         for url in urls:
             url = f"https://api.articlextractor.com/v1/extract?url={url}&language=en&api_token={self.api_key}"
             response = requests.get(url)
             if response.status_code == 200:
-                res_dict = json.loads(response.text)['data']
-                if res_dict['title'] != "" and res_dict['text'] != "":
-                    return_data.append({
-                        'title': res_dict['title'],
-                        'content': self.truncate("".join(res_dict['text'].split()), 10000)
-                    })
+                res_dict = json.loads(response.text)["data"]
+                if res_dict["title"] != "" and res_dict["text"] != "":
+                    return_data.append(
+                        {
+                            "title": res_dict["title"],
+                            "content": self.truncate(
+                                "".join(res_dict["text"]), 10000
+                            ),
+                        }
+                    )
+            else:
+                raise Exception(
+                    f"Error fetching data from ArticleExtractor API: {response.text}"
+                )
 
-        return return_data
+        return return_data
```

### Comparing `py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/src/openai.py` & `py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/src/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 import os
 from openai import OpenAI
 
 from dotenv import load_dotenv
+
 load_dotenv()
 
+
 class OpenAIAPI:
     def __init__(self):
-        self.api_key = os.getenv('OPENAI_API_KEY')
+        self.api_key = os.getenv("OPENAI_API_KEY")
+
     ########################################################
     # Define the OpenAi chat function
     ########################################################
     def chat(self, msgs):
         """
         Chat with the OpenAI API
         :param msgs: List of messages
         return: OpenAI response
         """
         openai = OpenAI(api_key=self.api_key)
         response = openai.chat.completions.create(
-            model="gpt-3.5-turbo",
-            messages=msgs
+            model="gpt-3.5-turbo", messages=msgs
         )
         message = response
         return message
-    
+
     ########################################################
     # Define the get_market_sentiment function
     ########################################################
     def get_sentiment_analysis(self, title, symbol, article):
         """
         Get the sentiment of the article using OpenAI API sentiment analysis
         :param article: Article
         return: Sentiment of the article (BULLISH, BEARISH, NEUTRAL)
         """
         message_history = []
         sentiments = []
         # Send the system message to the OpenAI API
-        system_message = 'You will work as a Sentiment Analysis for Financial news. I will share news headline, stock symbol and article. You will only answer as:\n\n BEARISH,BULLISH,NEUTRAL. No further explanation. \n Got it?'
-        message_history.append({'content': system_message, 'role': 'user'})
+        system_message = "You will work as a Sentiment Analysis for Financial news. \
+            I will share news headline, stock symbol and article. \
+                You will only answer as:\n\n BEARISH,BULLISH,NEUTRAL. No further explanation. \n Got it?"
+
+        message_history.append({"content": system_message, "role": "user"})
         response = self.chat(message_history)
 
         # Send the article to the OpenAI API
-        user_message = '{}\n{}\n{}'.format(title, symbol, article)
-        
-        message_history.append({'content': user_message, 'role': 'user'})
+        user_message = "{}\n{}\n{}".format(title, symbol, article)
+
+        message_history.append({"content": user_message, "role": "user"})
         response = self.chat(message_history)
         sentiments.append(
-            {'title': title, 'symbol': symbol, 'article': article, 'signal': response.choices[0].message.content})
+            {
+                "title": title,
+                "symbol": symbol,
+                "article": article,
+                "signal": response.choices[0].message.content,
+            }
+        )
         message_history.pop()
         # Return the sentiment
-        return sentiments[0]['signal']
+        return sentiments[0]["signal"]
```

### Comparing `py_alpaca_daily_losers-0.1.1/py_alpaca_daily_losers/src/slack.py` & `py_alpaca_daily_losers-0.2.0/py_alpaca_daily_losers/src/slack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import os
 
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
 from dotenv import load_dotenv
+
 load_dotenv()
 
 # Load environment variables
-production = os.getenv('PRODUCTION')
-slack_token = os.getenv('SLACK_ACCESS_TOKEN')
+production = os.getenv("PRODUCTION")
+slack_token = os.getenv("SLACK_ACCESS_TOKEN")
+
 
 class Slack:
-    '''
+    """
     A class to send messages to a Slack channel
     attributes: slack_workspace_token
-    '''
+    """
+
     def __init__(self):
         self.slack_workspace_token = slack_token
 
     ########################################################
     # Define the send_message function
     ########################################################
     def send_message(self, channel, message, username):
@@ -34,19 +37,23 @@
         if not self.slack_workspace_token:
             print(message)
             return
 
         client = WebClient(token=self.slack_workspace_token)
 
         try:
-            response = client.chat_postMessage(channel=channel, text=f"{message}", username=username)
+            response = client.chat_postMessage(
+                channel=channel, text=f"{message}", username=username
+            )
             assert response["message"]["text"] == f"{message}"
         except SlackApiError as e:
             # You will get a SlackApiError if "ok" is False
             assert e.response["ok"] is False
-            assert e.response["error"]  # str like 'invalid_auth', 'channel_not_found'
+            assert e.response[
+                "error"
+            ]  # str like 'invalid_auth', 'channel_not_found'
             print(f"Got an error: {e.response['error']}")
             # Also receive a corresponding status_code
             assert isinstance(e.response.status_code, int)
             print(f"Received a response status_code: {e.response.status_code}")
         # else:
-        #     print(f"Message sent successfully to {channel}")
+        #     print(f"Message sent successfully to {channel}")
```

### Comparing `py_alpaca_daily_losers-0.1.1/PKG-INFO` & `py_alpaca_daily_losers-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: py-alpaca-daily-losers
-Version: 0.1.1
+Version: 0.2.0
 Summary: Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration.
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.30.1,<2.0.0)
-Requires-Dist: py-alpaca-api (>=0.4.4,<0.5.0)
+Requires-Dist: py-alpaca-api (>=0.5.1,<0.6.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: slack-sdk (>=3.27.2,<4.0.0)
 Requires-Dist: ta (>=0.11.0,<0.12.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Description-Content-Type: text/markdown
 
@@ -54,14 +54,20 @@
 </details>
 <hr>
 
 ##  Overview
 
 The py-alpaca-daily-losers project integrates Alpaca Markets for a daily losers strategy, offering market data extraction, AI analysis, and Slack notifications. The core functionality centers on retrieving and analyzing daily stock market data using indicators like Bollinger Bands and RSI. It provides insights through news extraction, sentiment analysis, and chat functions via OpenAI integration. This project equips users with robust data analysis tools for informed decision-making in the stock market.
 
+This project is in no way trading advice, or a vaild strategy. Any trading done using this package should only be on a paper account, until proven to work.
+
+Visit [PyAlpacaApi](https://github.com/TexasCoding/py-alpaca-api) to learn more about the core of this project.
+
+Visit [AlpacaApiStrategies](https://github.com/TexasCoding/alpaca-api-strategies) for an example app using this strategy.
+
 ---
 
 ##  Features
 
 |    |   Feature         | Description |
 |----|-------------------|---------------------------------------------------------------|
 | ⚙️  | **Architecture**  | The project has a modular architecture that integrates various components for market data extraction, AI analysis, and Slack notifications. It leverages external APIs effectively within its architecture. |
```

