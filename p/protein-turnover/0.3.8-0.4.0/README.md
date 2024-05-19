# Comparing `tmp/protein_turnover-0.3.8.tar.gz` & `tmp/protein_turnover-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_turnover-0.3.8.tar", max compression
+gzip compressed data, was "protein_turnover-0.4.0.tar", max compression
```

## Comparing `protein_turnover-0.3.8.tar` & `protein_turnover-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1068 2024-04-10 10:25:59.389801 protein_turnover-0.3.8/LICENSE
--rw-r--r--   0        0        0       54 2024-04-26 05:23:38.437576 protein_turnover-0.3.8/prerelease.md
--rw-r--r--   0        0        0        0 2022-09-06 02:29:35.838848 protein_turnover-0.3.8/protein_turnover/__init__.py
--rw-r--r--   0        0        0      481 2024-04-12 09:19:03.438815 protein_turnover-0.3.8/protein_turnover/__main__.py
--rw-r--r--   0        0        0      142 2024-04-18 09:07:07.364073 protein_turnover-0.3.8/protein_turnover/api.py
--rw-r--r--   0        0        0     9778 2024-04-15 08:28:10.056355 protein_turnover-0.3.8/protein_turnover/background.py
--rw-r--r--   0        0        0     1594 2024-04-11 07:40:50.403214 protein_turnover-0.3.8/protein_turnover/background_ui.py
--rw-r--r--   0        0        0     6670 2024-04-11 05:21:49.849892 protein_turnover-0.3.8/protein_turnover/broken_api.py
--rw-r--r--   0        0        0     2745 2024-04-11 02:01:52.718758 protein_turnover-0.3.8/protein_turnover/cli.py
--rw-r--r--   0        0        0     1390 2024-04-18 06:46:32.496210 protein_turnover-0.3.8/protein_turnover/config.py
--rw-r--r--   0        0        0        0 2023-04-17 04:28:06.153132 protein_turnover-0.3.8/protein_turnover/dinosaur/__init__.py
--rw-r--r--   0        0        0     3062 2023-08-29 07:02:47.263592 protein_turnover-0.3.8/protein_turnover/dinosaur/cmd.py
--rw-r--r--   0        0        0     1918 2024-04-10 08:19:00.355662 protein_turnover-0.3.8/protein_turnover/dinosaur/dinosaur.py
--rw-r--r--   0        0        0     1691 2023-11-01 09:45:31.835472 protein_turnover-0.3.8/protein_turnover/filters.py
--rw-r--r--   0        0        0    19858 2024-03-28 01:40:54.972101 protein_turnover-0.3.8/protein_turnover/fitenvelopes.py
--rw-r--r--   0        0        0     7124 2024-04-15 08:28:10.056355 protein_turnover-0.3.8/protein_turnover/jobs.py
--rw-r--r--   0        0        0     1511 2023-10-31 22:36:14.534600 protein_turnover-0.3.8/protein_turnover/logger.py
--rw-r--r--   0        0        0      981 2023-08-28 10:18:07.794829 protein_turnover-0.3.8/protein_turnover/mailer.py
--rw-r--r--   0        0        0     2708 2024-04-11 05:19:39.944840 protein_turnover-0.3.8/protein_turnover/parallel_utils.py
--rw-r--r--   0        0        0    12680 2024-04-11 11:28:05.946176 protein_turnover-0.3.8/protein_turnover/pepxml.py
--rw-r--r--   0        0        0    29793 2023-11-06 13:19:24.639523 protein_turnover-0.3.8/protein_turnover/pepxml_reader.py
--rw-r--r--   0        0        0     4181 2024-04-11 03:10:41.293175 protein_turnover-0.3.8/protein_turnover/pepxml_ui.py
--rw-r--r--   0        0        0    18499 2023-10-31 22:36:18.510700 protein_turnover-0.3.8/protein_turnover/plotting.py
--rw-r--r--   0        0        0     3817 2024-02-06 08:48:02.313547 protein_turnover-0.3.8/protein_turnover/protxml.py
--rw-r--r--   0        0        0        0 2023-08-29 04:01:11.951477 protein_turnover-0.3.8/protein_turnover/py.typed
--rw-r--r--   0        0        0    26888 2024-04-26 00:23:46.745567 protein_turnover-0.3.8/protein_turnover/pymz.py
--rw-r--r--   0        0        0    10050 2024-04-24 05:27:48.262533 protein_turnover-0.3.8/protein_turnover/pymz_ui.py
--rw-r--r--   0        0        0     2571 2023-09-01 03:32:11.939419 protein_turnover-0.3.8/protein_turnover/settings.py
--rw-r--r--   0        0        0     2726 2023-11-05 07:06:29.593017 protein_turnover-0.3.8/protein_turnover/sns.py
--rw-r--r--   0        0        0        0 2022-11-02 03:43:40.908584 protein_turnover-0.3.8/protein_turnover/sqla/__init__.py
--rw-r--r--   0        0        0     4791 2024-04-02 05:33:08.127208 protein_turnover-0.3.8/protein_turnover/sqla/iso_peaks.py
--rw-r--r--   0        0        0     3982 2024-04-12 09:19:03.622817 protein_turnover-0.3.8/protein_turnover/sqla/iso_peaks_ui.py
--rw-r--r--   0        0        0    12901 2024-04-11 04:06:36.929908 protein_turnover-0.3.8/protein_turnover/sqla/model.py
--rw-r--r--   0        0        0    20036 2024-04-10 06:44:53.511669 protein_turnover-0.3.8/protein_turnover/sqla/query.py
--rw-r--r--   0        0        0     5249 2024-02-14 07:30:52.792197 protein_turnover-0.3.8/protein_turnover/sqla/utils.py
--rw-r--r--   0        0        0        0 2022-09-06 02:29:35.846848 protein_turnover-0.3.8/protein_turnover/types/__init__.py
--rw-r--r--   0        0        0     7955 2023-11-03 02:17:35.435401 protein_turnover-0.3.8/protein_turnover/types/checking.py
--rw-r--r--   0        0        0      956 2023-08-28 10:18:07.838829 protein_turnover-0.3.8/protein_turnover/types/mzmltypes.py
--rw-r--r--   0        0        0     1874 2023-08-28 10:18:07.806829 protein_turnover-0.3.8/protein_turnover/types/pepxmltypes.py
--rw-r--r--   0        0        0     2594 2023-08-28 10:18:07.838829 protein_turnover-0.3.8/protein_turnover/types/turnovertype.py
--rw-r--r--   0        0        0     7509 2023-11-05 22:47:34.227461 protein_turnover-0.3.8/protein_turnover/unimod.py
--rw-r--r--   0        0        0    20458 2024-04-18 12:12:35.320150 protein_turnover-0.3.8/protein_turnover/utils.py
--rw-r--r--   0        0        0     5798 2024-04-15 04:58:55.719116 protein_turnover-0.3.8/protein_turnover/web.py
--rw-r--r--   0        0        0     2614 2024-04-15 08:27:59.960224 protein_turnover-0.3.8/protein_turnover/web_ui.py
--rw-r--r--   0        0        0     1154 2024-04-26 05:23:56.101740 protein_turnover-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 protein_turnover-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-10 10:25:59.389801 protein_turnover-0.4.0/LICENSE
+-rw-r--r--   0        0        0       54 2024-04-26 05:23:38.437576 protein_turnover-0.4.0/prerelease.md
+-rw-r--r--   0        0        0        0 2022-09-06 02:29:35.838848 protein_turnover-0.4.0/protein_turnover/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-12 09:19:03.438815 protein_turnover-0.4.0/protein_turnover/__main__.py
+-rw-r--r--   0        0        0      142 2024-04-18 09:07:07.364073 protein_turnover-0.4.0/protein_turnover/api.py
+-rw-r--r--   0        0        0    11218 2024-05-17 13:48:47.050662 protein_turnover-0.4.0/protein_turnover/background.py
+-rw-r--r--   0        0        0     1615 2024-05-17 03:46:28.509498 protein_turnover-0.4.0/protein_turnover/background_ui.py
+-rw-r--r--   0        0        0     6670 2024-05-18 20:24:19.465998 protein_turnover-0.4.0/protein_turnover/broken_api.py
+-rw-r--r--   0        0        0     2683 2024-05-19 06:28:47.088765 protein_turnover-0.4.0/protein_turnover/cli.py
+-rw-r--r--   0        0        0     1086 2024-05-19 06:36:37.017269 protein_turnover-0.4.0/protein_turnover/config.py
+-rw-r--r--   0        0        0     2439 2024-05-19 06:23:04.469379 protein_turnover-0.4.0/protein_turnover/config2.py
+-rw-r--r--   0        0        0        0 2023-04-17 04:28:06.153132 protein_turnover-0.4.0/protein_turnover/dinosaur/__init__.py
+-rw-r--r--   0        0        0     3062 2023-08-29 07:02:47.263592 protein_turnover-0.4.0/protein_turnover/dinosaur/cmd.py
+-rw-r--r--   0        0        0     1914 2024-05-19 04:54:45.120734 protein_turnover-0.4.0/protein_turnover/dinosaur/dinosaur.py
+-rw-r--r--   0        0        0      393 2024-05-18 20:23:03.965361 protein_turnover-0.4.0/protein_turnover/exts.py
+-rw-r--r--   0        0        0     1691 2023-11-01 09:45:31.835472 protein_turnover-0.4.0/protein_turnover/filters.py
+-rw-r--r--   0        0        0    19860 2024-05-17 22:50:45.333397 protein_turnover-0.4.0/protein_turnover/fitenvelopes.py
+-rw-r--r--   0        0        0     8516 2024-05-17 11:31:30.621734 protein_turnover-0.4.0/protein_turnover/jobs.py
+-rw-r--r--   0        0        0     1511 2023-10-31 22:36:14.534600 protein_turnover-0.4.0/protein_turnover/logger.py
+-rw-r--r--   0        0        0      981 2023-08-28 10:18:07.794829 protein_turnover-0.4.0/protein_turnover/mailer.py
+-rw-r--r--   0        0        0     2708 2024-04-11 05:19:39.944840 protein_turnover-0.4.0/protein_turnover/parallel_utils.py
+-rw-r--r--   0        0        0    12689 2024-05-17 05:04:12.311778 protein_turnover-0.4.0/protein_turnover/pepxml.py
+-rw-r--r--   0        0        0    29793 2023-11-06 13:19:24.639523 protein_turnover-0.4.0/protein_turnover/pepxml_reader.py
+-rw-r--r--   0        0        0    18506 2024-04-29 01:52:56.745780 protein_turnover-0.4.0/protein_turnover/plotting.py
+-rw-r--r--   0        0        0     3826 2024-05-17 05:04:43.620071 protein_turnover-0.4.0/protein_turnover/protxml.py
+-rw-r--r--   0        0        0        0 2023-08-29 04:01:11.951477 protein_turnover-0.4.0/protein_turnover/py.typed
+-rw-r--r--   0        0        0    27261 2024-05-19 03:53:22.049512 protein_turnover-0.4.0/protein_turnover/pymz.py
+-rw-r--r--   0        0        0    10895 2024-05-19 07:29:37.874358 protein_turnover-0.4.0/protein_turnover/pymz_ui.py
+-rw-r--r--   0        0        0     2571 2023-09-01 03:32:11.939419 protein_turnover-0.4.0/protein_turnover/settings.py
+-rw-r--r--   0        0        0     2726 2023-11-05 07:06:29.593017 protein_turnover-0.4.0/protein_turnover/sns.py
+-rw-r--r--   0        0        0        0 2022-11-02 03:43:40.908584 protein_turnover-0.4.0/protein_turnover/sqla/__init__.py
+-rw-r--r--   0        0        0     4791 2024-04-02 05:33:08.127208 protein_turnover-0.4.0/protein_turnover/sqla/iso_peaks.py
+-rw-r--r--   0        0        0     3982 2024-04-12 09:19:03.622817 protein_turnover-0.4.0/protein_turnover/sqla/iso_peaks_ui.py
+-rw-r--r--   0        0        0    12901 2024-05-17 05:11:50.442492 protein_turnover-0.4.0/protein_turnover/sqla/model.py
+-rw-r--r--   0        0        0    20036 2024-04-10 06:44:53.511669 protein_turnover-0.4.0/protein_turnover/sqla/query.py
+-rw-r--r--   0        0        0     5249 2024-02-14 07:30:52.792197 protein_turnover-0.4.0/protein_turnover/sqla/utils.py
+-rw-r--r--   0        0        0        0 2022-09-06 02:29:35.846848 protein_turnover-0.4.0/protein_turnover/types/__init__.py
+-rw-r--r--   0        0        0     7955 2023-11-03 02:17:35.435401 protein_turnover-0.4.0/protein_turnover/types/checking.py
+-rw-r--r--   0        0        0      956 2023-08-28 10:18:07.838829 protein_turnover-0.4.0/protein_turnover/types/mzmltypes.py
+-rw-r--r--   0        0        0     1874 2023-08-28 10:18:07.806829 protein_turnover-0.4.0/protein_turnover/types/pepxmltypes.py
+-rw-r--r--   0        0        0     2594 2023-08-28 10:18:07.838829 protein_turnover-0.4.0/protein_turnover/types/turnovertype.py
+-rw-r--r--   0        0        0     7509 2023-11-05 22:47:34.227461 protein_turnover-0.4.0/protein_turnover/unimod.py
+-rw-r--r--   0        0        0    21118 2024-05-18 20:30:54.981335 protein_turnover-0.4.0/protein_turnover/utils.py
+-rw-r--r--   0        0        0     9788 2024-05-19 07:19:49.969162 protein_turnover-0.4.0/protein_turnover/web.py
+-rw-r--r--   0        0        0     6383 2024-05-19 08:16:02.332675 protein_turnover-0.4.0/protein_turnover/web_ui.py
+-rw-r--r--   0        0        0     1393 2024-05-19 09:00:24.475058 protein_turnover-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 protein_turnover-0.4.0/PKG-INFO
```

### Comparing `protein_turnover-0.3.8/LICENSE` & `protein_turnover-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/background.py` & `protein_turnover-0.4.0/protein_turnover/background.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,32 +81,70 @@
     def __call__(self, signum: int, frame: Any) -> None:
         if self.processing:
             return
         raise ContinueException()
 
 
 PID_FILENAME = "turnover.pid"
