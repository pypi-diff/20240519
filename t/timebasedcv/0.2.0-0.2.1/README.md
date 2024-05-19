# Comparing `tmp/timebasedcv-0.2.0.tar.gz` & `tmp/timebasedcv-0.2.1.tar.gz`

## Comparing `timebasedcv-0.2.0.tar` & `timebasedcv-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/timebasedcv/__init__.py
--rw-r--r--   0        0        0    21046 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/timebasedcv/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/timebasedcv/py.typed
--rw-r--r--   0        0        0     8511 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/timebasedcv/sklearn.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/timebasedcv/splitstate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/timebasedcv/utils/__init__.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/timebasedcv/utils/_backends.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/timebasedcv/utils/_funcs.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/timebasedcv/utils/_types.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/LICENSE
--rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/README.md
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    10407 2020-02-02 00:00:00.000000 timebasedcv-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/timebasedcv/__init__.py
+-rw-r--r--   0        0        0    24488 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/timebasedcv/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/timebasedcv/py.typed
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/timebasedcv/sklearn.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/timebasedcv/splitstate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/timebasedcv/utils/__init__.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/timebasedcv/utils/_backends.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/timebasedcv/utils/_funcs.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/timebasedcv/utils/_types.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/README.md
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10545 2020-02-02 00:00:00.000000 timebasedcv-0.2.1/PKG-INFO
```

### Comparing `timebasedcv-0.2.0/timebasedcv/core.py` & `timebasedcv-0.2.1/timebasedcv/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,53 +43,56 @@
     `_CoreTimeBasedSplit` implements all the logics to set up a time based splits class.
 
     In particular it implements `_splits_from_period` which is used to generate splits from a given time period (from
     start to end dates) from the given arguments of the class (frequency, train_size, forecast_horizon, gap, stride and
     window type).
 
     Arguments:
-        frequency: The frequency of the time series. Must be one of "days", "seconds", "microseconds", "milliseconds",
-            "minutes", "hours", "weeks". These are the only valid values for the `unit` argument of `timedelta` from
-            python `datetime` standard library.
-        train_size: The size of the training set.
-        forecast_horizon: The size of the forecast horizon, i.e. the size of the test set.
-        gap: The size of the gap between the training set and the forecast horizon.
-        stride: The size of the stride between consecutive splits. Notice that if stride is not provided (or set to 0),
-            it fallbacks to the `forecast_horizon` quantity.
+        frequency: The frequency (or time unit) of the time series. Must be one of "days", "seconds", "microseconds",
+            "milliseconds", "minutes", "hours", "weeks". These are the only valid values for the `unit` argument of
+            `timedelta` from python `datetime` standard library.
+        train_size: Defines the minimum number of time units required to be in the train set.
+        forecast_horizon: Specifies the number of time units to forecast.
+        gap: Sets the number of time units to skip between the end of the train set and the start of the forecast set.
+        stride: How many time unit to move forward after each split. If `None` (or set to 0), the stride is equal to the
+            `forecast_horizon` quantity.
         window: The type of window to use, either "rolling" or "expanding".
-        mode: Determines in which orders the splits are generated, either "forward" or "backward".
+        mode: Determines in which orders the splits are generated, either "forward" (start to end) or "backward"
+            (end to start).
 
     Raises:
-        ValueError: If `frequency` is not one of "days", "seconds", "microseconds", "milliseconds", "minutes", "hours",
+        ValueError:
+            - If `frequency` is not one of "days", "seconds", "microseconds", "milliseconds", "minutes", "hours",
             "weeks".
-        ValueError: If `window` is not one of "rolling" or "expanding".
+            - If `window` is not one of "rolling" or "expanding".
+            - If `mode` is not one of "forward" or "backward"
+            - If `train_size`, `forecast_horizon`, `gap` or `stride` are not strictly positive.
         TypeError: If `train_size`, `forecast_horizon`, `gap` or `stride` are not of type `int`.
-        ValueError: If `train_size`, `forecast_horizon`, `gap` or `stride` are not strictly positive.
 
     Although `_CoreTimeBasedSplit` is not meant to be used directly, it can be used as a template to create new time
     based splits classes.
 
