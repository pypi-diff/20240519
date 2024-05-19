# Comparing `tmp/coldp-2024.5.3.tar.gz` & `tmp/coldp-2024.5.4.tar.gz`

## Comparing `coldp-2024.5.3.tar` & `coldp-2024.5.4.tar`

### file list

```diff
@@ -1,103 +1,106 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 coldp-2024.5.3/.gitattributes
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 coldp-2024.5.3/VERSION
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coldp-2024.5.3/makefile
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coldp-2024.5.3/version.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/make.bat
--rw-r--r--   0        0        0   118424 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/coldp.html
--rw-r--r--   0        0        0    30155 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/genindex.html
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/index.html
--rw-r--r--   0        0        0    13606 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/name-bundle.html
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/objects.inv
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/search.html
--rw-r--r--   0        0        0    26118 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    21622 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/usage.html
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/alabaster.css
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/file.png
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/sphinx_paramlinks.css
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/.buildinfo
--rw-r--r--   0        0        0   215766 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/COLDP.pdf
--rw-r--r--   0        0        0   258568 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/index.html
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/objects.inv
--rw-r--r--   0        0        0    16018 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/doctools.js
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/file.png
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/language_data.js
--rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/main.css
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/plus.png
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/pygments.css
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/sphinx_highlight.js
--rw-r--r--   0        0        0   201708 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraMono-Bold.ttf
--rw-r--r--   0        0        0   169056 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraMono-Medium.ttf
--rw-r--r--   0        0        0   170204 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraMono-Regular.ttf
--rw-r--r--   0        0        0   521796 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Bold.otf
--rw-r--r--   0        0        0   524840 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Italic.otf
--rw-r--r--   0        0        0   505308 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Light.otf
--rw-r--r--   0        0        0   522236 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-LightItalic.otf
--rw-r--r--   0        0        0   507828 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Regular.otf
--rw-r--r--   0        0        0   192304 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/WorkSans-Bold.ttf
--rw-r--r--   0        0        0   191916 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/WorkSans-Regular.ttf
--rw-r--r--   0        0        0   192372 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/WorkSans-SemiBold.ttf
--rw-r--r--   0        0        0   194078 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.eot
--rw-r--r--   0        0        0   849240 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.svg
--rw-r--r--   0        0        0   193792 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.ttf
--rw-r--r--   0        0        0    99004 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.woff
--rw-r--r--   0        0        0    76120 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_admonition.scss
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_alerts.scss
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_api.scss
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_back-cover.scss
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_blocks.scss
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_code.scss
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_cover.scss
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_fonts.scss
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_lists.scss
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_needs.scss
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_pages.scss
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_tables.scss
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_text.scss
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_toc.scss
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_variables.scss
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/main.scss
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/coldp.rst
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/conf.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/index.pdf
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/index.rst
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/name-bundle.rst
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/usage.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 coldp-2024.5.3/src/coldp/__init__.py
--rw-r--r--   0        0        0   113448 2020-02-02 00:00:00.000000 coldp-2024.5.3/src/coldp/coldp.py
--rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 coldp-2024.5.3/src/coldp/coldp_distribution.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 coldp-2024.5.3/src/coldp/testit.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/test_coldp.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/Distribution.tsv
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/Media.tsv
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/NameRelation.tsv
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/NameUsage.tsv
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/Reference.tsv
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/SpeciesEstimate.tsv
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/SpeciesInteraction.tsv
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/TaxonConceptRelation.tsv
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/TypeMaterial.tsv
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/VernacularName.tsv
--rw-r--r--   0        0        0   697219 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/logo.png
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/metadata.yaml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/reference.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 coldp-2024.5.3/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coldp-2024.5.3/LICENSE
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 coldp-2024.5.3/README.md
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 coldp-2024.5.3/pyproject.toml
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 coldp-2024.5.3/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 coldp-2024.5.4/.gitattributes
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 coldp-2024.5.4/VERSION
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coldp-2024.5.4/makefile
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coldp-2024.5.4/version.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/make.bat
+-rw-r--r--   0        0        0   123233 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/coldp.html
+-rw-r--r--   0        0        0    32447 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/identifier-policy.html
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/index.html
+-rw-r--r--   0        0        0    13780 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/name-bundle.html
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/search.html
+-rw-r--r--   0        0        0    28258 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    21762 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/usage.html
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/.buildinfo
+-rw-r--r--   0        0        0   226469 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/COLDP.pdf
+-rw-r--r--   0        0        0   283336 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/index.html
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/objects.inv
+-rw-r--r--   0        0        0    16018 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/doctools.js
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/language_data.js
+-rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/main.css
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/plus.png
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0   201708 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraMono-Bold.ttf
+-rw-r--r--   0        0        0   169056 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraMono-Medium.ttf
+-rw-r--r--   0        0        0   170204 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraMono-Regular.ttf
+-rw-r--r--   0        0        0   521796 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-Bold.otf
+-rw-r--r--   0        0        0   524840 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-Italic.otf
+-rw-r--r--   0        0        0   505308 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-Light.otf
+-rw-r--r--   0        0        0   522236 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-LightItalic.otf
+-rw-r--r--   0        0        0   507828 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-Regular.otf
+-rw-r--r--   0        0        0   192304 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/WorkSans-Bold.ttf
+-rw-r--r--   0        0        0   191916 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/WorkSans-Regular.ttf
+-rw-r--r--   0        0        0   192372 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/WorkSans-SemiBold.ttf
+-rw-r--r--   0        0        0   194078 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   849240 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   193792 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0    99004 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    76120 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_admonition.scss
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_alerts.scss
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_api.scss
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_back-cover.scss
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_blocks.scss
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_code.scss
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_cover.scss
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_fonts.scss
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_lists.scss
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_needs.scss
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_pages.scss
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_tables.scss
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_text.scss
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_toc.scss
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_variables.scss
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/main.scss
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/source/coldp.rst
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/source/conf.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/source/identifier-policy.rst
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/source/index.pdf
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/source/index.rst
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/source/name-bundle.rst
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 coldp-2024.5.4/docs/source/usage.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 coldp-2024.5.4/src/coldp/__init__.py
+-rw-r--r--   0        0        0   121846 2020-02-02 00:00:00.000000 coldp-2024.5.4/src/coldp/coldp.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 coldp-2024.5.4/src/coldp/coldp_add.py
+-rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 coldp-2024.5.4/src/coldp/coldp_distribution.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 coldp-2024.5.4/src/coldp/testit.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/test_coldp.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/Distribution.tsv
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/Media.tsv
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/NameRelation.tsv
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/NameUsage.tsv
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/Reference.tsv
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/SpeciesEstimate.tsv
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/SpeciesInteraction.tsv
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/TaxonConceptRelation.tsv
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/TypeMaterial.tsv
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/VernacularName.tsv
+-rw-r--r--   0        0        0   697219 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/logo.png
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/metadata.yaml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.4/test/input/Tonzidae/reference.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 coldp-2024.5.4/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coldp-2024.5.4/LICENSE
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 coldp-2024.5.4/README.md
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 coldp-2024.5.4/pyproject.toml
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 coldp-2024.5.4/PKG-INFO
```

### Comparing `coldp-2024.5.3/makefile` & `coldp-2024.5.4/makefile`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/version.py` & `coldp-2024.5.4/version.py`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/Makefile` & `coldp-2024.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/make.bat` & `coldp-2024.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/html/coldp.html` & `coldp-2024.5.4/docs/build/html/coldp.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>coldp.COLDP &#8212; COLDP 2024.5.3 documentation</title>
+    <title>coldp.COLDP &#8212; COLDP 2024.5.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
+    <script src="_static/documentation_options.js?v=78d2dd00"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="coldp.NameBundle" href="name-bundle.html" />
     <link rel="prev" title="coldp" href="index.html" />
    
@@ -57,15 +57,15 @@
 <li><p><span class="target" id="coldp.COLDP.params.allow_repeated_binomials"></span><strong>allow_repeated_binomials</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.params.allow_repeated_binomials">¶</a> – If true, omit checks rejecting the addition of the same binomial more than once to the COLDP name dataframe.</p></li>
 <li><p><span class="target" id="coldp.COLDP.params.create_taxa_for_not_established"></span><strong>create_taxa_for_not_established</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.params.create_taxa_for_not_established">¶</a> – If true, generate taxon records even if the associated name is flagged as not established (i.e. not satisfying the relevant nomenclatural code)</p></li>
 <li><p><span class="target" id="coldp.COLDP.params.issues_to_stdout"></span><strong>issues_to_stdout</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.params.issues_to_stdout">¶</a> – If true, print any issue messages (see <a class="reference internal" href="#coldp.COLDP.issue" title="coldp.COLDP.issue"><code class="xref py py-func docutils literal notranslate"><span class="pre">issue()</span></code></a>) to stdout as well as inserting then in the issue dataframe.</p></li>
 <li><p><span class="target" id="coldp.COLDP.params.context"></span><strong>context</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.params.context">¶</a> – Value to be used in labeling issue records (see <a class="reference internal" href="#coldp.COLDP.issue" title="coldp.COLDP.issue"><code class="xref py py-func docutils literal notranslate"><span class="pre">issue()</span></code></a>). This value is more normally set using <a class="reference internal" href="#coldp.COLDP.set_context" title="coldp.COLDP.set_context"><code class="xref py py-func docutils literal notranslate"><span class="pre">set_context()</span></code></a>.</p></li>
 </ul>
 </dd>
 </dl>
-<p>A COLDP object is initalised with a source/destination folder, COLDP package
+<p>A COLDP object is initialised with a source/destination folder, COLDP package
 name and other options.</p>
 <p>If a subfolder exists with the supplied name in the supplied folder, it
 will be initialised with data from any CSV/TSV files it contains with any
 of the following base names: name, taxon, synonym, reference,
 distribution, speciesinteraction, namerelation, typematerial or nameusage,
 and with a file extension recognised via <code class="xref py py-data docutils literal notranslate"><span class="pre">csv_extensions</span></code>.
 File names are case insensitive.</p>
@@ -210,15 +210,15 @@
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>Updated <a class="reference internal" href="#coldp.COLDP.add_references.params.reference_list" title="coldp.COLDP.add_references"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">reference_list</span></code></a> with IDs for references in this COLDP instance</p>
 </dd>
 </dl>
 <p>Find existing ID values for each supplied reference, based on identity
 of: author, title, issued, containerTitle, volume, issue, page and citation. Add
-ID to the appropriate reference dictionary in references. If none
+ID from the appropriate reference dictionary in references. If none
 found, set ID to next unused index and add to references.</p>
 <p>The list is returned updated with current ID values so these can be used for referenceID values in other classes.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.add_type_material">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">add_type_material</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">type_material</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.add_type_material" title="Link to this definition">¶</a></dt>
@@ -357,14 +357,33 @@
 Any numpy NAN elements are replaced with an empty string.</p>
 </dd></dl>
 
 </section>
 <section id="find-or-get-records">
 <h3>Find or get records<a class="headerlink" href="#find-or-get-records" title="Link to this heading">¶</a></h3>
 <dl class="py method">
+<dt class="sig sig-object py" id="coldp.COLDP.find_taxon">
+<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_taxon</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">scientificName</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">authorship</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rank</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_taxon" title="Link to this definition">¶</a></dt>
+<dd><p>Get COLDP Taxon record (as Pandas dataframe) with accepted name matching supplied scientificName, authorship and rank values</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.find_taxon.params.scientificName"></span><strong>scientificName</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.scientificName">¶</a> – Scientific name in canonical format</p></li>
+<li><p><span class="target" id="coldp.COLDP.find_taxon.params.authorship"></span><strong>authorship</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.authorship">¶</a> – Authorship string</p></li>
+<li><p><span class="target" id="coldp.COLDP.find_taxon.params.rank"></span><strong>rank</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.rank">¶</a> – Rank name string</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>COLDP Taxon record matching supplied parameters</p>
+</dd>
+</dl>
+<p>Logs a warning issue if multiple taxon records exist for a matching name and returns the first such match. Returns None if no match.</p>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.find_name_record">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_name_record</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_name_record" title="Link to this definition">¶</a></dt>
 <dd><p>Return record from names DataFrame matching key fields (scientificName,
 authorship and rank) in supplied record</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="coldp.COLDP.find_name_record.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name_record.params.name">¶</a> – Dictionary containing Name properties</p>
@@ -393,14 +412,38 @@
 <dd class="field-even"><p>Set of COLDP Name records either as DataFrame or list of dictionaries</p>
 </dd>
 </dl>
 <p>Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches, None is returned.</p>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="coldp.COLDP.find_name">
+<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_name</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">scientificName</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">authorship</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rank</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_name" title="Link to this definition">¶</a></dt>
+<dd><p>Return record from names DataFrame matching supplied scientificName,
+authorship and rank</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.find_name.params.scientificName"></span><strong>scientificName</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.scientificName">¶</a> – Scientific name in canonical format</p></li>
+<li><p><span class="target" id="coldp.COLDP.find_name.params.authorship"></span><strong>authorship</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.authorship">¶</a> – Authorship string</p></li>
+<li><p><span class="target" id="coldp.COLDP.find_name.params.rank"></span><strong>rank</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.rank">¶</a> – Rank name string</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>Dictionary containing matching record if found</p>
+</dd>
+</dl>
+<p>Locates any existing record in the names DataFrame that matches the
+supplied scientificName, authorship and rank and returns it as a
+COLDP Name properties dictionary, or None if no match is found.</p>
+<p>If <a class="reference internal" href="#coldp.COLDP.find_name.params.authorship" title="coldp.COLDP.find_name"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">authorship</span></code></a> is None, returns a
+name based only on scientificName and rank.</p>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.find_distribution">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_distribution</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">distribution</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_distribution" title="Link to this definition">¶</a></dt>
 <dd><p>Locate existing COLDP distribution record exactly matching all major
 fields in <a class="reference internal" href="#coldp.COLDP.find_distribution.params.distribution" title="coldp.COLDP.find_distribution"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">distribution</span></code></a></p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="coldp.COLDP.find_distribution.params.distribution"></span><strong>distribution</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_distribution.params.distribution">¶</a> – Dictionary of COLDP distribution properties representing a record to be found</p>
@@ -622,14 +665,46 @@
 </dl>
 <p>The tree view shows the name, authorship and rank for the selected taxon.
 Synonyms follow, one to a row at the same indent level but preceded by a
 space and an asterisk. Then each child follows, indented two more spaces per level,
 with its own synonyms and children following.</p>
 </dd></dl>
 
+<dl class="py method">
+<dt class="sig sig-object py" id="coldp.COLDP.get_available_column_headings">
+<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">get_available_column_headings</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.get_available_column_headings" title="Link to this definition">¶</a></dt>
+<dd><p>Return dictionary mapping table names to lists of supported columns</p>
+<dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>Dictionary containing copies of internal heading lists</p>
+</dd>
+</dl>
+<p>Returns copies to avoid corrupting the lists used in this class</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="coldp.COLDP.get_identifier_policy">
+<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">get_identifier_policy</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">table_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">default_prefix</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">required</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">volatile</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.get_identifier_policy" title="Link to this definition">¶</a></dt>
+<dd><p>Find or create <code class="xref py py-class docutils literal notranslate"><span class="pre">IdentifierPolicy</span></code> associated with named table</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.get_identifier_policy.params.table_name"></span><strong>table_name</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_identifier_policy.params.table_name">¶</a> – Name of COLDP dataframe for which policy is required</p></li>
+<li><p><span class="target" id="coldp.COLDP.get_identifier_policy.params.default_prefix"></span><strong>default_prefix</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_identifier_policy.params.default_prefix">¶</a> – String prefix to use before numeric ID values if existing ID values are not consistently positive integer values</p></li>
+<li><p><span class="target" id="coldp.COLDP.get_identifier_policy.params.required"></span><strong>required</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_identifier_policy.params.required">¶</a> – Flag to indicate whether the table must have ID values - if False, the <code class="xref py py-class docutils literal notranslate"><span class="pre">IdentifierPolicy</span></code> will return None unless <a class="reference internal" href="identifier-policy.html#coldp.IdentifierPolicy.__init__.params.existing" title="coldp.IdentifierPolicy.__init__"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">existing</span></code></a> already contains ID values</p></li>
+<li><p><span class="target" id="coldp.COLDP.get_identifier_policy.params.volatile"></span><strong>volatile</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_identifier_policy.params.volatile">¶</a> – Flag to indicate if external code may modify ID values while the current COLDP instance is active - if False, the policy and future values will be determined on initialisation, otherwise the policy will be reviewed for each new ID value</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p><code class="xref py py-class docutils literal notranslate"><span class="pre">IdentifierPolicy</span></code> object or None if no policy is required for the table</p>
+</dd>
+</dl>
+<p>Creates new <code class="xref py py-class docutils literal notranslate"><span class="pre">IdentifierPolicy</span></code> instance if this is the first invocation for the given table. Policies take into account any existing ID values for the table.</p>
+</dd></dl>
+
 </section>
 <section id="access-to-dataframes">
 <h3>Access to DataFrames<a class="headerlink" href="#access-to-dataframes" title="Link to this heading">¶</a></h3>
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.table_by_name">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">table_by_name</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.table_by_name" title="Link to this definition">¶</a></dt>
 <dd><p>Return dataframe for named COLDP data class</p>
@@ -977,57 +1052,14 @@
 <dd class="field-even"><p></p>
 </dd>
 </dl>
 <p>Returns name following any updates.</p>
 </dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="coldp.COLDP.find_name">
-<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_name</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">scientificName</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">authorship</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rank</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_name" title="Link to this definition">¶</a></dt>
-<dd><p>Return record from names DataFrame matching supplied scientificName,
-authorship and rank</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><span class="target" id="coldp.COLDP.find_name.params.scientificName"></span><strong>scientificName</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.scientificName">¶</a> – Scientific name in canonical format</p></li>
-<li><p><span class="target" id="coldp.COLDP.find_name.params.authorship"></span><strong>authorship</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.authorship">¶</a> – Authorship string</p></li>
-<li><p><span class="target" id="coldp.COLDP.find_name.params.rank"></span><strong>rank</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.rank">¶</a> – Rank name string</p></li>
-</ul>
-</dd>
-<dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>Dictionary containing matching record if found</p>
-</dd>
-</dl>
-<p>Locates any existing record in the names DataFrame that matches the
-supplied scientificName, authorship and rank and returns it as a
-COLDP Name properties dictionary, or None if no match is found.</p>
-<p>If <a class="reference internal" href="#coldp.COLDP.find_name.params.authorship" title="coldp.COLDP.find_name"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">authorship</span></code></a> is None, returns a
-name based only on scientificName and rank.</p>
-</dd></dl>
-
-<dl class="py method">
-<dt class="sig sig-object py" id="coldp.COLDP.find_taxon">
-<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_taxon</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">scientificName</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">authorship</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rank</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_taxon" title="Link to this definition">¶</a></dt>
-<dd><p>Get COLDP Taxon record (as Pandas dataframe) with accepted name matching supplied scientificName, authorship and rank values</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><span class="target" id="coldp.COLDP.find_taxon.params.scientificName"></span><strong>scientificName</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.scientificName">¶</a> – Scientific name in canonical format</p></li>
-<li><p><span class="target" id="coldp.COLDP.find_taxon.params.authorship"></span><strong>authorship</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.authorship">¶</a> – Authorship string</p></li>
-<li><p><span class="target" id="coldp.COLDP.find_taxon.params.rank"></span><strong>rank</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.rank">¶</a> – Rank name string</p></li>
-</ul>
-</dd>
-<dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>COLDP Taxon record matching supplied parameters</p>
-</dd>
-</dl>
-<p>Logs a warning issue if multiple taxon records exist for a matching name and returns the first such match. Returns None if no match.</p>
-</dd></dl>
-
-<dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.construct_species_rank_name">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">construct_species_rank_name</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">g</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sg</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">s</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ss</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">marker</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.construct_species_rank_name" title="Link to this definition">¶</a></dt>
 <dd><p>Consistently construct a species or infraspecific name from the included epithets and optional rank marker</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="coldp.COLDP.construct_species_rank_name.params.g"></span><strong>g</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.construct_species_rank_name.params.g">¶</a> – Genus name</p></li>
@@ -1152,14 +1184,15 @@
 <li class="toctree-l2"><a class="reference internal" href="#methods">Methods</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#constants">Constants</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#internal-methods">Internal methods</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#index-and-search">Index and search</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="name-bundle.html">coldp.NameBundle</a></li>
+<li class="toctree-l1"><a class="reference internal" href="identifier-policy.html">coldp.IdentifierPolicy</a></li>
 </ul>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
 </ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
```

#### html2text {}

```diff
@@ -70,15 +70,15 @@
                   code)
                 * iissssuueess__ttoo__ssttddoouutt_¶ – If true, print any issue messages (see
                   _i_s_s_u_e_(_)) to stdout as well as inserting then in the issue
                   dataframe.
                 * ccoonntteexxtt_¶ – Value to be used in labeling issue records (see
                   _i_s_s_u_e_(_)). This value is more normally set using _s_e_t___c_o_n_t_e_x_t
                   _(_).
-      A COLDP object is initalised with a source/destination folder, COLDP
+      A COLDP object is initialised with a source/destination folder, COLDP
       package name and other options.
       If a subfolder exists with the supplied name in the supplied folder, it
       will be initialised with data from any CSV/TSV files it contains with any
       of the following base names: name, taxon, synonym, reference,
       distribution, speciesinteraction, namerelation, typematerial or
       nameusage, and with a file extension recognised via csv_extensions. File
       names are case insensitive.
@@ -186,15 +186,15 @@
             rreeffeerreennccee__lliisstt_¶ – List of dictionaries - each dictionary contains
             values keyed by terms from reference_headings
         Returns:
             Updated _r_e_f_e_r_e_n_c_e___l_i_s_t with IDs for references in this COLDP
             instance
       Find existing ID values for each supplied reference, based on identity
       of: author, title, issued, containerTitle, volume, issue, page and
-      citation. Add ID to the appropriate reference dictionary in references.
+      citation. Add ID from the appropriate reference dictionary in references.
       If none found, set ID to next unused index and add to references.
       The list is returned updated with current ID values so these can be used
       for referenceID values in other classes.
   COLDP.add_type_material(ttyyppee__mmaatteerriiaall)_¶
       Add COLDP TypeMaterial record to COLDP instance
         Parameters:
             ttyyppee__mmaatteerriiaall_¶ – COLDP TypeMaterial record represented as
@@ -273,14 +273,25 @@
                   name supplied to constructor, which defaults to None. If no
                   name provided, save will fail.
       If necessary creates subfolder with name _n_a_m_e in _d_e_s_t_i_n_a_t_i_o_n, and then
       writes CSV file representations for all DataFrames in the folder. Empty
       columns are dropped. Any numpy NAN elements are replaced with an empty
       string.
 ******** FFiinndd oorr ggeett rreeccoorrddss_?¶ ********
+  COLDP.find_taxon(sscciieennttiiffiiccNNaammee, aauutthhoorrsshhiipp, rraannkk)_¶
+      Get COLDP Taxon record (as Pandas dataframe) with accepted name matching
+      supplied scientificName, authorship and rank values
+        Parameters:
+                * sscciieennttiiffiiccNNaammee_¶ – Scientific name in canonical format
+                * aauutthhoorrsshhiipp_¶ – Authorship string
+                * rraannkk_¶ – Rank name string
+        Returns:
+            COLDP Taxon record matching supplied parameters
+      Logs a warning issue if multiple taxon records exist for a matching name
+      and returns the first such match. Returns None if no match.
   COLDP.find_name_record(nnaammee)_¶
       Return record from names DataFrame matching key fields (scientificName,
       authorship and rank) in supplied record
         Parameters:
             nnaammee_¶ – Dictionary containing Name properties
         Returns:
             Dictionary containing matching record if found
@@ -295,14 +306,28 @@
                 * ttoo__ddiicctt_¶ – True if records should be converted from Pandas
                   format to dictionary records, False (default) otherwise.
         Returns:
             Set of COLDP Name records either as DataFrame or list of
             dictionaries
       Returns all matching records as Pandas DataFrame or list of dictionaries.
       If no matches, None is returned.
+  COLDP.find_name(sscciieennttiiffiiccNNaammee, aauutthhoorrsshhiipp, rraannkk)_¶
+      Return record from names DataFrame matching supplied scientificName,
+      authorship and rank
+        Parameters:
+                * sscciieennttiiffiiccNNaammee_¶ – Scientific name in canonical format
+                * aauutthhoorrsshhiipp_¶ – Authorship string
+                * rraannkk_¶ – Rank name string
+        Returns:
+            Dictionary containing matching record if found
+      Locates any existing record in the names DataFrame that matches the
+      supplied scientificName, authorship and rank and returns it as a COLDP
+      Name properties dictionary, or None if no match is found.
+      If _a_u_t_h_o_r_s_h_i_p is None, returns a name based only on scientificName and
+      rank.
   COLDP.find_distribution(ddiissttrriibbuuttiioonn)_¶
       Locate existing COLDP distribution record exactly matching all major
       fields in _d_i_s_t_r_i_b_u_t_i_o_n
         Parameters:
             ddiissttrriibbuuttiioonn_¶ – Dictionary of COLDP distribution properties
             representing a record to be found
         Returns:
@@ -439,14 +464,42 @@
                   defaults to an equal sign with spaces on either side
         Returns:
             Multiline string representation of taxonomic hierarchy
       The tree view shows the name, authorship and rank for the selected taxon.
       Synonyms follow, one to a row at the same indent level but preceded by a
       space and an asterisk. Then each child follows, indented two more spaces
       per level, with its own synonyms and children following.
+  COLDP.get_available_column_headings()_¶
+      Return dictionary mapping table names to lists of supported columns
+        Returns:
+            Dictionary containing copies of internal heading lists
+      Returns copies to avoid corrupting the lists used in this class
+  COLDP.get_identifier_policy(ttaabbllee__nnaammee, ddeeffaauulltt__pprreeffiixx==NNoonnee, rreeqquuiirreedd==TTrruuee,
+  vvoollaattiillee==FFaallssee)_¶
+      Find or create IdentifierPolicy associated with named table
+        Parameters:
+                * ttaabbllee__nnaammee_¶ – Name of COLDP dataframe for which policy is
+                  required
+                * ddeeffaauulltt__pprreeffiixx_¶ – String prefix to use before numeric ID
+                  values if existing ID values are not consistently positive
+                  integer values
+                * rreeqquuiirreedd_¶ – Flag to indicate whether the table must have ID
+                  values - if False, the IdentifierPolicy will return None
+                  unless _e_x_i_s_t_i_n_g already contains ID values
+                * vvoollaattiillee_¶ – Flag to indicate if external code may modify ID
+                  values while the current COLDP instance is active - if False,
+                  the policy and future values will be determined on
+                  initialisation, otherwise the policy will be reviewed for
+                  each new ID value
+        Returns:
+            IdentifierPolicy object or None if no policy is required for the
+            table
+      Creates new IdentifierPolicy instance if this is the first invocation for
+      the given table. Policies take into account any existing ID values for
+      the table.
 ******** AAcccceessss ttoo DDaattaaFFrraammeess_?¶ ********
   COLDP.table_by_name(nnaammee)_¶
       Return dataframe for named COLDP data class
         Parameters:
             nnaammee_¶ – Name of data frame to return (one of: name, taxon, synonym,
             reference, type_material, distribution, species_interaction,
             name_relation)
@@ -652,39 +705,14 @@
         Parameters:
                 * nnaammee_¶ – Dictionary containing COLDP Name record for which
                   basionymID is to be fixed
                 * ssyynnoonnyymmss_¶ – List of COLDP Name records that may contain
                   basionym
         Returns:
       Returns name following any updates.
-  COLDP.find_name(sscciieennttiiffiiccNNaammee, aauutthhoorrsshhiipp, rraannkk)_¶
-      Return record from names DataFrame matching supplied scientificName,
-      authorship and rank
-        Parameters:
-                * sscciieennttiiffiiccNNaammee_¶ – Scientific name in canonical format
-                * aauutthhoorrsshhiipp_¶ – Authorship string
-                * rraannkk_¶ – Rank name string
-        Returns:
-            Dictionary containing matching record if found
-      Locates any existing record in the names DataFrame that matches the
-      supplied scientificName, authorship and rank and returns it as a COLDP
-      Name properties dictionary, or None if no match is found.
-      If _a_u_t_h_o_r_s_h_i_p is None, returns a name based only on scientificName and
-      rank.
-  COLDP.find_taxon(sscciieennttiiffiiccNNaammee, aauutthhoorrsshhiipp, rraannkk)_¶
-      Get COLDP Taxon record (as Pandas dataframe) with accepted name matching
-      supplied scientificName, authorship and rank values
-        Parameters:
-                * sscciieennttiiffiiccNNaammee_¶ – Scientific name in canonical format
-                * aauutthhoorrsshhiipp_¶ – Authorship string
-                * rraannkk_¶ – Rank name string
-        Returns:
-            COLDP Taxon record matching supplied parameters
-      Logs a warning issue if multiple taxon records exist for a matching name
-      and returns the first such match. Returns None if no match.
   COLDP.construct_species_rank_name(gg, ssgg, ss, ssss, mmaarrkkeerr)_¶
       Consistently construct a species or infraspecific name from the included
       epithets and optional rank marker
         Parameters:
                 * gg_¶ – Genus name
                 * ssgg_¶ – Subgenus name
                 * ss_¶ – Specific epithet
