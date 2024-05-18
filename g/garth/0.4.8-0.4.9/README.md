# Comparing `tmp/garth-0.4.8.tar.gz` & `tmp/garth-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.4.8.tar", last modified: Wed Aug  9 17:08:44 2023, max compression
+gzip compressed data, was "garth-0.4.9.tar", last modified: Wed Aug  9 17:30:44 2023, max compression
```

## Comparing `garth-0.4.8.tar` & `garth-0.4.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.8/LICENSE
--rw-r--r--   0        0        0    13307 2023-08-06 16:08:54.789312 garth-0.4.8/README.md
--rw-r--r--   0        0        0      701 2023-08-09 04:47:33.156063 garth-0.4.8/garth/__init__.py
--rw-r--r--   0        0        0      796 2023-08-04 15:13:28.651836 garth-0.4.8/garth/auth_tokens.py
--rw-r--r--   0        0        0      349 2023-08-09 04:47:33.159610 garth-0.4.8/garth/exc.py
--rw-r--r--   0        0        0     5546 2023-08-09 04:47:33.159734 garth-0.4.8/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.8/garth/py.typed
--rw-r--r--   0        0        0     4629 2023-08-06 15:02:02.370079 garth-0.4.8/garth/sso.py
--rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.8/garth/stats/__init__.py
--rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.8/garth/stats/_base.py
--rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.8/garth/stats/hrv.py
--rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.8/garth/stats/intensity_minutes.py
--rw-r--r--   0        0        0     3519 2023-08-09 17:08:00.942115 garth-0.4.8/garth/stats/sleep.py
--rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.8/garth/stats/steps.py
--rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.8/garth/stats/stress.py
--rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.8/garth/utils.py
--rw-r--r--   0        0        0       22 2023-08-09 17:08:23.354151 garth-0.4.8/garth/version.py
--rw-r--r--   0        0        0     1217 2023-08-09 17:08:44.574017 garth-0.4.8/pyproject.toml
--rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.8/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.8/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.8/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    50890 2023-08-04 23:53:42.180823 garth-0.4.8/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    54154 2023-08-04 23:59:00.720080 garth-0.4.8/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0    71602 2023-08-04 23:53:07.635030 garth-0.4.8/tests/cassettes/test_login_success_mfa.yaml
--rw-r--r--   0        0        0     8025 2023-08-06 15:02:02.370447 garth-0.4.8/tests/cassettes/test_refresh_oauth2_token.yaml
--rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.8/tests/cassettes/test_username.yaml
--rw-r--r--   0        0        0     3697 2023-08-09 04:56:27.707582 garth-0.4.8/tests/conftest.py
--rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.8/tests/stats/cassettes/test_daily_hrv.yaml
--rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.8/tests/stats/cassettes/test_daily_hrv_no_results.yaml
--rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.8/tests/stats/cassettes/test_daily_hrv_paginate.yaml
--rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.8/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
--rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.8/tests/stats/cassettes/test_daily_intensity_minutes.yaml
--rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.8/tests/stats/cassettes/test_daily_sleep.yaml
--rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.8/tests/stats/cassettes/test_daily_steps.yaml
--rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.8/tests/stats/cassettes/test_daily_stress.yaml
--rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.8/tests/stats/cassettes/test_daily_stress_pagination.yaml
--rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.8/tests/stats/cassettes/test_sleep_data_get.yaml
--rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.8/tests/stats/cassettes/test_sleep_data_list.yaml
--rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.8/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
--rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.8/tests/stats/cassettes/test_weekly_steps.yaml
--rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.8/tests/stats/cassettes/test_weekly_stress.yaml
--rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.8/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
--rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.8/tests/stats/cassettes/test_weekly_stress_pagination.yaml
--rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.8/tests/stats/test_hrv.py
--rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.8/tests/stats/test_intensity_minutes.py
--rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.8/tests/stats/test_sleep.py
--rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.8/tests/stats/test_steps.py
--rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.8/tests/stats/test_stress.py
--rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.8/tests/test_auth_tokens.py
--rw-r--r--   0        0        0     4177 2023-08-09 04:58:24.331059 garth-0.4.8/tests/test_http.py
--rw-r--r--   0        0        0     2674 2023-08-09 04:47:33.160003 garth-0.4.8/tests/test_sso.py
--rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.8/tests/test_utils.py
--rw-r--r--   0        0        0    13787 1970-01-01 00:00:00.000000 garth-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.9/LICENSE
+-rw-r--r--   0        0        0    13307 2023-08-06 16:08:54.789312 garth-0.4.9/README.md
+-rw-r--r--   0        0        0      701 2023-08-09 04:47:33.156063 garth-0.4.9/garth/__init__.py
+-rw-r--r--   0        0        0      796 2023-08-04 15:13:28.651836 garth-0.4.9/garth/auth_tokens.py
+-rw-r--r--   0        0        0      349 2023-08-09 04:47:33.159610 garth-0.4.9/garth/exc.py
+-rw-r--r--   0        0        0     5546 2023-08-09 04:47:33.159734 garth-0.4.9/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.9/garth/py.typed
+-rw-r--r--   0        0        0     4629 2023-08-06 15:02:02.370079 garth-0.4.9/garth/sso.py
+-rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.9/garth/stats/__init__.py
+-rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.9/garth/stats/_base.py
+-rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.9/garth/stats/hrv.py
+-rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.9/garth/stats/intensity_minutes.py
+-rw-r--r--   0        0        0     4262 2023-08-09 17:21:24.660526 garth-0.4.9/garth/stats/sleep.py
+-rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.9/garth/stats/steps.py
+-rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.9/garth/stats/stress.py
+-rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.9/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-08-09 17:29:57.507148 garth-0.4.9/garth/version.py
+-rw-r--r--   0        0        0     1179 2023-08-09 17:30:44.690882 garth-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.9/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.9/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.9/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    50890 2023-08-04 23:53:42.180823 garth-0.4.9/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    54154 2023-08-04 23:59:00.720080 garth-0.4.9/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0    71602 2023-08-04 23:53:07.635030 garth-0.4.9/tests/cassettes/test_login_success_mfa.yaml
+-rw-r--r--   0        0        0     8025 2023-08-06 15:02:02.370447 garth-0.4.9/tests/cassettes/test_refresh_oauth2_token.yaml
+-rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.9/tests/cassettes/test_username.yaml
+-rw-r--r--   0        0        0     3697 2023-08-09 04:56:27.707582 garth-0.4.9/tests/conftest.py
+-rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.9/tests/stats/cassettes/test_daily_hrv.yaml
+-rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.9/tests/stats/cassettes/test_daily_hrv_no_results.yaml
+-rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.9/tests/stats/cassettes/test_daily_hrv_paginate.yaml
+-rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.9/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
+-rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.9/tests/stats/cassettes/test_daily_intensity_minutes.yaml
+-rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.9/tests/stats/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.9/tests/stats/cassettes/test_daily_steps.yaml
+-rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.9/tests/stats/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.9/tests/stats/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.9/tests/stats/cassettes/test_sleep_data_get.yaml
+-rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.9/tests/stats/cassettes/test_sleep_data_list.yaml
+-rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.9/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
+-rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.9/tests/stats/cassettes/test_weekly_steps.yaml
+-rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.9/tests/stats/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.9/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.9/tests/stats/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.9/tests/stats/test_hrv.py
+-rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.9/tests/stats/test_intensity_minutes.py
+-rw-r--r--   0        0        0      947 2023-08-09 17:28:01.472198 garth-0.4.9/tests/stats/test_sleep.py
+-rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.9/tests/stats/test_steps.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.9/tests/stats/test_stress.py
+-rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.9/tests/test_auth_tokens.py
+-rw-r--r--   0        0        0     4177 2023-08-09 04:58:24.331059 garth-0.4.9/tests/test_http.py
+-rw-r--r--   0        0        0     2674 2023-08-09 04:47:33.160003 garth-0.4.9/tests/test_sso.py
+-rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.9/tests/test_utils.py
+-rw-r--r--   0        0        0    13759 1970-01-01 00:00:00.000000 garth-0.4.9/PKG-INFO
```

### Comparing `garth-0.4.8/LICENSE` & `garth-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/README.md` & `garth-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/__init__.py` & `garth-0.4.9/garth/__init__.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/auth_tokens.py` & `garth-0.4.9/garth/auth_tokens.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/http.py` & `garth-0.4.9/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/sso.py` & `garth-0.4.9/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/stats/_base.py` & `garth-0.4.9/garth/stats/_base.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/stats/hrv.py` & `garth-0.4.9/garth/stats/hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/stats/intensity_minutes.py` & `garth-0.4.9/garth/stats/intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/stats/sleep.py` & `garth-0.4.9/garth/stats/sleep.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import date, datetime
+from datetime import date, datetime, timedelta, timezone
 from typing import ClassVar, Optional
 
 from pydantic.dataclasses import dataclass
 
 from .. import http
 from ..utils import camel_to_snake_dict, date_range, format_end_date
 from ._base import Stats
