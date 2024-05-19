# Comparing `tmp/blint-2.1.5.tar.gz` & `tmp/blint-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blint-2.1.5.tar", max compression
+gzip compressed data, was "blint-2.1.6.tar", max compression
```

## Comparing `blint-2.1.5.tar` & `blint-2.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1068 2024-05-06 14:39:28.372417 blint-2.1.5/LICENSE
--rw-r--r--   0        0        0     6233 2024-05-06 14:39:28.372417 blint-2.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-06 14:39:28.372417 blint-2.1.5/blint/__init__.py
--rw-r--r--   0        0        0    24653 2024-05-06 14:39:28.372417 blint-2.1.5/blint/analysis.py
--rw-r--r--   0        0        0    13915 2024-05-06 14:39:28.372417 blint-2.1.5/blint/android.py
--rw-r--r--   0        0        0    58518 2024-05-06 14:39:28.372417 blint-2.1.5/blint/binary.py
--rw-r--r--   0        0        0     2794 2024-05-06 14:39:28.372417 blint-2.1.5/blint/checks.py
--rw-r--r--   0        0        0     6198 2024-05-06 14:39:28.372417 blint-2.1.5/blint/cli.py
--rw-r--r--   0        0        0    20192 2024-05-06 14:39:28.372417 blint-2.1.5/blint/config.py
--rw-r--r--   0        0        0      324 2024-05-06 14:39:28.372417 blint-2.1.5/blint/cyclonedx/README.md
--rw-r--r--   0        0        0        0 2024-05-06 14:39:28.372417 blint-2.1.5/blint/cyclonedx/__init__.py
--rw-r--r--   0        0        0    20843 2024-05-06 14:39:28.372417 blint-2.1.5/blint/cyclonedx/spdx.py
--rw-r--r--   0        0        0   169203 2024-05-06 14:39:28.372417 blint-2.1.5/blint/cyclonedx/spec.py
--rw-r--r--   0        0        0        0 2024-05-06 14:39:28.372417 blint-2.1.5/blint/data/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/__init__.py
--rw-r--r--   0        0        0     1498 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_entries_generic.yml
--rw-r--r--   0        0        0     2358 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_entries_pe.yml
--rw-r--r--   0        0        0    15418 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_exe_go.yml
--rw-r--r--   0        0        0   124932 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_imports_pe.yml
--rw-r--r--   0        0        0     8155 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_methods_generic.yml
--rw-r--r--   0        0        0     5764 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_methods_mips.yml
--rw-r--r--   0        0        0     2409 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_monero_generic.yml
--rw-r--r--   0        0        0     1522 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_monero_go.yml
--rw-r--r--   0        0        0      994 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_monero_rust
--rw-r--r--   0        0        0      994 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_monero_rust.yml
--rw-r--r--   0        0        0     5646 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_rootkits_win.yml
--rw-r--r--   0        0        0     3507 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_symbols_antiforensic.yml
--rw-r--r--   0        0        0     2943 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_symbols_generic.yml
--rw-r--r--   0        0        0     1277 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_symbols_hooka.yml
--rw-r--r--   0        0        0    23537 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_symbols_macho.yml
--rw-r--r--   0        0        0    10425 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/annotations/review_symbols_rust.yml
--rw-r--r--   0        0        0    11038 2024-05-06 14:39:28.376417 blint-2.1.5/blint/data/rules.yml
--rw-r--r--   0        0        0      936 2024-05-06 14:39:28.376417 blint-2.1.5/blint/logger.py
--rw-r--r--   0        0        0    24904 2024-05-06 14:39:28.376417 blint-2.1.5/blint/sbom.py
--rw-r--r--   0        0        0    14365 2024-05-06 14:39:28.376417 blint-2.1.5/blint/utils.py
--rw-r--r--   0        0        0     1872 2024-05-06 14:39:28.380417 blint-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     7494 1970-01-01 00:00:00.000000 blint-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-19 15:19:11.846203 blint-2.1.6/LICENSE
+-rw-r--r--   0        0        0     6233 2024-05-19 15:19:11.846203 blint-2.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 15:19:11.850203 blint-2.1.6/blint/__init__.py
+-rw-r--r--   0        0        0    24648 2024-05-19 15:19:11.850203 blint-2.1.6/blint/analysis.py
+-rw-r--r--   0        0        0    13915 2024-05-19 15:19:11.850203 blint-2.1.6/blint/android.py
+-rw-r--r--   0        0        0    59632 2024-05-19 15:19:11.850203 blint-2.1.6/blint/binary.py
+-rw-r--r--   0        0        0     2785 2024-05-19 15:19:11.850203 blint-2.1.6/blint/checks.py
+-rw-r--r--   0        0        0     6198 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cli.py
+-rw-r--r--   0        0        0    20192 2024-05-19 15:19:11.850203 blint-2.1.6/blint/config.py
+-rw-r--r--   0        0        0      324 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cyclonedx/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cyclonedx/__init__.py
+-rw-r--r--   0        0        0    20843 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cyclonedx/spdx.py
+-rw-r--r--   0        0        0   169203 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cyclonedx/spec.py
+-rw-r--r--   0        0        0        0 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/__init__.py
+-rw-r--r--   0        0        0     1498 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/review_entries_generic.yml
+-rw-r--r--   0        0        0     2358 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/review_entries_pe.yml
+-rw-r--r--   0        0        0    15418 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/review_exe_go.yml
+-rw-r--r--   0        0        0   124932 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/review_imports_pe.yml
+-rw-r--r--   0        0        0     8155 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_methods_generic.yml
+-rw-r--r--   0        0        0     5764 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_methods_mips.yml
+-rw-r--r--   0        0        0     2409 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_monero_generic.yml
+-rw-r--r--   0        0        0     1522 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_monero_go.yml
+-rw-r--r--   0        0        0      994 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_monero_rust
+-rw-r--r--   0        0        0      994 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_monero_rust.yml
+-rw-r--r--   0        0        0     5646 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_rootkits_win.yml
+-rw-r--r--   0        0        0     3507 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_antiforensic.yml
+-rw-r--r--   0        0        0     2943 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_generic.yml
+-rw-r--r--   0        0        0     1277 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_hooka.yml
+-rw-r--r--   0        0        0    23537 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_macho.yml
+-rw-r--r--   0        0        0    10425 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_rust.yml
+-rw-r--r--   0        0        0    11038 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/rules.yml
+-rw-r--r--   0        0        0      936 2024-05-19 15:19:11.854203 blint-2.1.6/blint/logger.py
+-rw-r--r--   0        0        0    24832 2024-05-19 15:19:11.854203 blint-2.1.6/blint/sbom.py
+-rw-r--r--   0        0        0    15610 2024-05-19 15:19:11.854203 blint-2.1.6/blint/utils.py
+-rw-r--r--   0        0        0     1884 2024-05-19 15:19:11.854203 blint-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 blint-2.1.6/PKG-INFO
```

### Comparing `blint-2.1.5/LICENSE` & `blint-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/README.md` & `blint-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/analysis.py` & `blint-2.1.6/blint/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,15 +442,15 @@
         """Performs a review of the given file."""
         self.progress.update(
             self.task, description="Checking methods against review rules")
         self.reviewer = ReviewRunner()
         self.reviewer.run_review(metadata)
         if self.reviewer.results:
             review = self.reviewer.process_review(f, exe_name)