@@ -746,14 +774,15 @@
     * _c_o_l_d_p_._C_O_L_D_P
           o _C_l_a_s_s
           o _M_e_t_h_o_d_s
           o _C_o_n_s_t_a_n_t_s
           o _I_n_t_e_r_n_a_l_ _m_e_t_h_o_d_s
           o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+    * _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
     * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o Previous: _c_o_l_d_p
           o Next: _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
```

### Comparing `coldp-2024.5.3/docs/build/html/genindex.html` & `coldp-2024.5.4/docs/build/html/genindex.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; COLDP 2024.5.3 documentation</title>
+    <title>Index &#8212; COLDP 2024.5.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
+    <script src="_static/documentation_options.js?v=78d2dd00"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
@@ -57,14 +57,16 @@
 </div>
 <h2 id="_">_</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.__init__">__init__() (coldp.COLDP method)</a>
 
       <ul>
+        <li><a href="identifier-policy.html#coldp.IdentifierPolicy.__init__">(coldp.IdentifierPolicy method)</a>
+</li>
         <li><a href="name-bundle.html#coldp.NameBundle.__init__">(coldp.NameBundle method)</a>
 </li>
       </ul></li>
   </ul></td>
 </tr></table>
 
 <h2 id="A">A</h2>
@@ -170,24 +172,30 @@
 </tr></table>
 
 <h2 id="D">D</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.initialise_dataframe.params.default_headings">default_headings (coldp.COLDP.initialise_dataframe parameter)</a>
 </li>
+      <li><a href="coldp.html#coldp.COLDP.get_identifier_policy.params.default_prefix">default_prefix (coldp.COLDP.get_identifier_policy parameter)</a>
+
+      <ul>
+        <li><a href="identifier-policy.html#coldp.IdentifierPolicy.params.default_prefix">(coldp.IdentifierPolicy parameter)</a>
+</li>
+      </ul></li>
       <li><a href="coldp.html#coldp.COLDP.params.default_taxon_record">default_taxon_record (coldp.COLDP parameter)</a>
 
       <ul>
         <li><a href="coldp.html#coldp.COLDP.set_default_taxon_record.params.default_taxon_record">(coldp.COLDP.set_default_taxon_record parameter)</a>
 </li>
       </ul></li>
-      <li><a href="name-bundle.html#coldp.NameBundle.derive_name">derive_name() (coldp.NameBundle method)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="name-bundle.html#coldp.NameBundle.derive_name">derive_name() (coldp.NameBundle method)</a>
+</li>
       <li><a href="coldp.html#coldp.COLDP.save.params.destination">destination (coldp.COLDP.save parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.extract_table.params.df">df (coldp.COLDP.extract_table parameter)</a>
 
       <ul>
         <li><a href="coldp.html#coldp.COLDP.sort_taxa_recursive.params.df">(coldp.COLDP.sort_taxa_recursive parameter)</a>
 </li>
@@ -206,18 +214,26 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.epithet_and_authorship_match.params.epithet">epithet (coldp.COLDP.epithet_and_authorship_match parameter)</a>
 
       <ul>
         <li><a href="coldp.html#coldp.COLDP.remove_gender.params.epithet">(coldp.COLDP.remove_gender parameter)</a>
 </li>
       </ul></li>
+      <li><a href="coldp.html#coldp.COLDP.epithet_and_authorship_match">epithet_and_authorship_match() (coldp.COLDP method)</a>
+</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="coldp.html#coldp.COLDP.epithet_and_authorship_match">epithet_and_authorship_match() (coldp.COLDP method)</a>
+      <li><a href="identifier-policy.html#coldp.IdentifierPolicy.params.existing">existing (coldp.IdentifierPolicy parameter)</a>
+
+      <ul>
+        <li><a href="identifier-policy.html#coldp.IdentifierPolicy.initialise.params.existing">(coldp.IdentifierPolicy.initialise parameter)</a>
 </li>
+        <li><a href="identifier-policy.html#coldp.IdentifierPolicy.next.params.existing">(coldp.IdentifierPolicy.next parameter)</a>
+</li>
+      </ul></li>
       <li><a href="coldp.html#coldp.COLDP.extract_table">extract_table() (coldp.COLDP method)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="F">F</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -252,22 +268,26 @@
 </tr></table>
 
 <h2 id="G">G</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.construct_species_rank_name.params.g">g (coldp.COLDP.construct_species_rank_name parameter)</a>
 </li>
+      <li><a href="coldp.html#coldp.COLDP.get_available_column_headings">get_available_column_headings() (coldp.COLDP method)</a>
+</li>
       <li><a href="coldp.html#coldp.COLDP.get_children">get_children() (coldp.COLDP method)</a>
 </li>
-      <li><a href="coldp.html#coldp.COLDP.get_name">get_name() (coldp.COLDP method)</a>
+      <li><a href="coldp.html#coldp.COLDP.get_identifier_policy">get_identifier_policy() (coldp.COLDP method)</a>
 </li>
-      <li><a href="coldp.html#coldp.COLDP.get_original_authorship">get_original_authorship() (coldp.COLDP method)</a>
+      <li><a href="coldp.html#coldp.COLDP.get_name">get_name() (coldp.COLDP method)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="coldp.html#coldp.COLDP.get_original_authorship">get_original_authorship() (coldp.COLDP method)</a>
+</li>
       <li><a href="coldp.html#coldp.COLDP.get_reference">get_reference() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.get_synonyms">get_synonyms() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.get_synonymy">get_synonymy() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.get_taxon">get_taxon() (coldp.COLDP method)</a>
@@ -308,17 +328,19 @@
 
       <ul>
         <li><a href="name-bundle.html#coldp.NameBundle.params.incertae_sedis">(coldp.NameBundle parameter)</a>
 </li>
       </ul></li>
       <li><a href="coldp.html#coldp.COLDP.get_text_tree.params.indent">indent (coldp.COLDP.get_text_tree parameter)</a>
 </li>
+      <li><a href="coldp.html#coldp.COLDP.get_text_tree.params.initial_prefix">initial_prefix (coldp.COLDP.get_text_tree parameter)</a>
+</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="coldp.html#coldp.COLDP.get_text_tree.params.initial_prefix">initial_prefix (coldp.COLDP.get_text_tree parameter)</a>
+      <li><a href="identifier-policy.html#coldp.IdentifierPolicy.initialise">initialise() (coldp.IdentifierPolicy method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.initialise_dataframe">initialise_dataframe() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.params.insert_species_for_trinomials">insert_species_for_trinomials (coldp.COLDP parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.insert_synonym">insert_synonym() (coldp.COLDP method)</a>
 </li>
@@ -398,14 +420,16 @@
 </li>
       <li><a href="coldp.html#coldp.COLDP.insert_synonym.params.name_id">name_id (coldp.COLDP.insert_synonym parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.add_name_relation.params.name_relation">name_relation (coldp.COLDP.add_name_relation parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.fix_basionyms.params.names">names (coldp.COLDP.fix_basionyms parameter)</a>
 </li>
+      <li><a href="identifier-policy.html#coldp.IdentifierPolicy.next">next() (coldp.IdentifierPolicy method)</a>
+</li>
       <li><a href="name-bundle.html#coldp.NameBundle.normalise_name">normalise_name() (coldp.NameBundle method)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="O">O</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -452,24 +476,30 @@
         <li><a href="coldp.html#coldp.COLDP.find_taxon.params.rank">(coldp.COLDP.find_taxon parameter)</a>
 </li>
       </ul></li>
       <li><a href="coldp.html#coldp.COLDP.fix_classification_recursive.params.ranks">ranks (coldp.COLDP.fix_classification_recursive parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.validate_record.params.record">record (coldp.COLDP.validate_record parameter)</a>
 </li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.validate_record.params.record_type">record_type (coldp.COLDP.validate_record parameter)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.find_reference.params.reference">reference (coldp.COLDP.find_reference parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.add_references.params.reference_list">reference_list (coldp.COLDP.add_references parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.remove_gender">remove_gender() (coldp.COLDP method)</a>
 </li>
+      <li><a href="coldp.html#coldp.COLDP.get_identifier_policy.params.required">required (coldp.COLDP.get_identifier_policy parameter)</a>
+
+      <ul>
+        <li><a href="identifier-policy.html#coldp.IdentifierPolicy.params.required">(coldp.IdentifierPolicy parameter)</a>
+</li>
+      </ul></li>
       <li><a href="coldp.html#coldp.COLDP.reset_ids">reset_ids() (coldp.COLDP method)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="S">S</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -538,14 +568,16 @@
 </tr></table>
 
 <h2 id="T">T</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.table_by_name">table_by_name() (coldp.COLDP method)</a>
 </li>
+      <li><a href="coldp.html#coldp.COLDP.get_identifier_policy.params.table_name">table_name (coldp.COLDP.get_identifier_policy parameter)</a>
+</li>
       <li><a href="coldp.html#coldp.COLDP.fix_classification_recursive.params.taxa">taxa (coldp.COLDP.fix_classification_recursive parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.taxon_from_nameusage">taxon_from_nameusage (in module coldp)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.insert_synonym.params.taxon_id">taxon_id (coldp.COLDP.insert_synonym parameter)</a>
 
       <ul>
@@ -582,18 +614,24 @@
 </tr></table>
 
 <h2 id="V">V</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.validate_record">validate_record() (coldp.COLDP method)</a>
 </li>
+      <li><a href="name-bundle.html#coldp.NameBundle.derive_name.params.values">values (coldp.NameBundle.derive_name parameter)</a>
+</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="name-bundle.html#coldp.NameBundle.derive_name.params.values">values (coldp.NameBundle.derive_name parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.get_identifier_policy.params.volatile">volatile (coldp.COLDP.get_identifier_policy parameter)</a>
+
+      <ul>
+        <li><a href="identifier-policy.html#coldp.IdentifierPolicy.params.volatile">(coldp.IdentifierPolicy parameter)</a>
 </li>
+      </ul></li>
   </ul></td>
 </tr></table>
 
 <h2 id="Y">Y</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.construct_authorship.params.y">y (coldp.COLDP.construct_authorship parameter)</a>
@@ -618,14 +656,15 @@
 
 
 
 <h3>Navigation</h3>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="coldp.html">coldp.COLDP</a></li>
 <li class="toctree-l1"><a class="reference internal" href="name-bundle.html">coldp.NameBundle</a></li>
+<li class="toctree-l1"><a class="reference internal" href="identifier-policy.html">coldp.IdentifierPolicy</a></li>
 </ul>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
 </ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 ************ IInnddeexx ************
 ___ | _AA | _BB | _CC | _DD | _EE | _FF | _GG | _HH | _II | _MM | _NN | _OO | _PP | _RR | _SS | _TT | _VV | _YY
 ********** __ **********
     * _____i_n_i_t_____(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+          o _(_c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y_ _m_e_t_h_o_d_)
           o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)
 ********** AA **********
     * _a_                                     * _a_d_d___s_p_e_c_i_e_s___i_n_t_e_r_a_c_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
       _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p       _m_e_t_h_o_d_)
       _p_a_r_a_m_e_t_e_r_)                            * _a_d_d___s_y_n_o_n_y_m_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
           o _(_c_o_l_d_p_._C_O_L_D_P_._s_a_m_e___b_a_s_i_o_n_y_m            o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)
             _p_a_r_a_m_e_t_e_r_)                      * _a_d_d___t_y_p_e___m_a_t_e_r_i_a_l_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
@@ -36,78 +37,83 @@
     * _c_o_l_d_p_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e           _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
       _p_a_r_a_m_e_t_e_r_)                      * _c_r_e_a_t_e___s_y_n_o_n_y_m_s___w_i_t_h_o_u_t___s_u_b_g_e_n_u_s_ 
     * _c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p_(_)_            _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
       _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)            * _c_r_e_a_t_e___t_a_x_a___f_o_r___n_o_t___e_s_t_a_b_l_i_s_h_e_d_ 
     * _c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e       _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
       _(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)         * _c_s_v___e_x_t_e_n_s_i_o_n_s_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)
 ********** DD **********
-    * _d_e_f_a_u_l_t___h_e_a_d_i_n_g_s_                                * _d_e_s_t_i_n_a_t_i_o_n_ _(_c_o_l_d_p_._C_O_L_D_P_._s_a_v_e
-      _(_c_o_l_d_p_._C_O_L_D_P_._i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e                 _p_a_r_a_m_e_t_e_r_)
-      _p_a_r_a_m_e_t_e_r_)                                      * _d_f_ _(_c_o_l_d_p_._C_O_L_D_P_._e_x_t_r_a_c_t___t_a_b_l_e
-    * _d_e_f_a_u_l_t___t_a_x_o_n___r_e_c_o_r_d_ _(_c_o_l_d_p_._C_O_L_D_P                 _p_a_r_a_m_e_t_e_r_)
-      _p_a_r_a_m_e_t_e_r_)                                            o _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e
-          o _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___d_e_f_a_u_l_t___t_a_x_o_n___r_e_c_o_r_d             _p_a_r_a_m_e_t_e_r_)
-            _p_a_r_a_m_e_t_e_r_)                                * _d_i_s_t_r_i_b_u_t_i_o_n_ 
-    * _d_e_r_i_v_e___n_a_m_e_(_)_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)           _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___d_i_s_t_r_i_b_u_t_i_o_n
-                                                        _p_a_r_a_m_e_t_e_r_)
+    * _d_e_f_a_u_l_t___h_e_a_d_i_n_g_s_                                * _d_e_r_i_v_e___n_a_m_e_(_)_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+      _(_c_o_l_d_p_._C_O_L_D_P_._i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e                 _m_e_t_h_o_d_)
+      _p_a_r_a_m_e_t_e_r_)                                      * _d_e_s_t_i_n_a_t_i_o_n_ _(_c_o_l_d_p_._C_O_L_D_P_._s_a_v_e
+    * _d_e_f_a_u_l_t___p_r_e_f_i_x_                                    _p_a_r_a_m_e_t_e_r_)
+      _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___i_d_e_n_t_i_f_i_e_r___p_o_l_i_c_y              * _d_f_ _(_c_o_l_d_p_._C_O_L_D_P_._e_x_t_r_a_c_t___t_a_b_l_e
+      _p_a_r_a_m_e_t_e_r_)                                        _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y_ _p_a_r_a_m_e_t_e_r_)              o _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e
+    * _d_e_f_a_u_l_t___t_a_x_o_n___r_e_c_o_r_d_ _(_c_o_l_d_p_._C_O_L_D_P                       _p_a_r_a_m_e_t_e_r_)
+      _p_a_r_a_m_e_t_e_r_)                                      * _d_i_s_t_r_i_b_u_t_i_o_n_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___d_e_f_a_u_l_t___t_a_x_o_n___r_e_c_o_r_d       _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___d_i_s_t_r_i_b_u_t_i_o_n
+            _p_a_r_a_m_e_t_e_r_)                                  _p_a_r_a_m_e_t_e_r_)
                                                             o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___d_i_s_t_r_i_b_u_t_i_o_n
                                                               _p_a_r_a_m_e_t_e_r_)
 ********** EE **********
-    * _e_p_i_t_h_e_t_                                       * _e_p_i_t_h_e_t___a_n_d___a_u_t_h_o_r_s_h_i_p___m_a_t_c_h
-      _(_c_o_l_d_p_._C_O_L_D_P_._e_p_i_t_h_e_t___a_n_d___a_u_t_h_o_r_s_h_i_p___m_a_t_c_h       _(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-      _p_a_r_a_m_e_t_e_r_)                                    * _e_x_t_r_a_c_t___t_a_b_l_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-          o _(_c_o_l_d_p_._C_O_L_D_P_._r_e_m_o_v_e___g_e_n_d_e_r                _m_e_t_h_o_d_)
-            _p_a_r_a_m_e_t_e_r_)
+    * _e_p_i_t_h_e_t_                                       * _e_x_i_s_t_i_n_g_ _(_c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
+      _(_c_o_l_d_p_._C_O_L_D_P_._e_p_i_t_h_e_t___a_n_d___a_u_t_h_o_r_s_h_i_p___m_a_t_c_h       _p_a_r_a_m_e_t_e_r_)
+      _p_a_r_a_m_e_t_e_r_)                                          o _(_c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y_._i_n_i_t_i_a_l_i_s_e
+          o _(_c_o_l_d_p_._C_O_L_D_P_._r_e_m_o_v_e___g_e_n_d_e_r                      _p_a_r_a_m_e_t_e_r_)
+            _p_a_r_a_m_e_t_e_r_)                                    o _(_c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y_._n_e_x_t
+    * _e_p_i_t_h_e_t___a_n_d___a_u_t_h_o_r_s_h_i_p___m_a_t_c_h_(_)_                        _p_a_r_a_m_e_t_e_r_)
+      _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)                          * _e_x_t_r_a_c_t___t_a_b_l_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
 ********** FF **********
     * _f_i_n_d___d_i_s_t_r_i_b_u_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P      * _f_i_x___b_a_s_i_o_n_y_m_i_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
       _m_e_t_h_o_d_)                                 _m_e_t_h_o_d_)
     * _f_i_n_d___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)      * _f_i_x___b_a_s_i_o_n_y_m_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
     * _f_i_n_d___n_a_m_e___r_e_c_o_r_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P         _m_e_t_h_o_d_)
       _m_e_t_h_o_d_)                               * _f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
     * _f_i_n_d___n_a_m_e_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)       _m_e_t_h_o_d_)
     * _f_i_n_d___r_e_f_e_r_e_n_c_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P         * _f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e_(_)_ 
       _m_e_t_h_o_d_)                                 _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
     * _f_i_n_d___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)     * _f_o_l_d_e_r_ _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
                                             * _f_o_l_d_e_r_n_a_m_e_ 
                                               _(_c_o_l_d_p_._C_O_L_D_P_._i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e
                                               _p_a_r_a_m_e_t_e_r_)
 ********** GG **********
-    * _g_                                            * _g_e_t___r_e_f_e_r_e_n_c_e_(_)_ 
+    * _g_                                            * _g_e_t___o_r_i_g_i_n_a_l___a_u_t_h_o_r_s_h_i_p_(_)_ 
       _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e       _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-      _p_a_r_a_m_e_t_e_r_)                                   * _g_e_t___s_y_n_o_n_y_m_s_(_)_ 
+      _p_a_r_a_m_e_t_e_r_)                                   * _g_e_t___r_e_f_e_r_e_n_c_e_(_)_ 
+    * _g_e_t___a_v_a_i_l_a_b_l_e___c_o_l_u_m_n___h_e_a_d_i_n_g_s_(_)_                _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+      _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)                         * _g_e_t___s_y_n_o_n_y_m_s_(_)_ 
     * _g_e_t___c_h_i_l_d_r_e_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)            _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-    * _g_e_t___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)              * _g_e_t___s_y_n_o_n_y_m_y_(_)_ 
-    * _g_e_t___o_r_i_g_i_n_a_l___a_u_t_h_o_r_s_h_i_p_(_)_ _(_c_o_l_d_p_._C_O_L_D_P         _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                      * _g_e_t___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+    * _g_e_t___i_d_e_n_t_i_f_i_e_r___p_o_l_i_c_y_(_)_ _(_c_o_l_d_p_._C_O_L_D_P         * _g_e_t___s_y_n_o_n_y_m_y_(_)_ 
+      _m_e_t_h_o_d_)                                        _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+    * _g_e_t___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)              * _g_e_t___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
                                                      _m_e_t_h_o_d_)
                                                    * _g_e_t___t_e_x_t___t_r_e_e_(_)_ 
                                                      _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
 ********** HH **********
     * _h_e_a_d_i_n_g_s_ _(_c_o_l_d_p_._C_O_L_D_P_._e_x_t_r_a_c_t___t_a_b_l_e_ _p_a_r_a_m_e_t_e_r_)
 ********** II **********
-    * _i_d_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)        * _i_n_i_t_i_a_l___p_r_e_f_i_x_ 
-          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___r_e_f_e_r_e_n_c_e             _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e
-            _p_a_r_a_m_e_t_e_r_)                             _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_a_x_o_n               * _i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-            _p_a_r_a_m_e_t_e_r_)                             _m_e_t_h_o_d_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e     * _i_n_s_e_r_t___s_p_e_c_i_e_s___f_o_r___t_r_i_n_o_m_i_a_l_s_ 
-            _p_a_r_a_m_e_t_e_r_)                             _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
-    * _i_d___m_a_p_p_i_n_g_s_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)              * _i_n_s_e_r_t___s_y_n_o_n_y_m_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-    * _i_d_e_n_t_i_f_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)         _m_e_t_h_o_d_)
-    * _i_d_s_ _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e       * _i_n_s_e_r_t___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-      _p_a_r_a_m_e_t_e_r_)                                 * _i_n_t_e_r_a_c_t_i_o_n_ 
-    * _i_n_c_e_r_t_a_e___s_e_d_i_s_                               _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___s_p_e_c_i_e_s___i_n_t_e_r_a_c_t_i_o_n
-      _(_c_o_l_d_p_._C_O_L_D_P_._s_t_a_r_t___n_a_m_e___b_u_n_d_l_e               _p_a_r_a_m_e_t_e_r_)
-      _p_a_r_a_m_e_t_e_r_)                                 * _i_s___b_a_s_i_o_n_y_m_ 
-          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _p_a_r_a_m_e_t_e_r_)           _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p
-    * _i_n_d_e_n_t_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e            _p_a_r_a_m_e_t_e_r_)
-      _p_a_r_a_m_e_t_e_r_)                                 * _i_s___i_n_f_r_a_s_u_b_s_p_e_c_i_f_i_c_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-                                                   _m_e_t_h_o_d_)
-                                                 * _i_s___s_p_e_c_i_e_s___g_r_o_u_p_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-                                                   _m_e_t_h_o_d_)
+    * _i_d_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)        * _i_n_i_t_i_a_l_i_s_e_(_)_ _(_c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
+          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___r_e_f_e_r_e_n_c_e             _m_e_t_h_o_d_)
+            _p_a_r_a_m_e_t_e_r_)                           * _i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_a_x_o_n                 _m_e_t_h_o_d_)
+            _p_a_r_a_m_e_t_e_r_)                           * _i_n_s_e_r_t___s_p_e_c_i_e_s___f_o_r___t_r_i_n_o_m_i_a_l_s_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e       _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
+            _p_a_r_a_m_e_t_e_r_)                           * _i_n_s_e_r_t___s_y_n_o_n_y_m_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+    * _i_d___m_a_p_p_i_n_g_s_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)                _m_e_t_h_o_d_)
+    * _i_d_e_n_t_i_f_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)       * _i_n_s_e_r_t___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+    * _i_d_s_ _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e       * _i_n_t_e_r_a_c_t_i_o_n_ 
+      _p_a_r_a_m_e_t_e_r_)                                   _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___s_p_e_c_i_e_s___i_n_t_e_r_a_c_t_i_o_n
+    * _i_n_c_e_r_t_a_e___s_e_d_i_s_                               _p_a_r_a_m_e_t_e_r_)
+      _(_c_o_l_d_p_._C_O_L_D_P_._s_t_a_r_t___n_a_m_e___b_u_n_d_l_e             * _i_s___b_a_s_i_o_n_y_m_ 
+      _p_a_r_a_m_e_t_e_r_)                                   _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p
+          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _p_a_r_a_m_e_t_e_r_)           _p_a_r_a_m_e_t_e_r_)
+    * _i_n_d_e_n_t_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e          * _i_s___i_n_f_r_a_s_u_b_s_p_e_c_i_f_i_c_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+      _p_a_r_a_m_e_t_e_r_)                                   _m_e_t_h_o_d_)
+    * _i_n_i_t_i_a_l___p_r_e_f_i_x_                             * _i_s___s_p_e_c_i_e_s___g_r_o_u_p_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+      _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e_ _p_a_r_a_m_e_t_e_r_)        _m_e_t_h_o_d_)
                                                  * _i_s_s_u_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
                                                  * _i_s_s_u_e_s___t_o___s_t_d_o_u_t_ _(_c_o_l_d_p_._C_O_L_D_P
                                                    _p_a_r_a_m_e_t_e_r_)
 ********** MM **********
     * _m_a_p_p_i_n_g_s_ _(_c_o_l_d_p_._C_O_L_D_P_._e_x_t_r_a_c_t___t_a_b_l_e          * _m_e_s_s_a_g_e_ _(_c_o_l_d_p_._C_O_L_D_P_._i_s_s_u_e
       _p_a_r_a_m_e_t_e_r_)                                     _p_a_r_a_m_e_t_e_r_)
     * _m_a_r_k_e_r_                                       * _m_o_d_i_f_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
@@ -122,18 +128,18 @@
           o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___b_a_s_i_o_n_y_m_i_d_ _p_a_r_a_m_e_t_e_r_)          _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._C_O_L_D_P_._i_d_e_n_t_i_f_y___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)         * _n_a_m_e___r_e_l_a_t_i_o_n_ 
           o _(_c_o_l_d_p_._C_O_L_D_P_._i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e               _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___n_a_m_e___r_e_l_a_t_i_o_n
             _p_a_r_a_m_e_t_e_r_)                                      _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___t_a_x_o_n_ _p_a_r_a_m_e_t_e_r_)          * _n_a_m_e_s_ 
           o _(_c_o_l_d_p_._C_O_L_D_P_._i_s___i_n_f_r_a_s_u_b_s_p_e_c_i_f_i_c                _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___b_a_s_i_o_n_y_m_s
             _p_a_r_a_m_e_t_e_r_)                                      _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._i_s___s_p_e_c_i_e_s___g_r_o_u_p_ _p_a_r_a_m_e_t_e_r_)      * _n_o_r_m_a_l_i_s_e___n_a_m_e_(_)_ 
-          o _(_c_o_l_d_p_._C_O_L_D_P_._r_e_s_e_t___i_d_s_ _p_a_r_a_m_e_t_e_r_)               _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._s_a_v_e_ _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___b_a_s_i_o_n_y_m_i_d_ _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._i_s___s_p_e_c_i_e_s___g_r_o_u_p_ _p_a_r_a_m_e_t_e_r_)      * _n_e_x_t_(_)_ _(_c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
+          o _(_c_o_l_d_p_._C_O_L_D_P_._r_e_s_e_t___i_d_s_ _p_a_r_a_m_e_t_e_r_)               _m_e_t_h_o_d_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._s_a_v_e_ _p_a_r_a_m_e_t_e_r_)                  * _n_o_r_m_a_l_i_s_e___n_a_m_e_(_)_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___b_a_s_i_o_n_y_m_i_d_ _p_a_r_a_m_e_t_e_r_)          _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)
           o _(_c_o_l_d_p_._C_O_L_D_P_._t_a_b_l_e___b_y___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._d_e_r_i_v_e___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._n_o_r_m_a_l_i_s_e___n_a_m_e
             _p_a_r_a_m_e_t_e_r_)
 ********** OO **********
     * _o_p_t_i_o_n_s_ _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___o_p_t_i_o_n_s_ _p_a_r_a_m_e_t_e_r_)
 ********** PP **********
@@ -143,27 +149,28 @@
     * _p_a_r_e_n_t_I_D_ _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___t_a_x_o_n_ _p_a_r_a_m_e_t_e_r_)         _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e_s
     * _p_r_e_f_i_x_ _(_c_o_l_d_p_._C_O_L_D_P_._r_e_s_e_t___i_d_s_ _p_a_r_a_m_e_t_e_r_)              _p_a_r_a_m_e_t_e_r_)
                                                                 o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___n_a_m_e
                                                                   _p_a_r_a_m_e_t_e_r_)
                                                                 o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___t_a_x_o_n
                                                                   _p_a_r_a_m_e_t_e_r_)
 ********** RR **********
-    * _r_a_n_k_ _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)        * _r_e_c_o_r_d___t_y_p_e_ 
-          o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___t_a_x_o_n_ _p_a_r_a_m_e_t_e_r_)        _(_c_o_l_d_p_._C_O_L_D_P_._v_a_l_i_d_a_t_e___r_e_c_o_r_d
+    * _r_a_n_k_ _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)        * _r_e_f_e_r_e_n_c_e_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___t_a_x_o_n_ _p_a_r_a_m_e_t_e_r_)        _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___r_e_f_e_r_e_n_c_e
     * _r_a_n_k_s_                                           _p_a_r_a_m_e_t_e_r_)
-      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e     * _r_e_f_e_r_e_n_c_e_ 
-      _p_a_r_a_m_e_t_e_r_)                                      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___r_e_f_e_r_e_n_c_e
+      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e     * _r_e_f_e_r_e_n_c_e___l_i_s_t_ 
+      _p_a_r_a_m_e_t_e_r_)                                      _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___r_e_f_e_r_e_n_c_e_s
     * _r_e_c_o_r_d_ _(_c_o_l_d_p_._C_O_L_D_P_._v_a_l_i_d_a_t_e___r_e_c_o_r_d             _p_a_r_a_m_e_t_e_r_)
-      _p_a_r_a_m_e_t_e_r_)                                    * _r_e_f_e_r_e_n_c_e___l_i_s_t_ 
-                                                      _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___r_e_f_e_r_e_n_c_e_s
+      _p_a_r_a_m_e_t_e_r_)                                    * _r_e_m_o_v_e___g_e_n_d_e_r_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+    * _r_e_c_o_r_d___t_y_p_e_ _(_c_o_l_d_p_._C_O_L_D_P_._v_a_l_i_d_a_t_e___r_e_c_o_r_d        _m_e_t_h_o_d_)
+      _p_a_r_a_m_e_t_e_r_)                                    * _r_e_q_u_i_r_e_d_ 
+                                                      _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___i_d_e_n_t_i_f_i_e_r___p_o_l_i_c_y
                                                       _p_a_r_a_m_e_t_e_r_)
