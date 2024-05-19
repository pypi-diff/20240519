# Comparing `tmp/mptradelib-0.5.2.tar.gz` & `tmp/mptradelib-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.5.2.tar", max compression
+gzip compressed data, was "mptradelib-0.5.3.tar", max compression
```

## Comparing `mptradelib-0.5.2.tar` & `mptradelib-0.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.2/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.2/mptradelib/__init__.py
--rw-r--r--   0        0        0     4562 2024-05-17 20:17:00.043228 mptradelib-0.5.2/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.2/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5.2/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.2/mptradelib/broker/session.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.2/mptradelib/broker/shoonya.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.2/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.2/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.2/mptradelib/cli/new.py
--rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.2/mptradelib/cli/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.2/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.2/mptradelib/cli/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.2/mptradelib/feed.py
--rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.2/mptradelib/livetrade.py
--rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.2/mptradelib/optimizers/__init__.py
--rw-r--r--   0        0        0     4949 2024-05-17 20:42:16.487036 mptradelib-0.5.2/mptradelib/optimizers/walkforward.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.2/mptradelib/test_renko.py
--rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.2/mptradelib/utils/__init__.py
--rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.2/mptradelib/utils/simulated_trades.py
--rw-r--r--   0        0        0     6887 2024-05-12 12:25:21.588670 mptradelib-0.5.2/mptradelib/utils/tearsheet.py
--rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.2/mptradelib/utils/utils.py
--rw-r--r--   0        0        0      846 2024-05-17 20:42:27.418984 mptradelib-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 mptradelib-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.3/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4562 2024-05-19 20:11:23.024752 mptradelib-0.5.3/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.3/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5.3/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.3/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.3/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.3/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.3/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.3/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.3/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.3/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.3/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.3/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.3/mptradelib/livetrade.py
+-rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.3/mptradelib/optimizers/__init__.py
+-rw-r--r--   0        0        0     5533 2024-05-19 20:11:15.319126 mptradelib-0.5.3/mptradelib/optimizers/walkforward.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.3/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.3/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.3/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0     6887 2024-05-12 12:25:21.588670 mptradelib-0.5.3/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.3/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0      822 2024-05-19 20:15:14.649317 mptradelib-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 mptradelib-0.5.3/PKG-INFO
```

### Comparing `mptradelib-0.5.2/README.md` & `mptradelib-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/backtest.py` & `mptradelib-0.5.3/mptradelib/backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/broker/broker.py` & `mptradelib-0.5.3/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/broker/session.py` & `mptradelib-0.5.3/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/broker/shoonya.py` & `mptradelib-0.5.3/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/broker/ticker.py` & `mptradelib-0.5.3/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/cli/new.py` & `mptradelib-0.5.3/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/cli/templates/strategy/__init__.py.jinja` & `mptradelib-0.5.3/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/cli/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.5.3/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/cli/templates/strategy/livetrade.py.jinja` & `mptradelib-0.5.3/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/feed.py` & `mptradelib-0.5.3/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/livetrade.py` & `mptradelib-0.5.3/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/optimizers/walkforward.py` & `mptradelib-0.5.3/mptradelib/optimizers/walkforward.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,82 +1,91 @@
 import pydantic as pyd
 import pandas as pd
 from mptradelib.backtest import Backtest
 from typing import Callable, List
 from tqdm import tqdm
-
-try:
-    import plotly.graph_objects as go
-except ImportError:
-    pass
+import plotly.graph_objects as go
 
 class Stage(pyd.BaseModel):
     model_config = pyd.ConfigDict(arbitrary_types_allowed=True)
 
-    df: pd.DataFrame
+    main_df: pd.DataFrame = pyd.Field(..., alias='df')
     stage_no: int
     stage_size: int
     test_fraction: float = 0.25
+    _opt_result: pd.DataFrame = None
 
     @property
     def test_df(self):
         test_size = self._get_test_size()
-        return self.stage_df[len(self.stage_df)-test_size : ]
+        return self.df[len(self.df)-test_size : ]
     
     @property
     def opt_df(self):
         test_size = self._get_test_size()
-        return self.stage_df[:len(self.stage_df)-test_size]
+        return self.df[:len(self.df)-test_size]
     
     @property
-    def stage_df(self):
+    def df(self):
         test_size = self._get_test_size()
         start_idx = test_size * self.stage_no
-        return self.df[start_idx:start_idx + self.stage_size]
+        return self.main_df[start_idx:start_idx + self.stage_size]
+    
+    @property
+    def opt_result(self):
+        return self._opt_result
     
     def _get_test_size(self):
         return int(self.stage_size * self.test_fraction)
 
     def optimize(self, compute, **params: dict):
         b = Backtest(self.opt_df, compute=compute)
-        return b.optimize(params)
+        self._opt_result = b.optimize(params)
+        return self
+
+    def validate(self):
+        pass
 
 
 class Walkforward(pyd.BaseModel):
     model_config = pyd.ConfigDict(arbitrary_types_allowed=True)
 
     df: pd.DataFrame
     stage_count: int = 6
     test_fraction: float = 0.25
     strategy: Callable[[pd.DataFrame, dict],pd.DataFrame]
+    stages: List[Stage] = []
 