@@ -76,14 +76,34 @@
     lowest_respiration_value: Optional[float] = None
     highest_respiration_value: Optional[float] = None
     avg_sleep_stress: Optional[float] = None
     age_group: Optional[str] = None
     sleep_score_feedback: Optional[str] = None
     sleep_score_insight: Optional[str] = None
 
+    def _get_localized_datetime(
+        self, gmt_timestamp: int, local_timestamp: int
+    ) -> datetime:
+        local_diff = local_timestamp - gmt_timestamp
+        local_offset = timezone(timedelta(milliseconds=local_diff))
+        gmt_time = datetime.fromtimestamp(gmt_timestamp / 1000, timezone.utc)
+        return gmt_time.astimezone(local_offset)
+
+    @property
+    def sleep_start(self) -> datetime:
+        return self._get_localized_datetime(
+            self.sleep_start_timestamp_gmt, self.sleep_start_timestamp_local
+        )
+
+    @property
+    def sleep_end(self) -> datetime:
+        return self._get_localized_datetime(
+            self.sleep_end_timestamp_gmt, self.sleep_end_timestamp_local
+        )
+
 
 @dataclass(frozen=True)
 class SleepMovement:
     start_gmt: datetime
     end_gmt: datetime
     activity_level: float
```

### Comparing `garth-0.4.8/garth/stats/steps.py` & `garth-0.4.9/garth/stats/steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/stats/stress.py` & `garth-0.4.9/garth/stats/stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/garth/utils.py` & `garth-0.4.9/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/pyproject.toml` & `garth-0.4.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 authors = [
     { name = "Matin Tamizi", email = "mtamizi@duck.com" },
 ]
 dependencies = [
     "requests",
     "pydantic",
     "requests-oauthlib>=1.3.1",
-    "pytz>=2023.3",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
-version = "0.4.8"
+version = "0.4.9"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -57,14 +56,13 @@
 ]
 linting = [
     "black",
     "ruff",
     "mypy",
     "isort",
     "types-requests",
-    "types-pytz",
 ]
 testing = [
     "coverage",
     "pytest",
     "pytest-vcr",
 ]