-                                                    * _r_e_m_o_v_e___g_e_n_d_e_r_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-                                                      _m_e_t_h_o_d_)
-                                                    * _r_e_s_e_t___i_d_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-                                                      _m_e_t_h_o_d_)
+                                                          o _(_c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
+                                                            _p_a_r_a_m_e_t_e_r_)
+                                                    * _r_e_s_e_t___i_d_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
 ********** SS **********
     * _s_                                            * _s_o_r_t___n_a_m_e_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
       _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e     * _s_o_r_t___t_a_x_a_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
       _p_a_r_a_m_e_t_e_r_)                                   * _s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
     * _s_a_m_e___b_a_s_i_o_n_y_m_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)           _m_e_t_h_o_d_)
     * _s_a_v_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)                  * _s_s_ 
     * _s_c_i_e_n_t_i_f_i_c_N_a_m_e_ _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e          _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e
@@ -182,39 +189,46 @@
           o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _p_a_r_a_m_e_t_e_r_)                   _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._a_d_d___s_y_n_o_n_y_m
             _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._n_o_r_m_a_l_i_s_e___n_a_m_e
             _p_a_r_a_m_e_t_e_r_)
 ********** TT **********
     * _t_a_b_l_e___b_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)          * _t_o___d_i_c_t_ _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e_s
-    * _t_a_x_a_                                            _p_a_r_a_m_e_t_e_r_)
-      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e           o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___c_h_i_l_d_r_e_n
+    * _t_a_b_l_e___n_a_m_e_                                      _p_a_r_a_m_e_t_e_r_)
+      _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___i_d_e_n_t_i_f_i_e_r___p_o_l_i_c_y                  o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___c_h_i_l_d_r_e_n
       _p_a_r_a_m_e_t_e_r_)                                            _p_a_r_a_m_e_t_e_r_)
-    * _t_a_x_o_n___f_r_o_m___n_a_m_e_u_s_a_g_e_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)              o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___s_y_n_o_n_y_m_s
-    * _t_a_x_o_n___i_d_ _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___s_y_n_o_n_y_m                  _p_a_r_a_m_e_t_e_r_)
+    * _t_a_x_a_                                                o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___s_y_n_o_n_y_m_s
+      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e             _p_a_r_a_m_e_t_e_r_)
       _p_a_r_a_m_e_t_e_r_)                                          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___s_y_n_o_n_y_m_y
-          o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)             _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___t_a_x_o_n               * _t_y_p_e___m_a_t_e_r_i_a_l_ 
-            _p_a_r_a_m_e_t_e_r_)                                _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___t_y_p_e___m_a_t_e_r_i_a_l
-    * _t_a_x_o_n_I_D_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___c_h_i_l_d_r_e_n               _p_a_r_a_m_e_t_e_r_)
+    * _t_a_x_o_n___f_r_o_m___n_a_m_e_u_s_a_g_e_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)                _p_a_r_a_m_e_t_e_r_)
+    * _t_a_x_o_n___i_d_ _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___s_y_n_o_n_y_m          * _t_y_p_e___m_a_t_e_r_i_a_l_ 
+      _p_a_r_a_m_e_t_e_r_)                                      _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___t_y_p_e___m_a_t_e_r_i_a_l
+          o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)       _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___t_a_x_o_n
+            _p_a_r_a_m_e_t_e_r_)
+    * _t_a_x_o_n_I_D_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___c_h_i_l_d_r_e_n
       _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___s_y_n_o_n_y_m_s
             _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___s_y_n_o_n_y_m_y
             _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e
             _p_a_r_a_m_e_t_e_r_)
 ********** VV **********
-    * _v_a_l_i_d_a_t_e___r_e_c_o_r_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P     * _v_a_l_u_e_s_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._d_e_r_i_v_e___n_a_m_e
-      _m_e_t_h_o_d_)                              _p_a_r_a_m_e_t_e_r_)
+    * _v_a_l_i_d_a_t_e___r_e_c_o_r_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P     * _v_o_l_a_t_i_l_e_ 
+      _m_e_t_h_o_d_)                              _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___i_d_e_n_t_i_f_i_e_r___p_o_l_i_c_y
+    * _v_a_l_u_e_s_                               _p_a_r_a_m_e_t_e_r_)
+      _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._d_e_r_i_v_e___n_a_m_e            o _(_c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
+      _p_a_r_a_m_e_t_e_r_)                                 _p_a_r_a_m_e_t_e_r_)
 ********** YY **********
     * _y_ _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p_ _p_a_r_a_m_e_t_e_r_)
 ************ _CC_OO_LL_DD_PP ************
 ******** NNaavviiggaattiioonn ********
     * _c_o_l_d_p_._C_O_L_D_P
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+    * _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
     * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
 ©2024, Donald Hobern. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r_ _0_._7_._1_6
```

### Comparing `coldp-2024.5.3/docs/build/html/index.html` & `coldp-2024.5.4/docs/build/html/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>coldp &#8212; COLDP 2024.5.3 documentation</title>
+    <title>coldp &#8212; COLDP 2024.5.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
+    <script src="_static/documentation_options.js?v=78d2dd00"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="coldp.COLDP" href="coldp.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
@@ -34,18 +34,19 @@
             
   <section id="coldp">
 <h1>coldp<a class="headerlink" href="#coldp" title="Link to this heading">¶</a></h1>
 <p>Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format</p>
 <section id="overview">
 <h2>Overview<a class="headerlink" href="#overview" title="Link to this heading">¶</a></h2>
 <p>coldp is a Python package to facilitate creation, manipulation, editing and serialisation of taxonomic checklists in the <a class="reference external" href="https://github.com/CatalogueOfLife/coldp">COL Data Package (COLDP)</a> format.</p>
-<p>The package includes two classes:</p>
+<p>The package includes three classes:</p>
 <ul class="simple">
 <li><p><strong>coldp.COLDP</strong> - A COLDP package loaded as a set of Pandas dataframes</p></li>
 <li><p><strong>coldp.NameBundle</strong> - A helper class to simplify addition of taxon names with sets of associated synonyms to a COLDP instance</p></li>
+<li><p><strong>coldp.IdentifierPolicy</strong> - An internal class to manage ID values in COLDP dataframes</p></li>
 </ul>
 <p>The main <strong>COLDP</strong> class instantiates a COLDP package in memory as a set of Pandas dataframes. An instance may be initialised from the contents of a folder containing a set of COLDP-compliant CSV or tab-delimited data files or alternatively can be initialised as an empty instance in memory. The class includes many methods for inserting new data, editing existing records and querying the contents of the package. The instance can then be saved as a set of CSV files in a named folder .</p>
 <p>The <strong>NameBundle</strong> class brings together a scientific name and its synonyms so that these can be added together and the COLDP package can automatically manage their relationships NameBundle objects are normally created using the <a class="reference internal" href="coldp.html#coldp.COLDP.start_name_bundle" title="coldp.COLDP.start_name_bundle"><code class="xref py py-func docutils literal notranslate"><span class="pre">coldp.COLDP.start_name_bundle()</span></code></a> method.</p>
 <p>At minimum a NameBundle is initialised with a dictionary holding a set of COLDP name record values. The scientific name represented by this dictionary should be the accepted name for a species or other taxon. Synonyms may then be added to the NameBundle.</p>
 <p>Once all names are included, the NameBundle can be added to the COLDP object via the <a class="reference internal" href="coldp.html#coldp.COLDP.add_names" title="coldp.COLDP.add_names"><code class="xref py py-func docutils literal notranslate"><span class="pre">coldp.COLDP.add_names()</span></code></a> method. This adds name, taxon and synonym records for the set of names supplied. COLDP options may expand the set of added synonyms to include variant formats or may trigger the addition of one or taxa that are implicit in the accepted name.</p>
 <p>The COLDP object will automatically manage record identifiers and the basionymID for any name records that are combinations of another name in the set.</p>
 </section>
@@ -70,14 +71,20 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="name-bundle.html">coldp.NameBundle</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="name-bundle.html#class">Class</a></li>
 <li class="toctree-l2"><a class="reference internal" href="name-bundle.html#methods">Methods</a></li>
 <li class="toctree-l2"><a class="reference internal" href="name-bundle.html#index-and-search">Index and search</a></li>
 </ul>
 </li>
+<li class="toctree-l1"><a class="reference internal" href="identifier-policy.html">coldp.IdentifierPolicy</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="identifier-policy.html#class">Class</a></li>
+<li class="toctree-l2"><a class="reference internal" href="identifier-policy.html#methods">Methods</a></li>
+<li class="toctree-l2"><a class="reference internal" href="identifier-policy.html#index-and-search">Index and search</a></li>
+</ul>
+</li>
 </ul>
 </div>
 </section>
 <section id="usage">
 <h2>Usage<a class="headerlink" href="#usage" title="Link to this heading">¶</a></h2>
 <div class="toctree-wrapper compound">
 <ul>
@@ -110,14 +117,15 @@
 
 
 
 <h3>Navigation</h3>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="coldp.html">coldp.COLDP</a></li>
 <li class="toctree-l1"><a class="reference internal" href="name-bundle.html">coldp.NameBundle</a></li>
+<li class="toctree-l1"><a class="reference internal" href="identifier-policy.html">coldp.IdentifierPolicy</a></li>
 </ul>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
 </ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
 ************ ccoollddpp_?¶ ************
 Python tools for working with taxonomic checklists organised as Catalogue of
 Life Data Package (COLDP) format
 ********** OOvveerrvviieeww_?¶ **********
 coldp is a Python package to facilitate creation, manipulation, editing and
 serialisation of taxonomic checklists in the _C_O_L_ _D_a_t_a_ _P_a_c_k_a_g_e_ _(_C_O_L_D_P_) format.
-The package includes two classes:
+The package includes three classes:
     * ccoollddpp..CCOOLLDDPP - A COLDP package loaded as a set of Pandas dataframes
     * ccoollddpp..NNaammeeBBuunnddllee - A helper class to simplify addition of taxon names
       with sets of associated synonyms to a COLDP instance
+    * ccoollddpp..IIddeennttiiffiieerrPPoolliiccyy - An internal class to manage ID values in COLDP
+      dataframes
 The main CCOOLLDDPP class instantiates a COLDP package in memory as a set of Pandas
 dataframes. An instance may be initialised from the contents of a folder
 containing a set of COLDP-compliant CSV or tab-delimited data files or
 alternatively can be initialised as an empty instance in memory. The class
 includes many methods for inserting new data, editing existing records and
 querying the contents of the package. The instance can then be saved as a set
 of CSV files in a named folder .
@@ -41,23 +43,28 @@
           o _C_o_n_s_t_a_n_t_s
           o _I_n_t_e_r_n_a_l_ _m_e_t_h_o_d_s
           o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
           o _C_l_a_s_s
           o _M_e_t_h_o_d_s
           o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
+    * _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
+          o _C_l_a_s_s
+          o _M_e_t_h_o_d_s
+          o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
 ********** UUssaaggee_?¶ **********
     * _U_s_a_g_e
 ******** IInnddeexx aanndd sseeaarrcchh_?¶ ********
     * _I_n_d_e_x
     * _S_e_a_r_c_h_ _P_a_g_e
 ************ _CC_OO_LL_DD_PP ************
 ******** NNaavviiggaattiioonn ********
     * _c_o_l_d_p_._C_O_L_D_P
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+    * _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
     * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o Next: _c_o_l_d_p_._C_O_L_D_P
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
 ©2024, Donald Hobern. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r_ _0_._7_._1_6 | _P_a_g_e
```

### Comparing `coldp-2024.5.3/docs/build/html/name-bundle.html` & `coldp-2024.5.4/docs/build/html/name-bundle.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>coldp.NameBundle &#8212; COLDP 2024.5.3 documentation</title>
+    <title>coldp.NameBundle &#8212; COLDP 2024.5.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
+    <script src="_static/documentation_options.js?v=78d2dd00"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="Usage" href="usage.html" />
+    <link rel="next" title="coldp.IdentifierPolicy" href="identifier-policy.html" />
     <link rel="prev" title="coldp.COLDP" href="coldp.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
 
   
   
@@ -144,25 +144,26 @@
 <li class="toctree-l1"><a class="reference internal" href="coldp.html">coldp.COLDP</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">coldp.NameBundle</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#class">Class</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#methods">Methods</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#index-and-search">Index and search</a></li>
 </ul>
 </li>
+<li class="toctree-l1"><a class="reference internal" href="identifier-policy.html">coldp.IdentifierPolicy</a></li>
 </ul>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
 </ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
       <li>Previous: <a href="coldp.html" title="previous chapter">coldp.COLDP</a></li>
-      <li>Next: <a href="usage.html" title="next chapter">Usage</a></li>
+      <li>Next: <a href="identifier-policy.html" title="next chapter">coldp.IdentifierPolicy</a></li>
   </ul></li>
 </ul>
 </div>
 <search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
```

#### html2text {}

```diff
@@ -59,16 +59,17 @@
 ************ _CC_OO_LL_DD_PP ************
 ******** NNaavviiggaattiioonn ********
     * _c_o_l_d_p_._C_O_L_D_P
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
           o _C_l_a_s_s
           o _M_e_t_h_o_d_s
           o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
+    * _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
     * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o Previous: _c_o_l_d_p_._C_O_L_D_P
-          o Next: _U_s_a_g_e
+          o Next: _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
 ©2024, Donald Hobern. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r_ _0_._7_._1_6 | _P_a_g_e
 _s_o_u_r_c_e
```

### Comparing `coldp-2024.5.3/docs/build/html/search.html` & `coldp-2024.5.4/docs/build/html/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; COLDP 2024.5.3 documentation</title>
+    <title>Search &#8212; COLDP 2024.5.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     
-    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
+    <script src="_static/documentation_options.js?v=78d2dd00"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
     <script src="searchindex.js" defer="defer"></script>
@@ -80,14 +80,15 @@
 
 
 
 <h3>Navigation</h3>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="coldp.html">coldp.COLDP</a></li>
 <li class="toctree-l1"><a class="reference internal" href="name-bundle.html">coldp.NameBundle</a></li>
+<li class="toctree-l1"><a class="reference internal" href="identifier-policy.html">coldp.IdentifierPolicy</a></li>
 </ul>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
 </ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
```

#### html2text {}

```diff
@@ -2,11 +2,12 @@
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ][search]
 ************ _CC_OO_LL_DD_PP ************
 ******** NNaavviiggaattiioonn ********
     * _c_o_l_d_p_._C_O_L_D_P
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+    * _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
     * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
 ©2024, Donald Hobern. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r_ _0_._7_._1_6
```

### Comparing `coldp-2024.5.3/docs/build/html/searchindex.js` & `coldp-2024.5.4/docs/build/html/searchindex.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -4,91 +4,100 @@
             [0, "access-to-dataframes"]
         ],
         "Add or modify records": [
             [0, "add-or-modify-records"]
         ],
         "Class": [
             [0, "class"],
-            [2, "class"]
+            [1, "class"],
+            [3, "class"]
         ],
         "Classes": [
-            [1, "classes"]
+            [2, "classes"]
         ],
         "Constants": [
             [0, "constants"]
         ],
         "Control behaviour": [
             [0, "control-behaviour"]
         ],
         "Find or get records": [
             [0, "find-or-get-records"]
         ],
         "Index and search": [
             [0, "index-and-search"],
             [1, "index-and-search"],
-            [2, "index-and-search"]
+            [2, "index-and-search"],
+            [3, "index-and-search"]
         ],
         "Installation": [
-            [1, "installation"]
+            [2, "installation"]
         ],
         "Internal methods": [
             [0, "internal-methods"]
         ],
         "Methods": [
             [0, "methods"],
-            [2, "methods"]
+            [1, "methods"],
+            [3, "methods"]
         ],
         "Overview": [
-            [1, "overview"]
+            [2, "overview"]
         ],
         "Save": [
             [0, "save"]
         ],
         "Tidy package": [
             [0, "tidy-package"]
         ],
         "Usage": [
-            [1, "usage"],
-            [3, "usage"]
+            [2, "usage"],
+            [4, "usage"]
         ],
         "Utilities": [
             [0, "utilities"]
         ],
         "coldp": [
-            [1, "coldp"]
+            [2, "coldp"]
         ],
         "coldp.COLDP": [
             [0, "coldp-coldp"]
         ],
+        "coldp.IdentifierPolicy": [
+            [1, "coldp-identifierpolicy"]
+        ],
         "coldp.NameBundle": [
-            [2, "coldp-namebundle"]
+            [3, "coldp-namebundle"]
         ]
     },
-    "docnames": ["coldp", "index", "name-bundle", "usage"],
+    "docnames": ["coldp", "identifier-policy", "index", "name-bundle", "usage"],
     "envversion": {
         "sphinx": 61,
         "sphinx.domains.c": 3,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
         "sphinx.domains.cpp": 9,
         "sphinx.domains.index": 1,
         "sphinx.domains.javascript": 3,
         "sphinx.domains.math": 2,
         "sphinx.domains.python": 4,
         "sphinx.domains.rst": 2,
         "sphinx.domains.std": 2,
         "sphinx.ext.intersphinx": 1
     },
-    "filenames": ["coldp.rst", "index.rst", "name-bundle.rst", "usage.rst"],
+    "filenames": ["coldp.rst", "identifier-policy.rst", "index.rst", "name-bundle.rst", "usage.rst"],
     "indexentries": {
         "__init__() (coldp.coldp method)": [
             [0, "coldp.COLDP.__init__", false]
         ],
+        "__init__() (coldp.identifierpolicy method)": [
+            [1, "coldp.IdentifierPolicy.__init__", false]
+        ],
         "__init__() (coldp.namebundle method)": [
-            [2, "coldp.NameBundle.__init__", false]
+            [3, "coldp.NameBundle.__init__", false]
         ],
         "add_distribution() (coldp.coldp method)": [
             [0, "coldp.COLDP.add_distribution", false]
         ],
         "add_name_relation() (coldp.coldp method)": [
             [0, "coldp.COLDP.add_name_relation", false]
         ],
@@ -101,30 +110,30 @@
         "add_species_interaction() (coldp.coldp method)": [
             [0, "coldp.COLDP.add_species_interaction", false]
         ],
         "add_synonym() (coldp.coldp method)": [
             [0, "coldp.COLDP.add_synonym", false]
         ],
         "add_synonym() (coldp.namebundle method)": [
-            [2, "coldp.NameBundle.add_synonym", false]
+            [3, "coldp.NameBundle.add_synonym", false]
         ],
         "add_type_material() (coldp.coldp method)": [
             [0, "coldp.COLDP.add_type_material", false]
         ],
         "construct_authorship() (coldp.coldp method)": [
             [0, "coldp.COLDP.construct_authorship", false]
         ],
         "construct_species_rank_name() (coldp.coldp method)": [
             [0, "coldp.COLDP.construct_species_rank_name", false]
         ],
         "csv_extensions (in module coldp)": [
             [0, "coldp.csv_extensions", false]
         ],
         "derive_name() (coldp.namebundle method)": [
-            [2, "coldp.NameBundle.derive_name", false]
+            [3, "coldp.NameBundle.derive_name", false]
         ],
         "epithet_and_authorship_match() (coldp.coldp method)": [
             [0, "coldp.COLDP.epithet_and_authorship_match", false]
         ],
         "extract_table() (coldp.coldp method)": [
             [0, "coldp.COLDP.extract_table", false]
         ],
@@ -154,17 +163,23 @@
         ],
         "fix_classification() (coldp.coldp method)": [
             [0, "coldp.COLDP.fix_classification", false]
         ],
         "fix_classification_recursive() (coldp.coldp method)": [
             [0, "coldp.COLDP.fix_classification_recursive", false]
         ],
+        "get_available_column_headings() (coldp.coldp method)": [
+            [0, "coldp.COLDP.get_available_column_headings", false]
+        ],
         "get_children() (coldp.coldp method)": [
             [0, "coldp.COLDP.get_children", false]
         ],
+        "get_identifier_policy() (coldp.coldp method)": [
+            [0, "coldp.COLDP.get_identifier_policy", false]
+        ],
         "get_name() (coldp.coldp method)": [
             [0, "coldp.COLDP.get_name", false]
         ],
         "get_original_authorship() (coldp.coldp method)": [
             [0, "coldp.COLDP.get_original_authorship", false]
         ],
         "get_reference() (coldp.coldp method)": [
@@ -184,14 +199,17 @@
         ],
         "id_mappings (in module coldp)": [
             [0, "coldp.id_mappings", false]
         ],
         "identify_name() (coldp.coldp method)": [
             [0, "coldp.COLDP.identify_name", false]
         ],
+        "initialise() (coldp.identifierpolicy method)": [
+            [1, "coldp.IdentifierPolicy.initialise", false]
+        ],
         "initialise_dataframe() (coldp.coldp method)": [
             [0, "coldp.COLDP.initialise_dataframe", false]
         ],
         "insert_synonym() (coldp.coldp method)": [
             [0, "coldp.COLDP.insert_synonym", false]
         ],
         "insert_taxon() (coldp.coldp method)": [
@@ -211,16 +229,19 @@
         ],
         "modify_taxon() (coldp.coldp method)": [
             [0, "coldp.COLDP.modify_taxon", false]
         ],
         "name_from_nameusage (in module coldp)": [
             [0, "coldp.name_from_nameusage", false]
         ],
+        "next() (coldp.identifierpolicy method)": [
+            [1, "coldp.IdentifierPolicy.next", false]
+        ],
         "normalise_name() (coldp.namebundle method)": [
-            [2, "coldp.NameBundle.normalise_name", false]
+            [3, "coldp.NameBundle.normalise_name", false]
         ],
         "prepare_bundle() (coldp.coldp method)": [
             [0, "coldp.COLDP.prepare_bundle", false]
         ],
         "remove_gender() (coldp.coldp method)": [
             [0, "coldp.COLDP.remove_gender", false]
         ],
@@ -297,15 +318,17 @@
             [0, 0, 1, "", "find_names"],
             [0, 0, 1, "", "find_reference"],
             [0, 0, 1, "", "find_taxon"],
             [0, 0, 1, "", "fix_basionymid"],
             [0, 0, 1, "", "fix_basionyms"],
             [0, 0, 1, "", "fix_classification"],
             [0, 0, 1, "", "fix_classification_recursive"],
+            [0, 0, 1, "", "get_available_column_headings"],
             [0, 0, 1, "", "get_children"],
+            [0, 0, 1, "", "get_identifier_policy"],
             [0, 0, 1, "", "get_name"],
             [0, 0, 1, "", "get_original_authorship"],
             [0, 0, 1, "", "get_reference"],
             [0, 0, 1, "", "get_synonyms"],
             [0, 0, 1, "", "get_synonymy"],
             [0, 0, 1, "", "get_taxon"],
             [0, 0, 1, "", "get_text_tree"],
@@ -414,14 +437,20 @@
             [0, 1, 1, "", "ranks"],
             [0, 1, 1, "", "taxa"]
         ],
         "coldp.COLDP.get_children.params": [
             [0, 1, 1, "", "taxonID"],
             [0, 1, 1, "", "to_dict"]
         ],
