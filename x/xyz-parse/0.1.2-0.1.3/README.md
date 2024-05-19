# Comparing `tmp/xyz_parse-0.1.2.tar.gz` & `tmp/xyz_parse-0.1.3.tar.gz`

## Comparing `xyz_parse-0.1.2.tar` & `xyz_parse-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 xyz_parse-0.1.2/Cargo.toml
--rw-r--r--   0     1001      127     2674 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/.github/workflows/cd.yaml
--rw-r--r--   0     1001      127      583 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/.github/workflows/ci.yaml
--rw-r--r--   0     1001      127      697 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/.gitignore
--rw-r--r--   0     1001      127      308 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/README.md
--rw-r--r--   0     1001      127     3214 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/src/atom.rs
--rw-r--r--   0     1001      127      572 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/src/lib.rs
--rw-r--r--   0     1001      127     4699 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/src/molecule.rs
--rw-r--r--   0     1001      127     4664 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/src/python.rs
--rw-r--r--   0     1001      127     8048 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/src/xyz.rs
--rw-r--r--   0     1001      127     8787 2024-05-17 14:42:03.000000 xyz_parse-0.1.2/Cargo.lock
--rw-r--r--   0     1001      127      375 2024-05-17 14:41:59.000000 xyz_parse-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 xyz_parse-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 xyz_parse-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      127     2674 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/.github/workflows/cd.yaml
+-rw-r--r--   0     1001      127      583 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/.github/workflows/ci.yaml
+-rw-r--r--   0     1001      127      697 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/.gitignore
+-rw-r--r--   0     1001      127      308 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/README.md
+-rw-r--r--   0     1001      127     3214 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/src/atom.rs
+-rw-r--r--   0     1001      127      593 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      127     5007 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/src/molecule.rs
+-rw-r--r--   0     1001      127     6177 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/src/python.rs
+-rw-r--r--   0     1001      127     8048 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/src/xyz.rs
+-rw-r--r--   0     1001      127     8787 2024-05-19 13:28:38.000000 xyz_parse-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      127      377 2024-05-19 13:28:34.000000 xyz_parse-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 xyz_parse-0.1.3/PKG-INFO
```

### Comparing `xyz_parse-0.1.2/Cargo.toml` & `xyz_parse-0.1.3/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "xyz-parse"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 authors = ["Julian Popescu <jpopesculian@gmail.com>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/aqora-io/xyz-parse"
 documentation = "https://docs.rs/xyz-parse/"
 repository = "https://github.com/aqora-io/xyz-parse"
@@ -15,12 +15,12 @@
 [lib]
 path = "src/lib.rs"
 name = "xyz_parse"
 crate-type = ["cdylib"]
 
 [features]
 default = []
-python = ["pyo3"]
+pyo3-lib = ["pyo3", "pyo3/extension-module", "pyo3/abi3-py37"]
 
 [dependencies]
 rust_decimal = { version = "1.35", default-features = false }
-pyo3 = { version = "0.21", features = ["rust_decimal", "extension-module", "abi3-py37"], optional = true }
+pyo3 = { version = "0.21", features = ["rust_decimal"], optional = true }
```

### Comparing `xyz_parse-0.1.2/.github/workflows/cd.yaml` & `xyz_parse-0.1.3/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.2/.github/workflows/ci.yaml` & `xyz_parse-0.1.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.2/.gitignore` & `xyz_parse-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.2/src/atom.rs` & `xyz_parse-0.1.3/src/atom.rs`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.2/src/lib.rs` & `xyz_parse-0.1.3/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 //!
 //! Currently the parser does not support extended XYZ format, but may do so in the future
 
 mod atom;
 mod molecule;
 mod xyz;
 
-#[cfg(feature = "python")]
+#[cfg(feature = "pyo3")]
 mod python;
 
+pub use rust_decimal;
+
 pub use atom::*;
 pub use molecule::*;
 pub use xyz::*;
 
 /// Parse an [`Xyz`] string
 pub fn parse_xyz(s: &str) -> Result<Xyz, XyzParseError> {
     Xyz::parse(s)
```

### Comparing `xyz_parse-0.1.2/src/molecule.rs` & `xyz_parse-0.1.3/src/molecule.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use crate::atom::{Atom, AtomParseError};
+use rust_decimal::Decimal;
 use std::{borrow::Cow, error::Error, fmt, str::FromStr};
 
 /// An error that can occur when parsing a [`Molecule`]
 #[derive(Debug, Clone)]
 pub enum MoleculeParseError<'a> {
     NoAtomNumber,
     InvalidAtomNumber(Cow<'a, str>, std::num::ParseIntError),
@@ -115,14 +116,22 @@
             atoms: self
                 .atoms
                 .into_iter()
                 .map(|atom| atom.into_owned())
                 .collect(),
         }
     }
+
+    pub fn symbols(&self) -> impl ExactSizeIterator<Item = &str> {
+        self.atoms.iter().map(|atom| atom.symbol.as_ref())
+    }
+
+    pub fn coordinates(&self) -> impl ExactSizeIterator<Item = [Decimal; 3]> + '_ {
+        self.atoms.iter().map(|atom| atom.coordinates())
+    }
 }
 
 impl<'a> fmt::Display for Molecule<'a> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         writeln!(f, "{}", self.atoms.len())?;
         write!(f, "{}", self.comment)?;
         for atom in &self.atoms {
```

### Comparing `xyz_parse-0.1.2/src/xyz.rs` & `xyz_parse-0.1.3/src/xyz.rs`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.2/Cargo.lock` & `xyz_parse-0.1.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
@@ -311,12 +311,12 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xyz-parse"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "pyo3",
  "rust_decimal",
 ]
```

### Comparing `xyz_parse-0.1.2/PKG-INFO` & `xyz_parse-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xyz-parse
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Simple parser for the XYZ file format
 Keywords: xyz,chemistry,parser,parse
 Home-Page: https://github.com/aqora-io/xyz-parse
 Author: Julian Popescu <jpopesculian@gmail.com>
```

