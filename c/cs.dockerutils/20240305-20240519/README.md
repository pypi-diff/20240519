# Comparing `tmp/cs.dockerutils-20240305.tar.gz` & `tmp/cs.dockerutils-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.dockerutils-20240305.tar", last modified: Mon Mar  4 21:49:48 2024, max compression
+gzip compressed data, was "cs.dockerutils-20240519.tar", last modified: Sun May 19 02:30:30 2024, max compression
```

## Comparing `cs.dockerutils-20240305.tar` & `cs.dockerutils-20240519.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:49:48.607600 cs.dockerutils-20240305/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-04 21:49:36.000000 cs.dockerutils-20240305/MANIFEST.in
--rw-r--r--   0 cameron    (501) cameron    (502)     4971 2024-03-04 21:49:48.607135 cs.dockerutils-20240305/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     5994 2024-03-04 21:49:37.000000 cs.dockerutils-20240305/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:49:48.606589 cs.dockerutils-20240305/cs.dockerutils.egg-info/
--rw-r--r--   0 cameron    (501) cameron    (502)     4971 2024-03-04 21:49:48.000000 cs.dockerutils-20240305/cs.dockerutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      254 2024-03-04 21:49:48.000000 cs.dockerutils-20240305/cs.dockerutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-04 21:49:48.000000 cs.dockerutils-20240305/cs.dockerutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       93 2024-03-04 21:49:48.000000 cs.dockerutils-20240305/cs.dockerutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-03-04 21:49:48.000000 cs.dockerutils-20240305/cs.dockerutils.egg-info/top_level.txt
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:49:48.602210 cs.dockerutils-20240305/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:49:48.602356 cs.dockerutils-20240305/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:49:48.605681 cs.dockerutils-20240305/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    13845 2024-03-04 21:49:21.000000 cs.dockerutils-20240305/lib/python/cs/dockerutils.py
--rw-rw-r--   0 cameron    (501) cameron    (502)     5167 2024-03-04 21:49:39.000000 cs.dockerutils-20240305/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-04 21:49:48.607698 cs.dockerutils-20240305/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:30:30.072690 cs.dockerutils-20240519/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-19 02:30:24.000000 cs.dockerutils-20240519/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6761 2024-05-19 02:30:30.072369 cs.dockerutils-20240519/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6027 2024-05-19 02:30:25.000000 cs.dockerutils-20240519/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:30:30.067613 cs.dockerutils-20240519/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:30:30.067977 cs.dockerutils-20240519/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:30:30.069512 cs.dockerutils-20240519/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    13873 2024-05-19 02:30:11.000000 cs.dockerutils-20240519/lib/python/cs/dockerutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:30:30.071730 cs.dockerutils-20240519/lib/python/cs.dockerutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6761 2024-05-19 02:30:29.000000 cs.dockerutils-20240519/lib/python/cs.dockerutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      309 2024-05-19 02:30:30.000000 cs.dockerutils-20240519/lib/python/cs.dockerutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-19 02:30:29.000000 cs.dockerutils-20240519/lib/python/cs.dockerutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       91 2024-05-19 02:30:29.000000 cs.dockerutils-20240519/lib/python/cs.dockerutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-19 02:30:29.000000 cs.dockerutils-20240519/lib/python/cs.dockerutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7211 2024-05-19 02:30:28.000000 cs.dockerutils-20240519/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-19 02:30:30.072803 cs.dockerutils-20240519/setup.cfg
```

### Comparing `cs.dockerutils-20240305/PKG-INFO` & `cs.dockerutils-20240519/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,11 @@
-Metadata-Version: 2.1
-Name: cs.dockerutils
-Version: 20240305
-Summary: Docker related utilities.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python3
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-Requires-Dist: cs.cmdutils>=20240211
-Requires-Dist: cs.context>=20240212.1
-Requires-Dist: cs.pfx>=20230604
-Requires-Dist: cs.psutils>=20240211
-Requires-Dist: typeguard
-
 Docker related utilities.
 
