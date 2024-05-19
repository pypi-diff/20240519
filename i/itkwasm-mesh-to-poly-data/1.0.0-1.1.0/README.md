# Comparing `tmp/itkwasm_mesh_to_poly_data-1.0.0.tar.gz` & `tmp/itkwasm_mesh_to_poly_data-1.1.0.tar.gz`

## Comparing `itkwasm_mesh_to_poly_data-1.0.0.tar` & `itkwasm_mesh_to_poly_data-1.1.0.tar`

### file list

```diff
@@ -1,92 +1,19 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/Makefile
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/conf.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/make.bat
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0  3524105 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/doctrees/apidocs/index.doctree
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/doctrees/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.doctree
--rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/doctrees/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.mesh_to_poly_data.doctree
--rw-r--r--   0        0        0    11085 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/doctrees/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.mesh_to_poly_data_async.doctree
--rw-r--r--   0        0        0    10545 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/doctrees/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.poly_data_to_mesh.doctree
--rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/doctrees/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.poly_data_to_mesh_async.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0    16534 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/genindex.html
--rw-r--r--   0        0        0    16628 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/index.html
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/objects.inv
--rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0    12358 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/search.html
--rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0    60288 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_images/social_previews/summary_apidocs_index_62d49fed.png
--rw-r--r--   0        0        0    57512 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_mesh_to_poly_data_itkwasm_mesh_to_poly_data.mesh_to_poly_data_async_1ce56da9.png
--rw-r--r--   0        0        0    55521 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_mesh_to_poly_data_itkwasm_mesh_to_poly_data.mesh_to_poly_data_cd05fe12.png
--rw-r--r--   0        0        0    57837 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_mesh_to_poly_data_itkwasm_mesh_to_poly_data.poly_data_to_mesh_async_7d0a0b71.png
--rw-r--r--   0        0        0    56108 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_mesh_to_poly_data_itkwasm_mesh_to_poly_data.poly_data_to_mesh_fd224eab.png
--rw-r--r--   0        0        0    64554 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_images/social_previews/summary_apidocs_itkwasm_mesh_to_poly_data_itkwasm_mesh_to_poly_data_64b76d4d.png
--rw-r--r--   0        0        0    65463 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_images/social_previews/summary_index_ed4eec34.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_sources/index.md.txt
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_sources/apidocs/index.rst.txt
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_sources/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.md.txt
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_sources/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.mesh_to_poly_data.md.txt
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_sources/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.mesh_to_poly_data_async.md.txt
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_sources/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.poly_data_to_mesh.md.txt
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_sources/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.poly_data_to_mesh_async.md.txt
--rw-r--r--   0        0        0    48417 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_sphinx_design_static/design-style.1e8bd061cd6da7fc9cf755528e8ffc24.min.css
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_sphinx_design_static/design-tabs.js
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/check-solid.svg
--rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/clipboard.min.js
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/copy-button.svg
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/copybutton.css
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/copybutton.js
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/copybutton_funcs.js
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/debug.css
--rw-r--r--   0        0        0    48417 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/design-style.1e8bd061cd6da7fc9cf755528e8ffc24.min.css
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/design-tabs.js
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/favicon.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/logo.svg
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/skeleton.css
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/scripts/furo-extensions.js
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/scripts/furo.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/scripts/furo.js.LICENSE.txt
--rw-r--r--   0        0        0    28547 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/scripts/furo.js.map
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/styles/furo-extensions.css
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/styles/furo-extensions.css.map
--rw-r--r--   0        0        0    48265 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/styles/furo.css
--rw-r--r--   0        0        0    72791 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/styles/furo.css.map
--rw-r--r--   0        0        0    17206 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/apidocs/index.html
--rw-r--r--   0        0        0    17470 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.html
--rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.mesh_to_poly_data.html
--rw-r--r--   0        0        0    19287 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.mesh_to_poly_data_async.html
--rw-r--r--   0        0        0    18387 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.poly_data_to_mesh.html
--rw-r--r--   0        0        0    19297 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.poly_data_to_mesh_async.html
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/_static/logo.svg
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/apidocs/index.rst
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.mesh_to_poly_data.md
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.mesh_to_poly_data_async.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.poly_data_to_mesh.md
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/docs/apidocs/itkwasm_mesh_to_poly_data/itkwasm_mesh_to_poly_data.poly_data_to_mesh_async.md
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/itkwasm_mesh_to_poly_data/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/itkwasm_mesh_to_poly_data/_version.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/itkwasm_mesh_to_poly_data/mesh_to_poly_data.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/itkwasm_mesh_to_poly_data/mesh_to_poly_data_async.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/itkwasm_mesh_to_poly_data/poly_data_to_mesh.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/itkwasm_mesh_to_poly_data/poly_data_to_mesh_async.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/tests/test_itkwasm_mesh_to_poly_data_async.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/tests/test_mesh_to_poly_data.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/.gitignore
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/README.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/docs/_static/favicon.png
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/itkwasm_mesh_to_poly_data/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/itkwasm_mesh_to_poly_data/_version.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/itkwasm_mesh_to_poly_data/mesh_to_poly_data.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/itkwasm_mesh_to_poly_data/mesh_to_poly_data_async.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/itkwasm_mesh_to_poly_data/poly_data_to_mesh.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/itkwasm_mesh_to_poly_data/poly_data_to_mesh_async.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/tests/test_itkwasm_mesh_to_poly_data_async.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/tests/test_mesh_to_poly_data.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/.gitignore
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/README.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data-1.1.0/PKG-INFO
```

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/docs/Makefile` & `itkwasm_mesh_to_poly_data-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/docs/conf.py` & `itkwasm_mesh_to_poly_data-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/docs/index.md` & `itkwasm_mesh_to_poly_data-1.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/docs/make.bat` & `itkwasm_mesh_to_poly_data-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/favicon.png` & `itkwasm_mesh_to_poly_data-1.1.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/docs/_build/html/_static/logo.svg` & `itkwasm_mesh_to_poly_data-1.1.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/itkwasm_mesh_to_poly_data/mesh_to_poly_data_async.py` & `itkwasm_mesh_to_poly_data-1.1.0/itkwasm_mesh_to_poly_data/mesh_to_poly_data_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/itkwasm_mesh_to_poly_data/poly_data_to_mesh.py` & `itkwasm_mesh_to_poly_data-1.1.0/itkwasm_mesh_to_poly_data/poly_data_to_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/itkwasm_mesh_to_poly_data/poly_data_to_mesh_async.py` & `itkwasm_mesh_to_poly_data-1.1.0/itkwasm_mesh_to_poly_data/poly_data_to_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/tests/test_itkwasm_mesh_to_poly_data_async.py` & `itkwasm_mesh_to_poly_data-1.1.0/tests/test_itkwasm_mesh_to_poly_data_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/tests/test_mesh_to_poly_data.py` & `itkwasm_mesh_to_poly_data-1.1.0/tests/test_mesh_to_poly_data.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/pyproject.toml` & `itkwasm_mesh_to_poly_data-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data-1.0.0/PKG-INFO` & `itkwasm_mesh_to_poly_data-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: itkwasm-mesh-to-poly-data
-Version: 1.0.0
+Version: 1.1.0
 Summary: Convert an ITK Mesh to a simple data structure compatible with vtkPolyData.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/ITKMeshToPolyData
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/ITKMeshToPolyData
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

