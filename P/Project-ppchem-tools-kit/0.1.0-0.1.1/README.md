# Comparing `tmp/project_ppchem_tools_kit-0.1.0.tar.gz` & `tmp/project_ppchem_tools_kit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_ppchem_tools_kit-0.1.0.tar", max compression
+gzip compressed data, was "project_ppchem_tools_kit-0.1.1.tar", max compression
```

## Comparing `project_ppchem_tools_kit-0.1.0.tar` & `project_ppchem_tools_kit-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,37 @@
--rw-r--r--   0        0        0     1096 2024-05-17 13:18:42.194501 project_ppchem_tools_kit-0.1.0/LICENSE
--rw-r--r--   0        0        0     6254 2024-05-18 14:31:41.440522 project_ppchem_tools_kit-0.1.0/README.md
--rw-r--r--   0        0        0      793 2024-05-18 15:43:28.633881 project_ppchem_tools_kit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 20:44:57.565187 project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/__init__.py
--rw-r--r--   0        0        0     1574 2024-05-17 12:06:36.279430 project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/display_molecule.py
--rw-r--r--   0        0        0     6172 2024-05-16 22:25:13.268440 project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/error_calculation_interface.py
--rw-r--r--   0        0        0     9287 2024-05-18 13:16:11.687288 project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/graph_function.py
--rw-r--r--   0        0        0     1631 2024-05-17 12:30:45.243767 project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/linear_regression.py
--rw-r--r--   0        0        0     1049 2024-05-17 12:30:47.913439 project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/make_graph.py
--rw-r--r--   0        0        0      371 2024-05-16 10:14:47.990043 project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/name_to_smiles.py
--rw-r--r--   0        0        0      231 2024-05-16 10:14:47.987920 project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/smiles_to_molar_mass.py
--rw-r--r--   0        0        0     7317 1970-01-01 00:00:00.000000 project_ppchem_tools_kit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-17 13:18:42.194501 project_ppchem_tools_kit-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6815 2024-05-19 09:06:31.287575 project_ppchem_tools_kit-0.1.1/README.md
+-rw-r--r--   0        0        0      650 2024-05-19 09:17:30.424278 project_ppchem_tools_kit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 20:44:57.565187 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/__init__.py
+-rw-r--r--   0        0        0      566 2024-05-18 16:20:56.501812 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/add_data_point.py
+-rw-r--r--   0        0        0      376 2024-05-19 09:11:37.994019 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/bind_enter.py
+-rw-r--r--   0        0        0      672 2024-05-18 17:45:23.130803 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/browse_excel_file.py
+-rw-r--r--   0        0        0      164 2024-05-18 17:45:23.131373 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/clear_input.py
+-rw-r--r--   0        0        0      504 2024-05-19 07:44:17.259322 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/copy_text.py
+-rw-r--r--   0        0        0      979 2024-05-19 09:11:37.994184 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/create_radio_button.py
+-rw-r--r--   0        0        0     2704 2024-05-19 09:11:37.993513 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_graph.py
+-rw-r--r--   0        0        0     2147 2024-05-18 16:20:56.504673 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_max_point_and_coords.py
+-rw-r--r--   0        0        0     1574 2024-05-17 12:06:36.279430 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_molecule.py
+-rw-r--r--   0        0        0      581 2024-05-18 16:20:56.505034 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_result.py
+-rw-r--r--   0        0        0     6226 2024-05-19 07:58:29.644129 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/error_calculation_interface.py
+-rw-r--r--   0        0        0     9287 2024-05-18 13:16:11.687288 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/graph_function.py
+-rw-r--r--   0        0        0     1646 2024-05-19 09:11:38.148414 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/linear_regression.py
+-rw-r--r--   0        0        0     1064 2024-05-19 09:11:38.148314 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/make_graph.py
+-rw-r--r--   0        0        0      371 2024-05-16 10:14:47.990043 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/name_to_smiles.py
+-rw-r--r--   0        0        0      226 2024-05-18 17:45:23.132897 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/on_closing.py
+-rw-r--r--   0        0        0      358 2024-05-19 09:11:37.994342 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/on_radio_select.py
+-rw-r--r--   0        0        0     1784 2024-05-19 09:11:37.993793 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/open_graph_settings_window.py
+-rw-r--r--   0        0        0     2504 2024-05-19 09:11:37.993466 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/process_input.py
+-rw-r--r--   0        0        0      212 2024-05-19 08:19:40.701466 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/relative_to_assets.py
+-rw-r--r--   0        0        0      147 2024-05-18 16:20:56.506233 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/select_all.py
+-rw-r--r--   0        0        0      391 2024-05-18 16:20:56.506577 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_axes_color.py
+-rw-r--r--   0        0        0      526 2024-05-18 16:20:56.506862 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_background_color.py
+-rw-r--r--   0        0        0      619 2024-05-18 16:20:56.507221 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_custom_labels_and_title.py
+-rw-r--r--   0        0        0      184 2024-05-18 16:20:56.507696 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_grid_color.py
+-rw-r--r--   0        0        0      270 2024-05-18 16:20:56.508228 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_label_color.py
+-rw-r--r--   0        0        0      432 2024-05-18 16:20:56.508577 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_line_color.py
+-rw-r--r--   0        0        0      492 2024-05-18 16:20:56.508962 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_scale.py
+-rw-r--r--   0        0        0      231 2024-05-16 10:14:47.987920 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/smiles_to_molar_mass.py
+-rw-r--r--   0        0        0      124 2024-05-18 16:20:56.509235 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/toggle_grid.py
+-rw-r--r--   0        0        0      573 2024-05-18 17:45:23.133845 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/update_clock.py
+-rw-r--r--   0        0        0      908 2024-05-19 08:54:54.692946 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/welcome_message.py
+-rw-r--r--   0        0        0     7754 1970-01-01 00:00:00.000000 project_ppchem_tools_kit-0.1.1/PKG-INFO
```

### Comparing `project_ppchem_tools_kit-0.1.0/LICENSE` & `project_ppchem_tools_kit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.0/README.md` & `project_ppchem_tools_kit-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,391 +1,426 @@
-00000000: 0a23 20f0 9fa7 b020 546f 6f6c 7320 4b69  .# .... Tools Ki
-00000010: 740a 215b 6c6f 676f 5d28 6874 7470 733a  t.![logo](https:
-00000020: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6772  //github.com/sgr
-00000030: 756e 6265 722f 5072 6f6a 6563 742d 7070  unber/Project-pp
-00000040: 6368 656d 2d74 6f6f 6c73 2d6b 6974 2f61  chem-tools-kit/a
-00000050: 7373 6574 732f 3136 3038 3831 3836 342f  ssets/160881864/
-00000060: 3265 3435 3930 6233 2d37 3031 352d 3466  2e4590b3-7015-4f
-00000070: 3639 2d39 3734 362d 6439 3530 6538 3761  69-9746-d950e87a
-00000080: 3766 3866 290a 0a5b 215b 6275 696c 645d  7f8f)..[![build]
-00000090: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000000a0: 656c 6473 2e69 6f2f 6261 6467 652f 6275  elds.io/badge/bu
-000000b0: 696c 642d 7061 7373 696e 672d 6272 6967  ild-passing-brig
-000000c0: 6874 6772 6565 6e29 5d28 6874 7470 733a  htgreen)](https:
-000000d0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6772  //github.com/sgr
-000000e0: 756e 6265 722f 5072 6f6a 6563 742d 7070  unber/Project-pp
-000000f0: 6368 656d 2d74 6f6f 6c73 2d6b 6974 290a  chem-tools-kit).
-00000100: 5b21 5b63 6f76 6572 6167 655d 2868 7474  [![coverage](htt
-00000110: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000120: 2e69 6f2f 6261 6467 652f 636f 7665 7261  .io/badge/covera
-00000130: 6765 2d39 3525 3235 2d62 7269 6768 7467  ge-95%25-brightg
-00000140: 7265 656e 295d 2868 7474 7073 3a2f 2f67  reen)](https://g
-00000150: 6974 6875 622e 636f 6d2f 7367 7275 6e62  ithub.com/sgrunb
-00000160: 6572 2f50 726f 6a65 6374 2d70 7063 6865  er/Project-ppche
-00000170: 6d2d 746f 6f6c 732d 6b69 7429 0a5b 215b  m-tools-kit).[![
-00000180: 6c69 6365 6e73 655d 2868 7474 7073 3a2f  license](https:/
-00000190: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000001a0: 6261 6467 652f 6c69 6365 6e73 652d 4d49  badge/license-MI
-000001b0: 542d 626c 7565 295d 2868 7474 7073 3a2f  T-blue)](https:/
-000001c0: 2f67 6974 6875 622e 636f 6d2f 7367 7275  /github.com/sgru
-000001d0: 6e62 6572 2f50 726f 6a65 6374 2d70 7063  nber/Project-ppc
-000001e0: 6865 6d2d 746f 6f6c 732d 6b69 742f 626c  hem-tools-kit/bl
-000001f0: 6f62 2f6d 6169 6e2f 4c49 4345 4e53 4529  ob/main/LICENSE)
-00000200: 0a0a 0a23 2320 f09f 9396 2044 6573 6372  ...## .... Descr
-00000210: 6970 7469 6f6e 0a54 6865 202a 2a54 6f6f  iption.The **Too
-00000220: 6c73 204b 6974 2a2a 2070 6163 6b61 6765  ls Kit** package
-00000230: 2061 6c6c 6f77 7320 6368 656d 6973 7472   allows chemistr
-00000240: 7920 7374 7564 656e 7473 2074 6f20 6669  y students to fi
-00000250: 6e64 2062 6173 6963 2069 6e66 6f72 6d61  nd basic informa
-00000260: 7469 6f6e 206f 6e20 6d6f 6c65 6375 6c65  tion on molecule
-00000270: 7320 616e 6420 7072 6f76 6964 6573 2065  s and provides e
-00000280: 6173 7920 6163 6365 7373 2074 6f20 736f  asy access to so
-00000290: 6d65 2067 7261 7068 7320 616e 6420 6361  me graphs and ca
-000002a0: 6c63 756c 6174 696f 6e73 2072 6571 7569  lculations requi
-000002b0: 7265 6420 696e 2065 7870 6572 696d 656e  red in experimen
-000002c0: 7461 6c20 6c61 626f 7261 746f 7269 6573  tal laboratories
-000002d0: 2e0a 0a23 2320 f09f 939a 2054 6162 6c65  ...## .... Table
-000002e0: 206f 6620 436f 6e74 656e 7473 0a2d 205b   of Contents.- [
-000002f0: 496e 7374 616c 6c61 7469 6f6e 5d28 23ef  Installation](#.
-00000300: b88f 2d69 6e73 7461 6c6c 6174 696f 6e29  ..-installation)
-00000310: 0a2d 205b 5573 6167 655d 2823 efb8 8f2d  .- [Usage](#...-
-00000320: 7573 6167 6529 0a2d 205b 4665 6174 7572  usage).- [Featur
-00000330: 6573 5d28 23ef b88f 2d66 6561 7475 7265  es](#...-feature
-00000340: 7329 0a2d 205b 436f 6e74 7269 6275 7469  s).- [Contributi
-00000350: 6e67 5d28 23ef b88f 2d63 6f6e 7472 6962  ng](#...-contrib
-00000360: 7574 696e 6729 0a2d 205b 4369 7465 2055  uting).- [Cite U
-00000370: 735d 2823 efb8 8f2d 6369 7465 2d75 7329  s](#...-cite-us)
-00000380: 0a2d 205b 4c69 6365 6e73 655d 2823 efb8  .- [License](#..
-00000390: 8f2d 6c69 6365 6e73 6529 0a2d 205b 5363  .-license).- [Sc
-000003a0: 7265 656e 7368 6f74 735d 2823 efb8 8f2d  reenshots](#...-
-000003b0: 7363 7265 656e 7368 6f74 7329 0a0a 2323  screenshots)..##
-000003c0: 20f0 9f9b a0ef b88f 2049 6e73 7461 6c6c   ....... Install
-000003d0: 6174 696f 6e0a 3c61 2069 643d 2269 6e73  ation.<a id="ins
-000003e0: 7461 6c6c 6174 696f 6e22 3e3c 2f61 3e0a  tallation"></a>.
-000003f0: 2323 2320 312e 20f0 9f8d b420 466f 726b  ### 1. .... Fork
-00000400: 2074 6865 2052 6570 6f73 6974 6f72 790a   the Repository.
-00000410: 546f 2073 7461 7274 2c20 666f 726b 2074  To start, fork t
-00000420: 6865 2072 6570 6f73 6974 6f72 7920 746f  he repository to
-00000430: 2079 6f75 7220 6f77 6e20 4769 7448 7562   your own GitHub
-00000440: 2061 6363 6f75 6e74 2e20 200a 546f 2064   account.  .To d
-00000450: 6f20 736f 2c20 6e61 7669 6761 7465 2074  o so, navigate t
-00000460: 6f20 7468 6520 7265 706f 7369 746f 7279  o the repository
-00000470: 2070 6167 6520 616e 6420 636c 6963 6b20   page and click 
-00000480: 7468 6520 2a22 466f 726b 222a 2062 7574  the *"Fork"* but
-00000490: 746f 6e2e 2054 6865 2072 6570 6f73 6974  ton. The reposit
-000004a0: 6f72 7920 7769 6c6c 2074 6865 6e20 6265  ory will then be
-000004b0: 2063 6f70 6965 6420 746f 2079 6f75 7220   copied to your 
-000004c0: 6163 636f 756e 742c 2061 6e64 2079 6f75  account, and you
-000004d0: 2077 696c 6c20 6265 2061 626c 6520 746f   will be able to
-000004e0: 2061 6363 6573 7320 6974 2e0a 0a23 2323   access it...###
-000004f0: 2032 2e20 f09f 93a5 2043 6c6f 6e65 2074   2. .... Clone t
-00000500: 6865 2052 6570 6f73 6974 6f72 790a 4e65  he Repository.Ne
-00000510: 7874 2c20 636c 6f6e 6520 7468 6520 7265  xt, clone the re
-00000520: 706f 7369 746f 7279 2075 7369 6e67 2074  pository using t
-00000530: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00000540: 6d61 6e64 2028 7265 706c 6163 6520 2a75  mand (replace *u
-00000550: 7365 726e 616d 652a 2077 6974 6820 796f  sername* with yo
-00000560: 7572 2047 6974 4875 6220 7573 6572 6e61  ur GitHub userna
-00000570: 6d65 293a 0a0a 6060 6062 6173 680a 6769  me):..```bash.gi
-00000580: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
-00000590: 6769 7468 7562 2e63 6f6d 2f2a 7573 6572  github.com/*user
-000005a0: 6e61 6d65 2a2f 5072 6f6a 6563 742d 7070  name*/Project-pp
-000005b0: 6368 656d 2d74 6f6f 6c73 2d6b 6974 2e67  chem-tools-kit.g
-000005c0: 6974 0a60 6060 0a0a 2323 2320 332e 20e2  it.```..### 3. .
-000005d0: ac87 efb8 8f20 496e 7374 616c 6c20 7769  ..... Install wi
-000005e0: 7468 2070 6970 0a59 6f75 2063 616e 2061  th pip.You can a
-000005f0: 6c73 6f20 696e 7374 616c 6c20 546f 6f6c  lso install Tool
-00000600: 7320 4b69 7420 7573 696e 6720 7069 703a  s Kit using pip:
-00000610: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
-00000620: 7374 616c 6c20 5072 6f6a 6563 745f 7070  stall Project_pp
-00000630: 6368 656d 2d74 6f6f 6c73 2d6b 6974 0a60  chem-tools-kit.`
-00000640: 6060 0a0a 2323 20f0 9f9a 8020 5573 6167  ``..## .... Usag
-00000650: 650a 3c61 2069 643d 2275 7361 6765 223e  e.<a id="usage">
-00000660: 3c2f 613e 0a0a 546f 2075 7365 2054 6f6f  </a>..To use Too
-00000670: 6c73 204b 6974 2061 6e64 2061 6363 6573  ls Kit and acces
-00000680: 7320 6974 7320 6665 6174 7572 6573 2c20  s its features, 
-00000690: 666f 6c6c 6f77 2074 6865 7365 2073 7465  follow these ste
-000006a0: 7073 2061 6674 6572 2063 6c6f 6e69 6e67  ps after cloning
-000006b0: 2074 6865 2072 6570 6f73 6974 6f72 793a   the repository:
-000006c0: 0a0a 2323 2320 5573 696e 6720 4a75 7079  ..### Using Jupy
-000006d0: 7465 7220 4e6f 7465 626f 6f6b 3a0a 0a31  ter Notebook:..1
-000006e0: 2e20 4c61 756e 6368 204a 7570 7974 6572  . Launch Jupyter
-000006f0: 204e 6f74 6562 6f6f 6b20 6279 206e 6176   Notebook by nav
-00000700: 6967 6174 696e 6720 746f 2074 6865 2063  igating to the c
-00000710: 6c6f 6e65 6420 7265 706f 7369 746f 7279  loned repository
-00000720: 2064 6972 6563 746f 7279 2069 6e20 796f   directory in yo
-00000730: 7572 2074 6572 6d69 6e61 6c20 616e 6420  ur terminal and 
-00000740: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
-00000750: 616e 643a 0a20 2020 6060 6062 6173 680a  and:.   ```bash.
-00000760: 2020 206a 7570 7974 6572 206e 6f74 6562     jupyter noteb
-00000770: 6f6f 6b0a 2020 2060 6060 0a32 2e20 496e  ook.   ```.2. In
-00000780: 2074 6865 204a 7570 7974 6572 204e 6f74   the Jupyter Not
-00000790: 6562 6f6f 6b20 696e 7465 7266 6163 652c  ebook interface,
-000007a0: 206e 6176 6967 6174 6520 746f 2074 6865   navigate to the
-000007b0: 2060 6e6f 7465 626f 6f6b 7360 2064 6972   `notebooks` dir
-000007c0: 6563 746f 7279 2e0a 0a33 2e20 4f70 656e  ectory...3. Open
-000007d0: 2074 6865 206e 6f74 6562 6f6f 6b20 6e61   the notebook na
-000007e0: 6d65 6420 6070 726f 6a65 6374 5f72 6570  med `project_rep
-000007f0: 6f72 742e 6970 796e 6260 2e0a 0a34 2e20  ort.ipynb`...4. 
-00000800: 466f 6c6c 6f77 2074 6865 2069 6e73 7472  Follow the instr
-00000810: 7563 7469 6f6e 7320 696e 7369 6465 2074  uctions inside t
-00000820: 6865 206e 6f74 6562 6f6f 6b20 746f 2069  he notebook to i
-00000830: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
-00000840: 2054 6f6f 6c73 204b 6974 2069 6e74 6572   Tools Kit inter
-00000850: 6661 6365 2061 6e64 2075 7469 6c69 7a65  face and utilize
-00000860: 2069 7473 2066 6561 7475 7265 7320 666f   its features fo
-00000870: 7220 6d6f 6c65 6375 6c65 2061 6e61 6c79  r molecule analy
-00000880: 7369 732c 2067 7261 7068 2070 6c6f 7474  sis, graph plott
-00000890: 696e 672c 2065 7272 6f72 2063 616c 6375  ing, error calcu
-000008a0: 6c61 7469 6f6e 2c20 616e 6420 6d6f 7265  lation, and more
-000008b0: 2e0a 5468 6973 206e 6f74 6562 6f6f 6b20  ..This notebook 
-000008c0: 7072 6f76 6964 6573 2061 6e20 696e 7465  provides an inte
-000008d0: 7261 6374 6976 6520 656e 7669 726f 6e6d  ractive environm
-000008e0: 656e 7420 666f 7220 636f 6e76 656e 6965  ent for convenie
-000008f0: 6e74 2075 7361 6765 206f 6620 546f 6f6c  nt usage of Tool
-00000900: 7320 4b69 7420 6469 7265 6374 6c79 2077  s Kit directly w
-00000910: 6974 6869 6e20 5669 7375 616c 2053 7475  ithin Visual Stu
-00000920: 6469 6f20 436f 6465 2e0a 0a0a 2323 2320  dio Code....### 
-00000930: 5573 6167 6520 7769 7468 2056 6973 7561  Usage with Visua
-00000940: 6c20 5374 7564 696f 2043 6f64 653a 0a0a  l Studio Code:..
-00000950: 312e 204f 7065 6e20 5669 7375 616c 2053  1. Open Visual S
-00000960: 7475 6469 6f20 436f 6465 2061 6e64 206e  tudio Code and n
-00000970: 6176 6967 6174 6520 746f 2074 6865 2063  avigate to the c
-00000980: 6c6f 6e65 6420 6469 7265 6374 6f72 792e  loned directory.
-00000990: 0a0a 322e 2049 6e73 7461 6c6c 2074 6865  ..2. Install the
-000009a0: 204a 7570 7974 6572 2065 7874 656e 7369   Jupyter extensi
-000009b0: 6f6e 2069 6620 6e6f 7420 616c 7265 6164  on if not alread
-000009c0: 7920 696e 7374 616c 6c65 642e 2059 6f75  y installed. You
-000009d0: 2063 616e 2064 6f20 7468 6973 2062 7920   can do this by 
-000009e0: 7365 6172 6368 696e 6720 666f 7220 224a  searching for "J
-000009f0: 7570 7974 6572 2220 696e 2074 6865 2045  upyter" in the E
-00000a00: 7874 656e 7369 6f6e 7320 7669 6577 2028  xtensions view (
-00000a10: 4374 726c 2b53 6869 6674 2b58 2920 616e  Ctrl+Shift+X) an
-00000a20: 6420 696e 7374 616c 6c69 6e67 2074 6865  d installing the
-00000a30: 2022 5079 7468 6f6e 2220 6578 7465 6e73   "Python" extens
-00000a40: 696f 6e20 7061 636b 2e0a 0a33 2e20 4f70  ion pack...3. Op
-00000a50: 656e 2074 6865 2060 6e6f 7465 626f 6f6b  en the `notebook
-00000a60: 7360 2064 6972 6563 746f 7279 2069 6e20  s` directory in 
-00000a70: 5669 7375 616c 2053 7475 6469 6f20 436f  Visual Studio Co
-00000a80: 6465 2e0a 0a34 2e20 4f70 656e 2074 6865  de...4. Open the
-00000a90: 206e 6f74 6562 6f6f 6b20 6e61 6d65 6420   notebook named 
-00000aa0: 6070 726f 6a65 6374 5f72 6570 6f72 742e  `project_report.
-00000ab0: 6970 796e 6260 2e0a 0a35 2e20 466f 6c6c  ipynb`...5. Foll
-00000ac0: 6f77 2074 6865 2069 6e73 7472 7563 7469  ow the instructi
-00000ad0: 6f6e 7320 696e 7369 6465 2074 6865 206e  ons inside the n
-00000ae0: 6f74 6562 6f6f 6b20 746f 2069 6e74 6572  otebook to inter
-00000af0: 6163 7420 7769 7468 2074 6865 2054 6f6f  act with the Too
-00000b00: 6c73 204b 6974 2069 6e74 6572 6661 6365  ls Kit interface
-00000b10: 2061 6e64 2075 7469 6c69 7a65 2069 7473   and utilize its
-00000b20: 2066 6561 7475 7265 7320 666f 7220 6d6f   features for mo
-00000b30: 6c65 6375 6c65 2061 6e61 6c79 7369 732c  lecule analysis,
-00000b40: 2067 7261 7068 2070 6c6f 7474 696e 672c   graph plotting,
-00000b50: 2065 7272 6f72 2063 616c 6375 6c61 7469   error calculati
-00000b60: 6f6e 2c20 616e 6420 6d6f 7265 2e0a 5468  on, and more..Th
-00000b70: 6973 206e 6f74 6562 6f6f 6b20 7072 6f76  is notebook prov
-00000b80: 6964 6573 2061 6e20 696e 7465 7261 6374  ides an interact
-00000b90: 6976 6520 656e 7669 726f 6e6d 656e 7420  ive environment 
-00000ba0: 666f 7220 636f 6e76 656e 6965 6e74 2075  for convenient u
-00000bb0: 7361 6765 206f 6620 546f 6f6c 7320 4b69  sage of Tools Ki
-00000bc0: 7420 7769 7468 204a 7570 7974 6572 204e  t with Jupyter N
-00000bd0: 6f74 6562 6f6f 6b2e 0a0a 2323 20f0 9fa7  otebook...## ...
-00000be0: aa20 4665 6174 7572 6573 0a0a 312e 20f0  . Features..1. .
-00000bf0: 9fa7 ac20 4d6f 6c65 6375 6c65 204e 616d  ... Molecule Nam
-00000c00: 650a 2020 202d 2049 6e70 7574 3a20 5261  e.   - Input: Ra
-00000c10: 7720 666f 726d 756c 6120 6f66 2074 6865  w formula of the
-00000c20: 206d 6f6c 6563 756c 650a 2020 202d 204f   molecule.   - O
-00000c30: 7574 7075 743a 2053 4d49 4c45 5320 6f66  utput: SMILES of
-00000c40: 2074 6865 206d 6f6c 6563 756c 650a 0a32   the molecule..2
-00000c50: 2e20 e29a 96ef b88f 204d 6f6c 6563 756c  . ...... Molecul
-00000c60: 6172 2057 6569 6768 740a 2020 202d 2049  ar Weight.   - I
-00000c70: 6e70 7574 3a20 534d 494c 4553 206f 6620  nput: SMILES of 
-00000c80: 7468 6520 6d6f 6c65 6375 6c65 0a20 2020  the molecule.   
-00000c90: 2d20 4f75 7470 7574 3a20 436f 7272 6573  - Output: Corres
-00000ca0: 706f 6e64 696e 6720 6d6f 6c61 7220 6d61  ponding molar ma
-00000cb0: 7373 2069 6e20 672f 6d6f 6c0a 0a33 2e20  ss in g/mol..3. 
-00000cc0: f09f 9388 204c 696e 6561 7220 5265 6772  .... Linear Regr
-00000cd0: 6573 7369 6f6e 0a20 2020 2d20 496e 7075  ession.   - Inpu
-00000ce0: 743a 2045 7863 656c 2064 6f63 756d 656e  t: Excel documen
-00000cf0: 7420 2869 6d70 6f72 7465 6420 6279 2070  t (imported by p
-00000d00: 7265 7373 696e 6720 7468 6520 4272 6f77  ressing the Brow
-00000d10: 7365 2062 7574 746f 6e29 0a20 2020 2d20  se button).   - 
-00000d20: 4f75 7470 7574 3a20 4c69 6e65 6172 2072  Output: Linear r
-00000d30: 6567 7265 7373 696f 6e20 6772 6170 6820  egression graph 
-00000d40: 7769 7468 2074 6865 2052 3c73 7570 3e32  with the R<sup>2
-00000d50: 3c2f 7375 703e 2076 616c 7565 0a0a 342e  </sup> value..4.
-00000d60: 20f0 9f93 8a20 4772 6170 6820 4d61 6b65   .... Graph Make
-00000d70: 720a 2020 202d 2049 6e70 7574 3a20 4578  r.   - Input: Ex
-00000d80: 6365 6c20 646f 6375 6d65 6e74 2077 6974  cel document wit
-00000d90: 6820 7820 616e 6420 7920 7661 6c75 6573  h x and y values
-00000da0: 2061 7272 616e 6765 6420 696e 2074 776f   arranged in two
-00000db0: 2063 6f6c 756d 6e73 0a20 2020 2d20 4f75   columns.   - Ou
-00000dc0: 7470 7574 3a20 4772 6170 6820 706c 6f74  tput: Graph plot
-00000dd0: 7469 6e67 2061 6c6c 2076 616c 7565 730a  ting all values.
-00000de0: 2020 2020 2020 2d20 4f70 7469 6f6e 733a        - Options:
-00000df0: 2054 6865 2067 7261 7068 2061 6c6c 6f77   The graph allow
-00000e00: 7320 6375 7374 6f6d 697a 6174 696f 6e20  s customization 
-00000e10: 6f66 2076 6172 696f 7573 2070 6172 616d  of various param
-00000e20: 6574 6572 7320 7375 6368 2061 7320 6368  eters such as ch
-00000e30: 616e 6769 6e67 2073 6361 6c65 732c 2061  anging scales, a
-00000e40: 7869 7320 6c61 6265 6c73 2c20 7469 746c  xis labels, titl
-00000e50: 652c 2064 6973 706c 6179 696e 6720 6d61  e, displaying ma
-00000e60: 7869 6d75 6d20 7661 6c75 6573 2c20 656e  ximum values, en
-00000e70: 6162 6c69 6e67 2067 7269 646c 696e 6573  abling gridlines
-00000e80: 2c20 6164 6a75 7374 696e 6720 6c69 6e65  , adjusting line
-00000e90: 2074 7970 6573 2061 6e64 2063 6f6c 6f72   types and color
-00000ea0: 732c 206d 6f64 6966 7969 6e67 2067 7269  s, modifying gri
-00000eb0: 6420 616e 6420 6c61 6265 6c20 6178 6573  d and label axes
-00000ec0: 2c20 616e 6420 6261 636b 6772 6f75 6e64  , and background
-00000ed0: 2063 6f6c 6f72 2e0a 0a0a 352e 20f0 9f93   color....5. ...
-00000ee0: 8920 4572 726f 7220 5072 6f70 6167 6174  . Error Propagat
-00000ef0: 696f 6e0a 2020 202d 2049 6e70 7574 3a20  ion.   - Input: 
-00000f00: 5661 7269 6162 6c65 732c 2074 6865 6972  Variables, their
-00000f10: 2076 616c 7565 732c 2061 6e64 2074 6865   values, and the
-00000f20: 6972 2075 6e63 6572 7461 696e 7469 6573  ir uncertainties
-00000f30: 2e0a 2020 202d 204f 7574 7075 743a 204d  ..   - Output: M
-00000f40: 6561 6e20 7661 6c75 652c 2069 7473 2075  ean value, its u
-00000f50: 6e63 6572 7461 696e 7479 2c20 616e 6420  ncertainty, and 
-00000f60: 7468 6520 7265 7375 6c74 2063 616e 2062  the result can b
-00000f70: 6520 636f 7069 6564 2061 7320 4c61 5465  e copied as LaTe
-00000f80: 5820 636f 6465 2066 6f72 2065 6173 7920  X code for easy 
-00000f90: 696e 636c 7573 696f 6e20 696e 2064 6f63  inclusion in doc
-00000fa0: 756d 656e 7473 2e0a 0a36 2e20 f09f a7aa  uments...6. ....
-00000fb0: 2053 686f 7720 4d6f 6c65 6375 6c65 0a20   Show Molecule. 
-00000fc0: 2020 2d20 496e 7075 743a 2053 4d49 4c45    - Input: SMILE
-00000fd0: 530a 2020 202d 204f 7574 7075 743a 204d  S.   - Output: M
-00000fe0: 6f6c 6563 756c 6172 2073 7472 7563 7475  olecular structu
-00000ff0: 7265 0a0a 5468 6520 6772 6170 6873 2069  re..The graphs i
-00001000: 6e20 7365 6374 696f 6e73 2033 2061 6e64  n sections 3 and
-00001010: 2034 2063 616e 2061 6c73 6f20 696e 636c   4 can also incl
-00001020: 7564 6520 696e 7075 7420 666f 7220 7468  ude input for th
-00001030: 6520 7469 746c 6520 616e 6420 582c 2059  e title and X, Y
-00001040: 2061 7869 7320 6c61 6265 6c73 2e0a 0a23   axis labels...#
-00001050: 2320 f09f a49d 2043 6f6e 7472 6962 7574  # .... Contribut
-00001060: 696e 670a 3c61 2069 643d 2263 6f6e 7472  ing.<a id="contr
-00001070: 6962 7574 696e 6722 3e3c 2f61 3e0a 0a43  ibuting"></a>..C
-00001080: 6f6e 7472 6962 7574 696f 6e73 2061 7265  ontributions are
-00001090: 2077 656c 636f 6d65 2120 546f 2063 6f6e   welcome! To con
-000010a0: 7472 6962 7574 6520 746f 202a 2a54 6f6f  tribute to **Too
-000010b0: 6c73 204b 6974 2a2a 2c20 706c 6561 7365  ls Kit**, please
-000010c0: 2066 6f6c 6c6f 7720 7468 6573 6520 7374   follow these st
-000010d0: 6570 733a 0a0a 312e 202a 2a46 6f72 6b2a  eps:..1. **Fork*
-000010e0: 2a20 7468 6520 7072 6f6a 6563 7420 746f  * the project to
-000010f0: 2079 6f75 7220 4769 7448 7562 2061 6363   your GitHub acc
-00001100: 6f75 6e74 2e0a 322e 2043 7265 6174 6520  ount..2. Create 
-00001110: 6120 6e65 7720 6272 616e 6368 2066 6f72  a new branch for
-00001120: 2079 6f75 7220 6665 6174 7572 6520 6f72   your feature or
-00001130: 2062 7567 2066 6978 3a20 0a20 2020 6060   bug fix: .   ``
-00001140: 6062 6173 680a 2020 2067 6974 2063 6865  `bash.   git che
-00001150: 636b 6f75 7420 2d62 2066 6561 7475 7265  ckout -b feature
-00001160: 2f79 6f75 722d 6665 6174 7572 652d 6e61  /your-feature-na
-00001170: 6d65 0a20 2020 6060 600a 332e 202a 2a43  me.   ```.3. **C
-00001180: 7265 6174 6520 6120 6e65 7720 6272 616e  reate a new bran
-00001190: 6368 2066 6f72 2079 6f75 7220 6665 6174  ch for your feat
-000011a0: 7572 6520 6f72 2062 7567 2066 6978 3a2a  ure or bug fix:*
-000011b0: 2a0a 0a20 2020 2060 6060 6261 7368 0a20  *..    ```bash. 
-000011c0: 2020 2067 6974 2063 6865 636b 6f75 7420     git checkout 
-000011d0: 2d62 2066 6561 7475 7265 2f79 6f75 722d  -b feature/your-
-000011e0: 6665 6174 7572 652d 6e61 6d65 0a20 2020  feature-name.   
-000011f0: 2060 6060 0a0a 342e 202a 2a4d 616b 6520   ```..4. **Make 
-00001200: 796f 7572 2063 6861 6e67 6573 2061 6e64  your changes and
-00001210: 2065 6e73 7572 6520 7468 6579 2061 6468   ensure they adh
-00001220: 6572 6520 746f 2074 6865 2070 726f 6a65  ere to the proje
-00001230: 6374 2773 2063 6f64 696e 6720 636f 6e76  ct's coding conv
-00001240: 656e 7469 6f6e 7320 616e 6420 7374 796c  entions and styl
-00001250: 6520 6775 6964 656c 696e 6573 2e2a 2a0a  e guidelines.**.
-00001260: 0a35 2e20 2a2a 436f 6d6d 6974 2079 6f75  .5. **Commit you
-00001270: 7220 6368 616e 6765 7320 7769 7468 2064  r changes with d
-00001280: 6573 6372 6970 7469 7665 206d 6573 7361  escriptive messa
-00001290: 6765 7320 6578 706c 6169 6e69 6e67 2074  ges explaining t
-000012a0: 6865 2070 7572 706f 7365 206f 6620 796f  he purpose of yo
-000012b0: 7572 2063 6861 6e67 6573 3a2a 2a0a 0a20  ur changes:**.. 
-000012c0: 2020 2060 6060 6261 7368 0a20 2020 2067     ```bash.    g
-000012d0: 6974 2063 6f6d 6d69 7420 2d61 6d20 2741  it commit -am 'A
-000012e0: 6464 2073 6f6d 6520 6665 6174 7572 6527  dd some feature'
-000012f0: 0a20 2020 2060 6060 0a0a 362e 202a 2a50  .    ```..6. **P
-00001300: 7573 6820 796f 7572 2063 6861 6e67 6573  ush your changes
-00001310: 2074 6f20 796f 7572 2062 7261 6e63 6820   to your branch 
-00001320: 6f6e 2079 6f75 7220 666f 726b 6564 2072  on your forked r
-00001330: 6570 6f73 6974 6f72 793a 2a2a 0a0a 2020  epository:**..  
-00001340: 2020 6060 6062 6173 680a 2020 2020 6769    ```bash.    gi
-00001350: 7420 7075 7368 206f 7269 6769 6e20 6665  t push origin fe
-00001360: 6174 7572 652f 796f 7572 2d66 6561 7475  ature/your-featu
-00001370: 7265 2d6e 616d 650a 2020 2020 6060 600a  re-name.    ```.
-00001380: 0a37 2e20 2a2a 4f6e 6365 2079 6f75 2776  .7. **Once you'v
-00001390: 6520 7075 7368 6564 2079 6f75 7220 6368  e pushed your ch
-000013a0: 616e 6765 732c 2079 6f75 2063 616e 206f  anges, you can o
-000013b0: 7065 6e20 6120 5075 6c6c 2052 6571 7565  pen a Pull Reque
-000013c0: 7374 2028 5052 2920 696e 2074 6865 206f  st (PR) in the o
-000013d0: 7269 6769 6e61 6c20 7265 706f 7369 746f  riginal reposito
-000013e0: 7279 2e20 5072 6f76 6964 6520 6120 636c  ry. Provide a cl
-000013f0: 6561 7220 6465 7363 7269 7074 696f 6e20  ear description 
-00001400: 6f66 2074 6865 2063 6861 6e67 6573 2079  of the changes y
-00001410: 6f75 2776 6520 6d61 6465 2069 6e20 7468  ou've made in th
-00001420: 6520 5052 2e2a 2a0a 0a38 2e20 2a2a 4166  e PR.**..8. **Af
-00001430: 7465 7220 7265 7669 6577 696e 6720 796f  ter reviewing yo
-00001440: 7572 2050 522c 2069 6620 6576 6572 7974  ur PR, if everyt
-00001450: 6869 6e67 206c 6f6f 6b73 2067 6f6f 642c  hing looks good,
-00001460: 2069 7420 7769 6c6c 2062 6520 6d65 7267   it will be merg
-00001470: 6564 2069 6e74 6f20 7468 6520 6d61 696e  ed into the main
-00001480: 2072 6570 6f73 6974 6f72 792e 2043 6f6e   repository. Con
-00001490: 6772 6174 756c 6174 696f 6e73 2c20 796f  gratulations, yo
-000014a0: 7527 7665 2073 7563 6365 7373 6675 6c6c  u've successfull
-000014b0: 7920 636f 6e74 7269 6275 7465 6420 746f  y contributed to
-000014c0: 202a 546f 6f6c 7320 4b69 742a 212a 2a0a   *Tools Kit*!**.
-000014d0: 0a54 6861 6e6b 2079 6f75 2066 6f72 2079  .Thank you for y
-000014e0: 6f75 7220 636f 6e74 7269 6275 7469 6f6e  our contribution
-000014f0: 2120 596f 7572 2065 6666 6f72 7473 2068  ! Your efforts h
-00001500: 656c 7020 696d 7072 6f76 6520 7468 6520  elp improve the 
-00001510: 7072 6f6a 6563 7420 666f 7220 6576 6572  project for ever
-00001520: 796f 6e65 2e0a 0a23 2320 f09f 939a 2043  yone...## .... C
-00001530: 6974 6520 5573 0a3c 6120 6964 3d22 6369  ite Us.<a id="ci
-00001540: 7465 2d75 7322 3e3c 2f61 3e0a 0a49 6620  te-us"></a>..If 
-00001550: 796f 7520 7573 6520 546f 6f6c 7320 4b69  you use Tools Ki
-00001560: 7420 696e 2079 6f75 7220 7265 7365 6172  t in your resear
-00001570: 6368 2077 6f72 6b20 6f72 2061 6361 6465  ch work or acade
-00001580: 6d69 6320 7072 6f6a 6563 7473 2c20 7765  mic projects, we
-00001590: 2077 6f75 6c64 2061 7070 7265 6369 6174   would appreciat
-000015a0: 6520 6974 2069 6620 796f 7520 636f 756c  e it if you coul
-000015b0: 6420 6369 7465 2075 732e 2059 6f75 2063  d cite us. You c
-000015c0: 616e 2075 7365 2074 6865 2066 6f6c 6c6f  an use the follo
-000015d0: 7769 6e67 2042 6962 5465 5820 656e 7472  wing BibTeX entr
-000015e0: 793a 0a0a 6060 6062 6962 7465 780a 406d  y:..```bibtex.@m
-000015f0: 6973 637b 7072 6f6a 6563 742d 7070 6368  isc{project-ppch
-00001600: 656d 2d74 6f6f 6c73 2d6b 6974 2c0a 2020  em-tools-kit,.  
-00001610: 7469 746c 6520 3d20 7b50 726f 6a65 6374  title = {Project
-00001620: 2d70 7063 6865 6d2d 746f 6f6c 732d 6b69  -ppchem-tools-ki
-00001630: 747d 2c0a 2020 6175 7468 6f72 203d 207b  t},.  author = {
-00001640: 7b4d c3a9 6c6f c3a9 2045 6e7a 696e 6765  {M..lo.. Enzinge
-00001650: 7220 2620 53c3 a962 6173 7469 656e 2047  r & S..bastien G
-00001660: 7275 6e62 6572 677d 7d2c 0a20 2079 6561  runberg}},.  yea
-00001670: 7220 3d20 7b32 3032 347d 2c0a 2020 7075  r = {2024},.  pu
-00001680: 626c 6973 6865 7220 3d20 7b47 6974 4875  blisher = {GitHu
-00001690: 627d 2c0a 2020 6a6f 7572 6e61 6c20 3d20  b},.  journal = 
-000016a0: 7b47 6974 4875 6220 5265 706f 7369 746f  {GitHub Reposito
-000016b0: 7279 7d2c 0a20 2068 6f77 7075 626c 6973  ry},.  howpublis
-000016c0: 6865 6420 3d20 7b5c 7572 6c7b 6874 7470  hed = {\url{http
-000016d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f75  s://github.com/u
-000016e0: 7365 726e 616d 652f 5072 6f6a 6563 742d  sername/Project-
-000016f0: 7070 6368 656d 2d74 6f6f 6c73 2d6b 6974  ppchem-tools-kit
-00001700: 7d7d 0a7d 0a60 6060 0a0a 2323 2320 4368  }}.}.```..### Ch
-00001710: 6963 6167 6f20 5374 796c 650a 6060 6062  icago Style.```b
-00001720: 6173 680a 456e 7a69 6e67 6572 2c20 4dc3  ash.Enzinger, M.
-00001730: a96c 6fc3 a92c 2061 6e64 2053 c3a9 6261  .lo.., and S..ba
-00001740: 7374 6965 6e20 4772 756e 6265 7267 2e20  stien Grunberg. 
-00001750: 3230 3234 2e20 5072 6f6a 6563 742d 7070  2024. Project-pp
-00001760: 6368 656d 2d74 6f6f 6c73 2d6b 6974 2e20  chem-tools-kit. 
-00001770: 436f 6d70 7574 6572 2073 6f66 7477 6172  Computer softwar
-00001780: 652e 2047 6974 4875 622e 2068 7474 7073  e. GitHub. https
-00001790: 3a2f 2f67 6974 6875 622e 636f 6d2f 7573  ://github.com/us
-000017a0: 6572 6e61 6d65 2f50 726f 6a65 6374 2d70  ername/Project-p
-000017b0: 7063 6865 6d2d 746f 6f6c 732d 6b69 742e  pchem-tools-kit.
-000017c0: 6020 0a60 6060 0a23 2320 f09f 939c 204c  ` .```.## .... L
-000017d0: 6963 656e 7365 0a3c 6120 6964 3d22 6c69  icense.<a id="li
-000017e0: 6365 6e73 6522 3e3c 2f61 3e0a 0a54 6869  cense"></a>..Thi
-000017f0: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
-00001800: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
-00001810: 4d49 5420 4c69 6365 6e73 652e 2053 6565  MIT License. See
-00001820: 2074 6865 204c 4943 454e 5345 2066 696c   the LICENSE fil
-00001830: 6520 666f 7220 6465 7461 696c 732e 0a0a  e for details...
-00001840: 2323 20f0 9f93 b820 5363 7265 656e 7368  ## .... Screensh
-00001850: 6f74 730a 3c61 2069 643d 2273 6372 6565  ots.<a id="scree
-00001860: 6e73 686f 7473 223e 3c2f 613e 0a0a       nshots"></a>..
+00000000: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000010: 7222 3e0a 2020 203c 696d 6720 7769 6474  r">.   <img widt
+00000020: 683d 2231 3234 3522 2061 6c74 3d22 6c6f  h="1245" alt="lo
+00000030: 676f 5f70 726f 6a65 6374 2220 7372 633d  go_project" src=
+00000040: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000050: 636f 6d2f 7367 7275 6e62 6572 2f50 726f  com/sgrunber/Pro
+00000060: 6a65 6374 2d70 7063 6865 6d2d 746f 6f6c  ject-ppchem-tool
+00000070: 732d 6b69 742f 7261 772f 6d61 696e 2f64  s-kit/raw/main/d
+00000080: 6f63 732f 736f 7572 6365 2f5f 7374 6174  ocs/source/_stat
+00000090: 6963 2f69 6d61 6765 732f 6c6f 676f 5f70  ic/images/logo_p
+000000a0: 726f 6a65 6374 2e70 6e67 223e 0a0a 203c  roject.png">.. <
+000000b0: 2f70 3e0a 0a0a 0a0a 203c 6831 2061 6c69  /p>..... <h1 ali
+000000c0: 676e 3d22 6365 6e74 6572 223e f09f a7b0  gn="center">....
+000000d0: 2054 6f6f 6c73 204b 6974 3c2f 6831 3e0a   Tools Kit</h1>.
+000000e0: 0a20 3c70 2061 6c69 676e 3d22 6365 6e74  . <p align="cent
+000000f0: 6572 223e 0a20 203c 6120 6872 6566 3d22  er">.  <a href="
+00000100: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000110: 6f6d 2f73 6772 756e 6265 722f 5072 6f6a  om/sgrunber/Proj
+00000120: 6563 742d 7070 6368 656d 2d74 6f6f 6c73  ect-ppchem-tools
+00000130: 2d6b 6974 2f61 6374 696f 6e73 223e 3c69  -kit/actions"><i
+00000140: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000150: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000160: 6164 6765 2f62 7569 6c64 2d70 6173 7369  adge/build-passi
+00000170: 6e67 2d62 7269 6768 7467 7265 656e 2220  ng-brightgreen" 
+00000180: 616c 743d 2242 7569 6c64 2053 7461 7475  alt="Build Statu
+00000190: 7322 3e3c 2f61 3e0a 2020 3c61 2068 7265  s"></a>.  <a hre
+000001a0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+000001b0: 622e 636f 6d2f 7367 7275 6e62 6572 2f50  b.com/sgrunber/P
+000001c0: 726f 6a65 6374 2d70 7063 6865 6d2d 746f  roject-ppchem-to
+000001d0: 6f6c 732d 6b69 7422 3e3c 696d 6720 7372  ols-kit"><img sr
+000001e0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000001f0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000200: 636f 7665 7261 6765 2d39 3525 3235 2d62  coverage-95%25-b
+00000210: 7269 6768 7467 7265 656e 2220 616c 743d  rightgreen" alt=
+00000220: 2243 6f76 6572 6167 6522 3e3c 2f61 3e0a  "Coverage"></a>.
+00000230: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000240: 3a2f 2f67 6974 6875 622e 636f 6d2f 7367  ://github.com/sg
+00000250: 7275 6e62 6572 2f50 726f 6a65 6374 2d70  runber/Project-p
+00000260: 7063 6865 6d2d 746f 6f6c 732d 6b69 742f  pchem-tools-kit/
+00000270: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+00000280: 4522 3e3c 696d 6720 7372 633d 2268 7474  E"><img src="htt
+00000290: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000002a0: 2e69 6f2f 6261 6467 652f 6c69 6365 6e73  .io/badge/licens
+000002b0: 652d 4d49 542d 626c 7565 2220 616c 743d  e-MIT-blue" alt=
+000002c0: 224c 6963 656e 7365 223e 3c2f 613e 0a3c  "License"></a>.<
+000002d0: 2f70 3e0a 0a23 2320 f09f 9396 2044 6573  /p>..## .... Des
+000002e0: 6372 6970 7469 6f6e 0a54 6865 202a 2a54  cription.The **T
+000002f0: 6f6f 6c73 204b 6974 2a2a 2070 6163 6b61  ools Kit** packa
+00000300: 6765 2061 6c6c 6f77 7320 6368 656d 6973  ge allows chemis
+00000310: 7472 7920 7374 7564 656e 7473 2074 6f20  try students to 
+00000320: 6669 6e64 2062 6173 6963 2069 6e66 6f72  find basic infor
+00000330: 6d61 7469 6f6e 206f 6e20 6d6f 6c65 6375  mation on molecu
+00000340: 6c65 7320 616e 6420 7072 6f76 6964 6573  les and provides
+00000350: 2065 6173 7920 6163 6365 7373 2074 6f20   easy access to 
+00000360: 736f 6d65 2067 7261 7068 7320 616e 6420  some graphs and 
+00000370: 6361 6c63 756c 6174 696f 6e73 2072 6571  calculations req
+00000380: 7569 7265 6420 696e 2065 7870 6572 696d  uired in experim
+00000390: 656e 7461 6c20 6c61 626f 7261 746f 7269  ental laboratori
+000003a0: 6573 2e0a 0a2a 2af0 9f8c 9920 4e6f 7465  es...**.... Note
+000003b0: 2a2a 3a20 466f 7220 616e 2061 6573 7468  **: For an aesth
+000003c0: 6574 6963 616c 6c79 2070 6c65 6173 696e  etically pleasin
+000003d0: 6720 6578 7065 7269 656e 6365 2c20 6974  g experience, it
+000003e0: 2069 7320 7265 636f 6d6d 656e 6465 6420   is recommended 
+000003f0: 746f 2075 7365 2074 6865 2064 6172 6b20  to use the dark 
+00000400: 6d6f 6465 2069 6e74 6572 6661 6365 2069  mode interface i
+00000410: 6620 796f 7520 6172 6520 6f6e 2061 204d  f you are on a M
+00000420: 6163 206f 7220 616e 7920 6f74 6865 7220  ac or any other 
+00000430: 706c 6174 666f 726d 2074 6861 7420 7375  platform that su
+00000440: 7070 6f72 7473 2069 742e 0a0a 0a23 2320  pports it....## 
+00000450: f09f 939a 2054 6162 6c65 206f 6620 436f  .... Table of Co
+00000460: 6e74 656e 7473 0a2d 205b 496e 7374 616c  ntents.- [Instal
+00000470: 6c61 7469 6f6e 5d28 23ef b88f 2d69 6e73  lation](#...-ins
+00000480: 7461 6c6c 6174 696f 6e29 0a2d 205b 5573  tallation).- [Us
+00000490: 6167 655d 2823 efb8 8f2d 7573 6167 6529  age](#...-usage)
+000004a0: 0a2d 205b 4665 6174 7572 6573 5d28 23ef  .- [Features](#.
+000004b0: b88f 2d66 6561 7475 7265 7329 0a2d 205b  ..-features).- [
+000004c0: 436f 6e74 7269 6275 7469 6e67 5d28 23ef  Contributing](#.
+000004d0: b88f 2d63 6f6e 7472 6962 7574 696e 6729  ..-contributing)
+000004e0: 0a2d 205b 4369 7465 2055 735d 2823 efb8  .- [Cite Us](#..
+000004f0: 8f2d 6369 7465 2d75 7329 0a2d 205b 4c69  .-cite-us).- [Li
+00000500: 6365 6e73 655d 2823 efb8 8f2d 6c69 6365  cense](#...-lice
+00000510: 6e73 6529 0a2d 205b 5363 7265 656e 7368  nse).- [Screensh
+00000520: 6f74 735d 2823 efb8 8f2d 7363 7265 656e  ots](#...-screen
+00000530: 7368 6f74 7329 0a0a 2323 20f0 9f9b a0ef  shots)..## .....
+00000540: b88f 2049 6e73 7461 6c6c 6174 696f 6e0a  .. Installation.
+00000550: 3c61 2069 643d 2269 6e73 7461 6c6c 6174  <a id="installat
+00000560: 696f 6e22 3e3c 2f61 3e0a 2323 2320 312e  ion"></a>.### 1.
+00000570: 20f0 9f8d b420 466f 726b 2074 6865 2052   .... Fork the R
+00000580: 6570 6f73 6974 6f72 790a 546f 2073 7461  epository.To sta
+00000590: 7274 2c20 666f 726b 2074 6865 2072 6570  rt, fork the rep
+000005a0: 6f73 6974 6f72 7920 746f 2079 6f75 7220  ository to your 
+000005b0: 6f77 6e20 4769 7448 7562 2061 6363 6f75  own GitHub accou
+000005c0: 6e74 2e20 200a 546f 2064 6f20 736f 2c20  nt.  .To do so, 
+000005d0: 6e61 7669 6761 7465 2074 6f20 7468 6520  navigate to the 
+000005e0: 7265 706f 7369 746f 7279 2070 6167 6520  repository page 
+000005f0: 616e 6420 636c 6963 6b20 7468 6520 2a22  and click the *"
+00000600: 466f 726b 222a 2062 7574 746f 6e2e 2054  Fork"* button. T
+00000610: 6865 2072 6570 6f73 6974 6f72 7920 7769  he repository wi
+00000620: 6c6c 2074 6865 6e20 6265 2063 6f70 6965  ll then be copie
+00000630: 6420 746f 2079 6f75 7220 6163 636f 756e  d to your accoun
+00000640: 742c 2061 6e64 2079 6f75 2077 696c 6c20  t, and you will 
+00000650: 6265 2061 626c 6520 746f 2061 6363 6573  be able to acces
+00000660: 7320 6974 2e0a 0a23 2323 2032 2e20 f09f  s it...### 2. ..
+00000670: 93a5 2043 6c6f 6e65 2074 6865 2052 6570  .. Clone the Rep
+00000680: 6f73 6974 6f72 790a 4e65 7874 2c20 636c  ository.Next, cl
+00000690: 6f6e 6520 7468 6520 7265 706f 7369 746f  one the reposito
+000006a0: 7279 2075 7369 6e67 2074 6865 2066 6f6c  ry using the fol
+000006b0: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2028  lowing command (
+000006c0: 7265 706c 6163 6520 2a75 7365 726e 616d  replace *usernam
+000006d0: 652a 2077 6974 6820 796f 7572 2047 6974  e* with your Git
+000006e0: 4875 6220 7573 6572 6e61 6d65 293a 0a0a  Hub username):..
+000006f0: 6060 6062 6173 680a 6769 7420 636c 6f6e  ```bash.git clon
+00000700: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
+00000710: 2e63 6f6d 2f2a 7573 6572 6e61 6d65 2a2f  .com/*username*/
+00000720: 5072 6f6a 6563 742d 7070 6368 656d 2d74  Project-ppchem-t
+00000730: 6f6f 6c73 2d6b 6974 2e67 6974 0a60 6060  ools-kit.git.```
+00000740: 0a0a 2323 2320 332e 20e2 ac87 efb8 8f20  ..### 3. ...... 
+00000750: 496e 7374 616c 6c20 7769 7468 2070 6970  Install with pip
+00000760: 0a59 6f75 2063 616e 2061 6c73 6f20 696e  .You can also in
+00000770: 7374 616c 6c20 546f 6f6c 7320 4b69 7420  stall Tools Kit 
+00000780: 7573 696e 6720 7069 703a 0a0a 6060 6062  using pip:..```b
+00000790: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+000007a0: 5072 6f6a 6563 745f 7070 6368 656d 2d74  Project_ppchem-t
+000007b0: 6f6f 6c73 2d6b 6974 0a60 6060 0a0a 2323  ools-kit.```..##
+000007c0: 20f0 9f9a 8020 5573 6167 650a 3c61 2069   .... Usage.<a i
+000007d0: 643d 2275 7361 6765 223e 3c2f 613e 0a0a  d="usage"></a>..
+000007e0: 546f 2075 7365 2054 6f6f 6c73 204b 6974  To use Tools Kit
+000007f0: 2061 6e64 2061 6363 6573 7320 6974 7320   and access its 
+00000800: 6665 6174 7572 6573 2c20 666f 6c6c 6f77  features, follow
+00000810: 2074 6865 7365 2073 7465 7073 2061 6674   these steps aft
+00000820: 6572 2063 6c6f 6e69 6e67 2074 6865 2072  er cloning the r
+00000830: 6570 6f73 6974 6f72 793a 0a0a 2323 2320  epository:..### 
+00000840: 5573 696e 6720 4a75 7079 7465 7220 4e6f  Using Jupyter No
+00000850: 7465 626f 6f6b 3a0a 0a31 2e20 4c61 756e  tebook:..1. Laun
+00000860: 6368 204a 7570 7974 6572 204e 6f74 6562  ch Jupyter Noteb
+00000870: 6f6f 6b20 6279 206e 6176 6967 6174 696e  ook by navigatin
+00000880: 6720 746f 2074 6865 2063 6c6f 6e65 6420  g to the cloned 
+00000890: 7265 706f 7369 746f 7279 2064 6972 6563  repository direc
+000008a0: 746f 7279 2069 6e20 796f 7572 2074 6572  tory in your ter
+000008b0: 6d69 6e61 6c20 616e 6420 7275 6e6e 696e  minal and runnin
+000008c0: 6720 7468 6520 636f 6d6d 616e 643a 0a20  g the command:. 
+000008d0: 2020 6060 6062 6173 680a 2020 206a 7570    ```bash.   jup
+000008e0: 7974 6572 206e 6f74 6562 6f6f 6b0a 2020  yter notebook.  
+000008f0: 2060 6060 0a32 2e20 496e 2074 6865 204a   ```.2. In the J
+00000900: 7570 7974 6572 204e 6f74 6562 6f6f 6b20  upyter Notebook 
+00000910: 696e 7465 7266 6163 652c 206e 6176 6967  interface, navig
+00000920: 6174 6520 746f 2074 6865 2060 6e6f 7465  ate to the `note
+00000930: 626f 6f6b 7360 2064 6972 6563 746f 7279  books` directory
+00000940: 2e0a 0a33 2e20 4f70 656e 2074 6865 206e  ...3. Open the n
+00000950: 6f74 6562 6f6f 6b20 6e61 6d65 6420 6070  otebook named `p
+00000960: 726f 6a65 6374 5f72 6570 6f72 742e 6970  roject_report.ip
+00000970: 796e 6260 2e0a 0a34 2e20 466f 6c6c 6f77  ynb`...4. Follow
+00000980: 2074 6865 2069 6e73 7472 7563 7469 6f6e   the instruction
+00000990: 7320 696e 7369 6465 2074 6865 206e 6f74  s inside the not
+000009a0: 6562 6f6f 6b20 746f 2069 6e74 6572 6163  ebook to interac
+000009b0: 7420 7769 7468 2074 6865 2054 6f6f 6c73  t with the Tools
+000009c0: 204b 6974 2069 6e74 6572 6661 6365 2061   Kit interface a
+000009d0: 6e64 2075 7469 6c69 7a65 2069 7473 2066  nd utilize its f
+000009e0: 6561 7475 7265 7320 666f 7220 6d6f 6c65  eatures for mole
+000009f0: 6375 6c65 2061 6e61 6c79 7369 732c 2067  cule analysis, g
+00000a00: 7261 7068 2070 6c6f 7474 696e 672c 2065  raph plotting, e
+00000a10: 7272 6f72 2063 616c 6375 6c61 7469 6f6e  rror calculation
+00000a20: 2c20 616e 6420 6d6f 7265 2e0a 5468 6973  , and more..This
+00000a30: 206e 6f74 6562 6f6f 6b20 7072 6f76 6964   notebook provid
+00000a40: 6573 2061 6e20 696e 7465 7261 6374 6976  es an interactiv
+00000a50: 6520 656e 7669 726f 6e6d 656e 7420 666f  e environment fo
+00000a60: 7220 636f 6e76 656e 6965 6e74 2075 7361  r convenient usa
+00000a70: 6765 206f 6620 546f 6f6c 7320 4b69 7420  ge of Tools Kit 
+00000a80: 6469 7265 6374 6c79 2077 6974 6869 6e20  directly within 
+00000a90: 5669 7375 616c 2053 7475 6469 6f20 436f  Visual Studio Co
+00000aa0: 6465 2e0a 0a0a 2323 2320 5573 6167 6520  de....### Usage 
+00000ab0: 7769 7468 2056 6973 7561 6c20 5374 7564  with Visual Stud
+00000ac0: 696f 2043 6f64 653a 0a0a 312e 204f 7065  io Code:..1. Ope
+00000ad0: 6e20 5669 7375 616c 2053 7475 6469 6f20  n Visual Studio 
+00000ae0: 436f 6465 2061 6e64 206e 6176 6967 6174  Code and navigat
+00000af0: 6520 746f 2074 6865 2063 6c6f 6e65 6420  e to the cloned 
+00000b00: 6469 7265 6374 6f72 792e 0a0a 322e 2049  directory...2. I
+00000b10: 6e73 7461 6c6c 2074 6865 204a 7570 7974  nstall the Jupyt
+00000b20: 6572 2065 7874 656e 7369 6f6e 2069 6620  er extension if 
+00000b30: 6e6f 7420 616c 7265 6164 7920 696e 7374  not already inst
+00000b40: 616c 6c65 642e 2059 6f75 2063 616e 2064  alled. You can d
+00000b50: 6f20 7468 6973 2062 7920 7365 6172 6368  o this by search
+00000b60: 696e 6720 666f 7220 224a 7570 7974 6572  ing for "Jupyter
+00000b70: 2220 696e 2074 6865 2045 7874 656e 7369  " in the Extensi
+00000b80: 6f6e 7320 7669 6577 2028 4374 726c 2b53  ons view (Ctrl+S
+00000b90: 6869 6674 2b58 2920 616e 6420 696e 7374  hift+X) and inst
+00000ba0: 616c 6c69 6e67 2074 6865 2022 5079 7468  alling the "Pyth
+00000bb0: 6f6e 2220 6578 7465 6e73 696f 6e20 7061  on" extension pa
+00000bc0: 636b 2e0a 0a33 2e20 4f70 656e 2074 6865  ck...3. Open the
+00000bd0: 2060 6e6f 7465 626f 6f6b 7360 2064 6972   `notebooks` dir
+00000be0: 6563 746f 7279 2069 6e20 5669 7375 616c  ectory in Visual
+00000bf0: 2053 7475 6469 6f20 436f 6465 2e0a 0a34   Studio Code...4
+00000c00: 2e20 4f70 656e 2074 6865 206e 6f74 6562  . Open the noteb
+00000c10: 6f6f 6b20 6e61 6d65 6420 6070 726f 6a65  ook named `proje
+00000c20: 6374 5f72 6570 6f72 742e 6970 796e 6260  ct_report.ipynb`
+00000c30: 2e0a 0a35 2e20 466f 6c6c 6f77 2074 6865  ...5. Follow the
+00000c40: 2069 6e73 7472 7563 7469 6f6e 7320 696e   instructions in
+00000c50: 7369 6465 2074 6865 206e 6f74 6562 6f6f  side the noteboo
+00000c60: 6b20 746f 2069 6e74 6572 6163 7420 7769  k to interact wi
+00000c70: 7468 2074 6865 2054 6f6f 6c73 204b 6974  th the Tools Kit
+00000c80: 2069 6e74 6572 6661 6365 2061 6e64 2075   interface and u
+00000c90: 7469 6c69 7a65 2069 7473 2066 6561 7475  tilize its featu
+00000ca0: 7265 7320 666f 7220 6d6f 6c65 6375 6c65  res for molecule
+00000cb0: 2061 6e61 6c79 7369 732c 2067 7261 7068   analysis, graph
+00000cc0: 2070 6c6f 7474 696e 672c 2065 7272 6f72   plotting, error
+00000cd0: 2063 616c 6375 6c61 7469 6f6e 2c20 616e   calculation, an
+00000ce0: 6420 6d6f 7265 2e0a 5468 6973 206e 6f74  d more..This not
+00000cf0: 6562 6f6f 6b20 7072 6f76 6964 6573 2061  ebook provides a
+00000d00: 6e20 696e 7465 7261 6374 6976 6520 656e  n interactive en
+00000d10: 7669 726f 6e6d 656e 7420 666f 7220 636f  vironment for co
+00000d20: 6e76 656e 6965 6e74 2075 7361 6765 206f  nvenient usage o
+00000d30: 6620 546f 6f6c 7320 4b69 7420 7769 7468  f Tools Kit with
+00000d40: 204a 7570 7974 6572 204e 6f74 6562 6f6f   Jupyter Noteboo
+00000d50: 6b2e 0a0a 2323 20f0 9fa7 aa20 4665 6174  k...## .... Feat
+00000d60: 7572 6573 0a0a 312e 20f0 9fa7 ac20 4d6f  ures..1. .... Mo
+00000d70: 6c65 6375 6c65 204e 616d 650a 2020 202d  lecule Name.   -
+00000d80: 2049 6e70 7574 3a20 5261 7720 666f 726d   Input: Raw form
+00000d90: 756c 6120 6f66 2074 6865 206d 6f6c 6563  ula of the molec
+00000da0: 756c 650a 2020 202d 204f 7574 7075 743a  ule.   - Output:
+00000db0: 2053 4d49 4c45 5320 6f66 2074 6865 206d   SMILES of the m
+00000dc0: 6f6c 6563 756c 650a 0a32 2e20 e29a 96ef  olecule..2. ....
+00000dd0: b88f 204d 6f6c 6563 756c 6172 2057 6569  .. Molecular Wei
+00000de0: 6768 740a 2020 202d 2049 6e70 7574 3a20  ght.   - Input: 
+00000df0: 534d 494c 4553 206f 6620 7468 6520 6d6f  SMILES of the mo
+00000e00: 6c65 6375 6c65 0a20 2020 2d20 4f75 7470  lecule.   - Outp
+00000e10: 7574 3a20 436f 7272 6573 706f 6e64 696e  ut: Correspondin
+00000e20: 6720 6d6f 6c61 7220 6d61 7373 2069 6e20  g molar mass in 
+00000e30: 672f 6d6f 6c0a 0a33 2e20 f09f 9388 204c  g/mol..3. .... L
+00000e40: 696e 6561 7220 5265 6772 6573 7369 6f6e  inear Regression
+00000e50: 0a20 2020 2d20 496e 7075 743a 2045 7863  .   - Input: Exc
+00000e60: 656c 2064 6f63 756d 656e 7420 2869 6d70  el document (imp
+00000e70: 6f72 7465 6420 6279 2070 7265 7373 696e  orted by pressin
+00000e80: 6720 7468 6520 4272 6f77 7365 2062 7574  g the Browse but
+00000e90: 746f 6e29 0a20 2020 2d20 4f75 7470 7574  ton).   - Output
+00000ea0: 3a20 4c69 6e65 6172 2072 6567 7265 7373  : Linear regress
+00000eb0: 696f 6e20 6772 6170 6820 7769 7468 2074  ion graph with t
+00000ec0: 6865 2052 3c73 7570 3e32 3c2f 7375 703e  he R<sup>2</sup>
+00000ed0: 2076 616c 7565 0a0a 342e 20f0 9f93 8a20   value..4. .... 
+00000ee0: 4772 6170 6820 4d61 6b65 720a 2020 202d  Graph Maker.   -
+00000ef0: 2049 6e70 7574 3a20 4578 6365 6c20 646f   Input: Excel do
+00000f00: 6375 6d65 6e74 2077 6974 6820 7820 616e  cument with x an
+00000f10: 6420 7920 7661 6c75 6573 2061 7272 616e  d y values arran
+00000f20: 6765 6420 696e 2074 776f 2063 6f6c 756d  ged in two colum
+00000f30: 6e73 0a20 2020 2d20 4f75 7470 7574 3a20  ns.   - Output: 
+00000f40: 4772 6170 6820 706c 6f74 7469 6e67 2061  Graph plotting a
+00000f50: 6c6c 2076 616c 7565 730a 2020 2020 2020  ll values.      
+00000f60: 2d20 4f70 7469 6f6e 733a 2054 6865 2067  - Options: The g
+00000f70: 7261 7068 2061 6c6c 6f77 7320 6375 7374  raph allows cust
+00000f80: 6f6d 697a 6174 696f 6e20 6f66 2076 6172  omization of var
+00000f90: 696f 7573 2070 6172 616d 6574 6572 7320  ious parameters 
+00000fa0: 7375 6368 2061 7320 6368 616e 6769 6e67  such as changing
+00000fb0: 2073 6361 6c65 732c 2061 7869 7320 6c61   scales, axis la
+00000fc0: 6265 6c73 2c20 7469 746c 652c 2064 6973  bels, title, dis
+00000fd0: 706c 6179 696e 6720 6d61 7869 6d75 6d20  playing maximum 
+00000fe0: 7661 6c75 6573 2c20 656e 6162 6c69 6e67  values, enabling
+00000ff0: 2067 7269 646c 696e 6573 2c20 6164 6a75   gridlines, adju
+00001000: 7374 696e 6720 6c69 6e65 2074 7970 6573  sting line types
+00001010: 2061 6e64 2063 6f6c 6f72 732c 206d 6f64   and colors, mod
+00001020: 6966 7969 6e67 2067 7269 6420 616e 6420  ifying grid and 
+00001030: 6c61 6265 6c20 6178 6573 2c20 616e 6420  label axes, and 
+00001040: 6261 636b 6772 6f75 6e64 2063 6f6c 6f72  background color
+00001050: 2e0a 0a0a 352e 20f0 9f93 8920 4572 726f  ....5. .... Erro
+00001060: 7220 5072 6f70 6167 6174 696f 6e0a 2020  r Propagation.  
+00001070: 202d 2049 6e70 7574 3a20 5661 7269 6162   - Input: Variab
+00001080: 6c65 732c 2074 6865 6972 2076 616c 7565  les, their value
+00001090: 732c 2061 6e64 2074 6865 6972 2075 6e63  s, and their unc
+000010a0: 6572 7461 696e 7469 6573 2e0a 2020 202d  ertainties..   -
+000010b0: 204f 7574 7075 743a 204d 6561 6e20 7661   Output: Mean va
+000010c0: 6c75 652c 2069 7473 2075 6e63 6572 7461  lue, its uncerta
+000010d0: 696e 7479 2c20 616e 6420 7468 6520 7265  inty, and the re
+000010e0: 7375 6c74 2063 616e 2062 6520 636f 7069  sult can be copi
+000010f0: 6564 2061 7320 4c61 5465 5820 636f 6465  ed as LaTeX code
+00001100: 2066 6f72 2065 6173 7920 696e 636c 7573   for easy inclus
+00001110: 696f 6e20 696e 2064 6f63 756d 656e 7473  ion in documents
+00001120: 2e0a 0a36 2e20 f09f a7aa 2053 686f 7720  ...6. .... Show 
+00001130: 4d6f 6c65 6375 6c65 0a20 2020 2d20 496e  Molecule.   - In
+00001140: 7075 743a 2053 4d49 4c45 530a 2020 202d  put: SMILES.   -
+00001150: 204f 7574 7075 743a 204d 6f6c 6563 756c   Output: Molecul
+00001160: 6172 2073 7472 7563 7475 7265 0a0a 5468  ar structure..Th
+00001170: 6520 6772 6170 6873 2069 6e20 7365 6374  e graphs in sect
+00001180: 696f 6e73 2033 2061 6e64 2034 2063 616e  ions 3 and 4 can
+00001190: 2061 6c73 6f20 696e 636c 7564 6520 696e   also include in
+000011a0: 7075 7420 666f 7220 7468 6520 7469 746c  put for the titl
+000011b0: 6520 616e 6420 582c 2059 2061 7869 7320  e and X, Y axis 
+000011c0: 6c61 6265 6c73 2e0a 0a23 2320 f09f a49d  labels...## ....
+000011d0: 2043 6f6e 7472 6962 7574 696e 670a 3c61   Contributing.<a
+000011e0: 2069 643d 2263 6f6e 7472 6962 7574 696e   id="contributin
+000011f0: 6722 3e3c 2f61 3e0a 0a43 6f6e 7472 6962  g"></a>..Contrib
+00001200: 7574 696f 6e73 2061 7265 2077 656c 636f  utions are welco
+00001210: 6d65 2120 546f 2063 6f6e 7472 6962 7574  me! To contribut
+00001220: 6520 746f 202a 2a54 6f6f 6c73 204b 6974  e to **Tools Kit
+00001230: 2a2a 2c20 706c 6561 7365 2066 6f6c 6c6f  **, please follo
+00001240: 7720 7468 6573 6520 7374 6570 733a 0a0a  w these steps:..
+00001250: 312e 202a 2a46 6f72 6b2a 2a20 7468 6520  1. **Fork** the 
+00001260: 7072 6f6a 6563 7420 746f 2079 6f75 7220  project to your 
+00001270: 4769 7448 7562 2061 6363 6f75 6e74 2e0a  GitHub account..
+00001280: 322e 2043 7265 6174 6520 6120 6e65 7720  2. Create a new 
+00001290: 6272 616e 6368 2066 6f72 2079 6f75 7220  branch for your 
+000012a0: 6665 6174 7572 6520 6f72 2062 7567 2066  feature or bug f
+000012b0: 6978 3a20 0a20 2020 6060 6062 6173 680a  ix: .   ```bash.
+000012c0: 2020 2067 6974 2063 6865 636b 6f75 7420     git checkout 
+000012d0: 2d62 2066 6561 7475 7265 2f79 6f75 722d  -b feature/your-
+000012e0: 6665 6174 7572 652d 6e61 6d65 0a20 2020  feature-name.   
+000012f0: 6060 600a 332e 202a 2a43 7265 6174 6520  ```.3. **Create 
+00001300: 6120 6e65 7720 6272 616e 6368 2066 6f72  a new branch for
+00001310: 2079 6f75 7220 6665 6174 7572 6520 6f72   your feature or
+00001320: 2062 7567 2066 6978 3a2a 2a0a 0a20 2020   bug fix:**..   
+00001330: 2060 6060 6261 7368 0a20 2020 2067 6974   ```bash.    git
+00001340: 2063 6865 636b 6f75 7420 2d62 2066 6561   checkout -b fea
+00001350: 7475 7265 2f79 6f75 722d 6665 6174 7572  ture/your-featur
+00001360: 652d 6e61 6d65 0a20 2020 2060 6060 0a0a  e-name.    ```..
+00001370: 342e 202a 2a4d 616b 6520 796f 7572 2063  4. **Make your c
+00001380: 6861 6e67 6573 2061 6e64 2065 6e73 7572  hanges and ensur
+00001390: 6520 7468 6579 2061 6468 6572 6520 746f  e they adhere to
+000013a0: 2074 6865 2070 726f 6a65 6374 2773 2063   the project's c
+000013b0: 6f64 696e 6720 636f 6e76 656e 7469 6f6e  oding convention
+000013c0: 7320 616e 6420 7374 796c 6520 6775 6964  s and style guid
+000013d0: 656c 696e 6573 2e2a 2a0a 0a35 2e20 2a2a  elines.**..5. **
+000013e0: 436f 6d6d 6974 2079 6f75 7220 6368 616e  Commit your chan
+000013f0: 6765 7320 7769 7468 2064 6573 6372 6970  ges with descrip
+00001400: 7469 7665 206d 6573 7361 6765 7320 6578  tive messages ex
+00001410: 706c 6169 6e69 6e67 2074 6865 2070 7572  plaining the pur
+00001420: 706f 7365 206f 6620 796f 7572 2063 6861  pose of your cha
+00001430: 6e67 6573 3a2a 2a0a 0a20 2020 2060 6060  nges:**..    ```
+00001440: 6261 7368 0a20 2020 2067 6974 2063 6f6d  bash.    git com
+00001450: 6d69 7420 2d61 6d20 2741 6464 2073 6f6d  mit -am 'Add som
+00001460: 6520 6665 6174 7572 6527 0a20 2020 2060  e feature'.    `
+00001470: 6060 0a0a 362e 202a 2a50 7573 6820 796f  ``..6. **Push yo
+00001480: 7572 2063 6861 6e67 6573 2074 6f20 796f  ur changes to yo
+00001490: 7572 2062 7261 6e63 6820 6f6e 2079 6f75  ur branch on you
+000014a0: 7220 666f 726b 6564 2072 6570 6f73 6974  r forked reposit
+000014b0: 6f72 793a 2a2a 0a0a 2020 2020 6060 6062  ory:**..    ```b
+000014c0: 6173 680a 2020 2020 6769 7420 7075 7368  ash.    git push
+000014d0: 206f 7269 6769 6e20 6665 6174 7572 652f   origin feature/
+000014e0: 796f 7572 2d66 6561 7475 7265 2d6e 616d  your-feature-nam
+000014f0: 650a 2020 2020 6060 600a 0a37 2e20 2a2a  e.    ```..7. **
+00001500: 4f6e 6365 2079 6f75 2776 6520 7075 7368  Once you've push
+00001510: 6564 2079 6f75 7220 6368 616e 6765 732c  ed your changes,
+00001520: 2079 6f75 2063 616e 206f 7065 6e20 6120   you can open a 
+00001530: 5075 6c6c 2052 6571 7565 7374 2028 5052  Pull Request (PR
+00001540: 2920 696e 2074 6865 206f 7269 6769 6e61  ) in the origina
+00001550: 6c20 7265 706f 7369 746f 7279 2e20 5072  l repository. Pr
+00001560: 6f76 6964 6520 6120 636c 6561 7220 6465  ovide a clear de
+00001570: 7363 7269 7074 696f 6e20 6f66 2074 6865  scription of the
+00001580: 2063 6861 6e67 6573 2079 6f75 2776 6520   changes you've 
+00001590: 6d61 6465 2069 6e20 7468 6520 5052 2e2a  made in the PR.*
+000015a0: 2a0a 0a38 2e20 2a2a 4166 7465 7220 7265  *..8. **After re
+000015b0: 7669 6577 696e 6720 796f 7572 2050 522c  viewing your PR,
+000015c0: 2069 6620 6576 6572 7974 6869 6e67 206c   if everything l
+000015d0: 6f6f 6b73 2067 6f6f 642c 2069 7420 7769  ooks good, it wi
+000015e0: 6c6c 2062 6520 6d65 7267 6564 2069 6e74  ll be merged int
+000015f0: 6f20 7468 6520 6d61 696e 2072 6570 6f73  o the main repos
+00001600: 6974 6f72 792e 2043 6f6e 6772 6174 756c  itory. Congratul
+00001610: 6174 696f 6e73 2c20 796f 7527 7665 2073  ations, you've s
+00001620: 7563 6365 7373 6675 6c6c 7920 636f 6e74  uccessfully cont
+00001630: 7269 6275 7465 6420 746f 202a 546f 6f6c  ributed to *Tool
+00001640: 7320 4b69 742a 212a 2a0a 0a54 6861 6e6b  s Kit*!**..Thank
+00001650: 2079 6f75 2066 6f72 2079 6f75 7220 636f   you for your co
+00001660: 6e74 7269 6275 7469 6f6e 2120 596f 7572  ntribution! Your
+00001670: 2065 6666 6f72 7473 2068 656c 7020 696d   efforts help im
+00001680: 7072 6f76 6520 7468 6520 7072 6f6a 6563  prove the projec
+00001690: 7420 666f 7220 6576 6572 796f 6e65 2e0a  t for everyone..
+000016a0: 0a23 2320 f09f 939a 2043 6974 6520 5573  .## .... Cite Us
+000016b0: 0a3c 6120 6964 3d22 6369 7465 2d75 7322  .<a id="cite-us"
+000016c0: 3e3c 2f61 3e0a 0a49 6620 796f 7520 7573  ></a>..If you us
+000016d0: 6520 546f 6f6c 7320 4b69 7420 696e 2079  e Tools Kit in y
+000016e0: 6f75 7220 7265 7365 6172 6368 2077 6f72  our research wor
+000016f0: 6b20 6f72 2061 6361 6465 6d69 6320 7072  k or academic pr
+00001700: 6f6a 6563 7473 2c20 7765 2077 6f75 6c64  ojects, we would
+00001710: 2061 7070 7265 6369 6174 6520 6974 2069   appreciate it i
+00001720: 6620 796f 7520 636f 756c 6420 6369 7465  f you could cite
+00001730: 2075 732e 2059 6f75 2063 616e 2075 7365   us. You can use
+00001740: 2074 6865 2066 6f6c 6c6f 7769 6e67 2042   the following B
+00001750: 6962 5465 5820 656e 7472 793a 0a0a 6060  ibTeX entry:..``
+00001760: 6062 6962 7465 780a 406d 6973 637b 7072  `bibtex.@misc{pr
+00001770: 6f6a 6563 742d 7070 6368 656d 2d74 6f6f  oject-ppchem-too
+00001780: 6c73 2d6b 6974 2c0a 2020 7469 746c 6520  ls-kit,.  title 
+00001790: 3d20 7b50 726f 6a65 6374 2d70 7063 6865  = {Project-ppche
+000017a0: 6d2d 746f 6f6c 732d 6b69 747d 2c0a 2020  m-tools-kit},.  
+000017b0: 6175 7468 6f72 203d 207b 7b4d c3a9 6c6f  author = {{M..lo
+000017c0: c3a9 2045 6e7a 696e 6765 7220 2620 53c3  .. Enzinger & S.
+000017d0: a962 6173 7469 656e 2047 7275 6e62 6572  .bastien Grunber
+000017e0: 677d 7d2c 0a20 2079 6561 7220 3d20 7b32  g}},.  year = {2
+000017f0: 3032 347d 2c0a 2020 7075 626c 6973 6865  024},.  publishe
+00001800: 7220 3d20 7b47 6974 4875 627d 2c0a 2020  r = {GitHub},.  
+00001810: 6a6f 7572 6e61 6c20 3d20 7b47 6974 4875  journal = {GitHu
+00001820: 6220 5265 706f 7369 746f 7279 7d2c 0a20  b Repository},. 
+00001830: 2068 6f77 7075 626c 6973 6865 6420 3d20   howpublished = 
+00001840: 7b5c 7572 6c7b 6874 7470 733a 2f2f 6769  {\url{https://gi
+00001850: 7468 7562 2e63 6f6d 2f75 7365 726e 616d  thub.com/usernam
+00001860: 652f 5072 6f6a 6563 742d 7070 6368 656d  e/Project-ppchem
+00001870: 2d74 6f6f 6c73 2d6b 6974 7d7d 0a7d 0a60  -tools-kit}}.}.`
+00001880: 6060 0a0a 2323 2320 4368 6963 6167 6f20  ``..### Chicago 
+00001890: 5374 796c 650a 6060 6062 6173 680a 456e  Style.```bash.En
+000018a0: 7a69 6e67 6572 2c20 4dc3 a96c 6fc3 a92c  zinger, M..lo..,
+000018b0: 2061 6e64 2053 c3a9 6261 7374 6965 6e20   and S..bastien 
+000018c0: 4772 756e 6265 7267 2e20 3230 3234 2e20  Grunberg. 2024. 
+000018d0: 5072 6f6a 6563 742d 7070 6368 656d 2d74  Project-ppchem-t
+000018e0: 6f6f 6c73 2d6b 6974 2e20 436f 6d70 7574  ools-kit. Comput
+000018f0: 6572 2073 6f66 7477 6172 652e 2047 6974  er software. Git
+00001900: 4875 622e 2068 7474 7073 3a2f 2f67 6974  Hub. https://git
+00001910: 6875 622e 636f 6d2f 7573 6572 6e61 6d65  hub.com/username
+00001920: 2f50 726f 6a65 6374 2d70 7063 6865 6d2d  /Project-ppchem-
+00001930: 746f 6f6c 732d 6b69 742e 6020 0a60 6060  tools-kit.` .```
+00001940: 0a23 2320 f09f 939c 204c 6963 656e 7365  .## .... License
+00001950: 0a3c 6120 6964 3d22 6c69 6365 6e73 6522  .<a id="license"
+00001960: 3e3c 2f61 3e0a 0a54 6869 7320 7072 6f6a  ></a>..This proj
+00001970: 6563 7420 6973 206c 6963 656e 7365 6420  ect is licensed 
+00001980: 756e 6465 7220 7468 6520 4d49 5420 4c69  under the MIT Li
+00001990: 6365 6e73 652e 2053 6565 2074 6865 204c  cense. See the L
+000019a0: 4943 454e 5345 2066 696c 6520 666f 7220  ICENSE file for 
+000019b0: 6465 7461 696c 732e 0a0a 2323 20f0 9f93  details...## ...
+000019c0: b820 5363 7265 656e 7368 6f74 730a 3c61  . Screenshots.<a
+000019d0: 2069 643d 2273 6372 6565 6e73 686f 7473   id="screenshots
+000019e0: 223e 3c2f 613e 0a3c 696d 6720 7769 6474  "></a>.<img widt
+000019f0: 683d 2231 3030 3222 2061 6c74 3d22 4361  h="1002" alt="Ca
+00001a00: 7074 7572 6520 64e2 8099 65cc 8163 7261  pture d...e..cra
+00001a10: 6e20 3230 3234 2d30 352d 3138 2061 cc80  n 2024-05-18 a..
+00001a20: 2031 3620 3434 2030 3922 2073 7263 3d22   16 44 09" src="
+00001a30: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001a40: 6f6d 2f73 6772 756e 6265 722f 5072 6f6a  om/sgrunber/Proj
+00001a50: 6563 742d 7070 6368 656d 2d74 6f6f 6c73  ect-ppchem-tools
+00001a60: 2d6b 6974 2f61 7373 6574 732f 3136 3038  -kit/assets/1608
+00001a70: 3831 3836 342f 6134 3433 3739 6634 2d38  81864/a44379f4-8
+00001a80: 6366 322d 3461 6338 2d62 3337 302d 3336  cf2-4ac8-b370-36
+00001a90: 6665 6535 3532 6565 3661 223e 0a0a 0a    fee552ee6a">...
```

### Comparing `project_ppchem_tools_kit-0.1.0/pyproject.toml` & `project_ppchem_tools_kit-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
-name = "project-ppchem-tools-kit"
-version = "0.1.0"
-description = "The Tools Kit package allows chemistry students to find basic information on molecules and provides easy access to some graphs and calculations required in experimental laboratories."
+name = "Project-ppchem-tools-kit"
+version = "0.1.1"
+description = "Basic Chemistry Toolkit"
 authors = ["Méloé Enzinger <meloe.enzinger@epfl.ch> and Sébastien Grunberg <sebastien.grunberg@epfl.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 scikit-learn = "1.3.0"
+numpy5 = "^0.1"
 numpy = "^1.26.4"
 pillow = "10.2.0"
 pubchempy = "1.0.4"
 rdkit = "2023.9.6"
 requests = "2.31.0"
 matplotlib = "3.7.2"
 pandas = "2.0.3"
```

### Comparing `project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/display_molecule.py` & `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_molecule.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/error_calculation_interface.py` & `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/error_calculation_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,18 @@
+# Chem_pack/error_calculation.py
 import tkinter as tk
 import pyperclip
 
-
+def calculate_error_propagation(derivatives, uncertainties):
+    average_values = sum(derivatives) / len(derivatives)
+    error = sum((unc / deriv) ** 2 for deriv, unc in zip(derivatives, uncertainties))
+    standard_dev = (error ** 0.5) * average_values
+    return standard_dev, average_values
 
 def error_calculation_interface():
-    # Fonction pour calculer la propagation d'erreur
-    def calculate_error_propagation(derivatives, uncertainties):
-        average_values = sum(derivatives) / len(derivatives)
-        error = sum((unc / deriv) ** 2 for deriv, unc in zip(derivatives, uncertainties))
-        standard_dev = (error** 0.5) * average_values
-        return standard_dev, average_values 
-
-
-
-
     def copy_latex_code(latex_code):
         pyperclip.copy(latex_code)
         result_window.clipboard_clear()
         result_window.clipboard_append(latex_code)
         result_window.update()
 
     def calculate_and_display():
@@ -38,40 +33,48 @@
         # Display the result with calculation details
         result_text = f"Propagation of Uncertainty (∆z): {error:.6f}\n"
         result_text += f"Average Value: {average:.6f}\n\n"
         result_text += "Calculation Details:\n"
         for var_name, var_value, var_uncertainty in data:
             result_text += f"{var_name}: Value: {var_value}, Uncertainty: {var_uncertainty}\n"
 
-      
         latex_code = r"""
 
+        \subsection*{Propagation of Uncertainty ($\Delta\bar{z}$)}
 
-        Propagation of Uncertainty ($\Delta z$)
         The propagation of uncertainty is calculated as follows:
+
         \begin{equation}
         \Delta \bar{z} = \bar{z} \times \sqrt{\left(\left(\frac{\Delta x}{x}\right)^2 + \left(\frac{\Delta y}{y}\right)^2 + \ldots\right)}
         \end{equation}
+
+        The calculated uncertainty is:
+
         \[
-        \Delta z = """ + f"{error:.6f}" + r"""
+        \Delta \bar{z} = """ + f"{error:.6f}" + r"""
         \]
-        
+
         The average value is calculated as follows:
-        
+
         \begin{equation}
         \bar{z} = \frac{1}{N} \sum_{i=1}^{N} z_i
         \end{equation}
+
+        The calculated average value is:
+
         \[
         \bar{z} = """ + f"{average:.6f}" + r"""
         \]
 
-        The details of variables:
+        \subsection*{Details of Variables}
+
         \begin{itemize}
-        """ + "\n".join([f"    \item {var_name}: Value: {var_value}, Uncertainty: {var_uncertainty}" for var_name, var_value, var_uncertainty in data]) + r"""
+        """ + "\n".join([f"    \\item {var_name}: Value: {var_value}, Uncertainty: {var_uncertainty}" for var_name, var_value, var_uncertainty in data]) + r"""
         \end{itemize}
+
         """
 
         # Create a new window to display the result
         global result_window
         result_window = tk.Toplevel(error_calc_window)
         result_window.title("Result")
 
@@ -80,15 +83,14 @@
         result_textbox.insert("1.0", result_text)
         result_textbox.grid(row=0, column=0, padx=5, pady=5)
 
         # Button to copy LaTeX code to clipboard
         copy_button = tk.Button(result_window, text="Copy LaTeX Code", command=lambda: copy_latex_code(latex_code))
         copy_button.grid(row=1, column=0, padx=5, pady=5)
 
-
     def add_variable_entry():
         # Ajouter des champs d'entrée pour une nouvelle variable
         row = len(entries) + 1
 
         var_name_label = tk.Label(error_calc_window, text="Variable Name", bg="#1B262C", fg="white")
         var_name_label.grid(row=row, column=0, padx=5, pady=5)
         var_name_entry = tk.Entry(error_calc_window)
@@ -143,8 +145,8 @@
     entries = []
     entry_vars = []
     entry_values = []
     entry_uncertainties = []
     remove_buttons = []
     labels = []
 
-    error_calc_window.mainloop()
+    error_calc_window.mainloop()
```

### Comparing `project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/graph_function.py` & `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/graph_function.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/linear_regression.py` & `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/linear_regression.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import pandas as pd
 from tkinter import messagebox
-from Chem_pack.graph_function import display_graph
+from project_ppchem_tools_kit.graph_function import display_graph
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import r2_score
 import numpy as np
 
 
 def linear_regression(entry_input, x_label, y_label, title, grid=True, save_as=None, line_style='-', line_color='k'):
     try:
```

### Comparing `project_ppchem_tools_kit-0.1.0/src/project_ppchem_tools_kit/make_graph.py` & `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/make_graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import matplotlib.pyplot as plt
 import pandas as pd
 from tkinter import messagebox
-from Chem_pack.graph_function import display_graph
+from project_ppchem_tools_kit.graph_function import display_graph
 
 def make_graph(entry_input, x_label, y_label, title, grid=True, save_as=None, line_style='-', line_color='k'):
     try:
         # Récupérez les données du fichier Excel ou d'une autre source
         df = pd.read_excel(entry_input.get().strip())  # Utilisez entry_input pour obtenir le chemin du fichier
         data_list = df.values.tolist()
         x_values = [row[0] for row in data_list]
```

### Comparing `project_ppchem_tools_kit-0.1.0/PKG-INFO` & `project_ppchem_tools_kit-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,458 +1,485 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7072 6f6a  : 2.1.Name: proj
+00000010: 3a20 322e 310a 4e61 6d65 3a20 5072 6f6a  : 2.1.Name: Proj
 00000020: 6563 742d 7070 6368 656d 2d74 6f6f 6c73  ect-ppchem-tools
 00000030: 2d6b 6974 0a56 6572 7369 6f6e 3a20 302e  -kit.Version: 0.
-00000040: 312e 300a 5375 6d6d 6172 793a 2054 6865  1.0.Summary: The
-00000050: 2054 6f6f 6c73 204b 6974 2070 6163 6b61   Tools Kit packa
-00000060: 6765 2061 6c6c 6f77 7320 6368 656d 6973  ge allows chemis
-00000070: 7472 7920 7374 7564 656e 7473 2074 6f20  try students to 
-00000080: 6669 6e64 2062 6173 6963 2069 6e66 6f72  find basic infor
-00000090: 6d61 7469 6f6e 206f 6e20 6d6f 6c65 6375  mation on molecu
-000000a0: 6c65 7320 616e 6420 7072 6f76 6964 6573  les and provides
-000000b0: 2065 6173 7920 6163 6365 7373 2074 6f20   easy access to 
-000000c0: 736f 6d65 2067 7261 7068 7320 616e 6420  some graphs and 
-000000d0: 6361 6c63 756c 6174 696f 6e73 2072 6571  calculations req
-000000e0: 7569 7265 6420 696e 2065 7870 6572 696d  uired in experim
-000000f0: 656e 7461 6c20 6c61 626f 7261 746f 7269  ental laboratori
-00000100: 6573 2e0a 4c69 6365 6e73 653a 204d 4954  es..License: MIT
-00000110: 0a41 7574 686f 723a 204d c3a9 6c6f c3a9  .Author: M..lo..
-00000120: 2045 6e7a 696e 6765 720a 4175 7468 6f72   Enzinger.Author
-00000130: 2d65 6d61 696c 3a20 6d65 6c6f 652e 656e  -email: meloe.en
-00000140: 7a69 6e67 6572 4065 7066 6c2e 6368 3e20  zinger@epfl.ch> 
-00000150: 616e 6420 53c3 a962 6173 7469 656e 2047  and S..bastien G
-00000160: 7275 6e62 6572 6720 3c73 6562 6173 7469  runberg <sebasti
-00000170: 656e 2e67 7275 6e62 6572 6740 6570 666c  en.grunberg@epfl
-00000180: 2e63 680a 5265 7175 6972 6573 2d50 7974  .ch.Requires-Pyt
-00000190: 686f 6e3a 203e 3d33 2e31 302c 3c34 2e30  hon: >=3.10,<4.0
-000001a0: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
-000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000001c0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-000001d0: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
-000001e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000200: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
-00000210: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000220: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000230: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
-00000240: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000250: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000260: 6e20 3a3a 2033 2e31 310a 436c 6173 7369  n :: 3.11.Classi
-00000270: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000280: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000290: 7468 6f6e 203a 3a20 332e 3132 0a52 6571  thon :: 3.12.Req
-000002a0: 7569 7265 732d 4469 7374 3a20 6d61 7470  uires-Dist: matp
-000002b0: 6c6f 746c 6962 2028 3d3d 332e 372e 3229  lotlib (==3.7.2)
-000002c0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000002d0: 6e75 6d70 7920 283e 3d31 2e32 362e 342c  numpy (>=1.26.4,
-000002e0: 3c32 2e30 2e30 290a 5265 7175 6972 6573  <2.0.0).Requires
-000002f0: 2d44 6973 743a 2070 616e 6461 7320 283d  -Dist: pandas (=
-00000300: 3d32 2e30 2e33 290a 5265 7175 6972 6573  =2.0.3).Requires
-00000310: 2d44 6973 743a 2070 696c 6c6f 7720 283d  -Dist: pillow (=
-00000320: 3d31 302e 322e 3029 0a52 6571 7569 7265  =10.2.0).Require
-00000330: 732d 4469 7374 3a20 7075 6263 6865 6d70  s-Dist: pubchemp
-00000340: 7920 283d 3d31 2e30 2e34 290a 5265 7175  y (==1.0.4).Requ
-00000350: 6972 6573 2d44 6973 743a 2070 7970 6572  ires-Dist: pyper
-00000360: 636c 6970 2028 3d3d 312e 382e 3229 0a52  clip (==1.8.2).R
-00000370: 6571 7569 7265 732d 4469 7374 3a20 7264  equires-Dist: rd
-00000380: 6b69 7420 283d 3d32 3032 332e 392e 3629  kit (==2023.9.6)
-00000390: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000003a0: 7265 706f 7274 6c61 6220 283d 3d34 2e32  reportlab (==4.2
-000003b0: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-000003c0: 743a 2072 6571 7565 7374 7320 283d 3d32  t: requests (==2
-000003d0: 2e33 312e 3029 0a52 6571 7569 7265 732d  .31.0).Requires-
-000003e0: 4469 7374 3a20 7363 696b 6974 2d6c 6561  Dist: scikit-lea
-000003f0: 726e 2028 3d3d 312e 332e 3029 0a44 6573  rn (==1.3.0).Des
-00000400: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000410: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000420: 646f 776e 0a0a 0a23 20f0 9fa7 b020 546f  down...# .... To
-00000430: 6f6c 7320 4b69 740a 215b 6c6f 676f 5d28  ols Kit.![logo](
-00000440: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000450: 6f6d 2f73 6772 756e 6265 722f 5072 6f6a  om/sgrunber/Proj
-00000460: 6563 742d 7070 6368 656d 2d74 6f6f 6c73  ect-ppchem-tools
-00000470: 2d6b 6974 2f61 7373 6574 732f 3136 3038  -kit/assets/1608
-00000480: 3831 3836 342f 3265 3435 3930 6233 2d37  81864/2e4590b3-7
-00000490: 3031 352d 3466 3639 2d39 3734 362d 6439  015-4f69-9746-d9
-000004a0: 3530 6538 3761 3766 3866 290a 0a5b 215b  50e87a7f8f)..[![
-000004b0: 6275 696c 645d 2868 7474 7073 3a2f 2f69  build](https://i
-000004c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-000004d0: 6467 652f 6275 696c 642d 7061 7373 696e  dge/build-passin
-000004e0: 672d 6272 6967 6874 6772 6565 6e29 5d28  g-brightgreen)](
-000004f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000500: 6f6d 2f73 6772 756e 6265 722f 5072 6f6a  om/sgrunber/Proj
-00000510: 6563 742d 7070 6368 656d 2d74 6f6f 6c73  ect-ppchem-tools
-00000520: 2d6b 6974 290a 5b21 5b63 6f76 6572 6167  -kit).[![coverag
-00000530: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
-00000540: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000550: 636f 7665 7261 6765 2d39 3525 3235 2d62  coverage-95%25-b
-00000560: 7269 6768 7467 7265 656e 295d 2868 7474  rightgreen)](htt
-00000570: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000580: 7367 7275 6e62 6572 2f50 726f 6a65 6374  sgrunber/Project
-00000590: 2d70 7063 6865 6d2d 746f 6f6c 732d 6b69  -ppchem-tools-ki
-000005a0: 7429 0a5b 215b 6c69 6365 6e73 655d 2868  t).[![license](h
-000005b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000005c0: 6473 2e69 6f2f 6261 6467 652f 6c69 6365  ds.io/badge/lice
-000005d0: 6e73 652d 4d49 542d 626c 7565 295d 2868  nse-MIT-blue)](h
-000005e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000005f0: 6d2f 7367 7275 6e62 6572 2f50 726f 6a65  m/sgrunber/Proje
-00000600: 6374 2d70 7063 6865 6d2d 746f 6f6c 732d  ct-ppchem-tools-
-00000610: 6b69 742f 626c 6f62 2f6d 6169 6e2f 4c49  kit/blob/main/LI
-00000620: 4345 4e53 4529 0a0a 0a23 2320 f09f 9396  CENSE)...## ....
-00000630: 2044 6573 6372 6970 7469 6f6e 0a54 6865   Description.The
-00000640: 202a 2a54 6f6f 6c73 204b 6974 2a2a 2070   **Tools Kit** p
-00000650: 6163 6b61 6765 2061 6c6c 6f77 7320 6368  ackage allows ch
-00000660: 656d 6973 7472 7920 7374 7564 656e 7473  emistry students
-00000670: 2074 6f20 6669 6e64 2062 6173 6963 2069   to find basic i
-00000680: 6e66 6f72 6d61 7469 6f6e 206f 6e20 6d6f  nformation on mo
-00000690: 6c65 6375 6c65 7320 616e 6420 7072 6f76  lecules and prov
-000006a0: 6964 6573 2065 6173 7920 6163 6365 7373  ides easy access
-000006b0: 2074 6f20 736f 6d65 2067 7261 7068 7320   to some graphs 
-000006c0: 616e 6420 6361 6c63 756c 6174 696f 6e73  and calculations
-000006d0: 2072 6571 7569 7265 6420 696e 2065 7870   required in exp
-000006e0: 6572 696d 656e 7461 6c20 6c61 626f 7261  erimental labora
-000006f0: 746f 7269 6573 2e0a 0a23 2320 f09f 939a  tories...## ....
-00000700: 2054 6162 6c65 206f 6620 436f 6e74 656e   Table of Conten
-00000710: 7473 0a2d 205b 496e 7374 616c 6c61 7469  ts.- [Installati
-00000720: 6f6e 5d28 23ef b88f 2d69 6e73 7461 6c6c  on](#...-install
-00000730: 6174 696f 6e29 0a2d 205b 5573 6167 655d  ation).- [Usage]
-00000740: 2823 efb8 8f2d 7573 6167 6529 0a2d 205b  (#...-usage).- [
-00000750: 4665 6174 7572 6573 5d28 23ef b88f 2d66  Features](#...-f
-00000760: 6561 7475 7265 7329 0a2d 205b 436f 6e74  eatures).- [Cont
-00000770: 7269 6275 7469 6e67 5d28 23ef b88f 2d63  ributing](#...-c
-00000780: 6f6e 7472 6962 7574 696e 6729 0a2d 205b  ontributing).- [
-00000790: 4369 7465 2055 735d 2823 efb8 8f2d 6369  Cite Us](#...-ci
-000007a0: 7465 2d75 7329 0a2d 205b 4c69 6365 6e73  te-us).- [Licens
-000007b0: 655d 2823 efb8 8f2d 6c69 6365 6e73 6529  e](#...-license)
-000007c0: 0a2d 205b 5363 7265 656e 7368 6f74 735d  .- [Screenshots]
-000007d0: 2823 efb8 8f2d 7363 7265 656e 7368 6f74  (#...-screenshot
-000007e0: 7329 0a0a 2323 20f0 9f9b a0ef b88f 2049  s)..## ....... I
-000007f0: 6e73 7461 6c6c 6174 696f 6e0a 3c61 2069  nstallation.<a i
-00000800: 643d 2269 6e73 7461 6c6c 6174 696f 6e22  d="installation"
-00000810: 3e3c 2f61 3e0a 2323 2320 312e 20f0 9f8d  ></a>.### 1. ...
-00000820: b420 466f 726b 2074 6865 2052 6570 6f73  . Fork the Repos
-00000830: 6974 6f72 790a 546f 2073 7461 7274 2c20  itory.To start, 
-00000840: 666f 726b 2074 6865 2072 6570 6f73 6974  fork the reposit
-00000850: 6f72 7920 746f 2079 6f75 7220 6f77 6e20  ory to your own 
-00000860: 4769 7448 7562 2061 6363 6f75 6e74 2e20  GitHub account. 
-00000870: 200a 546f 2064 6f20 736f 2c20 6e61 7669   .To do so, navi
-00000880: 6761 7465 2074 6f20 7468 6520 7265 706f  gate to the repo
-00000890: 7369 746f 7279 2070 6167 6520 616e 6420  sitory page and 
-000008a0: 636c 6963 6b20 7468 6520 2a22 466f 726b  click the *"Fork
-000008b0: 222a 2062 7574 746f 6e2e 2054 6865 2072  "* button. The r
-000008c0: 6570 6f73 6974 6f72 7920 7769 6c6c 2074  epository will t
-000008d0: 6865 6e20 6265 2063 6f70 6965 6420 746f  hen be copied to
-000008e0: 2079 6f75 7220 6163 636f 756e 742c 2061   your account, a
-000008f0: 6e64 2079 6f75 2077 696c 6c20 6265 2061  nd you will be a
-00000900: 626c 6520 746f 2061 6363 6573 7320 6974  ble to access it
-00000910: 2e0a 0a23 2323 2032 2e20 f09f 93a5 2043  ...### 2. .... C
-00000920: 6c6f 6e65 2074 6865 2052 6570 6f73 6974  lone the Reposit
-00000930: 6f72 790a 4e65 7874 2c20 636c 6f6e 6520  ory.Next, clone 
-00000940: 7468 6520 7265 706f 7369 746f 7279 2075  the repository u
-00000950: 7369 6e67 2074 6865 2066 6f6c 6c6f 7769  sing the followi
-00000960: 6e67 2063 6f6d 6d61 6e64 2028 7265 706c  ng command (repl
-00000970: 6163 6520 2a75 7365 726e 616d 652a 2077  ace *username* w
-00000980: 6974 6820 796f 7572 2047 6974 4875 6220  ith your GitHub 
-00000990: 7573 6572 6e61 6d65 293a 0a0a 6060 6062  username):..```b
-000009a0: 6173 680a 6769 7420 636c 6f6e 6520 6874  ash.git clone ht
-000009b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000009c0: 2f2a 7573 6572 6e61 6d65 2a2f 5072 6f6a  /*username*/Proj
-000009d0: 6563 742d 7070 6368 656d 2d74 6f6f 6c73  ect-ppchem-tools
-000009e0: 2d6b 6974 2e67 6974 0a60 6060 0a0a 2323  -kit.git.```..##
-000009f0: 2320 332e 20e2 ac87 efb8 8f20 496e 7374  # 3. ...... Inst
-00000a00: 616c 6c20 7769 7468 2070 6970 0a59 6f75  all with pip.You
-00000a10: 2063 616e 2061 6c73 6f20 696e 7374 616c   can also instal
-00000a20: 6c20 546f 6f6c 7320 4b69 7420 7573 696e  l Tools Kit usin
-00000a30: 6720 7069 703a 0a0a 6060 6062 6173 680a  g pip:..```bash.
-00000a40: 7069 7020 696e 7374 616c 6c20 5072 6f6a  pip install Proj
-00000a50: 6563 745f 7070 6368 656d 2d74 6f6f 6c73  ect_ppchem-tools
-00000a60: 2d6b 6974 0a60 6060 0a0a 2323 20f0 9f9a  -kit.```..## ...
-00000a70: 8020 5573 6167 650a 3c61 2069 643d 2275  . Usage.<a id="u
-00000a80: 7361 6765 223e 3c2f 613e 0a0a 546f 2075  sage"></a>..To u
-00000a90: 7365 2054 6f6f 6c73 204b 6974 2061 6e64  se Tools Kit and
-00000aa0: 2061 6363 6573 7320 6974 7320 6665 6174   access its feat
-00000ab0: 7572 6573 2c20 666f 6c6c 6f77 2074 6865  ures, follow the
-00000ac0: 7365 2073 7465 7073 2061 6674 6572 2063  se steps after c
-00000ad0: 6c6f 6e69 6e67 2074 6865 2072 6570 6f73  loning the repos
-00000ae0: 6974 6f72 793a 0a0a 2323 2320 5573 696e  itory:..### Usin
-00000af0: 6720 4a75 7079 7465 7220 4e6f 7465 626f  g Jupyter Notebo
-00000b00: 6f6b 3a0a 0a31 2e20 4c61 756e 6368 204a  ok:..1. Launch J
-00000b10: 7570 7974 6572 204e 6f74 6562 6f6f 6b20  upyter Notebook 
-00000b20: 6279 206e 6176 6967 6174 696e 6720 746f  by navigating to
-00000b30: 2074 6865 2063 6c6f 6e65 6420 7265 706f   the cloned repo
-00000b40: 7369 746f 7279 2064 6972 6563 746f 7279  sitory directory
-00000b50: 2069 6e20 796f 7572 2074 6572 6d69 6e61   in your termina
-00000b60: 6c20 616e 6420 7275 6e6e 696e 6720 7468  l and running th
-00000b70: 6520 636f 6d6d 616e 643a 0a20 2020 6060  e command:.   ``
-00000b80: 6062 6173 680a 2020 206a 7570 7974 6572  `bash.   jupyter
-00000b90: 206e 6f74 6562 6f6f 6b0a 2020 2060 6060   notebook.   ```
-00000ba0: 0a32 2e20 496e 2074 6865 204a 7570 7974  .2. In the Jupyt
-00000bb0: 6572 204e 6f74 6562 6f6f 6b20 696e 7465  er Notebook inte
-00000bc0: 7266 6163 652c 206e 6176 6967 6174 6520  rface, navigate 
-00000bd0: 746f 2074 6865 2060 6e6f 7465 626f 6f6b  to the `notebook
-00000be0: 7360 2064 6972 6563 746f 7279 2e0a 0a33  s` directory...3
-00000bf0: 2e20 4f70 656e 2074 6865 206e 6f74 6562  . Open the noteb
-00000c00: 6f6f 6b20 6e61 6d65 6420 6070 726f 6a65  ook named `proje
-00000c10: 6374 5f72 6570 6f72 742e 6970 796e 6260  ct_report.ipynb`
-00000c20: 2e0a 0a34 2e20 466f 6c6c 6f77 2074 6865  ...4. Follow the
-00000c30: 2069 6e73 7472 7563 7469 6f6e 7320 696e   instructions in
-00000c40: 7369 6465 2074 6865 206e 6f74 6562 6f6f  side the noteboo
-00000c50: 6b20 746f 2069 6e74 6572 6163 7420 7769  k to interact wi
-00000c60: 7468 2074 6865 2054 6f6f 6c73 204b 6974  th the Tools Kit
-00000c70: 2069 6e74 6572 6661 6365 2061 6e64 2075   interface and u
-00000c80: 7469 6c69 7a65 2069 7473 2066 6561 7475  tilize its featu
-00000c90: 7265 7320 666f 7220 6d6f 6c65 6375 6c65  res for molecule
-00000ca0: 2061 6e61 6c79 7369 732c 2067 7261 7068   analysis, graph
-00000cb0: 2070 6c6f 7474 696e 672c 2065 7272 6f72   plotting, error
-00000cc0: 2063 616c 6375 6c61 7469 6f6e 2c20 616e   calculation, an
-00000cd0: 6420 6d6f 7265 2e0a 5468 6973 206e 6f74  d more..This not
-00000ce0: 6562 6f6f 6b20 7072 6f76 6964 6573 2061  ebook provides a
-00000cf0: 6e20 696e 7465 7261 6374 6976 6520 656e  n interactive en
-00000d00: 7669 726f 6e6d 656e 7420 666f 7220 636f  vironment for co
-00000d10: 6e76 656e 6965 6e74 2075 7361 6765 206f  nvenient usage o
-00000d20: 6620 546f 6f6c 7320 4b69 7420 6469 7265  f Tools Kit dire
-00000d30: 6374 6c79 2077 6974 6869 6e20 5669 7375  ctly within Visu
-00000d40: 616c 2053 7475 6469 6f20 436f 6465 2e0a  al Studio Code..
-00000d50: 0a0a 2323 2320 5573 6167 6520 7769 7468  ..### Usage with
-00000d60: 2056 6973 7561 6c20 5374 7564 696f 2043   Visual Studio C
-00000d70: 6f64 653a 0a0a 312e 204f 7065 6e20 5669  ode:..1. Open Vi
-00000d80: 7375 616c 2053 7475 6469 6f20 436f 6465  sual Studio Code
-00000d90: 2061 6e64 206e 6176 6967 6174 6520 746f   and navigate to
-00000da0: 2074 6865 2063 6c6f 6e65 6420 6469 7265   the cloned dire
-00000db0: 6374 6f72 792e 0a0a 322e 2049 6e73 7461  ctory...2. Insta
-00000dc0: 6c6c 2074 6865 204a 7570 7974 6572 2065  ll the Jupyter e
-00000dd0: 7874 656e 7369 6f6e 2069 6620 6e6f 7420  xtension if not 
-00000de0: 616c 7265 6164 7920 696e 7374 616c 6c65  already installe
-00000df0: 642e 2059 6f75 2063 616e 2064 6f20 7468  d. You can do th
-00000e00: 6973 2062 7920 7365 6172 6368 696e 6720  is by searching 
-00000e10: 666f 7220 224a 7570 7974 6572 2220 696e  for "Jupyter" in
-00000e20: 2074 6865 2045 7874 656e 7369 6f6e 7320   the Extensions 
-00000e30: 7669 6577 2028 4374 726c 2b53 6869 6674  view (Ctrl+Shift
-00000e40: 2b58 2920 616e 6420 696e 7374 616c 6c69  +X) and installi
-00000e50: 6e67 2074 6865 2022 5079 7468 6f6e 2220  ng the "Python" 
-00000e60: 6578 7465 6e73 696f 6e20 7061 636b 2e0a  extension pack..
-00000e70: 0a33 2e20 4f70 656e 2074 6865 2060 6e6f  .3. Open the `no
-00000e80: 7465 626f 6f6b 7360 2064 6972 6563 746f  tebooks` directo
-00000e90: 7279 2069 6e20 5669 7375 616c 2053 7475  ry in Visual Stu
-00000ea0: 6469 6f20 436f 6465 2e0a 0a34 2e20 4f70  dio Code...4. Op
-00000eb0: 656e 2074 6865 206e 6f74 6562 6f6f 6b20  en the notebook 
-00000ec0: 6e61 6d65 6420 6070 726f 6a65 6374 5f72  named `project_r
-00000ed0: 6570 6f72 742e 6970 796e 6260 2e0a 0a35  eport.ipynb`...5
-00000ee0: 2e20 466f 6c6c 6f77 2074 6865 2069 6e73  . Follow the ins
-00000ef0: 7472 7563 7469 6f6e 7320 696e 7369 6465  tructions inside
-00000f00: 2074 6865 206e 6f74 6562 6f6f 6b20 746f   the notebook to
-00000f10: 2069 6e74 6572 6163 7420 7769 7468 2074   interact with t
-00000f20: 6865 2054 6f6f 6c73 204b 6974 2069 6e74  he Tools Kit int
-00000f30: 6572 6661 6365 2061 6e64 2075 7469 6c69  erface and utili
-00000f40: 7a65 2069 7473 2066 6561 7475 7265 7320  ze its features 
-00000f50: 666f 7220 6d6f 6c65 6375 6c65 2061 6e61  for molecule ana
-00000f60: 6c79 7369 732c 2067 7261 7068 2070 6c6f  lysis, graph plo
-00000f70: 7474 696e 672c 2065 7272 6f72 2063 616c  tting, error cal
-00000f80: 6375 6c61 7469 6f6e 2c20 616e 6420 6d6f  culation, and mo
-00000f90: 7265 2e0a 5468 6973 206e 6f74 6562 6f6f  re..This noteboo
-00000fa0: 6b20 7072 6f76 6964 6573 2061 6e20 696e  k provides an in
-00000fb0: 7465 7261 6374 6976 6520 656e 7669 726f  teractive enviro
-00000fc0: 6e6d 656e 7420 666f 7220 636f 6e76 656e  nment for conven
-00000fd0: 6965 6e74 2075 7361 6765 206f 6620 546f  ient usage of To
-00000fe0: 6f6c 7320 4b69 7420 7769 7468 204a 7570  ols Kit with Jup
-00000ff0: 7974 6572 204e 6f74 6562 6f6f 6b2e 0a0a  yter Notebook...
-00001000: 2323 20f0 9fa7 aa20 4665 6174 7572 6573  ## .... Features
-00001010: 0a0a 312e 20f0 9fa7 ac20 4d6f 6c65 6375  ..1. .... Molecu
-00001020: 6c65 204e 616d 650a 2020 202d 2049 6e70  le Name.   - Inp
-00001030: 7574 3a20 5261 7720 666f 726d 756c 6120  ut: Raw formula 
-00001040: 6f66 2074 6865 206d 6f6c 6563 756c 650a  of the molecule.
-00001050: 2020 202d 204f 7574 7075 743a 2053 4d49     - Output: SMI
-00001060: 4c45 5320 6f66 2074 6865 206d 6f6c 6563  LES of the molec
-00001070: 756c 650a 0a32 2e20 e29a 96ef b88f 204d  ule..2. ...... M
-00001080: 6f6c 6563 756c 6172 2057 6569 6768 740a  olecular Weight.
-00001090: 2020 202d 2049 6e70 7574 3a20 534d 494c     - Input: SMIL
-000010a0: 4553 206f 6620 7468 6520 6d6f 6c65 6375  ES of the molecu
-000010b0: 6c65 0a20 2020 2d20 4f75 7470 7574 3a20  le.   - Output: 
-000010c0: 436f 7272 6573 706f 6e64 696e 6720 6d6f  Corresponding mo
-000010d0: 6c61 7220 6d61 7373 2069 6e20 672f 6d6f  lar mass in g/mo
-000010e0: 6c0a 0a33 2e20 f09f 9388 204c 696e 6561  l..3. .... Linea
-000010f0: 7220 5265 6772 6573 7369 6f6e 0a20 2020  r Regression.   
-00001100: 2d20 496e 7075 743a 2045 7863 656c 2064  - Input: Excel d
-00001110: 6f63 756d 656e 7420 2869 6d70 6f72 7465  ocument (importe
-00001120: 6420 6279 2070 7265 7373 696e 6720 7468  d by pressing th
-00001130: 6520 4272 6f77 7365 2062 7574 746f 6e29  e Browse button)
-00001140: 0a20 2020 2d20 4f75 7470 7574 3a20 4c69  .   - Output: Li
-00001150: 6e65 6172 2072 6567 7265 7373 696f 6e20  near regression 
-00001160: 6772 6170 6820 7769 7468 2074 6865 2052  graph with the R
-00001170: 3c73 7570 3e32 3c2f 7375 703e 2076 616c  <sup>2</sup> val
-00001180: 7565 0a0a 342e 20f0 9f93 8a20 4772 6170  ue..4. .... Grap
-00001190: 6820 4d61 6b65 720a 2020 202d 2049 6e70  h Maker.   - Inp
-000011a0: 7574 3a20 4578 6365 6c20 646f 6375 6d65  ut: Excel docume
-000011b0: 6e74 2077 6974 6820 7820 616e 6420 7920  nt with x and y 
-000011c0: 7661 6c75 6573 2061 7272 616e 6765 6420  values arranged 
-000011d0: 696e 2074 776f 2063 6f6c 756d 6e73 0a20  in two columns. 
-000011e0: 2020 2d20 4f75 7470 7574 3a20 4772 6170    - Output: Grap
-000011f0: 6820 706c 6f74 7469 6e67 2061 6c6c 2076  h plotting all v
-00001200: 616c 7565 730a 2020 2020 2020 2d20 4f70  alues.      - Op
-00001210: 7469 6f6e 733a 2054 6865 2067 7261 7068  tions: The graph
-00001220: 2061 6c6c 6f77 7320 6375 7374 6f6d 697a   allows customiz
-00001230: 6174 696f 6e20 6f66 2076 6172 696f 7573  ation of various
-00001240: 2070 6172 616d 6574 6572 7320 7375 6368   parameters such
-00001250: 2061 7320 6368 616e 6769 6e67 2073 6361   as changing sca
-00001260: 6c65 732c 2061 7869 7320 6c61 6265 6c73  les, axis labels
-00001270: 2c20 7469 746c 652c 2064 6973 706c 6179  , title, display
-00001280: 696e 6720 6d61 7869 6d75 6d20 7661 6c75  ing maximum valu
-00001290: 6573 2c20 656e 6162 6c69 6e67 2067 7269  es, enabling gri
-000012a0: 646c 696e 6573 2c20 6164 6a75 7374 696e  dlines, adjustin
-000012b0: 6720 6c69 6e65 2074 7970 6573 2061 6e64  g line types and
-000012c0: 2063 6f6c 6f72 732c 206d 6f64 6966 7969   colors, modifyi
-000012d0: 6e67 2067 7269 6420 616e 6420 6c61 6265  ng grid and labe
-000012e0: 6c20 6178 6573 2c20 616e 6420 6261 636b  l axes, and back
-000012f0: 6772 6f75 6e64 2063 6f6c 6f72 2e0a 0a0a  ground color....
-00001300: 352e 20f0 9f93 8920 4572 726f 7220 5072  5. .... Error Pr
-00001310: 6f70 6167 6174 696f 6e0a 2020 202d 2049  opagation.   - I
-00001320: 6e70 7574 3a20 5661 7269 6162 6c65 732c  nput: Variables,
-00001330: 2074 6865 6972 2076 616c 7565 732c 2061   their values, a
-00001340: 6e64 2074 6865 6972 2075 6e63 6572 7461  nd their uncerta
-00001350: 696e 7469 6573 2e0a 2020 202d 204f 7574  inties..   - Out
-00001360: 7075 743a 204d 6561 6e20 7661 6c75 652c  put: Mean value,
-00001370: 2069 7473 2075 6e63 6572 7461 696e 7479   its uncertainty
-00001380: 2c20 616e 6420 7468 6520 7265 7375 6c74  , and the result
-00001390: 2063 616e 2062 6520 636f 7069 6564 2061   can be copied a
-000013a0: 7320 4c61 5465 5820 636f 6465 2066 6f72  s LaTeX code for
-000013b0: 2065 6173 7920 696e 636c 7573 696f 6e20   easy inclusion 
-000013c0: 696e 2064 6f63 756d 656e 7473 2e0a 0a36  in documents...6
-000013d0: 2e20 f09f a7aa 2053 686f 7720 4d6f 6c65  . .... Show Mole
-000013e0: 6375 6c65 0a20 2020 2d20 496e 7075 743a  cule.   - Input:
-000013f0: 2053 4d49 4c45 530a 2020 202d 204f 7574   SMILES.   - Out
-00001400: 7075 743a 204d 6f6c 6563 756c 6172 2073  put: Molecular s
-00001410: 7472 7563 7475 7265 0a0a 5468 6520 6772  tructure..The gr
-00001420: 6170 6873 2069 6e20 7365 6374 696f 6e73  aphs in sections
-00001430: 2033 2061 6e64 2034 2063 616e 2061 6c73   3 and 4 can als
-00001440: 6f20 696e 636c 7564 6520 696e 7075 7420  o include input 
-00001450: 666f 7220 7468 6520 7469 746c 6520 616e  for the title an
-00001460: 6420 582c 2059 2061 7869 7320 6c61 6265  d X, Y axis labe
-00001470: 6c73 2e0a 0a23 2320 f09f a49d 2043 6f6e  ls...## .... Con
-00001480: 7472 6962 7574 696e 670a 3c61 2069 643d  tributing.<a id=
-00001490: 2263 6f6e 7472 6962 7574 696e 6722 3e3c  "contributing"><
-000014a0: 2f61 3e0a 0a43 6f6e 7472 6962 7574 696f  /a>..Contributio
-000014b0: 6e73 2061 7265 2077 656c 636f 6d65 2120  ns are welcome! 
-000014c0: 546f 2063 6f6e 7472 6962 7574 6520 746f  To contribute to
-000014d0: 202a 2a54 6f6f 6c73 204b 6974 2a2a 2c20   **Tools Kit**, 
-000014e0: 706c 6561 7365 2066 6f6c 6c6f 7720 7468  please follow th
-000014f0: 6573 6520 7374 6570 733a 0a0a 312e 202a  ese steps:..1. *
-00001500: 2a46 6f72 6b2a 2a20 7468 6520 7072 6f6a  *Fork** the proj
-00001510: 6563 7420 746f 2079 6f75 7220 4769 7448  ect to your GitH
-00001520: 7562 2061 6363 6f75 6e74 2e0a 322e 2043  ub account..2. C
-00001530: 7265 6174 6520 6120 6e65 7720 6272 616e  reate a new bran
-00001540: 6368 2066 6f72 2079 6f75 7220 6665 6174  ch for your feat
-00001550: 7572 6520 6f72 2062 7567 2066 6978 3a20  ure or bug fix: 
-00001560: 0a20 2020 6060 6062 6173 680a 2020 2067  .   ```bash.   g
-00001570: 6974 2063 6865 636b 6f75 7420 2d62 2066  it checkout -b f
-00001580: 6561 7475 7265 2f79 6f75 722d 6665 6174  eature/your-feat
-00001590: 7572 652d 6e61 6d65 0a20 2020 6060 600a  ure-name.   ```.
-000015a0: 332e 202a 2a43 7265 6174 6520 6120 6e65  3. **Create a ne
-000015b0: 7720 6272 616e 6368 2066 6f72 2079 6f75  w branch for you
-000015c0: 7220 6665 6174 7572 6520 6f72 2062 7567  r feature or bug
-000015d0: 2066 6978 3a2a 2a0a 0a20 2020 2060 6060   fix:**..    ```
-000015e0: 6261 7368 0a20 2020 2067 6974 2063 6865  bash.    git che
-000015f0: 636b 6f75 7420 2d62 2066 6561 7475 7265  ckout -b feature
-00001600: 2f79 6f75 722d 6665 6174 7572 652d 6e61  /your-feature-na
-00001610: 6d65 0a20 2020 2060 6060 0a0a 342e 202a  me.    ```..4. *
-00001620: 2a4d 616b 6520 796f 7572 2063 6861 6e67  *Make your chang
-00001630: 6573 2061 6e64 2065 6e73 7572 6520 7468  es and ensure th
-00001640: 6579 2061 6468 6572 6520 746f 2074 6865  ey adhere to the
-00001650: 2070 726f 6a65 6374 2773 2063 6f64 696e   project's codin
-00001660: 6720 636f 6e76 656e 7469 6f6e 7320 616e  g conventions an
-00001670: 6420 7374 796c 6520 6775 6964 656c 696e  d style guidelin
-00001680: 6573 2e2a 2a0a 0a35 2e20 2a2a 436f 6d6d  es.**..5. **Comm
-00001690: 6974 2079 6f75 7220 6368 616e 6765 7320  it your changes 
-000016a0: 7769 7468 2064 6573 6372 6970 7469 7665  with descriptive
-000016b0: 206d 6573 7361 6765 7320 6578 706c 6169   messages explai
-000016c0: 6e69 6e67 2074 6865 2070 7572 706f 7365  ning the purpose
-000016d0: 206f 6620 796f 7572 2063 6861 6e67 6573   of your changes
-000016e0: 3a2a 2a0a 0a20 2020 2060 6060 6261 7368  :**..    ```bash
-000016f0: 0a20 2020 2067 6974 2063 6f6d 6d69 7420  .    git commit 
-00001700: 2d61 6d20 2741 6464 2073 6f6d 6520 6665  -am 'Add some fe
-00001710: 6174 7572 6527 0a20 2020 2060 6060 0a0a  ature'.    ```..
-00001720: 362e 202a 2a50 7573 6820 796f 7572 2063  6. **Push your c
-00001730: 6861 6e67 6573 2074 6f20 796f 7572 2062  hanges to your b
-00001740: 7261 6e63 6820 6f6e 2079 6f75 7220 666f  ranch on your fo
-00001750: 726b 6564 2072 6570 6f73 6974 6f72 793a  rked repository:
-00001760: 2a2a 0a0a 2020 2020 6060 6062 6173 680a  **..    ```bash.
-00001770: 2020 2020 6769 7420 7075 7368 206f 7269      git push ori
-00001780: 6769 6e20 6665 6174 7572 652f 796f 7572  gin feature/your
-00001790: 2d66 6561 7475 7265 2d6e 616d 650a 2020  -feature-name.  
-000017a0: 2020 6060 600a 0a37 2e20 2a2a 4f6e 6365    ```..7. **Once
-000017b0: 2079 6f75 2776 6520 7075 7368 6564 2079   you've pushed y
-000017c0: 6f75 7220 6368 616e 6765 732c 2079 6f75  our changes, you
-000017d0: 2063 616e 206f 7065 6e20 6120 5075 6c6c   can open a Pull
-000017e0: 2052 6571 7565 7374 2028 5052 2920 696e   Request (PR) in
-000017f0: 2074 6865 206f 7269 6769 6e61 6c20 7265   the original re
-00001800: 706f 7369 746f 7279 2e20 5072 6f76 6964  pository. Provid
-00001810: 6520 6120 636c 6561 7220 6465 7363 7269  e a clear descri
-00001820: 7074 696f 6e20 6f66 2074 6865 2063 6861  ption of the cha
-00001830: 6e67 6573 2079 6f75 2776 6520 6d61 6465  nges you've made
-00001840: 2069 6e20 7468 6520 5052 2e2a 2a0a 0a38   in the PR.**..8
-00001850: 2e20 2a2a 4166 7465 7220 7265 7669 6577  . **After review
-00001860: 696e 6720 796f 7572 2050 522c 2069 6620  ing your PR, if 
-00001870: 6576 6572 7974 6869 6e67 206c 6f6f 6b73  everything looks
-00001880: 2067 6f6f 642c 2069 7420 7769 6c6c 2062   good, it will b
-00001890: 6520 6d65 7267 6564 2069 6e74 6f20 7468  e merged into th
-000018a0: 6520 6d61 696e 2072 6570 6f73 6974 6f72  e main repositor
-000018b0: 792e 2043 6f6e 6772 6174 756c 6174 696f  y. Congratulatio
-000018c0: 6e73 2c20 796f 7527 7665 2073 7563 6365  ns, you've succe
-000018d0: 7373 6675 6c6c 7920 636f 6e74 7269 6275  ssfully contribu
-000018e0: 7465 6420 746f 202a 546f 6f6c 7320 4b69  ted to *Tools Ki
-000018f0: 742a 212a 2a0a 0a54 6861 6e6b 2079 6f75  t*!**..Thank you
-00001900: 2066 6f72 2079 6f75 7220 636f 6e74 7269   for your contri
-00001910: 6275 7469 6f6e 2120 596f 7572 2065 6666  bution! Your eff
-00001920: 6f72 7473 2068 656c 7020 696d 7072 6f76  orts help improv
-00001930: 6520 7468 6520 7072 6f6a 6563 7420 666f  e the project fo
-00001940: 7220 6576 6572 796f 6e65 2e0a 0a23 2320  r everyone...## 
-00001950: f09f 939a 2043 6974 6520 5573 0a3c 6120  .... Cite Us.<a 
-00001960: 6964 3d22 6369 7465 2d75 7322 3e3c 2f61  id="cite-us"></a
-00001970: 3e0a 0a49 6620 796f 7520 7573 6520 546f  >..If you use To
-00001980: 6f6c 7320 4b69 7420 696e 2079 6f75 7220  ols Kit in your 
-00001990: 7265 7365 6172 6368 2077 6f72 6b20 6f72  research work or
-000019a0: 2061 6361 6465 6d69 6320 7072 6f6a 6563   academic projec
-000019b0: 7473 2c20 7765 2077 6f75 6c64 2061 7070  ts, we would app
-000019c0: 7265 6369 6174 6520 6974 2069 6620 796f  reciate it if yo
-000019d0: 7520 636f 756c 6420 6369 7465 2075 732e  u could cite us.
-000019e0: 2059 6f75 2063 616e 2075 7365 2074 6865   You can use the
-000019f0: 2066 6f6c 6c6f 7769 6e67 2042 6962 5465   following BibTe
-00001a00: 5820 656e 7472 793a 0a0a 6060 6062 6962  X entry:..```bib
-00001a10: 7465 780a 406d 6973 637b 7072 6f6a 6563  tex.@misc{projec
-00001a20: 742d 7070 6368 656d 2d74 6f6f 6c73 2d6b  t-ppchem-tools-k
-00001a30: 6974 2c0a 2020 7469 746c 6520 3d20 7b50  it,.  title = {P
-00001a40: 726f 6a65 6374 2d70 7063 6865 6d2d 746f  roject-ppchem-to
-00001a50: 6f6c 732d 6b69 747d 2c0a 2020 6175 7468  ols-kit},.  auth
-00001a60: 6f72 203d 207b 7b4d c3a9 6c6f c3a9 2045  or = {{M..lo.. E
-00001a70: 6e7a 696e 6765 7220 2620 53c3 a962 6173  nzinger & S..bas
-00001a80: 7469 656e 2047 7275 6e62 6572 677d 7d2c  tien Grunberg}},
-00001a90: 0a20 2079 6561 7220 3d20 7b32 3032 347d  .  year = {2024}
-00001aa0: 2c0a 2020 7075 626c 6973 6865 7220 3d20  ,.  publisher = 
-00001ab0: 7b47 6974 4875 627d 2c0a 2020 6a6f 7572  {GitHub},.  jour
-00001ac0: 6e61 6c20 3d20 7b47 6974 4875 6220 5265  nal = {GitHub Re
-00001ad0: 706f 7369 746f 7279 7d2c 0a20 2068 6f77  pository},.  how
-00001ae0: 7075 626c 6973 6865 6420 3d20 7b5c 7572  published = {\ur
-00001af0: 6c7b 6874 7470 733a 2f2f 6769 7468 7562  l{https://github
-00001b00: 2e63 6f6d 2f75 7365 726e 616d 652f 5072  .com/username/Pr
-00001b10: 6f6a 6563 742d 7070 6368 656d 2d74 6f6f  oject-ppchem-too
-00001b20: 6c73 2d6b 6974 7d7d 0a7d 0a60 6060 0a0a  ls-kit}}.}.```..
-00001b30: 2323 2320 4368 6963 6167 6f20 5374 796c  ### Chicago Styl
-00001b40: 650a 6060 6062 6173 680a 456e 7a69 6e67  e.```bash.Enzing
-00001b50: 6572 2c20 4dc3 a96c 6fc3 a92c 2061 6e64  er, M..lo.., and
-00001b60: 2053 c3a9 6261 7374 6965 6e20 4772 756e   S..bastien Grun
-00001b70: 6265 7267 2e20 3230 3234 2e20 5072 6f6a  berg. 2024. Proj
-00001b80: 6563 742d 7070 6368 656d 2d74 6f6f 6c73  ect-ppchem-tools
-00001b90: 2d6b 6974 2e20 436f 6d70 7574 6572 2073  -kit. Computer s
-00001ba0: 6f66 7477 6172 652e 2047 6974 4875 622e  oftware. GitHub.
-00001bb0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00001bc0: 636f 6d2f 7573 6572 6e61 6d65 2f50 726f  com/username/Pro
-00001bd0: 6a65 6374 2d70 7063 6865 6d2d 746f 6f6c  ject-ppchem-tool
-00001be0: 732d 6b69 742e 6020 0a60 6060 0a23 2320  s-kit.` .```.## 
-00001bf0: f09f 939c 204c 6963 656e 7365 0a3c 6120  .... License.<a 
-00001c00: 6964 3d22 6c69 6365 6e73 6522 3e3c 2f61  id="license"></a
-00001c10: 3e0a 0a54 6869 7320 7072 6f6a 6563 7420  >..This project 
-00001c20: 6973 206c 6963 656e 7365 6420 756e 6465  is licensed unde
-00001c30: 7220 7468 6520 4d49 5420 4c69 6365 6e73  r the MIT Licens
-00001c40: 652e 2053 6565 2074 6865 204c 4943 454e  e. See the LICEN
-00001c50: 5345 2066 696c 6520 666f 7220 6465 7461  SE file for deta
-00001c60: 696c 732e 0a0a 2323 20f0 9f93 b820 5363  ils...## .... Sc
-00001c70: 7265 656e 7368 6f74 730a 3c61 2069 643d  reenshots.<a id=
-00001c80: 2273 6372 6565 6e73 686f 7473 223e 3c2f  "screenshots"></
-00001c90: 613e 0a0a 0a                             a>...
+00000040: 312e 310a 5375 6d6d 6172 793a 2042 6173  1.1.Summary: Bas
+00000050: 6963 2043 6865 6d69 7374 7279 2054 6f6f  ic Chemistry Too
+00000060: 6c6b 6974 0a4c 6963 656e 7365 3a20 4d49  lkit.License: MI
+00000070: 540a 4175 7468 6f72 3a20 4dc3 a96c 6fc3  T.Author: M..lo.
+00000080: a920 456e 7a69 6e67 6572 0a41 7574 686f  . Enzinger.Autho
+00000090: 722d 656d 6169 6c3a 206d 656c 6f65 2e65  r-email: meloe.e
+000000a0: 6e7a 696e 6765 7240 6570 666c 2e63 683e  nzinger@epfl.ch>
+000000b0: 2061 6e64 2053 c3a9 6261 7374 6965 6e20   and S..bastien 
+000000c0: 4772 756e 6265 7267 203c 7365 6261 7374  Grunberg <sebast
+000000d0: 6965 6e2e 6772 756e 6265 7267 4065 7066  ien.grunberg@epf
+000000e0: 6c2e 6368 0a52 6571 7569 7265 732d 5079  l.ch.Requires-Py
+000000f0: 7468 6f6e 3a20 3e3d 332e 3130 2c3c 342e  thon: >=3.10,<4.
+00000100: 300a 436c 6173 7369 6669 6572 3a20 4c69  0.Classifier: Li
+00000110: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000120: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000130: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+00000140: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000150: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000160: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
+00000170: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000180: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000190: 3a3a 2033 2e31 300a 436c 6173 7369 6669  :: 3.10.Classifi
+000001a0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000001b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001c0: 6f6e 203a 3a20 332e 3131 0a43 6c61 7373  on :: 3.11.Class
+000001d0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001f0: 7974 686f 6e20 3a3a 2033 2e31 320a 5265  ython :: 3.12.Re
+00000200: 7175 6972 6573 2d44 6973 743a 206d 6174  quires-Dist: mat
+00000210: 706c 6f74 6c69 6220 283d 3d33 2e37 2e32  plotlib (==3.7.2
+00000220: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+00000230: 206e 756d 7079 2028 3e3d 312e 3236 2e34   numpy (>=1.26.4
+00000240: 2c3c 322e 302e 3029 0a52 6571 7569 7265  ,<2.0.0).Require
+00000250: 732d 4469 7374 3a20 6e75 6d70 7935 2028  s-Dist: numpy5 (
+00000260: 3e3d 302e 312c 3c30 2e32 290a 5265 7175  >=0.1,<0.2).Requ
+00000270: 6972 6573 2d44 6973 743a 2070 616e 6461  ires-Dist: panda
+00000280: 7320 283d 3d32 2e30 2e33 290a 5265 7175  s (==2.0.3).Requ
+00000290: 6972 6573 2d44 6973 743a 2070 696c 6c6f  ires-Dist: pillo
+000002a0: 7720 283d 3d31 302e 322e 3029 0a52 6571  w (==10.2.0).Req
+000002b0: 7569 7265 732d 4469 7374 3a20 7075 6263  uires-Dist: pubc
+000002c0: 6865 6d70 7920 283d 3d31 2e30 2e34 290a  hempy (==1.0.4).
+000002d0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+000002e0: 7970 6572 636c 6970 2028 3d3d 312e 382e  yperclip (==1.8.
+000002f0: 3229 0a52 6571 7569 7265 732d 4469 7374  2).Requires-Dist
+00000300: 3a20 7264 6b69 7420 283d 3d32 3032 332e  : rdkit (==2023.
+00000310: 392e 3629 0a52 6571 7569 7265 732d 4469  9.6).Requires-Di
+00000320: 7374 3a20 7265 706f 7274 6c61 6220 283d  st: reportlab (=
+00000330: 3d34 2e32 2e30 290a 5265 7175 6972 6573  =4.2.0).Requires
+00000340: 2d44 6973 743a 2072 6571 7565 7374 7320  -Dist: requests 
+00000350: 283d 3d32 2e33 312e 3029 0a52 6571 7569  (==2.31.0).Requi
+00000360: 7265 732d 4469 7374 3a20 7363 696b 6974  res-Dist: scikit
+00000370: 2d6c 6561 726e 2028 3d3d 312e 332e 3029  -learn (==1.3.0)
+00000380: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000390: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000003a0: 6d61 726b 646f 776e 0a0a 0a3c 7020 616c  markdown...<p al
+000003b0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+000003c0: 203c 696d 6720 7769 6474 683d 2231 3234   <img width="124
+000003d0: 3522 2061 6c74 3d22 6c6f 676f 5f70 726f  5" alt="logo_pro
+000003e0: 6a65 6374 2220 7372 633d 2268 7474 7073  ject" src="https
+000003f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7367  ://github.com/sg
+00000400: 7275 6e62 6572 2f50 726f 6a65 6374 2d70  runber/Project-p
+00000410: 7063 6865 6d2d 746f 6f6c 732d 6b69 742f  pchem-tools-kit/
+00000420: 7261 772f 6d61 696e 2f64 6f63 732f 736f  raw/main/docs/so
+00000430: 7572 6365 2f5f 7374 6174 6963 2f69 6d61  urce/_static/ima
+00000440: 6765 732f 6c6f 676f 5f70 726f 6a65 6374  ges/logo_project
+00000450: 2e70 6e67 223e 0a0a 203c 2f70 3e0a 0a0a  .png">.. </p>...
+00000460: 0a0a 203c 6831 2061 6c69 676e 3d22 6365  .. <h1 align="ce
+00000470: 6e74 6572 223e f09f a7b0 2054 6f6f 6c73  nter">.... Tools
+00000480: 204b 6974 3c2f 6831 3e0a 0a20 3c70 2061   Kit</h1>.. <p a
+00000490: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+000004a0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000004b0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6772  //github.com/sgr
+000004c0: 756e 6265 722f 5072 6f6a 6563 742d 7070  unber/Project-pp
+000004d0: 6368 656d 2d74 6f6f 6c73 2d6b 6974 2f61  chem-tools-kit/a
+000004e0: 6374 696f 6e73 223e 3c69 6d67 2073 7263  ctions"><img src
+000004f0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000500: 6965 6c64 732e 696f 2f62 6164 6765 2f62  ields.io/badge/b
+00000510: 7569 6c64 2d70 6173 7369 6e67 2d62 7269  uild-passing-bri
+00000520: 6768 7467 7265 656e 2220 616c 743d 2242  ghtgreen" alt="B
+00000530: 7569 6c64 2053 7461 7475 7322 3e3c 2f61  uild Status"></a
+00000540: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+00000550: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000560: 7367 7275 6e62 6572 2f50 726f 6a65 6374  sgrunber/Project
+00000570: 2d70 7063 6865 6d2d 746f 6f6c 732d 6b69  -ppchem-tools-ki
+00000580: 7422 3e3c 696d 6720 7372 633d 2268 7474  t"><img src="htt
+00000590: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000005a0: 2e69 6f2f 6261 6467 652f 636f 7665 7261  .io/badge/covera
+000005b0: 6765 2d39 3525 3235 2d62 7269 6768 7467  ge-95%25-brightg
+000005c0: 7265 656e 2220 616c 743d 2243 6f76 6572  reen" alt="Cover
+000005d0: 6167 6522 3e3c 2f61 3e0a 2020 3c61 2068  age"></a>.  <a h
+000005e0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+000005f0: 6875 622e 636f 6d2f 7367 7275 6e62 6572  hub.com/sgrunber
+00000600: 2f50 726f 6a65 6374 2d70 7063 6865 6d2d  /Project-ppchem-
+00000610: 746f 6f6c 732d 6b69 742f 626c 6f62 2f6d  tools-kit/blob/m
+00000620: 6169 6e2f 4c49 4345 4e53 4522 3e3c 696d  ain/LICENSE"><im
+00000630: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000640: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000650: 6467 652f 6c69 6365 6e73 652d 4d49 542d  dge/license-MIT-
+00000660: 626c 7565 2220 616c 743d 224c 6963 656e  blue" alt="Licen
+00000670: 7365 223e 3c2f 613e 0a3c 2f70 3e0a 0a23  se"></a>.</p>..#
+00000680: 2320 f09f 9396 2044 6573 6372 6970 7469  # .... Descripti
+00000690: 6f6e 0a54 6865 202a 2a54 6f6f 6c73 204b  on.The **Tools K
+000006a0: 6974 2a2a 2070 6163 6b61 6765 2061 6c6c  it** package all
+000006b0: 6f77 7320 6368 656d 6973 7472 7920 7374  ows chemistry st
+000006c0: 7564 656e 7473 2074 6f20 6669 6e64 2062  udents to find b
+000006d0: 6173 6963 2069 6e66 6f72 6d61 7469 6f6e  asic information
+000006e0: 206f 6e20 6d6f 6c65 6375 6c65 7320 616e   on molecules an
+000006f0: 6420 7072 6f76 6964 6573 2065 6173 7920  d provides easy 
+00000700: 6163 6365 7373 2074 6f20 736f 6d65 2067  access to some g
+00000710: 7261 7068 7320 616e 6420 6361 6c63 756c  raphs and calcul
+00000720: 6174 696f 6e73 2072 6571 7569 7265 6420  ations required 
+00000730: 696e 2065 7870 6572 696d 656e 7461 6c20  in experimental 
+00000740: 6c61 626f 7261 746f 7269 6573 2e0a 0a2a  laboratories...*
+00000750: 2af0 9f8c 9920 4e6f 7465 2a2a 3a20 466f  *.... Note**: Fo
+00000760: 7220 616e 2061 6573 7468 6574 6963 616c  r an aesthetical
+00000770: 6c79 2070 6c65 6173 696e 6720 6578 7065  ly pleasing expe
+00000780: 7269 656e 6365 2c20 6974 2069 7320 7265  rience, it is re
+00000790: 636f 6d6d 656e 6465 6420 746f 2075 7365  commended to use
+000007a0: 2074 6865 2064 6172 6b20 6d6f 6465 2069   the dark mode i
+000007b0: 6e74 6572 6661 6365 2069 6620 796f 7520  nterface if you 
+000007c0: 6172 6520 6f6e 2061 204d 6163 206f 7220  are on a Mac or 
+000007d0: 616e 7920 6f74 6865 7220 706c 6174 666f  any other platfo
+000007e0: 726d 2074 6861 7420 7375 7070 6f72 7473  rm that supports
+000007f0: 2069 742e 0a0a 0a23 2320 f09f 939a 2054   it....## .... T
+00000800: 6162 6c65 206f 6620 436f 6e74 656e 7473  able of Contents
+00000810: 0a2d 205b 496e 7374 616c 6c61 7469 6f6e  .- [Installation
+00000820: 5d28 23ef b88f 2d69 6e73 7461 6c6c 6174  ](#...-installat
+00000830: 696f 6e29 0a2d 205b 5573 6167 655d 2823  ion).- [Usage](#
+00000840: efb8 8f2d 7573 6167 6529 0a2d 205b 4665  ...-usage).- [Fe
+00000850: 6174 7572 6573 5d28 23ef b88f 2d66 6561  atures](#...-fea
+00000860: 7475 7265 7329 0a2d 205b 436f 6e74 7269  tures).- [Contri
+00000870: 6275 7469 6e67 5d28 23ef b88f 2d63 6f6e  buting](#...-con
+00000880: 7472 6962 7574 696e 6729 0a2d 205b 4369  tributing).- [Ci
+00000890: 7465 2055 735d 2823 efb8 8f2d 6369 7465  te Us](#...-cite
+000008a0: 2d75 7329 0a2d 205b 4c69 6365 6e73 655d  -us).- [License]
+000008b0: 2823 efb8 8f2d 6c69 6365 6e73 6529 0a2d  (#...-license).-
+000008c0: 205b 5363 7265 656e 7368 6f74 735d 2823   [Screenshots](#
+000008d0: efb8 8f2d 7363 7265 656e 7368 6f74 7329  ...-screenshots)
+000008e0: 0a0a 2323 20f0 9f9b a0ef b88f 2049 6e73  ..## ....... Ins
+000008f0: 7461 6c6c 6174 696f 6e0a 3c61 2069 643d  tallation.<a id=
+00000900: 2269 6e73 7461 6c6c 6174 696f 6e22 3e3c  "installation"><
+00000910: 2f61 3e0a 2323 2320 312e 20f0 9f8d b420  /a>.### 1. .... 
+00000920: 466f 726b 2074 6865 2052 6570 6f73 6974  Fork the Reposit
+00000930: 6f72 790a 546f 2073 7461 7274 2c20 666f  ory.To start, fo
+00000940: 726b 2074 6865 2072 6570 6f73 6974 6f72  rk the repositor
+00000950: 7920 746f 2079 6f75 7220 6f77 6e20 4769  y to your own Gi
+00000960: 7448 7562 2061 6363 6f75 6e74 2e20 200a  tHub account.  .
+00000970: 546f 2064 6f20 736f 2c20 6e61 7669 6761  To do so, naviga
+00000980: 7465 2074 6f20 7468 6520 7265 706f 7369  te to the reposi
+00000990: 746f 7279 2070 6167 6520 616e 6420 636c  tory page and cl
+000009a0: 6963 6b20 7468 6520 2a22 466f 726b 222a  ick the *"Fork"*
+000009b0: 2062 7574 746f 6e2e 2054 6865 2072 6570   button. The rep
+000009c0: 6f73 6974 6f72 7920 7769 6c6c 2074 6865  ository will the
+000009d0: 6e20 6265 2063 6f70 6965 6420 746f 2079  n be copied to y
+000009e0: 6f75 7220 6163 636f 756e 742c 2061 6e64  our account, and
+000009f0: 2079 6f75 2077 696c 6c20 6265 2061 626c   you will be abl
+00000a00: 6520 746f 2061 6363 6573 7320 6974 2e0a  e to access it..
+00000a10: 0a23 2323 2032 2e20 f09f 93a5 2043 6c6f  .### 2. .... Clo
+00000a20: 6e65 2074 6865 2052 6570 6f73 6974 6f72  ne the Repositor
+00000a30: 790a 4e65 7874 2c20 636c 6f6e 6520 7468  y.Next, clone th
+00000a40: 6520 7265 706f 7369 746f 7279 2075 7369  e repository usi
+00000a50: 6e67 2074 6865 2066 6f6c 6c6f 7769 6e67  ng the following
+00000a60: 2063 6f6d 6d61 6e64 2028 7265 706c 6163   command (replac
+00000a70: 6520 2a75 7365 726e 616d 652a 2077 6974  e *username* wit
+00000a80: 6820 796f 7572 2047 6974 4875 6220 7573  h your GitHub us
+00000a90: 6572 6e61 6d65 293a 0a0a 6060 6062 6173  ername):..```bas
+00000aa0: 680a 6769 7420 636c 6f6e 6520 6874 7470  h.git clone http
+00000ab0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f2a  s://github.com/*
+00000ac0: 7573 6572 6e61 6d65 2a2f 5072 6f6a 6563  username*/Projec
+00000ad0: 742d 7070 6368 656d 2d74 6f6f 6c73 2d6b  t-ppchem-tools-k
+00000ae0: 6974 2e67 6974 0a60 6060 0a0a 2323 2320  it.git.```..### 
+00000af0: 332e 20e2 ac87 efb8 8f20 496e 7374 616c  3. ...... Instal
+00000b00: 6c20 7769 7468 2070 6970 0a59 6f75 2063  l with pip.You c
+00000b10: 616e 2061 6c73 6f20 696e 7374 616c 6c20  an also install 
+00000b20: 546f 6f6c 7320 4b69 7420 7573 696e 6720  Tools Kit using 
+00000b30: 7069 703a 0a0a 6060 6062 6173 680a 7069  pip:..```bash.pi
+00000b40: 7020 696e 7374 616c 6c20 5072 6f6a 6563  p install Projec
+00000b50: 745f 7070 6368 656d 2d74 6f6f 6c73 2d6b  t_ppchem-tools-k
+00000b60: 6974 0a60 6060 0a0a 2323 20f0 9f9a 8020  it.```..## .... 
+00000b70: 5573 6167 650a 3c61 2069 643d 2275 7361  Usage.<a id="usa
+00000b80: 6765 223e 3c2f 613e 0a0a 546f 2075 7365  ge"></a>..To use
+00000b90: 2054 6f6f 6c73 204b 6974 2061 6e64 2061   Tools Kit and a
+00000ba0: 6363 6573 7320 6974 7320 6665 6174 7572  ccess its featur
+00000bb0: 6573 2c20 666f 6c6c 6f77 2074 6865 7365  es, follow these
+00000bc0: 2073 7465 7073 2061 6674 6572 2063 6c6f   steps after clo
+00000bd0: 6e69 6e67 2074 6865 2072 6570 6f73 6974  ning the reposit
+00000be0: 6f72 793a 0a0a 2323 2320 5573 696e 6720  ory:..### Using 
+00000bf0: 4a75 7079 7465 7220 4e6f 7465 626f 6f6b  Jupyter Notebook
+00000c00: 3a0a 0a31 2e20 4c61 756e 6368 204a 7570  :..1. Launch Jup
+00000c10: 7974 6572 204e 6f74 6562 6f6f 6b20 6279  yter Notebook by
+00000c20: 206e 6176 6967 6174 696e 6720 746f 2074   navigating to t
+00000c30: 6865 2063 6c6f 6e65 6420 7265 706f 7369  he cloned reposi
+00000c40: 746f 7279 2064 6972 6563 746f 7279 2069  tory directory i
+00000c50: 6e20 796f 7572 2074 6572 6d69 6e61 6c20  n your terminal 
+00000c60: 616e 6420 7275 6e6e 696e 6720 7468 6520  and running the 
+00000c70: 636f 6d6d 616e 643a 0a20 2020 6060 6062  command:.   ```b
+00000c80: 6173 680a 2020 206a 7570 7974 6572 206e  ash.   jupyter n
+00000c90: 6f74 6562 6f6f 6b0a 2020 2060 6060 0a32  otebook.   ```.2
+00000ca0: 2e20 496e 2074 6865 204a 7570 7974 6572  . In the Jupyter
+00000cb0: 204e 6f74 6562 6f6f 6b20 696e 7465 7266   Notebook interf
+00000cc0: 6163 652c 206e 6176 6967 6174 6520 746f  ace, navigate to
+00000cd0: 2074 6865 2060 6e6f 7465 626f 6f6b 7360   the `notebooks`
+00000ce0: 2064 6972 6563 746f 7279 2e0a 0a33 2e20   directory...3. 
+00000cf0: 4f70 656e 2074 6865 206e 6f74 6562 6f6f  Open the noteboo
+00000d00: 6b20 6e61 6d65 6420 6070 726f 6a65 6374  k named `project
+00000d10: 5f72 6570 6f72 742e 6970 796e 6260 2e0a  _report.ipynb`..
+00000d20: 0a34 2e20 466f 6c6c 6f77 2074 6865 2069  .4. Follow the i
+00000d30: 6e73 7472 7563 7469 6f6e 7320 696e 7369  nstructions insi
+00000d40: 6465 2074 6865 206e 6f74 6562 6f6f 6b20  de the notebook 
+00000d50: 746f 2069 6e74 6572 6163 7420 7769 7468  to interact with
+00000d60: 2074 6865 2054 6f6f 6c73 204b 6974 2069   the Tools Kit i
+00000d70: 6e74 6572 6661 6365 2061 6e64 2075 7469  nterface and uti
+00000d80: 6c69 7a65 2069 7473 2066 6561 7475 7265  lize its feature
+00000d90: 7320 666f 7220 6d6f 6c65 6375 6c65 2061  s for molecule a
+00000da0: 6e61 6c79 7369 732c 2067 7261 7068 2070  nalysis, graph p
+00000db0: 6c6f 7474 696e 672c 2065 7272 6f72 2063  lotting, error c
+00000dc0: 616c 6375 6c61 7469 6f6e 2c20 616e 6420  alculation, and 
+00000dd0: 6d6f 7265 2e0a 5468 6973 206e 6f74 6562  more..This noteb
+00000de0: 6f6f 6b20 7072 6f76 6964 6573 2061 6e20  ook provides an 
+00000df0: 696e 7465 7261 6374 6976 6520 656e 7669  interactive envi
+00000e00: 726f 6e6d 656e 7420 666f 7220 636f 6e76  ronment for conv
+00000e10: 656e 6965 6e74 2075 7361 6765 206f 6620  enient usage of 
+00000e20: 546f 6f6c 7320 4b69 7420 6469 7265 6374  Tools Kit direct
+00000e30: 6c79 2077 6974 6869 6e20 5669 7375 616c  ly within Visual
+00000e40: 2053 7475 6469 6f20 436f 6465 2e0a 0a0a   Studio Code....
+00000e50: 2323 2320 5573 6167 6520 7769 7468 2056  ### Usage with V
+00000e60: 6973 7561 6c20 5374 7564 696f 2043 6f64  isual Studio Cod
+00000e70: 653a 0a0a 312e 204f 7065 6e20 5669 7375  e:..1. Open Visu
+00000e80: 616c 2053 7475 6469 6f20 436f 6465 2061  al Studio Code a
+00000e90: 6e64 206e 6176 6967 6174 6520 746f 2074  nd navigate to t
+00000ea0: 6865 2063 6c6f 6e65 6420 6469 7265 6374  he cloned direct
+00000eb0: 6f72 792e 0a0a 322e 2049 6e73 7461 6c6c  ory...2. Install
+00000ec0: 2074 6865 204a 7570 7974 6572 2065 7874   the Jupyter ext
+00000ed0: 656e 7369 6f6e 2069 6620 6e6f 7420 616c  ension if not al
+00000ee0: 7265 6164 7920 696e 7374 616c 6c65 642e  ready installed.
+00000ef0: 2059 6f75 2063 616e 2064 6f20 7468 6973   You can do this
+00000f00: 2062 7920 7365 6172 6368 696e 6720 666f   by searching fo
+00000f10: 7220 224a 7570 7974 6572 2220 696e 2074  r "Jupyter" in t
+00000f20: 6865 2045 7874 656e 7369 6f6e 7320 7669  he Extensions vi
+00000f30: 6577 2028 4374 726c 2b53 6869 6674 2b58  ew (Ctrl+Shift+X
+00000f40: 2920 616e 6420 696e 7374 616c 6c69 6e67  ) and installing
+00000f50: 2074 6865 2022 5079 7468 6f6e 2220 6578   the "Python" ex
+00000f60: 7465 6e73 696f 6e20 7061 636b 2e0a 0a33  tension pack...3
+00000f70: 2e20 4f70 656e 2074 6865 2060 6e6f 7465  . Open the `note
+00000f80: 626f 6f6b 7360 2064 6972 6563 746f 7279  books` directory
+00000f90: 2069 6e20 5669 7375 616c 2053 7475 6469   in Visual Studi
+00000fa0: 6f20 436f 6465 2e0a 0a34 2e20 4f70 656e  o Code...4. Open
+00000fb0: 2074 6865 206e 6f74 6562 6f6f 6b20 6e61   the notebook na
+00000fc0: 6d65 6420 6070 726f 6a65 6374 5f72 6570  med `project_rep
+00000fd0: 6f72 742e 6970 796e 6260 2e0a 0a35 2e20  ort.ipynb`...5. 
+00000fe0: 466f 6c6c 6f77 2074 6865 2069 6e73 7472  Follow the instr
+00000ff0: 7563 7469 6f6e 7320 696e 7369 6465 2074  uctions inside t
+00001000: 6865 206e 6f74 6562 6f6f 6b20 746f 2069  he notebook to i
+00001010: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
+00001020: 2054 6f6f 6c73 204b 6974 2069 6e74 6572   Tools Kit inter
+00001030: 6661 6365 2061 6e64 2075 7469 6c69 7a65  face and utilize
+00001040: 2069 7473 2066 6561 7475 7265 7320 666f   its features fo
+00001050: 7220 6d6f 6c65 6375 6c65 2061 6e61 6c79  r molecule analy
+00001060: 7369 732c 2067 7261 7068 2070 6c6f 7474  sis, graph plott
+00001070: 696e 672c 2065 7272 6f72 2063 616c 6375  ing, error calcu
+00001080: 6c61 7469 6f6e 2c20 616e 6420 6d6f 7265  lation, and more
+00001090: 2e0a 5468 6973 206e 6f74 6562 6f6f 6b20  ..This notebook 
+000010a0: 7072 6f76 6964 6573 2061 6e20 696e 7465  provides an inte
+000010b0: 7261 6374 6976 6520 656e 7669 726f 6e6d  ractive environm
+000010c0: 656e 7420 666f 7220 636f 6e76 656e 6965  ent for convenie
+000010d0: 6e74 2075 7361 6765 206f 6620 546f 6f6c  nt usage of Tool
+000010e0: 7320 4b69 7420 7769 7468 204a 7570 7974  s Kit with Jupyt
+000010f0: 6572 204e 6f74 6562 6f6f 6b2e 0a0a 2323  er Notebook...##
+00001100: 20f0 9fa7 aa20 4665 6174 7572 6573 0a0a   .... Features..
+00001110: 312e 20f0 9fa7 ac20 4d6f 6c65 6375 6c65  1. .... Molecule
+00001120: 204e 616d 650a 2020 202d 2049 6e70 7574   Name.   - Input
+00001130: 3a20 5261 7720 666f 726d 756c 6120 6f66  : Raw formula of
+00001140: 2074 6865 206d 6f6c 6563 756c 650a 2020   the molecule.  
+00001150: 202d 204f 7574 7075 743a 2053 4d49 4c45   - Output: SMILE
+00001160: 5320 6f66 2074 6865 206d 6f6c 6563 756c  S of the molecul
+00001170: 650a 0a32 2e20 e29a 96ef b88f 204d 6f6c  e..2. ...... Mol
+00001180: 6563 756c 6172 2057 6569 6768 740a 2020  ecular Weight.  
+00001190: 202d 2049 6e70 7574 3a20 534d 494c 4553   - Input: SMILES
+000011a0: 206f 6620 7468 6520 6d6f 6c65 6375 6c65   of the molecule
+000011b0: 0a20 2020 2d20 4f75 7470 7574 3a20 436f  .   - Output: Co
+000011c0: 7272 6573 706f 6e64 696e 6720 6d6f 6c61  rresponding mola
+000011d0: 7220 6d61 7373 2069 6e20 672f 6d6f 6c0a  r mass in g/mol.
+000011e0: 0a33 2e20 f09f 9388 204c 696e 6561 7220  .3. .... Linear 
+000011f0: 5265 6772 6573 7369 6f6e 0a20 2020 2d20  Regression.   - 
+00001200: 496e 7075 743a 2045 7863 656c 2064 6f63  Input: Excel doc
+00001210: 756d 656e 7420 2869 6d70 6f72 7465 6420  ument (imported 
+00001220: 6279 2070 7265 7373 696e 6720 7468 6520  by pressing the 
+00001230: 4272 6f77 7365 2062 7574 746f 6e29 0a20  Browse button). 
+00001240: 2020 2d20 4f75 7470 7574 3a20 4c69 6e65    - Output: Line
+00001250: 6172 2072 6567 7265 7373 696f 6e20 6772  ar regression gr
+00001260: 6170 6820 7769 7468 2074 6865 2052 3c73  aph with the R<s
+00001270: 7570 3e32 3c2f 7375 703e 2076 616c 7565  up>2</sup> value
+00001280: 0a0a 342e 20f0 9f93 8a20 4772 6170 6820  ..4. .... Graph 
+00001290: 4d61 6b65 720a 2020 202d 2049 6e70 7574  Maker.   - Input
+000012a0: 3a20 4578 6365 6c20 646f 6375 6d65 6e74  : Excel document
+000012b0: 2077 6974 6820 7820 616e 6420 7920 7661   with x and y va
+000012c0: 6c75 6573 2061 7272 616e 6765 6420 696e  lues arranged in
+000012d0: 2074 776f 2063 6f6c 756d 6e73 0a20 2020   two columns.   
+000012e0: 2d20 4f75 7470 7574 3a20 4772 6170 6820  - Output: Graph 
+000012f0: 706c 6f74 7469 6e67 2061 6c6c 2076 616c  plotting all val
+00001300: 7565 730a 2020 2020 2020 2d20 4f70 7469  ues.      - Opti
+00001310: 6f6e 733a 2054 6865 2067 7261 7068 2061  ons: The graph a
+00001320: 6c6c 6f77 7320 6375 7374 6f6d 697a 6174  llows customizat
+00001330: 696f 6e20 6f66 2076 6172 696f 7573 2070  ion of various p
+00001340: 6172 616d 6574 6572 7320 7375 6368 2061  arameters such a
+00001350: 7320 6368 616e 6769 6e67 2073 6361 6c65  s changing scale
+00001360: 732c 2061 7869 7320 6c61 6265 6c73 2c20  s, axis labels, 
+00001370: 7469 746c 652c 2064 6973 706c 6179 696e  title, displayin
+00001380: 6720 6d61 7869 6d75 6d20 7661 6c75 6573  g maximum values
+00001390: 2c20 656e 6162 6c69 6e67 2067 7269 646c  , enabling gridl
+000013a0: 696e 6573 2c20 6164 6a75 7374 696e 6720  ines, adjusting 
+000013b0: 6c69 6e65 2074 7970 6573 2061 6e64 2063  line types and c
+000013c0: 6f6c 6f72 732c 206d 6f64 6966 7969 6e67  olors, modifying
+000013d0: 2067 7269 6420 616e 6420 6c61 6265 6c20   grid and label 
+000013e0: 6178 6573 2c20 616e 6420 6261 636b 6772  axes, and backgr
+000013f0: 6f75 6e64 2063 6f6c 6f72 2e0a 0a0a 352e  ound color....5.
+00001400: 20f0 9f93 8920 4572 726f 7220 5072 6f70   .... Error Prop
+00001410: 6167 6174 696f 6e0a 2020 202d 2049 6e70  agation.   - Inp
+00001420: 7574 3a20 5661 7269 6162 6c65 732c 2074  ut: Variables, t
+00001430: 6865 6972 2076 616c 7565 732c 2061 6e64  heir values, and
+00001440: 2074 6865 6972 2075 6e63 6572 7461 696e   their uncertain
+00001450: 7469 6573 2e0a 2020 202d 204f 7574 7075  ties..   - Outpu
+00001460: 743a 204d 6561 6e20 7661 6c75 652c 2069  t: Mean value, i
+00001470: 7473 2075 6e63 6572 7461 696e 7479 2c20  ts uncertainty, 
+00001480: 616e 6420 7468 6520 7265 7375 6c74 2063  and the result c
+00001490: 616e 2062 6520 636f 7069 6564 2061 7320  an be copied as 
+000014a0: 4c61 5465 5820 636f 6465 2066 6f72 2065  LaTeX code for e
+000014b0: 6173 7920 696e 636c 7573 696f 6e20 696e  asy inclusion in
+000014c0: 2064 6f63 756d 656e 7473 2e0a 0a36 2e20   documents...6. 
+000014d0: f09f a7aa 2053 686f 7720 4d6f 6c65 6375  .... Show Molecu
+000014e0: 6c65 0a20 2020 2d20 496e 7075 743a 2053  le.   - Input: S
+000014f0: 4d49 4c45 530a 2020 202d 204f 7574 7075  MILES.   - Outpu
+00001500: 743a 204d 6f6c 6563 756c 6172 2073 7472  t: Molecular str
+00001510: 7563 7475 7265 0a0a 5468 6520 6772 6170  ucture..The grap
+00001520: 6873 2069 6e20 7365 6374 696f 6e73 2033  hs in sections 3
+00001530: 2061 6e64 2034 2063 616e 2061 6c73 6f20   and 4 can also 
+00001540: 696e 636c 7564 6520 696e 7075 7420 666f  include input fo
+00001550: 7220 7468 6520 7469 746c 6520 616e 6420  r the title and 
+00001560: 582c 2059 2061 7869 7320 6c61 6265 6c73  X, Y axis labels
+00001570: 2e0a 0a23 2320 f09f a49d 2043 6f6e 7472  ...## .... Contr
+00001580: 6962 7574 696e 670a 3c61 2069 643d 2263  ibuting.<a id="c
+00001590: 6f6e 7472 6962 7574 696e 6722 3e3c 2f61  ontributing"></a
+000015a0: 3e0a 0a43 6f6e 7472 6962 7574 696f 6e73  >..Contributions
+000015b0: 2061 7265 2077 656c 636f 6d65 2120 546f   are welcome! To
+000015c0: 2063 6f6e 7472 6962 7574 6520 746f 202a   contribute to *
+000015d0: 2a54 6f6f 6c73 204b 6974 2a2a 2c20 706c  *Tools Kit**, pl
+000015e0: 6561 7365 2066 6f6c 6c6f 7720 7468 6573  ease follow thes
+000015f0: 6520 7374 6570 733a 0a0a 312e 202a 2a46  e steps:..1. **F
+00001600: 6f72 6b2a 2a20 7468 6520 7072 6f6a 6563  ork** the projec
+00001610: 7420 746f 2079 6f75 7220 4769 7448 7562  t to your GitHub
+00001620: 2061 6363 6f75 6e74 2e0a 322e 2043 7265   account..2. Cre
+00001630: 6174 6520 6120 6e65 7720 6272 616e 6368  ate a new branch
+00001640: 2066 6f72 2079 6f75 7220 6665 6174 7572   for your featur
+00001650: 6520 6f72 2062 7567 2066 6978 3a20 0a20  e or bug fix: . 
+00001660: 2020 6060 6062 6173 680a 2020 2067 6974    ```bash.   git
+00001670: 2063 6865 636b 6f75 7420 2d62 2066 6561   checkout -b fea
+00001680: 7475 7265 2f79 6f75 722d 6665 6174 7572  ture/your-featur
+00001690: 652d 6e61 6d65 0a20 2020 6060 600a 332e  e-name.   ```.3.
+000016a0: 202a 2a43 7265 6174 6520 6120 6e65 7720   **Create a new 
+000016b0: 6272 616e 6368 2066 6f72 2079 6f75 7220  branch for your 
+000016c0: 6665 6174 7572 6520 6f72 2062 7567 2066  feature or bug f
+000016d0: 6978 3a2a 2a0a 0a20 2020 2060 6060 6261  ix:**..    ```ba
+000016e0: 7368 0a20 2020 2067 6974 2063 6865 636b  sh.    git check
+000016f0: 6f75 7420 2d62 2066 6561 7475 7265 2f79  out -b feature/y
+00001700: 6f75 722d 6665 6174 7572 652d 6e61 6d65  our-feature-name
+00001710: 0a20 2020 2060 6060 0a0a 342e 202a 2a4d  .    ```..4. **M
+00001720: 616b 6520 796f 7572 2063 6861 6e67 6573  ake your changes
+00001730: 2061 6e64 2065 6e73 7572 6520 7468 6579   and ensure they
+00001740: 2061 6468 6572 6520 746f 2074 6865 2070   adhere to the p
+00001750: 726f 6a65 6374 2773 2063 6f64 696e 6720  roject's coding 
+00001760: 636f 6e76 656e 7469 6f6e 7320 616e 6420  conventions and 
+00001770: 7374 796c 6520 6775 6964 656c 696e 6573  style guidelines
+00001780: 2e2a 2a0a 0a35 2e20 2a2a 436f 6d6d 6974  .**..5. **Commit
+00001790: 2079 6f75 7220 6368 616e 6765 7320 7769   your changes wi
+000017a0: 7468 2064 6573 6372 6970 7469 7665 206d  th descriptive m
+000017b0: 6573 7361 6765 7320 6578 706c 6169 6e69  essages explaini
+000017c0: 6e67 2074 6865 2070 7572 706f 7365 206f  ng the purpose o
+000017d0: 6620 796f 7572 2063 6861 6e67 6573 3a2a  f your changes:*
+000017e0: 2a0a 0a20 2020 2060 6060 6261 7368 0a20  *..    ```bash. 
+000017f0: 2020 2067 6974 2063 6f6d 6d69 7420 2d61     git commit -a
+00001800: 6d20 2741 6464 2073 6f6d 6520 6665 6174  m 'Add some feat
+00001810: 7572 6527 0a20 2020 2060 6060 0a0a 362e  ure'.    ```..6.
+00001820: 202a 2a50 7573 6820 796f 7572 2063 6861   **Push your cha
+00001830: 6e67 6573 2074 6f20 796f 7572 2062 7261  nges to your bra
+00001840: 6e63 6820 6f6e 2079 6f75 7220 666f 726b  nch on your fork
+00001850: 6564 2072 6570 6f73 6974 6f72 793a 2a2a  ed repository:**
+00001860: 0a0a 2020 2020 6060 6062 6173 680a 2020  ..    ```bash.  
+00001870: 2020 6769 7420 7075 7368 206f 7269 6769    git push origi
+00001880: 6e20 6665 6174 7572 652f 796f 7572 2d66  n feature/your-f
+00001890: 6561 7475 7265 2d6e 616d 650a 2020 2020  eature-name.    
+000018a0: 6060 600a 0a37 2e20 2a2a 4f6e 6365 2079  ```..7. **Once y
+000018b0: 6f75 2776 6520 7075 7368 6564 2079 6f75  ou've pushed you
+000018c0: 7220 6368 616e 6765 732c 2079 6f75 2063  r changes, you c
+000018d0: 616e 206f 7065 6e20 6120 5075 6c6c 2052  an open a Pull R
+000018e0: 6571 7565 7374 2028 5052 2920 696e 2074  equest (PR) in t
+000018f0: 6865 206f 7269 6769 6e61 6c20 7265 706f  he original repo
+00001900: 7369 746f 7279 2e20 5072 6f76 6964 6520  sitory. Provide 
+00001910: 6120 636c 6561 7220 6465 7363 7269 7074  a clear descript
+00001920: 696f 6e20 6f66 2074 6865 2063 6861 6e67  ion of the chang
+00001930: 6573 2079 6f75 2776 6520 6d61 6465 2069  es you've made i
+00001940: 6e20 7468 6520 5052 2e2a 2a0a 0a38 2e20  n the PR.**..8. 
+00001950: 2a2a 4166 7465 7220 7265 7669 6577 696e  **After reviewin
+00001960: 6720 796f 7572 2050 522c 2069 6620 6576  g your PR, if ev
+00001970: 6572 7974 6869 6e67 206c 6f6f 6b73 2067  erything looks g
+00001980: 6f6f 642c 2069 7420 7769 6c6c 2062 6520  ood, it will be 
+00001990: 6d65 7267 6564 2069 6e74 6f20 7468 6520  merged into the 
+000019a0: 6d61 696e 2072 6570 6f73 6974 6f72 792e  main repository.
+000019b0: 2043 6f6e 6772 6174 756c 6174 696f 6e73   Congratulations
+000019c0: 2c20 796f 7527 7665 2073 7563 6365 7373  , you've success
+000019d0: 6675 6c6c 7920 636f 6e74 7269 6275 7465  fully contribute
+000019e0: 6420 746f 202a 546f 6f6c 7320 4b69 742a  d to *Tools Kit*
+000019f0: 212a 2a0a 0a54 6861 6e6b 2079 6f75 2066  !**..Thank you f
+00001a00: 6f72 2079 6f75 7220 636f 6e74 7269 6275  or your contribu
+00001a10: 7469 6f6e 2120 596f 7572 2065 6666 6f72  tion! Your effor
+00001a20: 7473 2068 656c 7020 696d 7072 6f76 6520  ts help improve 
+00001a30: 7468 6520 7072 6f6a 6563 7420 666f 7220  the project for 
+00001a40: 6576 6572 796f 6e65 2e0a 0a23 2320 f09f  everyone...## ..
+00001a50: 939a 2043 6974 6520 5573 0a3c 6120 6964  .. Cite Us.<a id
+00001a60: 3d22 6369 7465 2d75 7322 3e3c 2f61 3e0a  ="cite-us"></a>.
+00001a70: 0a49 6620 796f 7520 7573 6520 546f 6f6c  .If you use Tool
+00001a80: 7320 4b69 7420 696e 2079 6f75 7220 7265  s Kit in your re
+00001a90: 7365 6172 6368 2077 6f72 6b20 6f72 2061  search work or a
+00001aa0: 6361 6465 6d69 6320 7072 6f6a 6563 7473  cademic projects
+00001ab0: 2c20 7765 2077 6f75 6c64 2061 7070 7265  , we would appre
+00001ac0: 6369 6174 6520 6974 2069 6620 796f 7520  ciate it if you 
+00001ad0: 636f 756c 6420 6369 7465 2075 732e 2059  could cite us. Y
+00001ae0: 6f75 2063 616e 2075 7365 2074 6865 2066  ou can use the f
+00001af0: 6f6c 6c6f 7769 6e67 2042 6962 5465 5820  ollowing BibTeX 
+00001b00: 656e 7472 793a 0a0a 6060 6062 6962 7465  entry:..```bibte
+00001b10: 780a 406d 6973 637b 7072 6f6a 6563 742d  x.@misc{project-
+00001b20: 7070 6368 656d 2d74 6f6f 6c73 2d6b 6974  ppchem-tools-kit
+00001b30: 2c0a 2020 7469 746c 6520 3d20 7b50 726f  ,.  title = {Pro
+00001b40: 6a65 6374 2d70 7063 6865 6d2d 746f 6f6c  ject-ppchem-tool
+00001b50: 732d 6b69 747d 2c0a 2020 6175 7468 6f72  s-kit},.  author
+00001b60: 203d 207b 7b4d c3a9 6c6f c3a9 2045 6e7a   = {{M..lo.. Enz
+00001b70: 696e 6765 7220 2620 53c3 a962 6173 7469  inger & S..basti
+00001b80: 656e 2047 7275 6e62 6572 677d 7d2c 0a20  en Grunberg}},. 
+00001b90: 2079 6561 7220 3d20 7b32 3032 347d 2c0a   year = {2024},.
+00001ba0: 2020 7075 626c 6973 6865 7220 3d20 7b47    publisher = {G
+00001bb0: 6974 4875 627d 2c0a 2020 6a6f 7572 6e61  itHub},.  journa
+00001bc0: 6c20 3d20 7b47 6974 4875 6220 5265 706f  l = {GitHub Repo
+00001bd0: 7369 746f 7279 7d2c 0a20 2068 6f77 7075  sitory},.  howpu
+00001be0: 626c 6973 6865 6420 3d20 7b5c 7572 6c7b  blished = {\url{
+00001bf0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001c00: 6f6d 2f75 7365 726e 616d 652f 5072 6f6a  om/username/Proj
+00001c10: 6563 742d 7070 6368 656d 2d74 6f6f 6c73  ect-ppchem-tools
+00001c20: 2d6b 6974 7d7d 0a7d 0a60 6060 0a0a 2323  -kit}}.}.```..##
+00001c30: 2320 4368 6963 6167 6f20 5374 796c 650a  # Chicago Style.
+00001c40: 6060 6062 6173 680a 456e 7a69 6e67 6572  ```bash.Enzinger
+00001c50: 2c20 4dc3 a96c 6fc3 a92c 2061 6e64 2053  , M..lo.., and S
+00001c60: c3a9 6261 7374 6965 6e20 4772 756e 6265  ..bastien Grunbe
+00001c70: 7267 2e20 3230 3234 2e20 5072 6f6a 6563  rg. 2024. Projec
+00001c80: 742d 7070 6368 656d 2d74 6f6f 6c73 2d6b  t-ppchem-tools-k
+00001c90: 6974 2e20 436f 6d70 7574 6572 2073 6f66  it. Computer sof
+00001ca0: 7477 6172 652e 2047 6974 4875 622e 2068  tware. GitHub. h
+00001cb0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001cc0: 6d2f 7573 6572 6e61 6d65 2f50 726f 6a65  m/username/Proje
+00001cd0: 6374 2d70 7063 6865 6d2d 746f 6f6c 732d  ct-ppchem-tools-
+00001ce0: 6b69 742e 6020 0a60 6060 0a23 2320 f09f  kit.` .```.## ..
+00001cf0: 939c 204c 6963 656e 7365 0a3c 6120 6964  .. License.<a id
+00001d00: 3d22 6c69 6365 6e73 6522 3e3c 2f61 3e0a  ="license"></a>.
+00001d10: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00001d20: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00001d30: 7468 6520 4d49 5420 4c69 6365 6e73 652e  the MIT License.
+00001d40: 2053 6565 2074 6865 204c 4943 454e 5345   See the LICENSE
+00001d50: 2066 696c 6520 666f 7220 6465 7461 696c   file for detail
+00001d60: 732e 0a0a 2323 20f0 9f93 b820 5363 7265  s...## .... Scre
+00001d70: 656e 7368 6f74 730a 3c61 2069 643d 2273  enshots.<a id="s
+00001d80: 6372 6565 6e73 686f 7473 223e 3c2f 613e  creenshots"></a>
+00001d90: 0a3c 696d 6720 7769 6474 683d 2231 3030  .<img width="100
+00001da0: 3222 2061 6c74 3d22 4361 7074 7572 6520  2" alt="Capture 
+00001db0: 64e2 8099 65cc 8163 7261 6e20 3230 3234  d...e..cran 2024
+00001dc0: 2d30 352d 3138 2061 cc80 2031 3620 3434  -05-18 a.. 16 44
+00001dd0: 2030 3922 2073 7263 3d22 6874 7470 733a   09" src="https:
+00001de0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6772  //github.com/sgr
+00001df0: 756e 6265 722f 5072 6f6a 6563 742d 7070  unber/Project-pp
+00001e00: 6368 656d 2d74 6f6f 6c73 2d6b 6974 2f61  chem-tools-kit/a
+00001e10: 7373 6574 732f 3136 3038 3831 3836 342f  ssets/160881864/
+00001e20: 6134 3433 3739 6634 2d38 6366 322d 3461  a44379f4-8cf2-4a
+00001e30: 6338 2d62 3337 302d 3336 6665 6535 3532  c8-b370-36fee552
+00001e40: 6565 3661 223e 0a0a 0a0a                 ee6a">....
```