-*Latest release 20240305*:
-DockerRun: new "network" attribute, default "none", for the --network CLI option.
+*Latest release 20240519*:
+DockerRun.outputpath: rename to output_hostdir, less confusing.
 
 ## Function `default_docker_command()`
 
 pylint: disable=unnecessary-lambda-assignment
 
 ## Function `default_docker_compose_command()`
 
@@ -65,19 +43,45 @@
 _Unlike_ a lot of docker setups, the default mode runs as the
 invoking user's UID/GID inside the container and expects the
 `s6-setuidgid` utility to be present in the image.
 
 See the `ffmpeg_docker` function from `cs.ffmpegutils` for
 an example invocation of this class.
 
+*Method `DockerRun.add_input(self, infspath: str) -> str`*:
+Add a host filesystem path to the `input_map`
+and return the corresponding container filesystem path.
+
+*Method `DockerRun.add_output(self, outfspath: str) -> str`*:
+Add a host filesystem path to the `output_map`
+and return the corresponding container filesystem path.
+
+*Method `DockerRun.popopts(self, argv: List[str]) -> None`*:
+Pop options from the list `argv`.
+
+The command's working directory will be /output.
+-i inputpath
+    Mount inputpath as /input/basename(inputpath)
+--root
+    Do not switch to the current effective uid:gid inside
+    the container.
+-U  Update the local copy of image before running.
+Other options are passed to "docker run".
+
+*Method `DockerRun.run(self, *argv, doit=None, quiet=None, docker_exe=None)`*:
+Run a command via `docker run`.
+Return the `CompletedProcess` result or `None` if `doit` is false.
+
 ## Class `DockerUtilCommand(cs.cmdutils.BaseCommand)`
 
 A command line mode for working with Docker et al.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: dockerutil [options...] [@container] subcommand...
         -f docker-compose.yml
           Specify ['docker', 'compose'] YAML file.
           Default: 'docker-compose.yml', overridden by $DK_COMPOSE_YML
         @container  Specify a target container.
 
@@ -100,15 +104,44 @@
               Do not switch to the current effective uid:gid inside
               the container.
           -U  Update the local copy of image before running.
           Other options are passed to "docker run".
         shell
           Run a command prompt via cmd.Cmd using this command's subcommands.
 
-## Class `DockerUtilCommandOptions(cs.cmdutils.BaseCommandOptions, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+*`DockerUtilCommand.Options`*
+
+*Method `DockerUtilCommand.apply_preargv(self, argv)`*:
+Consume a leading @container_name if present.
+
+*Method `DockerUtilCommand.cmd_ps(self, argv)`*:
+Usage: {cmd}
+Show the running docker containers.
+
+*Method `DockerUtilCommand.cmd_run(self, argv)`*:
+Usage: {cmd} [options] image [command] [arg...]
+Invoke command in an instance of image.
+A read only directory for input data will be present as /input.
+A read/write directory for output data will be present at /output.
+The command's working directory will be /output.
+-i inputpath
+    Mount inputpath as /input/basename(inputpath)
+--root
+    Do not switch to the current effective uid:gid inside
+    the container.
+-U  Update the local copy of image before running.
+Other options are passed to "docker run".
+
+*Method `DockerUtilCommand.docker(self, *dk_argv) -> subprocess.CompletedProcess`*:
+Invoke `docker`.
+
+*Method `DockerUtilCommand.docker_compose(self, *dc_argv) -> subprocess.CompletedProcess`*:
+Invoke `docker-compose`.
+
+## Class `DockerUtilCommandOptions(cs.cmdutils.BaseCommandOptions)`
 
 Command line options for `DockerUtilCommand`.
 
 ## Function `main(argv=None, **run_kw)`
 
 Invoke the `DockerUtilCommand` with `argv`.
 