+PROCESSING = "turnover.pid.is_running"
+
+
+class Processing:
+    """Is the background worker processing a job ATM?"""
+
+    def __init__(self, jobsdir: Path):
+        self._processing = jobsdir.joinpath(PROCESSING)
+
+    def is_processing(self) -> bool:
+        return self._processing.exists()
+
+    def set_processing(self, start: bool) -> None:
+        if start:
+            self._processing.touch()
+        else:
+            try:
+                self._processing.unlink(missing_ok=True)
+            except OSError:
+                pass
+
+
+def signal_me() -> signal.Signals:
+    if sys.platform == "win32":
+        return signal.SIGBREAK
+    return signal.SIGCONT
 
 
 class SimpleQueueClient:
     """Used by web client to interact with background Queue.
 
     Currently only just sends a signal to wake up.
     """
 
     def __init__(self, jobdir: Path):
         self.jobdir = jobdir
         self.pidfile = jobdir.joinpath(PID_FILENAME)
 
+    def terminate(self) -> bool:
+        pid = self.get_pid()
+        if pid is None:
+            return False
+        try:
+            os.kill(pid, signal.SIGINT)
+        except ProcessLookupError:
+            return False
+        except PermissionError:
+            return False
+        return True
+
     def signal(self) -> bool:
         pid = self.get_pid()
         if pid is None:
             return False
         try:
