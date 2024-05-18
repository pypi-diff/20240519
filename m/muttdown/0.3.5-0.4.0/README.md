# Comparing `tmp/muttdown-0.3.5.tar.gz` & `tmp/muttdown-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/muttdown-0.3.5.tar", last modified: Wed Sep 16 18:41:49 2020, max compression
+gzip compressed data, was "muttdown-0.4.0.tar", last modified: Sat May 18 23:15:03 2024, max compression
```

## Comparing `muttdown-0.3.5.tar` & `muttdown-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2020-09-16 18:41:49.105633 muttdown-0.3.5/
--rw-r--r--   0 jbrown     (501) staff       (20)      803 2020-09-16 18:25:42.000000 muttdown-0.3.5/CHANGES.md
--rw-r--r--   0 jbrown     (501) staff       (20)      757 2020-09-16 18:20:39.000000 muttdown-0.3.5/LICENSE.txt
--rw-r--r--   0 jbrown     (501) staff       (20)       27 2020-09-16 18:20:39.000000 muttdown-0.3.5/MANIFEST.in
--rw-r--r--   0 jbrown     (501) staff       (20)     4801 2020-09-16 18:41:49.105801 muttdown-0.3.5/PKG-INFO
--rw-r--r--   0 jbrown     (501) staff       (20)     3243 2020-09-16 18:25:42.000000 muttdown-0.3.5/README.md
-drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2020-09-16 18:41:49.103730 muttdown-0.3.5/muttdown/
--rw-r--r--   0 jbrown     (501) staff       (20)      122 2020-09-16 18:21:17.000000 muttdown-0.3.5/muttdown/__init__.py
--rw-r--r--   0 jbrown     (501) staff       (20)       62 2020-09-16 18:20:39.000000 muttdown-0.3.5/muttdown/__main__.py
--rw-r--r--   0 jbrown     (501) staff       (20)     3417 2020-09-16 18:20:39.000000 muttdown-0.3.5/muttdown/config.py
--rw-r--r--   0 jbrown     (501) staff       (20)       99 2020-09-16 18:20:39.000000 muttdown-0.3.5/muttdown/debug.py
--rw-r--r--   0 jbrown     (501) staff       (20)     7320 2020-09-16 18:20:39.000000 muttdown-0.3.5/muttdown/main.py
-drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2020-09-16 18:41:49.105385 muttdown-0.3.5/muttdown.egg-info/
--rw-r--r--   0 jbrown     (501) staff       (20)     4801 2020-09-16 18:41:49.000000 muttdown-0.3.5/muttdown.egg-info/PKG-INFO
--rw-r--r--   0 jbrown     (501) staff       (20)      376 2020-09-16 18:41:49.000000 muttdown-0.3.5/muttdown.egg-info/SOURCES.txt
--rw-r--r--   0 jbrown     (501) staff       (20)        1 2020-09-16 18:41:49.000000 muttdown-0.3.5/muttdown.egg-info/dependency_links.txt
--rw-r--r--   0 jbrown     (501) staff       (20)       49 2020-09-16 18:41:49.000000 muttdown-0.3.5/muttdown.egg-info/entry_points.txt
--rw-r--r--   0 jbrown     (501) staff       (20)       46 2020-09-16 18:41:49.000000 muttdown-0.3.5/muttdown.egg-info/requires.txt
--rw-r--r--   0 jbrown     (501) staff       (20)        9 2020-09-16 18:41:49.000000 muttdown-0.3.5/muttdown.egg-info/top_level.txt
--rw-r--r--   0 jbrown     (501) staff       (20)       52 2020-09-16 18:20:39.000000 muttdown-0.3.5/requirements-tests.txt
--rw-r--r--   0 jbrown     (501) staff       (20)       70 2020-09-16 18:41:49.106345 muttdown-0.3.5/setup.cfg
--rw-r--r--   0 jbrown     (501) staff       (20)     1371 2020-09-16 18:25:42.000000 muttdown-0.3.5/setup.py
+drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2024-05-18 23:15:03.544899 muttdown-0.4.0/
+-rw-r--r--   0 jbrown     (501) staff       (20)      979 2024-05-18 23:14:09.000000 muttdown-0.4.0/CHANGES.md
+-rw-r--r--   0 jbrown     (501) staff       (20)      762 2024-05-18 23:14:26.000000 muttdown-0.4.0/LICENSE.txt
+-rw-r--r--   0 jbrown     (501) staff       (20)       27 2024-05-18 22:47:08.000000 muttdown-0.4.0/MANIFEST.in
+-rw-r--r--   0 jbrown     (501) staff       (20)     4488 2024-05-18 23:15:03.544826 muttdown-0.4.0/PKG-INFO
+-rw-r--r--   0 jbrown     (501) staff       (20)     3408 2024-05-18 23:13:33.000000 muttdown-0.4.0/README.md
+drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2024-05-18 23:15:03.543422 muttdown-0.4.0/muttdown/
+-rw-r--r--   0 jbrown     (501) staff       (20)      122 2024-05-18 23:13:33.000000 muttdown-0.4.0/muttdown/__init__.py
+-rw-r--r--   0 jbrown     (501) staff       (20)       61 2024-05-18 23:13:33.000000 muttdown-0.4.0/muttdown/__main__.py
+-rw-r--r--   0 jbrown     (501) staff       (20)     3292 2024-05-18 23:13:33.000000 muttdown-0.4.0/muttdown/config.py
+-rw-r--r--   0 jbrown     (501) staff       (20)       98 2024-05-18 23:13:33.000000 muttdown-0.4.0/muttdown/debug.py
+-rw-r--r--   0 jbrown     (501) staff       (20)     7551 2024-05-18 23:13:33.000000 muttdown-0.4.0/muttdown/main.py
+drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2024-05-18 23:15:03.544576 muttdown-0.4.0/muttdown.egg-info/
+-rw-r--r--   0 jbrown     (501) staff       (20)     4488 2024-05-18 23:15:03.000000 muttdown-0.4.0/muttdown.egg-info/PKG-INFO
+-rw-r--r--   0 jbrown     (501) staff       (20)      417 2024-05-18 23:15:03.000000 muttdown-0.4.0/muttdown.egg-info/SOURCES.txt
+-rw-r--r--   0 jbrown     (501) staff       (20)        1 2024-05-18 23:15:03.000000 muttdown-0.4.0/muttdown.egg-info/dependency_links.txt
+-rw-r--r--   0 jbrown     (501) staff       (20)       48 2024-05-18 23:15:03.000000 muttdown-0.4.0/muttdown.egg-info/entry_points.txt
+-rw-r--r--   0 jbrown     (501) staff       (20)       51 2024-05-18 23:15:03.000000 muttdown-0.4.0/muttdown.egg-info/requires.txt
+-rw-r--r--   0 jbrown     (501) staff       (20)        9 2024-05-18 23:15:03.000000 muttdown-0.4.0/muttdown.egg-info/top_level.txt
+-rw-r--r--   0 jbrown     (501) staff       (20)       45 2024-05-18 23:13:33.000000 muttdown-0.4.0/requirements-tests.txt
+-rw-r--r--   0 jbrown     (501) staff       (20)       70 2024-05-18 23:15:03.545101 muttdown-0.4.0/setup.cfg
+-rw-r--r--   0 jbrown     (501) staff       (20)     1440 2024-05-18 23:14:46.000000 muttdown-0.4.0/setup.py
+drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2024-05-18 23:15:03.544422 muttdown-0.4.0/tests/
+-rw-r--r--   0 jbrown     (501) staff       (20)    11814 2024-05-18 23:13:33.000000 muttdown-0.4.0/tests/test_basic.py
+-rw-r--r--   0 jbrown     (501) staff       (20)      859 2024-05-18 23:13:33.000000 muttdown-0.4.0/tests/test_config.py
```

### Comparing `muttdown-0.3.5/CHANGES.md` & `muttdown-0.4.0/CHANGES.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.4.0
+=====
+- Drop support for Python <3.6
+- Switch to github actions for CI
+- Reformat entire project with `black` and add `pre-commit`
+- Add `assume_markdown` config option
+
 0.3.5
 =====
 - Fix some unicode handling (including, hopefully, fixing non-ASCII subject lines for real)
 - Drops support for Python 3.3 and Python 3.4 since we depend on libraries that have dropped support for them
 - Add support for Python 3.7 and Python 3.8
 
 0.3.4