+        "coldp.COLDP.get_identifier_policy.params": [
+            [0, 1, 1, "", "default_prefix"],
+            [0, 1, 1, "", "required"],
+            [0, 1, 1, "", "table_name"],
+            [0, 1, 1, "", "volatile"]
+        ],
         "coldp.COLDP.get_name.params": [
             [0, 1, 1, "", "id"]
         ],
         "coldp.COLDP.get_original_authorship.params": [
             [0, 1, 1, "", "authorship"]
         ],
         "coldp.COLDP.get_reference.params": [
@@ -536,813 +565,863 @@
         "coldp.COLDP.table_by_name.params": [
             [0, 1, 1, "", "name"]
         ],
         "coldp.COLDP.validate_record.params": [
             [0, 1, 1, "", "record"],
             [0, 1, 1, "", "record_type"]
         ],
+        "coldp.IdentifierPolicy": [
+            [1, 0, 1, "", "__init__"],
+            [1, 0, 1, "", "initialise"],
+            [1, 0, 1, "", "next"]
+        ],
+        "coldp.IdentifierPolicy.initialise.params": [
+            [1, 1, 1, "", "existing"]
+        ],
+        "coldp.IdentifierPolicy.next.params": [
+            [1, 1, 1, "", "existing"]
+        ],
+        "coldp.IdentifierPolicy.params": [
+            [1, 1, 1, "", "default_prefix"],
+            [1, 1, 1, "", "existing"],
+            [1, 1, 1, "", "required"],
+            [1, 1, 1, "", "volatile"]
+        ],
         "coldp.NameBundle": [
-            [2, 0, 1, "", "__init__"],
-            [2, 0, 1, "", "add_synonym"],
-            [2, 0, 1, "", "derive_name"],
-            [2, 0, 1, "", "normalise_name"]
+            [3, 0, 1, "", "__init__"],
+            [3, 0, 1, "", "add_synonym"],
+            [3, 0, 1, "", "derive_name"],
+            [3, 0, 1, "", "normalise_name"]
         ],
         "coldp.NameBundle.add_synonym.params": [
-            [2, 1, 1, "", "sic"],
-            [2, 1, 1, "", "synonym"]
+            [3, 1, 1, "", "sic"],
+            [3, 1, 1, "", "synonym"]
         ],
         "coldp.NameBundle.derive_name.params": [
-            [2, 1, 1, "", "name"],
-            [2, 1, 1, "", "values"]
+            [3, 1, 1, "", "name"],
+            [3, 1, 1, "", "values"]
         ],
         "coldp.NameBundle.normalise_name.params": [
-            [2, 1, 1, "", "name"],
-            [2, 1, 1, "", "sic"]
+            [3, 1, 1, "", "name"],
+            [3, 1, 1, "", "sic"]
         ],
         "coldp.NameBundle.params": [
-            [2, 1, 1, "", "accepted"],
-            [2, 1, 1, "", "coldp"],
-            [2, 1, 1, "", "incertae_sedis"],
-            [2, 1, 1, "", "sic"]
+            [3, 1, 1, "", "accepted"],
+            [3, 1, 1, "", "coldp"],
+            [3, 1, 1, "", "incertae_sedis"],
+            [3, 1, 1, "", "sic"]
         ]
     },
     "objnames": {
         "0": ["py", "method", "Python method"],
         "1": ["py", "parameter", "Python parameter"],
         "2": ["py", "data", "Python data"]
     },
     "objtypes": {
         "0": "py:method",
         "1": "py:parameter",
         "2": "py:data"
     },
     "terms": {
         "": 0,
-        "1": 0,
-        "10": 3,
-        "1111": 3,
-        "115": 3,
-        "12129": 3,
-        "127": 3,
-        "147": 3,
-        "150": 3,
-        "153": 3,
+        "1": [0, 1],
+        "10": 4,
+        "1111": 4,
+        "115": 4,
+        "12129": 4,
+        "127": 4,
+        "147": 4,
+        "150": 4,
+        "153": 4,
         "1831": 0,
         "1832": 0,
         "1838": 0,
-        "1923": 3,
-        "1978": 3,
-        "2": [0, 3],
-        "2014": 3,
-        "2015": 3,
-        "2019": 3,
-        "25077087": 3,
-        "27259": 3,
-        "3897": 3,
-        "4": 3,
-        "40": 3,
-        "463": 3,
-        "49": 3,
-        "505": 3,
-        "54": 3,
-        "56100973": 3,
-        "671": 3,
-        "697": 3,
-        "704": 3,
-        "819": 3,
-        "A": [0, 1, 3],
-        "At": 1,
+        "1923": 4,
+        "1978": 4,
+        "2": [0, 4],
+        "2014": 4,
+        "2015": 4,
+        "2019": 4,
+        "25077087": 4,
+        "27259": 4,
+        "3897": 4,
+        "4": 4,
+        "40": 4,
+        "463": 4,
+        "49": 4,
+        "505": 4,
+        "54": 4,
+        "56100973": 4,
+        "671": 4,
+        "697": 4,
+        "704": 4,
+        "819": 4,
+        "A": [0, 2, 4],
+        "At": 2,
         "For": 0,
-        "If": 0,
-        "In": [0, 3],
-        "It": [0, 3],
-        "One": [0, 2],
-        "The": [0, 1, 2, 3],
+        "If": [0, 1],
+        "In": [0, 4],
+        "It": [0, 4],
+        "One": [0, 3],
+        "The": [0, 2, 3, 4],
         "Then": 0,
         "These": 0,
-        "__init__": [0, 2],
+        "__init__": [0, 1, 3],
         "_sphinx_paramlinks_coldp": 0,
-        "ab": [0, 3],
+        "ab": [0, 4],
         "absent": 0,
-        "accept": [0, 1, 2, 3],
-        "accepted_taxon_id": [0, 3],
-        "ad": [0, 1, 2, 3],
-        "add": [1, 3],
-        "add_distribut": [0, 3],
-        "add_nam": [0, 1, 2, 3],
+        "accept": [0, 2, 3, 4],
+        "accepted_taxon_id": [0, 4],
+        "account": 0,
+        "activ": [0, 1],
+        "ad": [0, 2, 3, 4],
+        "add": [2, 4],
+        "add_distribut": [0, 4],
+        "add_nam": [0, 2, 3, 4],
         "add_name_rel": 0,
-        "add_refer": [0, 3],
+        "add_refer": [0, 4],
         "add_species_interact": 0,
-        "add_synonym": [0, 2, 3],
+        "add_synonym": [0, 3, 4],
         "add_type_materi": 0,
         "add_typemateri": 0,
-        "addit": [0, 1, 2, 3],
+        "addit": [0, 2, 3, 4],
         "after": 0,
-        "all": [0, 1, 2, 3],
+        "all": [0, 1, 2, 3, 4],
         "allow": 0,
         "allow_repeated_binomi": 0,
         "along": 0,
         "alphabet": 0,
-        "alreadi": [0, 3],
-        "also": [0, 2],
+        "alreadi": [0, 1, 4],
+        "also": [0, 3],
         "alter": 0,
-        "altern": [0, 1],
-        "american": 3,
+        "altern": [0, 2],
+        "alwai": 1,
+        "american": 4,
         "among": 0,
-        "an": [0, 1, 2, 3],
+        "an": [0, 2, 3, 4],
         "ancestri": 0,
-        "ani": [0, 1, 2],
-        "animalia": 3,
+        "ani": [0, 1, 2, 3],
+        "animalia": 4,
         "annot": 0,
-        "anoth": [0, 1],
+        "anoth": [0, 2],
         "appear": 0,
         "append": 0,
         "applic": 0,
-        "appropri": [0, 2],
-        "ar": [0, 1, 3],
-        "area": [0, 3],
+        "appropri": [0, 3],
+        "ar": [0, 1, 2, 4],
+        "area": [0, 4],
         "argument": 0,
         "around": 0,
-        "arthropoda": 3,
+        "arthropoda": 4,
         "assist": 0,
-        "associ": [0, 1, 2, 3],
+        "associ": [0, 1, 2, 3, 4],
         "asterisk": 0,
         "atom": 0,
-        "author": [0, 3],
-        "authorship": [0, 3],
-        "automat": [0, 1],
-        "b": [0, 3],
+        "author": [0, 4],
+        "authorship": [0, 4],
+        "automat": [0, 2],
+        "avoid": 0,
+        "b": [0, 4],
         "back": 0,
-        "base": [0, 2],
-        "basic": [0, 3],
+        "base": [0, 3],
+        "basic": [0, 4],
         "basionym": 0,
-        "basionymid": [0, 1, 3],
+        "basionymid": [0, 2, 4],
         "basionyms_from_synonym": 0,
         "basionyn": 0,
-        "bc": 3,
+        "bc": 4,
         "becom": 0,
         "been": 0,
-        "befor": 0,
+        "befor": [0, 1],
         "being": 0,
         "below": 0,
         "between": 0,
         "binomi": 0,
-        "biodiversitylibrari": 3,
+        "biodiversitylibrari": 4,
         "bodi": 0,
         "boolean": 0,
-        "both": [0, 3],
-        "braun": 3,
-        "braun_1923": 3,
-        "bring": 1,
-        "bundl": [0, 2, 3],
-        "c": 3,
-        "ca": 3,
+        "both": [0, 1, 4],
+        "braun": 4,
+        "braun_1923": 4,
+        "bring": 2,
+        "bundl": [0, 3, 4],
+        "c": 4,
+        "ca": 4,
         "call": 0,
-        "can": [0, 1, 2],
-        "canada": 3,
+        "can": [0, 2, 3],
+        "canada": 4,
         "canon": 0,
         "case": 0,
-        "catalogu": [0, 1],
+        "catalogu": [0, 2],
         "chang": 0,
-        "check": 0,
-        "checklist": 1,
-        "child": [0, 3],
+        "check": [0, 1],
+        "checklist": 2,
+        "child": [0, 4],
         "children": 0,
         "citat": 0,
-        "class": 3,
-        "classif": [0, 3],
+        "class": 4,
+        "classif": [0, 4],
         "classification_from_par": 0,
-        "code": [0, 2, 3],
-        "col": 1,
-        "coldp": 3,
+        "code": [0, 1, 3, 4],
+        "col": 2,
+        "coldp": 4,
         "column": 0,
-        "combin": [0, 1, 3],
+        "combin": [0, 2, 4],
         "comma": 0,
-        "compar": 3,
+        "compar": 4,
         "comparison": 0,
         "complet": 0,
-        "compliant": [0, 1, 2],
+        "compliant": [0, 2, 3],
         "compon": 0,
         "compos": 0,
+        "compris": 1,
+        "concaten": 1,
         "concept": 0,
         "consecut": 0,
-        "consist": 0,
-        "constant": 1,
+        "consist": [0, 1],
+        "constant": 2,
         "construct": 0,
         "construct_authorship": 0,
         "construct_species_rank_nam": 0,
         "constructor": 0,
-        "contain": [0, 1, 2],
-        "containertitl": [0, 3],
-        "content": [0, 1, 3],
+        "contain": [0, 1, 2, 3],
+        "containertitl": [0, 4],
+        "content": [0, 2, 4],
         "context": 0,
         "continu": 0,
         "conveni": 0,
         "convert": 0,
-        "copi": [0, 2],
+        "copi": [0, 3],
         "correct": 0,
         "correctli": 0,
         "correspond": 0,
-        "creat": [0, 1, 2, 3],
+        "corrupt": 0,
+        "creat": [0, 2, 3, 4],
         "create_subspecies_for_infrasubspecif": 0,
         "create_synonyms_without_subgenu": 0,
         "create_taxa_for_not_establish": 0,
-        "creation": 1,
+        "creation": 2,
         "cross": 0,
-        "csv": [0, 1],
+        "csv": [0, 2],
         "csv_extens": 0,
-        "cum": 3,
-        "curent": 3,
-        "current": [0, 3],
-        "d": 3,
-        "data": [0, 1, 3],
+        "cum": 4,
+        "curent": 4,
+        "current": [0, 1, 4],
+        "d": 4,
+        "data": [0, 2, 4],
         "databas": 0,
-        "datafram": [1, 3],
+        "datafram": [1, 2, 4],
         "dataset": 0,
-        "davi": 3,
-        "davis_1978": 3,
-        "default": [0, 3],
+        "davi": 4,
+        "davis_1978": 4,
+        "default": [0, 1, 4],
         "default_head": 0,
-        "default_taxon_record": [0, 3],
-        "delimit": [0, 1],
+        "default_prefix": [0, 1],
+        "default_taxon_record": [0, 4],
+        "delimit": [0, 2],
         "depend": 0,
-        "derive_nam": 2,
+        "derive_nam": 3,
         "descend": 0,
         "destin": 0,
-        "dewaard": 3,
+        "determin": [0, 1],
+        "dewaard": 4,
         "df": 0,
-        "dictionari": [0, 1, 2],
+        "dictionari": [0, 2, 3],
         "differ": 0,
-        "directli": 2,
-        "displai": 3,
-        "distribut": [0, 3],
-        "doe": [0, 2],
-        "doi": 3,
+        "directli": 3,
+        "displai": 4,
+        "distribut": [0, 4],
+        "doe": [0, 3],
+        "doi": 4,
         "drop": 0,
         "e": 0,
-        "each": [0, 3],
+        "each": [0, 1, 4],
         "easi": 0,
-        "edit": 1,
+        "edit": 2,
         "editor": 0,
         "either": 0,
-        "element": [0, 2, 3],
+        "element": [0, 3, 4],
         "els": 0,
-        "empti": [0, 1],
-        "enabl": 3,
+        "empti": [0, 1, 2],
+        "enabl": 4,
         "enclos": 0,
         "end": 0,
-        "ensur": [0, 2],
-        "entomolog": 3,
-        "entomologi": 3,
-        "entomologist": 3,
+        "ensur": [0, 3],
+        "entomolog": 4,
+        "entomologi": 4,
+        "entomologist": 4,
         "epithet": 0,
         "epithet_and_authorship_match": 0,
         "equal": 0,
         "error": 0,
-        "establish": [0, 3],
+        "establish": [0, 4],
         "etc": 0,
         "even": 0,
-        "evolut": 3,
+        "everi": 1,
+        "evolut": 4,
         "exactli": 0,
-        "exampl": [0, 3],
+        "exampl": [0, 4],
         "execut": 0,
-        "exist": [0, 1, 2, 3],
-        "expand": 1,
-        "expect": [0, 2],
+        "exist": [0, 1, 2, 3, 4],
+        "expand": 2,
+        "expect": [0, 3],
         "export": 0,
-        "extant": 3,
+        "extant": 4,
         "extens": 0,
-        "extern": 0,
-        "extra": [0, 2],
+        "extern": [0, 1],
+        "extra": [0, 3],
         "extract": 0,
         "extract_t": 0,
-        "f": [0, 3],
-        "facilit": 1,
+        "f": [0, 4],
+        "facilit": 2,
         "fail": 0,
-        "fals": [0, 2],
-        "famili": [0, 3],
-        "family_id": 3,
+        "fals": [0, 1, 3],
+        "famili": [0, 4],
+        "family_id": 4,
         "field": 0,
-        "file": [0, 1],
+        "file": [0, 2],
         "fill": 0,
         "filter": 0,
-        "final": 3,
+        "final": 4,
         "find_distribut": 0,
         "find_nam": 0,
         "find_name_record": 0,
         "find_refer": 0,
         "find_taxon": 0,
         "first": 0,
-        "fix": 0,
+        "fix": [0, 1],
         "fix_basionym": 0,
         "fix_basionymid": 0,
         "fix_classif": 0,
         "fix_classification_recurs": 0,
-        "flag": [0, 2],
-        "folder": [0, 1, 3],
+        "flag": [0, 1, 3],
+        "folder": [0, 2, 4],
         "foldernam": 0,
-        "follow": [0, 2, 3],
+        "follow": [0, 3, 4],
         "foreign": 0,
         "forign": 0,
         "form": 0,
-        "format": [0, 1, 2, 3],
+        "format": [0, 2, 3, 4],
         "forward": 0,
         "found": 0,
-        "four": [0, 3],
+        "four": [0, 4],
         "frame": 0,
         "free": 0,
-        "from": [0, 1, 2, 3],
-        "fuscoleuca": 3,
-        "g": [0, 3],
-        "gazett": [0, 3],
+        "from": [0, 2, 3, 4],
+        "fuscoleuca": 4,
+        "futur": [0, 1],
+        "g": [0, 4],
+        "gazett": [0, 4],
         "gender": 0,
-        "gener": [0, 3],
-        "genera": 3,
-        "genu": [0, 3],
-        "genus_id": 3,
-        "get": 3,
+        "gener": [0, 4],
+        "genera": 4,
+        "genu": [0, 4],
+        "genus_id": 4,
+        "get": 4,
+        "get_available_column_head": 0,
         "get_children": 0,
+        "get_identifier_polici": 0,
         "get_nam": 0,
         "get_original_authorship": 0,
         "get_refer": 0,
         "get_synonym": 0,
         "get_synonymi": 0,
         "get_taxon": 0,
-        "get_text_tre": [0, 3],
+        "get_text_tre": [0, 4],
         "given": 0,
         "greek": 0,
         "group": 0,
         "guarante": 0,
         "ha": 0,
-        "handl": [0, 2],
-        "harrison": 3,
+        "handl": [0, 3],
+        "harrison": 4,
+        "have": [0, 1],
         "head": 0,
-        "helper": 1,
+        "helper": 2,
         "hierarch": 0,
         "hierarchi": 0,
-        "higher": 0,
+        "higher": [0, 1],
         "highest": 0,
-        "histori": 3,
-        "hold": [0, 1],
+        "histori": 4,
+        "hold": [0, 2],
         "housekeep": 0,
-        "http": 3,
-        "i": [0, 1, 2, 3],
+        "http": 4,
+        "i": [0, 1, 2, 3, 4],
         "icbn": 0,
         "iczn": 0,
-        "id": [0, 3],
+        "id": [0, 1, 2, 4],
         "id_map": 0,
         "ident": 0,
-        "identifi": [0, 1],
+        "identifi": [0, 2],
+        "identifierpolici": [0, 2],
         "identify_nam": 0,
         "ignor": 0,
-        "illustr": 3,
+        "illustr": 4,
         "immedi": 0,
         "impli": 0,
-        "implic": 3,
-        "implicit": 1,
-        "import": [0, 3],
-        "incerta": [0, 2],
-        "incertae_sedi": [0, 2],
-        "includ": [0, 1, 3],
-        "incurvariida": 3,
-        "incurvariin": 3,
+        "implic": 4,
+        "implicit": 2,
+        "import": [0, 4],
+        "incerta": [0, 3],
+        "incertae_sedi": [0, 3],
+        "includ": [0, 2, 4],
+        "increment": 1,
+        "incurvariida": 4,
+        "incurvariin": 4,
         "inde": 0,
         "indent": 0,
-        "indic": [0, 2],
+        "indic": [0, 1, 3],
         "infer": 0,
         "infraspecif": 0,
         "infrasubspecif": 0,
-        "initalis": 0,
         "initial_prefix": 0,
-        "initialis": [0, 1],
+        "initialis": [0, 1, 2],
         "initialise_datafram": 0,
-        "insecta": 3,
+        "insecta": 4,
         "insensit": 0,
-        "insert": [0, 1],
+        "insert": [0, 2],
         "insert_species_for_trinomi": 0,
         "insert_synonym": 0,
         "insert_taxon": 0,
         "insid": 0,
-        "instanc": [0, 1, 3],
-        "instanti": 1,
-        "instead": [0, 2],
-        "integ": 0,
+        "instanc": [0, 1, 2, 4],
+        "instanti": 2,
+        "instead": [0, 3],
+        "integ": [0, 1],
         "intend": 0,
         "interact": 0,
-        "intern": 1,
-        "invalid": 2,
+        "intern": [1, 2],
+        "invalid": 3,
+        "invoc": [0, 1],
         "is_basionym": 0,
         "is_infrasubspecif": 0,
         "is_species_group": 0,
-        "iso": 3,
-        "issu": [0, 2, 3],
+        "iso": 4,
+        "issu": [0, 3, 4],
         "issues_to_stdout": 0,
         "ital": 0,
-        "item": 3,
-        "its": [0, 1],
-        "j": 3,
-        "jstor": 3,
+        "item": 4,
+        "its": [0, 2],
+        "j": 4,
+        "jstor": 4,
         "just": 0,
-        "k": 3,
-        "kei": [0, 2],
+        "k": 4,
+        "kei": [0, 3],
         "keyword": 0,
-        "kingdom": [0, 3],
-        "l": 3,
+        "kingdom": [0, 4],
+        "l": 4,
         "label": 0,
         "lack": 0,
-        "lampronia": 3,
-        "landri": 3,
-        "latest": 1,
+        "lampronia": 4,
+        "landri": 4,
+        "latest": 2,
         "latin": 0,
         "least": 0,
-        "leav": 3,
-        "lepidoptera": 3,
+        "leav": 4,
+        "length": 1,
+        "lepidoptera": 4,
         "level": 0,
-        "life": [0, 1, 3],
+        "life": [0, 2, 4],
         "like": 0,
-        "lineag": 3,
-        "link": 3,
+        "lineag": 4,
+        "link": 4,
         "list": 0,
-        "load": [0, 1, 3],
-        "locat": [0, 3],
-        "log": [0, 2],
-        "logic": 2,
+        "load": [0, 2, 4],
+        "locat": [0, 4],
+        "log": [0, 3],
+        "logic": 3,
         "lower": 0,
         "lowest": 0,
-        "m": 3,
+        "m": 4,
         "made": 0,
-        "mai": [0, 1],
-        "main": 1,
+        "mai": [0, 1, 2],
+        "main": 2,
         "major": 0,
-        "manag": [0, 1, 2, 3],
-        "mani": 1,
-        "manipul": 1,
-        "map": [0, 2],
-        "mark": 2,
+        "manag": [0, 1, 2, 3, 4],
+        "mani": 2,
+        "manipul": 2,
+        "map": [0, 3],
+        "mark": 3,
         "marker": 0,
-        "match": [0, 2],
+        "match": [0, 3],
+        "maximum": 1,
         "mechan": 0,
-        "memori": 1,
+        "memori": 2,
         "messag": 0,
-        "method": 1,
-        "microlepidoptera": 3,
-        "minim": 2,
-        "minimum": 1,
-        "miss": [0, 2],
-        "mitter": 3,
-        "mixtur": 3,
+        "method": 2,
+        "microlepidoptera": 4,
+        "minim": 3,
+        "minimum": 2,
+        "miss": [0, 3],
+        "mitter": 4,
+        "mixtur": 4,
+        "modifi": 1,
         "modify_nam": 0,
         "modify_taxon": 0,
-        "molecular": 3,
-        "monotyp": 3,
-        "more": [0, 2],
-        "morphologi": 3,
+        "molecular": 4,
+        "monotyp": 4,
+        "more": [0, 3],
+        "morphologi": 4,
         "most": 0,
-        "moth": 3,
+        "moth": 4,
         "move": 0,
         "multilin": 0,
         "multipl": 0,
-        "must": 0,
-        "name": [0, 1, 2, 3],
+        "must": [0, 1],
+        "name": [0, 2, 3, 4],
         "name_from_nameusag": 0,
         "name_id": 0,
         "name_rel": 0,
         "nameand": 0,
-        "namebundl": [0, 1, 3],
+        "namebundl": [0, 2, 4],
         "nameid": 0,
-        "namerel": [0, 3],
+        "namerel": [0, 4],
         "nameusag": 0,
         "nan": 0,
-        "nativ": 3,
-        "necessari": [0, 2],
+        "nativ": 4,
+        "necessari": [0, 3],
         "need": 0,
         "nest": 0,
-        "new": [0, 1, 2, 3],
-        "next": 0,
+        "new": [0, 1, 2, 3, 4],
+        "next": [0, 1],
         "node": 0,
         "nomenclatur": 0,
-        "nonditrysian": 3,
-        "none": 0,
-        "normal": [0, 1, 2],
-        "normalis": [0, 2],
-        "normalise_nam": 2,
-        "north": 3,
-        "note": 3,
+        "nonditrysian": 4,
+        "none": [0, 1],
+        "normal": [0, 2, 3],
+        "normalis": [0, 3],
+        "normalise_nam": 3,
+        "north": 4,
+        "note": 4,
         "number": 0,
+        "numer": [0, 1],
         "numpi": 0,
         "o": 0,
-        "object": [0, 1, 2, 3],
+        "object": [0, 2, 3, 4],
         "occur": 0,
         "often": 0,
-        "oldest": 3,
+        "oldest": 4,
         "omit": 0,
-        "onc": [0, 1],
-        "one": [0, 1, 2],
-        "onli": [0, 3],
-        "option": [0, 1],
-        "order": [0, 3],
-        "org": 3,
-        "organis": 1,
-        "origin": [0, 3],
-        "other": [0, 1, 3],
-        "otherwis": 0,
+        "onc": [0, 2],
+        "one": [0, 1, 2, 3],
+        "onli": [0, 1, 4],
+        "option": [0, 2],
+        "order": [0, 4],
+        "org": 4,
+        "organis": 2,
+        "origin": [0, 4],
+        "other": [0, 2, 4],
+        "otherwis": [0, 1],
         "output": 0,
         "over": 0,
-        "overrid": 2,
+        "overrid": 3,
         "own": 0,
-        "p": 3,
-        "pacif": 3,
-        "packag": [1, 2],
-        "page": [0, 1, 2, 3],
-        "pan": 3,
-        "panda": [0, 1],
+        "p": 4,
+        "pacif": 4,
+        "packag": [2, 3],
+        "page": [0, 1, 2, 3, 4],
+        "pan": 4,
+        "panda": [0, 1, 2],
         "param": 0,
-        "paramet": [0, 2],
+        "paramet": [0, 1, 3],
+        "paramref": 1,
         "parent": 0,
         "parenthensi": 0,
         "parenthes": 0,
         "parenthood": 0,
         "parentid": 0,
-        "pars": 3,
+        "pars": 4,
         "part": 0,
         "pass": 0,
         "path": 0,
-        "pattern": 3,
+        "pattern": 4,
         "per": 0,
-        "phylogeni": 3,
-        "phylum": [0, 3],
-        "pip": 1,
-        "pohl": 3,
-        "pohl_et_al_2019": 3,
+        "phylogeni": 4,
+        "phylum": [0, 4],
+        "pip": 2,
+        "plain": 1,
+        "pohl": 4,
+        "pohl_et_al_2019": 4,
         "point": 0,
-        "posit": 0,
+        "polici": [0, 1],
+        "posit": [0, 1],
         "possibl": 0,
         "potenti": 0,
         "prece": 0,
         "preced": 0,
         "prefer": 0,
-        "prefix": 0,
+        "prefix": [0, 1],
         "prepar": 0,
         "prepare_bundl": 0,
         "prepend": 0,
-        "present": 0,
+        "present": [0, 1],
         "preserv": 0,
         "previou": 0,
-        "print": [0, 3],
+        "print": [0, 4],
         "problem": 0,
-        "process": [0, 2],
+        "process": [0, 3],
         "produc": 0,
         "properli": 0,
-        "properti": [0, 2, 3],
-        "provid": [0, 3],
+        "properti": [0, 3, 4],
+        "provid": [0, 1, 4],
         "public": 0,
-        "publishedinpag": 3,
-        "publishedinyear": 3,
-        "py": 1,
-        "pypi": 1,
-        "python": 1,
-        "queri": 1,
+        "publishedinpag": 4,
+        "publishedinyear": 4,
+        "py": 2,
+        "pypi": 2,
+        "python": 2,
+        "queri": 2,
         "question": 0,
-        "r": 3,
-        "rank": [0, 3],
+        "r": 4,
+        "rank": [0, 4],
         "read": 0,
+        "recalcul": 1,
         "recent": 0,
         "recognis": 0,
-        "record": [1, 2, 3],
+        "record": [2, 3, 4],
         "record_typ": 0,
         "recurs": 0,
-        "refer": [0, 3],
+        "refer": [0, 4],
         "referenc": 0,
         "reference_head": 0,
         "reference_list": 0,
-        "referenceid": [0, 3],
-        "regier": 3,
-        "regier_et_al_2014": 3,
-        "regist": [0, 2],
+        "referenceid": [0, 4],
+        "refresh": 1,
+        "regier": 4,
+        "regier_et_al_2014": 4,
+        "regist": [0, 3],
         "reject": 0,
         "relatednameid": 0,
-        "relationship": [0, 1],
-        "relev": [0, 3],
+        "relationship": [0, 2],
+        "relev": [0, 4],
         "remov": 0,
         "remove_gend": 0,
         "renam": 0,
         "replac": 0,
-        "report": [0, 2],
-        "repres": [0, 1],
+        "report": [0, 3],
+        "repres": [0, 2],
         "represent": 0,
         "request": 0,
-        "requir": 0,
+        "requir": [0, 1],
         "reset": 0,
         "reset_id": 0,
         "resolv": 0,
-        "result": [0, 2],
-        "return": [0, 2],
-        "review": 0,
+        "result": [0, 3],
+        "return": [0, 1, 3],
+        "review": [0, 1],
+        "revis": 1,
         "ridden": 0,
         "root": 0,
         "row": 0,
-        "rule": 2,
-        "run": 3,
+        "rule": 3,
+        "run": 4,
         "s_": 0,
-        "same": [0, 3],
+        "same": [0, 4],
         "same_basionym": 0,
         "satisfi": 0,
-        "save": [1, 3],
-        "schmidt": 3,
-        "scientif": [0, 1],
-        "scientificnam": [0, 3],
-        "second": [0, 3],
+        "save": [2, 4],
+        "scan": 1,
+        "schmidt": 4,
+        "scientif": [0, 2],
+        "scientificnam": [0, 4],
+        "second": [0, 4],
         "section": 0,
-        "sedi": [0, 2],
+        "sedi": [0, 3],
         "see": 0,
         "select": 0,
         "separ": 0,
         "sequenc": 0,
-        "serialis": [0, 1],
+        "seri": 1,
+        "serialis": [0, 2],
         "serv": 0,
-        "set": [0, 1, 2],
+        "set": [0, 1, 2, 3],
         "set_basionymid": 0,
         "set_context": 0,
         "set_default_taxon_record": 0,
         "set_opt": 0,
         "sg": 0,
         "share": 0,
-        "should": [0, 1, 2],
-        "show": [0, 3],
+        "should": [0, 1, 2, 3],
+        "show": [0, 4],
         "sibl": 0,
-        "sic": [0, 2],
+        "sic": [0, 3],
         "side": 0,
         "sign": 0,
         "simpli": 0,
-        "simplifi": [0, 1],
-        "sinc": [0, 3],
-        "singl": 3,
-        "so": [0, 1],
-        "societi": 3,
-        "sohn": 3,
+        "simplifi": [0, 2],
+        "sinc": [0, 4],
+        "singl": 4,
+        "so": [0, 2],
+        "societi": 4,
+        "sohn": 4,
         "sort": 0,
         "sort_nam": 0,
         "sort_taxa": 0,
         "sort_taxa_recurs": 0,
         "sourc": 0,
         "space": 0,
-        "speci": [0, 1, 3],
-        "species_id": 3,
+        "speci": [0, 2, 4],
+        "species_id": 4,
         "species_interact": 0,
         "species_taxon_id": 0,
-        "speciesinteract": [0, 3],
+        "speciesinteract": [0, 4],
         "specif": 0,
         "specifi": 0,
-        "specificepithet": [0, 3],
+        "specificepithet": [0, 4],
         "spreadsheet": 0,
         "ss": 0,
-        "stabl": 3,
-        "start_name_bundl": [0, 1, 2, 3],
-        "statu": [0, 3],
+        "stabl": 4,
+        "start_name_bundl": [0, 2, 3, 4],
+        "statu": [0, 4],
         "stdout": 0,
         "step": 0,
         "store": 0,
-        "string": [0, 3],
+        "string": [0, 1, 4],
         "strip": 0,
         "subclass": 0,
         "subfamili": 0,
-        "subfold": [0, 3],
+        "subfold": [0, 4],
         "subgener": 0,
         "subgenu": 0,
-        "submit": 2,
+        "submit": 3,
         "subord": 0,
         "subphylum": 0,
-        "subsequ": 0,
+        "subsequ": [0, 1],
         "subset": 0,
         "subspeci": 0,
         "subspecif": 0,
         "subtrib": 0,
         "subvar": 0,
         "superfamili": 0,
-        "supplement": 2,
-        "suppli": [0, 1, 2],
+        "supplement": 3,
+        "suppli": [0, 2, 3],
         "support": 0,
-        "syen": 3,
-        "synonym": [0, 1, 2, 3],
+        "syen": 4,
+        "synonym": [0, 2, 3, 4],
         "synonym_from_nameusag": 0,
         "synonym_prefix": 0,
         "synonymis": 0,
-        "systemat": 3,
-        "t": 3,
-        "tab": [0, 1],
-        "tabl": [0, 3],
+        "systemat": 4,
+        "t": 4,
+        "tab": [0, 2],
+        "tabl": [0, 1, 4],
         "table_by_nam": 0,
+        "table_nam": 0,
+        "take": 0,
         "taken": 0,
         "target": 0,
-        "taxa": [0, 1, 3],
-        "taxon": [0, 1, 2, 3],
-        "taxon_default": 3,
+        "taxa": [0, 2, 4],
+        "taxon": [0, 2, 3, 4],
+        "taxon_default": 4,
         "taxon_from_nameusag": 0,
         "taxon_id": 0,
-        "taxonid": [0, 3],
-        "taxonom": [0, 1],
-        "tee": 3,
+        "taxonid": [0, 4],
+        "taxonom": [0, 2],
+        "tee": 4,
         "term": 0,
-        "text": [0, 3],
-        "than": 0,
+        "text": [0, 4],
+        "than": [0, 1],
         "thei": 0,
-        "thi": [0, 1, 2, 3],
+        "thi": [0, 1, 2, 3, 4],
         "those": 0,
-        "three": 3,
+        "three": [2, 4],
         "through": 0,
-        "time": [0, 3],
-        "titl": [0, 3],
+        "time": [0, 4],
+        "titl": [0, 4],
         "to_dict": 0,
-        "togeth": 1,
-        "tool": [0, 1],
+        "togeth": 2,
+        "tool": [0, 2],
         "top": 0,
-        "transact": 3,
+        "transact": 4,
         "tree": 0,
         "tribe": 0,
-        "tridentaforma": 3,
-        "tridentaformida": 3,
-        "trigger": 1,
+        "tridentaforma": 4,
+        "tridentaformida": 4,
+        "trigger": 2,
         "trinomi": 0,
-        "true": 0,
+        "true": [0, 1],
         "tsv": 0,
-        "tupl": 0,
-        "two": [0, 1, 3],
+        "tupl": [0, 1],
+        "two": [0, 4],
         "txt": 0,
         "type": 0,
         "type_materi": 0,
-        "typemateri": [0, 3],
-        "u": [0, 3],
+        "typemateri": [0, 4],
+        "u": [0, 4],
         "um": 0,
-        "unchang": [0, 3],
-        "uninomi": 3,
-        "unless": 0,
+        "unchang": [0, 4],
+        "uninomi": 4,
+        "unless": [0, 1],
         "unus": 0,
-        "updat": [0, 2],
+        "updat": [0, 3],
         "upon": 0,
-        "us": [0, 1, 2],
-        "usag": 2,
+        "us": [0, 1, 2, 3],
+        "usag": 3,
         "user": 0,
-        "valid": [0, 3],
+        "valid": [0, 4],
         "validate_record": 0,
-        "valu": [0, 1, 2],
+        "valu": [0, 1, 2, 3],
         "var": 0,
-        "variabl": 0,
-        "variant": 1,
-        "variat": 2,
+        "variabl": [0, 1],
+        "variant": 2,
+        "variat": 3,
         "varieti": 0,
         "verifi": 0,
-        "version": [0, 1],
-        "via": [0, 1],
+        "version": [0, 2],
+        "via": [0, 2],
         "view": 0,
-        "volum": [0, 3],
+        "volatil": [0, 1],
+        "volum": [0, 4],
         "wai": 0,
         "warn": 0,
         "well": 0,
-        "when": [0, 3],
+        "when": [0, 4],
         "whenev": 0,
         "where": 0,
-        "whether": 0,
-        "which": [0, 2],
+        "whether": [0, 1],
+        "which": [0, 3],
+        "while": [0, 1],
         "whole": 0,
         "within": 0,
-        "without": [0, 2],
+        "without": [0, 3],
         "word": 0,
-        "work": 1,
-        "would": 3,
-        "wrapper": 2,
+        "work": 2,
+        "would": 4,
+        "wrapper": 3,
         "write": 0,
         "written": 0,
-        "www": 3,
+        "www": 4,
         "y": 0,
         "year": 0,
-        "zookei": 3,
+        "zookei": 4,
         "zoolog": 0,
-        "zwick": 3
+        "zwick": 4
     },
