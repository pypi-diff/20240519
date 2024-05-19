# Comparing `tmp/cs.ffmpegutils-20240316.1.tar.gz` & `tmp/cs.ffmpegutils-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.ffmpegutils-20240316.1.tar", last modified: Sat Mar 16 06:51:48 2024, max compression
+gzip compressed data, was "cs.ffmpegutils-20240519.tar", last modified: Sun May 19 02:32:26 2024, max compression
```

## Comparing `cs.ffmpegutils-20240316.1.tar` & `cs.ffmpegutils-20240519.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:51:48.544501 cs.ffmpegutils-20240316.1/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:51:42.000000 cs.ffmpegutils-20240316.1/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     3187 2024-03-16 06:51:48.544233 cs.ffmpegutils-20240316.1/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     3011 2024-03-16 06:51:44.000000 cs.ffmpegutils-20240316.1/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:51:48.540520 cs.ffmpegutils-20240316.1/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:51:48.540789 cs.ffmpegutils-20240316.1/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:51:48.541921 cs.ffmpegutils-20240316.1/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    12660 2024-03-16 06:51:25.000000 cs.ffmpegutils-20240316.1/lib/python/cs/ffmpegutils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:51:48.543820 cs.ffmpegutils-20240316.1/lib/python/cs.ffmpegutils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     3187 2024-03-16 06:51:47.000000 cs.ffmpegutils-20240316.1/lib/python/cs.ffmpegutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      361 2024-03-16 06:51:48.000000 cs.ffmpegutils-20240316.1/lib/python/cs.ffmpegutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:51:48.000000 cs.ffmpegutils-20240316.1/lib/python/cs.ffmpegutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       68 2024-03-16 06:51:48.000000 cs.ffmpegutils-20240316.1/lib/python/cs.ffmpegutils.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      188 2024-03-16 06:51:48.000000 cs.ffmpegutils-20240316.1/lib/python/cs.ffmpegutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:51:48.000000 cs.ffmpegutils-20240316.1/lib/python/cs.ffmpegutils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     3828 2024-03-16 06:51:46.000000 cs.ffmpegutils-20240316.1/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:51:48.544595 cs.ffmpegutils-20240316.1/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:32:26.297368 cs.ffmpegutils-20240519/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-19 02:32:19.000000 cs.ffmpegutils-20240519/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3878 2024-05-19 02:32:26.297083 cs.ffmpegutils-20240519/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3079 2024-05-19 02:32:21.000000 cs.ffmpegutils-20240519/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:32:26.292662 cs.ffmpegutils-20240519/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:32:26.293095 cs.ffmpegutils-20240519/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:32:26.294374 cs.ffmpegutils-20240519/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    12682 2024-05-19 02:32:05.000000 cs.ffmpegutils-20240519/lib/python/cs/ffmpegutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:32:26.296599 cs.ffmpegutils-20240519/lib/python/cs.ffmpegutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3878 2024-05-19 02:32:25.000000 cs.ffmpegutils-20240519/lib/python/cs.ffmpegutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      361 2024-05-19 02:32:26.000000 cs.ffmpegutils-20240519/lib/python/cs.ffmpegutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-19 02:32:25.000000 cs.ffmpegutils-20240519/lib/python/cs.ffmpegutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       68 2024-05-19 02:32:25.000000 cs.ffmpegutils-20240519/lib/python/cs.ffmpegutils.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      190 2024-05-19 02:32:26.000000 cs.ffmpegutils-20240519/lib/python/cs.ffmpegutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-19 02:32:26.000000 cs.ffmpegutils-20240519/lib/python/cs.ffmpegutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4521 2024-05-19 02:32:24.000000 cs.ffmpegutils-20240519/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-19 02:32:26.297475 cs.ffmpegutils-20240519/setup.cfg
```

### Comparing `cs.ffmpegutils-20240316.1/PKG-INFO` & `cs.ffmpegutils-20240519/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.ffmpegutils
-Version: 20240316.1
+Version: 20240519
 Summary: Convenience facilities for using FFmpeg (ffmpeg.org), with invocation via `ffmpeg-python`.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,57 +15,84 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Convenience facilities for using FFmpeg (ffmpeg.org),
 with invocation via `ffmpeg-python`.
 