-            self.reviews.extend(review)
+            self.reviews += review
 
 
 class ReviewRunner:
     """Class for running reviews."""
 
     def __init__(self):
         self.results = {}
```

### Comparing `blint-2.1.5/blint/android.py` & `blint-2.1.6/blint/android.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/binary.py` & `blint-2.1.6/blint/binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,34 +25,60 @@
 if LOG.level != DEBUG:
     lief.logging.disable()
 
 ADDRESS_FMT = "0x{:<10x}"
 
 
 def demangle_symbolic_name(symbol, lang=None, no_args=False):
-    """Demangles symbol using llvm demangle falling back to some heuristics."""
+    """Demangles symbol using llvm demangle falling back to some heuristics. Covers legacy rust."""
     if not SYMBOLIC_FOUND:
         return symbol
     try:
         func = lib.symbolic_demangle_no_args if no_args else lib.symbolic_demangle
         lang_str = encode_str(lang) if lang else ffi.NULL
         demangled = rustcall(func, encode_str(symbol), lang_str)
         demangled_symbol = decode_str(demangled, free=True).strip()
         # demangling didn't work
         if symbol and symbol == demangled_symbol:
-            for ign in ("__imp_anon.", "anon."):
+            for ign in ("__imp_anon.", "anon.", ".L__unnamed"):
                 if symbol.startswith(ign):
                     return "anonymous"
             if symbol.startswith("GCC_except_table"):
                 return "GCC_except_table"
             if symbol.startswith("@feat.00"):
                 return "SAFESEH"
-            if symbol.startswith("__imp_") or symbol.startswith(".rdata$") or symbol.startswith(".refptr."):
+            if (
+                symbol.startswith("__imp_")
+                or symbol.startswith(".rdata$")
+                or symbol.startswith(".refptr.")
+            ):
                 symbol = f"__declspec(dllimport) {symbol.removeprefix('__imp_').removeprefix('.rdata$').removeprefix('.refptr.')}"
-            return symbol.replace("..", "::")
+            demangled_symbol = (
+                symbol.replace("..", "::")
+                .replace("$SP$", "@")
+                .replace("$BP$", "*")
+                .replace("$LT$", "<")
+                .replace("$u5b$", "[")
+                .replace("$u7b$", "{")
+                .replace("$u3b$", ";")
+                .replace("$u20$", " ")
+                .replace("$u5d$", "]")
+                .replace("$u7d$", "}")
+                .replace("$GT$", ">")
+                .replace("$RF$", "&")
+                .replace("$LP$", "(")
+                .replace("$RP$", ")")
+                .replace("$C$", ",")
+                .replace("$u27$", "'")
+            )
+        # In case of rust symbols, try and trim the hash part from the end of the symbols
+        if demangled_symbol.count("::") > 3:
+            last_part = demangled_symbol.split("::")[-1]
+            if len(last_part) == 17:
+                demangled_symbol = demangled_symbol.removesuffix(f"::{last_part}")
         return demangled_symbol
     except AttributeError:
         return symbol
 
 
 def is_shared_library(parsed_obj):
     """
@@ -89,15 +115,15 @@
         - The description is truncated to 16 words and appended with "..." if
             it exceeds 16 words.
     """
     data = []
     notes = parsed_obj.notes
     if isinstance(notes, lief.lief_errors):
         return data
-    data.extend(extract_note_data(idx, note) for idx, note in enumerate(notes))
+    data += [extract_note_data(idx, note) for idx, note in enumerate(notes)]
     return data
 
 
 def extract_note_data(idx, note):
     """
     Extracts metadata from a note object and returns a dictionary.
 
@@ -313,17 +339,17 @@
     Returns:
         str: The detected type of the binary.
     """
     with contextlib.suppress(AttributeError, TypeError):
         if parsed_obj.has_section(".note.go.buildid"):
             return "gobinary"
         if (
-                parsed_obj.has_section(".note.gnu.build-id")
-                or "musl" in metadata.get("interpreter")
-                or "ld-linux" in metadata.get("interpreter")
+            parsed_obj.has_section(".note.gnu.build-id")
+            or "musl" in metadata.get("interpreter")
+            or "ld-linux" in metadata.get("interpreter")
         ):
             return "genericbinary"
         if metadata.get("machine_type") and metadata.get("file_type"):
             return f'{metadata.get("machine_type")}-{metadata.get("file_type")}'.lower()
         if metadata["relro"] in ("partial", "full"):
             return "genericbinary"
     return ""
