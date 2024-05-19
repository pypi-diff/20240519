# Comparing `tmp/cs.cmdutils-20240422.tar.gz` & `tmp/cs.cmdutils-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.cmdutils-20240422.tar", last modified: Mon Apr 22 02:56:31 2024, max compression
+gzip compressed data, was "cs.cmdutils-20240519.tar", last modified: Sun May 19 02:28:51 2024, max compression
```

## Comparing `cs.cmdutils-20240422.tar` & `cs.cmdutils-20240519.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.562566 cs.cmdutils-20240422/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:55:45.000000 cs.cmdutils-20240422/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    31799 2024-04-22 02:56:31.561543 cs.cmdutils-20240422/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    30929 2024-04-22 02:56:00.000000 cs.cmdutils-20240422/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.557411 cs.cmdutils-20240422/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.557725 cs.cmdutils-20240422/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.559253 cs.cmdutils-20240422/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    52525 2024-04-22 02:55:32.000000 cs.cmdutils-20240422/lib/python/cs/cmdutils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.561063 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    31799 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      291 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      231 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    32520 2024-04-22 02:56:30.000000 cs.cmdutils-20240422/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 02:56:31.562677 cs.cmdutils-20240422/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:28:51.886320 cs.cmdutils-20240519/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-19 02:28:06.000000 cs.cmdutils-20240519/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    31640 2024-05-19 02:28:51.886001 cs.cmdutils-20240519/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    30770 2024-05-19 02:28:21.000000 cs.cmdutils-20240519/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:28:51.880688 cs.cmdutils-20240519/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:28:51.880980 cs.cmdutils-20240519/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:28:51.882668 cs.cmdutils-20240519/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    52542 2024-05-19 02:27:52.000000 cs.cmdutils-20240519/lib/python/cs/cmdutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:28:51.884956 cs.cmdutils-20240519/lib/python/cs.cmdutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    31640 2024-05-19 02:28:51.000000 cs.cmdutils-20240519/lib/python/cs.cmdutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      291 2024-05-19 02:28:51.000000 cs.cmdutils-20240519/lib/python/cs.cmdutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-19 02:28:51.000000 cs.cmdutils-20240519/lib/python/cs.cmdutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      231 2024-05-19 02:28:51.000000 cs.cmdutils-20240519/lib/python/cs.cmdutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-19 02:28:51.000000 cs.cmdutils-20240519/lib/python/cs.cmdutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    32361 2024-05-19 02:28:50.000000 cs.cmdutils-20240519/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-19 02:28:51.886432 cs.cmdutils-20240519/setup.cfg
```

### Comparing `cs.cmdutils-20240422/PKG-INFO` & `cs.cmdutils-20240519/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,13 @@
-Metadata-Version: 2.1
-Name: cs.cmdutils
-Version: 20240422
-Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20240422*:
-* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
-* BaseCommand.apply_preargv: apply the default options supported by self.options.
-* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
+*Latest release 20240519*:
+BaseCommand.run_context: attach the runstate to the options.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -251,15 +231,15 @@
 this can be overridden with a method which just returns `False`.
 
 Otherwise,
 the handler may perform any suitable action
 and return `True` to contain the exception
 or `False` to cause the exception to be reraised.
 
-*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x104df9f30>)`*:
+*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10a199f30>)`*:
 The default signal handler, which cancels the default `RunState`.
 
 *Method `BaseCommand.poparg(argv: List[str], *a, unpop_on_error=False)`*:
 Pop the leading argument off `argv` and parse it.
 Return the parsed argument.
 Raises `getopt.GetoptError` on a missing or invalid argument.
 
@@ -447,15 +427,15 @@
 Otherwise `self.main(argv)` is called
 and its value returned.
 
 If the command implementation requires some setup or teardown
 then this may be provided by the `run_context()`
 context manager method.
 
-*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x104cea3b0>, **kw)`*:
+*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x10a2e64d0>, **kw)`*:
 The context manager which surrounds `main` or `cmd_`*subcmd*.
 
 This default does several things, and subclasses should
 override it like this:
 
     @contextmanager
     def run_context(self):
@@ -653,14 +633,17 @@
             print("doing f with x =", x)
         ....
 
 # Release Log
 
 
 
+*Release 20240519*:
+BaseCommand.run_context: attach the runstate to the options.
+
 *Release 20240422*:
 * BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
 * BaseCommand.apply_preargv: apply the default options supported by self.options.
 * BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
 
 *Release 20240412*:
 * BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
@@ -834,8 +817,7 @@
 Minor documentation updates.
 
 *Release 20190617.2*:
 Lint.
 
 *Release 20190617.1*:
 Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class.
-
```

### Comparing `cs.cmdutils-20240422/README.md` & `cs.cmdutils-20240519/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,88 @@
+[project]
+name = "cs.cmdutils"
+description = "Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.context>=20240412",
+    "cs.deco>=20240412",
+    "cs.lex>=20240519",
+    "cs.logutils>=20230212",
+    "cs.pfx>=20240412",
+    "cs.py.doc>=20240422",
+    "cs.resources>=20240519",
+    "cs.result>=20240412",
+    "cs.threads>=20240422",
+    "cs.typingutils>=20230331",
+    "cs.upd>=20240412",
+    "typeguard",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20240519"
+
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20240422*:
-* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
-* BaseCommand.apply_preargv: apply the default options supported by self.options.
-* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
+*Latest release 20240519*:
+BaseCommand.run_context: attach the runstate to the options.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
 To implement a command line
 one instantiates a subclass of `BaseCommand`:
 
     class MyCommand(BaseCommand):
         GETOPT_SPEC = 'ab:c'