-*Latest release 20240316.1*:
-DISTINFO fix.
+*Latest release 20240519*:
+ffmpeg_docker: set DockerRun.output_hostdir from the output file dirname.
 
 ## Class `ConversionSource(builtins.tuple)`
 
 ConversionSource(src, srcfmt, start_s, end_s)
 
-*Method `ConversionSource.__new__(_cls, src, srcfmt, start_s, end_s)`*:
-Create new instance of ConversionSource(src, srcfmt, start_s, end_s)
+*Property `ConversionSource.end_s`*:
+Alias for field number 3
+
+*Property `ConversionSource.src`*:
+Alias for field number 0
+
+*Property `ConversionSource.srcfmt`*:
+Alias for field number 1
+
+*Property `ConversionSource.start_s`*:
+Alias for field number 2
 
-## Function `convert(*srcs, dstpath: str, doit=True, dstfmt=None, ffmpeg_exe=None, fstags: cs.fstags.FSTags, conversions=None, metadata: Optional[dict] = None, timespans=(), overwrite=False, acodec=None, vcodec=None, extra_opts=None) -> List[str]`
+## Function `convert(*srcs, dstpath: str, doit=True, dstfmt=None, ffmpeg_exe=None, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x10bd092d0>, conversions=None, metadata: Optional[dict] = None, timespans=(), overwrite=False, acodec=None, vcodec=None, extra_opts=None) -> List[str]`
 
 Transcode video to `dstpath` in FFMPEG compatible `dstfmt`.
 
-## Function `ffmpeg_docker(*ffmpeg_args: Iterable[str], docker_run_opts: Union[List[str], Mapping, NoneType] = None, doit: Optional[bool] = None, quiet: Optional[bool] = None, ffmpeg_exe: Optional[str] = None, docker_exe: Optional[str] = None, image: Optional[str] = None, outputpath: str = '.') -> Optional[subprocess.CompletedProcess]`
+## Function `ffmpeg_docker(*ffmpeg_args: Iterable[str], docker_run_opts: Union[List[str], Mapping, NoneType] = None, doit: Optional[bool] = None, quiet: Optional[bool] = None, ffmpeg_exe: Optional[str] = None, docker_exe: Optional[str] = None, image: Optional[str] = None, output_hostdir: Optional[str] = None) -> Optional[subprocess.CompletedProcess]`
 
 Invoke `ffmpeg` using docker.
 
 ## Class `FFmpegSource`
 
 A representation of an `ffmpeg` input source.
 
+*Method `FFmpegSource.add_as_input(self, ff)`*:
+Add as an input to `ff`.
+Return `None` if `self.source` is a pathname,
+otherwise return the file descriptor of the data source.
+
+Note: because we rely on `ff.input('pipe:')` for nonpathnames,
+you can only use a nonpathname `FFmpegSource` for one of the inputs.
+This is not checked.
+
+*Method `FFmpegSource.promote(source)`*:
+Promote `source` to an `FFmpegSource`.
+
 ## Function `ffprobe(input_file, *, doit=True, ffprobe_exe='ffprobe', quiet=False)`
 
 Run `ffprobe -print_format json` on `input_file`,
 return format, stream, program and chapter information
 as an `AttrableMapping` (a `dict` subclass).
 
 ## Function `main_ffmpeg_docker(argv=None)`
 
 The `ffm[peg-docker` command line implementation.
 
-## Class `MetaData(cs.tagset.TagSet, builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin)`
+## Class `MetaData(cs.tagset.TagSet)`
 
 Object containing fields which may be supplied to ffmpeg's -metadata option.
 
 *Method `MetaData.__init__(self, format, **kw)`*:
 pylint: disable=redefined-builtin
 
+*Method `MetaData.options(self)`*:
+Compute the FFmpeg -metadata option strings and return as a list.
+
 # Release Log
 
 
 
+*Release 20240519*:
+ffmpeg_docker: set DockerRun.output_hostdir from the output file dirname.
+
 *Release 20240316.1*:
 DISTINFO fix.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