-    "titles": ["coldp.COLDP", "coldp", "coldp.NameBundle", "Usage"],
+    "titles": ["coldp.COLDP", "coldp.IdentifierPolicy", "coldp", "coldp.NameBundle", "Usage"],
     "titleterms": {
         "access": 0,
         "add": 0,
         "behaviour": 0,
-        "class": [0, 1, 2],
-        "coldp": [0, 1, 2],
+        "class": [0, 1, 2, 3],
+        "coldp": [0, 1, 2, 3],
         "constant": 0,
         "control": 0,
         "datafram": 0,
         "find": 0,
         "get": 0,
-        "index": [0, 1, 2],
-        "instal": 1,
+        "identifierpolici": 1,
+        "index": [0, 1, 2, 3],
+        "instal": 2,
         "intern": 0,
-        "method": [0, 2],
+        "method": [0, 1, 3],
         "modifi": 0,
-        "namebundl": 2,
-        "overview": 1,
+        "namebundl": 3,
+        "overview": 2,
         "packag": 0,
         "record": 0,
         "save": 0,
-        "search": [0, 1, 2],
+        "search": [0, 1, 2, 3],
         "tidi": 0,
-        "usag": [1, 3],
+        "usag": [2, 4],
         "util": 0
     }
 })
```

### Comparing `coldp-2024.5.3/docs/build/html/usage.html` & `coldp-2024.5.4/docs/build/html/usage.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Usage &#8212; COLDP 2024.5.3 documentation</title>
+    <title>Usage &#8212; COLDP 2024.5.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
+    <script src="_static/documentation_options.js?v=78d2dd00"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="prev" title="coldp.NameBundle" href="name-bundle.html" />
+    <link rel="prev" title="coldp.IdentifierPolicy" href="identifier-policy.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
 
   
   
 
@@ -216,24 +216,25 @@
 
 
 
 <h3>Navigation</h3>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="coldp.html">coldp.COLDP</a></li>
 <li class="toctree-l1"><a class="reference internal" href="name-bundle.html">coldp.NameBundle</a></li>
+<li class="toctree-l1"><a class="reference internal" href="identifier-policy.html">coldp.IdentifierPolicy</a></li>
 </ul>
 <ul class="current">
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Usage</a></li>
 </ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
-      <li>Previous: <a href="name-bundle.html" title="previous chapter">coldp.NameBundle</a></li>
+      <li>Previous: <a href="identifier-policy.html" title="previous chapter">coldp.IdentifierPolicy</a></li>
   </ul></li>
 </ul>
 </div>
 <search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
```

#### html2text {}

```diff
@@ -166,15 +166,16 @@
 print(coldp.taxa)
 print(coldp.synonyms)
 print(coldp.distributions)
 ************ _CC_OO_LL_DD_PP ************
 ******** NNaavviiggaattiioonn ********
     * _c_o_l_d_p_._C_O_L_D_P
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+    * _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
     * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
-          o Previous: _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+          o Previous: _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
 ©2024, Donald Hobern. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r_ _0_._7_._1_6 | _P_a_g_e
 _s_o_u_r_c_e
```

### Comparing `coldp-2024.5.3/docs/build/html/_static/alabaster.css` & `coldp-2024.5.4/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/html/_static/basic.css` & `coldp-2024.5.4/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/html/_static/doctools.js` & `coldp-2024.5.4/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/html/_static/language_data.js` & `coldp-2024.5.4/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/html/_static/pygments.css` & `coldp-2024.5.4/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/html/_static/searchtools.js` & `coldp-2024.5.4/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/html/_static/sphinx_highlight.js` & `coldp-2024.5.4/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/COLDP.pdf` & `coldp-2024.5.4/docs/build/simplepdf/COLDP.pdf`

 * *Files 24% similar despite different names*

#### Comparing `coldp-2024.5.3/docs/build/simplepdf/COLDP.pdf` & `coldp-2024.5.4/docs/build/simplepdf/COLDP.pdf`

 * *Document info*

```diff
@@ -1,2 +1,2 @@
 Producer: 'WeasyPrint 62.1'
-Title: '\n   COLDP 2024.5.3 documentation\n  '
+Title: '\n   COLDP 2024.5.4 documentation\n  '
```

#### pdftotext {} -

```diff
@@ -14,27 +14,27 @@
 
 Methods
 
 8
 
 Constants
 
-20
+22
 
 Internal methods
 
-21
+23
 
 Index and search
 
-30
+31
 
 coldp.NameBundle
 
-30
+31
 
 •
 •
 •
 •
 •
 •
@@ -47,37 +47,58 @@
 
 Methods
 
 8
 
 Index and search
 
-30
+31
 
-Usage
+coldp.IdentifierPolicy
 
 33
 
+•
+•
+•
+
+Class
+
+6
+
+Methods
+
+8
+
+Index and search
+
+31
+
+Usage
+
+36
+
 3
 
 coldp
 Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package
 (COLDP) format
 
 4
 
 Overview
 
 Overview
 coldp is a Python package to facilitate creation, manipulation, editing and serialisation of
 taxonomic checklists in the COL Data Package (COLDP) format.
-The package includes two classes:
+The package includes three classes:
 • coldp.COLDP - A COLDP package loaded as a set of Pandas dataframes
 • coldp.NameBundle - A helper class to simplify addition of taxon names with sets of associated
 synonyms to a COLDP instance
+• coldp.IdentifierPolicy - An internal class to manage ID values in COLDP dataframes
 The main COLDP class instantiates a COLDP package in memory as a set of Pandas dataframes. An
 instance may be initialised from the contents of a folder containing a set of COLDP-compliant CSV
 or tab-delimited data files or alternatively can be initialised as an empty instance in memory. The
 class includes many methods for inserting new data, editing existing records and querying the
 contents of the package. The instance can then be saved as a set of CSV files in a named folder .
 The NameBundle class brings together a scientific name and its synonyms so that these can be
 added together and the COLDP package can automatically manage their relationships
@@ -196,15 +217,15 @@
 • issues_to_stdout – If true, print any issue messages (see
 issue() ) to stdout as well as inserting then in the issue
 dataframe.
 • context – Value to be used in labeling issue records (see
 issue() ). This value is more normally set using
 set_context() .
 
-A COLDP object is initalised with a source/destination folder, COLDP package name and
+A COLDP object is initialised with a source/destination folder, COLDP package name and
 other options.
 If a subfolder exists with the supplied name in the supplied folder, it will be initialised with
 data from any CSV/TSV files it contains with any of the following base names: name, taxon,
 synonym, reference, distribution, speciesinteraction, namerelation, typematerial or
 nameusage, and with a file extension recognised via csv_extensions . File names are case
 insensitive.
 Files with the base name nameusage are loaded only if the name, taxon or synonym file is
@@ -326,15 +347,15 @@
 Parameters :
 reference_list – List of dictionaries - each dictionary
 contains values keyed by terms from reference_headings
 Returns :
 Updated reference_list with IDs for references in this
 COLDP instance
 Find existing ID values for each supplied reference, based on identity of: author, title, issued,
-containerTitle, volume, issue, page and citation. Add ID to the appropriate reference
+containerTitle, volume, issue, page and citation. Add ID from the appropriate reference
 dictionary in references. If none found, set ID to next unused index and add to references.
 The list is returned updated with current ID values so these can be used for referenceID
 values in other classes.
 COLDP. add_type_material ( type_material )
 Add COLDP TypeMaterial record to COLDP instance
 Parameters :
 type_material – COLDP TypeMaterial record represented as
@@ -425,40 +446,69 @@
 Defaults to name supplied to constructor, which defaults
 to None. If no name provided, save will fail.
 If necessary creates subfolder with name name in destination , and then writes CSV file
 representations for all DataFrames in the folder. Empty columns are dropped. Any numpy
 NAN elements are replaced with an empty string.
 
 Find or get records
-COLDP. find_name_record ( name )
-Return record from names DataFrame matching key fields (scientificName, authorship and
-rank) in supplied record
+COLDP. find_taxon ( scientificName , authorship , rank )
+Get COLDP Taxon record (as Pandas dataframe) with accepted name matching supplied
+scientificName, authorship and rank values
 Parameters :
-name – Dictionary containing Name properties
+• scientificName – Scientific name in canonical format
+• authorship – Authorship string
+• rank – Rank name string
 Returns :
-Dictionary containing matching record if found
 
 Classes
 
 15
+COLDP Taxon record matching supplied parameters
 
+Logs a warning issue if multiple taxon records exist for a matching name and returns the
+first such match. Returns None if no match.
+COLDP. find_name_record ( name )
+Return record from names DataFrame matching key fields (scientificName, authorship and
+rank) in supplied record
+Parameters :
+name – Dictionary containing Name properties
+Returns :
+Dictionary containing matching record if found
 Locates any existing record in the names DataFrame that matches the supplied
 scientificName, authorship and rank and returns it as a COLDP Name properties dictionary,
 or None if no match is found.
 COLDP. find_names ( properties , to_dict = False )
 Get all COLDP Name records matching all the supplied properties
 Parameters :
 • properties – Dictionary of property values to serve as filter
 • to_dict – True if records should be converted from Pandas
 format to dictionary records, False (default) otherwise.
 Returns :
 Set of COLDP Name records either as DataFrame or list of
 dictionaries
 Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches,
 None is returned.
+COLDP. find_name ( scientificName , authorship , rank )
+Return record from names DataFrame matching supplied scientificName, authorship and
+rank
+
+Classes
+
+16
+Parameters :
+• scientificName – Scientific name in canonical format
+• authorship – Authorship string
+• rank – Rank name string
+Returns :
+Dictionary containing matching record if found
+
+Locates any existing record in the names DataFrame that matches the supplied
+scientificName, authorship and rank and returns it as a COLDP Name properties dictionary,
+or None if no match is found.
+If authorship is None, returns a name based only on scientificName and rank.
 COLDP. find_distribution ( distribution )
 Locate existing COLDP distribution record exactly matching all major fields in
 distribution
 
 Parameters :
 distribution – Dictionary of COLDP distribution properties
 representing a record to be found
@@ -468,15 +518,15 @@
 Only returns a record that exactly matches the values supplied in distribution for all of
 taxonID, area, gazetteer, status, referenceID.
 COLDP. get_name ( id )
 Return record from names DataFrame with supplied ID
 
 Classes
 
-16
+17
 Parameters :
 id – String ID for COLDP Name record
 Returns :
 Pandas DataFrame containing matching record if found
 
 Locates any existing record in the names DataFrame with the supplied ID, or None if no
 match is found. If multiple matches are found, logs an issue and returns the first.
@@ -498,15 +548,15 @@
 COLDP. get_synonyms ( taxonID , to_dict = False )
 Get all COLDP Synonym records for the supplied taxon ID
 Parameters :
 • taxonID – String taxonID value
 
 Classes
 
-17
+18
 • to_dict – True if records should be converted from Pandas
 format to dictionary records, False (default) otherwise.
 Returns :
 Set of COLDP Synonym records for taxon either as
 DataFrame or list of dictionaries
 
 Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches,
@@ -531,15 +581,15 @@
 • taxonID – String ID for COLDP Taxon record
 • to_dict – True if records should be converted from Pandas
 format to dictionary records, False (default) otherwise.
 Returns :
 
 Classes
 
-18
+19
 Set of COLDP Taxon records for children of identified taxon
 either as DataFrame or list of dictionaries
 
 Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches,
 None is returned.
 
 Tidy package
@@ -567,15 +617,15 @@
 alphabetically by scientific nameand each is followed immediately by its children and their
 descendents also sorted alphabetically. The result is a tree with siblings ordered
 alphabetically.
 Existing ID values for all records are unchanged.
 
 Classes
 
-19
+20
 
 This is a convenience method to simplify review of the data in a spreadsheet or editor tool.
 It also simplifies import of the data into a database since there are no forward references to
 parent taxa.
 COLDP. sort_names ( )
 Sort name records to match order of records in taxa dataframe and with accepted names
 and synonyms sorted alphabetically
@@ -603,29 +653,61 @@
 COLDP. get_text_tree ( taxonID , indent = ' ' , initial_prefix = '' , synonym_prefix = ' = ' )
 Generate formatted text tree for specified taxon and its descendents
 Parameters :
 • taxonID – String ID for taxon to be formatted
 
 Classes
 
-20
+21
 • indent – Indent string to be added one or more times
 before each nested row, defaults to two spaces
 • initial_prefix – Optional prefix string for all rows (preceeds
 indentation), defaults to empty string
 • synonym_prefix – Prefix to appear before synonymised
 names, defaults to an equal sign with spaces on either
 side
 Returns :
 Multiline string representation of taxonomic hierarchy
 
 The tree view shows the name, authorship and rank for the selected taxon. Synonyms
 follow, one to a row at the same indent level but preceded by a space and an asterisk. Then
 each child follows, indented two more spaces per level, with its own synonyms and children
 following.
+COLDP. get_available_column_headings ( )
+Return dictionary mapping table names to lists of supported columns
+Returns :
+Dictionary containing copies of internal heading lists
+Returns copies to avoid corrupting the lists used in this class
+COLDP. get_identifier_policy ( table_name , default_prefix = None , required = True , volatile =
+False )
+Find or create IdentifierPolicy associated with named table
+Parameters :
+• table_name – Name of COLDP dataframe for which policy
+is required
+• default_prefix – String prefix to use before numeric ID
+values if existing ID values are not consistently positive
+integer values
+• required – Flag to indicate whether the table must have ID
+values - if False, the IdentifierPolicy will return None
+unless existing already contains ID values
+
+Classes
+
+22
+• volatile – Flag to indicate if external code may modify ID
+values while the current COLDP instance is active - if False,
+the policy and future values will be determined on
+initialisation, otherwise the policy will be reviewed for
+each new ID value
+Returns :
+IdentifierPolicy object or None if no policy is required for
+
+the table
+Creates new IdentifierPolicy instance if this is the first invocation for the given table.
+Policies take into account any existing ID values for the table.
 
 Access to DataFrames
 COLDP. table_by_name ( name )
 Return dataframe for named COLDP data class
 Parameters :
 name – Name of data frame to return (one of: name, taxon,
 synonym,
@@ -637,20 +719,20 @@
 Requested dataframe or None if no such table exists
 Returns dataframe if one exists for supplied name.
 
 Constants
 coldp. csv_extensions
 Dictionary mapping supported CSV/TSV file extensions to the expected delimiter.
 Supported extensions are .csv for comma-separated data files and .tsv or .txt for tabdelimited data files.
+coldp. id_mappings
 
 Classes
 
-21
+23
 
-coldp. id_mappings
 Dictionary mapping table names (name, taxon, reference or synonym) to a dictionary that
 maps another table name to the properties in the second table that reference ID values
 from the first table.
 For example, id_mappings maps the key “name” to a dictionary that includes the key
 “namerelation” with a list containing “nameID” and “relatedNameID” as its value.
 This is a map of the foreign-key relationships that need to be validated and preserved
 between the COLDP data tables.
@@ -672,22 +754,22 @@
 containing serialised dataframe
 • name – Base name for COLDP class (name, taxon, etc.) for
 which the dataframe is requested
 • default_headings – Column headings to use if returning a
 new empty dataframe
 Returns :
 Dataframe for requested COLDP data class
+Checks for a file in the COLDP folder with a supported extension (.csv, .tsv, .txt) and a name
+matching one of the COLDP record types (name, taxon, synonym, reference, distribution,
+typematerial or speciesinteraction). If this exists, it is loaded as a Pandas dataframe.
 
 Classes
 
-22
+24
 
-Checks for a file in the COLDP folder with a supported extension (.csv, .tsv, .txt) and a name
-matching one of the COLDP record types (name, taxon, synonym, reference, distribution,
-typematerial or speciesinteraction). If this exists, it is loaded as a Pandas dataframe.
 If it is not found but the name is one of name, taxon or synonym and a file with the name
 nameusage does exist, the relevant columns will be loaded from the nameusage file.
 If no matching file is found, returns an empty dataframe.
 COLDP. extract_table ( df , headings , mappings )
 Extract a set of columns from a dataframe using a dictionary that maps source columns
 names to target column names
 Parameters :
@@ -706,29 +788,29 @@
 necessary
 Parameters :
 • name – COLDP Name record to be used as accepted name
 for new taxon
 • parentID – String identifier for parent taxon
 Returns :
 Dictionary containing taxon record
-
-Classes
-
-23
-
 If a taxon record already exists for the name, any parenthood change is made as required
 and the record is returned as a dictionary. Otherwise a new record is created and returned.
 Default values are taken from the default_taxon_record dictionary.
+
+Classes
+
+25
 COLDP. insert_synonym ( taxon_id , name_id )
 Add basic COLDP Synonym record to COLDP instance
 Parameters :
 • taxon_id – String ID for taxon for which synonym is being
 registered
 • name_id – String ID for name which is being registered as
 a synonym
+
 Ensures that a synonym record exists in the COLDP instance for the given taxon and name.
 COLDP. find_reference ( reference )
 Locate existing COLDP reference record exactly matching all major fields in reference
 Parameters :
 reference – Dictionary of COLDP reference properties
 representing a record to be found
 Returns :
@@ -741,20 +823,20 @@
 from a given parent or for all taxon records in the COLDP instance at the highest included
 rank
 Parameters :
 • taxa – Dataframe containing COLDP taxon records
 • ranks – DataFrame containing at least nameID, rank and
 scientificName for all names in COLDP instance (can be
 the complete table of COLDP names)
+• parent – Taxon record for which children should be
+updated, or None if all top-level taxa should be updated
 
 Classes
 
-24
-• parent – Taxon record for which children should be
-updated, or None if all top-level taxa should be updated
+26
 
 If taxa is None, select all top-level taxa from the dataframe (i.e. all without a parentID) and
 process these recursively.
 If a parent is supplied, copy classification properties (kingdom, phylum, subphylum, class,
 subclass, order, suborder, superfamily, family, subfamily, tribe, subtribe, genus, subgenus,
 section, species) from the parent record, set any rank-specific column matching the rank of
 the parent to the name of the parent taxon, and then copy these rank values into all taxon
@@ -780,21 +862,21 @@
 Add extra names to NameBundle if required based on current options
 Parameters :
 bundle – NameBundle to be processed
 If insert_species_for_trinomials is True, ensure that the implied binomial exists for any
 new trinomials.
 If create_subspecies_for_infrasubspecifics is True, add a subspecies-rank synonym to
 the bundle for each infrasubspecific name.
+If create_synonyms_without_subgenus is True, add a subgenus-free synonym to the bundle
+for each name containing a subgenus.
 
 Classes
 
-25
+27
 
-If create_synonyms_without_subgenus is True, add a subgenus-free synonym to the bundle
-for each name containing a subgenus.
 COLDP. validate_record ( record_type , record )
 Verify whether all ID values used as forign keys in record correspond with existing records
 in the relevant tables
 Parameters :
 • record_type – Name for the data class to which this
 record should below
 • record – Dictionary of COLDP properties for the record
@@ -834,20 +916,20 @@
 :param
 _sphinx_paramlinks_coldp.COLDP.same_basionym.b:
 Dictionary
 with
 parameters
 representing a COLDP Name record :return: True if the parenthensis-free authorship and
 lowest-ranked epithets match, False otherwise.
+COLDP. remove_gender ( epithet )
+Return epithet stripped on all likely gender-specific endings
 
 Classes
 
-26
-COLDP. remove_gender ( epithet )
-Return epithet stripped on all likely gender-specific endings
+28
 Parameters :
 epithet – String zoological epithet
 Returns :
 Epithet stripped of any possible Greek or Latin gender
 endings
 Removes “a”, “us”, “um”, “is”, “e”, “os” or “on” as an ending.
 COLDP. get_original_authorship ( authorship )
@@ -865,93 +947,64 @@
 • authorship – Authorship string
 Returns :
 True if the epithet matches the lowest-ranked epithet and
 authorship matches the authorship in the name record
 
 Comparison ignores epithet gender endings.
 COLDP. set_basionymid ( name , basionymid )
+Set basionymID on Name record in names DataFrame
 
 Classes
 
-27
-Set basionymID on Name record in names DataFrame
+29
 Parameters :
 • name – Name record as dictionary of COLDP properties
 • basionymid – String ID of associated basionyn record
 
 COLDP. fix_basionymid ( name , synonyms )
 Update name so its basionymID references the original combination in a list of synonyms
 Parameters :
 • name – Dictionary containing COLDP Name record for
 which basionymID is to be fixed
 • synonyms – List of COLDP Name records that may contain
 basionym
 Returns :
 
 Returns name following any updates.
-COLDP. find_name ( scientificName , authorship , rank )
-Return record from names DataFrame matching supplied scientificName, authorship and
-rank
-Parameters :
-• scientificName – Scientific name in canonical format
-• authorship – Authorship string
-• rank – Rank name string
-Returns :
-Dictionary containing matching record if found
-Locates any existing record in the names DataFrame that matches the supplied
-scientificName, authorship and rank and returns it as a COLDP Name properties dictionary,
-or None if no match is found.
-If authorship is None, returns a name based only on scientificName and rank.
-
-Classes
-
-28
-
-COLDP. find_taxon ( scientificName , authorship , rank )
-Get COLDP Taxon record (as Pandas dataframe) with accepted name matching supplied
-scientificName, authorship and rank values
-Parameters :
-• scientificName – Scientific name in canonical format
-• authorship – Authorship string
-• rank – Rank name string
-Returns :
-COLDP Taxon record matching supplied parameters
-Logs a warning issue if multiple taxon records exist for a matching name and returns the
-first such match. Returns None if no match.
 COLDP. construct_species_rank_name ( g , sg , s , ss , marker )
 Consistently construct a species or infraspecific name from the included epithets and
 optional rank marker
 Parameters :
 • g – Genus name
 • sg – Subgenus name
 • s – Specific epithet
 • ss – Infraspecific epithet
 • marker – Rank marker (e.g. “var.”) or rank name (“variety”)
 Returns :
 Complete scientific name string (no italics or authorship)
 Convenience method for composing a scientific name with option subgenus, infraspecific
 epithet and rank marker. A variety of markers are handled and mapped to one of “var.”,
 “subvar.”, “f.” and “ab.”.
-COLDP. construct_authorship ( a , y , is_basionym )
-Consistently construct a scientific name authorship from the included author names and
-year with parentheses where required
 
 Classes
 
-29
+30
+
+COLDP. construct_authorship ( a , y , is_basionym )
+Consistently construct a scientific name authorship from the included author names and
+year with parentheses where required
 Parameters :
 • a – Author string
 • y – Publication year as string
 • is_basionym – Boolean to indicate whether this is the
 original combination (basionym) or a subsequent
 combination that requires parentheses
 Returns :
 Tuple including 1) formatted authorship string and 2)
 publication year as a separate string
-
 Convenience method for composing an authorship string. Includes parentheses if
 is_basionym is True.
 If the year includes more than one part (e.g. “1832 [1831-1838]”), the first part (“1832”) is
 used for the year in the authorship string and the second part (“[1831-1838]”) is returned as
 the publication year. Otherwise, the same string is used in both cases.
 COLDP. is_species_group ( name )
 Check whether name is in the species group (species or lower rank)
@@ -960,20 +1013,20 @@
 Returns :
 True if the name is in the species group, False otherwise
 Simply checks if the name includes a specificEpithet value. Any name passed to this method
 should include atomic name components and not just a scientificName.
 COLDP. is_infrasubspecific ( name )
 Check whether name is in for a rank below the subspecies
 Parameters :
-name – Dictionary representing a COLDP Name record
-Returns :
 
 Classes
 
-30
+31
+name – Dictionary representing a COLDP Name record
+Returns :
 True if the name is infraspecific
 Simply checks if the supplied rank is one of those below the subspecies.
 COLDP. issue ( message )
 Log issue with data provided through methods
 Parameters :
 message – Text to be saved as body of issue
 
@@ -991,22 +1044,22 @@
 Class
 NameBundle. __init__ ( coldp , accepted , incertae_sedis = False , sic = False )
 Wrapper class to manage set of associated names, normally an accepted name and one or
 more synonyms. The bundle handles the logic of associated name variations.
 Parameters :
 • coldp – COLDP object to handle logging of any issues and
 normalise name records
+
+Classes
+
+32
 • accepted – Dictionary mapping COLDP name elements to
 values for the accepted name - a name record and a taxon
 record will be added to the COLDP package for the
 accepted name
-
-Classes
-
-31
 • incertae_sedis – Flag to indicate if the resulting taxon
 record should be marked “incertae sedis”
 • sic – Flag to indicate if the accepted name should be
 processed without reporting issues for invalid format
 
 The minimal usage is to create a new bundle with an accepted name. One or more
 synonyms can also be supplied using the add_synonym() method. The bundle is then
@@ -1043,20 +1096,20 @@
 the synonym
 • sic – Flag to indicate that the name does not follow
 expected formatting rules for a code-compliant name and
 that no issues should be logged for this
 
 NameBundle. normalise_name ( name , sic = False )
 Ensure that a name record dictionary contains all necessary/appropriate elements
-Parameters :
-• name – Dictionary containing name to be normalised
 
 Classes
 
-32
+33
+Parameters :
+• name – Dictionary containing name to be normalised
 • sic – Flag to indicate that the name does not follow
 expected formatting rules for a code-compliant name and
 that no issues should be logged for this
 Returns :
 Name dictionary updated with extra values
 
 NameBundle. derive_name ( name , values , sic = False )
@@ -1070,15 +1123,79 @@
 Name dictionary with supplied values supplemented from
 name
 
 Index and search
 • Index
 • Search Page
 
-33
+coldp.IdentifierPolicy
+Class
+IdentifierPolicy. __init__ ( existing , default_prefix , required = True , volatile = False )
+
+Classes
+
+34
+Internal class to manage ID values in COLDP dataframes.
+Parameters :
+• existing – Pandas series containing current ID values for
+table - may be empty or None
+• default_prefix – String prefix to use before numeric ID
+values if existing ID values are not consistently positive
+integer values
+• required – Flag to indicate whether the table must have ID
+values - if False, the IdentifierPolicy will return None
+unless existing already contains ID values
+• volatile – Flag to indicate if external code may modify ID
+values while the current COLDP instance is active - if False,
+the policy and future values will be determined on
+initialisation, otherwise the policy will be reviewed for
+each new ID value
+
+Checks any existing values in the series. If none are present, the next ID value will be 1. If all
+values are integer strings, the next value will be the integer string with a value one higher
+than the current maximum value. Otherwise ID values will be the concatenation of the prefix
+(defaulting to the empty string) and the current length of the ID series. Subsequent values
+will increment by one.
+If required is False and no current valus exist in the series, the policy will always return
+None.
+If volatile is True, the policy will be revised on every invocation of next. Otherwise, the
+series will only be scanned on initialisation and all policy values will then be fixed.
+
+Methods
+IdentifierPolicy. initialise ( existing )
+Internal method to set or refresh policy
+Parameters :
+existing – Pandas series containing current ID values for
+table - may be empty or None
+Returns :
+
+Classes
+
+35
+Tuple comprising the next integer value for the policy and a
+prefix for use if ID values should not be plain integer strings
+- one or both values will be None
+Provides the variables to determine the next ID value, if any
+IdentifierPolicy. next ( existing = None )
+Return next ID value for series
+Parameters :
+existing – Pandas series containing current ID values for
+table - may be empty or None - only required if volatile is
+True
+Returns :
+Next string ID value for policy or None if no ID is required
+
+Returns the next ID value for use in the Series associated with this IdentifierPolicy.
+Recalculates policy if paramref: ~coldp.IdentifierPolicy.__init__.volatile is True.
+
+Index and search
+• Index
+• Search Page
+
+36
 
 Usage
 
 Usage
 Usage
 The following example illustrates basic usage. It creates a new COLDP instance for the monotypic
 Lepidoptera family Tridentaformidae, including name and taxon records for the family, genus and
@@ -1107,15 +1224,15 @@
 }
 # Create new COLDP instance with name Tridentaformidae
 #
 # This would load an existing COLDP instance from a folder named
 # Tridentaformidae in the current folder if it already exists
 coldp = COLDP("Tridentaformidae", default_taxon_record =
 
-34
+37
 
 Usage
 
 taxon_defaults)
 # Add four COLDP Reference objects
 references = coldp.add_references([
 {
@@ -1165,15 +1282,15 @@
 morphology and life-history evolution",
 "containerTitle": "Systematic Entomology",
 "volume": "40",
 "issue": "4",
 
 Usage
 
-35
+38
 "page": "671–704",
 "link": "https://doi.org/10.1111/syen.12129",
 },
 ])
 # Add COLDP Name and Taxon records for family and get the ID string
 for the
 # family Taxon record