-    Usage:
-    ```python
-    from timebasedcv import _CoreTimeBasedSplit
-
-
-    class MyTimeBasedSplit(_CoreTimeBasedSplit):
-        def split(self, X, timeseries):
-            # Implement the split method to return a generator
-
-            for split in self._splits_from_period(timeseries.min(), timeseries.max()):
-                # Do something with the split to compute the train and forecast sets
-                ...
-                yield X_train, y_test
-    ```
+    Examples:
+        ```python
+        from timebasedcv.core import _CoreTimeBasedSplit
+
+
+        class MyTimeBasedSplit(_CoreTimeBasedSplit):
+            ...
+
+            def split(self, X, timeseries):
+                '''Implement the split method to return a generator'''
+
+                for split in self._splits_from_period(timeseries.min(), timeseries.max()):
+                    # Do something with the split to compute the train and forecast sets
+                    ...
+                    yield X_train, y_test
+        ```
     """
 
-    name_ = "_CoreTimeBasedSplit"
-
     def __init__(  # noqa: PLR0913
         self: Self,
         *,
         frequency: FrequencyUnit,
         train_size: int,
         forecast_horizon: int,
         gap: int = 0,
@@ -142,14 +145,18 @@
             msg = (
                 f"(`{'`, `'.join(_slot_names)}`) must be greater or equal than "
                 f"({', '.join(map(str, _lower_bounds))}).\n"
                 f"Found ({', '.join(str(v) for v in _values)})"
             )
             raise ValueError(msg)
 
+    @property
+    def name_(self: Self) -> str:
+        return self.__class__.__name__
+
     def __repr__(self: Self) -> str:
         """Custom repr method."""
         _attrs = (
             "frequency_",
             "train_size_",
             "forecast_horizon_",
             "gap_",
@@ -236,15 +243,31 @@
     def n_splits_of(
         self: Self,
         *,
         time_series: Union[SeriesLike[DateTimeLike], None] = None,
         start_dt: NullableDatetime = None,
         end_dt: NullableDatetime = None,
     ) -> int:
-        """Returns the number of splits that can be generated from `time_series`."""
+        """Returns the number of splits that can be generated from `time_series`.
+
+        Arguments:
+            time_series: A time series data. If provided it should support `.min()` and `.max().
+            start_dt: The start date and time of the time series. If not provided, it will be inferred from
+                `time_series`.
+            end_dt: The end date and time of the time series. If not provided, it will be inferred from
+                `time_series`.
+
+        Returns:
+            The number of splits that can be generated from the given time series.
+
+        Raises:
+            ValueError:
+                - If both `start_dt` and `end_dt` are provided and `start_dt` is greater than or equal to `end_dt`.
+                - If neither `time_series` nor (`start_dt`, `end_dt`) pair is provided.
+        """
         if (start_dt is not None) and (end_dt is not None):
             if start_dt >= end_dt:
                 msg = "`start_dt` must be before `end_dt`."
                 raise ValueError(msg)
             else:
                 time_start, time_end = start_dt, end_dt
         elif time_series is not None:
@@ -253,63 +276,35 @@
             msg = "Either `time_series` or (`start_dt`, `end_dt`) pair must be provided."
             raise ValueError(msg)
 
         return len(tuple(self._splits_from_period(time_start, time_end)))
 
 
 class TimeBasedSplit(_CoreTimeBasedSplit):
-    """Class that generates splits based on time values, independently from the number of samples in each split.
-
-    Arguments:
-        frequency: The frequency of the time series. Must be one of "days", "seconds", "microseconds", "milliseconds",
-            "minutes", "hours", "weeks". These are the only valid values for the `unit` argument of `timedelta` from
-            python `datetime` standard library.
-        train_size: The size of the training set.
-        forecast_horizon: The size of the forecast horizon, i.e. the size of the test set.
-        gap: The size of the gap between the training set and the forecast horizon.
-        stride: The size of the stride between consecutive splits. Notice that if stride is not provided (or set to 0),
-            it fallbacks to the `forecast_horizon` quantity.
-        window: The type of window to use, either "rolling" or "expanding".
-        mode: Determines in which orders the splits are generated, either "forward" or "backward".
-
-    Raises:
-        ValueError: If `frequency` is not one of "days", "seconds", "microseconds", "milliseconds", "minutes", "hours",
-            "weeks".
-        ValueError: If `window` is not one of "rolling" or "expanding".
-        TypeError: If `train_size`, `forecast_horizon`, `gap` or `stride` are not of type `int`.
-        ValueError: If `train_size`, `forecast_horizon`, `gap` or `stride` are not strictly positive.
-
-    Usage:
-    ```python
-    import pandas as pd
-    import numpy as np
+    """`TimeBasedSplit` generates splits based on time periods, independently from the number of samples in each split.
 
-    from timebasedcv import TimeBasedSplit
+    It inherits from [`_CoreTimeBasedSplit`][timebasedcv.core._CoreTimeBasedSplit] and it only implements the `.split()`
+    method and logic.
 
-    tbs = TimeBasedSplit(
-        frequency="days",
-        train_size=30,
-        forecast_horizon=7,
-        gap=0,
-        stride=3,
-        window="rolling",
-    )
+    !!! warning "Differences with scikit-learn"
 
-    dates = pd.Series(pd.date_range("2023-01-01", "2023-12-31", freq="D"))
-    size = len(dates)
+        `TimeBasedSplit` is **not** compatible with
+        [scikit-learn CV Splitters](https://scikit-learn.org/stable/common_pitfalls.html#id3){:target="_blank"}.
 
-    df = pd.DataFrame(data=np.random.randn(size, 2), columns=["a", "b"]).assign(y=lambda t: t[["a", "b"]].sum(axis=1))
+        In fact, we have made the (opinioned) choice to:
 
-    X, y = df[["a", "b"]], df["y"]
+        - Return the sliced arrays from `.split(...)`, while scikit-learn CV Splitters return train and test indices of
+            the split.
+        - Require to pass the time series as input to `.split(...)` method, while scikit-learn CV Splitters require to
+            provide only `X, y, groups` to `.split(...)`.
+        - Such time series is used to generate the boolean masks with which we slice the original arrays into train and
+            test for each split.
 
-    print(f"Number of splits: {tbs.n_splits_of(time_series=dates)}")
-
-    for X_train, X_forecast, y_train, y_forecast in tbs.split(X, y, time_series=dates):
-        print(f"Train: {X_train.shape}, Forecast: {X_forecast.shape}")
-    ```
+        If you are looking for a class compatible with scikit-learn, check out our
+        [`TimeBasedCVSplitter`][timebasedcv.sklearn.TimeBasedCVSplitter] in the `timebasedcv.sklearn` module.
 
     A few examples on how splits are generated given the parameters. Let:
 
     - `=` : train period unit
     - `*` : forecast period unit
     - `/` : gap period unit
     - `>` : stride period unit (absorbed in `=` if `window="expanding"`)
@@ -331,17 +326,106 @@
 
     train_size, forecast_horizon, gap, stride, window = (4, 3, 2, 2, "expanding")
     | ======= /// *****           |
     | =========== /// *****       |
     | =============== /// *****   |
     | =================== /// *** |
     ```
-    """
 