-            os.kill(pid, signal.SIGCONT)
+            os.kill(pid, signal_me())
         except ProcessLookupError:
             return False
         except PermissionError:
             return False
         return True
 
     def is_running(self) -> bool:
@@ -151,15 +189,16 @@
             if not os.path.exists(config):
                 logger.warning(
                     "configuration file %s doesn't exist! ignoring...",
                     config,
                 )
                 config = None
         self.config = config
-        signal.signal(signal.SIGCONT, self.handler)
+        self.processing = Processing(Path(jobdir))
+        signal.signal(signal_me(), self.handler)
 
     def command(self, *args: str) -> list[str]:
         nice = []
         if self.nice_cmd and self.nice:
             nice = [self.nice_cmd, "-n", str(self.nice)]
 
         config = [f"--config={self.config}"] if self.config is not None else []
@@ -191,40 +230,47 @@
             self.rmlog(tomlfile)
 
             with subprocess.Popen(
                 self.command(str(tomlfile)),
                 shell=False,
                 text=True,
             ) as proc:
-                logger.info("%s: running pid=%d", tomlfile, proc.pid)
-                # let website know that this job is running....
-                # see SimpleQueueClient
-                pid = self.pidfile(tomlfile)
-                with pid.open("w") as fp:
-                    fp.write(str(proc.pid))
-                try:
-                    _, errs = proc.communicate()
-                    if errs:
-                        logger.error("error from %s: %s", tomlfile, errs)
-                    ret = proc.wait()  # TODO what happens when we're terminated?
-                finally:  # can catch KeyboardInterrupt
-                    pid.unlink(missing_ok=True)
-                if ret < 0:
-                    if -ret in {signal.SIGTERM, signal.SIGKILL}:
-                        logger.warning("%s: killed...", tomlfile)
-                status = (
-                    "finished"
-                    if ret == 0
-                    else ("killed" if ret < 0 or ret == self.INTERROR else "failed")
-                )
-                logger.info("%s: status=%s", tomlfile, status)
                 try:
-                    self.update_status(tomlfile, status)
-                except Exception as e:
-                    logger.error("can't update status! %s: %s", tomlfile, e)
+                    logger.info("%s: running pid=%d", tomlfile, proc.pid)
+                    # let website know that this job is running....
+                    # see SimpleQueueClient
+                    pid = self.pidfile(tomlfile)
+                    with pid.open("w") as fp:
+                        fp.write(str(proc.pid))
+                    self.processing.set_processing(True)
+                    try:
+                        _, errs = proc.communicate()
+                        if errs:
+                            logger.error("error from %s: %s", tomlfile, errs)
+                        ret = proc.wait()  # TODO what happens when we're terminated?
+                    finally:  # can catch KeyboardInterrupt
+                        pid.unlink(missing_ok=True)
+                        self.processing.set_processing(False)
+                    if ret < 0:
+                        if -ret in {signal.SIGTERM, signal.SIGKILL}:
+                            logger.warning("%s: killed...", tomlfile)
+                    status = (
+                        "finished"
+                        if ret == 0
+                        else ("killed" if ret < 0 or ret == self.INTERROR else "failed")
+                    )
+                    logger.info("%s: status=%s", tomlfile, status)
+                    try:
+                        self.update_status(tomlfile, status)
+                    except Exception as e:
+                        logger.error("can't update status! %s: %s", tomlfile, e)
+                except KeyboardInterrupt:
+                    logger.info("sending signal to child process")
+                    proc.send_signal(signal.SIGINT)
+                    raise
 
     def update_status(self, tomlfile: Path, status: str) -> None:
         c = self.read_toml(tomlfile)
         if c is None:
             return
         c["status"] = status
         with tomlfile.open("wb") as fp:
@@ -290,15 +336,15 @@
 
     def process(self, jobdir: str, wait: float = 60.0) -> None:
         self.runjobs(self.search(jobdir, wait))
 
     def run(self) -> None:
         pidfile = Path(self.jobdir).joinpath(PID_FILENAME)
         try:
-            with pidfile.open("w", encoding="utf-8") as fp:
+            with pidfile.open("wt", encoding="utf-8") as fp:
                 pid = os.getpid()
                 fp.write(str(pid))
             w = "with 👍" if psutil_ok else "without 👎"
             print(f"protein_turnover queue running ({w} psutil) as pid={pid}")
             self.process(self.jobdir, self.wait)
         finally:
             pidfile.unlink(missing_ok=True)