@@ -1219,15 +1336,15 @@
 "publishedInPage": "150",
 "publishedInYear": "1978",
 })
 bundle.add_synonym({
 
 Usage
 
-36
+39
 "rank": "species",
 "scientificName": "Lampronia fuscoleuca",
 "authorship": "Braun, 1923",
 "referenceID": "Braun_1923",
 "publishedInPage": "127",
 })
 coldp.add_names(bundle, genus_id)
```

### Comparing `coldp-2024.5.3/docs/build/simplepdf/index.html` & `coldp-2024.5.4/docs/build/simplepdf/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 <html data-content_root="./" lang="en">
  <head>
   <meta charset="utf-8"/>
   <meta content="width=device-width, initial-scale=1.0" name="viewport"/>
   <meta content="width=device-width, initial-scale=1" name="viewport"/>
   <title>
-   COLDP 2024.5.3 documentation
+   COLDP 2024.5.4 documentation
   </title>
   <link href="_static/pygments.css" rel="stylesheet" type="text/css"/>
   <link href="_static/main.css?v=0eace31b" rel="stylesheet" type="text/css"/>
   <link href="_static/sphinx_paramlinks.css" rel="stylesheet" type="text/css"/>
   <script src="_static/documentation_options.js">
   </script>
   <script src="_static/doctools.js">
@@ -111,14 +111,36 @@
         <li class="toctree-l2">
          <a class="reference internal" href="#index-and-search">
           Index and search
          </a>
         </li>
        </ul>
       </li>
+      <li class="toctree-l1">
+       <a class="reference internal" href="#coldp-identifierpolicy">
+        coldp.IdentifierPolicy
+       </a>
+       <ul>
+        <li class="toctree-l2">
+         <a class="reference internal" href="#class">
+          Class
+         </a>
+        </li>
+        <li class="toctree-l2">
+         <a class="reference internal" href="#methods">
+          Methods
+         </a>
+        </li>
+        <li class="toctree-l2">
+         <a class="reference internal" href="#index-and-search">
+          Index and search
+         </a>
+        </li>
+       </ul>
+      </li>
      </ul>
      <ul>
       <li class="toctree-l1">
        <a class="reference internal" href="#usage">
         Usage
        </a>
       </li>
@@ -151,15 +173,15 @@
          coldp is a Python package to facilitate creation, manipulation, editing and serialisation of taxonomic checklists in the
          <a class="reference external" href="https://github.com/CatalogueOfLife/coldp">
           COL Data Package (COLDP)
          </a>
          format.
         </p>
         <p>
-         The package includes two classes:
+         The package includes three classes:
         </p>
         <ul class="simple">
          <li>
           <p>
            <strong>
             coldp.COLDP
            </strong>
@@ -170,14 +192,22 @@
           <p>
            <strong>
             coldp.NameBundle
            </strong>
            - A helper class to simplify addition of taxon names with sets of associated synonyms to a COLDP instance
           </p>
          </li>
+         <li>
+          <p>
+           <strong>
+            coldp.IdentifierPolicy
+           </strong>
+           - An internal class to manage ID values in COLDP dataframes
+          </p>
+         </li>
         </ul>
         <p>
          The main
          <strong>
           COLDP
          </strong>
          class instantiates a COLDP package in memory as a set of Pandas dataframes. An instance may be initialised from the contents of a folder containing a set of COLDP-compliant CSV or tab-delimited data files or alternatively can be initialised as an empty instance in memory. The class includes many methods for inserting new data, editing existing records and querying the contents of the package. The instance can then be saved as a set of CSV files in a named folder .
@@ -708,15 +738,15 @@
                   .
                  </p>
                 </li>
                </ul>
               </dd>
              </dl>
              <p>
-              A COLDP object is initalised with a source/destination folder, COLDP package
+              A COLDP object is initialised with a source/destination folder, COLDP package
 name and other options.
              </p>
              <p>
               If a subfolder exists with the supplied name in the supplied folder, it
 will be initialised with data from any CSV/TSV files it contains with any
 of the following base names: name, taxon, synonym, reference,
 distribution, speciesinteraction, namerelation, typematerial or nameusage,
@@ -1442,15 +1472,15 @@
                  with IDs for references in this COLDP instance
                 </p>
                </dd>
               </dl>
               <p>
                Find existing ID values for each supplied reference, based on identity
 of: author, title, issued, containerTitle, volume, issue, page and citation. Add
-ID to the appropriate reference dictionary in references. If none
+ID from the appropriate reference dictionary in references. If none
 found, set ID to next unused index and add to references.
               </p>
               <p>
                The list is returned updated with current ID values so these can be used for referenceID values in other classes.
               </p>
              </dd>
             </dl>
@@ -2129,14 +2159,130 @@
             <h5>
              Find or get records
              <a class="headerlink" href="#find-or-get-records" title="Link to this heading">
               &para;
              </a>
             </h5>
             <dl class="py method">
+             <dt class="sig sig-object py" id="coldp.COLDP.find_taxon">
+              <span class="sig-prename descclassname">
+               <span class="pre">
+                COLDP.
+               </span>
+              </span>
+              <span class="sig-name descname">
+               <span class="pre">
+                find_taxon
+               </span>
+              </span>
+              <span class="sig-paren">
+               (
+              </span>
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 scientificName
+                </span>
+               </span>
+              </em>
+              ,
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 authorship
+                </span>
+               </span>
+              </em>
+              ,
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 rank
+                </span>
+               </span>
+              </em>
+              <span class="sig-paren">
+               )
+              </span>
+              <a class="headerlink" href="#coldp.COLDP.find_taxon" title="Link to this definition">
+               &para;
+              </a>
+             </dt>
+             <dd>
+              <p>
+               Get COLDP Taxon record (as Pandas dataframe) with accepted name matching supplied scientificName, authorship and rank values
+              </p>
+              <dl class="field-list simple">
+               <dt class="field-odd">
+                Parameters
+                <span class="colon">
+                 :
+                </span>
+               </dt>
+               <dd class="field-odd">
+                <ul class="simple">
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.find_taxon.params.scientificName">
+                   </span>
+                   <strong>
+                    scientificName
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.scientificName">
+                    &para;
+                   </a>
+                   &ndash; Scientific name in canonical format
+                  </p>
+                 </li>
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.find_taxon.params.authorship">
+                   </span>
+                   <strong>
+                    authorship
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.authorship">
+                    &para;
+                   </a>
+                   &ndash; Authorship string
+                  </p>
+                 </li>
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.find_taxon.params.rank">
+                   </span>
+                   <strong>
+                    rank
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.rank">
+                    &para;
+                   </a>
+                   &ndash; Rank name string
+                  </p>
+                 </li>
+                </ul>
+               </dd>
+               <dt class="field-even">
+                Returns
+                <span class="colon">
+                 :
+                </span>
+               </dt>
+               <dd class="field-even">
+                <p>
+                 COLDP Taxon record matching supplied parameters
+                </p>
+               </dd>
+              </dl>
+              <p>
+               Logs a warning issue if multiple taxon records exist for a matching name and returns the first such match. Returns None if no match.
+              </p>
+             </dd>
+            </dl>
+            <dl class="py method">
              <dt class="sig sig-object py" id="coldp.COLDP.find_name_record">
               <span class="sig-prename descclassname">
                <span class="pre">
                 COLDP.
                </span>
               </span>
               <span class="sig-name descname">
@@ -2307,14 +2453,145 @@
               </dl>
               <p>
                Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches, None is returned.
               </p>
              </dd>
             </dl>
             <dl class="py method">
+             <dt class="sig sig-object py" id="coldp.COLDP.find_name">
+              <span class="sig-prename descclassname">
+               <span class="pre">
+                COLDP.
+               </span>
+              </span>
+              <span class="sig-name descname">
+               <span class="pre">
+                find_name
+               </span>
+              </span>
+              <span class="sig-paren">
+               (
+              </span>
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 scientificName
+                </span>
+               </span>
+              </em>
+              ,
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 authorship
+                </span>
+               </span>
+              </em>
+              ,
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 rank
+                </span>
+               </span>
+              </em>
+              <span class="sig-paren">
+               )
+              </span>
+              <a class="headerlink" href="#coldp.COLDP.find_name" title="Link to this definition">
+               &para;
+              </a>
+             </dt>
+             <dd>
+              <p>
+               Return record from names DataFrame matching supplied scientificName,
+authorship and rank
+              </p>
+              <dl class="field-list simple">
+               <dt class="field-odd">
+                Parameters
+                <span class="colon">
+                 :
+                </span>
+               </dt>
+               <dd class="field-odd">
+                <ul class="simple">
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.find_name.params.scientificName">
+                   </span>
+                   <strong>
+                    scientificName
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.scientificName">
+                    &para;
+                   </a>
+                   &ndash; Scientific name in canonical format
+                  </p>
+                 </li>
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.find_name.params.authorship">
+                   </span>
+                   <strong>
+                    authorship
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.authorship">
+                    &para;
+                   </a>
+                   &ndash; Authorship string
+                  </p>
+                 </li>
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.find_name.params.rank">
+                   </span>
+                   <strong>
+                    rank
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.rank">
+                    &para;
+                   </a>
+                   &ndash; Rank name string
+                  </p>
+                 </li>
+                </ul>
+               </dd>
+               <dt class="field-even">
+                Returns
+                <span class="colon">
+                 :
+                </span>
+               </dt>
+               <dd class="field-even">
+                <p>
+                 Dictionary containing matching record if found
+                </p>
+               </dd>
+              </dl>
+              <p>
+               Locates any existing record in the names DataFrame that matches the
+supplied scientificName, authorship and rank and returns it as a
+COLDP Name properties dictionary, or None if no match is found.
+              </p>
+              <p>
+               If
+               <a class="reference internal" href="#coldp.COLDP.find_name.params.authorship" title="coldp.COLDP.find_name">
+                <code class="xref py py-paramref docutils literal notranslate">
+                 <span class="pre">
+                  authorship
+                 </span>
+                </code>
+               </a>
+               is None, returns a
+name based only on scientificName and rank.
+              </p>
+             </dd>
+            </dl>
+            <dl class="py method">
              <dt class="sig sig-object py" id="coldp.COLDP.find_distribution">
               <span class="sig-prename descclassname">
                <span class="pre">
                 COLDP.
                </span>
               </span>
               <span class="sig-name descname">
@@ -3482,14 +3759,256 @@
                The tree view shows the name, authorship and rank for the selected taxon.
 Synonyms follow, one to a row at the same indent level but preceded by a
 space and an asterisk. Then each child follows, indented two more spaces per level,
 with its own synonyms and children following.
               </p>
              </dd>
             </dl>
+            <dl class="py method">
+             <dt class="sig sig-object py" id="coldp.COLDP.get_available_column_headings">
+              <span class="sig-prename descclassname">
+               <span class="pre">
+                COLDP.
+               </span>
+              </span>
+              <span class="sig-name descname">
+               <span class="pre">
+                get_available_column_headings
+               </span>
+              </span>
+              <span class="sig-paren">
+               (
+              </span>
+              <span class="sig-paren">
+               )
+              </span>
+              <a class="headerlink" href="#coldp.COLDP.get_available_column_headings" title="Link to this definition">
+               &para;
+              </a>
+             </dt>
+             <dd>
+              <p>
+               Return dictionary mapping table names to lists of supported columns
+              </p>
+              <dl class="field-list simple">
+               <dt class="field-odd">
+                Returns
+                <span class="colon">
+                 :
+                </span>
+               </dt>
+               <dd class="field-odd">
+                <p>
+                 Dictionary containing copies of internal heading lists
+                </p>
+               </dd>
+              </dl>
+              <p>
+               Returns copies to avoid corrupting the lists used in this class
+              </p>
+             </dd>
+            </dl>
+            <dl class="py method">
+             <dt class="sig sig-object py" id="coldp.COLDP.get_identifier_policy">
+              <span class="sig-prename descclassname">
+               <span class="pre">
+                COLDP.
+               </span>
+              </span>
+              <span class="sig-name descname">
+               <span class="pre">
+                get_identifier_policy
+               </span>
+              </span>
+              <span class="sig-paren">
+               (
+              </span>
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 table_name
+                </span>
+               </span>
+              </em>
+              ,
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 default_prefix
+                </span>
+               </span>
+               <span class="o">
+                <span class="pre">
+                 =
+                </span>
+               </span>
+               <span class="default_value">
+                <span class="pre">
+                 None
+                </span>
+               </span>
+              </em>
+              ,
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 required
+                </span>
+               </span>
+               <span class="o">
+                <span class="pre">
+                 =
+                </span>
+               </span>
+               <span class="default_value">
+                <span class="pre">
+                 True
+                </span>
+               </span>
+              </em>
+              ,
+              <em class="sig-param">
+               <span class="n">
+                <span class="pre">
+                 volatile
+                </span>
+               </span>
+               <span class="o">
+                <span class="pre">
+                 =
+                </span>
+               </span>
+               <span class="default_value">
+                <span class="pre">
+                 False
+                </span>
+               </span>
+              </em>
+              <span class="sig-paren">
+               )
+              </span>
+              <a class="headerlink" href="#coldp.COLDP.get_identifier_policy" title="Link to this definition">
+               &para;
+              </a>
+             </dt>
+             <dd>
+              <p>
+               Find or create
+               <code class="xref py py-class docutils literal notranslate">
+                <span class="pre">
+                 IdentifierPolicy
+                </span>
+               </code>
+               associated with named table
+              </p>
+              <dl class="field-list simple">
+               <dt class="field-odd">
+                Parameters
+                <span class="colon">
+                 :
+                </span>
+               </dt>
+               <dd class="field-odd">
+                <ul class="simple">
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.get_identifier_policy.params.table_name">
+                   </span>
+                   <strong>
+                    table_name
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_identifier_policy.params.table_name">
+                    &para;
+                   </a>
+                   &ndash; Name of COLDP dataframe for which policy is required
+                  </p>
+                 </li>
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.get_identifier_policy.params.default_prefix">
+                   </span>
+                   <strong>
+                    default_prefix
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_identifier_policy.params.default_prefix">
+                    &para;
+                   </a>
+                   &ndash; String prefix to use before numeric ID values if existing ID values are not consistently positive integer values
+                  </p>
+                 </li>
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.get_identifier_policy.params.required">
+                   </span>
+                   <strong>
+                    required
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_identifier_policy.params.required">
+                    &para;
+                   </a>
+                   &ndash; Flag to indicate whether the table must have ID values - if False, the
+                   <code class="xref py py-class docutils literal notranslate">
+                    <span class="pre">
+                     IdentifierPolicy
+                    </span>
+                   </code>
+                   will return None unless
+                   <a class="reference internal" href="index.html#coldp.IdentifierPolicy.__init__.params.existing" title="coldp.IdentifierPolicy.__init__">
+                    <code class="xref py py-paramref docutils literal notranslate">
+                     <span class="pre">
+                      existing
+                     </span>
+                    </code>
+                   </a>
+                   already contains ID values
+                  </p>
+                 </li>
+                 <li>
+                  <p>
+                   <span class="target" id="coldp.COLDP.get_identifier_policy.params.volatile">
+                   </span>
+                   <strong>
+                    volatile
+                   </strong>
+                   <a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_identifier_policy.params.volatile">
+                    &para;
+                   </a>
+                   &ndash; Flag to indicate if external code may modify ID values while the current COLDP instance is active - if False, the policy and future values will be determined on initialisation, otherwise the policy will be reviewed for each new ID value
+                  </p>
+                 </li>
+                </ul>
+               </dd>
+               <dt class="field-even">
+                Returns
+                <span class="colon">
+                 :
+                </span>
+               </dt>
+               <dd class="field-even">
+                <p>
+                 <code class="xref py py-class docutils literal notranslate">
+                  <span class="pre">
+                   IdentifierPolicy
+                  </span>
+                 </code>
+                 object or None if no policy is required for the table
+                </p>
+               </dd>
+              </dl>
+              <p>
+               Creates new
+               <code class="xref py py-class docutils literal notranslate">
+                <span class="pre">
+                 IdentifierPolicy
+                </span>
+               </code>
+               instance if this is the first invocation for the given table. Policies take into account any existing ID values for the table.
+              </p>
+             </dd>
+            </dl>
            </section>
            <section id="access-to-dataframes">
             <h5>
              Access to DataFrames
              <a class="headerlink" href="#access-to-dataframes" title="Link to this heading">
               &para;
              </a>
@@ -5291,261 +5810,14 @@
              </dl>
              <p>
               Returns name following any updates.
              </p>
             </dd>
            </dl>
            <dl class="py method">
-            <dt class="sig sig-object py" id="coldp.COLDP.find_name">
-             <span class="sig-prename descclassname">
-              <span class="pre">
-               COLDP.
-              </span>
-             </span>
-             <span class="sig-name descname">
-              <span class="pre">
-               find_name
-              </span>
-             </span>
-             <span class="sig-paren">
-              (
-             </span>
-             <em class="sig-param">
-              <span class="n">
-               <span class="pre">
-                scientificName
-               </span>
-              </span>
-             </em>
-             ,
-             <em class="sig-param">
-              <span class="n">
-               <span class="pre">
-                authorship
-               </span>
-              </span>
-             </em>
-             ,
-             <em class="sig-param">
-              <span class="n">
-               <span class="pre">
-                rank
-               </span>
-              </span>
-             </em>
-             <span class="sig-paren">
-              )
-             </span>
-             <a class="headerlink" href="#coldp.COLDP.find_name" title="Link to this definition">
-              &para;
-             </a>
-            </dt>
-            <dd>
-             <p>
-              Return record from names DataFrame matching supplied scientificName,
-authorship and rank
-             </p>
-             <dl class="field-list simple">
-              <dt class="field-odd">
-               Parameters
-               <span class="colon">
-                :
-               </span>
-              </dt>
-              <dd class="field-odd">
-               <ul class="simple">
-                <li>
-                 <p>
-                  <span class="target" id="coldp.COLDP.find_name.params.scientificName">
-                  </span>
-                  <strong>
-                   scientificName
-                  </strong>
-                  <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.scientificName">
-                   &para;
-                  </a>
-                  &ndash; Scientific name in canonical format
-                 </p>
-                </li>
-                <li>
-                 <p>
-                  <span class="target" id="coldp.COLDP.find_name.params.authorship">
-                  </span>
-                  <strong>
-                   authorship
-                  </strong>
-                  <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.authorship">
-                   &para;
-                  </a>
-                  &ndash; Authorship string
-                 </p>
-                </li>
-                <li>
-                 <p>
-                  <span class="target" id="coldp.COLDP.find_name.params.rank">
-                  </span>
-                  <strong>
-                   rank
-                  </strong>
-                  <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.rank">
-                   &para;
-                  </a>
-                  &ndash; Rank name string
-                 </p>
-                </li>
-               </ul>
-              </dd>
-              <dt class="field-even">
-               Returns
-               <span class="colon">
-                :
-               </span>
-              </dt>
-              <dd class="field-even">
-               <p>
-                Dictionary containing matching record if found
-               </p>
-              </dd>
-             </dl>
-             <p>
-              Locates any existing record in the names DataFrame that matches the
-supplied scientificName, authorship and rank and returns it as a
-COLDP Name properties dictionary, or None if no match is found.
-             </p>
-             <p>
-              If
-              <a class="reference internal" href="#coldp.COLDP.find_name.params.authorship" title="coldp.COLDP.find_name">
-               <code class="xref py py-paramref docutils literal notranslate">
-                <span class="pre">
-                 authorship
-                </span>
-               </code>
-              </a>
-              is None, returns a
-name based only on scientificName and rank.
-             </p>
-            </dd>
-           </dl>
-           <dl class="py method">
-            <dt class="sig sig-object py" id="coldp.COLDP.find_taxon">
-             <span class="sig-prename descclassname">
-              <span class="pre">
-               COLDP.
-              </span>
-             </span>
-             <span class="sig-name descname">
-              <span class="pre">
-               find_taxon
-              </span>
-             </span>
-             <span class="sig-paren">
-              (
-             </span>
-             <em class="sig-param">
-              <span class="n">
-               <span class="pre">
-                scientificName
-               </span>
-              </span>
-             </em>
-             ,
-             <em class="sig-param">
-              <span class="n">
-               <span class="pre">
-                authorship
-               </span>
-              </span>
-             </em>
-             ,
-             <em class="sig-param">
-              <span class="n">
-               <span class="pre">
-                rank
-               </span>
-              </span>
-             </em>
-             <span class="sig-paren">
-              )
-             </span>
-             <a class="headerlink" href="#coldp.COLDP.find_taxon" title="Link to this definition">
-              &para;
-             </a>
-            </dt>
-            <dd>
-             <p>
-              Get COLDP Taxon record (as Pandas dataframe) with accepted name matching supplied scientificName, authorship and rank values
-             </p>
-             <dl class="field-list simple">
-              <dt class="field-odd">
-               Parameters
-               <span class="colon">
-                :
-               </span>
-              </dt>
-              <dd class="field-odd">
-               <ul class="simple">
-                <li>
-                 <p>
-                  <span class="target" id="coldp.COLDP.find_taxon.params.scientificName">
-                  </span>
-                  <strong>
-                   scientificName
-                  </strong>
-                  <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.scientificName">
-                   &para;
-                  </a>
-                  &ndash; Scientific name in canonical format
-                 </p>
-                </li>
-                <li>
-                 <p>
-                  <span class="target" id="coldp.COLDP.find_taxon.params.authorship">
-                  </span>
-                  <strong>
-                   authorship
-                  </strong>
-                  <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.authorship">
-                   &para;
-                  </a>
-                  &ndash; Authorship string
-                 </p>
-                </li>
-                <li>
-                 <p>
-                  <span class="target" id="coldp.COLDP.find_taxon.params.rank">
-                  </span>
-                  <strong>
-                   rank
-                  </strong>
-                  <a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.rank">
-                   &para;
-                  </a>
-                  &ndash; Rank name string
-                 </p>
-                </li>
-               </ul>
-              </dd>
-              <dt class="field-even">
-               Returns
-               <span class="colon">
-                :
-               </span>
-              </dt>
-              <dd class="field-even">
-               <p>
-                COLDP Taxon record matching supplied parameters
-               </p>
-              </dd>
-             </dl>
-             <p>
-              Logs a warning issue if multiple taxon records exist for a matching name and returns the first such match. Returns None if no match.
-             </p>
-            </dd>
-           </dl>
-           <dl class="py method">
             <dt class="sig sig-object py" id="coldp.COLDP.construct_species_rank_name">
              <span class="sig-prename descclassname">
               <span class="pre">
                COLDP.
               </span>
              </span>
              <span class="sig-name descname">
@@ -6625,14 +6897,412 @@
             </dd>
            </dl>
           </section>
           <section id="index-and-search">
            <h4>
             Index and search
             <a class="headerlink" href="#index-and-search" title="Link to this heading">
+             &para;
+            </a>
+           </h4>
+           <ul class="simple">
+            <li>
+             <p>
+              <a class="reference internal" href="genindex.html">
+               <span class="std std-ref">
+                Index
+               </span>
+              </a>
+             </p>
+            </li>
+            <li>
+             <p>
+              <a class="reference internal" href="search.html">
+               <span class="std std-ref">
+                Search Page
+               </span>
+              </a>
+             </p>
+            </li>
+           </ul>
+          </section>
+         </section>
+         <span id="document-identifier-policy">
+         </span>
+         <section id="coldp-identifierpolicy">
+          <h3>
+           coldp.IdentifierPolicy
+           <a class="headerlink" href="#coldp-identifierpolicy" title="Link to this heading">
+            &para;
+           </a>
+          </h3>
+          <section id="class">
+           <h4>
+            Class
+            <a class="headerlink" href="#class" title="Link to this heading">
+             &para;
+            </a>
+           </h4>
+           <dl class="py method">
+            <dt class="sig sig-object py" id="coldp.IdentifierPolicy.__init__">
+             <span class="sig-prename descclassname">
+              <span class="pre">
+               IdentifierPolicy.
+              </span>
+             </span>
+             <span class="sig-name descname">
+              <span class="pre">
+               __init__
+              </span>
+             </span>
+             <span class="sig-paren">
+              (
+             </span>
+             <em class="sig-param">
+              <span class="n">
+               <span class="pre">
+                existing
+               </span>
+              </span>
+             </em>
+             ,
+             <em class="sig-param">
+              <span class="n">
+               <span class="pre">
+                default_prefix
+               </span>
+              </span>
+             </em>
+             ,
+             <em class="sig-param">
+              <span class="n">
+               <span class="pre">
+                required
+               </span>
+              </span>
+              <span class="o">
+               <span class="pre">
+                =
+               </span>
+              </span>
+              <span class="default_value">
+               <span class="pre">
+                True
+               </span>
+              </span>
+             </em>
+             ,
+             <em class="sig-param">
+              <span class="n">
+               <span class="pre">
+                volatile
+               </span>
+              </span>
+              <span class="o">
+               <span class="pre">
+                =
+               </span>
+              </span>
+              <span class="default_value">
+               <span class="pre">
+                False
+               </span>
+              </span>
+             </em>
+             <span class="sig-paren">
+              )
+             </span>
+             <a class="headerlink" href="#coldp.IdentifierPolicy.__init__" title="Link to this definition">
+              &para;
+             </a>
+            </dt>
+            <dd>
+             <p>
+              Internal class to manage ID values in COLDP dataframes.
+             </p>
+             <dl class="field-list simple">
+              <dt class="field-odd">
+               Parameters
+               <span class="colon">
+                :
+               </span>
+              </dt>
+              <dd class="field-odd">
+               <ul class="simple">
+                <li>
+                 <p>
+                  <span class="target" id="coldp.IdentifierPolicy.params.existing">
+                  </span>
+                  <strong>
+                   existing
+                  </strong>
+                  <a class="paramlink headerlink reference internal" href="#coldp.IdentifierPolicy.params.existing">
+                   &para;
+                  </a>
+                  &ndash; Pandas series containing current ID values for table - may be empty or None
+                 </p>
+                </li>
+                <li>
+                 <p>
+                  <span class="target" id="coldp.IdentifierPolicy.params.default_prefix">
+                  </span>
+                  <strong>
+                   default_prefix
+                  </strong>
+                  <a class="paramlink headerlink reference internal" href="#coldp.IdentifierPolicy.params.default_prefix">
+                   &para;
+                  </a>
+                  &ndash; String prefix to use before numeric ID values if existing ID values are not consistently positive integer values
+                 </p>
+                </li>
+                <li>
+                 <p>
+                  <span class="target" id="coldp.IdentifierPolicy.params.required">
+                  </span>
+                  <strong>
+                   required
+                  </strong>
+                  <a class="paramlink headerlink reference internal" href="#coldp.IdentifierPolicy.params.required">
+                   &para;
+                  </a>
+                  &ndash; Flag to indicate whether the table must have ID values - if False, the
+                  <code class="xref py py-class docutils literal notranslate">
+                   <span class="pre">
+                    IdentifierPolicy
+                   </span>
+                  </code>
+                  will return None unless
+                  <a class="reference internal" href="#coldp.IdentifierPolicy.__init__.params.existing" title="coldp.IdentifierPolicy.__init__">
+                   <code class="xref py py-paramref docutils literal notranslate">
+                    <span class="pre">
+                     existing
+                    </span>
+                   </code>
+                  </a>
+                  already contains ID values
+                 </p>
+                </li>
+                <li>
+                 <p>
+                  <span class="target" id="coldp.IdentifierPolicy.params.volatile">
+                  </span>
+                  <strong>
+                   volatile
+                  </strong>
+                  <a class="paramlink headerlink reference internal" href="#coldp.IdentifierPolicy.params.volatile">
+                   &para;
+                  </a>
+                  &ndash; Flag to indicate if external code may modify ID values while the current COLDP instance is active - if False, the policy and future values will be determined on initialisation, otherwise the policy will be reviewed for each new ID value
+                 </p>
+                </li>
+               </ul>
+              </dd>
+             </dl>
+             <p>
+              Checks any existing values in the series. If none are present, the next ID value will be 1. If all values are integer strings, the next value will be the integer string with a value one higher than the current maximum value. Otherwise ID values will be the concatenation of the prefix (defaulting to the empty string) and the current length of the ID series. Subsequent values will increment by one.
+             </p>
+             <p>
+              If
+              <a class="reference internal" href="#coldp.IdentifierPolicy.__init__.params.required" title="coldp.IdentifierPolicy.__init__">
+               <code class="xref py py-paramref docutils literal notranslate">
+                <span class="pre">
+                 required
+                </span>
+               </code>
+              </a>
+              is False and no current valus exist in the series, the policy will always return None.
+             </p>
+             <p>
+              If
+              <a class="reference internal" href="#coldp.IdentifierPolicy.__init__.params.volatile" title="coldp.IdentifierPolicy.__init__">
+               <code class="xref py py-paramref docutils literal notranslate">
+                <span class="pre">
+                 volatile
+                </span>
+               </code>
+              </a>
+              is True, the policy will be revised on every invocation of next. Otherwise, the series will only be scanned on initialisation and all policy values will then be fixed.
+             </p>
+            </dd>
+           </dl>
+          </section>
+          <section id="methods">
+           <h4>
+            Methods
+            <a class="headerlink" href="#methods" title="Link to this heading">
+             &para;
+            </a>
+           </h4>
+           <dl class="py method">
+            <dt class="sig sig-object py" id="coldp.IdentifierPolicy.initialise">
+             <span class="sig-prename descclassname">
+              <span class="pre">
+               IdentifierPolicy.
+              </span>
+             </span>
+             <span class="sig-name descname">
+              <span class="pre">
+               initialise
+              </span>
+             </span>
+             <span class="sig-paren">
+              (
+             </span>
+             <em class="sig-param">
+              <span class="n">
+               <span class="pre">
+                existing
+               </span>
+              </span>
+             </em>
+             <span class="sig-paren">
+              )
+             </span>
+             <a class="headerlink" href="#coldp.IdentifierPolicy.initialise" title="Link to this definition">
+              &para;
+             </a>
+            </dt>
+            <dd>
+             <p>
+              Internal method to set or refresh policy
+             </p>
+             <dl class="field-list simple">
+              <dt class="field-odd">
+               Parameters
+               <span class="colon">
+                :
+               </span>
+              </dt>
+              <dd class="field-odd">
+               <p>
+                <span class="target" id="coldp.IdentifierPolicy.initialise.params.existing">
+                </span>
+                <strong>
+                 existing
+                </strong>
+                <a class="paramlink headerlink reference internal" href="#coldp.IdentifierPolicy.initialise.params.existing">
+                 &para;
+                </a>
+                &ndash; Pandas series containing current ID values for table - may be empty or None
+               </p>
+              </dd>
+              <dt class="field-even">
+               Returns
+               <span class="colon">
+                :
+               </span>
+              </dt>
+              <dd class="field-even">
+               <p>
+                Tuple comprising the next integer value for the policy and a prefix for use if ID values should not be plain integer strings - one or both values will be None
+               </p>
+              </dd>
+             </dl>
+             <p>
+              Provides the variables to determine the next ID value, if any
+             </p>
+            </dd>
+           </dl>
+           <dl class="py method">
+            <dt class="sig sig-object py" id="coldp.IdentifierPolicy.next">
+             <span class="sig-prename descclassname">
+              <span class="pre">
+               IdentifierPolicy.
+              </span>
+             </span>
+             <span class="sig-name descname">
+              <span class="pre">
+               next
+              </span>
+             </span>
+             <span class="sig-paren">
+              (
+             </span>
+             <em class="sig-param">
+              <span class="n">
+               <span class="pre">
+                existing
+               </span>
+              </span>
+              <span class="o">
+               <span class="pre">
+                =
+               </span>
+              </span>
+              <span class="default_value">
+               <span class="pre">
+                None
+               </span>
+              </span>
+             </em>
+             <span class="sig-paren">
+              )
+             </span>
+             <a class="headerlink" href="#coldp.IdentifierPolicy.next" title="Link to this definition">
+              &para;
+             </a>
+            </dt>
+            <dd>
+             <p>
+              Return next ID value for series
+             </p>
+             <dl class="field-list simple">
+              <dt class="field-odd">
+               Parameters
+               <span class="colon">
+                :
+               </span>
+              </dt>
+              <dd class="field-odd">
+               <p>
+                <span class="target" id="coldp.IdentifierPolicy.next.params.existing">
+                </span>
+                <strong>
+                 existing
+                </strong>
+                <a class="paramlink headerlink reference internal" href="#coldp.IdentifierPolicy.next.params.existing">
+                 &para;
+                </a>
+                &ndash; Pandas series containing current ID values for table - may be empty or None - only required if
+                <a class="reference internal" href="#coldp.IdentifierPolicy.__init__.params.volatile" title="coldp.IdentifierPolicy.__init__">
+                 <code class="xref py py-paramref docutils literal notranslate">
+                  <span class="pre">
+                   volatile
+                  </span>
+                 </code>
+                </a>
+                is True
+               </p>
+              </dd>
+              <dt class="field-even">
+               Returns
+               <span class="colon">
+                :
+               </span>
+              </dt>
+              <dd class="field-even">
+               <p>
+                Next string ID value for policy or None if no ID is required
+               </p>
+              </dd>
+             </dl>
+             <p>
+              Returns the next ID value for use in the Series associated with this IdentifierPolicy. Recalculates policy if paramref:
+              <cite>
+               ~coldp.IdentifierPolicy.__init__.volatile
+              </cite>
+              is True.
+             </p>
+            </dd>
+           </dl>
+          </section>
+          <section id="index-and-search">
+           <h4>
+            Index and search
+            <a class="headerlink" href="#index-and-search" title="Link to this heading">
              &para;
             </a>
            </h4>
            <ul class="simple">
             <li>
              <p>
               <a class="reference internal" href="genindex.html">
