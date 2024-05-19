# Comparing `tmp/cs.lex-20240316.tar.gz` & `tmp/cs.lex-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.lex-20240316.tar", last modified: Sat Mar 16 06:59:18 2024, max compression
+gzip compressed data, was "cs.lex-20240519.tar", last modified: Sun May 19 02:14:18 2024, max compression
```

## Comparing `cs.lex-20240316.tar` & `cs.lex-20240519.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:18.270111 cs.lex-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:58:46.000000 cs.lex-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    29939 2024-03-16 06:59:18.269698 cs.lex-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    34434 2024-03-16 06:58:56.000000 cs.lex-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:18.264630 cs.lex-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:18.264890 cs.lex-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:18.266217 cs.lex-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    63151 2024-03-16 06:58:36.000000 cs.lex-20240316/lib/python/cs/lex.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:18.269156 cs.lex-20240316/lib/python/cs.lex.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    29939 2024-03-16 06:59:17.000000 cs.lex-20240316/lib/python/cs.lex.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      261 2024-03-16 06:59:18.000000 cs.lex-20240316/lib/python/cs.lex.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:59:17.000000 cs.lex-20240316/lib/python/cs.lex.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      154 2024-03-16 06:59:18.000000 cs.lex-20240316/lib/python/cs.lex.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:59:18.000000 cs.lex-20240316/lib/python/cs.lex.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    30513 2024-03-16 06:59:16.000000 cs.lex-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:59:18.270221 cs.lex-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:14:18.794865 cs.lex-20240519/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-19 02:13:44.000000 cs.lex-20240519/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    35932 2024-05-19 02:14:18.794427 cs.lex-20240519/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    34921 2024-05-19 02:13:55.000000 cs.lex-20240519/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:14:18.788799 cs.lex-20240519/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:14:18.789198 cs.lex-20240519/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:14:18.791157 cs.lex-20240519/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    65001 2024-05-19 02:13:28.000000 cs.lex-20240519/lib/python/cs/lex.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:14:18.793714 cs.lex-20240519/lib/python/cs.lex.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    35932 2024-05-19 02:14:18.000000 cs.lex-20240519/lib/python/cs.lex.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      261 2024-05-19 02:14:18.000000 cs.lex-20240519/lib/python/cs.lex.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-19 02:14:18.000000 cs.lex-20240519/lib/python/cs.lex.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      154 2024-05-19 02:14:18.000000 cs.lex-20240519/lib/python/cs.lex.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-19 02:14:18.000000 cs.lex-20240519/lib/python/cs.lex.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    36512 2024-05-19 02:14:17.000000 cs.lex-20240519/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-19 02:14:18.795073 cs.lex-20240519/setup.cfg
```

### Comparing `cs.lex-20240316/PKG-INFO` & `cs.lex-20240519/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,15 @@
-Metadata-Version: 2.1
-Name: cs.lex
-Version: 20240316
-Summary: Lexical analysis functions, tokenisers, transcribers: an arbitrary assortment of lexical and tokenisation functions useful for writing recursive descent parsers, of which I have several. There are also some transcription functions for producing text from various objects, such as `hexify` and `unctrl`.
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
 Lexical analysis functions, tokenisers, transcribers:
 an arbitrary assortment of lexical and tokenisation functions useful
 for writing recursive descent parsers, of which I have several.
 There are also some transcription functions for producing text
 from various objects, such as `hexify` and `unctrl`.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240519*:
+New get_suffix_part() to extract things line ": Part One" from something such as a TV episode name.
 
 Generally the get_* functions accept a source string and an offset
 (usually optional, default `0`) and return a token and the new offset,
 raising `ValueError` on failed tokenisation.
 
 ## Function `as_lines(chunks, partials=None)`
 
@@ -125,26 +107,32 @@
     >>> cutsuffix(abc_def, '.def')
     'abc'
     >>> cutsuffix(abc_def, '.zzz')
     'abc.def'
     >>> cutsuffix(abc_def, '.zzz') is abc_def
     True
 
-## Class `FFloat(FNumericMixin, FormatableMixin, FormatableFormatter, string.Formatter, builtins.float)`
+## Class `FFloat(FNumericMixin, builtins.float)`
 
 Formattable `float`.
 
-## Class `FInt(FNumericMixin, FormatableMixin, FormatableFormatter, string.Formatter, builtins.int)`
+## Class `FInt(FNumericMixin, builtins.int)`
 
 Formattable `int`.
 
-## Class `FNumericMixin(FormatableMixin, FormatableFormatter, string.Formatter)`
+## Class `FNumericMixin(FormatableMixin)`
 
 A `FormatableMixin` subclass.
 
+*Method `FNumericMixin.localtime(self)`*:
+Treat this as a UNIX timestamp and return a localtime `datetime`.
+
+*Method `FNumericMixin.utctime(self)`*:
+Treat this as a UNIX timestamp and return a UTC `datetime`.
+
 ## Function `format_as(format_s: str, format_mapping, formatter=None, error_sep=None, strict=None)`
 
 Format the string `format_s` using `Formatter.vformat`,
 return the formatted result.
 This is a wrapper for `str.format_map`
 which raises a more informative `FormatAsError` exception on failure.
 
@@ -196,15 +184,64 @@
 with `{self:format_spec}`.
 
 ## Class `FormatableFormatter(string.Formatter)`
 
 A `string.Formatter` subclass interacting with objects
 which inherit from `FormatableMixin`.
 
-## Class `FormatableMixin(FormatableFormatter, string.Formatter)`
+*Method `FormatableFormatter.format_field(value, format_spec: str)`*:
+Format a value using `value.format_format_field`,
+returning an `FStr`
+(a `str` subclass with additional `format_spec` features).
+
+We actually recognise colon separated chains of formats
+and apply each format to the previously converted value.
+The final result is promoted to an `FStr` before return.
+
+*Property `FormatableFormatter.format_mode`*:
+Thread local state object.
+
+Attributes:
+* `strict`: initially `False`; raise a `KeyError` for
+  unresolveable field names
+
+*Method `FormatableFormatter.get_arg_name(field_name)`*:
+Default initial arg_name is an identifier.
+
+Returns `(prefix,offset)`, and `('',0)` if there is no arg_name.
+
+*Method `FormatableFormatter.get_field(self, field_name, args, kwargs)`*:
+Get the object referenced by the field text `field_name`.
+Raises `KeyError` for an unknown `field_name`.
+
+*Method `FormatableFormatter.get_format_subspecs(format_spec)`*:
+Parse a `format_spec` as a sequence of colon separated components,
+return a list of the components.
+
+*Method `FormatableFormatter.get_subfield(value, subfield_text: str)`*:
+Resolve `value` against `subfield_text`,
+the remaining field text after the term which resolved to `value`.
+
+For example, a format `{name.blah[0]}`
+has the field text `name.blah[0]`.
+A `get_field` implementation might initially
+resolve `name` to some value,
+leaving `.blah[0]` as the `subfield_text`.
+This method supports taking that value
+and resolving it against the remaining text `.blah[0]`.
+
+For generality, if `subfield_text` is the empty string
+`value` is returned unchanged.
+
+*Method `FormatableFormatter.get_value(self, arg_name, args, kwargs)`*:
+Get the object with index `arg_name`.
+
+This default implementation returns `(kwargs[arg_name],arg_name)`.
+
+## Class `FormatableMixin(FormatableFormatter)`
 
 A subclass of `FormatableFormatter` which  provides 2 features:
 - a `__format__` method which parses the `format_spec` string
   into multiple colon separated terms whose results chain
 - a `format_as` method which formats a format string using `str.format_map`
   with a suitable mapping derived from the instance
   via its `format_kwargs` method
@@ -232,27 +269,125 @@
   terms with no colons, letting `format_field` do the split into terms
 - override `FormatableFormatter.get_format_subspecs` to implement
   the parse of `format_spec` into a sequence of terms.
   This might recognise a special additional syntax
   and quietly fall back to `super().get_format_subspecs`
   if that is not present.
 