```

### Comparing `protein_turnover-0.3.8/protein_turnover/background_ui.py` & `protein_turnover-0.4.0/protein_turnover/background_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     type=click.Path(file_okay=True, dir_okay=False, exists=True),
     help="configuration file to pass off to the background process",
 )
 @click.option(
     "--no-email",
     is_flag=True,
     help="don't send any emails",
-    hidden=True,
+    hidden=False,
 )  # see runner.py
 @click.argument(
     "directory",
     type=click.Path(dir_okay=True, exists=True, file_okay=False),
 )
 @pass_config
 def background_cmd(
@@ -57,15 +57,16 @@
     from os import cpu_count
     from .background import SimpleQueue
 
     if workers is None:
         workers = max((cpu_count() or 1) // 2, 1)
         logger.warning("using %d workers", workers)
 
-    SimpleQueue(
+    squeue = SimpleQueue(
         directory,
         workers=workers,
         wait=sleep,
         nice=nice,
         config=run_config or cfg.user_config,
         no_email=no_email,
-    ).run()
+    )
+    squeue.run()
```

### Comparing `protein_turnover-0.3.8/protein_turnover/broken_api.py` & `protein_turnover-0.4.0/protein_turnover/broken_api.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/cli.py` & `protein_turnover-0.4.0/protein_turnover/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
+from pathlib import Path
 
 import click
 
 # from click_didyoumean import DYMGroup
 
 
 IsFile = click.Path(dir_okay=False, file_okay=True)
 
+CONFIG = Path("~/.turnover.toml").expanduser()
+
 
 @dataclass
 class Config:
-    logfile: bool
-    loglevel: bool
+    logfile: str | None = None
+    loglevel: str | None = None
     user_config: str | None = None
 
 
 pass_config = click.make_pass_decorator(Config, ensure=True)
 
 
 def update_mailhost(mailhost: str) -> None:
     from . import config
 
     config.MAIL_SERVER = mailhost
 
 
-def update_config(filename: str) -> None:
+def update_config(filename: str | Path) -> None:
     from . import config
     import tomli as tomllib
 
     try:
         with open(filename, "rb") as fp:
             d = tomllib.load(fp)
     except Exception as e:
         raise click.BadParameter(
             f"can't read configuration file: {e}",
             param_hint="config",
         )
 
     for k, v in d.items():
-        k = k.upper()
-        # don't changes these!
-        if k in {
-            "PEPXML",
-            "PROTXML",
-            "MZML",
-            "MZMAP",
-            "EICS",
-            "EXT",
-            "RESULT_EXT",
-            "VERSION",
-            "DINOSAUR",
-        }:
+        if k == "website":
             continue
+        k = k.upper()
         if hasattr(config, k):
             setattr(config, k, v)
         else:
             click.secho(f"unknown configuration attribute {k}", fg="red")
 
 
 @click.group(epilog=click.style("turnover commands\n", fg="magenta"))
@@ -81,15 +73,15 @@
     help="where to send emails to",
     metavar="HOST",
 )
 @click.option(
     "-c",
     "--config",
     type=click.Path(file_okay=True, dir_okay=False, exists=True),
-    help="configuration file for turnover",
+    help="configuration file for turnover [.TOML format]",
 )
 @click.version_option()
 @click.pass_context
 def cli(
     ctx: click.Context,
     level: str | None,
     logfile: str | None = None,
@@ -103,20 +95,23 @@
     # if not df_can_write_parquet():
     #     click.secho(
     #         "Please install pyarrow or fastparquet", fg="red", bold=True, err=True
     #     )
     #     raise click.Abort()
 
     ctx.obj = Config(
-        logfile=logfile is not None,
-        loglevel=level is not None,
+        logfile=logfile,
+        loglevel=level,
         user_config=config,
     )
     if level is None:
         level = "WARNING"
 
     if config is not None:
         update_config(config)
+    else:
+        if CONFIG.exists():
+            update_config(CONFIG)
     if mailhost is not None:
         update_mailhost(mailhost)
 
     init_logger(level=level, logfile=logfile)
```

### Comparing `protein_turnover-0.3.8/protein_turnover/dinosaur/cmd.py` & `protein_turnover-0.4.0/protein_turnover/dinosaur/cmd.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/dinosaur/dinosaur.py` & `protein_turnover-0.4.0/protein_turnover/dinosaur/dinosaur.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         return [str(javapath), "-jar", str(self.jarpath.absolute())]
 
     @classmethod
     def from_config(cls) -> DinoRunner | None:
         from ..config import DINOSAUR_JAR, JAVA_PATH
 
-        if DINOSAUR_JAR is None:
+        if not DINOSAUR_JAR:
             return None
         return DinoRunner(jarpath=Path(DINOSAUR_JAR), javapath=Path(JAVA_PATH))
 
     def can_run(self) -> bool:
         from shutil import which
 
         return self.jarpath.exists() and which(self.javapath) is not None
```

### Comparing `protein_turnover-0.3.8/protein_turnover/filters.py` & `protein_turnover-0.4.0/protein_turnover/filters.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/fitenvelopes.py` & `protein_turnover-0.4.0/protein_turnover/fitenvelopes.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     eicIds: np.ndarray,  # bool[N]
     mono_intensity: np.ndarray,  # float[N,3]
 ) -> Iterator[list[float]]:
     eic: np.ndarray
     for eic in rawEIC:
         try:
             intensity = eic[eicIds, 1]
-            x, residues, rank, s = lstsq(mono_intensity, intensity)
+            x, _residues, rank, _s = lstsq(mono_intensity, intensity)
             alpha, slope = x
             # if rank < 2:
             #     assert residues.shape == ()
             #     residue = np.nan
             # else:
             #     assert residues.shape == (0,)
             #     residue = float(np.sqrt(residues))
```

### Comparing `protein_turnover-0.3.8/protein_turnover/jobs.py` & `protein_turnover-0.4.0/protein_turnover/jobs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import re
+import sys
 import unicodedata
 from dataclasses import asdict
 from dataclasses import dataclass
 from dataclasses import fields
 from dataclasses import MISSING
 from os.path import commonprefix
 from os.path import sep
@@ -17,14 +18,24 @@
 
 from .utils import MzMLResourceFile
 from .utils import PeptideSettings
 from .utils import PepXMLResourceFile
 from .utils import ProtXMLResourceFile
 from .utils import ResourceFiles
 
+try:
+    from unidecode import unidecode
+except ImportError:
+
+    def unidecode(string: str, errors: str = "ignore", replace_str: str = "?") -> str:
+        return string
+
+
+WIDE = sys.maxunicode > 0xFFFF
+
 
 def find_prefix(filenames: Sequence[Path]) -> Path:
     prefix = commonprefix([Path(m).absolute() for m in filenames])
     if not prefix.endswith(sep):
         i = prefix.rfind(sep)
         if i > 0:
             prefix = prefix[: i + 1]
@@ -39,16 +50,41 @@
     m.update(str(Path(protxml).resolve()).encode("utf-8"))
     for s in mzmlfiles:
         m.update(str(Path(s).resolve()).encode("utf-8"))
 
     return m.hexdigest()
 
 
-def slugify(s: str) -> str:
-    s = unicodedata.normalize("NFKD", s)
+# def safe_jobid(job_name: str, filename: Path) -> str:
+
+#     jobid = slugify(filename.stem)
+#     if len(jobid) >= 5:
+#         return jobid
+#     if job_name:
+#         jobid = slugify(job_name)
+#     if not jobid or len(jobid) < 4:
+#         from hashlib import md5
+
+#         m = md5()
+#         with filename.open("rb") as fp:
+#             m.update(fp.read())
+#         jobid = m.hexdigest()
+
+#     return jobid
+
+
+def slugify(s: str, transliterate: bool = True) -> str:
+    if not s:
+        return s
+
+    if WIDE and transliterate:  # UCS-4 build of python
+        s = unidecode(s)
+    else:
+        s = unicodedata.normalize("NFKD", s)
+
     slug = s.encode("ascii", "ignore").lower()
     slug = re.sub(b"[^a-z0-9]+", b"-", slug).strip(b"-")
     slug = re.sub(b"[-]+", b"-", slug)
     return slug.decode("ascii")
 
 
 @dataclass
@@ -57,17 +93,18 @@
     pepxml: list[str]
     protxml: str
     mzmlfiles: list[str]
     jobid: str = ""
     settings: PeptideSettings = PeptideSettings()
     cache_dir: str | None = None
     email: str | None = None
-    status: str = "stopped"  # pending, started, finished, failed, stopped.
+    status: str | None = None  # pending, started, finished, failed, stopped.
     mzfile_to_run: dict[str, str] | None = None
     match_runNames: bool = False
+    auto_generated_jobid: bool = False
     """Match peptides to mzML files via their `spectrum` names"""
 
     def cache_ok(self) -> bool:
         return len(self.to_resource_files().todo()) == 0
 
     def get_mzfile_to_run(self) -> dict[str, str]:
         if self.mzfile_to_run is None:
@@ -137,19 +174,27 @@
         d["pepxml"] = [str(Path(m).resolve()) for m in self.pepxml]
         d["protxml"] = str(Path(d["protxml"]).resolve())
         d["mzmlfiles"] = [str(f.relative_to(prefix)) for f in mzmlfiles]
         d["mzmlprefix"] = str(Path(prefix).resolve())
         # d["settings"] = asdict(d["settings"])
         # settings = d.pop("settings")
         # d.update(settings)
+        if "auto_generated_jobid" in d:
+            del d["auto_generated_jobid"]
         with out.open("wb") as fp:
             tomli_w.dump(d, fp)
         return out
 
     @classmethod
+    def safe_jobid(cls, turnover_dict: dict[str, Any], filename: Path) -> str:
+        return filename.stem
+        # job_name = str(turnover_dict["job_name"])
+        # return safe_jobid(job_name, filename)
+
+    @classmethod
     def restore(cls, filename: str | Path) -> TurnoverJob:
         def ensure_list(key: str) -> None:
             if key in turnover_dict:
                 r = turnover_dict[key]
                 if isinstance(r, str):
                     turnover_dict[key] = [r]
 
@@ -159,23 +204,29 @@
             # just what we want...
 
             ensure_list("mzmlfiles")
             ensure_list("pepxml")
             if "job_name" not in turnover_dict:
                 raise TypeError("please specify a job_name")
             if "jobid" not in turnover_dict:
-                job_name = str(turnover_dict["job_name"])
-                turnover_dict["jobid"] = slugify(job_name)
+                turnover_dict["jobid"] = cls.safe_jobid(turnover_dict, filename)
+                turnover_dict["auto_generated_jobid"] = True
             if "mzmlprefix" in turnover_dict:
                 prefix = Path(turnover_dict.pop("mzmlprefix"))
                 turnover_dict["mzmlfiles"] = [
                     str(prefix.joinpath(m)) for m in turnover_dict["mzmlfiles"]
                 ]
             if "settings" in turnover_dict:
-                turnover_dict["settings"] = PeptideSettings(**turnover_dict["settings"])
+                settings = turnover_dict["settings"]
+                settingsd = {
+                    f.name: settings[f.name]
+                    for f in fields(PeptideSettings)
+                    if f.name in settings
+                }
+                turnover_dict["settings"] = PeptideSettings(**settingsd)
             else:
                 settingsd = {
                     f.name: turnover_dict[f.name]
                     for f in fields(PeptideSettings)
                     if f.name in turnover_dict
                 }
                 turnover_dict["settings"] = PeptideSettings(**settingsd)
```

### Comparing `protein_turnover-0.3.8/protein_turnover/logger.py` & `protein_turnover-0.4.0/protein_turnover/logger.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/mailer.py` & `protein_turnover-0.4.0/protein_turnover/mailer.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/parallel_utils.py` & `protein_turnover-0.4.0/protein_turnover/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/pepxml.py` & `protein_turnover-0.4.0/protein_turnover/pepxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,21 +391,22 @@
         )
 
 
 def pepxml_create(
     pepxml: PepXMLResourceFile,
     level: int = 0,
     number_of_bg_processes: int = 1,
-) -> None:
+) -> int:
     df = pepxml_raw(
         pepxml,
         level=level,
         number_of_bg_processes=number_of_bg_processes,
     )
