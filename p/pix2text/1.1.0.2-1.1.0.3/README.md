# Comparing `tmp/pix2text-1.1.0.2.tar.gz` & `tmp/pix2text-1.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix2text-1.1.0.2.tar", last modified: Fri May 10 08:29:54 2024, max compression
+gzip compressed data, was "pix2text-1.1.0.3.tar", last modified: Sun May 19 09:15:08 2024, max compression
```

## Comparing `pix2text-1.1.0.2.tar` & `pix2text-1.1.0.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.101494 pix2text-1.1.0.2/
--rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.1.0.2/LICENSE
--rw-r--r--   0 king       (501) staff       (20)    14138 2024-05-10 08:29:54.101276 pix2text-1.1.0.2/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    12919 2024-05-06 08:46:19.000000 pix2text-1.1.0.2/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.089170 pix2text-1.1.0.2/pix2text/
--rw-r--r--   0 king       (501) staff       (20)      456 2024-04-02 11:11:40.000000 pix2text-1.1.0.2/pix2text/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      203 2024-05-10 08:21:55.000000 pix2text-1.1.0.2/pix2text/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.1.0.2/pix2text/app.py
--rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.1.0.2/pix2text/category_mapping.py
--rw-r--r--   0 king       (501) staff       (20)    10451 2024-04-22 00:51:42.000000 pix2text-1.1.0.2/pix2text/cli.py
--rw-r--r--   0 king       (501) staff       (20)     3710 2024-04-16 14:50:16.000000 pix2text-1.1.0.2/pix2text/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.091837 pix2text-1.1.0.2/pix2text/doc_xl_layout/
--rw-r--r--   0 king       (501) staff       (20)      192 2024-04-03 01:13:56.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/__init__.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.092874 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     8390 2024-04-02 08:34:16.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/base_detector_subfield.py
--rw-r--r--   0 king       (501) staff       (20)     8722 2024-04-02 07:16:21.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/ctdet_subfield.py
--rw-r--r--   0 king       (501) staff       (20)      137 2024-04-02 06:45:51.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/detector_factory.py
--rw-r--r--   0 king       (501) staff       (20)    17861 2024-04-30 02:52:35.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/doc_xl_layout_parser.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.093174 pix2text-1.1.0.2/pix2text/doc_xl_layout/external/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/external/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2510 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/external/shapelyNMS.py
--rw-r--r--   0 king       (501) staff       (20)      365 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/huntie_subfield.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.094558 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     5178 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/data_parallel.py
--rw-r--r--   0 king       (501) staff       (20)    23840 2024-04-02 07:32:06.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/decode.py
--rw-r--r--   0 king       (501) staff       (20)     3443 2024-04-10 11:32:17.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/model.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.094873 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/networks/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/networks/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    24395 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py
--rw-r--r--   0 king       (501) staff       (20)     1528 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/scatter_gather.py
--rw-r--r--   0 king       (501) staff       (20)     1800 2024-04-02 07:31:48.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/utils.py
--rw-r--r--   0 king       (501) staff       (20)    23801 2024-04-02 00:43:23.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/opts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.096803 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4818 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/ddd_utils.py
--rw-r--r--   0 king       (501) staff       (20)    26623 2024-04-02 06:59:29.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/debugger.py
--rw-r--r--   0 king       (501) staff       (20)    18383 2024-04-02 06:47:12.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/evaluation_bk.py
--rw-r--r--   0 king       (501) staff       (20)     7851 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/image.py
--rw-r--r--   0 king       (501) staff       (20)     5368 2024-04-02 06:47:54.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/post_process.py
--rw-r--r--   0 king       (501) staff       (20)      533 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/utils.py
--rw-r--r--   0 king       (501) staff       (20)     8844 2024-04-02 06:20:49.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/wrapper.py
--rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.1.0.2/pix2text/element.py
--rw-r--r--   0 king       (501) staff       (20)    17431 2024-04-22 02:21:39.000000 pix2text-1.1.0.2/pix2text/latex_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.1.0.2/pix2text/latex_ocr0.py
--rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.1.0.2/pix2text/latex_recog.py
--rw-r--r--   0 king       (501) staff       (20)     4016 2024-04-06 13:32:28.000000 pix2text-1.1.0.2/pix2text/layout_parser.py
--rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.1.0.2/pix2text/object_detector.py
--rw-r--r--   0 king       (501) staff       (20)     7285 2024-04-27 13:58:01.000000 pix2text-1.1.0.2/pix2text/ocr_engine.py
--rw-r--r--   0 king       (501) staff       (20)    10497 2024-04-30 02:55:47.000000 pix2text-1.1.0.2/pix2text/page_elements.py
--rw-r--r--   0 king       (501) staff       (20)    28192 2024-04-24 14:01:37.000000 pix2text-1.1.0.2/pix2text/pix_to_text.py
--rw-r--r--   0 king       (501) staff       (20)     5413 2024-04-30 02:57:49.000000 pix2text-1.1.0.2/pix2text/render.py
--rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.1.0.2/pix2text/screenshot_daemon_with_server2.py
--rw-r--r--   0 king       (501) staff       (20)     2776 2024-04-21 15:29:44.000000 pix2text-1.1.0.2/pix2text/serve.py
--rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.1.0.2/pix2text/table_inference.py
--rw-r--r--   0 king       (501) staff       (20)    38370 2024-04-30 02:58:35.000000 pix2text-1.1.0.2/pix2text/table_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    37328 2024-03-29 23:43:03.000000 pix2text-1.1.0.2/pix2text/table_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)    24628 2024-04-22 00:24:28.000000 pix2text-1.1.0.2/pix2text/text_formula_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    31718 2024-05-10 08:12:46.000000 pix2text-1.1.0.2/pix2text/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.090366 pix2text-1.1.0.2/pix2text.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    14138 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     2405 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       42 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.1.0.2/pix2text.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      269 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)       17 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/top_level.txt
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.099933 pix2text-1.1.0.2/scripts/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.1.0.2/scripts/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.1.0.2/scripts/convert_label_studio_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.1.0.2/scripts/extract_p2t_results.py
--rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.1.0.2/scripts/gen_label_studio_json.py
--rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.1.0.2/scripts/gen_pure_formula_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.1.0.2/scripts/merge_label_studio_anno_pred_json.py
--rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.1.0.2/scripts/object_detection3.py
--rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.1.0.2/scripts/screenshot_daemon.py
--rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.1.0.2/scripts/try_easyocr.py
--rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.1.0.2/scripts/try_latex_correction.py
--rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.1.0.2/scripts/try_layout.py
--rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.1.0.2/scripts/try_pix2text_mfr.py
--rw-r--r--   0 king       (501) staff       (20)      845 2024-04-21 15:31:13.000000 pix2text-1.1.0.2/scripts/try_service.py
--rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.1.0.2/scripts/try_texify.py
--rw-r--r--   0 king       (501) staff       (20)       38 2024-05-10 08:29:54.101539 pix2text-1.1.0.2/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     2522 2024-04-30 03:06:08.000000 pix2text-1.1.0.2/setup.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.100682 pix2text-1.1.0.2/tests/
--rw-r--r--   0 king       (501) staff       (20)     5861 2024-04-10 11:52:24.000000 pix2text-1.1.0.2/tests/test_pix2text.py
--rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.1.0.2/tests/test_sort_boxes.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.282020 pix2text-1.1.0.3/
+-rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.1.0.3/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    14231 2024-05-19 09:15:08.281818 pix2text-1.1.0.3/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    13012 2024-05-12 07:12:01.000000 pix2text-1.1.0.3/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.269099 pix2text-1.1.0.3/pix2text/
+-rw-r--r--   0 king       (501) staff       (20)      456 2024-04-02 11:11:40.000000 pix2text-1.1.0.3/pix2text/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      203 2024-05-16 22:38:57.000000 pix2text-1.1.0.3/pix2text/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.1.0.3/pix2text/app.py
+-rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.1.0.3/pix2text/category_mapping.py
+-rw-r--r--   0 king       (501) staff       (20)    10451 2024-04-22 00:51:42.000000 pix2text-1.1.0.3/pix2text/cli.py
+-rw-r--r--   0 king       (501) staff       (20)     4158 2024-05-19 07:51:56.000000 pix2text-1.1.0.3/pix2text/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.271898 pix2text-1.1.0.3/pix2text/doc_xl_layout/
+-rw-r--r--   0 king       (501) staff       (20)      192 2024-04-03 01:13:56.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/__init__.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.272942 pix2text-1.1.0.3/pix2text/doc_xl_layout/detectors/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/detectors/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     8390 2024-04-02 08:34:16.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/detectors/base_detector_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     8722 2024-04-02 07:16:21.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/detectors/ctdet_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)      137 2024-04-02 06:45:51.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/detectors/detector_factory.py
+-rw-r--r--   0 king       (501) staff       (20)    17964 2024-05-16 22:26:07.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/doc_xl_layout_parser.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.273275 pix2text-1.1.0.3/pix2text/doc_xl_layout/external/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/external/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2510 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/external/shapelyNMS.py
+-rw-r--r--   0 king       (501) staff       (20)      365 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/huntie_subfield.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.274865 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     5178 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/data_parallel.py
+-rw-r--r--   0 king       (501) staff       (20)    23840 2024-04-02 07:32:06.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/decode.py
+-rw-r--r--   0 king       (501) staff       (20)     3443 2024-04-10 11:32:17.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/model.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.275173 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/networks/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/networks/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    24395 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     1528 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/scatter_gather.py
+-rw-r--r--   0 king       (501) staff       (20)     1800 2024-04-02 07:31:48.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/models/utils.py
+-rw-r--r--   0 king       (501) staff       (20)    23801 2024-04-02 00:43:23.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/opts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.277318 pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4818 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/ddd_utils.py
+-rw-r--r--   0 king       (501) staff       (20)    26623 2024-04-02 06:59:29.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/debugger.py
+-rw-r--r--   0 king       (501) staff       (20)    18383 2024-04-02 06:47:12.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/evaluation_bk.py
+-rw-r--r--   0 king       (501) staff       (20)     7851 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/image.py
+-rw-r--r--   0 king       (501) staff       (20)     5368 2024-04-02 06:47:54.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/post_process.py
+-rw-r--r--   0 king       (501) staff       (20)      533 2024-04-01 15:18:57.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/utils.py
+-rw-r--r--   0 king       (501) staff       (20)     8844 2024-04-02 06:20:49.000000 pix2text-1.1.0.3/pix2text/doc_xl_layout/wrapper.py
+-rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.1.0.3/pix2text/element.py
+-rw-r--r--   0 king       (501) staff       (20)    17923 2024-05-19 08:38:51.000000 pix2text-1.1.0.3/pix2text/latex_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.1.0.3/pix2text/latex_ocr0.py
+-rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.1.0.3/pix2text/latex_recog.py
+-rw-r--r--   0 king       (501) staff       (20)     4016 2024-04-06 13:32:28.000000 pix2text-1.1.0.3/pix2text/layout_parser.py
+-rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.1.0.3/pix2text/object_detector.py
+-rw-r--r--   0 king       (501) staff       (20)     7485 2024-05-16 22:36:06.000000 pix2text-1.1.0.3/pix2text/ocr_engine.py
+-rw-r--r--   0 king       (501) staff       (20)    10633 2024-05-12 14:22:25.000000 pix2text-1.1.0.3/pix2text/page_elements.py
+-rw-r--r--   0 king       (501) staff       (20)    28192 2024-04-24 14:01:37.000000 pix2text-1.1.0.3/pix2text/pix_to_text.py
+-rw-r--r--   0 king       (501) staff       (20)     5413 2024-04-30 02:57:49.000000 pix2text-1.1.0.3/pix2text/render.py
+-rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.1.0.3/pix2text/screenshot_daemon_with_server2.py
+-rw-r--r--   0 king       (501) staff       (20)     2776 2024-04-21 15:29:44.000000 pix2text-1.1.0.3/pix2text/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.1.0.3/pix2text/table_inference.py
+-rw-r--r--   0 king       (501) staff       (20)    38370 2024-04-30 02:58:35.000000 pix2text-1.1.0.3/pix2text/table_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    37328 2024-03-29 23:43:03.000000 pix2text-1.1.0.3/pix2text/table_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)    24628 2024-04-22 00:24:28.000000 pix2text-1.1.0.3/pix2text/text_formula_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    31718 2024-05-10 08:12:46.000000 pix2text-1.1.0.3/pix2text/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.270335 pix2text-1.1.0.3/pix2text.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    14231 2024-05-19 09:15:08.000000 pix2text-1.1.0.3/pix2text.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     2405 2024-05-19 09:15:08.000000 pix2text-1.1.0.3/pix2text.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2024-05-19 09:15:08.000000 pix2text-1.1.0.3/pix2text.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       42 2024-05-19 09:15:08.000000 pix2text-1.1.0.3/pix2text.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.1.0.3/pix2text.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      269 2024-05-19 09:15:08.000000 pix2text-1.1.0.3/pix2text.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)       17 2024-05-19 09:15:08.000000 pix2text-1.1.0.3/pix2text.egg-info/top_level.txt
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.280763 pix2text-1.1.0.3/scripts/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.1.0.3/scripts/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.1.0.3/scripts/convert_label_studio_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.1.0.3/scripts/extract_p2t_results.py
+-rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.1.0.3/scripts/gen_label_studio_json.py
+-rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.1.0.3/scripts/gen_pure_formula_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.1.0.3/scripts/merge_label_studio_anno_pred_json.py
+-rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.1.0.3/scripts/object_detection3.py
+-rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.1.0.3/scripts/screenshot_daemon.py
+-rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.1.0.3/scripts/try_easyocr.py
+-rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.1.0.3/scripts/try_latex_correction.py
+-rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.1.0.3/scripts/try_layout.py
+-rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.1.0.3/scripts/try_pix2text_mfr.py
+-rw-r--r--   0 king       (501) staff       (20)      845 2024-04-21 15:31:13.000000 pix2text-1.1.0.3/scripts/try_service.py
+-rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.1.0.3/scripts/try_texify.py
+-rw-r--r--   0 king       (501) staff       (20)       38 2024-05-19 09:15:08.282080 pix2text-1.1.0.3/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     2522 2024-04-30 03:06:08.000000 pix2text-1.1.0.3/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-19 09:15:08.281594 pix2text-1.1.0.3/tests/
+-rw-r--r--   0 king       (501) staff       (20)     5861 2024-04-10 11:52:24.000000 pix2text-1.1.0.3/tests/test_pix2text.py
+-rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.1.0.3/tests/test_sort_boxes.py
```

### Comparing `pix2text-1.1.0.2/LICENSE` & `pix2text-1.1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/PKG-INFO` & `pix2text-1.1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 1.1.0.2
+Version: 1.1.0.3
 Summary: An Open-Source Python3 tool for recognizing layouts, tables, math formulas, and text in images, converting them into Markdown format. A free alternative to Mathpix, empowering seamless conversion of visual content into text-based representations.
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
@@ -86,14 +86,18 @@
 - **Table Recognition Model**: [breezedeus/pix2text-table-rec](https://huggingface.co/breezedeus/pix2text-table-rec) ([Mirror](https://hf-mirror.com/breezedeus/pix2text-table-rec)).
 - **Text Recognition Engine**: Supports **80+ languages** such as **English, Simplified Chinese, Traditional Chinese, Vietnamese**, etc. For English and Simplified Chinese recognition, it uses the open-source OCR tool [CnOCR](https://github.com/breezedeus/cnocr), while for other languages, it uses the open-source OCR tool [EasyOCR](https://github.com/JaidedAI/EasyOCR).
 - **Mathematical Formula Detection Model (MFD)**: Mathematical formula detection model (MFD) from [CnSTD](https://github.com/breezedeus/cnstd).
 - **Mathematical Formula Recognition Model (MFR)**: [breezedeus/pix2text-mfr](https://huggingface.co/breezedeus/pix2text-mfr) ([Mirror](https://hf-mirror.com/breezedeus/pix2text-mfr)).
 
 Several models are contributed by other open-source authors, and their contributions are highly appreciated.
 
+<div align="center">
+  <img src="docs/figs/arch-flow.jpg" alt="Pix2Text Arch Flow"/>
+</div>
+
 For detailed explanations, please refer to the [Pix2Text Online Documentation/Models](https://pix2text.readthedocs.io/zh/latest/models/).
 
 <br/>
 
 As a Python3 toolkit, P2T may not be very user-friendly for those who are not familiar with Python. Therefore, we also provide a **[free-to-use P2T Online Web](https://p2t.breezedeus.com)**, where you can directly upload images and get P2T parsing results. The web version uses the latest models, resulting in better performance compared to the open-source models.
 
 If you're interested, feel free to add the assistant as a friend by scanning the QR code and mentioning `p2t`. The assistant will regularly invite everyone to join the group where the latest developments related to P2T tools will be announced:
```

### Comparing `pix2text-1.1.0.2/README.md` & `pix2text-1.1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 - **Table Recognition Model**: [breezedeus/pix2text-table-rec](https://huggingface.co/breezedeus/pix2text-table-rec) ([Mirror](https://hf-mirror.com/breezedeus/pix2text-table-rec)).
 - **Text Recognition Engine**: Supports **80+ languages** such as **English, Simplified Chinese, Traditional Chinese, Vietnamese**, etc. For English and Simplified Chinese recognition, it uses the open-source OCR tool [CnOCR](https://github.com/breezedeus/cnocr), while for other languages, it uses the open-source OCR tool [EasyOCR](https://github.com/JaidedAI/EasyOCR).
 - **Mathematical Formula Detection Model (MFD)**: Mathematical formula detection model (MFD) from [CnSTD](https://github.com/breezedeus/cnstd).
 - **Mathematical Formula Recognition Model (MFR)**: [breezedeus/pix2text-mfr](https://huggingface.co/breezedeus/pix2text-mfr) ([Mirror](https://hf-mirror.com/breezedeus/pix2text-mfr)).
 
 Several models are contributed by other open-source authors, and their contributions are highly appreciated.
 
+<div align="center">
+  <img src="docs/figs/arch-flow.jpg" alt="Pix2Text Arch Flow"/>
+</div>
+
 For detailed explanations, please refer to the [Pix2Text Online Documentation/Models](https://pix2text.readthedocs.io/zh/latest/models/).
 
 <br/>
 
 As a Python3 toolkit, P2T may not be very user-friendly for those who are not familiar with Python. Therefore, we also provide a **[free-to-use P2T Online Web](https://p2t.breezedeus.com)**, where you can directly upload images and get P2T parsing results. The web version uses the latest models, resulting in better performance compared to the open-source models.
 
 If you're interested, feel free to add the assistant as a friend by scanning the QR code and mentioning `p2t`. The assistant will regularly invite everyone to join the group where the latest developments related to P2T tools will be announced:
```

### Comparing `pix2text-1.1.0.2/pix2text/app.py` & `pix2text-1.1.0.3/pix2text/app.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/category_mapping.py` & `pix2text-1.1.0.3/pix2text/category_mapping.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/cli.py` & `pix2text-1.1.0.3/pix2text/cli.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/consts.py` & `pix2text-1.1.0.3/pix2text/consts.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,23 @@
                 'hf_model_id': 'breezedeus/pix2text-mfr-pro',
                 'local_model_id': 'mfr-pro-onnx',
             },
             ('mfr-pro', 'pytorch'): {
                 'filename': 'p2t-mfr-pro-pytorch.zip',  # download the file from CN OSS
                 'local_model_id': 'mfr-pro-pytorch',
             },
+            ('mfr-plus', 'onnx'): {
+                'filename': 'p2t-mfr-plus-onnx.zip',  # download the file from CN OSS
+                'hf_model_id': 'breezedeus/pix2text-mfr-plus',
+                'local_model_id': 'mfr-plus-onnx',
+            },
+            ('mfr-plus', 'pytorch'): {
+                'filename': 'p2t-mfr-plus-pytorch.zip',  # download the file from CN OSS
+                'local_model_id': 'mfr-plus-pytorch',
+            },
         }
     )
 
     P2T_MODELS = deepcopy(FREE_MODELS)
     P2T_MODELS.update(PAID_MODELS)
     OUTER_MODELS = {}
```

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/base_detector_subfield.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/detectors/base_detector_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/ctdet_subfield.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/detectors/ctdet_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/doc_xl_layout_parser.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/doc_xl_layout_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,17 +351,20 @@
         for _box_info in final_out:
             if _box_info['col_number'] != -2:
                 continue
             overlap_vals = []
             for col_number, col_info in column_meta.items():
                 overlap_val = x_overlap(_box_info, col_info, key='position')
                 overlap_vals.append([col_number, overlap_val])
-            overlap_vals.sort(key=lambda x: (x[1], x[0]), reverse=True)
-            match_col_number = overlap_vals[0][0]
-            _box_info['col_number'] = match_col_number
+            if overlap_vals:
+                overlap_vals.sort(key=lambda x: (x[1], x[0]), reverse=True)
+                match_col_number = overlap_vals[0][0]
+                _box_info['col_number'] = match_col_number
+            else:
+                _box_info['col_number'] = 0
 
         return final_out, column_meta
 
     def _merge_overlapped_boxes(self, layout_out):
         """
         Detected bounding boxes may overlap; merge these overlapping boxes into a single one.
         """
```

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/external/shapelyNMS.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/external/shapelyNMS.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/data_parallel.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/models/data_parallel.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/decode.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/models/decode.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/model.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/models/model.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/scatter_gather.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/models/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/utils.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/models/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/opts.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/opts.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/ddd_utils.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/ddd_utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/debugger.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/debugger.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/evaluation_bk.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/evaluation_bk.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/image.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/image.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/post_process.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/post_process.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/utils.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/doc_xl_layout/wrapper.py` & `pix2text-1.1.0.3/pix2text/doc_xl_layout/wrapper.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/element.py` & `pix2text-1.1.0.3/pix2text/element.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/latex_ocr.py` & `pix2text-1.1.0.3/pix2text/latex_ocr.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 from optimum.onnxruntime import ORTModelForVision2Seq
 from transformers import (
     TrOCRProcessor,
     VisionEncoderDecoderModel,
 )
 
 from PIL import Image
-from cnstd.utils import get_model_file
 from cnocr.utils import get_default_ort_providers
+from transformers.generation import (
+    GenerateEncoderDecoderOutput,
+    GenerateBeamEncoderDecoderOutput,
+)
 
 from .consts import MODEL_VERSION, AVAILABLE_MODELS
 from .utils import data_dir, select_device, prepare_imgs
 
 logger = logging.getLogger(__name__)
 
 
@@ -192,38 +195,48 @@
         pixel_values = self.processor(images=img_list, return_tensors="pt").pixel_values
         outs = self.model.generate(
             pixel_values.to(self.device),
             return_dict_in_generate=True,
             output_scores=True,
             **rec_config,
         )
-        logits = torch.stack(outs.scores, dim=1)
-        scores = torch.softmax(logits, dim=-1).max(dim=2).values
-
-        mean_probs = []
-        for idx, example in enumerate(scores):
-            cur_length = int(
-                (outs.sequences[idx] != self.processor.tokenizer.pad_token_id).sum()
-            )
-            assert cur_length > 1
-            # 获得几何平均值。注意：example中的第一个元素对应sequence中的第二个元素
-            mean_probs.append(
-                float((example[: cur_length - 1] + 1e-8).log().mean().exp())
-            )
+        mean_probs = self._cal_scores(outs)
 
         generated_text = self.processor.batch_decode(
             outs.sequences, skip_special_tokens=True
         )
         assert len(img_list) == len(generated_text) == len(mean_probs)
 
         final_out = []
         for text, prob in zip(generated_text, mean_probs):
             final_out.append({'text': text, 'score': prob})
         return final_out
 
+    def _cal_scores(self, outs):
+        if isinstance(outs, GenerateBeamEncoderDecoderOutput):
+            mean_probs = outs.sequences_scores.exp().tolist()
+        elif isinstance(outs, GenerateEncoderDecoderOutput):
+            logits = torch.stack(outs.scores, dim=1)
+            scores = torch.softmax(logits, dim=-1).max(dim=2).values
+
+            mean_probs = []
+            for idx, example in enumerate(scores):
+                cur_length = int(
+                    (outs.sequences[idx] != self.processor.tokenizer.pad_token_id).sum()
+                )
+                assert cur_length > 1
+                # 获得几何平均值。注意：example中的第一个元素对应sequence中的第二个元素
+                mean_probs.append(
+                    float((example[: cur_length - 1] + 1e-8).log().mean().exp())
+                )
+        else:
+            raise Exception(f'unprocessed output type: {type(outs)}')
+
+        return mean_probs
+
     def post_process(self, text):
         text = remove_redundant_script(text)
         text = remove_trailing_whitespace(text)
         text = replace_illegal_symbols(text)
         for _ in range(10):
             new_text = remove_empty_text(text)
             if new_text == text:
@@ -243,18 +256,18 @@
     pattern = r'^_\s*{\s*(.*?)\s*}'
     result = re.sub(pattern, r'\1', result)
     return result.strip()
 
 
 def replace_illegal_symbols(text):
     illegal_to_legals = [
-        (r'\\\.', r'\\ .'),   # \. -> \ .
-        (r'\\=', r'\\ ='),   # \= -> \ =
-        (r'\\-', r'\\ -'),   # \- -> \ -
-        (r'\\~', r'\\ ~'),   # \~ -> \ ~
+        (r'\\\.', r'\\ .'),  # \. -> \ .
+        (r'\\=', r'\\ ='),  # \= -> \ =
+        (r'\\-', r'\\ -'),  # \- -> \ -
+        (r'\\~', r'\\ ~'),  # \~ -> \ ~
     ]
     for illegal, legal in illegal_to_legals:
         text = re.sub(illegal, legal, text)
     return text
 
 
 def remove_empty_text(latex_expression):
```

### Comparing `pix2text-1.1.0.2/pix2text/latex_ocr0.py` & `pix2text-1.1.0.3/pix2text/latex_ocr0.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/latex_recog.py` & `pix2text-1.1.0.3/pix2text/latex_recog.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/layout_parser.py` & `pix2text-1.1.0.3/pix2text/layout_parser.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/object_detector.py` & `pix2text-1.1.0.3/pix2text/object_detector.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/ocr_engine.py` & `pix2text-1.1.0.3/pix2text/ocr_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # coding: utf-8
 # [Pix2Text](https://github.com/breezedeus/pix2text): an Open-Source Alternative to Mathpix.
 # Copyright (C) 2022-2024, [Breezedeus](https://www.breezedeus.com).
+import string
 from typing import Sequence, List, Optional
 
 import numpy as np
 import cv2
 
 
 def clip(x, min_value, max_value):
@@ -173,14 +174,16 @@
         return outs
 
 
 def prepare_ocr_engine(languages: Sequence[str], ocr_engine_config):
     if len(set(languages).difference({'en', 'ch_sim'})) == 0:
         from cnocr import CnOcr
 
+        if 'ch_sim' not in languages and 'cand_alphabet' not in ocr_engine_config:  # only recognize english characters
+            ocr_engine_config['cand_alphabet'] = string.printable
         ocr_engine = CnOcr(**ocr_engine_config)
         engine_wrapper = CnOCREngine(languages, ocr_engine)
     else:
         try:
             from easyocr import Reader
         except:
             raise ImportError('Please install easyocr first: pip install easyocr')
```

### Comparing `pix2text-1.1.0.2/pix2text/page_elements.py` & `pix2text-1.1.0.3/pix2text/page_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,18 @@
         self.spellchecker = spellchecker
         self.config = config or {}
 
     def __repr__(self) -> str:
         return f"Page(id={self.id}, number={self.number}, elements={self.elements})"
 
     def to_markdown(
-        self, out_dir: Union[str, Path], root_url: Optional[str]=None, markdown_fn: Optional[str] = 'output.md'
+        self,
+        out_dir: Union[str, Path],
+        root_url: Optional[str] = None,
+        markdown_fn: Optional[str] = 'output.md',
     ) -> str:
         out_dir = Path(out_dir)
         out_dir.mkdir(exist_ok=True, parents=True)
         self.elements.sort()
         if not self.elements:
             return ''
         md_out = self._ele_to_markdown(self.elements[0], root_url, out_dir)
@@ -220,15 +223,17 @@
             rf'{line_sep}{{2,}}', f'{line_sep}{line_sep}', md_out
         )  # 把2个以上的连续 '\n' 替换为 '\n\n'
         if markdown_fn:
             with open(out_dir / markdown_fn, 'w', encoding='utf-8') as f:
                 f.write(md_out)
         return md_out
 
-    def _ele_to_markdown(self, element: Element, root_url: Optional[str], out_dir: Union[str, Path]):
+    def _ele_to_markdown(
+        self, element: Element, root_url: Optional[str], out_dir: Union[str, Path]
+    ):
         type = element.type
         text = element.text
         if type in (ElementType.TEXT, ElementType.TABLE):
             if type == ElementType.TABLE:
                 visualize_cells(
                     element.total_img.crop(element.box),
                     element.meta['cells'][0],
@@ -279,25 +284,28 @@
         self.spellchecker = spellchecker
         self.config = config or {}
 
     def __repr__(self) -> str:
         return f"Document(id={self.id}, number={self.number}, pages={self.pages})"
 
     def to_markdown(
-        self, out_dir: Union[str, Path], markdown_fn: Optional[str] = 'output.md'
+        self,
+        out_dir: Union[str, Path],
+        root_url: Optional[str] = None,
+        markdown_fn: Optional[str] = 'output.md',
     ) -> str:
         out_dir = Path(out_dir)
         out_dir.mkdir(exist_ok=True, parents=True)
         self.pages.sort(key=lambda page: page.number)
         if not self.pages:
             return ''
-        md_out = self.pages[0].to_markdown(out_dir, markdown_fn=None)
+        md_out = self.pages[0].to_markdown(out_dir, root_url=root_url, markdown_fn=None)
         for idx, page in enumerate(self.pages[1:]):
             prev_page = self.pages[idx]
-            cur_txt = page.to_markdown(out_dir, markdown_fn=None)
+            cur_txt = page.to_markdown(out_dir, mroot_url=root_url, arkdown_fn=None)
             if (
                 md_out
                 and prev_page.elements
                 and prev_page.elements[-1].type in (ElementType.TEXT, ElementType.TITLE)
                 and page.elements
                 and page.elements[0].type in (ElementType.TEXT, ElementType.TITLE)
                 and md_out[-1] != '\n'
```

### Comparing `pix2text-1.1.0.2/pix2text/pix_to_text.py` & `pix2text-1.1.0.3/pix2text/pix_to_text.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/render.py` & `pix2text-1.1.0.3/pix2text/render.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/screenshot_daemon_with_server2.py` & `pix2text-1.1.0.3/pix2text/screenshot_daemon_with_server2.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/serve.py` & `pix2text-1.1.0.3/pix2text/serve.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/table_inference.py` & `pix2text-1.1.0.3/pix2text/table_inference.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/table_ocr.py` & `pix2text-1.1.0.3/pix2text/table_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/table_postprocess.py` & `pix2text-1.1.0.3/pix2text/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/text_formula_ocr.py` & `pix2text-1.1.0.3/pix2text/text_formula_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text/utils.py` & `pix2text-1.1.0.3/pix2text/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/pix2text.egg-info/PKG-INFO` & `pix2text-1.1.0.3/pix2text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 1.1.0.2
+Version: 1.1.0.3
 Summary: An Open-Source Python3 tool for recognizing layouts, tables, math formulas, and text in images, converting them into Markdown format. A free alternative to Mathpix, empowering seamless conversion of visual content into text-based representations.
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
@@ -86,14 +86,18 @@
 - **Table Recognition Model**: [breezedeus/pix2text-table-rec](https://huggingface.co/breezedeus/pix2text-table-rec) ([Mirror](https://hf-mirror.com/breezedeus/pix2text-table-rec)).
 - **Text Recognition Engine**: Supports **80+ languages** such as **English, Simplified Chinese, Traditional Chinese, Vietnamese**, etc. For English and Simplified Chinese recognition, it uses the open-source OCR tool [CnOCR](https://github.com/breezedeus/cnocr), while for other languages, it uses the open-source OCR tool [EasyOCR](https://github.com/JaidedAI/EasyOCR).
 - **Mathematical Formula Detection Model (MFD)**: Mathematical formula detection model (MFD) from [CnSTD](https://github.com/breezedeus/cnstd).
 - **Mathematical Formula Recognition Model (MFR)**: [breezedeus/pix2text-mfr](https://huggingface.co/breezedeus/pix2text-mfr) ([Mirror](https://hf-mirror.com/breezedeus/pix2text-mfr)).
 
 Several models are contributed by other open-source authors, and their contributions are highly appreciated.
 
+<div align="center">
+  <img src="docs/figs/arch-flow.jpg" alt="Pix2Text Arch Flow"/>
+</div>
+
 For detailed explanations, please refer to the [Pix2Text Online Documentation/Models](https://pix2text.readthedocs.io/zh/latest/models/).
 
 <br/>
 
 As a Python3 toolkit, P2T may not be very user-friendly for those who are not familiar with Python. Therefore, we also provide a **[free-to-use P2T Online Web](https://p2t.breezedeus.com)**, where you can directly upload images and get P2T parsing results. The web version uses the latest models, resulting in better performance compared to the open-source models.
 
 If you're interested, feel free to add the assistant as a friend by scanning the QR code and mentioning `p2t`. The assistant will regularly invite everyone to join the group where the latest developments related to P2T tools will be announced:
```

### Comparing `pix2text-1.1.0.2/pix2text.egg-info/SOURCES.txt` & `pix2text-1.1.0.3/pix2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/convert_label_studio_to_yolov7.py` & `pix2text-1.1.0.3/scripts/convert_label_studio_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/extract_p2t_results.py` & `pix2text-1.1.0.3/scripts/extract_p2t_results.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/gen_label_studio_json.py` & `pix2text-1.1.0.3/scripts/gen_label_studio_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/gen_pure_formula_to_yolov7.py` & `pix2text-1.1.0.3/scripts/gen_pure_formula_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/merge_label_studio_anno_pred_json.py` & `pix2text-1.1.0.3/scripts/merge_label_studio_anno_pred_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/object_detection3.py` & `pix2text-1.1.0.3/scripts/object_detection3.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/screenshot_daemon.py` & `pix2text-1.1.0.3/scripts/screenshot_daemon.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/try_latex_correction.py` & `pix2text-1.1.0.3/scripts/try_latex_correction.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/try_layout.py` & `pix2text-1.1.0.3/scripts/try_layout.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/try_pix2text_mfr.py` & `pix2text-1.1.0.3/scripts/try_pix2text_mfr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/try_service.py` & `pix2text-1.1.0.3/scripts/try_service.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/scripts/try_texify.py` & `pix2text-1.1.0.3/scripts/try_texify.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/setup.py` & `pix2text-1.1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/tests/test_pix2text.py` & `pix2text-1.1.0.3/tests/test_pix2text.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.2/tests/test_sort_boxes.py` & `pix2text-1.1.0.3/tests/test_sort_boxes.py`

 * *Files identical despite different names*