-        USAGE_FORMAT = r"""Usage: {cmd} [-a] [-b bvalue] [-c] [--] arguments...
+        USAGE_FORMAT = r\"\"\"Usage: {cmd} [-a] [-b bvalue] [-c] [--] arguments...
           -a    Do it all.
           -b    But using bvalue.
           -c    The 'c' option!
-        """
+        \"\"\"
         ...
 
 and provides either a `main` method if the command has no subcommands
 or a suite of `cmd_`*subcommand* methods, one per subcommand.
 
 Running a command is done by:
 
     MyCommand(argv).run()
 
 Modules which implement a command line mode generally look like this:
 
     ... imports etc ...
     def main(argv=None, **run_kw):
-        """ The command line mode.
-        """
+        \"\"\" The command line mode.
+        \"\"\"
         return MyCommand(argv).run(**run_kw)
     ... other code ...
     class MyCommand(BaseCommand):
     ... other code ...
     if __name__ == '__main__':
         sys.exit(main(sys.argv))
 
@@ -63,20 +104,20 @@
 Returning to methods, if there is a paragraph in the method docstring
 commencing with `Usage:`
 then that paragraph is incorporated automatically
 into the main usage message.
 Example:
 
     def cmd_ls(self, argv):
-        """ Usage: {cmd} [paths...]
+        \"\"\" Usage: {cmd} [paths...]
               Emit a listing for the named paths.
 
             Further docstring non-usage information here.
-        """
-        ... do the "ls" subcommand ...
+        \"\"\"
+        ... do the \"ls\" subcommand ...
 
 The subclass is customised by overriding the following methods:
 * `apply_opt(opt,val)`:
   apply an individual getopt global command line option
   to `self.options`.
 * `apply_opts(opts)`:
   apply the `opts` to `self.options`.
@@ -233,15 +274,15 @@
 this can be overridden with a method which just returns `False`.
 
 Otherwise,
 the handler may perform any suitable action
 and return `True` to contain the exception
 or `False` to cause the exception to be reraised.
 
-*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x104df9f30>)`*:
+*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10a199f30>)`*:
 The default signal handler, which cancels the default `RunState`.
 
 *Method `BaseCommand.poparg(argv: List[str], *a, unpop_on_error=False)`*:
 Pop the leading argument off `argv` and parse it.
 Return the parsed argument.
 Raises `getopt.GetoptError` on a missing or invalid argument.
 
@@ -266,49 +307,49 @@
   for values failing the validation
 * `unpop_on_error`: optional keyword parameter, default `False`;
   if true then push the argument back onto the front of `argv`
   if it fails to parse; `GetoptError` is still raised
 
 Typical use inside a `main` or `cmd_*` method might look like:
 