```

### Comparing `garth-0.4.8/tests/cassettes/test_client_request.yaml` & `garth-0.4.9/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/cassettes/test_connectapi.yaml` & `garth-0.4.9/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/cassettes/test_exchange.yaml` & `garth-0.4.9/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.4.9/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/cassettes/test_login_success.yaml` & `garth-0.4.9/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/cassettes/test_login_success_mfa.yaml` & `garth-0.4.9/tests/cassettes/test_login_success_mfa.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/cassettes/test_refresh_oauth2_token.yaml` & `garth-0.4.9/tests/cassettes/test_refresh_oauth2_token.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/cassettes/test_username.yaml` & `garth-0.4.9/tests/cassettes/test_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/conftest.py` & `garth-0.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_daily_hrv.yaml` & `garth-0.4.9/tests/stats/cassettes/test_daily_hrv.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_daily_hrv_no_results.yaml` & `garth-0.4.9/tests/stats/cassettes/test_daily_hrv_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_daily_hrv_paginate.yaml` & `garth-0.4.9/tests/stats/cassettes/test_daily_hrv_paginate.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml` & `garth-0.4.9/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_daily_intensity_minutes.yaml` & `garth-0.4.9/tests/stats/cassettes/test_daily_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_daily_sleep.yaml` & `garth-0.4.9/tests/stats/cassettes/test_daily_sleep.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_daily_steps.yaml` & `garth-0.4.9/tests/stats/cassettes/test_daily_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_daily_stress.yaml` & `garth-0.4.9/tests/stats/cassettes/test_daily_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_daily_stress_pagination.yaml` & `garth-0.4.9/tests/stats/cassettes/test_daily_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_sleep_data_get.yaml` & `garth-0.4.9/tests/stats/cassettes/test_sleep_data_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_sleep_data_list.yaml` & `garth-0.4.9/tests/stats/cassettes/test_sleep_data_list.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_weekly_intensity_minutes.yaml` & `garth-0.4.9/tests/stats/cassettes/test_weekly_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_weekly_steps.yaml` & `garth-0.4.9/tests/stats/cassettes/test_weekly_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_weekly_stress.yaml` & `garth-0.4.9/tests/stats/cassettes/test_weekly_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml` & `garth-0.4.9/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/cassettes/test_weekly_stress_pagination.yaml` & `garth-0.4.9/tests/stats/cassettes/test_weekly_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/test_hrv.py` & `garth-0.4.9/tests/stats/test_hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/test_intensity_minutes.py` & `garth-0.4.9/tests/stats/test_intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/test_sleep.py` & `garth-0.4.9/tests/stats/test_sleep.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     assert len(daily_sleep) == days
 
 
 @pytest.mark.vcr
 def test_sleep_data_get(authed_client: Client):
     sleep_data = SleepData.get("2021-07-20", client=authed_client)
     assert sleep_data.daily_sleep_dto.calendar_date == date(2021, 7, 20)