@@ -125,14 +158,17 @@
 Rather that try to enumerate what needs escaping, here we use
 the `csv` module to escape using the default "excel" dialect.
 
 # Release Log
 
 
 
+*Release 20240519*:
+DockerRun.outputpath: rename to output_hostdir, less confusing.
+
 *Release 20240305*:
 DockerRun: new "network" attribute, default "none", for the --network CLI option.
 
 *Release 20240201*:
 * mount_escape: strip trailing carriage return also.
 * DockerRun: new output_map attribute much like input_map; also mount existing outputs within the container.
```

### Comparing `cs.dockerutils-20240305/README.md` & `cs.dockerutils-20240519/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,29 @@
+Metadata-Version: 2.1
+Name: cs.dockerutils
+Version: 20240519
+Summary: Docker related utilities.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 Docker related utilities.
 
-*Latest release 20240305*:
-DockerRun: new "network" attribute, default "none", for the --network CLI option.
+*Latest release 20240519*:
+DockerRun.outputpath: rename to output_hostdir, less confusing.
 
 ## Function `default_docker_command()`
 
 pylint: disable=unnecessary-lambda-assignment
 
 ## Function `default_docker_compose_command()`
 
@@ -71,15 +89,17 @@
 Run a command via `docker run`.
 Return the `CompletedProcess` result or `None` if `doit` is false.
 
 ## Class `DockerUtilCommand(cs.cmdutils.BaseCommand)`
 
 A command line mode for working with Docker et al.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: dockerutil [options...] [@container] subcommand...
         -f docker-compose.yml
           Specify ['docker', 'compose'] YAML file.
           Default: 'docker-compose.yml', overridden by $DK_COMPOSE_YML
         @container  Specify a target container.
 
@@ -131,15 +151,15 @@
 
 *Method `DockerUtilCommand.docker(self, *dk_argv) -> subprocess.CompletedProcess`*:
 Invoke `docker`.
 
 *Method `DockerUtilCommand.docker_compose(self, *dc_argv) -> subprocess.CompletedProcess`*:
 Invoke `docker-compose`.
 
-## Class `DockerUtilCommandOptions(cs.cmdutils.BaseCommandOptions, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `DockerUtilCommandOptions(cs.cmdutils.BaseCommandOptions)`
 
 Command line options for `DockerUtilCommand`.
 
 ## Function `main(argv=None, **run_kw)`
 
 Invoke the `DockerUtilCommand` with `argv`.
 
@@ -156,16 +176,20 @@
 Rather that try to enumerate what needs escaping, here we use
 the `csv` module to escape using the default "excel" dialect.
 
 # Release Log
 
 
 
+*Release 20240519*:
+DockerRun.outputpath: rename to output_hostdir, less confusing.
+
 *Release 20240305*:
 DockerRun: new "network" attribute, default "none", for the --network CLI option.
 
 *Release 20240201*:
 * mount_escape: strip trailing carriage return also.
 * DockerRun: new output_map attribute much like input_map; also mount existing outputs within the container.
 
 *Release 20231202*:
 Initial PyPI release.
+
```

### Comparing `cs.dockerutils-20240305/cs.dockerutils.egg-info/PKG-INFO` & `cs.dockerutils-20240519/lib/python/cs.dockerutils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: cs.dockerutils
-Version: 20240305
+Version: 20240519
 Summary: Docker related utilities.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
-Requires-Dist: cs.cmdutils>=20240211
-Requires-Dist: cs.context>=20240212.1
-Requires-Dist: cs.pfx>=20230604
-Requires-Dist: cs.psutils>=20240211
-Requires-Dist: typeguard
 
 Docker related utilities.
 
-*Latest release 20240305*:
-DockerRun: new "network" attribute, default "none", for the --network CLI option.
+*Latest release 20240519*:
+DockerRun.outputpath: rename to output_hostdir, less confusing.
 
 ## Function `default_docker_command()`
 
 pylint: disable=unnecessary-lambda-assignment
 
 ## Function `default_docker_compose_command()`
 