-    self.options.word = self.poparg(argv, int, "a count value")
+    self.options.word = self.poparg(argv, int, \"a count value\")
     self.options.word = self.poparg(
-        argv, int, "a count value",
-       lambda count: count > 0, "count should be positive")
+        argv, int, \"a count value\",
+       lambda count: count > 0, \"count should be positive\")
 
 Because it raises `GetoptError` on a bad argument
 the normal usage message failure mode follows automatically.
 
 Demonstration:
 
     >>> argv = ['word', '3', 'nine', '4']
-    >>> BaseCommand.poparg(argv, "word to process")
+    >>> BaseCommand.poparg(argv, \"word to process\")
     'word'
-    >>> BaseCommand.poparg(argv, int, "count value")
+    >>> BaseCommand.poparg(argv, int, \"count value\")
     3
-    >>> BaseCommand.poparg(argv, float, "length")
+    >>> BaseCommand.poparg(argv, float, \"length\")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: length 'nine': float('nine'): could not convert string to float: 'nine'
-    >>> BaseCommand.poparg(argv, float, "width", lambda width: width > 5)
+    >>> BaseCommand.poparg(argv, float, \"width\", lambda width: width > 5)
     Traceback (most recent call last):
       ...
     getopt.GetoptError: width '4': invalid value
-    >>> BaseCommand.poparg(argv, float, "length")
+    >>> BaseCommand.poparg(argv, float, \"length\")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: length: missing argument
     >>> argv = ['-5', 'zz']
-    >>> BaseCommand.poparg(argv, float, "size", lambda f: f>0, "size should be >0")
+    >>> BaseCommand.poparg(argv, float, \"size\", lambda f: f>0, \"size should be >0\")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: size '-5': size should be >0
     >>> argv  # -5 was still consumed
     ['zz']
-    >>> BaseCommand.poparg(argv, float, "size2", unpop_on_error=True)
+    >>> BaseCommand.poparg(argv, float, \"size2\", unpop_on_error=True)
     Traceback (most recent call last):
       ...
     getopt.GetoptError: size2 'zz': float('zz'): could not convert string to float: 'zz'
     >>> argv  # zz was pushed back
     ['zz']
 
 *Method `BaseCommand.popopts(argv, attrfor=None, **opt_specs)`*:
@@ -343,20 +384,20 @@
 
     class SomeCommand(BaseCommand):
 
         def cmd_foo(self, argv):
             options = self.options
             # accept a -j or --jobs options
             options.popopts(argv, jobs=1, j='jobs')
-            print("jobs =", options.jobs)
+            print(\"jobs =\", options.jobs)
 
 The `self.options` object is preprovided as an instance of
 the `self.Options` class, which is `BaseCommandOptions` by
 default. This presupplies support for some basic options
-like `-v` for "verbose" and so forth, and a subcommand
+like `-v` for \"verbose\" and so forth, and a subcommand
 need not describe these in a call to `self.options.popopts()`.
 
 Example:
 
     >>> import os.path
     >>> from typing import Optional
     >>> @dataclass
@@ -403,17 +444,17 @@
 * the attributes of `self`
 
 This is not presented automatically as a subcommand, but
 commands wishing such a command should provide something
 like this:
 
     def cmd_repl(self, argv):
-        """ Usage: {cmd}
+        \"\"\" Usage: {cmd}
               Run an interactive Python prompt with some predefined local names.
-        """
+        \"\"\"
         return self.repl(*argv)
 
 *Method `BaseCommand.run(self, **kw_options)`*:
 Run a command.
 Returns the exit status of the command.
 May raise `GetoptError` from subcommands.
 
@@ -429,15 +470,15 @@
 Otherwise `self.main(argv)` is called
 and its value returned.
 
 If the command implementation requires some setup or teardown
 then this may be provided by the `run_context()`
 context manager method.
 
-*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x104cea3b0>, **kw)`*:
+*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x10a2e64d0>, **kw)`*:
 The context manager which surrounds `main` or `cmd_`*subcmd*.
 
 This default does several things, and subclasses should
 override it like this:
 
     @contextmanager
     def run_context(self):
@@ -458,15 +499,15 @@
 
 *Method `BaseCommand.subcommands()`*:
 Return a mapping of subcommand names to subcommand specifications
 for class attributes which commence with `cls.SUBCOMMAND_METHOD_PREFIX`
 by default `'cmd_'`.
 
 *Method `BaseCommand.usage_text(*, cmd=None, format_mapping=None, subcmd=None, short=False)`*:
-Compute the "Usage:" message for this class
+Compute the \"Usage:\" message for this class
 from the top level `USAGE_FORMAT`
 and the `'Usage:'`-containing docstrings of its `cmd_*` methods.
 
 Parameters:
 * `cmd`: optional command name, default derived from the class name
 * `format_mapping`: an optional format mapping for filling
   in format strings in the usage text
@@ -552,15 +593,15 @@
     def cmd_foo(self, argv):
         self.options.popopts(
             c_='config',
             l='long',
             x='trace',
         )
         if self.options.dry_run:
-            print("dry run!")
+            print(\"dry run!\")
 
 The class attribute `COMMON_OPT_SPECS` is a mapping of
 options which are always supported. `BaseCommandOptions`
 has: `COMMON_OPT_SPECS={'n': 'dry_run', 'q': 'quiet', 'v': 'verbose'}`.
 
 A subclass with more common options might extend this like so,
 from `cs.hashindex`:
@@ -617,43 +658,46 @@
   provided its `cls.Options` class is used.
 * `options_param_name`: the parameter name to provide, default `options`
 
 Examples:
 
     @uses_cmd_options
     def f(x,*,options):
-        """ Run directly from the prevailing options. """
+        \"\"\" Run directly from the prevailing options. \"\"\"
         if options.verbose:
-            print("doing f with x =", x)
+            print(\"doing f with x =\", x)
         ....
 
     @uses_cmd_options
     def f(x,*,verbose=None,options):
-        """ Get defaults from the prevailing options. """
+        \"\"\" Get defaults from the prevailing options. \"\"\"
         if verbose is None:
             verbose = options.verbose
         if verbose:
-            print("doing f with x =", x)
+            print(\"doing f with x =\", x)
         ....
 
 # Release Log
 
 
 
+*Release 20240519*:
+BaseCommand.run_context: attach the runstate to the options.
+
 *Release 20240422*:
 * BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
 * BaseCommand.apply_preargv: apply the default options supported by self.options.
 * BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
 
 *Release 20240412*:
 * BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
 * BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
 
 *Release 20240316*:
-* New @uses_cmd_options decorator to provide an "options" parameter being the prevailing BaseCommandOptions instance.
+* New @uses_cmd_options decorator to provide an \"options\" parameter being the prevailing BaseCommandOptions instance.
 * BaseCommandOptions.popopts: get common options from BaseCommandOptions.COMMON_OPT_SPECS.
 
 *Release 20240211*:
 * Include the first sentence of the subcommand description in the short help.
 * BaseCommandOptions: move the runstate_signals into this directly.
 * BaseCommand: move the run() options stuff into run_context() and have it work on a copy of the original options.
 * BaseCommandCmd: implement get_names(), provide docstrings for the do_* attributes, thus help.
@@ -708,27 +752,27 @@
 * BaseCommand: new poparg(argv,...) compact validating argument consumer.
 * BaseCommand: drop run_argv, provided no utility.
 * BaseCommand.run: get the RunState signal list from self.options.runstate_signals.
 * BaseCommand.apply_opts: support multiple individual options raising GetoptError, as I hate commands which abort at the first bad option.
 * Assorted other small things.
 
 *Release 20220429*:
-* BaseCommand: fold dots in argv[0] into underscores, supports subcommands like "setup.py".
+* BaseCommand: fold dots in argv[0] into underscores, supports subcommands like \"setup.py\".
 * BaseCommand: new popargv(argv[,help_text[,parse[,validate[,unvalidated_message]]]]) helper class method.
 * BaseCommand: accept dashed-form of the underscored_form subcommand name.
 * BaseCommand: new self.options.runstate_signals=SIGINT,SIGTERM specifying singals to catch-and-cancel, shuffle run() context managers.
 
 *Release 20220318*:
 BaseCommand.__init__: handle main() method in the New Scheme.
 
 *Release 20220315*:
 _BaseSubCommand.__init__: hook in the class USAGE_KEYWORDS for methods.
 
 *Release 20220311*:
-BaseCommand: big refactor of subcommand internals and make the "cmd_foo=FooCommand" implementation work properly.
+BaseCommand: big refactor of subcommand internals and make the \"cmd_foo=FooCommand\" implementation work properly.
 
 *Release 20211208*:
 BaseCommand: better handle an unknown subcommand.
 
 *Release 20210927*:
 * Usage: show only the per subcommand usage for in-subcommand GetoptError.
 * Usage: show terse usage when the subcommand cannot be recognised.
@@ -743,57 +787,57 @@
 
 *Release 20210809*:
 Bugfix BaseCommand.cmd_help for modern API.
 
 *Release 20210731*:
 * BaseCommand.run: apply optional keyword arguments to self.options during the run.
 * Look for self.SUBCOMMAND_ARGV_DEFAULT if no subcommand is supplied.
-* Bugfix case for "main" method and no "cmd_*" methods.
+* Bugfix case for \"main\" method and no \"cmd_*\" methods.
 * Bugfix BaseCommand.cmd_help.
 
 *Release 20210420*:
 * BaseCommand.getopt_error_handler: replace error print() with warning().
 * Docstring improvements.
 
 *Release 20210407.1*:
 BaseCommand: bugfix for __init_subclass__ docstring update.
 
 *Release 20210407*:
 * BaseCommand.__init_subclass__: behave sanely if the subclass has no initial __doc__.
-* BaseCommand: new .run_argv convenience method, obviates the "def main" boilerplate.
+* BaseCommand: new .run_argv convenience method, obviates the \"def main\" boilerplate.
 
 *Release 20210404*:
 BaseCommand subclasses: automatically add the main usage message to the subclass docstring.
 
 *Release 20210306*:
 * BREAKING CHANGE: rework BaseCommand as a more normal class instantiated with argv and with most methods being instance methods, getting the former `options` parameter from self.options.
 * BaseCommand: provide default `apply_opt` and `apply_opts` methods; subclasses will generally just override the former.
 
 *Release 20210123*:
 BaseCommand: propagate the format mapping (cmd, USAGE_KEYWORDS) to the subusage generation.
 
 *Release 20201102*:
-* BaseCommand.cmd_help: supply usage only for "all commands", full docstring for specified commands.
+* BaseCommand.cmd_help: supply usage only for \"all commands\", full docstring for specified commands.
 * BaseCommand: honour presupplied options.log_level.
 * BaseCommand.usage_text: handle missing USAGE_FORMAT better.
 * BaseCommand.run: provide options.upd.
 * BaseCommand subclasses may now override BaseCommand.OPTIONS_CLASS (default SimpleNamespace) in order to provide convenience methods on the options.
 * BaseCommand.run: separate variable for subcmd with dash translated to underscore to match method names.
 * Minor fixes.
 
 *Release 20200615*:
-BaseCommand.usage_text: do not mention the "help" command if it is the only subcommand (it won't be available if there are no other subcommands).
+BaseCommand.usage_text: do not mention the \"help\" command if it is the only subcommand (it won't be available if there are no other subcommands).
 
 *Release 20200521.1*:
 Fix DISTINFO.install_requires.
 
 *Release 20200521*:
 * BaseCommand.run: support using BaseCommand subclasses as cmd_* names to make it easy to nest BaseCommands.
 * BaseCommand: new hack_postopts_argv method called after parsing the main command line options, for inferring subcommands or the like.
-* BaseCommand: extract "Usage:" paragraphs from subcommand method docstrings to build the main usage message.
+* BaseCommand: extract \"Usage:\" paragraphs from subcommand method docstrings to build the main usage message.
 * BaseCommand: new cmd_help default command.
 * Assorted bugfixes and small improvements.
 
 *Release 20200318*:
 * BaseCommand.run: make argv optional, get additional usage keywords from self.USAGE_KEYWORDS.
 * @BaseCommand.add_usage_to_docstring: honour cls.USAGE_KEYWORDS.
 * BaseCommand: do not require GETOPT_SPEC for commands with no defined options.
@@ -815,8 +859,25 @@
 *Release 20190619*:
 Minor documentation updates.
 
 *Release 20190617.2*:
 Lint.
 
 *Release 20190617.1*:
-Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class.
+Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class."""
+content-type = "text/markdown"
+
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+
+[tool.setuptools]
+py-modules = [
+    "cs.cmdutils",
+]
+
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

### Comparing `cs.cmdutils-20240422/lib/python/cs/cmdutils.py` & `cs.cmdutils-20240519/lib/python/cs/cmdutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from cs.py.doc import obj_docstring
 from cs.resources import RunState, uses_runstate
 from cs.result import CancellationError
 from cs.threads import HasThreadState, ThreadState
 from cs.typingutils import subtype
 from cs.upd import Upd, uses_upd
 
-__version__ = '20240422'
+__version__ = '20240519'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -1327,15 +1327,15 @@
     ''' The default signal handler, which cancels the default `RunState`.
     '''
     runstate.cancel()
 
   @contextmanager
   @uses_runstate
   @uses_upd
-  def run_context(self, *, runstate: RunState, upd: Upd, **kw_options):
+  def run_context(self, *, runstate: RunState, upd: Upd, **options_kw):
     ''' The context manager which surrounds `main` or `cmd_`*subcmd*.
 
         This default does several things, and subclasses should
         override it like this:
 
             @contextmanager
             def run_context(self):
@@ -1344,26 +1344,29 @@
                   ... subclass context setup ...
                     yield
                 finally:
                   ... any unconditional cleanup ...
     '''
     # redundant try/finally to remind subclassers of correct structure
     try:
-      run_options = self.options.copy(**kw_options)
+      run_options = self.options.copy(runstate=runstate, **options_kw)
       with run_options:  # make the default ThreadState
-        with stackattrs(self, options=run_options):
-          with stackattrs(self, cmd=self._subcmd or self.cmd):
-            with upd:
-              with runstate:
-                with runstate.catch_signal(
-                    run_options.runstate_signals,
-                    call_previous=False,
-                    handle_signal=self.handle_signal,
-                ):
-                  yield
+        with stackattrs(
+            self,
+            options=run_options,
+            cmd=self._subcmd or self.cmd,
+        ):
+          with upd:
+            with runstate:
+              with runstate.catch_signal(
+                  run_options.runstate_signals,
+                  call_previous=False,
+                  handle_signal=self.handle_signal,
+              ):
+                yield
 
     finally:
       pass
 
   # pylint: disable=unused-argument
   @classmethod
   def cmd_help(cls, argv):
```

### Comparing `cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/PKG-INFO` & `cs.cmdutils-20240519/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.cmdutils
-Version: 20240422
+Version: 20240519
 Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -16,18 +16,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20240422*:
-* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
-* BaseCommand.apply_preargv: apply the default options supported by self.options.
-* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
+*Latest release 20240519*:
+BaseCommand.run_context: attach the runstate to the options.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -251,15 +249,15 @@
 this can be overridden with a method which just returns `False`.
 
 Otherwise,
 the handler may perform any suitable action
 and return `True` to contain the exception
 or `False` to cause the exception to be reraised.
 
-*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x104df9f30>)`*:
+*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10a199f30>)`*:
 The default signal handler, which cancels the default `RunState`.
 
 *Method `BaseCommand.poparg(argv: List[str], *a, unpop_on_error=False)`*:
 Pop the leading argument off `argv` and parse it.
 Return the parsed argument.
 Raises `getopt.GetoptError` on a missing or invalid argument.
 
@@ -447,15 +445,15 @@
 Otherwise `self.main(argv)` is called
 and its value returned.
 
 If the command implementation requires some setup or teardown
 then this may be provided by the `run_context()`
 context manager method.
 
-*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x104cea3b0>, **kw)`*:
+*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x10a2e64d0>, **kw)`*:
 The context manager which surrounds `main` or `cmd_`*subcmd*.
 
 This default does several things, and subclasses should
 override it like this:
 
     @contextmanager
     def run_context(self):
@@ -653,14 +651,17 @@
             print("doing f with x =", x)
         ....
 
 # Release Log
 
 
 
+*Release 20240519*:
+BaseCommand.run_context: attach the runstate to the options.
+
 *Release 20240422*:
 * BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
 * BaseCommand.apply_preargv: apply the default options supported by self.options.
 * BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
 
 *Release 20240412*:
 * BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
```

### Comparing `cs.cmdutils-20240422/pyproject.toml` & `cs.cmdutils-20240519/lib/python/cs.cmdutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,63 @@
-[project]
-name = "cs.cmdutils"
-description = "Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python2",
-    "python3",
-]
-dependencies = [
-    "cs.context>=20240412",
-    "cs.deco>=20240412",
-    "cs.lex>=20240316",
-    "cs.logutils>=20230212",
-    "cs.pfx>=20240412",
-    "cs.py.doc>=20240422",
-    "cs.resources>=20240422",
-    "cs.result>=20240412",
-    "cs.threads>=20240422",
-    "cs.typingutils>=20230331",
-    "cs.upd>=20240412",
-    "typeguard",
-]
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20240422"
+Metadata-Version: 2.1
+Name: cs.cmdutils
+Version: 20240519
+Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
 
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
-
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.readme]
-text = """
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20240422*:
-* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
-* BaseCommand.apply_preargv: apply the default options supported by self.options.
-* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
+*Latest release 20240519*:
+BaseCommand.run_context: attach the runstate to the options.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
 To implement a command line
 one instantiates a subclass of `BaseCommand`:
 
     class MyCommand(BaseCommand):
         GETOPT_SPEC = 'ab:c'
-        USAGE_FORMAT = r\"\"\"Usage: {cmd} [-a] [-b bvalue] [-c] [--] arguments...
+        USAGE_FORMAT = r"""Usage: {cmd} [-a] [-b bvalue] [-c] [--] arguments...
           -a    Do it all.
           -b    But using bvalue.
           -c    The 'c' option!
-        \"\"\"
+        """
         ...
 
 and provides either a `main` method if the command has no subcommands
 or a suite of `cmd_`*subcommand* methods, one per subcommand.
 
 Running a command is done by:
 
     MyCommand(argv).run()
 
 Modules which implement a command line mode generally look like this:
 
     ... imports etc ...
     def main(argv=None, **run_kw):
-        \"\"\" The command line mode.
-        \"\"\"
+        """ The command line mode.
+        """
         return MyCommand(argv).run(**run_kw)
     ... other code ...
     class MyCommand(BaseCommand):
     ... other code ...
     if __name__ == '__main__':
         sys.exit(main(sys.argv))
 
@@ -106,20 +79,20 @@
 Returning to methods, if there is a paragraph in the method docstring
 commencing with `Usage:`
 then that paragraph is incorporated automatically
 into the main usage message.
 Example:
 
     def cmd_ls(self, argv):
-        \"\"\" Usage: {cmd} [paths...]
+        """ Usage: {cmd} [paths...]
               Emit a listing for the named paths.
 
             Further docstring non-usage information here.
-        \"\"\"
-        ... do the \"ls\" subcommand ...
+        """
+        ... do the "ls" subcommand ...
 
 The subclass is customised by overriding the following methods:
 * `apply_opt(opt,val)`:
   apply an individual getopt global command line option
   to `self.options`.
 * `apply_opts(opts)`:
   apply the `opts` to `self.options`.
@@ -276,15 +249,15 @@
 this can be overridden with a method which just returns `False`.
 
 Otherwise,
 the handler may perform any suitable action
 and return `True` to contain the exception
 or `False` to cause the exception to be reraised.
 
-*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x104df9f30>)`*:
+*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10a199f30>)`*:
 The default signal handler, which cancels the default `RunState`.
 
 *Method `BaseCommand.poparg(argv: List[str], *a, unpop_on_error=False)`*:
 Pop the leading argument off `argv` and parse it.
 Return the parsed argument.
 Raises `getopt.GetoptError` on a missing or invalid argument.
 
@@ -309,49 +282,49 @@
   for values failing the validation
 * `unpop_on_error`: optional keyword parameter, default `False`;
   if true then push the argument back onto the front of `argv`
   if it fails to parse; `GetoptError` is still raised
 
 Typical use inside a `main` or `cmd_*` method might look like:
 
-    self.options.word = self.poparg(argv, int, \"a count value\")
+    self.options.word = self.poparg(argv, int, "a count value")
     self.options.word = self.poparg(
-        argv, int, \"a count value\",
-       lambda count: count > 0, \"count should be positive\")
+        argv, int, "a count value",
+       lambda count: count > 0, "count should be positive")
 
 Because it raises `GetoptError` on a bad argument
 the normal usage message failure mode follows automatically.
 
 Demonstration:
 
     >>> argv = ['word', '3', 'nine', '4']
-    >>> BaseCommand.poparg(argv, \"word to process\")
+    >>> BaseCommand.poparg(argv, "word to process")
     'word'
-    >>> BaseCommand.poparg(argv, int, \"count value\")
+    >>> BaseCommand.poparg(argv, int, "count value")
     3
-    >>> BaseCommand.poparg(argv, float, \"length\")
+    >>> BaseCommand.poparg(argv, float, "length")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: length 'nine': float('nine'): could not convert string to float: 'nine'
-    >>> BaseCommand.poparg(argv, float, \"width\", lambda width: width > 5)
+    >>> BaseCommand.poparg(argv, float, "width", lambda width: width > 5)
     Traceback (most recent call last):
       ...
     getopt.GetoptError: width '4': invalid value
-    >>> BaseCommand.poparg(argv, float, \"length\")
+    >>> BaseCommand.poparg(argv, float, "length")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: length: missing argument
     >>> argv = ['-5', 'zz']
-    >>> BaseCommand.poparg(argv, float, \"size\", lambda f: f>0, \"size should be >0\")
+    >>> BaseCommand.poparg(argv, float, "size", lambda f: f>0, "size should be >0")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: size '-5': size should be >0
     >>> argv  # -5 was still consumed
     ['zz']
-    >>> BaseCommand.poparg(argv, float, \"size2\", unpop_on_error=True)
+    >>> BaseCommand.poparg(argv, float, "size2", unpop_on_error=True)
     Traceback (most recent call last):
       ...
     getopt.GetoptError: size2 'zz': float('zz'): could not convert string to float: 'zz'
     >>> argv  # zz was pushed back
     ['zz']
 
 *Method `BaseCommand.popopts(argv, attrfor=None, **opt_specs)`*:
@@ -386,20 +359,20 @@
 
     class SomeCommand(BaseCommand):
 
         def cmd_foo(self, argv):
             options = self.options
             # accept a -j or --jobs options
             options.popopts(argv, jobs=1, j='jobs')
-            print(\"jobs =\", options.jobs)
+            print("jobs =", options.jobs)
 
 The `self.options` object is preprovided as an instance of
 the `self.Options` class, which is `BaseCommandOptions` by
 default. This presupplies support for some basic options
-like `-v` for \"verbose\" and so forth, and a subcommand
+like `-v` for "verbose" and so forth, and a subcommand
 need not describe these in a call to `self.options.popopts()`.
 
 Example:
 
     >>> import os.path
     >>> from typing import Optional
     >>> @dataclass
@@ -446,17 +419,17 @@
 * the attributes of `self`
 
 This is not presented automatically as a subcommand, but
 commands wishing such a command should provide something
 like this:
 
     def cmd_repl(self, argv):
-        \"\"\" Usage: {cmd}
+        """ Usage: {cmd}
               Run an interactive Python prompt with some predefined local names.
-        \"\"\"
+        """
         return self.repl(*argv)
 
 *Method `BaseCommand.run(self, **kw_options)`*:
 Run a command.
 Returns the exit status of the command.
 May raise `GetoptError` from subcommands.
 
@@ -472,15 +445,15 @@
 Otherwise `self.main(argv)` is called
 and its value returned.
 
 If the command implementation requires some setup or teardown
 then this may be provided by the `run_context()`
 context manager method.
 
-*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x104cea3b0>, **kw)`*:
+*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x10a2e64d0>, **kw)`*:
 The context manager which surrounds `main` or `cmd_`*subcmd*.
 
 This default does several things, and subclasses should
 override it like this:
 
     @contextmanager
     def run_context(self):
@@ -501,15 +474,15 @@
 
 *Method `BaseCommand.subcommands()`*:
 Return a mapping of subcommand names to subcommand specifications
 for class attributes which commence with `cls.SUBCOMMAND_METHOD_PREFIX`
 by default `'cmd_'`.
 
 *Method `BaseCommand.usage_text(*, cmd=None, format_mapping=None, subcmd=None, short=False)`*:
-Compute the \"Usage:\" message for this class
+Compute the "Usage:" message for this class
 from the top level `USAGE_FORMAT`
 and the `'Usage:'`-containing docstrings of its `cmd_*` methods.
 
 Parameters:
 * `cmd`: optional command name, default derived from the class name
 * `format_mapping`: an optional format mapping for filling
   in format strings in the usage text
@@ -595,15 +568,15 @@
     def cmd_foo(self, argv):
         self.options.popopts(
             c_='config',
             l='long',
             x='trace',
         )
         if self.options.dry_run:
-            print(\"dry run!\")
+            print("dry run!")
 
 The class attribute `COMMON_OPT_SPECS` is a mapping of
 options which are always supported. `BaseCommandOptions`
 has: `COMMON_OPT_SPECS={'n': 'dry_run', 'q': 'quiet', 'v': 'verbose'}`.
 
 A subclass with more common options might extend this like so,
 from `cs.hashindex`:
@@ -660,43 +633,46 @@
   provided its `cls.Options` class is used.
 * `options_param_name`: the parameter name to provide, default `options`
 
 Examples:
 
     @uses_cmd_options
     def f(x,*,options):
-        \"\"\" Run directly from the prevailing options. \"\"\"
+        """ Run directly from the prevailing options. """
         if options.verbose:
-            print(\"doing f with x =\", x)
+            print("doing f with x =", x)
         ....
 
     @uses_cmd_options
     def f(x,*,verbose=None,options):
-        \"\"\" Get defaults from the prevailing options. \"\"\"
+        """ Get defaults from the prevailing options. """
         if verbose is None:
             verbose = options.verbose
         if verbose:
-            print(\"doing f with x =\", x)
+            print("doing f with x =", x)
         ....
 
 # Release Log
 
 
 
+*Release 20240519*:
+BaseCommand.run_context: attach the runstate to the options.
+
 *Release 20240422*:
 * BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
 * BaseCommand.apply_preargv: apply the default options supported by self.options.
 * BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
 
 *Release 20240412*:
 * BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
 * BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
 
 *Release 20240316*:
-* New @uses_cmd_options decorator to provide an \"options\" parameter being the prevailing BaseCommandOptions instance.
+* New @uses_cmd_options decorator to provide an "options" parameter being the prevailing BaseCommandOptions instance.
 * BaseCommandOptions.popopts: get common options from BaseCommandOptions.COMMON_OPT_SPECS.
 
 *Release 20240211*:
 * Include the first sentence of the subcommand description in the short help.
 * BaseCommandOptions: move the runstate_signals into this directly.
 * BaseCommand: move the run() options stuff into run_context() and have it work on a copy of the original options.
 * BaseCommandCmd: implement get_names(), provide docstrings for the do_* attributes, thus help.
@@ -751,27 +727,27 @@
 * BaseCommand: new poparg(argv,...) compact validating argument consumer.
 * BaseCommand: drop run_argv, provided no utility.
 * BaseCommand.run: get the RunState signal list from self.options.runstate_signals.
 * BaseCommand.apply_opts: support multiple individual options raising GetoptError, as I hate commands which abort at the first bad option.
 * Assorted other small things.
 
 *Release 20220429*:
-* BaseCommand: fold dots in argv[0] into underscores, supports subcommands like \"setup.py\".
+* BaseCommand: fold dots in argv[0] into underscores, supports subcommands like "setup.py".
 * BaseCommand: new popargv(argv[,help_text[,parse[,validate[,unvalidated_message]]]]) helper class method.
 * BaseCommand: accept dashed-form of the underscored_form subcommand name.
 * BaseCommand: new self.options.runstate_signals=SIGINT,SIGTERM specifying singals to catch-and-cancel, shuffle run() context managers.
 
 *Release 20220318*:
 BaseCommand.__init__: handle main() method in the New Scheme.
 
 *Release 20220315*:
 _BaseSubCommand.__init__: hook in the class USAGE_KEYWORDS for methods.
 
 *Release 20220311*:
-BaseCommand: big refactor of subcommand internals and make the \"cmd_foo=FooCommand\" implementation work properly.
+BaseCommand: big refactor of subcommand internals and make the "cmd_foo=FooCommand" implementation work properly.
 
 *Release 20211208*:
 BaseCommand: better handle an unknown subcommand.
 
 *Release 20210927*:
 * Usage: show only the per subcommand usage for in-subcommand GetoptError.
 * Usage: show terse usage when the subcommand cannot be recognised.
@@ -786,57 +762,57 @@
 
 *Release 20210809*:
 Bugfix BaseCommand.cmd_help for modern API.
 
 *Release 20210731*:
 * BaseCommand.run: apply optional keyword arguments to self.options during the run.
 * Look for self.SUBCOMMAND_ARGV_DEFAULT if no subcommand is supplied.
-* Bugfix case for \"main\" method and no \"cmd_*\" methods.
+* Bugfix case for "main" method and no "cmd_*" methods.
 * Bugfix BaseCommand.cmd_help.
 
 *Release 20210420*:
 * BaseCommand.getopt_error_handler: replace error print() with warning().
 * Docstring improvements.
 
 *Release 20210407.1*:
 BaseCommand: bugfix for __init_subclass__ docstring update.
 
 *Release 20210407*:
 * BaseCommand.__init_subclass__: behave sanely if the subclass has no initial __doc__.
-* BaseCommand: new .run_argv convenience method, obviates the \"def main\" boilerplate.
+* BaseCommand: new .run_argv convenience method, obviates the "def main" boilerplate.
 
 *Release 20210404*:
 BaseCommand subclasses: automatically add the main usage message to the subclass docstring.
 
 *Release 20210306*:
 * BREAKING CHANGE: rework BaseCommand as a more normal class instantiated with argv and with most methods being instance methods, getting the former `options` parameter from self.options.
 * BaseCommand: provide default `apply_opt` and `apply_opts` methods; subclasses will generally just override the former.
 
 *Release 20210123*:
 BaseCommand: propagate the format mapping (cmd, USAGE_KEYWORDS) to the subusage generation.
 
 *Release 20201102*:
-* BaseCommand.cmd_help: supply usage only for \"all commands\", full docstring for specified commands.
+* BaseCommand.cmd_help: supply usage only for "all commands", full docstring for specified commands.
 * BaseCommand: honour presupplied options.log_level.
 * BaseCommand.usage_text: handle missing USAGE_FORMAT better.
 * BaseCommand.run: provide options.upd.
 * BaseCommand subclasses may now override BaseCommand.OPTIONS_CLASS (default SimpleNamespace) in order to provide convenience methods on the options.
 * BaseCommand.run: separate variable for subcmd with dash translated to underscore to match method names.
 * Minor fixes.
 
 *Release 20200615*:
-BaseCommand.usage_text: do not mention the \"help\" command if it is the only subcommand (it won't be available if there are no other subcommands).
+BaseCommand.usage_text: do not mention the "help" command if it is the only subcommand (it won't be available if there are no other subcommands).
 
 *Release 20200521.1*:
 Fix DISTINFO.install_requires.
 
 *Release 20200521*:
 * BaseCommand.run: support using BaseCommand subclasses as cmd_* names to make it easy to nest BaseCommands.
 * BaseCommand: new hack_postopts_argv method called after parsing the main command line options, for inferring subcommands or the like.
-* BaseCommand: extract \"Usage:\" paragraphs from subcommand method docstrings to build the main usage message.
+* BaseCommand: extract "Usage:" paragraphs from subcommand method docstrings to build the main usage message.
 * BaseCommand: new cmd_help default command.
 * Assorted bugfixes and small improvements.
 
 *Release 20200318*:
 * BaseCommand.run: make argv optional, get additional usage keywords from self.USAGE_KEYWORDS.
 * @BaseCommand.add_usage_to_docstring: honour cls.USAGE_KEYWORDS.
 * BaseCommand: do not require GETOPT_SPEC for commands with no defined options.
@@ -858,25 +834,9 @@
 *Release 20190619*:
 Minor documentation updates.
 
 *Release 20190617.2*:
 Lint.
 
 *Release 20190617.1*:
-Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class."""
-content-type = "text/markdown"
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-
-[tool.setuptools]
-py-modules = [
-    "cs.cmdutils",
-]
+Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class.
 
-[tool.setuptools.package-dir]
-"" = "lib/python"
```