```

#### html2text {}

```diff
@@ -7,25 +7,31 @@
           o _C_o_n_s_t_a_n_t_s
           o _I_n_t_e_r_n_a_l_ _m_e_t_h_o_d_s
           o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
           o _C_l_a_s_s
           o _M_e_t_h_o_d_s
           o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
+    * _c_o_l_d_p_._I_d_e_n_t_i_f_i_e_r_P_o_l_i_c_y
+          o _C_l_a_s_s
+          o _M_e_t_h_o_d_s
+          o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
     * _U_s_a_g_e
 ************ ccoollddpp _?¶ ************
 Python tools for working with taxonomic checklists organised as Catalogue of
 Life Data Package (COLDP) format
 ********** OOvveerrvviieeww _?¶ **********
 coldp is a Python package to facilitate creation, manipulation, editing and
 serialisation of taxonomic checklists in the _C_O_L_ _D_a_t_a_ _P_a_c_k_a_g_e_ _(_C_O_L_D_P_)_ format.
-The package includes two classes:
+The package includes three classes:
     * ccoollddpp..CCOOLLDDPP - A COLDP package loaded as a set of Pandas dataframes
     * ccoollddpp..NNaammeeBBuunnddllee - A helper class to simplify addition of taxon names
       with sets of associated synonyms to a COLDP instance
+    * ccoollddpp..IIddeennttiiffiieerrPPoolliiccyy - An internal class to manage ID values in COLDP
+      dataframes
 The main CCOOLLDDPP class instantiates a COLDP package in memory as a set of Pandas
 dataframes. An instance may be initialised from the contents of a folder
 containing a set of COLDP-compliant CSV or tab-delimited data files or
 alternatively can be initialised as an empty instance in memory. The class
 includes many methods for inserting new data, editing existing records and
 querying the contents of the package. The instance can then be saved as a set
 of CSV files in a named folder .
@@ -122,15 +128,15 @@
                   code)
                 * iissssuueess__ttoo__ssttddoouutt _¶_ – If true, print any issue messages (see
                   _i_s_s_u_e_(_)_ ) to stdout as well as inserting then in the issue
                   dataframe.
                 * ccoonntteexxtt _¶_ – Value to be used in labeling issue records (see
                   _i_s_s_u_e_(_)_ ). This value is more normally set using _s_e_t___c_o_n_t_e_x_t
                   _(_)_ .
-      A COLDP object is initalised with a source/destination folder, COLDP
+      A COLDP object is initialised with a source/destination folder, COLDP
       package name and other options.
       If a subfolder exists with the supplied name in the supplied folder, it
       will be initialised with data from any CSV/TSV files it contains with any
       of the following base names: name, taxon, synonym, reference,
       distribution, speciesinteraction, namerelation, typematerial or
       nameusage, and with a file extension recognised via csv_extensions . File
       names are case insensitive.
@@ -239,15 +245,15 @@
             rreeffeerreennccee__lliisstt _¶_ – List of dictionaries - each dictionary contains
             values keyed by terms from reference_headings
         Returns :
             Updated _r_e_f_e_r_e_n_c_e___l_i_s_t_ with IDs for references in this COLDP
             instance
       Find existing ID values for each supplied reference, based on identity
       of: author, title, issued, containerTitle, volume, issue, page and
-      citation. Add ID to the appropriate reference dictionary in references.
+      citation. Add ID from the appropriate reference dictionary in references.
       If none found, set ID to next unused index and add to references.
       The list is returned updated with current ID values so these can be used
       for referenceID values in other classes.
   COLDP. add_type_material ( ttyyppee__mmaatteerriiaall ) _¶
       Add COLDP TypeMaterial record to COLDP instance
         Parameters :
             ttyyppee__mmaatteerriiaall _¶_ – COLDP TypeMaterial record represented as
@@ -326,14 +332,25 @@
                   name supplied to constructor, which defaults to None. If no
                   name provided, save will fail.
       If necessary creates subfolder with name _n_a_m_e_ in _d_e_s_t_i_n_a_t_i_o_n_ , and then
       writes CSV file representations for all DataFrames in the folder. Empty
       columns are dropped. Any numpy NAN elements are replaced with an empty
       string.
 **** FFiinndd oorr ggeett rreeccoorrddss _?¶ ****
+  COLDP. find_taxon ( sscciieennttiiffiiccNNaammee , aauutthhoorrsshhiipp , rraannkk ) _¶
+      Get COLDP Taxon record (as Pandas dataframe) with accepted name matching
+      supplied scientificName, authorship and rank values
+        Parameters :
+                * sscciieennttiiffiiccNNaammee _¶_ – Scientific name in canonical format
+                * aauutthhoorrsshhiipp _¶_ – Authorship string
+                * rraannkk _¶_ – Rank name string
+        Returns :
+            COLDP Taxon record matching supplied parameters
+      Logs a warning issue if multiple taxon records exist for a matching name
+      and returns the first such match. Returns None if no match.
   COLDP. find_name_record ( nnaammee ) _¶
       Return record from names DataFrame matching key fields (scientificName,
       authorship and rank) in supplied record
         Parameters :
             nnaammee _¶_ – Dictionary containing Name properties
         Returns :
             Dictionary containing matching record if found
@@ -348,14 +365,28 @@
                 * ttoo__ddiicctt _¶_ – True if records should be converted from Pandas
                   format to dictionary records, False (default) otherwise.
         Returns :
             Set of COLDP Name records either as DataFrame or list of
             dictionaries
       Returns all matching records as Pandas DataFrame or list of dictionaries.
       If no matches, None is returned.
+  COLDP. find_name ( sscciieennttiiffiiccNNaammee , aauutthhoorrsshhiipp , rraannkk ) _¶
+      Return record from names DataFrame matching supplied scientificName,
+      authorship and rank
+        Parameters :
+                * sscciieennttiiffiiccNNaammee _¶_ – Scientific name in canonical format
+                * aauutthhoorrsshhiipp _¶_ – Authorship string
+                * rraannkk _¶_ – Rank name string
+        Returns :
+            Dictionary containing matching record if found
+      Locates any existing record in the names DataFrame that matches the
+      supplied scientificName, authorship and rank and returns it as a COLDP
+      Name properties dictionary, or None if no match is found.
+      If _a_u_t_h_o_r_s_h_i_p_ is None, returns a name based only on scientificName and
+      rank.
   COLDP. find_distribution ( ddiissttrriibbuuttiioonn ) _¶
       Locate existing COLDP distribution record exactly matching all major
       fields in _d_i_s_t_r_i_b_u_t_i_o_n
         Parameters :
             ddiissttrriibbuuttiioonn _¶_ – Dictionary of COLDP distribution properties
             representing a record to be found
         Returns :
@@ -492,14 +523,42 @@
                   defaults to an equal sign with spaces on either side
         Returns :
             Multiline string representation of taxonomic hierarchy
       The tree view shows the name, authorship and rank for the selected taxon.
       Synonyms follow, one to a row at the same indent level but preceded by a
       space and an asterisk. Then each child follows, indented two more spaces
       per level, with its own synonyms and children following.
+  COLDP. get_available_column_headings ( ) _¶
+      Return dictionary mapping table names to lists of supported columns
+        Returns :
+            Dictionary containing copies of internal heading lists
+      Returns copies to avoid corrupting the lists used in this class
+  COLDP. get_identifier_policy ( ttaabbllee__nnaammee , ddeeffaauulltt__pprreeffiixx == NNoonnee , rreeqquuiirreedd
+  == TTrruuee , vvoollaattiillee == FFaallssee ) _¶
+      Find or create IdentifierPolicy associated with named table
+        Parameters :
+                * ttaabbllee__nnaammee _¶_ – Name of COLDP dataframe for which policy is
+                  required
+                * ddeeffaauulltt__pprreeffiixx _¶_ – String prefix to use before numeric ID
+                  values if existing ID values are not consistently positive
+                  integer values
+                * rreeqquuiirreedd _¶_ – Flag to indicate whether the table must have ID
+                  values - if False, the IdentifierPolicy will return None
+                  unless _e_x_i_s_t_i_n_g_ already contains ID values
+                * vvoollaattiillee _¶_ – Flag to indicate if external code may modify ID
+                  values while the current COLDP instance is active - if False,
+                  the policy and future values will be determined on
+                  initialisation, otherwise the policy will be reviewed for
+                  each new ID value
+        Returns :
+            IdentifierPolicy object or None if no policy is required for the
+            table
+      Creates new IdentifierPolicy instance if this is the first invocation for
+      the given table. Policies take into account any existing ID values for
+      the table.
 **** AAcccceessss ttoo DDaattaaFFrraammeess _?¶ ****
   COLDP. table_by_name ( nnaammee ) _¶
       Return dataframe for named COLDP data class
         Parameters :
             nnaammee _¶_ – Name of data frame to return (one of: name, taxon,
             synonym, reference, type_material, distribution,
             species_interaction, name_relation)
@@ -707,39 +766,14 @@
         Parameters :
                 * nnaammee _¶_ – Dictionary containing COLDP Name record for which
                   basionymID is to be fixed
                 * ssyynnoonnyymmss _¶_ – List of COLDP Name records that may contain
                   basionym
         Returns :
       Returns name following any updates.
-  COLDP. find_name ( sscciieennttiiffiiccNNaammee , aauutthhoorrsshhiipp , rraannkk ) _¶
-      Return record from names DataFrame matching supplied scientificName,
-      authorship and rank
-        Parameters :
-                * sscciieennttiiffiiccNNaammee _¶_ – Scientific name in canonical format
-                * aauutthhoorrsshhiipp _¶_ – Authorship string
-                * rraannkk _¶_ – Rank name string
-        Returns :
-            Dictionary containing matching record if found
-      Locates any existing record in the names DataFrame that matches the
-      supplied scientificName, authorship and rank and returns it as a COLDP
-      Name properties dictionary, or None if no match is found.
-      If _a_u_t_h_o_r_s_h_i_p_ is None, returns a name based only on scientificName and
-      rank.
-  COLDP. find_taxon ( sscciieennttiiffiiccNNaammee , aauutthhoorrsshhiipp , rraannkk ) _¶
-      Get COLDP Taxon record (as Pandas dataframe) with accepted name matching
-      supplied scientificName, authorship and rank values
-        Parameters :
-                * sscciieennttiiffiiccNNaammee _¶_ – Scientific name in canonical format
-                * aauutthhoorrsshhiipp _¶_ – Authorship string
-                * rraannkk _¶_ – Rank name string
-        Returns :
-            COLDP Taxon record matching supplied parameters
-      Logs a warning issue if multiple taxon records exist for a matching name
-      and returns the first such match. Returns None if no match.
   COLDP. construct_species_rank_name ( gg , ssgg , ss , ssss , mmaarrkkeerr ) _¶
       Consistently construct a species or infraspecific name from the included
       epithets and optional rank marker
         Parameters :
                 * gg _¶_ – Genus name
                 * ssgg _¶_ – Subgenus name
                 * ss _¶_ – Specific epithet
@@ -851,14 +885,68 @@
                   be based
                 * vvaalluueess _¶_ – Dictionary of values to override values in name
         Returns :
             Name dictionary with supplied values supplemented from name
 ****** IInnddeexx aanndd sseeaarrcchh _?¶ ******
     * _I_n_d_e_x
     * _S_e_a_r_c_h_ _P_a_g_e
+******** ccoollddpp..IIddeennttiiffiieerrPPoolliiccyy _?¶ ********
+****** CCllaassss _?¶ ******
+  IdentifierPolicy. __init__ ( eexxiissttiinngg , ddeeffaauulltt__pprreeffiixx , rreeqquuiirreedd == TTrruuee ,
+  vvoollaattiillee == FFaallssee ) _¶
+      Internal class to manage ID values in COLDP dataframes.
+        Parameters :
+                * eexxiissttiinngg _¶_ – Pandas series containing current ID values for
+                  table - may be empty or None
+                * ddeeffaauulltt__pprreeffiixx _¶_ – String prefix to use before numeric ID
+                  values if existing ID values are not consistently positive
+                  integer values
+                * rreeqquuiirreedd _¶_ – Flag to indicate whether the table must have ID
+                  values - if False, the IdentifierPolicy will return None
+                  unless _e_x_i_s_t_i_n_g_ already contains ID values
+                * vvoollaattiillee _¶_ – Flag to indicate if external code may modify ID
+                  values while the current COLDP instance is active - if False,
+                  the policy and future values will be determined on
+                  initialisation, otherwise the policy will be reviewed for
+                  each new ID value
+      Checks any existing values in the series. If none are present, the next
+      ID value will be 1. If all values are integer strings, the next value
+      will be the integer string with a value one higher than the current
+      maximum value. Otherwise ID values will be the concatenation of the
+      prefix (defaulting to the empty string) and the current length of the ID
+      series. Subsequent values will increment by one.
+      If _r_e_q_u_i_r_e_d_ is False and no current valus exist in the series, the policy
+      will always return None.
+      If _v_o_l_a_t_i_l_e_ is True, the policy will be revised on every invocation of
+      next. Otherwise, the series will only be scanned on initialisation and
+      all policy values will then be fixed.
+****** MMeetthhooddss _?¶ ******
+  IdentifierPolicy. initialise ( eexxiissttiinngg ) _¶
+      Internal method to set or refresh policy
+        Parameters :
+            eexxiissttiinngg _¶_ – Pandas series containing current ID values for table -
+            may be empty or None
+        Returns :
+            Tuple comprising the next integer value for the policy and a prefix
+            for use if ID values should not be plain integer strings - one or
+            both values will be None
+      Provides the variables to determine the next ID value, if any
+  IdentifierPolicy. next ( eexxiissttiinngg == NNoonnee ) _¶
+      Return next ID value for series
+        Parameters :
+            eexxiissttiinngg _¶_ – Pandas series containing current ID values for table -
+            may be empty or None - only required if _v_o_l_a_t_i_l_e_ is True
+        Returns :
+            Next string ID value for policy or None if no ID is required
+      Returns the next ID value for use in the Series associated with this
+      IdentifierPolicy. Recalculates policy if paramref:
+      ~coldp.IdentifierPolicy.__init__.volatileis True.
+****** IInnddeexx aanndd sseeaarrcchh _?¶ ******
+    * _I_n_d_e_x
+    * _S_e_a_r_c_h_ _P_a_g_e
 ********** UUssaaggee _?¶ **********
 ******** UUssaaggee _?¶ ********
 The following example illustrates basic usage. It creates a new COLDP instance
 for the monotypic Lepidoptera family Tridentaformidae, including name and taxon
 records for the family, genus and species, the original combination for the
 species, three distribution records for the species, and references for all
 elements.
```

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/basic.css` & `coldp-2024.5.4/docs/build/simplepdf/_static/basic.css`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/doctools.js` & `coldp-2024.5.4/docs/build/simplepdf/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/language_data.js` & `coldp-2024.5.4/docs/build/simplepdf/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/main.css` & `coldp-2024.5.4/docs/build/simplepdf/_static/main.css`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/pygments.css` & `coldp-2024.5.4/docs/build/simplepdf/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/searchtools.js` & `coldp-2024.5.4/docs/build/simplepdf/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/sphinx_highlight.js` & `coldp-2024.5.4/docs/build/simplepdf/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraMono-Bold.ttf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraMono-Medium.ttf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraMono-Regular.ttf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Bold.otf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-Bold.otf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Italic.otf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-Italic.otf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Light.otf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-Light.otf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-LightItalic.otf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Regular.otf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/FiraSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/WorkSans-Bold.ttf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/WorkSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/WorkSans-Regular.ttf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/WorkSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/WorkSans-SemiBold.ttf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/WorkSans-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.eot` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.svg` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.ttf` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.woff` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.woff2` & `coldp-2024.5.4/docs/build/simplepdf/_static/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_admonition.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_admonition.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_alerts.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_alerts.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_api.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_api.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_back-cover.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_back-cover.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_code.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_code.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_cover.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_cover.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_fonts.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_fonts.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_lists.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_lists.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_pages.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_pages.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_tables.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_tables.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_text.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_text.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_toc.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_toc.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_variables.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/_variables.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/main.scss` & `coldp-2024.5.4/docs/build/simplepdf/_static/styles/sources/main.scss`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/source/coldp.rst` & `coldp-2024.5.4/docs/source/coldp.rst`

 * *Files 8% similar despite different names*

```diff
@@ -33,16 +33,18 @@
 
 Save
 ^^^^
 .. automethod:: coldp.COLDP.save
 
 Find or get records
 ^^^^^^^^^^^^^^^^^^^
+.. automethod:: coldp.COLDP.find_taxon
 .. automethod:: coldp.COLDP.find_name_record
 .. automethod:: coldp.COLDP.find_names
+.. automethod:: coldp.COLDP.find_name
 .. automethod:: coldp.COLDP.find_distribution
 .. automethod:: coldp.COLDP.get_name
 .. automethod:: coldp.COLDP.get_reference
 .. automethod:: coldp.COLDP.get_taxon
 .. automethod:: coldp.COLDP.get_synonyms
 .. automethod:: coldp.COLDP.get_synonymy
 .. automethod:: coldp.COLDP.get_children
@@ -54,14 +56,16 @@
 .. automethod:: coldp.COLDP.sort_taxa
 .. automethod:: coldp.COLDP.sort_names
 .. automethod:: coldp.COLDP.reset_ids
 
 Utilities
 ^^^^^^^^^
 .. automethod:: coldp.COLDP.get_text_tree
+.. automethod:: coldp.COLDP.get_available_column_headings
+.. automethod:: coldp.COLDP.get_identifier_policy
 
 Access to DataFrames
 ^^^^^^^^^^^^^^^^^^^^
 .. automethod:: coldp.COLDP.table_by_name
 
 Constants
 ~~~~~~~~~
@@ -97,16 +101,14 @@
 .. automethod:: coldp.COLDP.identify_name
 .. automethod:: coldp.COLDP.same_basionym
 .. automethod:: coldp.COLDP.remove_gender
 .. automethod:: coldp.COLDP.get_original_authorship
 .. automethod:: coldp.COLDP.epithet_and_authorship_match
 .. automethod:: coldp.COLDP.set_basionymid
 .. automethod:: coldp.COLDP.fix_basionymid
-.. automethod:: coldp.COLDP.find_name
-.. automethod:: coldp.COLDP.find_taxon
 .. automethod:: coldp.COLDP.construct_species_rank_name
 .. automethod:: coldp.COLDP.construct_authorship
 .. automethod:: coldp.COLDP.is_species_group
 .. automethod:: coldp.COLDP.is_infrasubspecific
 .. automethod:: coldp.COLDP.issue
```

### Comparing `coldp-2024.5.3/docs/source/conf.py` & `coldp-2024.5.4/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import sys
 
 sys.path.insert(0, os.path.abspath("../../src/coldp"))
 
 project = "COLDP"
 copyright = "2024, Donald Hobern"
 author = "Donald Hobern"
-release = "2024.5.3"
+release = "2024.5.4"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.doctest",
```

### Comparing `coldp-2024.5.3/docs/source/index.pdf` & `coldp-2024.5.4/docs/source/index.pdf`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/docs/source/index.rst` & `coldp-2024.5.4/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 =====
 Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format
 
 Overview
 --------
 coldp is a Python package to facilitate creation, manipulation, editing and serialisation of taxonomic checklists in the `COL Data Package (COLDP) <https://github.com/CatalogueOfLife/coldp>`_ format.
 
-The package includes two classes:
+The package includes three classes:
 
 * **coldp.COLDP** - A COLDP package loaded as a set of Pandas dataframes
 * **coldp.NameBundle** - A helper class to simplify addition of taxon names with sets of associated synonyms to a COLDP instance
+* **coldp.IdentifierPolicy** - An internal class to manage ID values in COLDP dataframes
 
 The main **COLDP** class instantiates a COLDP package in memory as a set of Pandas dataframes. An instance may be initialised from the contents of a folder containing a set of COLDP-compliant CSV or tab-delimited data files or alternatively can be initialised as an empty instance in memory. The class includes many methods for inserting new data, editing existing records and querying the contents of the package. The instance can then be saved as a set of CSV files in a named folder .
 
 The **NameBundle** class brings together a scientific name and its synonyms so that these can be added together and the COLDP package can automatically manage their relationships NameBundle objects are normally created using the :py:func:`coldp.COLDP.start_name_bundle` method. 
 
 At minimum a NameBundle is initialised with a dictionary holding a set of COLDP name record values. The scientific name represented by this dictionary should be the accepted name for a species or other taxon. Synonyms may then be added to the NameBundle. 
 
@@ -34,14 +35,15 @@
 Classes
 -------
 .. toctree::
    :maxdepth: 2
 
    coldp
    name-bundle
+   identifier-policy
 
 Usage
 -----
 .. toctree::
    :maxdepth: 2
 
    usage