-    name_ = "TimeBasedSplit"
+    Arguments:
+        frequency: The frequency (or time unit) of the time series. Must be one of "days", "seconds", "microseconds",
+            "milliseconds", "minutes", "hours", "weeks". These are the only valid values for the `unit` argument of
+            `timedelta` from python `datetime` standard library.
+        train_size: Defines the minimum number of time units required to be in the train set.
+        forecast_horizon: Specifies the number of time units to forecast.
+        gap: Sets the number of time units to skip between the end of the train set and the start of the forecast set.
+        stride: How many time unit to move forward after each split. If `None` (or set to 0), the stride is equal to the
+            `forecast_horizon` quantity.
+        window: The type of window to use, either "rolling" or "expanding".
+        mode: Determines in which orders the splits are generated, either "forward" (start to end) or "backward"
+            (end to start).
+
+    Raises:
+        ValueError:
+            - If `frequency` is not one of "days", "seconds", "microseconds", "milliseconds", "minutes", "hours",
+            "weeks".
+            - If `window` is not one of "rolling" or "expanding".
+            - If `mode` is not one of "forward" or "backward"
+            - If `train_size`, `forecast_horizon`, `gap` or `stride` are not strictly positive.
+        TypeError: If `train_size`, `forecast_horizon`, `gap` or `stride` are not of type `int`.
+
+
+    Examples:
+        ```python
+        # Let's first generate some data
+        import pandas as pd
+        import numpy as np
+
+        RNG = np.random.default_rng(seed=42)
+
+        dates = pd.Series(pd.date_range("2023-01-01", "2023-01-31", freq="D"))
+        size = len(dates)
+
+        df = (
+            pd.concat(
+                [
+                    pd.DataFrame(
+                        {
+                            "time": pd.date_range(start, end, periods=_size, inclusive="left"),
+                            "a": RNG.normal(size=_size - 1),
+                            "b": RNG.normal(size=_size - 1),
+                        }
+                    )
+                    for start, end, _size in zip(dates[:-1], dates[1:], RNG.integers(2, 24, size - 1))
+                ]
+            )
+            .reset_index(drop=True)
+            .assign(y=lambda t: t[["a", "b"]].sum(axis=1) + RNG.normal(size=t.shape[0]) / 25)
+        )
+
+        df.set_index("time").resample("D").agg(count=("y", np.size)).head(5)
+        ```
+
+        ```terminal
+                    count
+        time
+        2023-01-01      2
+        2023-01-02     18
+        2023-01-03     15
+        2023-01-04     10
+        2023-01-05     10
+        ```
+
+        Now let's run split the data with the provided `TimeBasedSplit` instance:
+
+        ```py
+        from timebasedcv import TimeBasedSplit
+
+
+        tbs = TimeBasedSplit(
+            frequency="days",
+            train_size=10,
+            forecast_horizon=5,
+            gap=1,
+            stride=3
+        )
+        X, y, time_series = df.loc[:, ["a", "b"]], df["y"], df["time"]
+
+        for X_train, X_forecast, y_train, y_forecast in tbs.split(X, y, time_series=time_series):
+            print(f"Train: {X_train.shape}, Forecast: {X_forecast.shape}")
+        ```
+
+        ```terminal
+        Train: (100, 2), Forecast: (51, 2)
+        Train: (114, 2), Forecast: (50, 2)
+        ...
+        Train: (124, 2), Forecast: (40, 2)
+        Train: (137, 2), Forecast: (22, 2)
+        ```
+    """
 
     @overload
     def split(
         self: Self,
         *arrays: TL,
         time_series: SeriesLike[DateTimeLike],
         start_dt: NullableDatetime = None,
@@ -420,17 +504,18 @@
         Returns:
             A generator of tuples of arrays containing the training and forecast data.
                 Each tuple corresponds to a split generated by the `TimeBasedSplit` instance. If `return_splitstate` is
                 True, each tuple is of the form `(train_forecast_arrays, split_state)`, othersiwe it is of the form
                 `train_forecast_arrays`.
 
         Raises:
-            ValueError: If no arrays are provided as input.
-            ValueError: If the arrays provided have different lengths.
-            ValueError: If the length of the time series does not match the length of the arrays.
+            ValueError:
+                - If no arrays are provided as input.
+                - If the arrays provided have different lengths.
+                - If the length of the time series does not match the length of the arrays.
         """
         n_arrays = len(arrays)
         if n_arrays == 0:
             msg = "At least one array required as input"
             raise ValueError(msg)
 
         ts_shape = time_series.shape