+    assert sleep_data.daily_sleep_dto.sleep_start
+    assert sleep_data.daily_sleep_dto.sleep_end
 
 
 @pytest.mark.vcr
 def test_sleep_data_list(authed_client: Client):
     end = date(2021, 7, 20)
     days = 20
     sleep_data = SleepData.list(end, days, client=authed_client)
```

### Comparing `garth-0.4.8/tests/stats/test_steps.py` & `garth-0.4.9/tests/stats/test_steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/stats/test_stress.py` & `garth-0.4.9/tests/stats/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/test_http.py` & `garth-0.4.9/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/test_sso.py` & `garth-0.4.9/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/tests/test_utils.py` & `garth-0.4.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.8/PKG-INFO` & `garth-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.4.8
+Version: 0.4.9
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Requires-Dist: requests
 Requires-Dist: pydantic
 Requires-Dist: requests-oauthlib>=1.3.1
-Requires-Dist: pytz>=2023.3
 Description-Content-Type: text/markdown
 
 # Garth
 
 [![CI](https://github.com/matin/garth/workflows/CI/badge.svg?event=push)](https://github.com/matin/garth/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![codecov](https://codecov.io/gh/matin/garth/branch/main/graph/badge.svg?token=0EFFYJNFIL)](https://codecov.io/gh/matin/garth)
```