-    return pepxml_out(df, pepxml)
+    pepxml_out(df, pepxml)
+    return level
 
 
 def dehydrate_pepxml(df: pd.DataFrame) -> pd.DataFrame:
     if "mzranges" in df.columns:
         df["mzranges"] = df["mzranges"].apply(lambda x: x.flatten())
     return df
```

### Comparing `protein_turnover-0.3.8/protein_turnover/pepxml_reader.py` & `protein_turnover-0.4.0/protein_turnover/pepxml_reader.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/plotting.py` & `protein_turnover-0.4.0/protein_turnover/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     else:
         eici = list(sorted(set(eici) & idx))
     if ax is None:
         fig = Figure(figsize=figsize if figsize else FIGSIZE)
         ax = fig.subplots(1, 1)
     for i in eici:
         ints = peptide.eics[i, :, 1]
-        fit, residues, rank, s = lstsq(im, ints)
+        fit, _residues, _rank, _s = lstsq(im, ints)
 
         y = fit[0] + fit[1] * x
         ax.scatter(intensity, ints, s=10)
         ax.plot(x, y)
     ax.set(
         title=f"{peptide.peptide} {peptide.modcol}",
         xlabel="mono intensity",
@@ -560,18 +560,18 @@
 
 
 # for use in jupyter notebooks....
 def plot_all_sidebyside(
     b: TurnoverRow,
     settings: PeptideSettings,
 ) -> tuple[Figure, Figure, Figure, Figure]:
-    f1, *axes = plot_eics_sidebyside(b)
-    f2, *axes = plot_fitted_sidebyside(b, settings)
-    f3, *axes = plot_labelled_sidebyside(b, settings)
-    f4, axes = plot_fit_arrays(b)
+    f1, *_axes = plot_eics_sidebyside(b)
+    f2, *_axes = plot_fitted_sidebyside(b, settings)
+    f3, *_axes = plot_labelled_sidebyside(b, settings)
+    f4, _axes = plot_fit_arrays(b)
     return f1, f2, f3, f4
 
 
 def to_image_url(fig: Figure, format: str = "png") -> str:
     out = BytesIO()
     fig.savefig(out, format=format)
     data = f"data:image/{format.lower()};base64,".encode("ascii") + b64encode(
```

### Comparing `protein_turnover-0.3.8/protein_turnover/protxml.py` & `protein_turnover-0.4.0/protein_turnover/protxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,18 +121,19 @@
         )
 
 
 def protxml_create(
     protxml: ProtXMLResourceFile,
     level: int = 0,
     number_of_bg_processes: int = 1,
-) -> None:
+) -> int:
     df = protxml_raw(
         protxml,
         level=level,
         number_of_bg_processes=number_of_bg_processes,
     )
-    return protxml_out(df, protxml)
+    protxml_out(df, protxml)
+    return level
 
 
 def dehydrate_protxml(df: pd.DataFrame) -> pd.DataFrame:
     return df
```

### Comparing `protein_turnover-0.3.8/protein_turnover/pymz.py` & `protein_turnover-0.4.0/protein_turnover/pymz.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import pandas as pd
 
 from .fitenvelopes import fitEnvelopes
 from .jobs import TurnoverJob
 from .logger import logger
 from .parallel_utils import Task
 from .types.pepxmltypes import PepXMLRunRowRT
+from .utils import BaseResourceFile
 from .utils import getsize
 from .utils import human
 from .utils import IO
 from .utils import MzMLResourceFile
 from .utils import MzMLResourceFileLocal
 from .utils import PeptideSettings
 from .utils import PepXMLResourceFile
@@ -271,15 +272,15 @@
 MAGIC_BYTES = np.array([MAGIC_NO], dtype=np.float32).tobytes()
 
 
 def mzml_create(
     mzml: MzMLResourceFile,
     level: int = 0,
     number_of_bg_processes: int = 1,
-) -> None:
+) -> int:
     """Create cache files for a mzML file"""
     from .broken_api import PyMzMLReader
     from .logger import log_iterator
 
     mzreader = PyMzMLReader(
         mzml.original,
         build_index_from_scratch=False,
@@ -335,14 +336,16 @@
 
     mzml_out(mzml, df)
 
     from .dinosaur.dinosaur import mzml_dinosaur
 
     mzml_dinosaur(mzml)
 
+    return level
+
 
 def mzml_out(
     mzml: MzMLResourceFile,
     df: pd.DataFrame,
 ) -> None:
     out = mzml.cache_mzml()
     IO(out, df).save_df()
@@ -380,15 +383,15 @@
     *,
     workers: int = 4,
     save_subset: bool = True,
     nspectra: int | None = None,
 ) -> None:
     from .pepxml import process_pep_prot, dehydrate_pepxml
     from .utils import human, rmfiles