-    def _create_stages(self) -> Stage:
+    def _create_stages(self) -> List[Stage]:
         stage_size = int(len(self.df)/(1 + (self.stage_count-1) * self.test_fraction))
         stages = []
         for i in range(self.stage_count):
             stage = Stage(df=self.df, stage_no=i, stage_size=stage_size, test_fraction=self.test_fraction)
             stages.append(stage)
         return stages
 
     def optimize(self, **params: dict):
         show_progressbar = params.pop('show_progressbar', True)
 
-        results = []
-        stages = self._create_stages()
+        stages: Stage = self._create_stages()
         if show_progressbar:
             with tqdm(total=len(stages)) as pb:
                 for stage in stages:
-                    r = stage.optimize(self.strategy,**params)
-                    results.append(r)
+                    s = stage.optimize(self.strategy, **params)
+                    self.stages.append(s)
                     pb.update()
         else:
             for stage in stages:
-                r = stage.optimize(self.strategy,**params)
-                results.append(r)
-        return results
+                stage.optimize(self.strategy, **params)
+                self.stages.append(stage)
+        return self
+    
+    @property
+    def opt_result(self):
+        return [s.opt_result for s in self.stages]
 
     def _get_date(self, d, index):
         return d.datetime.iloc[index].strftime("%Y-%m-%d")
 
     def plot_splits(self):
         stages = self._create_stages()
         fig = go.Figure()
@@ -111,47 +120,55 @@
 class MultiSymbolWalkforwardAnalysis(pyd.BaseModel):
     model_config = pyd.ConfigDict(arbitrary_types_allowed=True)
 
     dfs: List[pd.DataFrame]
     stage_count: int = 6
     test_fraction: float = 0.25
     strategy: Callable[[pd.DataFrame, dict],pd.DataFrame]
+    walkforwards: List[Walkforward] = []
+    __computed_result = None
 
     def optimize(self, **params: dict):
-        results = []
         with tqdm(total=len(self.dfs)) as pb:
             for df in self.dfs:
                 w = Walkforward(
                     df=df, 
                     stage_count=self.stage_count, 
                     test_fraction=self.test_fraction, 
                     strategy=self.strategy
                 )
-                r = w.optimize(**params)
-                results.append(r)
+                w.optimize(**params)
                 pb.update()
-        return self._aggregate(results)
+                self.walkforwards.append(w)
+        return self
     
-    def _aggregate(self, results):
+    @property
+    def opt_result(self):
+        return [w.opt_result for w in self.walkforwards]
+
+    def transform_to_agg_stages(self):
+        if self.__computed_result is not None:
+            return self.__computed_result
+        
         stages = []
-        for i in range(len(results[0])):
+        for i in range(len(self.walkforwards[0].opt_result)):
             stage = []
-            for sym in results:
-                stage.append(sym[i])
+            for sym in self.walkforwards:
+                stage.append(sym.stages[i])
             stages.append(stage)
 
         final_result = []
         for stage in stages:
             pp = []
-            for i in range(len(stage[0])):
+            for i in range(len(stage[0].opt_result)):
                 result_agg = {
                     'trades': []
                 }
                 for j in range(len(stage)):
-                    result_agg['params'] = stage[j][i]['params']
-                    result_agg['trades'].append(stage[j][i]['trades'])
+                    result_agg['params'] = stage[j].opt_result[i]['params']
+                    result_agg['trades'].append(stage[j].opt_result[i]['trades'])
                 result_agg['trades'] = pd.concat(result_agg['trades'])
                 pp.append(result_agg)
             final_result.append(pp)
         return final_result
```

### Comparing `mptradelib-0.5.2/mptradelib/test_renko.py` & `mptradelib-0.5.3/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/utils/simulated_trades.py` & `mptradelib-0.5.3/mptradelib/utils/simulated_trades.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/utils/tearsheet.py` & `mptradelib-0.5.3/mptradelib/utils/tearsheet.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/mptradelib/utils/utils.py` & `mptradelib-0.5.3/mptradelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.2/pyproject.toml` & `mptradelib-0.5.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.5.2"
+version = "0.5.3"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
@@ -12,15 +12,14 @@
 fyers-apiv3 = "3.0.6"
 retry = "0.9.2"
 pyotp = "2.9.0"
 jinja2 = "^3.1.3"
 click = "^8.1.7"
 jinja2-strcase = "^0.0.2"
 redis = "^5.0.4"
-pandas-ta = "^0.3.14b0"
 tqdm = "^4.66.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 
 pandas_ta = { version = "^0.3.14b", optional = true }
 pandas = { version = "^2.1.4", optional = true }
```

### Comparing `mptradelib-0.5.2/PKG-INFO` & `mptradelib-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.5.2
+Version: 0.5.3
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,14 @@
 Provides-Extra: hyperopt
 Provides-Extra: pandas
 Provides-Extra: pandasta
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: fyers-apiv3 (==3.0.6)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: jinja2-strcase (>=0.0.2,<0.0.3)
-Requires-Dist: pandas-ta (>=0.3.14b0,<0.4.0) ; extra == "pandasta"
 Requires-Dist: pydantic (==2.7.1)
 Requires-Dist: pyotp (==2.9.0)
 Requires-Dist: redis (>=5.0.4,<6.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: retry (==0.9.2)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Description-Content-Type: text/markdown
```