@@ -833,15 +859,15 @@
         symbols_version = parsed_obj.symbols_version
         if symbols_version and not isinstance(symbols_version, lief.lief_errors):
             metadata["symbols_version"] = []
             symbol_version_auxiliary_cache = {}
             for entry in symbols_version:
                 symbol_version_auxiliary = entry.symbol_version_auxiliary
                 if symbol_version_auxiliary and not symbol_version_auxiliary_cache.get(
-                        symbol_version_auxiliary.name
+                    symbol_version_auxiliary.name
                 ):
                     symbol_version_auxiliary_cache[symbol_version_auxiliary.name] = True
                     metadata["symbols_version"].append(
                         {
                             "name": demangle_symbolic_name(symbol_version_auxiliary.name),
                             "hash": symbol_version_auxiliary.hash,
                             "value": entry.value,
@@ -939,25 +965,27 @@
             .replace("\n", "")
             .replace("  ", "")
         )
         if overlay_str.find('{"runtimeTarget') > -1:
             start_index = overlay_str.find('{"runtimeTarget')
             end_index = overlay_str.rfind("}}}")
             if end_index > -1:
-                overlay_str = overlay_str[start_index: end_index + 3]
+                overlay_str = overlay_str[start_index : end_index + 3]
                 try:
                     # deps should have runtimeTarget, compilationOptions, targets, and libraries
                     # Use libraries to construct BOM components and targets for the dependency tree
                     deps = orjson.loads(overlay_str)
                 except orjson.JSONDecodeError:
                     pass
     return deps
 
 
-def parse_go_buildinfo(parsed_obj: lief.Binary) -> Tuple[dict[str, dict[str, str]], dict[str, str]]:
+def parse_go_buildinfo(
+    parsed_obj: lief.Binary,
+) -> Tuple[dict[str, dict[str, str]], dict[str, str]]:
     """
     Parse the go build info section to extract go dependencies
     Args:
         parsed_obj (lief.Binary): The parsed object representing the binary.
 
     Returns:
         tuple(dict[str, str], dict[str, str]): Tuple representing the dependencies and formulation.
@@ -974,35 +1002,43 @@
     if build_info and build_info.size:
         build_info_str = (
             codecs.decode(build_info.content.tobytes(), encoding="utf-8", errors="replace")
             .replace("\0", "")
             .replace("\uFFFD", "")
             .replace("\t", " ")
         ).strip()
-        build_info_str = build_info_str.encode('ascii', 'ignore').decode('ascii')
+        build_info_str = build_info_str.encode("ascii", "ignore").decode("ascii")
     elif isinstance(parsed_obj, lief.PE.Binary):
         # For PE binaries look for .data section
         s: lief.PE.Section = parsed_obj.get_section(".data")
-        build_info_str = codecs.decode(s.content.tobytes()[:int(s.size / 32)], encoding="ascii",
-                                       errors="replace").replace("\0", "").replace("\uFFFD", "").replace("\t", " ")
+        build_info_str = (
+            codecs.decode(
+                s.content.tobytes()[: int(s.size / 32)], encoding="ascii", errors="replace"
+            )
+            .replace("\0", "")
+            .replace("\uFFFD", "")
+            .replace("\t", " ")
+        )
     lines = build_info_str.split("\n")
     for line in lines:
         if line.startswith("Go buildinf:"):
             tmp_a = line.split("Go buildinf:")
             formulation["go_version"] = tmp_a[-1].split("\x19")[0].split(" ")[-1]
         if "path " in line:
             tmp_a = line.split("path ")
             formulation["path"] = tmp_a[-1]
         if line.startswith("mod "):
             tmp_a = line.split("mod ")
             formulation["module"] = tmp_a[-1]
         if line.startswith("dep "):
             tmp_a = line.removeprefix("dep ").split(" ")
-            deps[tmp_a[0]] = {"version": tmp_a[1],
-                              "hash": tmp_a[2] if len(tmp_a) == 3 and tmp_a[2].startswith("h1:") else None}
+            deps[tmp_a[0]] = {
+                "version": tmp_a[1],
+                "hash": tmp_a[2] if len(tmp_a) == 3 and tmp_a[2].startswith("h1:") else None,
+            }
         if line.startswith("build "):
             tmp_a = line.removeprefix("build ").split("=")
             formulation[tmp_a[0].replace("-", "")] = tmp_a[1]
 
     return deps, formulation
 
 
@@ -1014,22 +1050,24 @@
 
     Returns:
         list: List representing the dependencies.
     """
     deps = []
 
     try:
-        audit_data_section = next(filter(lambda section: section.name == ".dep-v0", parsed_obj.sections), None)
+        audit_data_section = next(
+            filter(lambda section: section.name == ".dep-v0", parsed_obj.sections), None
+        )
         if audit_data_section is not None and audit_data_section.content:
             json_string = zlib.decompress(audit_data_section.content)
             audit_data = orjson.loads(json_string)
 
             if audit_data and audit_data["packages"]:
                 packages = audit_data["packages"]
-                deps = [x for x in packages if 'root' not in x]
+                deps = [x for x in packages if "root" not in x]
     except orjson.JSONDecodeError:
         pass
 
     return deps
 
 
 def add_pe_metadata(exe_file: str, metadata: dict, parsed_obj: lief.PE.Binary):
```

### Comparing `blint-2.1.5/blint/checks.py` & `blint-2.1.6/blint/checks.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,71 +6,70 @@
     return metadata.get("has_nx") is not False
 
 
 def check_pie(f, metadata, rule_obj):  # noqa
     return metadata.get("is_pie") is not False
 
 
-def check_relro(f, metadata, rule_obj): # noqa
+def check_relro(f, metadata, rule_obj):  # noqa
     return metadata.get("relro") != "no"
 
 
-def check_canary(f, metadata, rule_obj): # noqa
+def check_canary(f, metadata, rule_obj):  # noqa
     return metadata.get("has_canary") is not False
 
 
-def check_rpath(f, metadata, rule_obj): # noqa
+def check_rpath(f, metadata, rule_obj):  # noqa
     # Do not recommend setting rpath or runpath
     return not metadata.get("has_rpath") and not metadata.get("has_runpath")
 
 
-def check_virtual_size(f, metadata, rule_obj): # noqa
+def check_virtual_size(f, metadata, rule_obj):  # noqa
     if metadata.get("virtual_size"):
         virtual_size = metadata.get("virtual_size") / 1024 / 1024
         size_limit = 30
         if rule_obj.get("limit"):
             limit = rule_obj.get("limit")
             limit = limit.replace("MB", "").replace("M", "")
             if isinstance(limit, str) and rule_obj.get("limit").isdigit():
                 size_limit = int(rule_obj.get("limit"))
         return virtual_size < size_limit
     return True
 
 
-def check_authenticode(f, metadata, rule_obj): # noqa
+def check_authenticode(f, metadata, rule_obj):  # noqa
     if metadata.get("authenticode"):
         authenticode_obj = metadata.get("authenticode")
         vf = authenticode_obj.get("verification_flags", "").lower()
-        return False if vf != "ok" else bool(
-            authenticode_obj.get("cert_signer"))
+        return False if vf != "ok" else bool(authenticode_obj.get("cert_signer"))
     return True
 
 
 def check_dll_characteristics(f, metadata, rule_obj):  # noqa
     res = []
     if metadata.get("dll_characteristics"):
-        res.extend(
+        res += [
             c
             for c in rule_obj.get("mandatory_values", [])
             if c not in metadata.get("dll_characteristics")
-        )
+        ]
     if res:
         res = ", ".join(res)
 
     return res or True
 
 
-def check_codesign(f, metadata, rule_obj): # noqa
+def check_codesign(f, metadata, rule_obj):  # noqa
     if metadata.get("code_signature"):
         code_signature = metadata.get("code_signature")
         return not code_signature or code_signature.get("available") is not False
     return True
 
 
-def check_trust_info(f, metadata, rule_obj): # noqa
+def check_trust_info(f, metadata, rule_obj):  # noqa
     if metadata.get("resources"):
         if manifest := metadata.get("resources").get("manifest"):
             attribs_dict = parse_pe_manifest(manifest)
             if not attribs_dict:
                 return True
             allowed_values = rule_obj.get("allowed_values", {})
             for k, v in allowed_values.items():
```

### Comparing `blint-2.1.5/blint/cli.py` & `blint-2.1.6/blint/cli.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/config.py` & `blint-2.1.6/blint/config.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/cyclonedx/spdx.py` & `blint-2.1.6/blint/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/cyclonedx/spec.py` & `blint-2.1.6/blint/cyclonedx/spec.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_entries_generic.yml` & `blint-2.1.6/blint/data/annotations/review_entries_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_entries_pe.yml` & `blint-2.1.6/blint/data/annotations/review_entries_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_exe_go.yml` & `blint-2.1.6/blint/data/annotations/review_exe_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_imports_pe.yml` & `blint-2.1.6/blint/data/annotations/review_imports_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_methods_generic.yml` & `blint-2.1.6/blint/data/annotations/review_methods_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_methods_mips.yml` & `blint-2.1.6/blint/data/annotations/review_methods_mips.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_monero_generic.yml` & `blint-2.1.6/blint/data/annotations/review_monero_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_monero_go.yml` & `blint-2.1.6/blint/data/annotations/review_monero_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_monero_rust` & `blint-2.1.6/blint/data/annotations/review_monero_rust`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_monero_rust.yml` & `blint-2.1.6/blint/data/annotations/review_monero_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_rootkits_win.yml` & `blint-2.1.6/blint/data/annotations/review_rootkits_win.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_symbols_antiforensic.yml` & `blint-2.1.6/blint/data/annotations/review_symbols_antiforensic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_symbols_generic.yml` & `blint-2.1.6/blint/data/annotations/review_symbols_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_symbols_hooka.yml` & `blint-2.1.6/blint/data/annotations/review_symbols_hooka.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_symbols_macho.yml` & `blint-2.1.6/blint/data/annotations/review_symbols_macho.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/annotations/review_symbols_rust.yml` & `blint-2.1.6/blint/data/annotations/review_symbols_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/data/rules.yml` & `blint-2.1.6/blint/data/rules.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/logger.py` & `blint-2.1.6/blint/logger.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.5/blint/sbom.py` & `blint-2.1.6/blint/sbom.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,21 @@
     Property,
     RefType,
     Scope,
     Tools,
     Type,
 )
 from blint.logger import LOG
-from blint.utils import camel_to_snake, create_component_evidence, find_android_files, gen_file_list, get_version
+from blint.utils import (
+    camel_to_snake,
+    create_component_evidence,
+    find_android_files,
+    gen_file_list,
+    get_version,
+)
 
 
 def default_parent(src_dirs: list[str]) -> Component:
     """
     Creates a default parent Component object for the given source directories.
 
     Args:
@@ -39,14 +45,17 @@
 
     Returns:
         Component: A Component object representing the default parent.
     """
     if not src_dirs:
         raise ValueError("No source directories provided")
     name = os.path.basename(src_dirs[0])
+    # Extract the name from the .rlib files
+    if name.endswith(".rlib"):
+        name = name.split("-")[0].removeprefix("lib")
     purl = f"pkg:generic/{name}@latest"
     component = Component(type=Type.application, name=name, version="latest", purl=purl)
     component.bom_ref = RefType(purl)
     return component
 
 
 def default_metadata(src_dirs):
@@ -58,28 +67,26 @@
 
     Returns:
         Metadata: A Metadata object for SBOM generation.
     """
     metadata = Metadata()
     metadata.timestamp = f'{datetime.now().isoformat(timespec="seconds")}Z'
     metadata.component = default_parent(src_dirs)
-    metadata.tools = (
-        Tools(
-            components=[
-                Component(
-                    type=Type.application,
-                    author="OWASP Foundation",
-                    publisher="OWASP Foundation",
-                    group="owasp-dep-scan",
-                    name="blint",
-                    version=get_version(),
-                    purl=f"pkg:pypi/blint@{get_version()}",
-                )
-            ]
-        )
+    metadata.tools = Tools(
+        components=[
+            Component(
+                type=Type.application,
+                author="OWASP Foundation",
+                publisher="OWASP Foundation",
+                group="owasp-dep-scan",
+                name="blint",
+                version=get_version(),
+                purl=f"pkg:pypi/blint@{get_version()}",
+            )
+        ]
     )
     metadata.lifecycles = [Lifecycles(phase=Phase.post_build)]
     return metadata
 
 
 def generate(src_dirs: list[str], output_file: str, deep_mode: bool) -> bool:
     """
@@ -107,44 +114,48 @@
     exe_files = gen_file_list(src_dirs)
     for src in src_dirs:
         if files := find_android_files(src):
             android_files += files
     if not android_files and not exe_files:
         return False
     with Progress(
-            transient=True,
-            redirect_stderr=True,
-            redirect_stdout=True,
-            refresh_per_second=1,
+        transient=True,
+        redirect_stderr=True,
+        redirect_stdout=True,
+        refresh_per_second=1,
     ) as progress:
         if exe_files:
             task = progress.add_task(
                 f"[green] Parsing {len(exe_files)} binaries",
                 total=len(exe_files),
                 start=True,
             )
         for exe in exe_files:
             progress.update(task, description=f"Processing [bold]{exe}[/bold]", advance=1)
-            components.extend(process_exe_file(dependencies_dict, components, deep_mode, exe, sbom))
+            components += process_exe_file(dependencies_dict, deep_mode, exe, sbom)
         if android_files:
             task = progress.add_task(
                 f"[green] Parsing {len(android_files)} android apps",
                 total=len(android_files),
                 start=True,
             )
         for f in android_files:
             progress.update(task, description=f"Processing [bold]{f}[/bold]", advance=1)
-            components.extend(process_android_file(dependencies_dict, components, deep_mode, f, sbom))
+            components += process_android_file(dependencies_dict, deep_mode, f, sbom)
     if dependencies_dict:
-        dependencies.extend({"ref": k, "dependsOn": list(v)} for k, v in dependencies_dict.items())
+        dependencies += [{"ref": k, "dependsOn": list(v)} for k, v in dependencies_dict.items()]
     return create_sbom(components, dependencies, output_file, sbom, deep_mode)
 
 
 def create_sbom(
-        components: list[Component], dependencies: list[dict], output_file: str, sbom: CycloneDX, deep_mode: bool
+    components: list[Component],
+    dependencies: list[dict],
+    output_file: str,
+    sbom: CycloneDX,
+    deep_mode: bool,
 ) -> bool:
     """
     Creates a Software Bill of Materials (SBOM) with the provided components,
     dependencies, output file, and SBOM object.
 
     Args:
         components (list): A list of Component objects.
@@ -181,26 +192,24 @@
         with open(output_file, mode="w", encoding="utf-8") as fp:
             fp.write(
                 sbom.model_dump_json(
                     indent=None if deep_mode else 2,
                     exclude_none=True,
                     exclude_defaults=True,
                     warnings=False,
-                    by_alias=True
+                    by_alias=True,
                 )
             )
             LOG.debug(f"SBOM file generated successfully at {output_file}")
     else:
-        output_file.write(sbom.model_dump_json(
-            indent=2,
-            exclude_none=True,
-            exclude_defaults=True,
-            warnings=False,
-            by_alias=True
-        ))
+        output_file.write(
+            sbom.model_dump_json(
+                indent=2, exclude_none=True, exclude_defaults=True, warnings=False, by_alias=True
+            )
+        )
     return True
 
 
 def components_from_symbols_version(symbols_version: list[dict]) -> list[Component]:
     """
     Creates a list of Component objects from symbols version.
     This style of detection is quite imprecise since the version is just a min specifier.
@@ -220,149 +229,157 @@
             tmp_a = name.split("_")
             if len(tmp_a) == 2:
                 version = tmp_a[-1]
                 name = tmp_a[0].lower()
                 if name.startswith("glib"):
                     name = name.removeprefix("g")
                     group = "gnu"
-        purl = f"pkg:generic/{group}/{name}@{version}" if group else f"pkg:generic/{name}@{version}"
+        purl = (
+            f"pkg:generic/{group}/{name}@{version}" if group else f"pkg:generic/{name}@{version}"
+        )
         if symbol.get("hash"):
             purl = f"{purl}?hash={symbol.get('hash')}"
         comp = Component(
             type=Type.library,
             group=group,
             name=name,
             version=version,
             purl=purl,
             evidence=create_component_evidence(symbol["name"], 0.5),
-            properties=[
-                Property(name="internal:symbol_version", value=symbol["name"])
-            ]
+            properties=[Property(name="internal:symbol_version", value=symbol["name"])],
         )
         comp.bom_ref = RefType(purl)
         lib_components.append(comp)
     return lib_components
 
 
 def _add_to_parent_component(metadata_components: list[Component], parent_component: Component):
     for mc in metadata_components:
-        if mc.bom_ref.model_dump(mode="python") == parent_component.bom_ref.model_dump(mode="python"):
+        if mc.bom_ref.model_dump(mode="python") == parent_component.bom_ref.model_dump(
+            mode="python"
+        ):
             return
     metadata_components.append(parent_component)
 
 
 def process_exe_file(
-        dependencies_dict: dict[str, set],
-        components: list[Component],
-        deep_mode: bool,
-        exe: str,
-        sbom: CycloneDX,
+    dependencies_dict: dict[str, set],
+    deep_mode: bool,
+    exe: str,
+    sbom: CycloneDX,
 ) -> list[Component]:
     """
     Processes an executable file, extracts metadata, and generates a Software Bill of Materials.
 
     Args:
         dependencies_dict (dict[str, set]): A dictionary of dependencies.
-        components: The list of existing components.
         deep_mode: A flag indicating whether to include deep analysis of the executable.
         exe: The path to the executable file.
         sbom: The CycloneDX SBOM object.
 
     Returns:
         list[Component]: The updated list of components.
 
     """
     metadata: Dict[str, Any] = parse(exe)
     parent_component: Component = default_parent([exe])
     parent_component.properties = []
     lib_components: list[Component] = []
     for prop in (
-            "binary_type",
-            "magic",
-            "class",
-            "platform",
-            "minos",
-            "interpreter",
-            "dylinker",
-            "machine_type",
-            "sdk",
-            "uuid",
-            "cpu_type",
-            "flags",
-            "relro",
-            "is_pie",
-            "is_reproducible_build",
-            "has_nx",
-            "static",
-            "characteristics",
-            "dll_characteristics",
-            "subsystem",
-            "is_gui",
-            "is_driver",
-            "is_dotnet",
-            "major_linker_version",
-            "minor_linker_version",
-            "major_operating_system_version",
-            "minor_operating_system_version",
+        "binary_type",
+        "magic",
+        "class",
+        "platform",
+        "minos",
+        "interpreter",
+        "dylinker",
+        "machine_type",
+        "sdk",
+        "uuid",
+        "cpu_type",
+        "flags",
+        "relro",
+        "is_pie",
+        "is_reproducible_build",
+        "has_nx",
+        "static",
+        "characteristics",
+        "dll_characteristics",
+        "subsystem",
+        "is_gui",
+        "is_driver",
+        "is_dotnet",
+        "major_linker_version",
+        "minor_linker_version",
+        "major_operating_system_version",
+        "minor_operating_system_version",
     ):
         if metadata.get(prop):
             value = str(metadata.get(prop))
             if isinstance(metadata.get(prop), bool):
                 value = value.lower()
             if value:
                 parent_component.properties.append(Property(name=f"internal:{prop}", value=value))
     if metadata.get("notes"):
         for note in metadata.get("notes"):
             if note.get("version"):
                 parent_component.properties.append(
-                    Property(name=f"internal:{note.get('type')}", value=note.get('version')))
-    # For PE binaries, resources could have a dict called version_metadata with interesting properties
+                    Property(name=f"internal:{note.get('type')}", value=note.get("version"))
+                )
+    # For PE, resources could have a dict called version_metadata with interesting properties
     if metadata.get("resources"):
         version_metadata = metadata.get("resources").get("version_metadata")
         if version_metadata and isinstance(version_metadata, dict):
             for vk, vv in version_metadata.items():
                 parent_component.properties.append(
-                    Property(name=f"internal:{camel_to_snake(vk)}", value=vv))
+                    Property(name=f"internal:{camel_to_snake(vk)}", value=vv)
+                )
     if deep_mode:
         symbols_version: list[dict] = metadata.get("symbols_version", [])
         # Attempt to detect library components from the symbols version block
         # If this is unsuccessful then store the information as a property
         lib_components += components_from_symbols_version(symbols_version)
         if not lib_components and symbols_version:
             parent_component.properties.append(
                 Property(
                     name="internal:symbols_version",
                     value=", ".join([f["name"] for f in symbols_version]),
                 )
             )
-        internal_functions = [f["name"] for f in metadata.get("functions", []) if not f["name"].startswith("__")]
+        internal_functions = sorted(
+            {f["name"] for f in metadata.get("functions", []) if f["name"]}
+        )
         if internal_functions:
             parent_component.properties.append(
                 Property(
                     name="internal:functions",
                     value=SYMBOL_DELIMITER.join(internal_functions),
                 )
             )
-        symtab_symbols = [f["name"] for f in metadata.get("symtab_symbols", [])]
+        symtab_symbols = sorted(
+            {f["name"] for f in metadata.get("symtab_symbols", []) if f["name"]}
+        )
         if symtab_symbols:
             parent_component.properties.append(
                 Property(
                     name="internal:symtab_symbols",
                     value=SYMBOL_DELIMITER.join(symtab_symbols),
                 )
             )
-        all_imports = [f["name"] for f in metadata.get("imports", [])]
+        all_imports = sorted({f["name"] for f in metadata.get("imports", [])})
         if all_imports:
             parent_component.properties.append(
                 Property(
                     name="internal:imports",
                     value=SYMBOL_DELIMITER.join(all_imports),
                 )
             )
-        dynamic_symbols = [f["name"] for f in metadata.get("dynamic_symbols", [])]
+        dynamic_symbols = sorted(
+            {f["name"] for f in metadata.get("dynamic_symbols", []) if f["name"]}
+        )
         if dynamic_symbols:
             parent_component.properties.append(
                 Property(
                     name="internal:dynamic_symbols",
                     value=SYMBOL_DELIMITER.join(dynamic_symbols),
                 )
             )
@@ -375,15 +392,17 @@
             lib_components.append(comp)
     if metadata.get("dynamic_entries"):
         for entry in metadata["dynamic_entries"]:
             comp = create_dynamic_component(entry, exe)
             lib_components.append(comp)
     # Convert libraries and targets from dotnet binaries
     if metadata.get("dotnet_dependencies"):
-        pe_components = process_dotnet_dependencies(metadata.get("dotnet_dependencies"), dependencies_dict)
+        pe_components = process_dotnet_dependencies(
+            metadata.get("dotnet_dependencies"), dependencies_dict
+        )
         lib_components += pe_components
     # Convert go dependencies
     if metadata.get("go_dependencies"):
         go_components = process_go_dependencies(metadata.get("go_dependencies"))
         lib_components += go_components
     # Convert go formulation section
     for k, v in metadata.get("go_formulation", {}).items():
@@ -391,21 +410,22 @@
             Property(
                 name=f"internal:{camel_to_snake(k)}",
                 value=str(v).strip(),
             )
         )
     # Convert rust dependencies
     if metadata.get("rust_dependencies"):
-        rust_components = process_rust_dependencies(metadata.get("rust_dependencies"), dependencies_dict)
+        rust_components = process_rust_dependencies(
+            metadata.get("rust_dependencies"), dependencies_dict
+        )
         lib_components += rust_components
     if lib_components:
-        components += lib_components
         track_dependency(dependencies_dict, parent_component, lib_components)
 
-    return components
+    return lib_components
 
 
 def create_library_component(entry: Dict, exe: str) -> Component:
     """
     Processes a library entry and creates a component object.
 
     Args:
@@ -461,63 +481,71 @@
     if entry.get("tag") == "NEEDED":
         comp.scope = Scope.required
     comp.bom_ref = RefType(purl)
     return comp
 
 
 def process_android_file(
-        dependencies_dict: dict[str, set], components: list[Component], deep_mode: bool,
-        f: str, sbom: CycloneDX
+    dependencies_dict: dict[str, set],
+    deep_mode: bool,
+    f: str,
+    sbom: CycloneDX,
 ) -> list[Component]:
     """
     Process an Android file and update the dependencies and components.
 
     Args:
         dependencies_dict (dict[str, set]): Existing dependencies dictionary.
-        components (list): List of components to be processed.
         deep_mode (bool): Flag indicating whether to process in deep mode.
         f (str): File to be processed.
         sbom (obj): Software Bill of Materials object to be updated.
 
     Returns:
         list: Updated components list after processing.
     """
     parent_component, app_components = collect_app_metadata(f, deep_mode)
     if parent_component:
         if not sbom.metadata.component.components:
             sbom.metadata.component.components = []
         _add_to_parent_component(sbom.metadata.component.components, parent_component)
     if app_components:
-        components += app_components
         track_dependency(dependencies_dict, parent_component, app_components)
-    return components
+    return app_components
 
 
-def process_dotnet_dependencies(dotnet_deps: dict[str, dict], dependencies_dict: dict[str, set]) -> list[Component]:
+def process_dotnet_dependencies(
+    dotnet_deps: dict[str, dict], dependencies_dict: dict[str, set]
+) -> list[Component]:
     """
     Process the dotnet dependencies metadata extracted for binary overlays
 
     Args:
         dotnet_deps (dict[str, dict]): PE dependencies metadata
         dependencies_dict (dict[str, set]): Existing dependencies dictionary
 
     Returns:
         list: New component list
     """
     components = []
     libraries = dotnet_deps.get("libraries", {})
     # k: 'Microsoft.CodeAnalysis.Analyzers/3.3.4'
-    # v: {'type': 'package', 'serviceable': True, 'sha512': 'sha512-AxkxcPR+rheX0SmvpLVIGLhOUXAKG56a64kV9VQZ4y9gR9ZmPXnqZvHJnmwLSwzrEP6junUF11vuc+aqo5r68g==', 'path': 'microsoft.codeanalysis.analyzers/3.3.4', 'hashPath': 'microsoft.codeanalysis.analyzers.3.3.4.nupkg.sha512'}
+    # v: {'type': 'package', 'serviceable': True,
+    #      'sha512': 'sha512-AxkxcPR+rheX0SmvpLVIGLhOUXAKG5vuc+aqo5r68g==',
+    #      'path': 'microsoft.codeanalysis.analyzers/3.3.4',
+    #      'hashPath': 'microsoft.codeanalysis.analyzers.3.3.4.nupkg.sha512'
+    #    }
     for k, v in libraries.items():
         tmp_a = k.split("/")
         purl = f"pkg:nuget/{tmp_a[0]}@{tmp_a[1]}"
         hash_content = ""
         try:
-            hash_content = codecs.encode(base64.b64decode(v.get("sha512").removeprefix("sha512-"), validate=True),
-                                         encoding="hex")
+            hash_content = codecs.encode(
+                base64.b64decode(v.get("sha512").removeprefix("sha512-"), validate=True),
+                encoding="hex",
+            )
         except binascii.Error:
             hash_content = str(v.get("hash").removeprefix("sha512-"))
         comp = Component(
             type=Type.application if v.get("type") == "project" else Type.library,
             name=tmp_a[0],
             version=tmp_a[1],
             purl=purl,
@@ -567,31 +595,35 @@
         purl = f"""pkg:golang/{k.lower()}@{v.get("version")}"""
         comp = Component(
             type=Type.library,
             name=k,
             version=v.get("version"),
             purl=purl,
             scope=Scope.required,
-            evidence=create_component_evidence(k, 1.0)
+            evidence=create_component_evidence(k, 1.0),
         )
         hash_content = ""
         if v.get("hash"):
             try:
-                hash_content = codecs.encode(base64.b64decode(v.get("hash").removeprefix("h1:"), validate=True),
-                                             encoding="hex")
+                hash_content = codecs.encode(
+                    base64.b64decode(v.get("hash").removeprefix("h1:"), validate=True),
+                    encoding="hex",
+                )
             except binascii.Error:
                 hash_content = str(v.get("hash").removeprefix("h1:"))
         if hash_content:
             comp.hashes = [Hash(alg=HashAlg.SHA_256, content=hash_content)]
         comp.bom_ref = RefType(f"""pkg:golang/{k}@{v.get("version")}""")
         components.append(comp)
     return components
 
 
-def process_rust_dependencies(rust_deps: list, dependencies_dict: dict[str, set]) -> list[Component]:
+def process_rust_dependencies(
+    rust_deps: list, dependencies_dict: dict[str, set]
+) -> list[Component]:
     """
     Process the rust dependencies metadata extracted for binary overlays
 
     Args:
         rust_deps (list): dependencies metadata
 
     Returns:
@@ -599,36 +631,40 @@
     """
     components = []
     idx_to_purl = {}
     for idx, dep in enumerate(rust_deps):
         idx_to_purl[idx] = f"""pkg:cargo/{dep["name"]}@{dep["version"]}"""
     for dependency in rust_deps:
         purl = f"""pkg:cargo/{dependency["name"]}@{dependency["version"]}"""
-        purl_qualifer = f"""?repository={dependency.get("source")}""" if dependency.get("source", "") != "crates.io" else ""
+        purl_qualifer = (
+            f"""?repository={dependency.get("source")}"""
+            if dependency.get("source", "") != "crates.io"
+            else ""
+        )
         comp = Component(
             type=Type.library,
             name=dependency["name"],
             version=dependency["version"],
             purl=f"{purl}{purl_qualifer}",
             scope=Scope.required,
-            evidence=create_component_evidence(dependency["name"], 0.8)
+            evidence=create_component_evidence(dependency["name"], 0.8),
         )
         comp.bom_ref = RefType(purl)
         components.append(comp)
         if not dependencies_dict.get(purl):
             dependencies_dict[purl] = set()
         # Recover the dependency tree
         if dependency.get("dependencies"):
             for adep in dependency.get("dependencies"):
                 dependencies_dict[purl].add(idx_to_purl[adep])
     return components
 
 
 def track_dependency(
-        dependencies_dict: dict[str, set], parent_component: Component, app_components: list[Component]
+    dependencies_dict: dict[str, set], parent_component: Component, app_components: list[Component]
 ) -> None:
     """
     Track dependencies between components and update the dependencies dict.
 
     Args:
         dependencies_dict (dict[str, set]): The dictionary to store the dependencies.
         parent_component (Component): The parent component.
```

### Comparing `blint-2.1.5/blint/utils.py` & `blint-2.1.6/blint/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import base64
 import binascii
 import math
 import os
 import re
 import shutil
 import string
+import tempfile
 import zipfile
 from importlib.metadata import distribution
 from pathlib import Path
 
+from ar import Archive
 import lief
 from defusedxml.ElementTree import fromstring
 from rich import box
 from rich.table import Table
 
 from blint.config import (
     ignore_directories,
@@ -22,14 +24,17 @@
     secrets_regex
 )
 from blint.cyclonedx.spec import ComponentEvidence, FieldModel, Identity, Method, Technique
 from blint.logger import console, LOG
 
 CHARSET = string.digits + string.ascii_letters + r"""!&@"""
 
+# Known files compressed with ar
+KNOWN_AR_EXTNS = (".a", ".rlib", ".lib")
+
 
 def is_base64(s):
     """
     Checks if the given string is a valid Base64 encoded string.
 
     Args:
         s (str or bytes): The string to be checked.
@@ -247,14 +252,18 @@
     result = []
     for root, dirs, files in os.walk(src):
         filter_ignored_dirs(dirs)
         for file in files:
             if is_ignored_file(file):
                 continue
             full_path = os.path.join(root, file)
+            for ar_extn in KNOWN_AR_EXTNS:
+                if full_path.endswith(ar_extn):
+                    result += extract_ar(full_path)
+                    continue
             if is_exe(full_path):
                 result.append(full_path)
     return result
 
 
 def find_android_files(path):
     """
@@ -269,20 +278,20 @@
 
 def find_files(path, extns):
     """
     Method to find files matching an extension
     """
     result = []
     if os.path.isfile(path):
-        result.extend(path for ext in extns if path.endswith(ext))
+        result += [path for ext in extns if path.endswith(ext)]
     else:
         for root, dirs, files in os.walk(path):
             filter_ignored_dirs(dirs)
             for file in files:
-                result.extend(os.path.join(root, file) for ext in extns if file.endswith(ext))
+                result += [os.path.join(root, file) for ext in extns if file.endswith(ext)]
     return result
 
 
 def bom_strip(manifest):
     """
     Function to delete UTF-8 BOM character in "string"
 
@@ -400,14 +409,18 @@
     for s in src:
         if os.path.isdir(s):
             files += find_exe_files(s)
         else:
             if is_ignored_file(s):
                 continue
             full_path = os.path.abspath(s)
+            for ar_extn in KNOWN_AR_EXTNS:
+                if full_path.endswith(ar_extn):
+                    files += extract_ar(full_path)
+                    continue
             if is_exe(full_path):
                 files.append(full_path)
     return files
 
 
 def unzip_unsafe(zf, to_dir):
     """Method to unzip the file in an unsafe manne"""
@@ -504,7 +517,27 @@
     )
 
 
 def camel_to_snake(name: str) -> str:
     """Convert camelCase to snake_case"""
     name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
     return re.sub('([a-z0-9])([A-Z])', r'\1_\2', name).lower()
+
+
+def extract_ar(ar_file: str, to_dir: str | None = None) -> list[str]:
+    """
+    Extract the given ar compressed files to the directory specified by to_dir.
+    Returns the list of extracted files
+    """
+    if not to_dir:
+        to_dir = tempfile.mkdtemp(prefix="ar-temp-")
+    files_list = []
+    with open(ar_file, 'rb') as fp:
+        with Archive(fp) as archive:
+            for entry in archive:
+                # This workarounds a bug in ar that returns multiple names
+                file_name = entry.name.split("\n")[0].removesuffix("/")
+                afile = os.path.join(to_dir, file_name)
+                with open(afile, 'wb') as output:
+                    output.write(archive.open(entry, 'rb').read())
+                    files_list.append(afile)
+    return files_list
```

### Comparing `blint-2.1.5/pyproject.toml` & `blint-2.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blint"
-version = "2.1.5"
+version = "2.1.6"
 description = "Linter and SBOM generator for binary files."
 authors = ["Prabhu Subramanian <prabhu@appthreat.com>", "Caroline Russell <caroline@appthreat.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/OWASP-dep-scan/blint"
 repository = "https://github.com/OWASP-dep-scan/blint"
 keywords = ["linter", "binary", "security", "sast"]
@@ -32,14 +32,15 @@
 lief = "^0.14.0"
 rich = "^13.7.0"
 PyYAML = "^6.0.1"
 defusedxml = "^0.7.1"
 pydantic = {version = "^2.6.0", extras = ["email"]}
 orjson = "^3.10.1"
 symbolic = "10.2.1"
+ar = "^0.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 black = "^24.0.0"
 flake8 = "^7.0.0"
 pylint = "^3.0.0"
 pytest-cov = "^4.0.0"
```

### Comparing `blint-2.1.5/PKG-INFO` & `blint-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blint
-Version: 2.1.5
+Version: 2.1.6
 Summary: Linter and SBOM generator for binary files.
 Home-page: https://github.com/OWASP-dep-scan/blint
 License: MIT
 Keywords: linter,binary,security,sast
 Author: Prabhu Subramanian
 Author-email: prabhu@appthreat.com
 Requires-Python: >=3.10,<3.13
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: ar (>=0.8,<0.9)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: lief (>=0.14.0,<0.15.0)
 Requires-Dist: orjson (>=3.10.1,<4.0.0)
 Requires-Dist: pydantic[email] (>=2.6.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: symbolic (==10.2.1)
 Project-URL: CI, https://github.com/AppThreat/blint/actions
```