@@ -65,19 +61,45 @@
 _Unlike_ a lot of docker setups, the default mode runs as the
 invoking user's UID/GID inside the container and expects the
 `s6-setuidgid` utility to be present in the image.
 
 See the `ffmpeg_docker` function from `cs.ffmpegutils` for
 an example invocation of this class.
 
+*Method `DockerRun.add_input(self, infspath: str) -> str`*:
+Add a host filesystem path to the `input_map`
+and return the corresponding container filesystem path.
+
+*Method `DockerRun.add_output(self, outfspath: str) -> str`*:
+Add a host filesystem path to the `output_map`
+and return the corresponding container filesystem path.
+
+*Method `DockerRun.popopts(self, argv: List[str]) -> None`*:
+Pop options from the list `argv`.
+
+The command's working directory will be /output.
+-i inputpath
+    Mount inputpath as /input/basename(inputpath)
+--root
+    Do not switch to the current effective uid:gid inside
+    the container.
+-U  Update the local copy of image before running.
+Other options are passed to "docker run".
+
+*Method `DockerRun.run(self, *argv, doit=None, quiet=None, docker_exe=None)`*:
+Run a command via `docker run`.
+Return the `CompletedProcess` result or `None` if `doit` is false.
+
 ## Class `DockerUtilCommand(cs.cmdutils.BaseCommand)`
 
 A command line mode for working with Docker et al.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: dockerutil [options...] [@container] subcommand...
         -f docker-compose.yml
           Specify ['docker', 'compose'] YAML file.
           Default: 'docker-compose.yml', overridden by $DK_COMPOSE_YML
         @container  Specify a target container.
 
@@ -100,15 +122,44 @@
               Do not switch to the current effective uid:gid inside
               the container.
           -U  Update the local copy of image before running.
           Other options are passed to "docker run".
         shell
           Run a command prompt via cmd.Cmd using this command's subcommands.
 
-## Class `DockerUtilCommandOptions(cs.cmdutils.BaseCommandOptions, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+*`DockerUtilCommand.Options`*
+
+*Method `DockerUtilCommand.apply_preargv(self, argv)`*:
+Consume a leading @container_name if present.
+
+*Method `DockerUtilCommand.cmd_ps(self, argv)`*:
+Usage: {cmd}
+Show the running docker containers.
+
+*Method `DockerUtilCommand.cmd_run(self, argv)`*:
+Usage: {cmd} [options] image [command] [arg...]
+Invoke command in an instance of image.
+A read only directory for input data will be present as /input.
+A read/write directory for output data will be present at /output.
+The command's working directory will be /output.
+-i inputpath
+    Mount inputpath as /input/basename(inputpath)
+--root
+    Do not switch to the current effective uid:gid inside
+    the container.
+-U  Update the local copy of image before running.
+Other options are passed to "docker run".
+
+*Method `DockerUtilCommand.docker(self, *dk_argv) -> subprocess.CompletedProcess`*:
+Invoke `docker`.
+
+*Method `DockerUtilCommand.docker_compose(self, *dc_argv) -> subprocess.CompletedProcess`*:
+Invoke `docker-compose`.
+
+## Class `DockerUtilCommandOptions(cs.cmdutils.BaseCommandOptions)`
 
 Command line options for `DockerUtilCommand`.
 
 ## Function `main(argv=None, **run_kw)`
 
 Invoke the `DockerUtilCommand` with `argv`.
 
@@ -125,16 +176,20 @@
 Rather that try to enumerate what needs escaping, here we use
 the `csv` module to escape using the default "excel" dialect.
 
 # Release Log
 
 
 
+*Release 20240519*:
+DockerRun.outputpath: rename to output_hostdir, less confusing.
+
 *Release 20240305*:
 DockerRun: new "network" attribute, default "none", for the --network CLI option.
 
 *Release 20240201*:
 * mount_escape: strip trailing carriage return also.
 * DockerRun: new output_map attribute much like input_map; also mount existing outputs within the container.
 
 *Release 20231202*:
 Initial PyPI release.