```

### Comparing `muttdown-0.3.5/LICENSE.txt` & `muttdown-0.4.0/LICENSE.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2015-2018 James Brown <Roguelazer@gmail.com>
+Copyright (c) 2015-2024 James Brown <roguelazer@roguelazer.com>
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted, provided that the above
 copyright notice and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
```

### Comparing `muttdown-0.3.5/PKG-INFO` & `muttdown-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,116 @@
 Metadata-Version: 2.1
 Name: muttdown
-Version: 0.3.5
+Version: 0.4.0
 Summary: Sendmail replacement that compiles markdown into HTML
 Home-page: https://github.com/Roguelazer/muttdown
 Author: James Brown
-Author-email: Roguelazer@gmail.com
+Author-email: roguelazer@roguelazer.com
 License: ISC
-Description: muttdown
-        ========
-        
-        [![Build Status](https://travis-ci.com/Roguelazer/muttdown.svg?branch=master)](https://travis-ci.com/Roguelazer/muttdown)
-        
-        `muttdown` is a sendmail-replacement designed for use with the [mutt][] email client which will transparently compile annotated `text/plain` mail into `text/html` using the [Markdown][] standard.  It will recursively walk the MIME tree and compile any `text/plain` or `text/markdown` part which begins with the sigil "!m" into Markdown, which it will insert alongside the original in a multipart/alternative container.
-        
-        It's also smart enough not to break `multipart/signed`.
-        
-        For example, the following tree before parsing:
-        
-            - multipart/mixed
-             |
-             -- multipart/signed
-             |
-             ---- text/markdown
-             |
-             ---- application/pgp-signature
-             |
-             -- image/png
-        
-        Will get compiled into
-        
-            - multipart/mixed
-             |
-             -- multipart/alternative
-             |
-             ---- text/html
-             |
-             ---- multipart/signed
-             |
-             ------ text/markdown
-             |
-             ------ application/pgp-signature
-             |
-             -- image/png
-        
-        
-        Configuration
-        -------------
-        Muttdown's configuration file is written using [YAML][]. Example:
-        
-            smtp_host: smtp.gmail.com
-            smtp_port: 587
-            smtp_ssl: false
-            smtp_username: foo@bar.com
-            smtp_password: foo
-            css_file: ~/.muttdown.css
-        
-        
-        If you prefer not to put your password in plaintext in a configuration file, you can instead specify the `smtp_password_command` parameter to invoke a shell command to lookup your password. The command should output your password, followed by a newline, and no other text. On OS X, the following invocation will extract a generic "Password" entry with the application set to "mutt" and the title set to "foo@bar.com":
-        
-            smtp_password_command: security find-generic-password -w -s mutt -a foo@bar.com
-        
-        NOTE: If `smtp_ssl` is set to False, `muttdown` will do a non-SSL session and then invoke `STARTTLS`. If `smtp_ssl` is set to True, `muttdown` will do an SSL session from the get-go. There is no option to send mail in plaintext.
-        
-        The `css_file` should be regular CSS styling blocks; we use [pynliner][] to inline all CSS rules for maximum client compatibility.
-        
-        Muttdown can also send its mail using the native `sendmail` if you have that set up (instead of doing SMTP itself). To do so, just leave the smtp options in the config file blank, set the `sendmail` option to the fully-qualified path to your `sendmail` binary, and run muttdown with the `-s` flag
-        
-        Installation
-        ------------
-        Install muttdown with `pip install muttdown` or by downloading this package and running `python setup.py install`. You will need the [PyYAML][] and [Python-Markdown][] libraries, as specified in `requirements.txt`. This should work with Python 2.7 or Python 3.5+.
-        
-        Usage
-        -----
-        Invoke as
-        
-            muttdown -c /path/to/config -f "from_address" -- "to_address" [more to addresses...]
-        
-        Send a RFC822 formatted mail on stdin.
-        
-        If the config path is not passed, it will assume `~/.muttdown.yaml`.
-        
-        
-        
-        
-        [Markdown]: http://daringfireball.net/projects/markdown/
-        [YAML]: http://yaml.org
-        [PyYAML]: http://pyyaml.org
-        [Python-Markdown]: https://pypi.python.org/pypi/Markdown
-        [mutt]: http://www.mutt.org
-        [pynliner]: https://github.com/rennat/pynliner
-        
 Keywords: email
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Topic :: Communications :: Email
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: Markdown<4.0,>=3.0
+Requires-Dist: PyYAML>=3.0
+Requires-Dist: pynliner==0.8.0
+Requires-Dist: six
+
+muttdown
+========
+
+[![Build Status](https://github.com/Roguelazer/muttdown/actions/workflows/ci.yml/badge.svg)](https://github.com/Roguelazer/muttdown/actions/workflows/ci.yml)
+
+`muttdown` is a sendmail-replacement designed for use with the [mutt][] email client which will transparently compile annotated `text/plain` mail into `text/html` using the [Markdown][] standard.  It will recursively walk the MIME tree and compile any `text/plain` or `text/markdown` part which begins with the sigil "!m" into Markdown, which it will insert alongside the original in a multipart/alternative container.
+
+It's also smart enough not to break `multipart/signed`.
+
+For example, the following tree before parsing:
+
+    - multipart/mixed
+     |
+     -- multipart/signed
+     |
+     ---- text/markdown
+     |
+     ---- application/pgp-signature
+     |
+     -- image/png
+
+Will get compiled into
+
+    - multipart/mixed
+     |
+     -- multipart/alternative
+     |
+     ---- text/html
+     |
+     ---- multipart/signed
+     |
+     ------ text/markdown
+     |
+     ------ application/pgp-signature
+     |
+     -- image/png
+
+
+Configuration
+-------------
+Muttdown's configuration file is written using [YAML][]. Example:
+
+    smtp_host: smtp.gmail.com
+    smtp_port: 587
+    smtp_ssl: false
+    smtp_username: foo@bar.com
+    smtp_password: foo
+    css_file: ~/.muttdown.css
+    assume_markdown: false
+
+
+If you prefer not to put your password in plaintext in a configuration file, you can instead specify the `smtp_password_command` parameter to invoke a shell command to lookup your password. The command should output your password, followed by a newline, and no other text. On OS X, the following invocation will extract a generic "Password" entry with the application set to "mutt" and the title set to "foo@bar.com":
+
+    smtp_password_command: security find-generic-password -w -s mutt -a foo@bar.com
+
+NOTE: If `smtp_ssl` is set to False, `muttdown` will do a non-SSL session and then invoke `STARTTLS`. If `smtp_ssl` is set to True, `muttdown` will do an SSL session from the get-go. There is no option to send mail in plaintext.
+
+The `css_file` should be regular CSS styling blocks; we use [pynliner][] to inline all CSS rules for maximum client compatibility.
+
+Muttdown can also send its mail using the native `sendmail` if you have that set up (instead of doing SMTP itself). To do so, just leave the smtp options in the config file blank, set the `sendmail` option to the fully-qualified path to your `sendmail` binary, and run muttdown with the `-s` flag
+
+If `assume_markdown` is true, then all input is assumed to be Markdown by default and the `!m` sigil does nothing.
+
+Installation
+------------
+Install muttdown with `pip install muttdown` or by downloading this package and running `python setup.py install`. You will need the [PyYAML][] and [Python-Markdown][] libraries, as specified in `requirements.txt`. This should work with Python 3.6+.
+
+Usage
+-----
+Invoke as
+
+    muttdown -c /path/to/config -f "from_address" -- "to_address" [more to addresses...]
+
+Send a RFC822 formatted mail on stdin.
+
+If the config path is not passed, it will assume `~/.muttdown.yaml`.
+
+
+
+
+[Markdown]: http://daringfireball.net/projects/markdown/
+[YAML]: http://yaml.org
+[PyYAML]: http://pyyaml.org
+[Python-Markdown]: https://pypi.python.org/pypi/Markdown
+[mutt]: http://www.mutt.org
+[pynliner]: https://github.com/rennat/pynliner
```

### Comparing `muttdown-0.3.5/README.md` & `muttdown-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 muttdown
 ========
 
-[![Build Status](https://travis-ci.com/Roguelazer/muttdown.svg?branch=master)](https://travis-ci.com/Roguelazer/muttdown)
+[![Build Status](https://github.com/Roguelazer/muttdown/actions/workflows/ci.yml/badge.svg)](https://github.com/Roguelazer/muttdown/actions/workflows/ci.yml)
 
 `muttdown` is a sendmail-replacement designed for use with the [mutt][] email client which will transparently compile annotated `text/plain` mail into `text/html` using the [Markdown][] standard.  It will recursively walk the MIME tree and compile any `text/plain` or `text/markdown` part which begins with the sigil "!m" into Markdown, which it will insert alongside the original in a multipart/alternative container.
 
 It's also smart enough not to break `multipart/signed`.
 
 For example, the following tree before parsing:
 
@@ -42,29 +42,32 @@
 
     smtp_host: smtp.gmail.com
     smtp_port: 587
     smtp_ssl: false
     smtp_username: foo@bar.com
     smtp_password: foo
     css_file: ~/.muttdown.css
+    assume_markdown: false
 
 
 If you prefer not to put your password in plaintext in a configuration file, you can instead specify the `smtp_password_command` parameter to invoke a shell command to lookup your password. The command should output your password, followed by a newline, and no other text. On OS X, the following invocation will extract a generic "Password" entry with the application set to "mutt" and the title set to "foo@bar.com":
 
     smtp_password_command: security find-generic-password -w -s mutt -a foo@bar.com
 
 NOTE: If `smtp_ssl` is set to False, `muttdown` will do a non-SSL session and then invoke `STARTTLS`. If `smtp_ssl` is set to True, `muttdown` will do an SSL session from the get-go. There is no option to send mail in plaintext.
 
 The `css_file` should be regular CSS styling blocks; we use [pynliner][] to inline all CSS rules for maximum client compatibility.
 
 Muttdown can also send its mail using the native `sendmail` if you have that set up (instead of doing SMTP itself). To do so, just leave the smtp options in the config file blank, set the `sendmail` option to the fully-qualified path to your `sendmail` binary, and run muttdown with the `-s` flag
 
+If `assume_markdown` is true, then all input is assumed to be Markdown by default and the `!m` sigil does nothing.
+
 Installation
 ------------
-Install muttdown with `pip install muttdown` or by downloading this package and running `python setup.py install`. You will need the [PyYAML][] and [Python-Markdown][] libraries, as specified in `requirements.txt`. This should work with Python 2.7 or Python 3.5+.
+Install muttdown with `pip install muttdown` or by downloading this package and running `python setup.py install`. You will need the [PyYAML][] and [Python-Markdown][] libraries, as specified in `requirements.txt`. This should work with Python 3.6+.
 
 Usage
 -----
 Invoke as
 
     muttdown -c /path/to/config -f "from_address" -- "to_address" [more to addresses...]
```

### Comparing `muttdown-0.3.5/muttdown/config.py` & `muttdown-0.4.0/muttdown/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 import copy
-import yaml
-import subprocess
 import os.path
+from subprocess import check_output
 
 import six
+import yaml
 
 # largely copied from my earlier work in fakemtpd
 
 
-if hasattr(subprocess, 'check_output'):
-    check_output = subprocess.check_output
-else:
-    def check_output(*args, **kwargs):
-        kwargs['stdout'] = subprocess.PIPE
-        p = subprocess.Popen(*args, **kwargs)
-        stdout, _ = p.communicate()
-        assert p.returncode == 0
-        return stdout
-
-
 def _param_getter_factory(parameter):
     def f(self):
         return self._config[parameter]
+
     f.__name__ = parameter
     return f
 
 
 class _ParamsAsProps(type):
     """Create properties on the classes that apply this for everything
     in cls._parameters which read out of self._config.
 
     Cool fact: you can override any of these properties by just defining
     your own with the same name. Just like if they were statically defined!"""
+
     def __new__(clsarg, name, bases, d):
         cls = super(_ParamsAsProps, clsarg).__new__(clsarg, name, bases, d)
         for parameter in cls._parameters.keys():
             if parameter not in d:
                 f = _param_getter_factory(parameter)
                 setattr(cls, parameter, property(f))
         return cls
 
 
 class ConfigError(Exception):
     def __init__(self, message):
         self.message = message
 
     def __repr__(self):
-        return '%s(%r)' % (self.__class__.__name__, self.message)
+        return "%s(%r)" % (self.__class__.__name__, self.message)
 
     def __str__(self):
-        return '%s(%r)' % (self.__class__.__name__, self.message)
+        return "%s(%r)" % (self.__class__.__name__, self.message)
 
 
 @six.add_metaclass(_ParamsAsProps)
 class Config(object):
     _parameters = {
-        'smtp_host': '127.0.0.1',
-        'smtp_port': 25,
-        'smtp_ssl': True,  # if false, do STARTTLS
-        'smtp_username': '',
-        'smtp_password': None,
-        'smtp_password_command': None,
-        'smtp_timeout': 10,
-        'css_file': None,
-        'sendmail': '/usr/sbin/sendmail',
+        "smtp_host": "127.0.0.1",
+        "smtp_port": 25,
+        "smtp_ssl": True,  # if false, do STARTTLS
+        "smtp_username": "",
+        "smtp_password": None,
+        "smtp_password_command": None,
+        "smtp_timeout": 10,
+        "css_file": None,
+        "sendmail": "/usr/sbin/sendmail",
+        "assume_markdown": False,
     }
 
     def __init__(self):
         self._config = copy.copy(self._parameters)
         self._css = None
 
     def merge_config(self, d):
         invalid_keys = set(d.keys()) - set(self._config.keys())
         if invalid_keys:
-            raise ConfigError('Unexpected config keys: %s' % ', '.join(sorted(invalid_keys)))
+            raise ConfigError(
+                "Unexpected config keys: %s" % ", ".join(sorted(invalid_keys))
+            )
         for key in self._config:
             if key in d:
                 self._config[key] = d[key]
-        if self._config['smtp_password'] and self._config['smtp_password_command']:
-            raise ConfigError('Cannot set smtp_password *and* smtp_password_command')
-        if self._config['css_file']:
+        if self._config["smtp_password"] and self._config["smtp_password_command"]:
+            raise ConfigError("Cannot set smtp_password *and* smtp_password_command")
+        if self._config["css_file"]:
             self._css = None
-            self._config['css_file'] = os.path.expanduser(self._config['css_file'])
-            if not os.path.exists(self._config['css_file']):
-                raise ConfigError('CSS file %s does not exist' % self._config['css_file'])
+            self._config["css_file"] = os.path.expanduser(self._config["css_file"])
+            if not os.path.exists(self._config["css_file"]):
+                raise ConfigError(
+                    "CSS file %s does not exist" % self._config["css_file"]
+                )
 
     def load(self, fobj):
         d = yaml.safe_load(fobj)
         self.merge_config(d)
 
     @property
     def css(self):
         if self._css is None:
             if self.css_file is not None:
-                with open(os.path.expanduser(self.css_file), 'r') as f:
+                with open(os.path.expanduser(self.css_file), "r") as f:
                     self._css = f.read()
             else:
-                self._css = ''
+                self._css = ""
         return self._css
 
     @property
     def smtp_password(self):
-        if self._config['smtp_password_command']:
-            return check_output(self._config['smtp_password_command'], shell=True, universal_newlines=True).rstrip('\n')
+        if self._config["smtp_password_command"]:
+            return check_output(
+                self._config["smtp_password_command"],
+                shell=True,
+                universal_newlines=True,
+            ).rstrip("\n")
         else:
-            return self._config['smtp_password']
+            return self._config["smtp_password"]
```

### Comparing `muttdown-0.3.5/muttdown/main.py` & `muttdown-0.4.0/muttdown/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from __future__ import print_function
 
 import argparse
-import sys
-import smtplib
-import re
-import os.path
 import email
 import email.iterators
+import os.path
+import re
+import smtplib
+import subprocess
+import sys
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 
-import subprocess
-import six
-
 import markdown
 import pynliner
+import six
 
-from . import config
-from . import __version__
+from . import __version__, config
 
-__name__ = 'muttdown'
+__name__ = "muttdown"
 
 
 def get_charset_from_message_fragment(part):
     cs = part.get_charset()
     if cs:
         return cs.output_charset
     return None
@@ -36,42 +34,45 @@
     if not isinstance(text, six.text_type):
         # decode=True only decodes the base64/uuencoded nature, and
         # will always return bytes; gotta decode it
         if charset is not None:
             text = text.decode(charset)
         else:
             try:
-                text = text.decode('ascii')
+                text = text.decode("ascii")
             except UnicodeError:
                 # this is because of message.py:278 and seems like a hack
-                text = text.decode('raw-unicode-escape')
-    if not text.startswith('!m'):
-        return None
-    text = re.sub(r'\s*!m\s*', '', text, re.M)
-    if '\n-- \n' in text:
-        pre_signature, signature = text.split('\n-- \n')
-        md = markdown.markdown(pre_signature, output_format="html5")
+                text = text.decode("raw-unicode-escape")
+    if not config.assume_markdown:
+        if not text.startswith("!m"):
+            return None
+        text = re.sub(r"\s*!m\s*", "", text, re.M)
+    if "\n-- \n" in text:
+        pre_signature, signature = text.split("\n-- \n")
+        md = markdown.markdown(
+            pre_signature, extensions=["extra"], output_format="html5"
+        )
         md += '\n<div class="signature" style="font-size: small"><p>-- <br />'
-        md += '<br />'.join(signature.split('\n'))
-        md += '</p></div>'
+        md += "<br />".join(signature.split("\n"))
+        md += "</p></div>"
     else:
-        md = markdown.markdown(text)
+        md = markdown.markdown(text, extensions=["extra"])
     if config.css:
-        md = '<style>' + config.css + '</style>' + md
+        md = "<style>" + config.css + "</style>" + md
         md = pynliner.fromString(md)
-    message = MIMEText(md, 'html', _charset="UTF-8")
+    message = MIMEText(md, "html", _charset="UTF-8")
     return message
 
 
 def _move_headers(source, dest):
     for k, v in source.items():
         # mutt sometimes sticks in a fake bcc header
-        if k.lower() == 'bcc':
+        if k.lower() == "bcc":
             del source[k]
-        elif not (k.startswith('Content-') or k.startswith('MIME')):
+        elif not (k.startswith("Content-") or k.startswith("MIME")):
             dest.add_header(k, v)
             del source[k]
 
 
 def convert_tree(message, config, indent=0, wrap_alternative=True, charset=None):
     """Recursively convert a potentially-multipart tree.
 
@@ -80,62 +81,68 @@
     ct = message.get_content_type()
     cs = message.get_content_subtype()
     if charset is None:
         charset = get_charset_from_message_fragment(message)
     if not message.is_multipart():
         # we're on a leaf
         converted = None
-        disposition = message.get('Content-Disposition', 'inline')
-        if disposition == 'inline' and ct in ('text/plain', 'text/markdown'):
+        disposition = message.get("Content-Disposition", "inline")
+        if disposition == "inline" and ct in ("text/plain", "text/markdown"):
             converted = convert_one(message, config, charset)
         if converted is not None:
             if wrap_alternative:
-                new_tree = MIMEMultipart('alternative')
+                new_tree = MIMEMultipart("alternative")
                 _move_headers(message, new_tree)
                 new_tree.attach(message)
                 new_tree.attach(converted)
                 return new_tree, True
             else:
                 return converted, True
         return message, False
     else:
-        if ct == 'multipart/signed':
+        if ct == "multipart/signed":
             # if this is a multipart/signed message, then let's just
             # recurse into the non-signature part
-            new_root = MIMEMultipart('alternative')
+            new_root = MIMEMultipart("alternative")
             if message.preamble:
                 new_root.preamble = message.preamble
             _move_headers(message, new_root)
             converted = None
             for part in message.get_payload():
-                if part.get_content_type() != 'application/pgp-signature':
-                    converted, did_conversion = convert_tree(part, config, indent=indent + 1,
-                                                             wrap_alternative=False,
-                                                             charset=charset)
+                if part.get_content_type() != "application/pgp-signature":
+                    converted, did_conversion = convert_tree(
+                        part,
+                        config,
+                        indent=indent + 1,
+                        wrap_alternative=False,
+                        charset=charset,
+                    )
                     if did_conversion:
                         new_root.attach(converted)
             new_root.attach(message)
             return new_root, did_conversion
         else:
             did_conversion = False
             new_root = MIMEMultipart(cs, message.get_charset())
             if message.preamble:
                 new_root.preamble = message.preamble
             _move_headers(message, new_root)
             for part in message.get_payload():
-                part, did_this_conversion = convert_tree(part, config, indent=indent + 1, charset=charset)
+                part, did_this_conversion = convert_tree(
+                    part, config, indent=indent + 1, charset=charset
+                )
                 did_conversion |= did_this_conversion
                 new_root.attach(part)
             return new_root, did_conversion
 
 
 def process_message(mail, config):
     converted, did_any_markdown = convert_tree(mail, config)
-    if 'Bcc' in converted:
-        del converted['Bcc']
+    if "Bcc" in converted:
+        del converted["Bcc"]
     return converted
 
 
 def smtp_connection(c):
     """Create an SMTP connection from a Config object"""
     if c.smtp_ssl:
         klass = smtplib.SMTP_SSL
@@ -152,67 +159,76 @@
 
 
 def read_message():
     return sys.stdin.read()
 
 
 def main(argv=None):
-    parser = argparse.ArgumentParser(prog='muttdown')
-    parser.add_argument('-v', '--version', action='version', version='%s %s' % (__name__, __version__))
+    parser = argparse.ArgumentParser(prog="muttdown")
+    parser.add_argument(
+        "-v", "--version", action="version", version="%s %s" % (__name__, __version__)
+    )
     parser.add_argument(
-        '-c', '--config_file', default=os.path.expanduser('~/.muttdown.yaml'),
-        type=argparse.FileType('r'), required=False,
-        help='Path to YAML config file (default %(default)s)'
+        "-c",
+        "--config_file",
+        default=os.path.expanduser("~/.muttdown.yaml"),
+        type=argparse.FileType("r"),
+        required=False,
+        help="Path to YAML config file (default %(default)s)",
     )
     parser.add_argument(
-        '-p', '--print-message', action='store_true',
-        help='Print the translated message to stdout instead of sending it'
+        "-p",
+        "--print-message",
+        action="store_true",
+        help="Print the translated message to stdout instead of sending it",
     )
-    parser.add_argument('-f', '--envelope-from', required=True)
+    parser.add_argument("-f", "--envelope-from", required=True)
     parser.add_argument(
-        '-s', '--sendmail-passthru', action='store_true',
-        help='Pass mail through to sendmail for delivery'
+        "-s",
+        "--sendmail-passthru",
+        action="store_true",
+        help="Pass mail through to sendmail for delivery",
     )
-    parser.add_argument('addresses', nargs='+')
+    parser.add_argument("addresses", nargs="+")
     args = parser.parse_args(argv)
 
     c = config.Config()
     try:
         c.load(args.config_file)
     except config.ConfigError as e:
-        sys.stderr.write('Error(s) in configuration %s:\n' % args.config_file.name)
-        sys.stderr.write(' - %s\n' % e.message)
+        sys.stderr.write("Error(s) in configuration %s:\n" % args.config_file.name)
+        sys.stderr.write(" - %s\n" % e.message)
         sys.stderr.flush()
         return 1
 
     message = read_message()
 
     mail = email.message_from_string(message)
 
     rebuilt = process_message(mail, c)
     rebuilt.set_unixfrom(args.envelope_from)
 
     if args.print_message:
         print(rebuilt.as_string())
     elif args.sendmail_passthru:
-        cmd = c.sendmail.split() + ['-f', args.envelope_from] + args.addresses
+        cmd = c.sendmail.split() + ["-f", args.envelope_from] + args.addresses
 
         proc = subprocess.Popen(cmd, stdin=subprocess.PIPE, shell=False)
         msg = rebuilt.as_string()
         if sys.version_info > (3, 0):
-            msg = msg.encode('utf-8')
+            msg = msg.encode("utf-8")
         proc.stdin.write(msg)
         proc.stdin.close()
         proc.wait()
         return proc.returncode
     else:
         conn = smtp_connection(c)
         msg = rebuilt.as_string()
         if sys.version_info > (3, 0):
-            msg = msg.encode('utf-8')
+            msg = msg.encode("utf-8")
         conn.sendmail(args.envelope_from, args.addresses, msg)
         conn.quit()
     return 0
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `muttdown-0.3.5/muttdown.egg-info/PKG-INFO` & `muttdown-0.4.0/muttdown.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,116 @@
 Metadata-Version: 2.1
 Name: muttdown
-Version: 0.3.5
+Version: 0.4.0
 Summary: Sendmail replacement that compiles markdown into HTML
 Home-page: https://github.com/Roguelazer/muttdown
 Author: James Brown
-Author-email: Roguelazer@gmail.com
+Author-email: roguelazer@roguelazer.com
 License: ISC
-Description: muttdown
-        ========
-        
-        [![Build Status](https://travis-ci.com/Roguelazer/muttdown.svg?branch=master)](https://travis-ci.com/Roguelazer/muttdown)
-        
-        `muttdown` is a sendmail-replacement designed for use with the [mutt][] email client which will transparently compile annotated `text/plain` mail into `text/html` using the [Markdown][] standard.  It will recursively walk the MIME tree and compile any `text/plain` or `text/markdown` part which begins with the sigil "!m" into Markdown, which it will insert alongside the original in a multipart/alternative container.
-        
-        It's also smart enough not to break `multipart/signed`.
-        
-        For example, the following tree before parsing:
-        
-            - multipart/mixed
-             |
-             -- multipart/signed
-             |
-             ---- text/markdown
-             |
-             ---- application/pgp-signature
-             |
-             -- image/png
-        
-        Will get compiled into
-        
-            - multipart/mixed
-             |
-             -- multipart/alternative
-             |
-             ---- text/html
-             |
-             ---- multipart/signed
-             |
-             ------ text/markdown
-             |
-             ------ application/pgp-signature
-             |
-             -- image/png
-        
-        
-        Configuration
-        -------------
-        Muttdown's configuration file is written using [YAML][]. Example:
-        
-            smtp_host: smtp.gmail.com
-            smtp_port: 587
-            smtp_ssl: false
-            smtp_username: foo@bar.com
-            smtp_password: foo
-            css_file: ~/.muttdown.css
-        
-        
-        If you prefer not to put your password in plaintext in a configuration file, you can instead specify the `smtp_password_command` parameter to invoke a shell command to lookup your password. The command should output your password, followed by a newline, and no other text. On OS X, the following invocation will extract a generic "Password" entry with the application set to "mutt" and the title set to "foo@bar.com":
-        
-            smtp_password_command: security find-generic-password -w -s mutt -a foo@bar.com
-        
-        NOTE: If `smtp_ssl` is set to False, `muttdown` will do a non-SSL session and then invoke `STARTTLS`. If `smtp_ssl` is set to True, `muttdown` will do an SSL session from the get-go. There is no option to send mail in plaintext.
-        
-        The `css_file` should be regular CSS styling blocks; we use [pynliner][] to inline all CSS rules for maximum client compatibility.
-        
-        Muttdown can also send its mail using the native `sendmail` if you have that set up (instead of doing SMTP itself). To do so, just leave the smtp options in the config file blank, set the `sendmail` option to the fully-qualified path to your `sendmail` binary, and run muttdown with the `-s` flag
-        
-        Installation
-        ------------
-        Install muttdown with `pip install muttdown` or by downloading this package and running `python setup.py install`. You will need the [PyYAML][] and [Python-Markdown][] libraries, as specified in `requirements.txt`. This should work with Python 2.7 or Python 3.5+.
-        
-        Usage
-        -----
-        Invoke as
-        
-            muttdown -c /path/to/config -f "from_address" -- "to_address" [more to addresses...]
-        
-        Send a RFC822 formatted mail on stdin.
-        
-        If the config path is not passed, it will assume `~/.muttdown.yaml`.
-        
-        
-        
-        
-        [Markdown]: http://daringfireball.net/projects/markdown/
-        [YAML]: http://yaml.org
-        [PyYAML]: http://pyyaml.org
-        [Python-Markdown]: https://pypi.python.org/pypi/Markdown
-        [mutt]: http://www.mutt.org
-        [pynliner]: https://github.com/rennat/pynliner
-        
 Keywords: email
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Topic :: Communications :: Email
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: Markdown<4.0,>=3.0
+Requires-Dist: PyYAML>=3.0
+Requires-Dist: pynliner==0.8.0
+Requires-Dist: six
+
+muttdown
+========
+
+[![Build Status](https://github.com/Roguelazer/muttdown/actions/workflows/ci.yml/badge.svg)](https://github.com/Roguelazer/muttdown/actions/workflows/ci.yml)
+
+`muttdown` is a sendmail-replacement designed for use with the [mutt][] email client which will transparently compile annotated `text/plain` mail into `text/html` using the [Markdown][] standard.  It will recursively walk the MIME tree and compile any `text/plain` or `text/markdown` part which begins with the sigil "!m" into Markdown, which it will insert alongside the original in a multipart/alternative container.
+
+It's also smart enough not to break `multipart/signed`.
+
+For example, the following tree before parsing:
+
+    - multipart/mixed
+     |
+     -- multipart/signed
+     |
+     ---- text/markdown
+     |
+     ---- application/pgp-signature
+     |
+     -- image/png
+
+Will get compiled into
+
+    - multipart/mixed
+     |
+     -- multipart/alternative
+     |
+     ---- text/html
+     |
+     ---- multipart/signed
+     |
+     ------ text/markdown
+     |
+     ------ application/pgp-signature
+     |
+     -- image/png
+
+
+Configuration
+-------------
+Muttdown's configuration file is written using [YAML][]. Example:
+
+    smtp_host: smtp.gmail.com
+    smtp_port: 587
+    smtp_ssl: false
+    smtp_username: foo@bar.com
+    smtp_password: foo
+    css_file: ~/.muttdown.css
+    assume_markdown: false
+
+
+If you prefer not to put your password in plaintext in a configuration file, you can instead specify the `smtp_password_command` parameter to invoke a shell command to lookup your password. The command should output your password, followed by a newline, and no other text. On OS X, the following invocation will extract a generic "Password" entry with the application set to "mutt" and the title set to "foo@bar.com":
+
+    smtp_password_command: security find-generic-password -w -s mutt -a foo@bar.com
+
+NOTE: If `smtp_ssl` is set to False, `muttdown` will do a non-SSL session and then invoke `STARTTLS`. If `smtp_ssl` is set to True, `muttdown` will do an SSL session from the get-go. There is no option to send mail in plaintext.
+
+The `css_file` should be regular CSS styling blocks; we use [pynliner][] to inline all CSS rules for maximum client compatibility.
+
+Muttdown can also send its mail using the native `sendmail` if you have that set up (instead of doing SMTP itself). To do so, just leave the smtp options in the config file blank, set the `sendmail` option to the fully-qualified path to your `sendmail` binary, and run muttdown with the `-s` flag
+
+If `assume_markdown` is true, then all input is assumed to be Markdown by default and the `!m` sigil does nothing.
+
+Installation
+------------
+Install muttdown with `pip install muttdown` or by downloading this package and running `python setup.py install`. You will need the [PyYAML][] and [Python-Markdown][] libraries, as specified in `requirements.txt`. This should work with Python 3.6+.
+
+Usage
+-----
+Invoke as
+
+    muttdown -c /path/to/config -f "from_address" -- "to_address" [more to addresses...]
+
+Send a RFC822 formatted mail on stdin.
+
+If the config path is not passed, it will assume `~/.muttdown.yaml`.
+
+
+
+
+[Markdown]: http://daringfireball.net/projects/markdown/
+[YAML]: http://yaml.org
+[PyYAML]: http://pyyaml.org
+[Python-Markdown]: https://pypi.python.org/pypi/Markdown
+[mutt]: http://www.mutt.org
+[pynliner]: https://github.com/rennat/pynliner
```

### Comparing `muttdown-0.3.5/setup.py` & `muttdown-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-#!/usr/bin/env python
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-with open('README.md', 'r') as f:
+with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="muttdown",
-    version="0.3.5",
+    version="0.4.0",
     author="James Brown",
-    author_email="Roguelazer@gmail.com",
+    author_email="roguelazer@roguelazer.com",
     url="https://github.com/Roguelazer/muttdown",
     license="ISC",
-    packages=find_packages(exclude=['tests']),
+    packages=find_packages(exclude=["tests"]),
     keywords=["email"],
     description="Sendmail replacement that compiles markdown into HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
-        'Markdown>=2.0',
-        'PyYAML>=3.0',
-        'pynliner==0.8.0',
-        'six',
+        "Markdown>=3.0,<4.0",
+        "PyYAML>=3.0",
+        "pynliner==0.8.0",
+        "six",
     ],
     entry_points={
-        'console_scripts': [
-            'muttdown = muttdown.main:main',
+        "console_scripts": [
+            "muttdown = muttdown.main:main",
         ]
     },
+    python_requires=">=3.6",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Intended Audience :: End Users/Desktop",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: ISC License (ISCL)",
         "Topic :: Communications :: Email",
-    ]
+    ],
 )
```