```

### Comparing `cs.ffmpegutils-20240316.1/README.md` & `cs.ffmpegutils-20240519/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Convenience facilities for using FFmpeg (ffmpeg.org),
 with invocation via `ffmpeg-python`.
 
-*Latest release 20240316.1*:
-DISTINFO fix.
+*Latest release 20240519*:
+ffmpeg_docker: set DockerRun.output_hostdir from the output file dirname.
 
 ## Class `ConversionSource(builtins.tuple)`
 
 ConversionSource(src, srcfmt, start_s, end_s)
 
 *Property `ConversionSource.end_s`*:
 Alias for field number 3
@@ -16,19 +16,19 @@
 
 *Property `ConversionSource.srcfmt`*:
 Alias for field number 1
 
 *Property `ConversionSource.start_s`*:
 Alias for field number 2
 
-## Function `convert(*srcs, dstpath: str, doit=True, dstfmt=None, ffmpeg_exe=None, fstags: cs.fstags.FSTags, conversions=None, metadata: Optional[dict] = None, timespans=(), overwrite=False, acodec=None, vcodec=None, extra_opts=None) -> List[str]`
+## Function `convert(*srcs, dstpath: str, doit=True, dstfmt=None, ffmpeg_exe=None, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x10bd092d0>, conversions=None, metadata: Optional[dict] = None, timespans=(), overwrite=False, acodec=None, vcodec=None, extra_opts=None) -> List[str]`
 
 Transcode video to `dstpath` in FFMPEG compatible `dstfmt`.
 
-## Function `ffmpeg_docker(*ffmpeg_args: Iterable[str], docker_run_opts: Union[List[str], Mapping, NoneType] = None, doit: Optional[bool] = None, quiet: Optional[bool] = None, ffmpeg_exe: Optional[str] = None, docker_exe: Optional[str] = None, image: Optional[str] = None, outputpath: str = '.') -> Optional[subprocess.CompletedProcess]`
+## Function `ffmpeg_docker(*ffmpeg_args: Iterable[str], docker_run_opts: Union[List[str], Mapping, NoneType] = None, doit: Optional[bool] = None, quiet: Optional[bool] = None, ffmpeg_exe: Optional[str] = None, docker_exe: Optional[str] = None, image: Optional[str] = None, output_hostdir: Optional[str] = None) -> Optional[subprocess.CompletedProcess]`
 
 Invoke `ffmpeg` using docker.
 
 ## Class `FFmpegSource`
 
 A representation of an `ffmpeg` input source.
 
@@ -50,28 +50,31 @@
 return format, stream, program and chapter information
 as an `AttrableMapping` (a `dict` subclass).
 
 ## Function `main_ffmpeg_docker(argv=None)`
 
 The `ffm[peg-docker` command line implementation.
 
-## Class `MetaData(cs.tagset.TagSet, builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin)`
+## Class `MetaData(cs.tagset.TagSet)`
 
 Object containing fields which may be supplied to ffmpeg's -metadata option.
 
 *Method `MetaData.__init__(self, format, **kw)`*:
 pylint: disable=redefined-builtin
 
 *Method `MetaData.options(self)`*:
 Compute the FFmpeg -metadata option strings and return as a list.
 
 # Release Log
 
 
 
+*Release 20240519*:
+ffmpeg_docker: set DockerRun.output_hostdir from the output file dirname.
+
 *Release 20240316.1*:
 DISTINFO fix.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