@@ -480,16 +565,14 @@
             else:
                 yield train_forecast_arrays
 
 
 class ExpandingTimeSplit(TimeBasedSplit):  # pragma: no cover
     """Alias for `TimeBasedSplit(..., window="expanding")`."""
 
-    name_ = "ExpandingTimeSplit"
-
     def __init__(  # noqa: PLR0913
         self: Self,
         *,
         frequency: FrequencyUnit,
         train_size: int,
         forecast_horizon: int,
         gap: int = 0,
@@ -506,16 +589,14 @@
             mode=mode,
         )
 
 
 class RollingTimeSplit(TimeBasedSplit):  # pragma: no cover
     """Alias for `TimeBasedSplit(..., window="rolling")`."""
 
-    name_ = "RollingTimeSplit"
-
     def __init__(  # noqa: PLR0913
         self: Self,
         *,
         frequency: FrequencyUnit,
         train_size: int,
         forecast_horizon: int,
         gap: int = 0,
```

### Comparing `timebasedcv-0.2.0/timebasedcv/sklearn.py` & `timebasedcv-0.2.1/timebasedcv/sklearn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 import sys
-from typing import TYPE_CHECKING, Generator, Union
+from typing import TYPE_CHECKING, Generator, Tuple, Union
 
 import numpy as np
 
 from timebasedcv.core import TimeBasedSplit
 
 if sys.version_info >= (3, 11):  # pragma: no cover
     from typing import Self
@@ -39,103 +39,105 @@
         NullableDatetime,
         SeriesLike,
         WindowType,
     )
 
 
 class TimeBasedCVSplitter(_BaseKFold):
-    """The `TimeBasedCVSplitter` is a scikit-learn CV Splitters that generates splits based on time values.
+    """The `TimeBasedCVSplitter` is a scikit-learn compatible CV Splitter that generates splits based on time values.
 
     The number of sample in each split is independent of the number of splits but based purely on the timestamp of the
     sample.
 
-    In order to achieve such behaviour we include the arguments of `TimeBasedSplit.split()` method (namely
-    `time_series`, `start_dt` and `end_dt`) in the constructor (a.k.a. `__init__` method) and store the for future use
-    in its `split` and `get_n_splits` methods.
+    In order to achieve such behaviour we include the arguments of
+    [`TimeBasedSplit.split()`][timebasedcv.core.TimeBasedSplit.split] method (namely `time_series`, `start_dt` and
+    `end_dt`) in the constructor (a.k.a. `__init__` method) and store the for future use in its `split` and
+    `get_n_splits` methods.
 
     In this way we can restrict the arguments of `split` and `get_n_splits` to the arrays to split (i.e. `X`, `y` and
     `groups`), which are the only arguments required by scikit-learn CV Splitters.
 
     Arguments:
-        frequency: The frequency of the time series. Must be one of "days", "seconds", "microseconds", "milliseconds",
-            "minutes", "hours", "weeks". These are the only valid values for the `unit` argument of `timedelta` from
-            python `datetime` standard library.
-        train_size: The size of the training set.
-        forecast_horizon: The size of the forecast horizon, i.e. the size of the test set.
+        frequency: The frequency (or time unit) of the time series. Must be one of "days", "seconds", "microseconds",
+            "milliseconds", "minutes", "hours", "weeks". These are the only valid values for the `unit` argument of
+            `timedelta` from python `datetime` standard library.
+        train_size: Defines the minimum number of time units required to be in the train set.
+        forecast_horizon: Specifies the number of time units to forecast.
         time_series: The time series used to create boolean mask for splits. It is not required to be sorted, but it
             must support:
 
             - comparison operators (with other date-like objects).
             - bitwise operators (with other boolean arrays).
             - `.min()` and `.max()` methods.
             - `.shape` attribute.
-        gap: The size of the gap between the training set and the forecast horizon.
-        stride: The size of the stride between consecutive splits. Notice that if stride is not provided (or set to 0),
-            it fallbacks to the `forecast_horizon` quantity.
+        gap: Sets the number of time units to skip between the end of the train set and the start of the forecast set.
+        stride: How many time unit to move forward after each split. If `None` (or set to 0), the stride is equal to the
+            `forecast_horizon` quantity.
         window: The type of window to use, either "rolling" or "expanding".
-        mode: Determines in which orders the splits are generated, either "forward" or "backward".
+        mode: Determines in which orders the splits are generated, either "forward" (start to end) or "backward"
+            (end to start).
         start_dt: The start of the time period. If provided, it is used in place of the `time_series.min()`.
         end_dt: The end of the time period. If provided,it is used in place of the `time_series.max()`.
 
     Raises:
-        ValueError: If `frequency` is not one of "days", "seconds", "microseconds", "milliseconds", "minutes", "hours",
+        ValueError:
+            - If `frequency` is not one of "days", "seconds", "microseconds", "milliseconds", "minutes", "hours",
             "weeks".
-        ValueError: If `window` is not one of "rolling" or "expanding".
+            - If `window` is not one of "rolling" or "expanding".
+            - If `mode` is not one of "forward" or "backward"
+            - If `train_size`, `forecast_horizon`, `gap` or `stride` are not strictly positive.
         TypeError: If `train_size`, `forecast_horizon`, `gap` or `stride` are not of type `int`.
-        ValueError: If `train_size`, `forecast_horizon`, `gap` or `stride` are not strictly positive.
 
-    Usage:
-    ```python
-    import pandas as pd
-    import numpy as np
-
-    from sklearn.linear_model import Ridge
-    from sklearn.model_selection import RandomizedSearchCV
-
-    from timebasedcv.sklearn import TimeBasedCVSplitter
-
-    start_dt = pd.Timestamp(2023, 1, 1)
-    end_dt = pd.Timestamp(2023, 1, 31)
-
-    time_series = pd.Series(pd.date_range(start_dt, end_dt, freq="D"))
-    size = len(time_series)
-
-    df = pd.DataFrame(data=np.random.randn(size, 2), columns=["a", "b"]).assign(y=lambda t: t[["a", "b"]].sum(axis=1))
-
-    X, y = df[["a", "b"]], df["y"]
-
-    cv = TimeBasedCVSplitter(
-        frequency="days",
-        train_size=7,
-        forecast_horizon=11,
-        gap=0,
-        stride=1,
-        window="rolling",
-        time_series=time_series,
-        start_dt=start_dt,
-        end_dt=end_dt,
-    )
+    Examples:
+        ```python
+        import pandas as pd
+        import numpy as np
+
+        from sklearn.linear_model import Ridge
+        from sklearn.model_selection import RandomizedSearchCV
+
+        from timebasedcv.sklearn import TimeBasedCVSplitter
+
+        start_dt = pd.Timestamp(2023, 1, 1)
+        end_dt = pd.Timestamp(2023, 1, 31)
+
+        time_series = pd.Series(pd.date_range(start_dt, end_dt, freq="D"))
+        size = len(time_series)
+
+        df = pd.DataFrame(data=np.random.randn(size, 2), columns=["a", "b"])
+
+        X, y = df[["a", "b"]], df[["a", "b"]].sum(axis=1)
+
+        cv = TimeBasedCVSplitter(
+            frequency="days",
+            train_size=7,
+            forecast_horizon=11,
+            gap=0,
+            stride=1,
+            window="rolling",
+            time_series=time_series,
+            start_dt=start_dt,
+            end_dt=end_dt,
+        )
 