-    from .config import EICS
+    from .exts import EICS
     from .parallel_utils import parallel_tasks
 
     start = datetime.now()
     pepxml_df = process_pep_prot(job)
 
     tasks = create_mz_tasks(pepxml_df, job, nspectra=nspectra)
     if logger.isEnabledFor(logging.INFO):
@@ -843,30 +846,32 @@
         logger.warning("no mzML files!")
         return
 
     files.ensure_directories()
 
     procs: list[
         tuple[
-            Callable[[Any, int, int], None],
+            Callable[[Any, int, int], int],
             MzMLResourceFile | PepXMLResourceFile | ProtXMLResourceFile,
         ]
     ] = []
 
     for pepxml in files.pepxmls:
         if force or not pepxml.cache_pepxml_ok():
             procs.append((pepxml_create, pepxml))
+
         else:
             logger.info(
                 'skipping creation of "%s" cache: %s',
                 pepxml.name,
                 pepxml.cache_pepxml().name,
             )
     if force or not files.protxml.cache_protxml_ok():
         procs.append((protxml_create, files.protxml))
+
     else:
         logger.info(
             'skipping creation of "%s" cache: %s',
             files.protxml.name,
             files.protxml.cache_protxml().name,
         )
     todo = (
@@ -878,21 +883,30 @@
     if skipped:
         for t in skipped:
             logger.info(
                 'skipping creation of "%s" cache: %s',
                 t.name,
                 t.cache_mzml().name,
             )
-
+    target: MzMLResourceFile | PepXMLResourceFile | ProtXMLResourceFile
     for target in todo:
         procs.append((mzml_create, target))
 
     if not procs:
         return
-    exe: list[Callable[[], None]] = [
-        partial(func, target, idx, len(procs))
-        for idx, (func, target) in enumerate(procs, start=1)
-    ]
+    cleanups: dict[int, BaseResourceFile] = {}
+    exe: list[Callable[[], int]] = []
+    for idx, (func, target) in enumerate(procs, start=1):
+        exe.append(partial(func, target, idx, len(procs)))
+        cleanups[idx] = target
 
     ntotal = len(exe)
-    for idx, _ in enumerate(parallel_result(exe, workers=workers), start=1):
-        logger.info("turnover_prepare task done: [%d/%d]", idx, ntotal)
+    try:
+        for ridx in parallel_result(exe, workers=workers):
+            logger.info("turnover_prepare task done: [%d/%d]", ridx, ntotal)
+            if ridx in cleanups:
+                del cleanups[ridx]
+
+    except KeyboardInterrupt:
+        for c in cleanups.values():
+            c.cleanup()
+        raise
```

### Comparing `protein_turnover-0.3.8/protein_turnover/pymz_ui.py` & `protein_turnover-0.4.0/protein_turnover/pymz_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .cli import pass_config
 from .jobs import slugify
 from .logger import logger
 from .settings import setting_options
 from .utils import PeptideSettings
 
 
-@cli.command(name="mzml-create", hidden=False)
+@cli.command(name="mzi-create", hidden=False)
 @click.option("--force", is_flag=True, help="force creation")
 @click.option(
     "-w",
     "--workers",
     type=int,
     help="number of background workers [default: half number of cpus]",
 )
@@ -32,15 +32,15 @@
 @click.argument("mzmlfiles", nargs=-1, type=IsFile)
 def mzml_create_cmd(
     mzmlfiles: tuple[str, ...],
     out: str | None,
     workers: int | None,
     force: bool = False,
 ) -> None:
-    """Create intensity/mz memory mapped files for mzML files"""
+    """Create mz/intensity memory mapped files for mzML files"""
 
     from functools import partial
     from os import cpu_count
 
     from .utils import MzMLResourceFileLocal
     from .parallel_utils import parallel_result
     from .pymz import mzml_create
@@ -57,15 +57,15 @@
     if not todo:
         return
     if out is not None:
         pout = Path(out)
         if not pout.exists():
             pout.mkdir(parents=True, exist_ok=True)
 
-    exe: list[Callable[[], None]] = []
+    exe: list[Callable[[], int]] = []
     for idx, target in enumerate(todo, start=1):
         exe.append(partial(mzml_create, target, idx, len(todo)))
 
     ntotal = len(exe)
 
     for idx, _ in enumerate(parallel_result(exe, workers=workers), start=1):
         logger.info("mzml prepare task done: [%d/%d]", idx, ntotal)
@@ -100,15 +100,15 @@
     default=0,
     help="accept keyboard interrupt as error. Value will be exit code",
     hidden=True,  # only useful to for background process: see runner.py
 )  # see runner.py
 @click.argument("job")
 @pass_config
 def turnover_job_run_cmd(
-    config: Config,
+    cfg: Config,
     job: str,
     force: bool = False,
     workers: int | None = None,
     nspectra: int | None = None,
     job_dir: str | None = None,
     interrupt_as_error: int = 0,
     no_email: bool = False,
@@ -157,137 +157,165 @@
 
     if cache_dir is not None:
         jobby = replace(jobby, cache_dir=cache_dir)
 
     pjobdir = Path(job_dir)
     pjobdir.mkdir(exist_ok=True, parents=True)
 
-    # send fitEnvelope warnings to a logfile
-    logfile = pjobdir / f"{jobby.jobid}.log"
-    level: str | int = "INFO" if not config.loglevel else logger.getEffectiveLevel()
+    # send fitEnvelope warnings to a logfile if running in background
+    logfile: str | Path | None
+    if cfg.logfile is None and interrupt_as_error > 0:
+        # this is a background job and no logfile has been specified
+        logfile = pjobdir / f"{jobby.jobid}.log"
+    else:
+        logfile = cfg.logfile
+    level: str | int = "INFO" if cfg.loglevel is None else logger.getEffectiveLevel()
     # only reinit if we haven't specified logfile
-    init_logger(level=level, logfile=logfile, reinit=not config.logfile)
+    init_logger(level=level, logfile=logfile, reinit=cfg.logfile is None)
 
     # lock the cache directories so we don't delete anything until results done
     # we assume the job dirctory is never deleted
     rf = jobby.to_resource_files()
+    results = ResultsResourceFile(
+        jobby.jobid,
+        job_dir,
+    )
     try:
         rf.ensure_directories()
         rf.lock(jobby.jobid)
         turnover_prepare(rf, force=force, workers=workers)
 
         turnover_run(
             jobby,
-            ResultsResourceFile(
-                jobby.jobid,
-                job_dir,
-            ),  # where to store stuff for this job
+            results,  # where to store stuff for this job
             workers=workers,
             nspectra=nspectra,
             save_subset=True,
         )
         # interrupt as_error != 0 means we are running as the
         # background job for the website.
         if interrupt_as_error:
             jobby = replace(jobby, status="finished")
             jobby.save(job_dir)  # save a copy of the job
     except Exception as e:
         logger.error("turnover %s failed. reason: %s", jobby.jobid, e)
+        results.cleanup()
         maybeemail('Protein Turnover Job "{job.job_name}" has <b>failed</b>!')
-
         raise e
     except KeyboardInterrupt as e:
+        results.cleanup()
         if interrupt_as_error:
             logger.error("turnover %s killed", jobby.jobid)
             raise SystemExit(interrupt_as_error) from e
         raise e
     finally:
         rf.unlock(jobby.jobid)
 
     maybeemail(MAIL_TEXT, INSPECT_URL)
 
 
-@cli.command(name="create")
+@cli.command(name="job")
 @click.option(
     "-o",
     "--out",
-    default=".",
-    show_default=True,
-    help="directory to write file to",
-    type=click.Path(dir_okay=True, file_okay=False),
+    help="filename to write file to",
+    type=click.Path(dir_okay=False, file_okay=True),
+)
+@click.option("-j", "--jobid", help="job id")
+@click.option("-n", "--name", help="job name")
+@click.option(
+    "-x",
+    "--no-check",
+    is_flag=True,
+    help="don't do any sanity checks on the files",
 )
-@click.option("--jobid", help="job id")
-@click.option("--name", help="job name")
 @click.argument("pepxml", type=IsFile)
 @click.argument("protxml", type=IsFile)
 @click.argument("mzmlfiles", nargs=-1, type=IsFile)
 @setting_options
 def turnover_job(
     pepxml: str,
     protxml: str,
     mzmlfiles: list[str],
+    no_check: bool,
     name: str | None,
     jobid: str | None,
     settings: PeptideSettings,
     out: str | None = None,
 ) -> None:
     """Create a turnover job file"""
     from .jobs import TurnoverJob, jobidkey
     from .pepxml import scan_spectra
     from .protxml import scan_proteins
     from .pymz import scan_mzml_spectra
 
-    missing = []
-    for f in [pepxml, protxml, *mzmlfiles]:
-        if not Path(f).exists():
-            missing.append(f)
-    if missing:
-        click.secho(f"These are not files: {', '.join(missing)}", fg="red", err=True)
-        raise click.Abort()
-
-    n = sum(1 for _ in scan_spectra(Path(pepxml)))
-    if n == 0:
-        raise click.BadParameter(
-            f"peptide XML {pepxml} has no spectra",
-            param_hint="pepxml",
-        )
-    mzmlfiles = list(set(mzmlfiles))
-    n = sum(1 for _ in scan_proteins(Path(protxml)))
-    if n == 0:
-        raise click.BadParameter(
-            f"protein XML {protxml} has no proteins",
-            param_hint="protxml",
-        )
-    failed = []
-    for mzml in mzmlfiles:
-        n = sum(1 for _ in scan_mzml_spectra(Path(mzml)))
+    if not no_check:
+        missing = []
+        for f in [pepxml, protxml, *mzmlfiles]:
+            if not Path(f).exists():
+                missing.append(f)
+        if missing:
+            click.secho(
+                f"These are not files: {', '.join(missing)}",
+                fg="red",
+                err=True,
+            )
+            raise click.Abort()
+
+        n = sum(1 for _ in scan_spectra(Path(pepxml)))
         if n == 0:
-            failed.append(mzml)
-    if failed:
-        raise click.BadParameter(
-            f'mzML "{ ", ".join(failed) }" has no spectra',
-            param_hint="mzmlfiles",
-        )
-    if not jobid and name:
-        jobid = slugify(name)
+            raise click.BadParameter(
+                f"peptide XML {pepxml} has no spectra",
+                param_hint="pepxml",
+            )
+        mzmlfiles = list(set(mzmlfiles))
+        n = sum(1 for _ in scan_proteins(Path(protxml)))
+        if n == 0:
+            raise click.BadParameter(
+                f"protein XML {protxml} has no proteins",
+                param_hint="protxml",
+            )
+        failed = []
+        for mzml in mzmlfiles:
+            n = sum(1 for _ in scan_mzml_spectra(Path(mzml)))
+            if n == 0:
+                failed.append(mzml)
+        if failed:
+            raise click.BadParameter(
+                f'mzML "{ ", ".join(failed) }" has no spectra',
+                param_hint="mzmlfiles",
+            )
+
+    if not jobid:
+        if name:
+            jobid = slugify(name)
+        if not jobid or len(jobid) < 4:
+            jobid = jobidkey(pepxml, protxml, mzmlfiles)
 
-    jobid = jobid if jobid else jobidkey(pepxml, protxml, mzmlfiles)
     job_name = name or jobid
 
+    if out is None:
+        filename = Path(f"{jobid}.toml")
+    else:
+        filename = Path(out)
+    if not filename.parent.exists():
+        filename.parent.mkdir(parents=True, exist_ok=True)
+
     job = TurnoverJob(
         job_name=job_name,
         pepxml=[pepxml],
         protxml=protxml,
         mzmlfiles=mzmlfiles,
-        cache_dir=out or ".",
+        cache_dir=str(filename.parent),
         jobid=jobid,
         settings=settings,
     )
-    jobfile = job.save(".", job_name)
-    click.secho(f"written job to {jobfile}", fg="yellow")
+
+    jobfile = job.save(filename.parent, filename.name)
+    click.secho(f'written job to "{jobfile}"', fg="yellow")
 
 
 @cli.command(name="prepare", hidden=True)
 @click.option(
     "-o",
     "--out",
     help="directory to write",
```

### Comparing `protein_turnover-0.3.8/protein_turnover/settings.py` & `protein_turnover-0.4.0/protein_turnover/settings.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/sns.py` & `protein_turnover-0.4.0/protein_turnover/sns.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/sqla/iso_peaks.py` & `protein_turnover-0.4.0/protein_turnover/sqla/iso_peaks.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/sqla/iso_peaks_ui.py` & `protein_turnover-0.4.0/protein_turnover/sqla/iso_peaks_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/sqla/model.py` & `protein_turnover-0.4.0/protein_turnover/sqla/model.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/sqla/query.py` & `protein_turnover-0.4.0/protein_turnover/sqla/query.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/sqla/utils.py` & `protein_turnover-0.4.0/protein_turnover/sqla/utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/types/checking.py` & `protein_turnover-0.4.0/protein_turnover/types/checking.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/types/mzmltypes.py` & `protein_turnover-0.4.0/protein_turnover/types/mzmltypes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/types/pepxmltypes.py` & `protein_turnover-0.4.0/protein_turnover/types/pepxmltypes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/types/turnovertype.py` & `protein_turnover-0.4.0/protein_turnover/types/turnovertype.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/unimod.py` & `protein_turnover-0.4.0/protein_turnover/unimod.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.8/protein_turnover/utils.py` & `protein_turnover-0.4.0/protein_turnover/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,36 +11,37 @@
 from typing import TypedDict
 
 import numpy as np
 import pandas as pd
 from scipy.fft import fft
 from scipy.fft import ifft
 
-from .config import DINOSAUR
-from .config import EICS
-from .config import MZMAP
-from .config import MZML
-from .config import PEPXML
-from .config import PROTXML
-from .config import RESULT_EXT
+from .exts import DINOSAUR
+from .exts import EICS
+from .exts import EXT
+from .exts import MZMAP
+from .exts import MZML
+from .exts import PEPXML
+from .exts import PROTXML
+from .exts import RESULT_EXT
 from .types.pepxmltypes import PepXMLRow
 from .types.pepxmltypes import PepXMLRunRow
 
 
 @dataclass
 class PeptideSettings:
     rtTolerance: float = 15.0  # seconds
     mzTolerance: float = 1e-5  # ppm
     labelledIsotopeNumber: int = 15
     labelledElement: str = "N"
     maximumLabelEnrichment: float = 0.95
     retentionTimeCorrection: Literal["UseInSample", "SimpleMedian"] = "SimpleMedian"
     useObservedMz: bool = False
     minProbabilityCutoff: float = 0.8
-    fdrMaximum: float = 0.0
+    # fdrMaximum: float = 0.0
     # psmFilters: Filter | None = None
 
     def hash(self) -> str:
         from hashlib import md5
 
         m = md5()
         for k, v in asdict(self).items():
@@ -404,14 +405,24 @@
 
         self._hash = self.get_hash()
         return self._hash
 
     def get_hash(self) -> str:
         return hash256(self.original)
 
+    def cleanup(self):
+        for pth in self.all_cache_files():
+            try:
+                pth.unlink(missing_ok=True)
+            except OSError:
+                pass
+
+    def all_cache_files(self) -> list[Path]:
+        return []
+
 
 class MzMLResourceFile(BaseResourceFile):
     @property
     def runName(self) -> str:
         """Name possibly in pep.xml file as <spectrum_query spectrum="{runName}.{start_scan}.{end_scan}.0 ...>"""
         return self.original.stem
 
@@ -447,14 +458,17 @@
     def touch(self) -> bool:
         if self.cache_ok():
             self.cache_memmap().touch()
             self.cache_mzml().touch()
             return True
         return False
 
+    def all_cache_files(self) -> list[Path]:
+        return [self.cache_mzml(), self.cache_memmap()]
+
 
 class MzMLResourceFileLocal(MzMLResourceFile):
     def __init__(
         self,
         original: Path | str,
         directory: Path | str | None = None,
         name: str | None = None,
@@ -465,24 +479,20 @@
         self.outname = name
 
     def cache_file(self, ext: str) -> Path:
         # return self.cache_dir.joinpath(self.name + ext)
         return self.cache_dir.joinpath(self.outname + ext)
 
     def cache_mzml(self) -> Path:
-        from .config import EXT
-
         return self.cache_file("." + EXT)
 
     def cache_memmap(self) -> Path:
         return self.cache_file(".mzi")
 
     def cache_mzml_ok(self) -> bool:
-        from .config import EXT
-
         return self.extok("." + EXT, ".mzi")
 
 
 class PepXMLResourceFile(BaseResourceFile):
     def cache_pepxml(self) -> Path:
         return self.cache_file(PEPXML)
 
@@ -494,14 +504,17 @@
 
     def touch(self) -> bool:
         if self.cache_ok():
             self.cache_pepxml().touch()
             return True
         return False
 
+    def all_cache_files(self) -> list[Path]:
+        return [self.cache_pepxml()]
+
 
 class ProtXMLResourceFile(BaseResourceFile):
     def cache_protxml(self) -> Path:
         return self.cache_file(PROTXML)
 
     def cache_protxml_ok(self) -> bool:
         return self.extok(PROTXML)
@@ -511,28 +524,37 @@
 
     def touch(self) -> bool:
         if self.cache_ok():
             self.cache_protxml().touch()
             return True
         return False
 
+    def all_cache_files(self) -> list[Path]:
+        return [self.cache_protxml()]
+
 
 class ResultsResourceFile(BaseResourceFile):
     def cache_result(self) -> Path:
         return self.cache_file(RESULT_EXT)
 
     def cache_pepxml(self) -> Path:
         return self.cache_file(PEPXML)
 
     def cache_envelope(self) -> Path:
         return self.cache_file(EICS)
 
     def cache_file(self, ext: str) -> Path:
         return self.cache_dir.joinpath(self.original.name + ext)
 
+    def all_cache_files(self) -> list[Path]:
+        return [self.cache_result(), self.cache_pepxml(), self.cache_envelope()]
+
+    def has_result(self) -> bool:
+        return self.cache_result().exists()
+
 
 class ResourceFiles:
     def __init__(
         self,
         pepxmls: list[PepXMLResourceFile],
         protxml: ProtXMLResourceFile,
         mzmlfiles: list[MzMLResourceFile],
```

### Comparing `protein_turnover-0.3.8/pyproject.toml` & `protein_turnover-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 [tool.poetry]
 name = "protein-turnover"
-version = "0.3.8"
+version = "0.4.0"
 description = "protein turnover pipeline"
 authors = ["Ian Castleden <ian.castleden@uwa.edu.au>"]
 license = "MIT"
 readme = "prerelease.md"
 exclude = ["oldcode/**", "tests/**"]
 packages = [{ include = "protein_turnover" }]
 repository = "https://github.com/arabidopsis/protein_turnover.git"
 
-classifiers =[
+classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3 :: Only",
-    "Topic :: Scientific/Engineering :: Bio-Informatics"
+    "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 pymzml = "^2.5.2"
 pyteomics = "^4.5.3"
 lxml = "^4.9.0"
 click = "^8.1.3"
-scipy = "^1.8.1"
+scipy = "^1.8.1"  # for fitting
 pandas = "^2.0.3"
-pyarrow = "^15.0.0"
-more-itertools = "^8.13.0"
+pyarrow = "^15.0.0" # for parquet
+more-itertools = "^8.13.0" # ichunked
 matplotlib = "^3.5.2"
 SQLAlchemy = "^2.0.20"
 tomli = "^2.0.1"
 tomli-w = "^1.0.0"
+unidecode = { version = "^1.3.8", optional = true }
+psutil = { version = "^5.0", optional = true }
 
 [tool.poetry.scripts]
 turnover = "protein_turnover.__main__:cli"
 
+[tool.poetry.extras]
+unidecode = ["unidecode"]
+psutil = ["psutil"]
+all = ["psutil", "unidecode"]
+
 [tool.poetry.group.dev.dependencies]
 mypy = ">=1.6.1"
 black = "^22.6.0"
 pre-commit = "^2.19.0"
 requests = "^2.28.1"
 
 [build-system]
```

### Comparing `protein_turnover-0.3.8/PKG-INFO` & `protein_turnover-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-turnover
-Version: 0.3.8
+Version: 0.4.0
 Summary: protein turnover pipeline
 Home-page: https://github.com/arabidopsis/protein_turnover.git
 License: MIT
 Author: Ian Castleden
 Author-email: ian.castleden@uwa.edu.au
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
@@ -12,26 +12,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Provides-Extra: all
+Provides-Extra: psutil
+Provides-Extra: unidecode
 Requires-Dist: SQLAlchemy (>=2.0.20,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: lxml (>=4.9.0,<5.0.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: more-itertools (>=8.13.0,<9.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: psutil (>=5.0,<6.0) ; extra == "psutil" or extra == "all"
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pymzml (>=2.5.2,<3.0.0)
 Requires-Dist: pyteomics (>=4.5.3,<5.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
+Requires-Dist: unidecode (>=1.3.8,<2.0.0) ; extra == "unidecode" or extra == "all"
 Project-URL: Repository, https://github.com/arabidopsis/protein_turnover.git
 Description-Content-Type: text/markdown
 
 # Protein Turnover Pipeline
 
 More documentation soon.
```