```

### Comparing `cs.ffmpegutils-20240316.1/lib/python/cs/ffmpegutils.py` & `cs.ffmpegutils-20240519/lib/python/cs/ffmpegutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 '''
 
 from collections import namedtuple
 from dataclasses import dataclass
 import json
 import os
 from os.path import (
+    dirname,
     isdir as isdirpath,
     isfile as isfilepath,
 )
 import shlex
 from subprocess import CompletedProcess
 import sys
 from typing import Any, Iterable, List, Mapping, Optional, Tuple, Union
@@ -30,15 +31,15 @@
 from cs.lex import cutprefix
 from cs.logutils import warning
 from cs.mappings import attrable
 from cs.pfx import Pfx, pfx, pfx_call
 from cs.psutils import pipefrom, print_argv
 from cs.tagset import TagSet
 
-__version__ = '20240316.1'
+__version__ = '20240519'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -345,28 +346,26 @@
     *ffmpeg_args: Iterable[str],
     docker_run_opts: Optional[Union[List[str], Mapping]] = None,
     doit: Optional[bool] = None,
     quiet: Optional[bool] = None,
     ffmpeg_exe: Optional[str] = None,
     docker_exe: Optional[str] = None,
     image: Optional[str] = None,
-    outputpath: str = '.',
+    output_hostdir: Optional[str] = None,
 ) -> Optional[CompletedProcess]:
   ''' Invoke `ffmpeg` using docker.
   '''
   ffmpeg_args: List[str] = list(ffmpeg_args)
   if docker_run_opts is None:
     docker_run_opts = []
   if ffmpeg_exe is None:
     ffmpeg_exe = FFMPEG_DOCKER_EXE_DEFAULT
   if image is None:
     image = FFMPEG_DOCKER_IMAGE_DEFAULT
-  if not isdirpath(outputpath):
-    raise ValueError(f'outputpath:{outputpath!r}: not a directory')
-  DR = DockerRun(image=image, outputpath=outputpath)
+  DR = DockerRun(image=image)
   DR.popopts(docker_run_opts)
   if docker_run_opts:
     raise ValueError(f'unparsed docker_run args: {docker_run_opts!r}')
   # parse ffmpeg options in order to extract the input and output files
   ffmpeg_argv = [ffmpeg_exe]
   while ffmpeg_args:
     arg = ffmpeg_args.pop(0)
@@ -378,14 +377,16 @@
         ffmpeg_argv.append(arg)
       elif not arg.startswith('-'):
         # output filename
         # TODO: URLs?
         outputpath = arg
         outputpath = cutprefix(outputpath, 'file:')
         ffmpeg_argv.append(DR.add_output(outputpath))
+        if output_hostdir is None:
+          output_hostdir = dirname(outputpath)
       elif arg == '-i':
         # an input filename
         # TODO: URLs?
         inputpath = ffmpeg_args.pop(0)
         inputpath = cutprefix(inputpath, 'file:')
         if inputpath == '-':
           # input from stdin
@@ -428,8 +429,9 @@
             'dn',  # Audio options
             'an',  # Subtitle options
             'sn',
         ):
           ffmpeg_argv.append(arg)
         else:
           ffmpeg_argv.extend([arg, ffmpeg_args.pop(0)])
+  DR.output_hostdir = output_hostdir
   return DR.run(*ffmpeg_argv, docker_exe=docker_exe, doit=doit, quiet=quiet)
```

### Comparing `cs.ffmpegutils-20240316.1/lib/python/cs.ffmpegutils.egg-info/PKG-INFO` & `cs.ffmpegutils-20240519/lib/python/cs.ffmpegutils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.ffmpegutils
-Version: 20240316.1
+Version: 20240519
 Summary: Convenience facilities for using FFmpeg (ffmpeg.org), with invocation via `ffmpeg-python`.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,57 +15,84 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Convenience facilities for using FFmpeg (ffmpeg.org),
 with invocation via `ffmpeg-python`.
 
-*Latest release 20240316.1*:
-DISTINFO fix.
+*Latest release 20240519*:
+ffmpeg_docker: set DockerRun.output_hostdir from the output file dirname.
 
 ## Class `ConversionSource(builtins.tuple)`
 
 ConversionSource(src, srcfmt, start_s, end_s)
 
-*Method `ConversionSource.__new__(_cls, src, srcfmt, start_s, end_s)`*:
-Create new instance of ConversionSource(src, srcfmt, start_s, end_s)
+*Property `ConversionSource.end_s`*:
+Alias for field number 3
+
+*Property `ConversionSource.src`*:
+Alias for field number 0
+
+*Property `ConversionSource.srcfmt`*:
+Alias for field number 1
+
+*Property `ConversionSource.start_s`*:
+Alias for field number 2
 
-## Function `convert(*srcs, dstpath: str, doit=True, dstfmt=None, ffmpeg_exe=None, fstags: cs.fstags.FSTags, conversions=None, metadata: Optional[dict] = None, timespans=(), overwrite=False, acodec=None, vcodec=None, extra_opts=None) -> List[str]`
+## Function `convert(*srcs, dstpath: str, doit=True, dstfmt=None, ffmpeg_exe=None, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x10bd092d0>, conversions=None, metadata: Optional[dict] = None, timespans=(), overwrite=False, acodec=None, vcodec=None, extra_opts=None) -> List[str]`
 
 Transcode video to `dstpath` in FFMPEG compatible `dstfmt`.
 
-## Function `ffmpeg_docker(*ffmpeg_args: Iterable[str], docker_run_opts: Union[List[str], Mapping, NoneType] = None, doit: Optional[bool] = None, quiet: Optional[bool] = None, ffmpeg_exe: Optional[str] = None, docker_exe: Optional[str] = None, image: Optional[str] = None, outputpath: str = '.') -> Optional[subprocess.CompletedProcess]`
+## Function `ffmpeg_docker(*ffmpeg_args: Iterable[str], docker_run_opts: Union[List[str], Mapping, NoneType] = None, doit: Optional[bool] = None, quiet: Optional[bool] = None, ffmpeg_exe: Optional[str] = None, docker_exe: Optional[str] = None, image: Optional[str] = None, output_hostdir: Optional[str] = None) -> Optional[subprocess.CompletedProcess]`
 
 Invoke `ffmpeg` using docker.
 
 ## Class `FFmpegSource`
 
 A representation of an `ffmpeg` input source.
 
+*Method `FFmpegSource.add_as_input(self, ff)`*:
+Add as an input to `ff`.
+Return `None` if `self.source` is a pathname,
+otherwise return the file descriptor of the data source.
+
+Note: because we rely on `ff.input('pipe:')` for nonpathnames,
+you can only use a nonpathname `FFmpegSource` for one of the inputs.
+This is not checked.
+
+*Method `FFmpegSource.promote(source)`*:
+Promote `source` to an `FFmpegSource`.
+
 ## Function `ffprobe(input_file, *, doit=True, ffprobe_exe='ffprobe', quiet=False)`
 
 Run `ffprobe -print_format json` on `input_file`,
 return format, stream, program and chapter information
 as an `AttrableMapping` (a `dict` subclass).
 
 ## Function `main_ffmpeg_docker(argv=None)`
 
 The `ffm[peg-docker` command line implementation.
 
-## Class `MetaData(cs.tagset.TagSet, builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin)`
+## Class `MetaData(cs.tagset.TagSet)`
 
 Object containing fields which may be supplied to ffmpeg's -metadata option.
 
 *Method `MetaData.__init__(self, format, **kw)`*:
 pylint: disable=redefined-builtin
 
+*Method `MetaData.options(self)`*:
+Compute the FFmpeg -metadata option strings and return as a list.
+
 # Release Log
 
 
 
+*Release 20240519*:
+ffmpeg_docker: set DockerRun.output_hostdir from the output file dirname.
+
 *Release 20240316.1*:
 DISTINFO fix.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
```

### Comparing `cs.ffmpegutils-20240316.1/pyproject.toml` & `cs.ffmpegutils-20240519/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 authors = [
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python3",
 ]
 dependencies = [
-    "cs.dockerutils>=20240305",
-    "cs.fstags>=20240316",
-    "cs.lex>=20240211",
+    "cs.dockerutils>=20240519",
+    "cs.fstags>=20240422",
+    "cs.lex>=20240519",
     "cs.logutils>=20230212",
     "cs.mappings>=20231129",
-    "cs.pfx>=20230604",
-    "cs.psutils>=20240211",
-    "cs.tagset>=20240316",
+    "cs.pfx>=20240412",
+    "cs.psutils>=20240316",
+    "cs.tagset>=20240422.2",
     "ffmpeg-python",
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
-version = "20240316.1"
+version = "20240519"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
@@ -40,57 +40,84 @@
 ffmpeg-docker = "cs.ffmpegutils:main_ffmpeg_docker"
 
 [project.readme]
 text = """
 Convenience facilities for using FFmpeg (ffmpeg.org),
 with invocation via `ffmpeg-python`.
 
-*Latest release 20240316.1*:
-DISTINFO fix.
+*Latest release 20240519*:
+ffmpeg_docker: set DockerRun.output_hostdir from the output file dirname.
 
 ## Class `ConversionSource(builtins.tuple)`
 
 ConversionSource(src, srcfmt, start_s, end_s)
 
-*Method `ConversionSource.__new__(_cls, src, srcfmt, start_s, end_s)`*:
-Create new instance of ConversionSource(src, srcfmt, start_s, end_s)
+*Property `ConversionSource.end_s`*:
+Alias for field number 3
+
+*Property `ConversionSource.src`*:
+Alias for field number 0
+
+*Property `ConversionSource.srcfmt`*:
+Alias for field number 1
+
+*Property `ConversionSource.start_s`*:
+Alias for field number 2
 
-## Function `convert(*srcs, dstpath: str, doit=True, dstfmt=None, ffmpeg_exe=None, fstags: cs.fstags.FSTags, conversions=None, metadata: Optional[dict] = None, timespans=(), overwrite=False, acodec=None, vcodec=None, extra_opts=None) -> List[str]`
+## Function `convert(*srcs, dstpath: str, doit=True, dstfmt=None, ffmpeg_exe=None, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x10bd092d0>, conversions=None, metadata: Optional[dict] = None, timespans=(), overwrite=False, acodec=None, vcodec=None, extra_opts=None) -> List[str]`
 
 Transcode video to `dstpath` in FFMPEG compatible `dstfmt`.
 
-## Function `ffmpeg_docker(*ffmpeg_args: Iterable[str], docker_run_opts: Union[List[str], Mapping, NoneType] = None, doit: Optional[bool] = None, quiet: Optional[bool] = None, ffmpeg_exe: Optional[str] = None, docker_exe: Optional[str] = None, image: Optional[str] = None, outputpath: str = '.') -> Optional[subprocess.CompletedProcess]`
+## Function `ffmpeg_docker(*ffmpeg_args: Iterable[str], docker_run_opts: Union[List[str], Mapping, NoneType] = None, doit: Optional[bool] = None, quiet: Optional[bool] = None, ffmpeg_exe: Optional[str] = None, docker_exe: Optional[str] = None, image: Optional[str] = None, output_hostdir: Optional[str] = None) -> Optional[subprocess.CompletedProcess]`
 
 Invoke `ffmpeg` using docker.
 
 ## Class `FFmpegSource`
 
 A representation of an `ffmpeg` input source.
 
+*Method `FFmpegSource.add_as_input(self, ff)`*:
+Add as an input to `ff`.
+Return `None` if `self.source` is a pathname,
+otherwise return the file descriptor of the data source.
+
+Note: because we rely on `ff.input('pipe:')` for nonpathnames,
+you can only use a nonpathname `FFmpegSource` for one of the inputs.
+This is not checked.
+
+*Method `FFmpegSource.promote(source)`*:
+Promote `source` to an `FFmpegSource`.
+
 ## Function `ffprobe(input_file, *, doit=True, ffprobe_exe='ffprobe', quiet=False)`
 
 Run `ffprobe -print_format json` on `input_file`,
 return format, stream, program and chapter information
 as an `AttrableMapping` (a `dict` subclass).
 
 ## Function `main_ffmpeg_docker(argv=None)`
 
 The `ffm[peg-docker` command line implementation.
 
-## Class `MetaData(cs.tagset.TagSet, builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin)`
+## Class `MetaData(cs.tagset.TagSet)`
 
 Object containing fields which may be supplied to ffmpeg's -metadata option.
 
 *Method `MetaData.__init__(self, format, **kw)`*:
 pylint: disable=redefined-builtin
 
+*Method `MetaData.options(self)`*:
+Compute the FFmpeg -metadata option strings and return as a list.
+
 # Release Log
 
 
 
+*Release 20240519*:
+ffmpeg_docker: set DockerRun.output_hostdir from the output file dirname.
+
 *Release 20240316.1*:
 DISTINFO fix.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
```