```

### Comparing `coldp-2024.5.3/docs/source/usage.rst` & `coldp-2024.5.4/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/src/coldp/coldp.py` & `coldp-2024.5.4/src/coldp/coldp.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,34 @@
 Catalogue of Life for organising taxonomic checklist datasets. 
 
 See: `COL Data Package (ColDP) Specification <https://github.com/CatalogueOfLife/coldp>`_
 """
 # ---------------------------------------------------------------------------
 # Imports
 # ---------------------------------------------------------------------------
+from collections import abc
 import pandas as pd
 import numpy as np
 import logging
 import os
 import re
 import shutil
 
+
+# ---------------------------------------------------------------------------
+# Class pre-declarations
+# ---------------------------------------------------------------------------
+class NameBundle:
+    pass
+
+
+class IdentifierPolicy:
+    pass
+
+
 # ---------------------------------------------------------------------------
 # Column headings for each data class within COLDP packages
 # ---------------------------------------------------------------------------
 nameusage_headings = [
     "ID",
     "sourceID",
     "parentID",
@@ -218,15 +231,15 @@
     "sex",
     "remarks",
 ]
 
 name_relation_headings = ["nameID", "relatedNameID", "type", "referenceID", "remarks"]
 
 distribution_headings = [
-    "taxonId",
+    "taxonID",
     "area",
     "gazetteer",
     "status",
     "referenceID",
     "remarks",
 ]
 
@@ -375,198 +388,14 @@
 epithet_pattern = re.compile("^[a-z]-?[a-z]+$")
 name_pattern = re.compile("^[A-Za-z]-?[a-z]+$")
 scientific_name_pattern = re.compile(
     r"^([A-Z][a-z]+)( ([A-Z][a-z]+))?( ([a-z]-?[a-z]+))?( [abfrpsuv]+\.)?( ([a-z]-?[a-z]+))?$"
 )
 
 
-class NameBundle:
-    def __init__(
-        self,
-        coldp,
-        accepted: dict[str:str],
-        incertae_sedis: bool = False,
-        sic: bool = False,
-    ) -> None:
-        """
-        Wrapper class to manage set of associated names, normally an accepted name
-        and one or more synonyms. The bundle handles the logic of associated name
-        variations.
-
-        :param coldp: :py:class:`~coldp.COLDP` object to handle logging of any issues and normalise name records
-        :param accepted: Dictionary mapping COLDP name elements to values for the accepted name - a name record and a taxon record will be added to the COLDP package for the accepted name
-        :param incertae_sedis: Flag to indicate if the resulting taxon record should be marked "incertae sedis"
-        :param sic: Flag to indicate if the accepted name should be processed without reporting issues for invalid format
-
-        The minimal usage is to create a new bundle with an accepted name. One
-        or more synonyms can also be supplied using the :py:func:`~coldp.NameBundle.add_synonym` method.
-        The bundle is then submitted to the :py:func:`coldp.COLDP.add_names` method for
-        processing.
-
-        NameBundle objects should not be created directly. Use the :py:func:`coldp.COLDP.start_name_bundle` method instead.
-
-        accepted should contain a dictionary with keys that match property names from the `COLDP Name class <https://github.com/CatalogueOfLife/coldp?tab=readme-ov-file#name>`_
-        """
-
-        self.coldp = coldp
-        if "rank" not in accepted:
-            self.coldp.issue(
-                "Accepted name missing rank, assume species: " + str(accepted)
-            )
-            accepted["rank"] = "species"
-        self.accepted_sic = sic
-        self.accepted = self.normalise_name(accepted.copy(), sic)
-        self.incertae_sedis = incertae_sedis
-        self.accepted_taxon_id = None
-        self.synonyms = []
-        self.species = None
-        self.species_synonym = None
-        self.accepted_species_id = None
-
-    def add_synonym(self, synonym: dict[str:str], sic: bool = False) -> None:
-        """
-        Register an additional name as a synonym for the accepted name
-
-        synonym should contain a dictionary with keys that match property names from the `COLDP Name class <https://github.com/CatalogueOfLife/coldp?tab=readme-ov-file#name>`_
-
-        :param synonym: Dictionary mapping COLDP name elements to values for the synonymous name - a name record and a synonym record will be added to the COLDP package for the synonym
-        :param sic: Flag to indicate that the name does not follow expected formatting rules for a code-compliant name and that no issues should be logged for this
-
-        """
-
-        normalised = self.normalise_name(synonym, sic)
-        present = normalised["scientificName"] == self.accepted["scientificName"]
-        if not present:
-            for s in self.synonyms:
-                if normalised["scientificName"] == s["scientificName"]:
-                    if (
-                        normalised["authorship"] is None
-                        or s["authorship"] is None
-                        or normalised["authorship"] == s["authorship"]
-                    ):
-                        present = True
-                        break
-        if not present:
-            self.synonyms.append(normalised)
-
-    def normalise_name(self, name: dict[str:str], sic: bool = False) -> dict:
-        """
-        Ensure that a name record dictionary contains all necessary/appropriate elements
-
-        :param name: Dictionary containing name to be normalised
-        :param sic: Flag to indicate that the name does not follow expected formatting rules for a code-compliant name and that no issues should be logged for this
-        :return: Name dictionary updated with extra values
-        """
-
-        # Ensure main elements are present in dictionary
-        for k in required_properties["name"]:
-            if k not in name:
-                name[k] = ""
-
-        # If code is missing, use value from COLDP
-        if "code" not in name or name["code"] == "":
-            name["code"] = self.coldp.code
-
-        # Skip processing if sic
-        if not sic:
-            # Check uninomials for formatting - log issues and fix case
-            for k in ["uninomial", "genus", "infragenericEpithet"]:
-                if len(name[k]) > 0:
-                    if not name_pattern.match(name[k]):
-                        self.coldp.issue(
-                            f'Invalid pattern for supraspecific name: "{name[k]}"'
-                        )
-                    elif name[k][0].islower():
-                        self.coldp.issue(
-                            "Lowercase initial letter "
-                            + "for supraspecific name: "
-                            + name[k]
-                        )
-                        name[k] = name[k][0].upper() + name[k][1:]
-
-            # Check epithets for formatting - log issues and fix case
-            for k in ["specificEpithet", "infraspecificEpithet"]:
-                if len(name[k]) > 0:
-                    if not name_pattern.match(name[k]):
-                        self.coldp.issue("Invalid pattern for epithet: " + name[k])
-                    elif name[k][0].isupper():
-                        self.coldp.issue(
-                            "Uppercase initial letter for epithet: " + name[k]
-                        )
-                        name[k] = name[k][0].lower() + name[k][1:]
-
-        # If scientificName is present, make sure all parts are
-        # also completed.
-        if name["scientificName"]:
-            match = scientific_name_pattern.match(name["scientificName"])
-            if match is not None:
-                # Handle any name with a specificEpithet
-                if match.group(5):
-                    if not name["genus"]:
-                        name["genus"] = match.group(1)
-                    if not name["infragenericEpithet"] and match.group(3):
-                        name["infragenericEpithet"] = match.group(3)
-                    if not name["specificEpithet"] and match.group(5):
-                        name["specificEpithet"] = match.group(5)
-                    if not name["infraspecificEpithet"] and match.group(8):
-                        name["infraspecificEpithet"] = match.group(8)
-                elif name["rank"] == "subgenus":
-                    if not name["genus"]:
-                        name["genus"] = match.group(1)
-                    if not name["uninomial"] and match.group(3):
-                        name["uninomial"] = match.group(3)
-                else:
-                    if not name["uninomial"]:
-                        name["uninomial"] = match.group(1)
-
-        # Generate properly formatted scientific name unless sic is True.
-        # If sic is True but scientificName is empty, generate anyway.
-        if not sic or not name["scientificName"]:
-            if self.coldp.is_species_group(name):
-                (
-                    name["scientificName"],
-                    name["rank"],
-                ) = self.coldp.construct_species_rank_name(
-                    name["genus"],
-                    name["infragenericEpithet"],
-                    name["specificEpithet"],
-                    name["infraspecificEpithet"],
-                    name["rank"],
-                )
-            else:
-                name["scientificName"] = name["uninomial"]
-
-        # Return normalised version of name
-        return name
-
-    def derive_name(
-        self, name: dict[str:str], values: dict[str:str], sic: bool = False
-    ) -> dict:
-        """
-        Use supplied values to create new name dictionary with missing elements copied from an existing name dictionary
-
-        :param name: Dictionary containing name on which new name is to be based
-        :param values: Dictionary of values to override values in name
-        :return: Name dictionary with supplied values supplemented from name
-        """
-
-        if (
-            "authorship" not in values
-            and "authorship" in name
-            and not name["authorship"].startswith("(")
-        ):
-            if "genus" in values or "specificEpithet" in values:
-                values["authorship"] = "(" + name["authorship"] + ")"
-
-        for k in required_properties["name"]:
-            if k in name and k not in values:
-                values[k] = name[k]
-        return self.normalise_name(values, sic)
-
-
 class COLDP:
     def __init__(
         self,
         name: str,
         folder: str = ".",
         code: str = "ICZN",
         default_taxon_record: dict[str:str] = None,
@@ -594,15 +423,15 @@
         :param basionyms_from_synonyms: If true, basionym associations are automatically created from synonyms within a loaded COLDP dataset. If an accepted name includes parentheses around the authorship, and if a name with the same epithet and authorship but no parentheses is included in the synonyms, the ID value for the synonym will be used for the basionymID element in the accepted name. This is normally a housekeeping step when first loading a new COLDP dataset. This option is only used when the dataset is first loaded. Addition of basionym relationships is automatic for names added as part of the same NameBundle.
         :param classification_from_parents: If true, insert names for higher ranks into relevant elements in each taxon record based on the parent and higher ancestry for the taxon.
         :param allow_repeated_binomials: If true, omit checks rejecting the addition of the same binomial more than once to the COLDP name dataframe.
         :param create_taxa_for_not_established: If true, generate taxon records even if the associated name is flagged as not established (i.e. not satisfying the relevant nomenclatural code)
         :param issues_to_stdout: If true, print any issue messages (see :py:func:`~coldp.COLDP.issue`) to stdout as well as inserting then in the issue dataframe.
         :param context: Value to be used in labeling issue records (see :py:func:`~coldp.COLDP.issue`). This value is more normally set using :py:func:`~coldp.COLDP.set_context`.
 
-        A COLDP object is initalised with a source/destination folder, COLDP package
+        A COLDP object is initialised with a source/destination folder, COLDP package
         name and other options.
 
         If a subfolder exists with the supplied name in the supplied folder, it
         will be initialised with data from any CSV/TSV files it contains with any
         of the following base names: name, taxon, synonym, reference,
         distribution, speciesinteraction, namerelation, typematerial or nameusage,
         and with a file extension recognised via :py:data:`~coldp.COLDP.csv_extensions`.
@@ -662,28 +491,30 @@
         self.references = self.initialise_dataframe(
             source_folder, "reference", reference_headings
         )
         self.distributions = self.initialise_dataframe(
             source_folder, "distribution", distribution_headings
         )
         self.species_interactions = self.initialise_dataframe(
-            source_folder, "speciesinteration", species_interaction_headings
+            source_folder, "speciesinteraction", species_interaction_headings
         )
         self.name_relations = self.initialise_dataframe(
             source_folder, "namerelation", name_relation_headings
         )
         self.type_materials = self.initialise_dataframe(
             source_folder, "typematerial", type_material_headings
         )
         if self.classification_from_parents:
             self.fix_classification()
         if self.basionyms_from_synonyms:
             self.fix_basionyms(self.names, self.synonyms)
         self.issues = None
 
+        self.identifier_policies = {}
+
     def set_options(self, **options: bool):
         """
         Set options controlling COLDP instance from keyword arguments
 
         :param options: Set of boolean options for controlling the behaviour of the COLDP package - see :py:class:`~coldp.COLDP` for boolean options that can be set.
 
         Convenience method for setting options via keyword arguments after the COLDP instance has been created.
@@ -1215,44 +1046,63 @@
         Ensure one or more references are included in references dataframe
 
         :param reference_list: List of dictionaries - each dictionary contains values keyed by terms from reference_headings
         :return: Updated :paramref:`~coldp.COLDP.add_references.reference_list` with IDs for references in this COLDP instance
 
         Find existing ID values for each supplied reference, based on identity
         of: author, title, issued, containerTitle, volume, issue, page and citation. Add
-        ID to the appropriate reference dictionary in references. If none
+        ID from the appropriate reference dictionary in references. If none
         found, set ID to next unused index and add to references.
 
         The list is returned updated with current ID values so these can be used for referenceID values in other classes.
         """
 
         for i in range(len(reference_list)):
-            has_content = False
-            for k in reference_list[i].keys():
-                if reference_list[i][k]:
-                    has_content = True
-                    break
-            if has_content:
-                r = reference_list[i]
-                reference = self.find_reference(reference_list[i])
-                if reference is not None:
-                    reference_list[i] = reference
-                    logging.debug("Matched reference ID " + reference_list[i]["ID"])
-                else:
-                    if not r["ID"]:
-                        r["ID"] = "r_" + str(len(self.references) + 1)
-                    self.references = pd.concat(
-                        (self.references, pd.DataFrame.from_records([r])),
-                        ignore_index=True,
-                    )
-                    logging.debug("Added reference " + str(r))
-            else:
-                reference_list[i]["ID"] = ""
+            reference_list[i] = self.add_reference(reference_list[i])
+
         return reference_list
 
+    def add_reference(self, reference: dict[str:str]) -> dict[str:str]:
+        """
+        Ensure a reference is included in references dataframe
+
+        :param reference: Dictionary containing values keyed by terms from reference_headings
+        :return: Updated :paramref:`~coldp.COLDP.add_references.reference` with ID for reference in this COLDP instance
+
+        Find existing ID values for supplied reference, based on identity
+        of: author, title, issued, containerTitle, volume, issue, page and citation. Add
+        ID from the appropriate reference dictionary in references. If none
+        found, set ID to next unused index and add to references.
+
+        The reference is returned updated with the current ID value so this can be used for referenceID values in other classes.
+        """
+
+        has_content = False
+        for k in reference.keys():
+            if reference[k]:
+                has_content = True
+                break
+        if has_content:
+            r = self.find_reference(reference)
+            if r is not None:
+                logging.debug("Matched reference ID " + r["ID"])
+                reference = r
+            else:
+                if not reference["ID"]:
+                    policy = self.get_identifier_policy("reference", "r_")
+                    reference["ID"] = policy.next(self.references["ID"])
+                self.references = pd.concat(
+                    (self.references, pd.DataFrame.from_records([reference])),
+                    ignore_index=True,
+                )
+                logging.debug("Added reference " + str(reference))
+        else:
+            reference["ID"] = ""
+        return reference
+
     def get_reference(self, id: str) -> dict[str:str]:
         """
         Get reference record as dictionary from ID string
 
         :param id: ID string for requested COLDP reference record
         :return: Dictionary of COLDP reference properties for requested ID
 
@@ -1490,14 +1340,20 @@
             self.issue("Synonym must be associated with a valid taxon ID")
             return None
 
         if "nameID" not in synonym or synonym["nameID"] not in self.names["ID"].values:
             self.issue("Synonym must be associated with a valid name ID")
             return None
 
+        if "ID" in self.synonyms.columns and not synonym["ID"]:
+            policy = self.get_identifier_policy("synonym", "s_", False)
+            next_id = policy.next(self.synonyms["ID"])
+            if next_id is not None:
+                synonym["ID"] = next_id
+
         self.synonyms = pd.concat(
             (self.synonyms, pd.DataFrame.from_records([synonym])),
             ignore_index=True,
         )
         return synonym
 
     def add_type_material(self, type_material: dict[str:str]) -> dict[str:str]:
@@ -1833,22 +1689,26 @@
             if parentID:
                 match = self.taxa[self.taxa["ID"] == parentID]
                 if len(match) == 0:
                     self.issue("Parent taxon not found " + parentID)
                     taxon_row = self.default_taxon
                 else:
                     taxon_row = match.iloc[0].copy()
+                    taxon_row["remarks"] = ""
                     parent_name_row = self.names[
                         self.names["ID"] == taxon_row["nameID"]
                     ]
                     parent_rank = parent_name_row.iloc[0]["rank"]
                     parent_name = parent_name_row.iloc[0]["scientificName"]
             else:
                 taxon_row = self.default_taxon
-            taxon_row["ID"] = str(len(self.taxa) + 1)
+
+            policy = self.get_identifier_policy("taxon", "t_")
+            taxon_row["ID"] = policy.next(self.taxa["ID"])
+
             taxon_row["parentID"] = parentID if parentID else ""
             taxon_row["nameID"] = name["ID"]
             if parent_rank in [
                 "kingdom",
                 "phylum",
                 "class",
                 "order",
@@ -1935,15 +1795,17 @@
 
         if name["rank"] != "species" or not self.allow_repeated_binomials:
             match = self.find_name_record(name)
         if match is not None:
             return match
         else:
             if "ID" not in name or not name["ID"]:
-                name["ID"] = str(len(self.names) + 1)
+                policy = self.get_identifier_policy("name", "n_", False)
+                name["ID"] = policy.next(self.names["ID"])
+
             self.names = pd.concat(
                 (self.names, pd.DataFrame.from_records([name])), ignore_index=True
             )
         return name
 
     def same_basionym(self, a: dict[str:str], b: dict[str:str]) -> bool:
         """
@@ -2481,14 +2343,67 @@
         return "rank" in name and name["rank"] in [
             "variety",
             "subvariety",
             "form",
             "aberration",
         ]
 
+    def get_available_column_headings(self) -> dict[str, list[str]]:
+        """
+        Return dictionary mapping table names to lists of supported columns
+
+        :return: Dictionary containing copies of internal heading lists
+
+        Returns copies to avoid corrupting the lists used in this class
+        """
+        return {
+            "reference": reference_headings.copy(),
+            "name": name_headings.copy(),
+            "taxon": taxon_headings.copy(),
+            "synonym": synonym_headings.copy(),
+            "distribution": distribution_headings.copy(),
+            "typematerial": type_material_headings.copy(),
+            "speciesinteraction": species_interaction_headings.copy(),
+        }
+
+    def get_identifier_policy(
+        self, table_name: str, default_prefix: str = None, required=True, volatile=False
+    ) -> IdentifierPolicy:
+        """
+        Find or create :py:class:`~coldp.IdentifierPolicy` associated with named table
+
+        :param table_name: Name of COLDP dataframe for which policy is required
+        :param default_prefix: String prefix to use before numeric ID values if existing ID values are not consistently positive integer values
+        :param required: Flag to indicate whether the table must have ID values - if False, the :py:class:`~coldp.IdentifierPolicy` will return None unless :paramref:`~coldp.IdentifierPolicy.__init__.existing` already contains ID values
+        :param volatile: Flag to indicate if external code may modify ID values while the current COLDP instance is active - if False, the policy and future values will be determined on initialisation, otherwise the policy will be reviewed for each new ID value
+        :return: :py:class:`~coldp.IdentifierPolicy` object or None if no policy is required for the table
+
+        Creates new :py:class:`~coldp.IdentifierPolicy` instance if this is the first invocation for the given table. Policies take into account any existing ID values for the table.
+        """
+        if table_name not in self.identifier_policies:
+
+            table = self.table_by_name(table_name)
+            if table is None:
+                return None
+
+            headings = self.get_available_column_headings(table)
+            if headings is None or "ID" not in headings:
+                return None
+
+            if "ID" in table.columns:
+                existing = table["ID"]
+            else:
+                existing = None
+
+            self.identifier_policies[table_name] = IdentifierPolicy(
+                table["ID"], default_prefix, required, volatile
+            )
+
+        return self.identifier_policies[table_name]
+
     def save(self, destination: str = None, name: str = None) -> None:
         """
         Write dataframes as COLDP CSV files
 
         :param destination: Path to folder in which package should be saved. Defaults to destination supplied to constructor, which defaults to "."
         :param name: Name for COLDP package (subfolder name). Defaults to name supplied to constructor, which defaults to None. If no name provided, save will fail.
 
@@ -2555,14 +2470,281 @@
             logging.error(context + ": " + message)
 
         self.issues = pd.concat(
             (self.issues, pd.DataFrame.from_records([issue_record])), ignore_index=True
         )
 
 
+class NameBundle:
+    def __init__(
+        self,
+        coldp,
+        accepted: dict[str:str],
+        incertae_sedis: bool = False,
+        sic: bool = False,
+    ) -> None:
+        """
+        Wrapper class to manage set of associated names, normally an accepted name
+        and one or more synonyms. The bundle handles the logic of associated name
+        variations.
+
+        :param coldp: :py:class:`~coldp.COLDP` object to handle logging of any issues and normalise name records
+        :param accepted: Dictionary mapping COLDP name elements to values for the accepted name - a name record and a taxon record will be added to the COLDP package for the accepted name
+        :param incertae_sedis: Flag to indicate if the resulting taxon record should be marked "incertae sedis"
+        :param sic: Flag to indicate if the accepted name should be processed without reporting issues for invalid format
+
+        The minimal usage is to create a new bundle with an accepted name. One
+        or more synonyms can also be supplied using the :py:func:`~coldp.NameBundle.add_synonym` method.
+        The bundle is then submitted to the :py:func:`coldp.COLDP.add_names` method for
+        processing.
+
+        NameBundle objects should not be created directly. Use the :py:func:`coldp.COLDP.start_name_bundle` method instead.
+
+        accepted should contain a dictionary with keys that match property names from the `COLDP Name class <https://github.com/CatalogueOfLife/coldp?tab=readme-ov-file#name>`_
+        """
+
+        self.coldp = coldp
+        if "rank" not in accepted:
+            self.coldp.issue(
+                "Accepted name missing rank, assume species: " + str(accepted)
+            )
+            accepted["rank"] = "species"
+        self.accepted_sic = sic
+        self.accepted = self.normalise_name(accepted.copy(), sic)
+        self.incertae_sedis = incertae_sedis
+        self.accepted_taxon_id = None
+        self.synonyms = []
+        self.species = None
+        self.species_synonym = None
+        self.accepted_species_id = None
+
+    def add_synonym(self, synonym: dict[str:str], sic: bool = False) -> None:
+        """
+        Register an additional name as a synonym for the accepted name
+
+        synonym should contain a dictionary with keys that match property names from the `COLDP Name class <https://github.com/CatalogueOfLife/coldp?tab=readme-ov-file#name>`_
+
+        :param synonym: Dictionary mapping COLDP name elements to values for the synonymous name - a name record and a synonym record will be added to the COLDP package for the synonym
+        :param sic: Flag to indicate that the name does not follow expected formatting rules for a code-compliant name and that no issues should be logged for this
+
+        """
+
+        normalised = self.normalise_name(synonym, sic)
+        present = normalised["scientificName"] == self.accepted["scientificName"]
+        if not present:
+            for s in self.synonyms:
+                if normalised["scientificName"] == s["scientificName"]:
+                    if (
+                        normalised["authorship"] is None
+                        or s["authorship"] is None
+                        or normalised["authorship"] == s["authorship"]
+                    ):
+                        present = True
+                        break
+        if not present:
+            self.synonyms.append(normalised)
+
+    def normalise_name(self, name: dict[str:str], sic: bool = False) -> dict:
+        """
+        Ensure that a name record dictionary contains all necessary/appropriate elements
+
+        :param name: Dictionary containing name to be normalised
+        :param sic: Flag to indicate that the name does not follow expected formatting rules for a code-compliant name and that no issues should be logged for this
+        :return: Name dictionary updated with extra values
+        """
+
+        # Ensure main elements are present in dictionary
+        for k in required_properties["name"]:
+            if k not in name:
+                name[k] = ""
+
+        # If code is missing, use value from COLDP
+        if "code" not in name or name["code"] == "":
+            name["code"] = self.coldp.code
+
+        # Skip processing if sic
+        if not sic:
+            # Check uninomials for formatting - log issues and fix case
+            for k in ["uninomial", "genus", "infragenericEpithet"]:
+                if len(name[k]) > 0:
+                    if not name_pattern.match(name[k]):
+                        self.coldp.issue(
+                            f'Invalid pattern for supraspecific name: "{name[k]}"'
+                        )
+                    elif name[k][0].islower():
+                        self.coldp.issue(
+                            "Lowercase initial letter "
+                            + "for supraspecific name: "
+                            + name[k]
+                        )
+                        name[k] = name[k][0].upper() + name[k][1:]
+
+            # Check epithets for formatting - log issues and fix case
+            for k in ["specificEpithet", "infraspecificEpithet"]:
+                if len(name[k]) > 0:
+                    if not name_pattern.match(name[k]):
+                        self.coldp.issue("Invalid pattern for epithet: " + name[k])
+                    elif name[k][0].isupper():
+                        self.coldp.issue(
+                            "Uppercase initial letter for epithet: " + name[k]
+                        )
+                        name[k] = name[k][0].lower() + name[k][1:]
+
+        # If scientificName is present, make sure all parts are
+        # also completed.
+        if name["scientificName"]:
+            match = scientific_name_pattern.match(name["scientificName"])
+            if match is not None:
+                # Handle any name with a specificEpithet
+                if match.group(5):
+                    if not name["genus"]:
+                        name["genus"] = match.group(1)
+                    if not name["infragenericEpithet"] and match.group(3):
+                        name["infragenericEpithet"] = match.group(3)
+                    if not name["specificEpithet"] and match.group(5):
+                        name["specificEpithet"] = match.group(5)
+                    if not name["infraspecificEpithet"] and match.group(8):
+                        name["infraspecificEpithet"] = match.group(8)
+                elif name["rank"] == "subgenus":
+                    if not name["genus"]:
+                        name["genus"] = match.group(1)
+                    if not name["uninomial"] and match.group(3):
+                        name["uninomial"] = match.group(3)
+                else:
+                    if not name["uninomial"]:
+                        name["uninomial"] = match.group(1)
+
+        # Generate properly formatted scientific name unless sic is True.
+        # If sic is True but scientificName is empty, generate anyway.
+        if not sic or not name["scientificName"]:
+            if self.coldp.is_species_group(name):
+                (
+                    name["scientificName"],
+                    name["rank"],
+                ) = self.coldp.construct_species_rank_name(
+                    name["genus"],
+                    name["infragenericEpithet"],
+                    name["specificEpithet"],
+                    name["infraspecificEpithet"],
+                    name["rank"],
+                )
+            else:
+                name["scientificName"] = name["uninomial"]
+
+        # Return normalised version of name
+        return name
+
+    def derive_name(
+        self, name: dict[str:str], values: dict[str:str], sic: bool = False
+    ) -> dict:
+        """
+        Use supplied values to create new name dictionary with missing elements copied from an existing name dictionary
+
+        :param name: Dictionary containing name on which new name is to be based
+        :param values: Dictionary of values to override values in name
+        :return: Name dictionary with supplied values supplemented from name
+        """
+
+        if (
+            "authorship" not in values
+            and "authorship" in name
+            and not name["authorship"].startswith("(")
+        ):
+            if "genus" in values or "specificEpithet" in values:
+                values["authorship"] = "(" + name["authorship"] + ")"
+
+        for k in required_properties["name"]:
+            if k in name and k not in values:
+                values[k] = name[k]
+        return self.normalise_name(values, sic)
+
+
+class IdentifierPolicy:
+
+    def __init__(
+        self,
+        existing: pd.Series,
+        default_prefix: str,
+        required: bool = True,
+        volatile: bool = False,
+    ) -> None:
+        """
+        Internal class to manage ID values in COLDP dataframes.
+
+        :param existing: Pandas series containing current ID values for table - may be empty or None
+        :param default_prefix: String prefix to use before numeric ID values if existing ID values are not consistently positive integer values
+        :param required: Flag to indicate whether the table must have ID values - if False, the :py:class:`~coldp.IdentifierPolicy` will return None unless :paramref:`~coldp.IdentifierPolicy.__init__.existing` already contains ID values
+        :param volatile: Flag to indicate if external code may modify ID values while the current COLDP instance is active - if False, the policy and future values will be determined on initialisation, otherwise the policy will be reviewed for each new ID value
+
+        Checks any existing values in the series. If none are present, the next ID value will be 1. If all values are integer strings, the next value will be the integer string with a value one higher than the current maximum value. Otherwise ID values will be the concatenation of the prefix (defaulting to the empty string) and the current length of the ID series. Subsequent values will increment by one.
+
+        If :paramref:`~coldp.IdentifierPolicy.__init__.required` is False and no current valus exist in the series, the policy will always return None.
+
+        If :paramref:`~coldp.IdentifierPolicy.__init__.volatile` is True, the policy will be revised on every invocation of next. Otherwise, the series will only be scanned on initialisation and all policy values will then be fixed.
+        """
+
+        self.required = required
+        self.volatile = volatile
+        self.default_prefix = default_prefix
+
+        if not self.volatile:
+            self.next_value, self.prefix = self.initialise(existing)
+        else:
+            self.next_value = None
+            self.prefix = None
+
+        return
+
+    def initialise(self, existing: pd.Series) -> tuple[int, str]:
+        """
+        Internal method to set or refresh policy
+
+        :param existing: Pandas series containing current ID values for table - may be empty or None
+        :return: Tuple comprising the next integer value for the policy and a prefix for use if ID values should not be plain integer strings - one or both values will be None
+
+        Provides the variables to determine the next ID value, if any
+        """
+
+        if existing is None or len(existing) == 0:
+            if self.required:
+                return 1, None
+            else:
+                return None, None
+
+        if len(existing.str.match(r"^[0-9]+$")) == len(existing):
+            return existing.astype(int).max() + 1, None
+
+        elif self.default_prefix is not None:
+            return None, self.default_prefix
+
+        return None, ""
+
+    def next(self, existing: pd.Series = None) -> str:
+        """
+        Return next ID value for series
+
+        :param existing: Pandas series containing current ID values for table - may be empty or None - only required if :paramref:`~coldp.IdentifierPolicy.__init__.volatile` is True
+        :return: Next string ID value for policy or None if no ID is required
+
+        Returns the next ID value for use in the Series associated with this IdentifierPolicy. Recalculates policy if paramref:`~coldp.IdentifierPolicy.__init__.volatile` is True.
+        """
+        if self.volatile:
+            next_value, prefix = self.initialise(existing)
+        else:
+            next_value = self.next_value
+            self.next_value = self.next_value + 1
+            prefix = self.prefix
+
+        if next_value is not None:
+            return str(next_value)
+        elif prefix is not None:
+            return f"{prefix}{len(existing) + 1}"
+        return None
+
+
 if __name__ == "__main__":
     logging.basicConfig(filename="COLDP.log", level=logging.DEBUG)
 
     test_folder = "../../test"
 
     default_taxon = {
         "kingdom": "Animalia",
```

### Comparing `coldp-2024.5.3/src/coldp/coldp_distribution.py` & `coldp-2024.5.4/src/coldp/coldp_distribution.py`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/src/coldp/testit.py` & `coldp-2024.5.4/src/coldp/testit.py`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/test/test_coldp.py` & `coldp-2024.5.4/test/test_coldp.py`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/test/input/Tonzidae/NameUsage.tsv` & `coldp-2024.5.4/test/input/Tonzidae/NameUsage.tsv`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/test/input/Tonzidae/Reference.tsv` & `coldp-2024.5.4/test/input/Tonzidae/Reference.tsv`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/test/input/Tonzidae/logo.png` & `coldp-2024.5.4/test/input/Tonzidae/logo.png`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/test/input/Tonzidae/metadata.yaml` & `coldp-2024.5.4/test/input/Tonzidae/metadata.yaml`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/LICENSE` & `coldp-2024.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.3/README.md` & `coldp-2024.5.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,10 +23,10 @@
 
 # Installation
 ```console
 pip install py-coldp
 ```
 
 # Documentation
-[Browsable documentation for COLDP version: 2024.5.3](https://html-preview.github.io/?url=https://github.com/dhobern/py-coldp/blob/main/docs/build/html/index.html)
+[Browsable documentation for COLDP version: 2024.5.4](https://html-preview.github.io/?url=https://github.com/dhobern/py-coldp/blob/main/docs/build/html/index.html)
 
-[PDF documentation for COLDP version: 2024.5.3](https://github.com/dhobern/py-coldp/blob/main/docs/build/simplepdf/COLDP.pdf)
+[PDF documentation for COLDP version: 2024.5.4](https://github.com/dhobern/py-coldp/blob/main/docs/build/simplepdf/COLDP.pdf)
```

### Comparing `coldp-2024.5.3/pyproject.toml` & `coldp-2024.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "coldp"
-version = "2024.5.3"
+version = "2024.5.4"
 authors = [
   { name="Donald Hobern", email="dhobern@gmail.com" },
 ]
 description = "Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format"
 keywords = ["Catalogue of Life", "COLDP", "taxonomic checklist"]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `coldp-2024.5.3/PKG-INFO` & `coldp-2024.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coldp
-Version: 2024.5.3
+Version: 2024.5.4
 Summary: Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format
 Project-URL: Homepage, https://github.com/dhobern/py-coldp
 Project-URL: Issues, https://github.com/dhobern/py-coldp/issues
 Author-email: Donald Hobern <dhobern@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Donald Hobern]
@@ -67,10 +67,10 @@
 
 # Installation
 ```console
 pip install py-coldp
 ```
 
 # Documentation
-[Browsable documentation for COLDP version: 2024.5.3](https://html-preview.github.io/?url=https://github.com/dhobern/py-coldp/blob/main/docs/build/html/index.html)
+[Browsable documentation for COLDP version: 2024.5.4](https://html-preview.github.io/?url=https://github.com/dhobern/py-coldp/blob/main/docs/build/html/index.html)
 
-[PDF documentation for COLDP version: 2024.5.3](https://github.com/dhobern/py-coldp/blob/main/docs/build/simplepdf/COLDP.pdf)
+[PDF documentation for COLDP version: 2024.5.4](https://github.com/dhobern/py-coldp/blob/main/docs/build/simplepdf/COLDP.pdf)
```