-    param_grid = {
-        "alpha": np.linspace(0.1, 2, 10),
-        "fit_intercept": [True, False],
-        "positive": [True, False],
-    }
-
-    random_search_cv = RandomizedSearchCV(
-        estimator=Ridge(),
-        param_distributions=param_grid,
-        cv=cv,
-        n_jobs=-1,
-    ).fit(X, y)
-    ```
+        param_grid = {
+            "alpha": np.linspace(0.1, 2, 10),
+            "fit_intercept": [True, False],
+            "positive": [True, False],
+        }
+
+        random_search_cv = RandomizedSearchCV(
+            estimator=Ridge(),
+            param_distributions=param_grid,
+            cv=cv,
+            n_jobs=-1,
+        ).fit(X, y)
+        ```
     """
 
-    name_ = "TimeBasedCVSplitter"
-
     def __init__(  # noqa: PLR0913
         self: Self,
         *,
         frequency: FrequencyUnit,
         train_size: int,
         forecast_horizon: int,
         time_series: Union[SeriesLike[date], SeriesLike[datetime], SeriesLike[pd.Datetime]],
@@ -164,18 +166,28 @@
         self.size_ = time_series.shape[0]
 
     def split(
         self: Self,
         X: Union[NDArray, None] = None,
         y: Union[NDArray, None] = None,
         groups: Union[NDArray, None] = None,
-    ) -> Generator[NDArray[np.int_], None, None]:
-        """Generates integer indices corresponding to test sets.
+    ) -> Generator[Tuple[NDArray[np.int_], NDArray[np.int_]], None, None]:
+        """Generates integer indices corresponding to train and test sets.
+
+        Arguments:
+            X: Optional input features array.
+            y: Optional target variable array.
+            groups: Optional array containing group labels for the samples.
+
+        Returns:
+            A generator that yields tuples of train and test indices.
+
+        Raises:
+            ValueError: If the input arrays have incompatible lengths with reference `time_series`.
 
-        Required method to conform with scikit-learn `BaseCrossValidator`
         """
         self._validate_split_args(self.size_, X, y, groups)
 
         _indexes = np.arange(self.size_)
 
         yield from self.splitter.split(  # type: ignore[call-overload]
             _indexes,
```

### Comparing `timebasedcv-0.2.0/timebasedcv/splitstate.py` & `timebasedcv-0.2.1/timebasedcv/splitstate.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     import pandas as pd
 
 
 @dataclass(frozen=True)
 class SplitState(Generic[DateTimeLike]):
-    """The `SplitState` class represents the state of a split.
+    """A `SplitState` represents the state of a split in terms of its 4 cut/split points.
 
-    This is a set of split points where to partition a time series into training set and forecast set.
+    Namely these are start and end of training set, start and end of forecasting/test set.
 
     The class ensures that the split is valid by checking that the attributes are of the correct type and are ordered
     chronologically.
 
     The class provides properties to calculate the length of the training set, forecast set, gap between them, and the
     total length of the split.
```

### Comparing `timebasedcv-0.2.0/timebasedcv/utils/_backends.py` & `timebasedcv-0.2.1/timebasedcv/utils/_backends.py`

 * *Files identical despite different names*

### Comparing `timebasedcv-0.2.0/timebasedcv/utils/_funcs.py` & `timebasedcv-0.2.1/timebasedcv/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `timebasedcv-0.2.0/timebasedcv/utils/_types.py` & `timebasedcv-0.2.1/timebasedcv/utils/_types.py`

 * *Files identical despite different names*

### Comparing `timebasedcv-0.2.0/.gitignore` & `timebasedcv-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `timebasedcv-0.2.0/LICENSE` & `timebasedcv-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timebasedcv-0.2.0/README.md` & `timebasedcv-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,47 +14,49 @@
 
 [Documentation](https://fbruzzesi.github.io/timebasedcv) | [Repository](https://github.com/fbruzzesi/timebasedcv) | [Issue Tracker](https://github.com/fbruzzesi/timebasedcv/issues)
 
 ---
 
 ## Disclaimer ⚠️
 
-This codebase is experimental and is working for my use cases. It is very probable that there are cases not covered and for which it could break (badly). If you find them, please feel free to open an issue in the [issue page](https://github.com/FBruzzesi/timebasedcv/issues/new) of the repo.
+This codebase is experimental and is working for my use cases. It is very probable that there are cases not entirely covered and for which it could break (badly). If you find them, please feel free to open an issue in the [issue page](https://github.com/FBruzzesi/timebasedcv/issues/new){:target="_blank"} of the repo.
 
-## Description
+## Description ✨
 
-The current implementation of [scikit-learn TimeSeriesSplit](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.TimeSeriesSplit.html) lacks the flexibility of having multiple samples within the same time period or time unit.
+The current implementation of [scikit-learn TimeSeriesSplit](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.TimeSeriesSplit.html){:target="_blank"} lacks the flexibility of having multiple samples within the same time period (or time unit).
 
-**timebasedcv** addresses such problem by providing a cross validation strategy based on a **time unit** rather than the number of samples. This is useful when the data is time dependent, and the split should keep together samples within the same time window.
+**timebasedcv** addresses such problem by providing a cross validation strategy based on a **time period** rather than the number of samples. This is useful when the data is time dependent, and the split should keep together samples within the same time window.
 
-Temporal data leakage is an issue and we want to prevent that from happening by providing splits to make sure that models can train on past data and tested on future data, independently from the number of observations present within a given time period.
+Temporal data leakage is an issue and we want to prevent it from happening by providing splits that make sure the past and the future are well separated, so that data leakage does not spoil in a model cross validation.
 
-### Features ✨
+Again, these splits points solely depend on the time period and not the number of observations.
+
+### Features 📜
 
 We introduce two main classes:
 
 - [`TimeBasedSplit`](https://fbruzzesi.github.io/timebasedcv/api/timebasedcv/#timebasedcv.core.TimeBasedSplit) allows to define a split based on time unit (frequency), train size, test size, gap, stride, window type and mode. Remark that `TimeBasedSplit` is **not** compatible with [scikit-learn CV Splitters](https://scikit-learn.org/stable/common_pitfalls.html#id3). In fact, we have made the (opinioned) choice to:
 
   - Return the sliced arrays from `.split(...)`, while scikit-learn CV Splitters return train and test indices of the split.
   - Require to pass the time series as input to `.split(...)` method, while scikit-learn CV Splitters require to provide only `X, y, groups` to `.split(...)`.
   - Such time series is used to generate the boolean masks with which we slice the original arrays into train and test for each split.
 
 - Considering the above choices, we also provide a scikit-learn compatible splitter: [`TimeBasedCVSplitter`](https://fbruzzesi.github.io/timebasedcv/api/sklearn/#timebasedcv.sklearn.TimeBasedCVSplitter). Considering the signature that `.split(...)` requires and the fact that CV Splitters need to know a priori the number of splits, `TimeBasedCVSplitter` is initialized with the time series containing the time information used to generate the train and test indices of each split.
 
-## Installation
+## Installation 💻
 
 TL;DR:
 
 ```bash
 python -m pip install timebasedcv
 ```
 
 For further information, please refer to the dedicated [installation](https://fbruzzesi.github.io/timebasedcv/installation) section.
 
-## Quickstart
+## Quickstart 🏃
 
 The following code snippet is all you need to get started, yet consider checking out the [getting started](https://fbruzzesi.github.io/timebasedcv/user-guide/getting-started/) section of the documentation for a detailed guide on how to use the library.
 
 The main takeaway should be that `TimeBasedSplit` allows for a lot of flexibility at the cost of having to specify a long list of parameters. This is what makes the library so powerful and flexible to cover the large majority of use cases.
 
 First let's generate some data with different number of points per day:
 
@@ -127,14 +129,14 @@
 
 As we can see, each split does not necessarely have the same number of points, this is because the time series has a different number of points per day.
 
 A picture is worth a thousand words, let's visualize the splits (blue dots represent the train points, while the red dots represent the forecastng points):
 
 ![cross-validation](docs/img/basic-cv-split.png)
 
-## Contributing
+## Contributing ✌️
 
 Please read the [Contributing guidelines](https://fbruzzesi.github.io/timebasedcv/contribute/) in the documentation site.
 
-## License
+## License 👀
 
 The project has a [MIT Licence](https://github.com/FBruzzesi/timebasedcv/blob/main/LICENSE)
```

### Comparing `timebasedcv-0.2.0/pyproject.toml` & `timebasedcv-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "timebasedcv"
-version = "0.2.0"
+version = "0.2.1"
 description = "Time based cross validation"
 
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Francesco Bruzzesi"}]
```

### Comparing `timebasedcv-0.2.0/PKG-INFO` & `timebasedcv-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: timebasedcv
-Version: 0.2.0
+Version: 0.2.1
 Summary: Time based cross validation
 Project-URL: documentation, https://fbruzzesi.github.io/timebasedcv/
 Project-URL: repository, https://github.com/fbruzzesi/timebasedcv
 Project-URL: issue-tracker, https://github.com/fbruzzesi/timebasedcv/issues
 Author: Francesco Bruzzesi
 License: MIT License
         
@@ -99,47 +99,49 @@
 
 [Documentation](https://fbruzzesi.github.io/timebasedcv) | [Repository](https://github.com/fbruzzesi/timebasedcv) | [Issue Tracker](https://github.com/fbruzzesi/timebasedcv/issues)
 
 ---
 
 ## Disclaimer ⚠️
 
-This codebase is experimental and is working for my use cases. It is very probable that there are cases not covered and for which it could break (badly). If you find them, please feel free to open an issue in the [issue page](https://github.com/FBruzzesi/timebasedcv/issues/new) of the repo.
+This codebase is experimental and is working for my use cases. It is very probable that there are cases not entirely covered and for which it could break (badly). If you find them, please feel free to open an issue in the [issue page](https://github.com/FBruzzesi/timebasedcv/issues/new){:target="_blank"} of the repo.
 
-## Description
+## Description ✨
 
-The current implementation of [scikit-learn TimeSeriesSplit](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.TimeSeriesSplit.html) lacks the flexibility of having multiple samples within the same time period or time unit.
+The current implementation of [scikit-learn TimeSeriesSplit](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.TimeSeriesSplit.html){:target="_blank"} lacks the flexibility of having multiple samples within the same time period (or time unit).
 
-**timebasedcv** addresses such problem by providing a cross validation strategy based on a **time unit** rather than the number of samples. This is useful when the data is time dependent, and the split should keep together samples within the same time window.
+**timebasedcv** addresses such problem by providing a cross validation strategy based on a **time period** rather than the number of samples. This is useful when the data is time dependent, and the split should keep together samples within the same time window.
 
-Temporal data leakage is an issue and we want to prevent that from happening by providing splits to make sure that models can train on past data and tested on future data, independently from the number of observations present within a given time period.
+Temporal data leakage is an issue and we want to prevent it from happening by providing splits that make sure the past and the future are well separated, so that data leakage does not spoil in a model cross validation.
 
-### Features ✨
+Again, these splits points solely depend on the time period and not the number of observations.
+
+### Features 📜
 
 We introduce two main classes:
 
 - [`TimeBasedSplit`](https://fbruzzesi.github.io/timebasedcv/api/timebasedcv/#timebasedcv.core.TimeBasedSplit) allows to define a split based on time unit (frequency), train size, test size, gap, stride, window type and mode. Remark that `TimeBasedSplit` is **not** compatible with [scikit-learn CV Splitters](https://scikit-learn.org/stable/common_pitfalls.html#id3). In fact, we have made the (opinioned) choice to:
 
   - Return the sliced arrays from `.split(...)`, while scikit-learn CV Splitters return train and test indices of the split.
   - Require to pass the time series as input to `.split(...)` method, while scikit-learn CV Splitters require to provide only `X, y, groups` to `.split(...)`.
   - Such time series is used to generate the boolean masks with which we slice the original arrays into train and test for each split.
 
 - Considering the above choices, we also provide a scikit-learn compatible splitter: [`TimeBasedCVSplitter`](https://fbruzzesi.github.io/timebasedcv/api/sklearn/#timebasedcv.sklearn.TimeBasedCVSplitter). Considering the signature that `.split(...)` requires and the fact that CV Splitters need to know a priori the number of splits, `TimeBasedCVSplitter` is initialized with the time series containing the time information used to generate the train and test indices of each split.
 
-## Installation
+## Installation 💻
 
 TL;DR:
 
 ```bash
 python -m pip install timebasedcv
 ```
 
 For further information, please refer to the dedicated [installation](https://fbruzzesi.github.io/timebasedcv/installation) section.
 
-## Quickstart
+## Quickstart 🏃
 
 The following code snippet is all you need to get started, yet consider checking out the [getting started](https://fbruzzesi.github.io/timebasedcv/user-guide/getting-started/) section of the documentation for a detailed guide on how to use the library.
 
 The main takeaway should be that `TimeBasedSplit` allows for a lot of flexibility at the cost of having to specify a long list of parameters. This is what makes the library so powerful and flexible to cover the large majority of use cases.
 
 First let's generate some data with different number of points per day:
 
@@ -212,14 +214,14 @@
 
 As we can see, each split does not necessarely have the same number of points, this is because the time series has a different number of points per day.
 
 A picture is worth a thousand words, let's visualize the splits (blue dots represent the train points, while the red dots represent the forecastng points):
 
 ![cross-validation](docs/img/basic-cv-split.png)
 
-## Contributing
+## Contributing ✌️
 
 Please read the [Contributing guidelines](https://fbruzzesi.github.io/timebasedcv/contribute/) in the documentation site.
 
-## License
+## License 👀
 
 The project has a [MIT Licence](https://github.com/FBruzzesi/timebasedcv/blob/main/LICENSE)
```