-## Class `FormatAsError(builtins.LookupError, builtins.Exception, builtins.BaseException)`
+*Method `FormatableMixin.__format__(self, format_spec)`*:
+Format `self` according to `format_spec`.
+
+This implementation calls `self.format_field`.
+As such, a `format_spec` is considered
+a sequence of colon separated terms.
+
+Classes wanting to implement additional format string syntaxes
+should either:
+- override `FormatableFormatter.format_field1` to implement
+  terms with no colons, letting `format_field1` do the split into terms
+- override `FormatableFormatter.get_format_subspecs` to implement
+  the term parse.
+
+The default implementation of `__format1__` just calls `super().__format__`.
+Implementations providing specialised formats
+should implement them in `__format1__`
+with fallback to `super().__format1__`.
+
+*Method `FormatableMixin.convert_field(self, value, conversion)`*:
+The default converter for fields calls `Formatter.convert_field`.
+
+*Method `FormatableMixin.convert_via_method_or_attr(self, value, format_spec)`*:
+Apply a method or attribute name based conversion to `value`
+where `format_spec` starts with a method name
+applicable to `value`.
+Return `(converted,offset)`
+being the converted value and the offset after the method name.
+
+Note that if there is not a leading identifier on `format_spec`
+then `value` is returned unchanged with `offset=0`.
+
+The methods/attributes are looked up in the mapping
+returned by `.format_attributes()` which represents allowed methods
+(broadly, one should not allow methods which modify any state).
+
+If this returns a callable, it is called to obtain the converted value
+otherwise it is used as is.
+
+As a final tweak,
+if `value.get_format_attribute()` raises an `AttributeError`
+(the attribute is not an allowed attribute)
+or calling the attribute raises a `TypeError`
+(the `value` isn't suitable)
+and the `value` is not an instance of `FStr`,
+convert it to an `FStr` and try again.
+This provides the common utility methods on other types.
+
+The motivating example was a `PurePosixPath`,
+which does not JSON transcribe;
+this tweak supports both
+`posixpath:basename` via the pathlib stuff
+and `posixpath:json` via `FStr`
+even though a `PurePosixPath` does not subclass `FStr`.
+
+*Method `FormatableMixin.format_as(self, format_s, error_sep=None, strict=None, **control_kw)`*:
+Return the string `format_s` formatted using the mapping
+returned by `self.format_kwargs(**control_kw)`.
+
+If a class using the mixin has no `format_kwargs(**control_kw)` method
+to provide a mapping for `str.format_map`
+then the instance itself is used as the mapping.
+
+*Method `FormatableMixin.get_format_attribute(self, attr)`*:
+Return a mapping of permitted methods to functions of an instance.
+This is used to whitelist allowed `:`*name* method formats
+to prevent scenarios like little Bobby Tables calling `delete()`.
+
+*Method `FormatableMixin.get_format_attributes()`*:
+Return the mapping of format attributes.
+
+*Method `FormatableMixin.json(self)`*:
+The value transcribed as compact JSON.
+
+## Class `FormatAsError(builtins.LookupError)`
 
 Subclass of `LookupError` for use by `format_as`.
 
-## Class `FStr(FormatableMixin, FormatableFormatter, string.Formatter, builtins.str)`
+## Class `FStr(FormatableMixin, builtins.str)`
 
 A `str` subclass with the `FormatableMixin` methods,
 particularly its `__format__` method
 which uses `str` method names as valid formats.
 
 It also has a bunch of utility methods which are available
 as `:`*method* in format strings.
 
+*Method `FStr.basename(self)`*:
+Treat as a filesystem path and return the basename.
+
+*Method `FStr.dirname(self)`*:
+Treat as a filesystem path and return the dirname.
+
+*Method `FStr.f(self)`*:
+Parse `self` as a `float`.
+
+*Method `FStr.i(self, base=10)`*:
+Parse `self` as an `int`.
+
+*Method `FStr.lc(self)`*:
+Lowercase using `lc_()`.
+
+*Method `FStr.path(self)`*:
+Convert to a native filesystem `pathlib.Path`.
+
+*Method `FStr.posix_path(self)`*:
+Convert to a Posix filesystem `pathlib.Path`.
+
+*Method `FStr.windows_path(self)`*:
+Convert to a Windows filesystem `pathlib.Path`.
+
 ## Function `get_chars(s, offset, gochars)`
 
 Scan the string `s` for characters in `gochars` starting at `offset`.
 Return `(match,new_offset)`.
 
 `gochars` may also be a callable, in which case a character
 `ch` is accepted if `gochars(ch)` is true.
@@ -407,15 +542,15 @@
 * `environ`: if not `None`, also parse and expand `$`*envvar* references.
 * `default`: passed to `get_envvar`
 
 ## Function `get_qstr_or_identifier(s, offset)`
 
 Parse a double quoted string or an identifier.
 
-## Function `get_sloshed_text(s, delim, offset=0, slosh='\\', mapper=<function slosh_mapper at 0x104903eb0>, specials=None)`
+## Function `get_sloshed_text(s, delim, offset=0, slosh='\\', mapper=<function slosh_mapper at 0x102494550>, specials=None)`
 
 Collect slosh escaped text from the string `s` from position
 `offset` (default `0`) and return the decoded unicode string and
 the offset of the completed parse.
 
 Parameters:
 * `delim`: end of string delimiter, such as a single or double quote.
@@ -442,14 +577,32 @@
   2 hexadecimal digits.
 * the character 'u', insert the character with code from the following
   4 hexadecimal digits.
 * the character 'U', insert the character with code from the following
   8 hexadecimal digits.
 * a character from the keys of `mapper`
 
+## Function `get_suffix_part(s, *, keywords=('part',), numeral_map=None)`
+
+Strip a trailing "part N" suffix from the string `s`.
+Return the matched suffix and the number part number.
+Retrn `(None,None)` on no match.
+
+Parameters:
+* `s`: the string
+* `keywords`: an iterable of `str` to match, or a single `str`;
+  default `'part'`
+* `numeral_map`: an optional mapping of numeral names to numeric values;
+  default `NUMERAL_NAMES['en']`, the English numerals
+
+Exanmple:
+
+    >>> get_suffix_part('s09e10 - A New World: Part One')
+    (': Part One', 1)
+
 ## Function `get_tokens(s, offset, getters)`
 
 Parse the string `s` from position `offset` using the supplied
 tokeniser functions `getters`.
 Return the list of tokens matched and the final offset.
 
 Parameters:
@@ -747,14 +900,17 @@
 * `shiftout`: Optional. The marker string ending a sequence
   of direct text transcription, default `']'`.
 
 # Release Log
 
 
 
+*Release 20240519*:
+New get_suffix_part() to extract things line ": Part One" from something such as a TV episode name.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240211*:
 New split_remote_path() function to recognise [[user@]host]:path.
 
 *Release 20231018*:
@@ -872,8 +1028,7 @@
 cs.lex: texthexify: backport to python 2 using cs.py3 bytes type
 
 *Release 20150118*:
 metadata updates
 
 *Release 20150116*:
 PyPI metadata and slight code cleanup.
-
```

### Comparing `cs.lex-20240316/README.md` & `cs.lex-20240519/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,33 @@
+Metadata-Version: 2.1
+Name: cs.lex
+Version: 20240519
+Summary: Lexical analysis functions, tokenisers, transcribers: an arbitrary assortment of lexical and tokenisation functions useful for writing recursive descent parsers, of which I have several. There are also some transcription functions for producing text from various objects, such as `hexify` and `unctrl`.
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
+
 Lexical analysis functions, tokenisers, transcribers:
 an arbitrary assortment of lexical and tokenisation functions useful
 for writing recursive descent parsers, of which I have several.
 There are also some transcription functions for producing text
 from various objects, such as `hexify` and `unctrl`.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240519*:
+New get_suffix_part() to extract things line ": Part One" from something such as a TV episode name.
 
 Generally the get_* functions accept a source string and an offset
 (usually optional, default `0`) and return a token and the new offset,
 raising `ValueError` on failed tokenisation.
 
 ## Function `as_lines(chunks, partials=None)`
 
@@ -107,23 +125,23 @@
     >>> cutsuffix(abc_def, '.def')
     'abc'
     >>> cutsuffix(abc_def, '.zzz')
     'abc.def'
     >>> cutsuffix(abc_def, '.zzz') is abc_def
     True
 
-## Class `FFloat(FNumericMixin, FormatableMixin, FormatableFormatter, string.Formatter, builtins.float)`
+## Class `FFloat(FNumericMixin, builtins.float)`
 
 Formattable `float`.
 
-## Class `FInt(FNumericMixin, FormatableMixin, FormatableFormatter, string.Formatter, builtins.int)`
+## Class `FInt(FNumericMixin, builtins.int)`
 
 Formattable `int`.
 
-## Class `FNumericMixin(FormatableMixin, FormatableFormatter, string.Formatter)`
+## Class `FNumericMixin(FormatableMixin)`
 
 A `FormatableMixin` subclass.
 
 *Method `FNumericMixin.localtime(self)`*:
 Treat this as a UNIX timestamp and return a localtime `datetime`.
 
 *Method `FNumericMixin.utctime(self)`*:
@@ -233,15 +251,15 @@
 `value` is returned unchanged.
 
 *Method `FormatableFormatter.get_value(self, arg_name, args, kwargs)`*:
 Get the object with index `arg_name`.
 
 This default implementation returns `(kwargs[arg_name],arg_name)`.
 
-## Class `FormatableMixin(FormatableFormatter, string.Formatter)`
+## Class `FormatableMixin(FormatableFormatter)`
 
 A subclass of `FormatableFormatter` which  provides 2 features:
 - a `__format__` method which parses the `format_spec` string
   into multiple colon separated terms whose results chain
 - a `format_as` method which formats a format string using `str.format_map`
   with a suitable mapping derived from the instance
   via its `format_kwargs` method
@@ -343,19 +361,19 @@
 
 *Method `FormatableMixin.get_format_attributes()`*:
 Return the mapping of format attributes.
 
 *Method `FormatableMixin.json(self)`*:
 The value transcribed as compact JSON.
 
-## Class `FormatAsError(builtins.LookupError, builtins.Exception, builtins.BaseException)`
+## Class `FormatAsError(builtins.LookupError)`
 
 Subclass of `LookupError` for use by `format_as`.
 
-## Class `FStr(FormatableMixin, FormatableFormatter, string.Formatter, builtins.str)`
+## Class `FStr(FormatableMixin, builtins.str)`
 
 A `str` subclass with the `FormatableMixin` methods,
 particularly its `__format__` method
 which uses `str` method names as valid formats.
 
 It also has a bunch of utility methods which are available
 as `:`*method* in format strings.
@@ -542,15 +560,15 @@
 * `environ`: if not `None`, also parse and expand `$`*envvar* references.
 * `default`: passed to `get_envvar`
 
 ## Function `get_qstr_or_identifier(s, offset)`
 
 Parse a double quoted string or an identifier.
 
-## Function `get_sloshed_text(s, delim, offset=0, slosh='\\', mapper=<function slosh_mapper at 0x104903eb0>, specials=None)`
+## Function `get_sloshed_text(s, delim, offset=0, slosh='\\', mapper=<function slosh_mapper at 0x102494550>, specials=None)`
 
 Collect slosh escaped text from the string `s` from position
 `offset` (default `0`) and return the decoded unicode string and
 the offset of the completed parse.
 
 Parameters:
 * `delim`: end of string delimiter, such as a single or double quote.
@@ -577,14 +595,32 @@
   2 hexadecimal digits.
 * the character 'u', insert the character with code from the following
   4 hexadecimal digits.
 * the character 'U', insert the character with code from the following
   8 hexadecimal digits.
 * a character from the keys of `mapper`
 
+## Function `get_suffix_part(s, *, keywords=('part',), numeral_map=None)`
+
+Strip a trailing "part N" suffix from the string `s`.
+Return the matched suffix and the number part number.
+Retrn `(None,None)` on no match.
+
+Parameters:
+* `s`: the string
+* `keywords`: an iterable of `str` to match, or a single `str`;
+  default `'part'`
+* `numeral_map`: an optional mapping of numeral names to numeric values;
+  default `NUMERAL_NAMES['en']`, the English numerals
+
+Exanmple:
+
+    >>> get_suffix_part('s09e10 - A New World: Part One')
+    (': Part One', 1)
+
 ## Function `get_tokens(s, offset, getters)`
 
 Parse the string `s` from position `offset` using the supplied
 tokeniser functions `getters`.
 Return the list of tokens matched and the final offset.
 
 Parameters:
@@ -882,14 +918,17 @@
 * `shiftout`: Optional. The marker string ending a sequence
   of direct text transcription, default `']'`.
 
 # Release Log
 
 
 
+*Release 20240519*:
+New get_suffix_part() to extract things line ": Part One" from something such as a TV episode name.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240211*:
 New split_remote_path() function to recognise [[user@]host]:path.
 
 *Release 20231018*:
@@ -1007,7 +1046,8 @@
 cs.lex: texthexify: backport to python 2 using cs.py3 bytes type
 
 *Release 20150118*:
 metadata updates
 
 *Release 20150116*:
 PyPI metadata and slight code cleanup.
+
```

### Comparing `cs.lex-20240316/lib/python/cs/lex.py` & `cs.lex-20240519/lib/python/cs/lex.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from cs.dateutils import unixtime2datetime, UTC
 from cs.deco import fmtdoc, decorator
 from cs.gimmicks import warning
 from cs.pfx import Pfx, pfx_call, pfx_method
 from cs.py.func import funcname
 from cs.seq import common_prefix_length, common_suffix_length
 
-__version__ = '20240316'
+__version__ = '20240519'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -488,14 +488,89 @@
   if offset >= len(s) or not s[offset].isdigit():
     return no_match
   gn, offset = get_decimal_value(s, offset)
   if n is not None and gn != n:
     return no_match
   return matched, gn, offset
 
+NUMERAL_NAMES = {
+    'en': {
+        # all the single word numbers
+        'zero': 0,
+        'nought': 0,
+        'one': 1,
+        'two': 2,
+        'three': 3,
+        'four': 4,
+        'five': 5,
+        'six': 6,
+        'seven': 7,
+        'eight': 8,
+        'nine': 9,
+        'ten': 10,
+        'eleven': 11,
+        'twelve': 12,
+        'thirteen': 13,
+        'fourteen': 14,
+        'fifteen': 15,
+        'sixteen': 16,
+        'seventeen': 17,
+        'eighteen': 18,
+        'nineteen': 19,
+        'twenty': 20,
+    },
+}
+
+def get_suffix_part(s, *, keywords=('part',), numeral_map=None):
+  ''' Strip a trailing "part N" suffix from the string `s`.
+      Return the matched suffix and the number part number.
+      Retrn `(None,None)` on no match.
+
+      Parameters:
+      * `s`: the string
+      * `keywords`: an iterable of `str` to match, or a single `str`;
+        default `'part'`
+      * `numeral_map`: an optional mapping of numeral names to numeric values;
+        default `NUMERAL_NAMES['en']`, the English numerals
+
+      Exanmple:
+
+          >>> get_suffix_part('s09e10 - A New World: Part One')
+          (': Part One', 1)
+  '''
+  if isinstance(keywords, str):
+    keywords = (keywords,)
+  if numeral_map is None:
+    numeral_map = NUMERAL_NAMES['en']
+  regexp_s = ''.join(
+      (
+          r'\W+(',
+          r'|'.join(keywords),
+          r')\s+(?P<numeral>\d+|',
+          r'|'.join(numeral_map.keys()),
+          r')\s*$',
+      )
+  )
+  regexp = re.compile(regexp_s, re.I)
+  m = regexp.search(s)
+  if not m:
+    return None, None
+  numeral = m.group('numeral')
+  try:
+    part_n = int(numeral)
+  except ValueError:
+    try:
+      part_n = numeral_map[numeral]
+    except KeyError:
+      try:
+        part_n = numeral_map[numeral.lower()]
+      except KeyError:
+        return None, None
+  return m.group(0), part_n
+
 # pylint: disable=redefined-outer-name
 def get_nonwhite(s, offset=0):
   ''' Scan the string `s` for characters not in `string.whitespace`
       starting at `offset` (default `0`).
       Return `(match,new_offset)`.
   '''
   return get_other_chars(s, offset=offset, stopchars=whitespace)
```

### Comparing `cs.lex-20240316/lib/python/cs.lex.egg-info/PKG-INFO` & `cs.lex-20240519/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,55 @@
-Metadata-Version: 2.1
-Name: cs.lex
-Version: 20240316
-Summary: Lexical analysis functions, tokenisers, transcribers: an arbitrary assortment of lexical and tokenisation functions useful for writing recursive descent parsers, of which I have several. There are also some transcription functions for producing text from various objects, such as `hexify` and `unctrl`.
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
+[project]
+name = "cs.lex"
+description = "Lexical analysis functions, tokenisers, transcribers: an arbitrary assortment of lexical and tokenisation functions useful for writing recursive descent parsers, of which I have several. There are also some transcription functions for producing text from various objects, such as `hexify` and `unctrl`."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.dateutils>=20230210",
+    "cs.deco>=20240412",
+    "cs.gimmicks>=20240316",
+    "cs.pfx>=20240412",
+    "cs.py.func>=20230331",
+    "cs.seq>=20200914",
+    "icontract",
+    "python-dateutil",
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
 
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
 Lexical analysis functions, tokenisers, transcribers:
 an arbitrary assortment of lexical and tokenisation functions useful
 for writing recursive descent parsers, of which I have several.
 There are also some transcription functions for producing text
 from various objects, such as `hexify` and `unctrl`.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240519*:
+New get_suffix_part() to extract things line \": Part One\" from something such as a TV episode name.
 
 Generally the get_* functions accept a source string and an offset
 (usually optional, default `0`) and return a token and the new offset,
 raising `ValueError` on failed tokenisation.
 
 ## Function `as_lines(chunks, partials=None)`
 
@@ -125,26 +147,32 @@
     >>> cutsuffix(abc_def, '.def')
     'abc'
     >>> cutsuffix(abc_def, '.zzz')
     'abc.def'
     >>> cutsuffix(abc_def, '.zzz') is abc_def
     True
 
-## Class `FFloat(FNumericMixin, FormatableMixin, FormatableFormatter, string.Formatter, builtins.float)`
+## Class `FFloat(FNumericMixin, builtins.float)`
 
 Formattable `float`.
 
-## Class `FInt(FNumericMixin, FormatableMixin, FormatableFormatter, string.Formatter, builtins.int)`
+## Class `FInt(FNumericMixin, builtins.int)`
 
 Formattable `int`.
 
-## Class `FNumericMixin(FormatableMixin, FormatableFormatter, string.Formatter)`
+## Class `FNumericMixin(FormatableMixin)`
 
 A `FormatableMixin` subclass.
 
+*Method `FNumericMixin.localtime(self)`*:
+Treat this as a UNIX timestamp and return a localtime `datetime`.
+
+*Method `FNumericMixin.utctime(self)`*:
+Treat this as a UNIX timestamp and return a UTC `datetime`.
+
 ## Function `format_as(format_s: str, format_mapping, formatter=None, error_sep=None, strict=None)`
 
 Format the string `format_s` using `Formatter.vformat`,
 return the formatted result.
 This is a wrapper for `str.format_map`
 which raises a more informative `FormatAsError` exception on failure.
 
@@ -196,15 +224,64 @@
 with `{self:format_spec}`.
 
 ## Class `FormatableFormatter(string.Formatter)`
 
 A `string.Formatter` subclass interacting with objects
 which inherit from `FormatableMixin`.
 
-## Class `FormatableMixin(FormatableFormatter, string.Formatter)`
+*Method `FormatableFormatter.format_field(value, format_spec: str)`*:
+Format a value using `value.format_format_field`,
+returning an `FStr`
+(a `str` subclass with additional `format_spec` features).
+
+We actually recognise colon separated chains of formats
+and apply each format to the previously converted value.
+The final result is promoted to an `FStr` before return.
+
+*Property `FormatableFormatter.format_mode`*:
+Thread local state object.
+
+Attributes:
+* `strict`: initially `False`; raise a `KeyError` for
+  unresolveable field names
+
+*Method `FormatableFormatter.get_arg_name(field_name)`*:
+Default initial arg_name is an identifier.
+
+Returns `(prefix,offset)`, and `('',0)` if there is no arg_name.
+
+*Method `FormatableFormatter.get_field(self, field_name, args, kwargs)`*:
+Get the object referenced by the field text `field_name`.
+Raises `KeyError` for an unknown `field_name`.
+
+*Method `FormatableFormatter.get_format_subspecs(format_spec)`*:
+Parse a `format_spec` as a sequence of colon separated components,
+return a list of the components.
+
+*Method `FormatableFormatter.get_subfield(value, subfield_text: str)`*:
+Resolve `value` against `subfield_text`,
+the remaining field text after the term which resolved to `value`.
+
+For example, a format `{name.blah[0]}`
+has the field text `name.blah[0]`.
+A `get_field` implementation might initially
+resolve `name` to some value,
+leaving `.blah[0]` as the `subfield_text`.
+This method supports taking that value
+and resolving it against the remaining text `.blah[0]`.
+
+For generality, if `subfield_text` is the empty string
+`value` is returned unchanged.
+
+*Method `FormatableFormatter.get_value(self, arg_name, args, kwargs)`*:
+Get the object with index `arg_name`.
+
+This default implementation returns `(kwargs[arg_name],arg_name)`.
+
+## Class `FormatableMixin(FormatableFormatter)`
 
 A subclass of `FormatableFormatter` which  provides 2 features:
 - a `__format__` method which parses the `format_spec` string
   into multiple colon separated terms whose results chain
 - a `format_as` method which formats a format string using `str.format_map`
   with a suitable mapping derived from the instance
   via its `format_kwargs` method
@@ -232,27 +309,125 @@
   terms with no colons, letting `format_field` do the split into terms
 - override `FormatableFormatter.get_format_subspecs` to implement
   the parse of `format_spec` into a sequence of terms.
   This might recognise a special additional syntax
   and quietly fall back to `super().get_format_subspecs`
   if that is not present.
 
-## Class `FormatAsError(builtins.LookupError, builtins.Exception, builtins.BaseException)`
+*Method `FormatableMixin.__format__(self, format_spec)`*:
+Format `self` according to `format_spec`.
+
+This implementation calls `self.format_field`.
+As such, a `format_spec` is considered
+a sequence of colon separated terms.
+
+Classes wanting to implement additional format string syntaxes
+should either:
+- override `FormatableFormatter.format_field1` to implement
+  terms with no colons, letting `format_field1` do the split into terms
+- override `FormatableFormatter.get_format_subspecs` to implement
+  the term parse.
+
+The default implementation of `__format1__` just calls `super().__format__`.
+Implementations providing specialised formats
+should implement them in `__format1__`
+with fallback to `super().__format1__`.
+
+*Method `FormatableMixin.convert_field(self, value, conversion)`*:
+The default converter for fields calls `Formatter.convert_field`.
+
+*Method `FormatableMixin.convert_via_method_or_attr(self, value, format_spec)`*:
+Apply a method or attribute name based conversion to `value`
+where `format_spec` starts with a method name
+applicable to `value`.
+Return `(converted,offset)`
+being the converted value and the offset after the method name.
+
+Note that if there is not a leading identifier on `format_spec`
+then `value` is returned unchanged with `offset=0`.
+
+The methods/attributes are looked up in the mapping
+returned by `.format_attributes()` which represents allowed methods
+(broadly, one should not allow methods which modify any state).
+
+If this returns a callable, it is called to obtain the converted value
+otherwise it is used as is.
+
+As a final tweak,
+if `value.get_format_attribute()` raises an `AttributeError`
+(the attribute is not an allowed attribute)
+or calling the attribute raises a `TypeError`
+(the `value` isn't suitable)
+and the `value` is not an instance of `FStr`,
+convert it to an `FStr` and try again.
+This provides the common utility methods on other types.
+
+The motivating example was a `PurePosixPath`,
+which does not JSON transcribe;
+this tweak supports both
+`posixpath:basename` via the pathlib stuff
+and `posixpath:json` via `FStr`
+even though a `PurePosixPath` does not subclass `FStr`.
+
+*Method `FormatableMixin.format_as(self, format_s, error_sep=None, strict=None, **control_kw)`*:
+Return the string `format_s` formatted using the mapping
+returned by `self.format_kwargs(**control_kw)`.
+
+If a class using the mixin has no `format_kwargs(**control_kw)` method
+to provide a mapping for `str.format_map`
+then the instance itself is used as the mapping.
+
+*Method `FormatableMixin.get_format_attribute(self, attr)`*:
+Return a mapping of permitted methods to functions of an instance.
+This is used to whitelist allowed `:`*name* method formats
+to prevent scenarios like little Bobby Tables calling `delete()`.
+
+*Method `FormatableMixin.get_format_attributes()`*:
+Return the mapping of format attributes.
+
+*Method `FormatableMixin.json(self)`*:
+The value transcribed as compact JSON.
+
+## Class `FormatAsError(builtins.LookupError)`
 
 Subclass of `LookupError` for use by `format_as`.
 
-## Class `FStr(FormatableMixin, FormatableFormatter, string.Formatter, builtins.str)`
+## Class `FStr(FormatableMixin, builtins.str)`
 
 A `str` subclass with the `FormatableMixin` methods,
 particularly its `__format__` method
 which uses `str` method names as valid formats.
 
 It also has a bunch of utility methods which are available
 as `:`*method* in format strings.
 
+*Method `FStr.basename(self)`*:
+Treat as a filesystem path and return the basename.
+
+*Method `FStr.dirname(self)`*:
+Treat as a filesystem path and return the dirname.
+
+*Method `FStr.f(self)`*:
+Parse `self` as a `float`.
+
+*Method `FStr.i(self, base=10)`*:
+Parse `self` as an `int`.
+
+*Method `FStr.lc(self)`*:
+Lowercase using `lc_()`.
+
+*Method `FStr.path(self)`*:
+Convert to a native filesystem `pathlib.Path`.
+
+*Method `FStr.posix_path(self)`*:
+Convert to a Posix filesystem `pathlib.Path`.
+
+*Method `FStr.windows_path(self)`*:
+Convert to a Windows filesystem `pathlib.Path`.
+
 ## Function `get_chars(s, offset, gochars)`
 
 Scan the string `s` for characters in `gochars` starting at `offset`.
 Return `(match,new_offset)`.
 
 `gochars` may also be a callable, in which case a character
 `ch` is accepted if `gochars(ch)` is true.
@@ -292,15 +467,15 @@
 
 Keyword arguments are passed to `get_identifier`
 (used for each component of the dotted identifier).
 
 ## Function `get_envvar(s, offset=0, environ=None, default=None, specials=None)`
 
 Parse a simple environment variable reference to $varname or
-$x where "x" is a special character.
+$x where \"x\" is a special character.
 
 Parameters:
 * `s`: the string with the variable reference
 * `offset`: the starting point for the reference
 * `default`: default value for missing environment variables;
    if `None` (the default) a `ValueError` is raised
 * `environ`: the environment mapping, default `os.environ`
@@ -371,16 +546,16 @@
 * `prefix`: the prefix string which must appear at `offset`
   or an object with a `match(str,offset)` method
   such as an `re.Pattern` regexp instance
 * `n`: optional integer value;
   if omitted any value will be accepted, otherwise the numeric
   part must match `n`
 
-If `prefix` is a `str`, the "matched prefix" return value is `prefix`.
-Otherwise the "matched prefix" return value is the result of
+If `prefix` is a `str`, the \"matched prefix\" return value is `prefix`.
+Otherwise the \"matched prefix\" return value is the result of
 the `prefix.match(s,offset)` call. The result must also support
 a `.end()` method returning the offset in `s` beyond the match,
 used to locate the following numeric portion.
 
 Examples:
 
    >>> import re
@@ -391,43 +566,43 @@
    >>> get_prefix_n('s03e01--', 's', 4)
    (None, None, 0)
    >>> get_prefix_n('s03e01--', re.compile('[es]',re.I))
    (<re.Match object; span=(0, 1), match='s'>, 3, 3)
    >>> get_prefix_n('s03e01--', re.compile('[es]',re.I), offset=3)
    (<re.Match object; span=(3, 4), match='e'>, 1, 6)
 
-## Function `get_qstr(s, offset=0, q='"', environ=None, default=None, env_specials=None)`
+## Function `get_qstr(s, offset=0, q='\"', environ=None, default=None, env_specials=None)`
 
 Get quoted text with slosh escapes and optional environment substitution.
 
 Parameters:
 * `s`: the string containg the quoted text.
 * `offset`: the starting point, default `0`.
-* `q`: the quote character, default `'"'`. If `q` is `None`,
+* `q`: the quote character, default `'\"'`. If `q` is `None`,
   do not expect the string to be delimited by quote marks.
 * `environ`: if not `None`, also parse and expand `$`*envvar* references.
 * `default`: passed to `get_envvar`
 
 ## Function `get_qstr_or_identifier(s, offset)`
 
 Parse a double quoted string or an identifier.
 
-## Function `get_sloshed_text(s, delim, offset=0, slosh='\\', mapper=<function slosh_mapper at 0x104903eb0>, specials=None)`
+## Function `get_sloshed_text(s, delim, offset=0, slosh='\\\\', mapper=<function slosh_mapper at 0x102494550>, specials=None)`
 
 Collect slosh escaped text from the string `s` from position
 `offset` (default `0`) and return the decoded unicode string and
 the offset of the completed parse.
 
 Parameters:
 * `delim`: end of string delimiter, such as a single or double quote.
 * `offset`: starting offset within `s`, default `0`.
-* `slosh`: escape character, default a slosh ('\').
+* `slosh`: escape character, default a slosh ('\\').
 * `mapper`: a mapping function which accepts a single character
   and returns a replacement string or `None`; this is used the
-  replace things such as '\t' or '\n'. The default is the
+  replace things such as '\\t' or '\\n'. The default is the
   `slosh_mapper` function, whose default mapping is `SLOSH_CHARMAP`.
 * `specials`: a mapping of other special character sequences and parse
   functions for gathering them up. When one of the special
   character sequences is found in the string, the parse
   function is called to parse at that point.
   The parse functions accept
   `s` and the offset of the special character. They return
@@ -442,14 +617,32 @@
   2 hexadecimal digits.
 * the character 'u', insert the character with code from the following
   4 hexadecimal digits.
 * the character 'U', insert the character with code from the following
   8 hexadecimal digits.
 * a character from the keys of `mapper`
 
+## Function `get_suffix_part(s, *, keywords=('part',), numeral_map=None)`
+
+Strip a trailing \"part N\" suffix from the string `s`.
+Return the matched suffix and the number part number.
+Retrn `(None,None)` on no match.
+
+Parameters:
+* `s`: the string
+* `keywords`: an iterable of `str` to match, or a single `str`;
+  default `'part'`
+* `numeral_map`: an optional mapping of numeral names to numeric values;
+  default `NUMERAL_NAMES['en']`, the English numerals
+
+Exanmple:
+
+    >>> get_suffix_part('s09e10 - A New World: Part One')
+    (': Part One', 1)
+
 ## Function `get_tokens(s, offset, getters)`
 
 Parse the string `s` from position `offset` using the supplied
 tokeniser functions `getters`.
 Return the list of tokens matched and the final offset.
 
 Parameters:
@@ -499,15 +692,15 @@
 
 ## Function `htmlify(s, nbsp=False)`
 
 Convert a string for safe transcription in HTML.
 
 Parameters:
 * `s`: the string
-* `nbsp`: replaces spaces with `"&nbsp;"` to prevent word folding,
+* `nbsp`: replaces spaces with `\"&nbsp;\"` to prevent word folding,
   default `False`.
 
 ## Function `htmlquote(s)`
 
 Quote a string for use in HTML.
 
 ## Function `is_dotted_identifier(s, offset=0, **kw)`
@@ -563,28 +756,28 @@
 ## Function `r(o, max_length=None, *, use_cls=False)`
 
 Like `typed_str` but using `repr` instead of `str`.
 This is available as both `typed_repr` and `r`.
 
 ## Function `s(o, use_cls=False, use_repr=False, max_length=32)`
 
-Return "type(o).__name__:str(o)" for some object `o`.
+Return \"type(o).__name__:str(o)\" for some object `o`.
 This is available as both `typed_str` and `s`.
 
 Parameters:
 * `use_cls`: default `False`;
   if true, use `str(type(o))` instead of `type(o).__name__`
 * `use_repr`: default `False`;
   if true, use `repr(o)` instead of `str(o)`
 
 I use this a lot when debugging. Example:
 
     from cs.lex import typed_str as s
     ......
-    X("foo = %s", s(foo))
+    X(\"foo = %s\", s(foo))
 
 ## Function `skipwhite(s, offset=0)`
 
 Convenience routine for skipping past whitespace;
 returns the offset of the next nonwhitespace character.
 
 ## Function `slosh_mapper(c, charmap=None)`
@@ -627,18 +820,18 @@
 
 This supports my preferred docstring layout, where the opening
 line of text is on the same line as the opening quote.
 
 Example:
 
     >>> def func(s):
-    ...   """ Slightly smarter dedent which ignores a string's opening indent.
+    ...   \"\"\" Slightly smarter dedent which ignores a string's opening indent.
     ...       Strip the supplied string `s`. Pull off the leading line.
     ...       Dedent the rest. Put back the leading line.
-    ...   """
+    ...   \"\"\"
     ...   pass
     ...
     >>> from cs.lex import stripped_dedent
     >>> print(stripped_dedent(func.__doc__))
     Slightly smarter dedent which ignores a string's opening indent.
     Strip the supplied string `s`. Pull off the leading line.
     Dedent the rest. Put back the leading line.
@@ -655,15 +848,15 @@
 
 Transcribe the bytes `bs` to text using compact text runs for
 some common text values.
 
 This can be reversed with the `untexthexify` function.
 
 This is an ad doc format devised to be compact but also to
-expose "text" embedded within to the eye. The original use
+expose \"text\" embedded within to the eye. The original use
 case was transcribing a binary directory entry format, where
 the filename parts would be somewhat visible in the transcription.
 
 The output is a string of hexadecimal digits for the encoded
 bytes except for runs of values from the whitelist, which are
 enclosed in the shiftin and shiftout markers and transcribed
 as is. The default whitelist is values of the ASCII letters,
@@ -701,28 +894,28 @@
 ## Function `typed_repr(o, max_length=None, *, use_cls=False)`
 
 Like `typed_str` but using `repr` instead of `str`.
 This is available as both `typed_repr` and `r`.
 
 ## Function `typed_str(o, use_cls=False, use_repr=False, max_length=32)`
 
-Return "type(o).__name__:str(o)" for some object `o`.
+Return \"type(o).__name__:str(o)\" for some object `o`.
 This is available as both `typed_str` and `s`.
 
 Parameters:
 * `use_cls`: default `False`;
   if true, use `str(type(o))` instead of `type(o).__name__`
 * `use_repr`: default `False`;
   if true, use `repr(o)` instead of `str(o)`
 
 I use this a lot when debugging. Example:
 
     from cs.lex import typed_str as s
     ......
-    X("foo = %s", s(foo))
+    X(\"foo = %s\", s(foo))
 
 ## Function `unctrl(s, tabsize=8)`
 
 Return the string `s` with `TAB`s expanded and control characters
 replaced with printable representations.
 
 ## Function `untexthexify(s, shiftin='[', shiftout=']')`
@@ -747,14 +940,17 @@
 * `shiftout`: Optional. The marker string ending a sequence
   of direct text transcription, default `']'`.
 
 # Release Log
 
 
 
+*Release 20240519*:
+New get_suffix_part() to extract things line \": Part One\" from something such as a TV episode name.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240211*:
 New split_remote_path() function to recognise [[user@]host]:path.
 
 *Release 20231018*:
@@ -785,15 +981,15 @@
 * typed_str,typed_repr: make max_length the first optional positional parameter, make other parameters keyword only.
 * New camelcase() and snakecase() functions.
 
 *Release 20211208*:
 Docstring updates.
 
 *Release 20210913*:
-* FormatableFormatter.FORMAT_RE_ARG_NAME_s: strings commencing with digits now match \d+(\.\d+)[a-z]+, eg "02d".
+* FormatableFormatter.FORMAT_RE_ARG_NAME_s: strings commencing with digits now match \\d+(\\.\\d+)[a-z]+, eg \"02d\".
 * Alias typed_str as s and typed_repr as r.
 * FormatableFormatter: new .format_mode thread local state object initially with strict=False, used to control whether unknown fields leave a placeholder or raise KeyError.
 * FormatableFormatter.format_field: assorted fixes.
 
 *Release 20210906*:
 New strip_prefix_n() function to strip a leading `prefix` and numeric value `n` from the start of a string.
 
@@ -818,17 +1014,17 @@
 *Release 20200718*:
 get_chars: accept a callable for gochars, indicating a per character test function.
 
 *Release 20200613*:
 cropped_repr: replace hardwired 29 with computed length
 
 *Release 20200517*:
-* New get_ini_clausename to parse "[clausename]".
-* New get_ini_clause_entryname parsing "[clausename]entryname".
-* New cropped_repr for returning a shortened repr()+"..." if the length exceeds a threshold.
+* New get_ini_clausename to parse \"[clausename]\".
+* New get_ini_clause_entryname parsing \"[clausename]entryname\".
+* New cropped_repr for returning a shortened repr()+\"...\" if the length exceeds a threshold.
 * New format_escape function to double {} characters to survive str.format.
 
 *Release 20200318*:
 * New lc_() function to lowercase and dash a string, new titleify_lc() to mostly reverse lc_().
 * New format_as function, FormatableMixin and related FormatAsError.
 
 *Release 20200229*:
@@ -853,15 +1049,15 @@
 *Release 20171231*:
 New function get_decimal. Drop unused function dict2js.
 
 *Release 20170904*:
 Python 2/3 ports, move rfc2047 into new cs.rfc2047 module.
 
 *Release 20160828*:
-* Use "install_requires" instead of "requires" in DISTINFO.
+* Use \"install_requires\" instead of \"requires\" in DISTINFO.
 * Discard str1(), pointless optimisation.
 * unrfc2047: map _ to SPACE, improve exception handling.
 * Add phpquote: quote a string for use in PHP code; add docstring to jsquote.
 * Add is_identifier test.
 * Add get_dotted_identifier.
 * Add is_dotted_identifier.
 * Add get_hexadecimal.
@@ -871,9 +1067,25 @@
 *Release 20150120*:
 cs.lex: texthexify: backport to python 2 using cs.py3 bytes type
 
 *Release 20150118*:
 metadata updates
 
 *Release 20150116*:
-PyPI metadata and slight code cleanup.
+PyPI metadata and slight code cleanup."""
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
+    "cs.lex",
+]
 
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

### Comparing `cs.lex-20240316/pyproject.toml` & `cs.lex-20240519/lib/python/cs.lex.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,33 @@
-[project]
-name = "cs.lex"
-description = "Lexical analysis functions, tokenisers, transcribers: an arbitrary assortment of lexical and tokenisation functions useful for writing recursive descent parsers, of which I have several. There are also some transcription functions for producing text from various objects, such as `hexify` and `unctrl`."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python2",
-    "python3",
-]
-dependencies = [
-    "cs.dateutils>=20230210",
-    "cs.deco>=20240316",
-    "cs.gimmicks>=20240316",
-    "cs.pfx>=20230604",
-    "cs.py.func>=20230331",
-    "cs.seq>=20200914",
-    "icontract",
-    "python-dateutil",
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
-version = "20240316"
+Metadata-Version: 2.1
+Name: cs.lex
+Version: 20240519
+Summary: Lexical analysis functions, tokenisers, transcribers: an arbitrary assortment of lexical and tokenisation functions useful for writing recursive descent parsers, of which I have several. There are also some transcription functions for producing text from various objects, such as `hexify` and `unctrl`.
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
 Lexical analysis functions, tokenisers, transcribers:
 an arbitrary assortment of lexical and tokenisation functions useful
 for writing recursive descent parsers, of which I have several.
 There are also some transcription functions for producing text
 from various objects, such as `hexify` and `unctrl`.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240519*:
+New get_suffix_part() to extract things line ": Part One" from something such as a TV episode name.
 
 Generally the get_* functions accept a source string and an offset
 (usually optional, default `0`) and return a token and the new offset,
 raising `ValueError` on failed tokenisation.
 
 ## Function `as_lines(chunks, partials=None)`
 
@@ -147,26 +125,32 @@
     >>> cutsuffix(abc_def, '.def')
     'abc'
     >>> cutsuffix(abc_def, '.zzz')
     'abc.def'
     >>> cutsuffix(abc_def, '.zzz') is abc_def
     True
 
-## Class `FFloat(FNumericMixin, FormatableMixin, FormatableFormatter, string.Formatter, builtins.float)`
+## Class `FFloat(FNumericMixin, builtins.float)`
 
 Formattable `float`.
 
-## Class `FInt(FNumericMixin, FormatableMixin, FormatableFormatter, string.Formatter, builtins.int)`
+## Class `FInt(FNumericMixin, builtins.int)`
 
 Formattable `int`.
 
-## Class `FNumericMixin(FormatableMixin, FormatableFormatter, string.Formatter)`
+## Class `FNumericMixin(FormatableMixin)`
 
 A `FormatableMixin` subclass.
 
+*Method `FNumericMixin.localtime(self)`*:
+Treat this as a UNIX timestamp and return a localtime `datetime`.
+
+*Method `FNumericMixin.utctime(self)`*:
+Treat this as a UNIX timestamp and return a UTC `datetime`.
+
 ## Function `format_as(format_s: str, format_mapping, formatter=None, error_sep=None, strict=None)`
 
 Format the string `format_s` using `Formatter.vformat`,
 return the formatted result.
 This is a wrapper for `str.format_map`
 which raises a more informative `FormatAsError` exception on failure.
 
@@ -218,15 +202,64 @@
 with `{self:format_spec}`.
 
 ## Class `FormatableFormatter(string.Formatter)`
 
 A `string.Formatter` subclass interacting with objects
 which inherit from `FormatableMixin`.
 
-## Class `FormatableMixin(FormatableFormatter, string.Formatter)`
+*Method `FormatableFormatter.format_field(value, format_spec: str)`*:
+Format a value using `value.format_format_field`,
+returning an `FStr`
+(a `str` subclass with additional `format_spec` features).
+
+We actually recognise colon separated chains of formats
+and apply each format to the previously converted value.
+The final result is promoted to an `FStr` before return.
+
+*Property `FormatableFormatter.format_mode`*:
+Thread local state object.
+
+Attributes:
+* `strict`: initially `False`; raise a `KeyError` for
+  unresolveable field names
+
+*Method `FormatableFormatter.get_arg_name(field_name)`*:
+Default initial arg_name is an identifier.
+
+Returns `(prefix,offset)`, and `('',0)` if there is no arg_name.
+
+*Method `FormatableFormatter.get_field(self, field_name, args, kwargs)`*:
+Get the object referenced by the field text `field_name`.
+Raises `KeyError` for an unknown `field_name`.
+
+*Method `FormatableFormatter.get_format_subspecs(format_spec)`*:
+Parse a `format_spec` as a sequence of colon separated components,
+return a list of the components.
+
+*Method `FormatableFormatter.get_subfield(value, subfield_text: str)`*:
+Resolve `value` against `subfield_text`,
+the remaining field text after the term which resolved to `value`.
+
+For example, a format `{name.blah[0]}`
+has the field text `name.blah[0]`.
+A `get_field` implementation might initially
+resolve `name` to some value,
+leaving `.blah[0]` as the `subfield_text`.
+This method supports taking that value
+and resolving it against the remaining text `.blah[0]`.
+
+For generality, if `subfield_text` is the empty string
+`value` is returned unchanged.
+
+*Method `FormatableFormatter.get_value(self, arg_name, args, kwargs)`*:
+Get the object with index `arg_name`.
+
+This default implementation returns `(kwargs[arg_name],arg_name)`.
+
+## Class `FormatableMixin(FormatableFormatter)`
 
 A subclass of `FormatableFormatter` which  provides 2 features:
 - a `__format__` method which parses the `format_spec` string
   into multiple colon separated terms whose results chain
 - a `format_as` method which formats a format string using `str.format_map`
   with a suitable mapping derived from the instance
   via its `format_kwargs` method
@@ -254,27 +287,125 @@
   terms with no colons, letting `format_field` do the split into terms
 - override `FormatableFormatter.get_format_subspecs` to implement
   the parse of `format_spec` into a sequence of terms.
   This might recognise a special additional syntax
   and quietly fall back to `super().get_format_subspecs`
   if that is not present.
 
-## Class `FormatAsError(builtins.LookupError, builtins.Exception, builtins.BaseException)`
+*Method `FormatableMixin.__format__(self, format_spec)`*:
+Format `self` according to `format_spec`.
+
+This implementation calls `self.format_field`.
+As such, a `format_spec` is considered
+a sequence of colon separated terms.
+
+Classes wanting to implement additional format string syntaxes
+should either:
+- override `FormatableFormatter.format_field1` to implement
+  terms with no colons, letting `format_field1` do the split into terms
+- override `FormatableFormatter.get_format_subspecs` to implement
+  the term parse.
+
+The default implementation of `__format1__` just calls `super().__format__`.
+Implementations providing specialised formats
+should implement them in `__format1__`
+with fallback to `super().__format1__`.
+
+*Method `FormatableMixin.convert_field(self, value, conversion)`*:
+The default converter for fields calls `Formatter.convert_field`.
+
+*Method `FormatableMixin.convert_via_method_or_attr(self, value, format_spec)`*:
+Apply a method or attribute name based conversion to `value`
+where `format_spec` starts with a method name
+applicable to `value`.
+Return `(converted,offset)`
+being the converted value and the offset after the method name.
+
+Note that if there is not a leading identifier on `format_spec`
+then `value` is returned unchanged with `offset=0`.
+
+The methods/attributes are looked up in the mapping
+returned by `.format_attributes()` which represents allowed methods
+(broadly, one should not allow methods which modify any state).
+
+If this returns a callable, it is called to obtain the converted value
+otherwise it is used as is.
+
+As a final tweak,
+if `value.get_format_attribute()` raises an `AttributeError`
+(the attribute is not an allowed attribute)
+or calling the attribute raises a `TypeError`
+(the `value` isn't suitable)
+and the `value` is not an instance of `FStr`,
+convert it to an `FStr` and try again.
+This provides the common utility methods on other types.
+
+The motivating example was a `PurePosixPath`,
+which does not JSON transcribe;
+this tweak supports both
+`posixpath:basename` via the pathlib stuff
+and `posixpath:json` via `FStr`
+even though a `PurePosixPath` does not subclass `FStr`.
+
+*Method `FormatableMixin.format_as(self, format_s, error_sep=None, strict=None, **control_kw)`*:
+Return the string `format_s` formatted using the mapping
+returned by `self.format_kwargs(**control_kw)`.
+
+If a class using the mixin has no `format_kwargs(**control_kw)` method
+to provide a mapping for `str.format_map`
+then the instance itself is used as the mapping.
+
+*Method `FormatableMixin.get_format_attribute(self, attr)`*:
+Return a mapping of permitted methods to functions of an instance.
+This is used to whitelist allowed `:`*name* method formats
+to prevent scenarios like little Bobby Tables calling `delete()`.
+
+*Method `FormatableMixin.get_format_attributes()`*:
+Return the mapping of format attributes.
+
+*Method `FormatableMixin.json(self)`*:
+The value transcribed as compact JSON.
+
+## Class `FormatAsError(builtins.LookupError)`
 
 Subclass of `LookupError` for use by `format_as`.
 
-## Class `FStr(FormatableMixin, FormatableFormatter, string.Formatter, builtins.str)`
+## Class `FStr(FormatableMixin, builtins.str)`
 
 A `str` subclass with the `FormatableMixin` methods,
 particularly its `__format__` method
 which uses `str` method names as valid formats.
 
 It also has a bunch of utility methods which are available
 as `:`*method* in format strings.
 
+*Method `FStr.basename(self)`*:
+Treat as a filesystem path and return the basename.
+
+*Method `FStr.dirname(self)`*:
+Treat as a filesystem path and return the dirname.
+
+*Method `FStr.f(self)`*:
+Parse `self` as a `float`.
+
+*Method `FStr.i(self, base=10)`*:
+Parse `self` as an `int`.
+
+*Method `FStr.lc(self)`*:
+Lowercase using `lc_()`.
+
+*Method `FStr.path(self)`*:
+Convert to a native filesystem `pathlib.Path`.
+
+*Method `FStr.posix_path(self)`*:
+Convert to a Posix filesystem `pathlib.Path`.
+
+*Method `FStr.windows_path(self)`*:
+Convert to a Windows filesystem `pathlib.Path`.
+
 ## Function `get_chars(s, offset, gochars)`
 
 Scan the string `s` for characters in `gochars` starting at `offset`.
 Return `(match,new_offset)`.
 
 `gochars` may also be a callable, in which case a character
 `ch` is accepted if `gochars(ch)` is true.
@@ -314,15 +445,15 @@
 
 Keyword arguments are passed to `get_identifier`
 (used for each component of the dotted identifier).
 
 ## Function `get_envvar(s, offset=0, environ=None, default=None, specials=None)`
 
 Parse a simple environment variable reference to $varname or
-$x where \"x\" is a special character.
+$x where "x" is a special character.
 
 Parameters:
 * `s`: the string with the variable reference
 * `offset`: the starting point for the reference
 * `default`: default value for missing environment variables;
    if `None` (the default) a `ValueError` is raised
 * `environ`: the environment mapping, default `os.environ`
@@ -393,16 +524,16 @@
 * `prefix`: the prefix string which must appear at `offset`
   or an object with a `match(str,offset)` method
   such as an `re.Pattern` regexp instance
 * `n`: optional integer value;
   if omitted any value will be accepted, otherwise the numeric
   part must match `n`
 
-If `prefix` is a `str`, the \"matched prefix\" return value is `prefix`.
-Otherwise the \"matched prefix\" return value is the result of
+If `prefix` is a `str`, the "matched prefix" return value is `prefix`.
+Otherwise the "matched prefix" return value is the result of
 the `prefix.match(s,offset)` call. The result must also support
 a `.end()` method returning the offset in `s` beyond the match,
 used to locate the following numeric portion.
 
 Examples:
 
    >>> import re
@@ -413,43 +544,43 @@
    >>> get_prefix_n('s03e01--', 's', 4)
    (None, None, 0)
    >>> get_prefix_n('s03e01--', re.compile('[es]',re.I))
    (<re.Match object; span=(0, 1), match='s'>, 3, 3)
    >>> get_prefix_n('s03e01--', re.compile('[es]',re.I), offset=3)
    (<re.Match object; span=(3, 4), match='e'>, 1, 6)
 
-## Function `get_qstr(s, offset=0, q='\"', environ=None, default=None, env_specials=None)`
+## Function `get_qstr(s, offset=0, q='"', environ=None, default=None, env_specials=None)`
 
 Get quoted text with slosh escapes and optional environment substitution.
 
 Parameters:
 * `s`: the string containg the quoted text.
 * `offset`: the starting point, default `0`.
-* `q`: the quote character, default `'\"'`. If `q` is `None`,
+* `q`: the quote character, default `'"'`. If `q` is `None`,
   do not expect the string to be delimited by quote marks.
 * `environ`: if not `None`, also parse and expand `$`*envvar* references.
 * `default`: passed to `get_envvar`
 
 ## Function `get_qstr_or_identifier(s, offset)`
 
 Parse a double quoted string or an identifier.
 
-## Function `get_sloshed_text(s, delim, offset=0, slosh='\\\\', mapper=<function slosh_mapper at 0x104903eb0>, specials=None)`
+## Function `get_sloshed_text(s, delim, offset=0, slosh='\\', mapper=<function slosh_mapper at 0x102494550>, specials=None)`
 
 Collect slosh escaped text from the string `s` from position
 `offset` (default `0`) and return the decoded unicode string and
 the offset of the completed parse.
 
 Parameters:
 * `delim`: end of string delimiter, such as a single or double quote.
 * `offset`: starting offset within `s`, default `0`.
-* `slosh`: escape character, default a slosh ('\\').
+* `slosh`: escape character, default a slosh ('\').
 * `mapper`: a mapping function which accepts a single character
   and returns a replacement string or `None`; this is used the
-  replace things such as '\\t' or '\\n'. The default is the
+  replace things such as '\t' or '\n'. The default is the
   `slosh_mapper` function, whose default mapping is `SLOSH_CHARMAP`.
 * `specials`: a mapping of other special character sequences and parse
   functions for gathering them up. When one of the special
   character sequences is found in the string, the parse
   function is called to parse at that point.
   The parse functions accept
   `s` and the offset of the special character. They return
@@ -464,14 +595,32 @@
   2 hexadecimal digits.
 * the character 'u', insert the character with code from the following
   4 hexadecimal digits.
 * the character 'U', insert the character with code from the following
   8 hexadecimal digits.
 * a character from the keys of `mapper`
 
+## Function `get_suffix_part(s, *, keywords=('part',), numeral_map=None)`
+
+Strip a trailing "part N" suffix from the string `s`.
+Return the matched suffix and the number part number.
+Retrn `(None,None)` on no match.
+
+Parameters:
+* `s`: the string
+* `keywords`: an iterable of `str` to match, or a single `str`;
+  default `'part'`
+* `numeral_map`: an optional mapping of numeral names to numeric values;
+  default `NUMERAL_NAMES['en']`, the English numerals
+
+Exanmple:
+
+    >>> get_suffix_part('s09e10 - A New World: Part One')
+    (': Part One', 1)
+
 ## Function `get_tokens(s, offset, getters)`
 
 Parse the string `s` from position `offset` using the supplied
 tokeniser functions `getters`.
 Return the list of tokens matched and the final offset.
 
 Parameters:
@@ -521,15 +670,15 @@
 
 ## Function `htmlify(s, nbsp=False)`
 
 Convert a string for safe transcription in HTML.
 
 Parameters:
 * `s`: the string
-* `nbsp`: replaces spaces with `\"&nbsp;\"` to prevent word folding,
+* `nbsp`: replaces spaces with `"&nbsp;"` to prevent word folding,
   default `False`.
 
 ## Function `htmlquote(s)`
 
 Quote a string for use in HTML.
 
 ## Function `is_dotted_identifier(s, offset=0, **kw)`
@@ -585,28 +734,28 @@
 ## Function `r(o, max_length=None, *, use_cls=False)`
 
 Like `typed_str` but using `repr` instead of `str`.
 This is available as both `typed_repr` and `r`.
 
 ## Function `s(o, use_cls=False, use_repr=False, max_length=32)`
 
-Return \"type(o).__name__:str(o)\" for some object `o`.
+Return "type(o).__name__:str(o)" for some object `o`.
 This is available as both `typed_str` and `s`.
 
 Parameters:
 * `use_cls`: default `False`;
   if true, use `str(type(o))` instead of `type(o).__name__`
 * `use_repr`: default `False`;
   if true, use `repr(o)` instead of `str(o)`
 
 I use this a lot when debugging. Example:
 
     from cs.lex import typed_str as s
     ......
-    X(\"foo = %s\", s(foo))
+    X("foo = %s", s(foo))
 
 ## Function `skipwhite(s, offset=0)`
 
 Convenience routine for skipping past whitespace;
 returns the offset of the next nonwhitespace character.
 
 ## Function `slosh_mapper(c, charmap=None)`
@@ -649,18 +798,18 @@
 
 This supports my preferred docstring layout, where the opening
 line of text is on the same line as the opening quote.
 
 Example:
 
     >>> def func(s):
-    ...   \"\"\" Slightly smarter dedent which ignores a string's opening indent.
+    ...   """ Slightly smarter dedent which ignores a string's opening indent.
     ...       Strip the supplied string `s`. Pull off the leading line.
     ...       Dedent the rest. Put back the leading line.
-    ...   \"\"\"
+    ...   """
     ...   pass
     ...
     >>> from cs.lex import stripped_dedent
     >>> print(stripped_dedent(func.__doc__))
     Slightly smarter dedent which ignores a string's opening indent.
     Strip the supplied string `s`. Pull off the leading line.
     Dedent the rest. Put back the leading line.
@@ -677,15 +826,15 @@
 
 Transcribe the bytes `bs` to text using compact text runs for
 some common text values.
 
 This can be reversed with the `untexthexify` function.
 
 This is an ad doc format devised to be compact but also to
-expose \"text\" embedded within to the eye. The original use
+expose "text" embedded within to the eye. The original use
 case was transcribing a binary directory entry format, where
 the filename parts would be somewhat visible in the transcription.
 
 The output is a string of hexadecimal digits for the encoded
 bytes except for runs of values from the whitelist, which are
 enclosed in the shiftin and shiftout markers and transcribed
 as is. The default whitelist is values of the ASCII letters,
@@ -723,28 +872,28 @@
 ## Function `typed_repr(o, max_length=None, *, use_cls=False)`
 
 Like `typed_str` but using `repr` instead of `str`.
 This is available as both `typed_repr` and `r`.
 
 ## Function `typed_str(o, use_cls=False, use_repr=False, max_length=32)`
 
-Return \"type(o).__name__:str(o)\" for some object `o`.
+Return "type(o).__name__:str(o)" for some object `o`.
 This is available as both `typed_str` and `s`.
 
 Parameters:
 * `use_cls`: default `False`;
   if true, use `str(type(o))` instead of `type(o).__name__`
 * `use_repr`: default `False`;
   if true, use `repr(o)` instead of `str(o)`
 
 I use this a lot when debugging. Example:
 
     from cs.lex import typed_str as s
     ......
-    X(\"foo = %s\", s(foo))
+    X("foo = %s", s(foo))
 
 ## Function `unctrl(s, tabsize=8)`
 
 Return the string `s` with `TAB`s expanded and control characters
 replaced with printable representations.
 
 ## Function `untexthexify(s, shiftin='[', shiftout=']')`
@@ -769,14 +918,17 @@
 * `shiftout`: Optional. The marker string ending a sequence
   of direct text transcription, default `']'`.
 
 # Release Log
 
 
 
+*Release 20240519*:
+New get_suffix_part() to extract things line ": Part One" from something such as a TV episode name.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240211*:
 New split_remote_path() function to recognise [[user@]host]:path.
 
 *Release 20231018*:
@@ -807,15 +959,15 @@
 * typed_str,typed_repr: make max_length the first optional positional parameter, make other parameters keyword only.
 * New camelcase() and snakecase() functions.
 
 *Release 20211208*:
 Docstring updates.
 
 *Release 20210913*:
-* FormatableFormatter.FORMAT_RE_ARG_NAME_s: strings commencing with digits now match \\d+(\\.\\d+)[a-z]+, eg \"02d\".
+* FormatableFormatter.FORMAT_RE_ARG_NAME_s: strings commencing with digits now match \d+(\.\d+)[a-z]+, eg "02d".
 * Alias typed_str as s and typed_repr as r.
 * FormatableFormatter: new .format_mode thread local state object initially with strict=False, used to control whether unknown fields leave a placeholder or raise KeyError.
 * FormatableFormatter.format_field: assorted fixes.
 
 *Release 20210906*:
 New strip_prefix_n() function to strip a leading `prefix` and numeric value `n` from the start of a string.
 
@@ -840,17 +992,17 @@
 *Release 20200718*:
 get_chars: accept a callable for gochars, indicating a per character test function.
 
 *Release 20200613*:
 cropped_repr: replace hardwired 29 with computed length
 
 *Release 20200517*:
-* New get_ini_clausename to parse \"[clausename]\".
-* New get_ini_clause_entryname parsing \"[clausename]entryname\".
-* New cropped_repr for returning a shortened repr()+\"...\" if the length exceeds a threshold.
+* New get_ini_clausename to parse "[clausename]".
+* New get_ini_clause_entryname parsing "[clausename]entryname".
+* New cropped_repr for returning a shortened repr()+"..." if the length exceeds a threshold.
 * New format_escape function to double {} characters to survive str.format.
 
 *Release 20200318*:
 * New lc_() function to lowercase and dash a string, new titleify_lc() to mostly reverse lc_().
 * New format_as function, FormatableMixin and related FormatAsError.
 
 *Release 20200229*:
@@ -875,15 +1027,15 @@
 *Release 20171231*:
 New function get_decimal. Drop unused function dict2js.
 
 *Release 20170904*:
 Python 2/3 ports, move rfc2047 into new cs.rfc2047 module.
 
 *Release 20160828*:
-* Use \"install_requires\" instead of \"requires\" in DISTINFO.
+* Use "install_requires" instead of "requires" in DISTINFO.
 * Discard str1(), pointless optimisation.
 * unrfc2047: map _ to SPACE, improve exception handling.
 * Add phpquote: quote a string for use in PHP code; add docstring to jsquote.
 * Add is_identifier test.
 * Add get_dotted_identifier.
 * Add is_dotted_identifier.
 * Add get_hexadecimal.
@@ -893,25 +1045,9 @@
 *Release 20150120*:
 cs.lex: texthexify: backport to python 2 using cs.py3 bytes type
 
 *Release 20150118*:
 metadata updates
 
 *Release 20150116*:
-PyPI metadata and slight code cleanup."""
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
-    "cs.lex",
-]
+PyPI metadata and slight code cleanup.
 
-[tool.setuptools.package-dir]
-"" = "lib/python"
```