+
```

### Comparing `cs.dockerutils-20240305/lib/python/cs/dockerutils.py` & `cs.dockerutils-20240519/lib/python/cs/dockerutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from typeguard import typechecked
 
 from cs.cmdutils import BaseCommand, BaseCommandOptions
 from cs.context import stackattrs
 from cs.pfx import Pfx, pfx, pfx_method
 from cs.psutils import run
 
-__version__ = '20240305'
+__version__ = '20240519'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -244,15 +244,15 @@
   OUTPUTDIR_DEFAULT = '/output'
   image: str = None
   network: str = 'none'
   options: List[str] = field(default_factory=list)
   input_root: str = INPUTDIR_DEFAULT
   input_map: dict = field(default_factory=dict)
   output_root: str = OUTPUTDIR_DEFAULT
-  outputpath: str = '.'
+  output_hostdir: str = '.'
   output_map: dict = field(default_factory=dict)
   as_root: bool = False
   pull_mode: str = 'missing'
 
   @typechecked
   def popopts(self, argv: List[str]) -> None:
     ''' Pop options from the list `argv`.
@@ -373,19 +373,19 @@
       if self.input_root != normpath(self.input_root):
         raise ValueError('not normalised')
     with Pfx("output_root:%r", self.output_root):
       if not isabspath(self.output_root):
         raise ValueError('not an absolute path')
       if self.output_root != normpath(self.output_root):
         raise ValueError('not normalised')
-    with Pfx("outputpath:%r", self.outputpath):
+    with Pfx("output_hostdir:%r", self.output_hostdir):
       # output mount point
-      if not self.outputpath:
-        self.outputpath = '.'
-      if not isdirpath(self.outputpath):
+      if not self.output_hostdir:
+        self.output_hostdir = '.'
+      if not isdirpath(self.output_hostdir):
         raise ValueError('not a directory')
     docker_argv = [
         docker_exe,
         'run',
         '--rm',
         ('--network', self.network),
         '-w',
@@ -409,15 +409,15 @@
         )
     # mount the output directory
     docker_argv.extend(
         [
             '--mount',
             mount_escape(
                 'type=bind',
-                f'source={abspath(self.outputpath)}',
+                f'source={abspath(self.output_hostdir)}',
                 f'destination={self.output_root}',
             ),
         ]
     )
     # if any named outputs exist, mount them inside /output
     for outbase, outfspath in self.output_map.items():
       if not existspath(outfspath):
```

### Comparing `cs.dockerutils-20240305/pyproject.toml` & `cs.dockerutils-20240519/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 authors = [
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python3",
 ]
 dependencies = [
-    "cs.cmdutils>=20240211",
-    "cs.context>=20240212.1",
-    "cs.pfx>=20230604",
-    "cs.psutils>=20240211",
+    "cs.cmdutils>=20240519",
+    "cs.context>=20240412",
+    "cs.pfx>=20240412",
+    "cs.psutils>=20240316",
     "typeguard",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240305"
+version = "20240519"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Docker related utilities.
 
-*Latest release 20240305*:
-DockerRun: new \"network\" attribute, default \"none\", for the --network CLI option.
+*Latest release 20240519*:
+DockerRun.outputpath: rename to output_hostdir, less confusing.
 
 ## Function `default_docker_command()`
 
 pylint: disable=unnecessary-lambda-assignment
 
 ## Function `default_docker_compose_command()`
 
@@ -78,19 +78,45 @@
 _Unlike_ a lot of docker setups, the default mode runs as the
 invoking user's UID/GID inside the container and expects the
 `s6-setuidgid` utility to be present in the image.
 
 See the `ffmpeg_docker` function from `cs.ffmpegutils` for
 an example invocation of this class.
 
+*Method `DockerRun.add_input(self, infspath: str) -> str`*:
+Add a host filesystem path to the `input_map`
+and return the corresponding container filesystem path.
+
+*Method `DockerRun.add_output(self, outfspath: str) -> str`*:
+Add a host filesystem path to the `output_map`
+and return the corresponding container filesystem path.
+
+*Method `DockerRun.popopts(self, argv: List[str]) -> None`*:
+Pop options from the list `argv`.
+
+The command's working directory will be /output.
+-i inputpath
+    Mount inputpath as /input/basename(inputpath)
+--root
+    Do not switch to the current effective uid:gid inside
+    the container.
+-U  Update the local copy of image before running.
+Other options are passed to \"docker run\".
+
+*Method `DockerRun.run(self, *argv, doit=None, quiet=None, docker_exe=None)`*:
+Run a command via `docker run`.
+Return the `CompletedProcess` result or `None` if `doit` is false.
+
 ## Class `DockerUtilCommand(cs.cmdutils.BaseCommand)`
 
 A command line mode for working with Docker et al.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: dockerutil [options...] [@container] subcommand...
         -f docker-compose.yml
           Specify ['docker', 'compose'] YAML file.
           Default: 'docker-compose.yml', overridden by $DK_COMPOSE_YML
         @container  Specify a target container.
 
@@ -113,15 +139,44 @@
               Do not switch to the current effective uid:gid inside
               the container.
           -U  Update the local copy of image before running.
           Other options are passed to \"docker run\".
         shell
           Run a command prompt via cmd.Cmd using this command's subcommands.
 
-## Class `DockerUtilCommandOptions(cs.cmdutils.BaseCommandOptions, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+*`DockerUtilCommand.Options`*
+
+*Method `DockerUtilCommand.apply_preargv(self, argv)`*:
+Consume a leading @container_name if present.
+
+*Method `DockerUtilCommand.cmd_ps(self, argv)`*:
+Usage: {cmd}
+Show the running docker containers.
+
+*Method `DockerUtilCommand.cmd_run(self, argv)`*:
+Usage: {cmd} [options] image [command] [arg...]
+Invoke command in an instance of image.
+A read only directory for input data will be present as /input.
+A read/write directory for output data will be present at /output.
+The command's working directory will be /output.
+-i inputpath
+    Mount inputpath as /input/basename(inputpath)
+--root
+    Do not switch to the current effective uid:gid inside
+    the container.
+-U  Update the local copy of image before running.
+Other options are passed to \"docker run\".
+
+*Method `DockerUtilCommand.docker(self, *dk_argv) -> subprocess.CompletedProcess`*:
+Invoke `docker`.
+
+*Method `DockerUtilCommand.docker_compose(self, *dc_argv) -> subprocess.CompletedProcess`*:
+Invoke `docker-compose`.
+
+## Class `DockerUtilCommandOptions(cs.cmdutils.BaseCommandOptions)`
 
 Command line options for `DockerUtilCommand`.
 
 ## Function `main(argv=None, **run_kw)`
 
 Invoke the `DockerUtilCommand` with `argv`.
 
@@ -138,14 +193,17 @@
 Rather that try to enumerate what needs escaping, here we use
 the `csv` module to escape using the default \"excel\" dialect.
 
 # Release Log
 
 
 
+*Release 20240519*:
+DockerRun.outputpath: rename to output_hostdir, less confusing.
+
 *Release 20240305*:
 DockerRun: new \"network\" attribute, default \"none\", for the --network CLI option.
 
 *Release 20240201*:
 * mount_escape: strip trailing carriage return also.
 * DockerRun: new output_map attribute much like input_map; also mount existing outputs within the container.
 
@@ -156,7 +214,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
     "setuptools >= 61.2",
     "trove-classifiers",
     "wheel",
 ]
+
+[tool.setuptools]
+py-modules = [
+    "cs.dockerutils",
+]
+
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

