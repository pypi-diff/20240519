# Comparing `tmp/libresvip-1.1.2.tar.gz` & `tmp/libresvip-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libresvip-1.1.2.tar", last modified: Mon May  6 14:07:16 2024, max compression
+gzip compressed data, was "libresvip-1.1.3.tar", last modified: Sun May 19 13:03:35 2024, max compression
```

## Comparing `libresvip-1.1.2.tar` & `libresvip-1.1.3.tar`

### file list

```diff
@@ -1,403 +1,403 @@
--rw-r--r--   0        0        0     1093 2024-02-22 15:40:21.193635 libresvip-1.1.2/LICENSE
--rw-r--r--   0        0        0     2562 2024-02-22 15:40:21.193635 libresvip-1.1.2/README.md
--rw-r--r--   0        0        0       87 2024-05-06 13:05:54.799731 libresvip-1.1.2/libresvip/__init__.py
--rw-r--r--   0        0        0      295 2024-04-04 15:32:50.232340 libresvip-1.1.2/libresvip/cli/__init__.py
--rw-r--r--   0        0        0       76 2024-02-22 15:40:21.198477 libresvip-1.1.2/libresvip/cli/__main__.py
--rw-r--r--   0        0        0      213 2024-02-22 15:40:21.198477 libresvip-1.1.2/libresvip/cli/app.py
--rw-r--r--   0        0        0      180 2024-02-22 15:40:21.198477 libresvip-1.1.2/libresvip/cli/commands/__init__.py
--rw-r--r--   0        0        0      862 2024-03-04 16:48:04.970405 libresvip-1.1.2/libresvip/cli/commands/conf.py
--rw-r--r--   0        0        0     6395 2024-03-09 15:39:33.257482 libresvip-1.1.2/libresvip/cli/commands/plugin.py
--rw-r--r--   0        0        0     9237 2024-04-04 15:32:50.233347 libresvip-1.1.2/libresvip/cli/commands/proj.py
--rw-r--r--   0        0        0     3231 2024-04-19 22:32:21.141370 libresvip-1.1.2/libresvip/cli/prompt.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.199452 libresvip-1.1.2/libresvip/core/__init__.py
--rw-r--r--   0        0        0      647 2024-03-10 04:18:39.143052 libresvip-1.1.2/libresvip/core/compat.py
--rw-r--r--   0        0        0     5142 2024-04-26 03:48:21.746001 libresvip-1.1.2/libresvip/core/config.py
--rw-r--r--   0        0        0      635 2024-03-02 16:03:26.993803 libresvip-1.1.2/libresvip/core/constants.py
--rw-r--r--   0        0        0      270 2024-03-04 16:48:04.971414 libresvip-1.1.2/libresvip/core/exceptions.py
--rw-r--r--   0        0        0        2 2024-02-22 15:40:21.201450 libresvip-1.1.2/libresvip/core/lyric_phoneme/__init__.py
--rw-r--r--   0        0        0     2988 2024-03-04 16:48:04.972451 libresvip-1.1.2/libresvip/core/lyric_phoneme/chinese/__init__.py
--rw-r--r--   0        0        0     9449 2024-03-04 16:48:04.973454 libresvip-1.1.2/libresvip/core/lyric_phoneme/chinese/vocaloid_xsampa.py
--rw-r--r--   0        0        0      464 2024-03-12 17:52:45.770726 libresvip-1.1.2/libresvip/core/lyric_phoneme/japanese/__init__.py
--rw-r--r--   0        0        0     2789 2024-03-04 16:48:04.974452 libresvip-1.1.2/libresvip/core/lyric_phoneme/japanese/vocaloid_xsampa.py
--rw-r--r--   0        0        0     1646 2024-02-24 21:21:43.979932 libresvip-1.1.2/libresvip/core/tick_counter.py
--rw-r--r--   0        0        0     5850 2024-03-04 16:48:04.975456 libresvip-1.1.2/libresvip/core/time_interval.py
--rw-r--r--   0        0        0     4280 2024-02-24 21:21:43.979932 libresvip-1.1.2/libresvip/core/time_sync.py
--rw-r--r--   0        0        0     1551 2024-04-04 15:32:50.235346 libresvip-1.1.2/libresvip/core/warning_types.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.203986 libresvip-1.1.2/libresvip/extension/__init__.py
--rw-r--r--   0        0        0      986 2024-03-09 15:39:33.261482 libresvip-1.1.2/libresvip/extension/base.py
--rw-r--r--   0        0        0     7583 2024-03-09 15:39:33.262482 libresvip-1.1.2/libresvip/extension/manager.py
--rw-r--r--   0        0        0     3700 2024-03-09 15:39:33.263482 libresvip-1.1.2/libresvip/extension/meta_info.py
--rw-r--r--   0        0        0    93928 2024-04-27 16:08:27.372830 libresvip-1.1.2/libresvip/gui/__init__.py
--rw-r--r--   0        0        0     1135 2024-04-04 15:32:50.237346 libresvip-1.1.2/libresvip/gui/__main__.py
--rw-r--r--   0        0        0        0 2024-04-04 15:32:50.238347 libresvip-1.1.2/libresvip/gui/models/__init__.py
--rw-r--r--   0        0        0      499 2024-04-04 15:32:50.238347 libresvip-1.1.2/libresvip/gui/models/base_task.py
--rw-r--r--   0        0        0     8893 2024-04-26 15:58:39.835740 libresvip-1.1.2/libresvip/gui/models/list_models.py
--rw-r--r--   0        0        0     7284 2024-04-27 00:43:36.532622 libresvip-1.1.2/libresvip/gui/models/table_models.py
--rw-r--r--   0        0        0      846 2024-03-26 19:35:54.341234 libresvip-1.1.2/libresvip/gui/modules/__init__.py
--rw-r--r--   0        0        0      518 2024-03-26 19:35:54.342244 libresvip-1.1.2/libresvip/gui/modules/application.py
--rw-r--r--   0        0        0      865 2024-02-24 21:21:43.980924 libresvip-1.1.2/libresvip/gui/modules/clipboard.py
--rw-r--r--   0        0        0     5483 2024-04-25 23:57:25.750197 libresvip-1.1.2/libresvip/gui/modules/config_items.py
--rw-r--r--   0        0        0      810 2024-02-22 15:40:21.213022 libresvip-1.1.2/libresvip/gui/modules/font_loader.py
--rw-r--r--   0        0        0     2533 2024-03-04 16:48:04.979510 libresvip-1.1.2/libresvip/gui/modules/frameless_window.py
--rw-r--r--   0        0        0     8815 2024-03-04 16:48:04.980438 libresvip-1.1.2/libresvip/gui/modules/frameless_window_win32.py
--rw-r--r--   0        0        0     2218 2024-04-17 18:49:57.998947 libresvip-1.1.2/libresvip/gui/modules/locale_switcher.py
--rw-r--r--   0        0        0    10128 2024-04-28 13:23:02.012032 libresvip-1.1.2/libresvip/gui/modules/notifier.py
--rw-r--r--   0        0        0    39784 2024-04-27 01:43:02.793017 libresvip-1.1.2/libresvip/gui/modules/task_manager.py
--rw-r--r--   0        0        0      390 2024-02-22 15:40:21.215023 libresvip-1.1.2/libresvip/gui/modules/url_opener.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.215023 libresvip-1.1.2/libresvip/gui/modules/vendor/__init__.py
--rw-r--r--   0        0        0    25262 2024-03-24 06:00:55.521020 libresvip-1.1.2/libresvip/gui/modules/vendor/qasync/__init__.py
--rw-r--r--   0        0        0      497 2024-03-04 16:48:04.983407 libresvip-1.1.2/libresvip/gui/modules/vendor/qasync/_common.py
--rw-r--r--   0        0        0     7507 2024-03-04 16:48:04.984405 libresvip-1.1.2/libresvip/gui/modules/vendor/qasync/_unix.py
--rw-r--r--   0        0        0     9345 2024-03-04 16:48:04.985406 libresvip-1.1.2/libresvip/gui/modules/vendor/qasync/_windows.py
--rw-r--r--   0        0        0      981 2024-02-22 15:40:21.217025 libresvip-1.1.2/libresvip/gui/modules/win32_constants.py
--rw-r--r--   0        0        0        0 2024-03-09 15:39:33.266482 libresvip-1.1.2/libresvip/middlewares/pitch_shift/__init__.py
--rw-r--r--   0        0        0      219 2024-03-09 15:39:33.266482 libresvip-1.1.2/libresvip/middlewares/pitch_shift/options.py
--rw-r--r--   0        0        0     2136 2024-03-09 15:39:33.267482 libresvip-1.1.2/libresvip/middlewares/pitch_shift/pitch_shift.py
--rw-r--r--   0        0        0      181 2024-03-09 15:39:33.267482 libresvip-1.1.2/libresvip/middlewares/pitch_shift/pitch_shift.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-03-09 15:39:33.267482 libresvip-1.1.2/libresvip/middlewares/project_zoom/__init__.py
--rw-r--r--   0        0        0     1009 2024-03-09 15:39:33.267482 libresvip-1.1.2/libresvip/middlewares/project_zoom/options.py
--rw-r--r--   0        0        0      508 2024-03-09 15:39:33.267482 libresvip-1.1.2/libresvip/middlewares/project_zoom/project_zoom.py
--rw-r--r--   0        0        0      220 2024-03-09 15:39:33.269050 libresvip-1.1.2/libresvip/middlewares/project_zoom/project_zoom.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-03-09 15:39:33.269050 libresvip-1.1.2/libresvip/middlewares/pronounciation_conversion/__init__.py
--rw-r--r--   0        0        0      791 2024-03-09 15:39:33.269050 libresvip-1.1.2/libresvip/middlewares/pronounciation_conversion/options.py
--rw-r--r--   0        0        0     1510 2024-03-09 15:39:33.269050 libresvip-1.1.2/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.py
--rw-r--r--   0        0        0      270 2024-03-09 15:39:33.269989 libresvip-1.1.2/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-03-09 15:39:33.269989 libresvip-1.1.2/libresvip/middlewares/remove_short_silences/__init__.py
--rw-r--r--   0        0        0      882 2024-03-09 15:39:33.269989 libresvip-1.1.2/libresvip/middlewares/remove_short_silences/options.py
--rw-r--r--   0        0        0      953 2024-03-09 15:39:33.270989 libresvip-1.1.2/libresvip/middlewares/remove_short_silences/remove_short_silences.py
--rw-r--r--   0        0        0      243 2024-03-09 15:39:33.270989 libresvip-1.1.2/libresvip/middlewares/remove_short_silences/remove_short_silences.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-04-17 19:53:22.520237 libresvip-1.1.2/libresvip/middlewares/replace_lyric/__init__.py
--rw-r--r--   0        0        0      212 2024-04-19 05:00:08.861563 libresvip-1.1.2/libresvip/middlewares/replace_lyric/options.py
--rw-r--r--   0        0        0     1326 2024-04-27 16:08:27.375841 libresvip-1.1.2/libresvip/middlewares/replace_lyric/replace_lyric.py
--rw-r--r--   0        0        0      319 2024-04-19 21:12:02.082450 libresvip-1.1.2/libresvip/middlewares/replace_lyric/replace_lyric.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.217025 libresvip-1.1.2/libresvip/model/__init__.py
--rw-r--r--   0        0        0    10233 2024-04-22 20:47:04.172800 libresvip-1.1.2/libresvip/model/base.py
--rw-r--r--   0        0        0     1373 2024-03-23 15:29:05.921080 libresvip-1.1.2/libresvip/model/option_mixins.py
--rw-r--r--   0        0        0     3152 2024-02-24 21:21:43.981935 libresvip-1.1.2/libresvip/model/point.py
--rw-r--r--   0        0        0     7529 2024-05-03 03:31:10.216309 libresvip-1.1.2/libresvip/model/relative_pitch_curve.py
--rw-r--r--   0        0        0     7848 2024-03-18 14:03:10.224552 libresvip-1.1.2/libresvip/model/reset_time_axis.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.218004 libresvip-1.1.2/libresvip/plugins/acep/__init__.py
--rw-r--r--   0        0        0    54700 2024-02-22 15:40:21.219535 libresvip-1.1.2/libresvip/plugins/acep/ace-studio.yapsy-plugin
--rw-r--r--   0        0        0     1487 2024-02-22 15:40:21.219535 libresvip-1.1.2/libresvip/plugins/acep/ace_curve_utils.py
--rw-r--r--   0        0        0      949 2024-04-25 14:59:40.397933 libresvip-1.1.2/libresvip/plugins/acep/ace_studio_converter.py
--rw-r--r--   0        0        0    19572 2024-04-25 14:57:35.603703 libresvip-1.1.2/libresvip/plugins/acep/ace_studio_generator.py
--rw-r--r--   0        0        0    17695 2024-04-25 15:01:55.236085 libresvip-1.1.2/libresvip/plugins/acep/ace_studio_parser.py
--rw-r--r--   0        0        0     1620 2024-03-04 16:48:04.991428 libresvip-1.1.2/libresvip/plugins/acep/acep_io.py
--rw-r--r--   0        0        0     5339 2024-03-04 16:48:04.991428 libresvip-1.1.2/libresvip/plugins/acep/base_pitch_curve.py
--rw-r--r--   0        0        0      386 2024-02-22 15:40:21.221571 libresvip-1.1.2/libresvip/plugins/acep/color_pool.py
--rw-r--r--   0        0        0      565 2024-02-24 21:21:43.984931 libresvip-1.1.2/libresvip/plugins/acep/curve_segment_utils.py
--rw-r--r--   0        0        0    14273 2024-04-25 15:01:55.235088 libresvip-1.1.2/libresvip/plugins/acep/model.py
--rw-r--r--   0        0        0    11102 2024-04-04 15:32:50.247348 libresvip-1.1.2/libresvip/plugins/acep/options.py
--rw-r--r--   0        0        0     2518 2024-04-04 15:32:50.248346 libresvip-1.1.2/libresvip/plugins/acep/singers.py
--rw-r--r--   0        0        0     1215 2024-02-22 15:40:21.223573 libresvip-1.1.2/libresvip/plugins/acep/time_utils.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.223573 libresvip-1.1.2/libresvip/plugins/aisp/__init__.py
--rw-r--r--   0        0        0     1486 2024-02-22 15:40:21.223573 libresvip-1.1.2/libresvip/plugins/aisp/aisingers_converter.py
--rw-r--r--   0        0        0     9276 2024-03-04 16:48:04.992962 libresvip-1.1.2/libresvip/plugins/aisp/aisingers_generator.py
--rw-r--r--   0        0        0     4725 2024-03-23 15:29:05.925080 libresvip-1.1.2/libresvip/plugins/aisp/aisingers_parser.py
--rw-r--r--   0        0        0    23952 2024-02-22 15:40:21.224550 libresvip-1.1.2/libresvip/plugins/aisp/aisp.yapsy-plugin
--rw-r--r--   0        0        0     4713 2024-02-22 15:40:21.225582 libresvip-1.1.2/libresvip/plugins/aisp/model.py
--rw-r--r--   0        0        0      325 2024-04-22 06:45:10.507210 libresvip-1.1.2/libresvip/plugins/aisp/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.225582 libresvip-1.1.2/libresvip/plugins/ccs/__init__.py
--rw-r--r--   0        0        0    38382 2024-02-22 15:40:21.226575 libresvip-1.1.2/libresvip/plugins/ccs/ccs.yapsy-plugin
--rw-r--r--   0        0        0     1350 2024-02-22 15:40:21.227574 libresvip-1.1.2/libresvip/plugins/ccs/cevio_converter.py
--rw-r--r--   0        0        0     8349 2024-04-04 15:32:50.249954 libresvip-1.1.2/libresvip/plugins/ccs/cevio_generator.py
--rw-r--r--   0        0        0    10117 2024-04-30 12:50:10.287752 libresvip-1.1.2/libresvip/plugins/ccs/cevio_parser.py
--rw-r--r--   0        0        0    12923 2024-05-04 23:42:40.106850 libresvip-1.1.2/libresvip/plugins/ccs/cevio_pitch.py
--rw-r--r--   0        0        0      296 2024-02-22 15:40:21.228574 libresvip-1.1.2/libresvip/plugins/ccs/constants.py
--rw-r--r--   0        0        0    31399 2024-02-22 15:40:21.228574 libresvip-1.1.2/libresvip/plugins/ccs/model.py
--rw-r--r--   0        0        0      567 2024-03-23 15:29:05.927080 libresvip-1.1.2/libresvip/plugins/ccs/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.229551 libresvip-1.1.2/libresvip/plugins/ds/__init__.py
--rw-r--r--   0        0        0     6352 2024-02-22 15:40:21.230060 libresvip-1.1.2/libresvip/plugins/ds/dicts/opencpop-extension.txt
--rw-r--r--   0        0        0     4475 2024-02-22 15:40:21.230241 libresvip-1.1.2/libresvip/plugins/ds/dicts/opencpop-strict.txt
--rw-r--r--   0        0        0     4468 2024-02-22 15:40:21.230241 libresvip-1.1.2/libresvip/plugins/ds/dicts/opencpop.txt
--rw-r--r--   0        0        0     2051 2024-02-22 15:40:21.230241 libresvip-1.1.2/libresvip/plugins/ds/diffsinger_converter.py
--rw-r--r--   0        0        0     1846 2024-02-22 15:40:21.231089 libresvip-1.1.2/libresvip/plugins/ds/diffsinger_generator.py
--rw-r--r--   0        0        0     5222 2024-03-23 15:29:05.928079 libresvip-1.1.2/libresvip/plugins/ds/diffsinger_parser.py
--rw-r--r--   0        0        0    31348 2024-02-22 15:40:21.232090 libresvip-1.1.2/libresvip/plugins/ds/ds.yapsy-plugin
--rw-r--r--   0        0        0     3192 2024-02-22 15:40:21.232090 libresvip-1.1.2/libresvip/plugins/ds/model.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.232090 libresvip-1.1.2/libresvip/plugins/ds/models/__init__.py
--rw-r--r--   0        0        0     1292 2024-02-22 15:40:21.233090 libresvip-1.1.2/libresvip/plugins/ds/models/ds_note.py
--rw-r--r--   0        0        0      225 2024-02-22 15:40:21.233090 libresvip-1.1.2/libresvip/plugins/ds/models/ds_param_curve.py
--rw-r--r--   0        0        0      118 2024-02-22 15:40:21.233090 libresvip-1.1.2/libresvip/plugins/ds/models/ds_param_node.py
--rw-r--r--   0        0        0     3205 2024-02-22 15:40:21.233090 libresvip-1.1.2/libresvip/plugins/ds/models/ds_project.py
--rw-r--r--   0        0        0     1984 2024-03-23 15:29:05.929080 libresvip-1.1.2/libresvip/plugins/ds/options.py
--rw-r--r--   0        0        0      786 2024-02-24 21:21:43.986928 libresvip-1.1.2/libresvip/plugins/ds/phoneme_dict.py
--rw-r--r--   0        0        0        2 2024-02-22 15:40:21.234069 libresvip-1.1.2/libresvip/plugins/ds/utils/__init__.py
--rw-r--r--   0        0        0     1452 2024-03-04 16:48:04.996982 libresvip-1.1.2/libresvip/plugins/ds/utils/gender_param_utils.py
--rw-r--r--   0        0        0      294 2024-04-04 23:42:44.572812 libresvip-1.1.2/libresvip/plugins/ds/utils/lyric_util.py
--rw-r--r--   0        0        0     6771 2024-04-04 23:06:53.822302 libresvip-1.1.2/libresvip/plugins/ds/utils/note_list_util.py
--rw-r--r--   0        0        0     1380 2024-02-24 21:21:43.988828 libresvip-1.1.2/libresvip/plugins/ds/utils/pinyin_util.py
--rw-r--r--   0        0        0     1613 2024-02-24 21:21:43.988828 libresvip-1.1.2/libresvip/plugins/ds/utils/pitch_param_utils.py
--rw-r--r--   0        0        0     3990 2024-02-22 15:40:21.236071 libresvip-1.1.2/libresvip/plugins/ds/utils/project_util.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.236071 libresvip-1.1.2/libresvip/plugins/dv/__init__.py
--rw-r--r--   0        0        0    11432 2024-03-04 16:48:04.999015 libresvip-1.1.2/libresvip/plugins/dv/constants.py
--rw-r--r--   0        0        0      847 2024-02-22 15:40:21.237092 libresvip-1.1.2/libresvip/plugins/dv/deepvocal_converter.py
--rw-r--r--   0        0        0    10745 2024-02-22 23:04:58.757287 libresvip-1.1.2/libresvip/plugins/dv/deepvocal_pitch.py
--rw-r--r--   0        0        0     6453 2024-02-22 15:40:21.238069 libresvip-1.1.2/libresvip/plugins/dv/dv.yapsy-plugin
--rw-r--r--   0        0        0     8519 2024-02-24 21:21:43.989880 libresvip-1.1.2/libresvip/plugins/dv/dv_generator.py
--rw-r--r--   0        0        0     6800 2024-03-23 15:29:05.930098 libresvip-1.1.2/libresvip/plugins/dv/dv_parser.py
--rw-r--r--   0        0        0     4927 2024-02-22 15:40:21.239070 libresvip-1.1.2/libresvip/plugins/dv/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.931081 libresvip-1.1.2/libresvip/plugins/dv/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.239070 libresvip-1.1.2/libresvip/plugins/gj/__init__.py
--rw-r--r--   0        0        0     5113 2024-02-22 15:40:21.239070 libresvip-1.1.2/libresvip/plugins/gj/constants.py
--rw-r--r--   0        0        0    72345 2024-02-22 15:40:21.240660 libresvip-1.1.2/libresvip/plugins/gj/gjgj.yapsy-plugin
--rw-r--r--   0        0        0     1120 2024-02-22 15:40:21.240660 libresvip-1.1.2/libresvip/plugins/gj/gjgj_converter.py
--rw-r--r--   0        0        0    10541 2024-04-04 15:32:50.250856 libresvip-1.1.2/libresvip/plugins/gj/gjgj_generator.py
--rw-r--r--   0        0        0     8051 2024-03-23 15:29:05.933100 libresvip-1.1.2/libresvip/plugins/gj/gjgj_parser.py
--rw-r--r--   0        0        0     6172 2024-02-22 15:40:21.241591 libresvip-1.1.2/libresvip/plugins/gj/model.py
--rw-r--r--   0        0        0      784 2024-03-23 15:29:05.933100 libresvip-1.1.2/libresvip/plugins/gj/options.py
--rw-r--r--   0        0        0      303 2024-02-22 15:40:21.241591 libresvip-1.1.2/libresvip/plugins/gj/singers.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.241591 libresvip-1.1.2/libresvip/plugins/json/__init__.py
--rw-r--r--   0        0        0     1225 2024-02-22 15:40:21.242586 libresvip-1.1.2/libresvip/plugins/json/jsonsvip.yapsy-plugin
--rw-r--r--   0        0        0      965 2024-04-25 14:59:49.047701 libresvip-1.1.2/libresvip/plugins/json/jsonsvip_converter.py
--rw-r--r--   0        0        0      350 2024-02-22 15:40:21.243587 libresvip-1.1.2/libresvip/plugins/json/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.243587 libresvip-1.1.2/libresvip/plugins/lrc/__init__.py
--rw-r--r--   0        0        0     1400 2024-02-22 15:40:21.243587 libresvip-1.1.2/libresvip/plugins/lrc/lrc.yapsy-plugin
--rw-r--r--   0        0        0      484 2024-02-22 15:40:21.244588 libresvip-1.1.2/libresvip/plugins/lrc/lrc_converter.py
--rw-r--r--   0        0        0     4320 2024-02-24 21:21:43.990884 libresvip-1.1.2/libresvip/plugins/lrc/lrc_generator.py
--rw-r--r--   0        0        0      670 2024-02-22 15:40:21.244588 libresvip-1.1.2/libresvip/plugins/lrc/model.py
--rw-r--r--   0        0        0     2391 2024-02-22 15:40:21.244588 libresvip-1.1.2/libresvip/plugins/lrc/options.py
--rw-r--r--   0        0        0      692 2024-02-22 15:40:21.245587 libresvip-1.1.2/libresvip/plugins/lrc/template.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.245587 libresvip-1.1.2/libresvip/plugins/mid/__init__.py
--rw-r--r--   0        0        0     1990 2024-02-22 15:40:21.245587 libresvip-1.1.2/libresvip/plugins/mid/constants.py
--rw-r--r--   0        0        0     5992 2024-02-22 15:40:21.246587 libresvip-1.1.2/libresvip/plugins/mid/mid.yapsy-plugin
--rw-r--r--   0        0        0      982 2024-02-24 00:53:21.067110 libresvip-1.1.2/libresvip/plugins/mid/midi_converter.py
--rw-r--r--   0        0        0     6509 2024-03-04 16:48:04.999015 libresvip-1.1.2/libresvip/plugins/mid/midi_generator.py
--rw-r--r--   0        0        0    12410 2024-04-04 15:32:50.251856 libresvip-1.1.2/libresvip/plugins/mid/midi_parser.py
--rw-r--r--   0        0        0     2784 2024-03-04 16:48:05.001983 libresvip-1.1.2/libresvip/plugins/mid/midi_pitch.py
--rw-r--r--   0        0        0      485 2024-02-22 15:40:21.247587 libresvip-1.1.2/libresvip/plugins/mid/note_overlap.py
--rw-r--r--   0        0        0     3008 2024-03-23 15:29:05.936080 libresvip-1.1.2/libresvip/plugins/mid/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.247587 libresvip-1.1.2/libresvip/plugins/mtp/__init__.py
--rw-r--r--   0        0        0     5764 2024-02-22 15:40:21.247587 libresvip-1.1.2/libresvip/plugins/mtp/model.py
--rw-r--r--   0        0        0    63944 2024-02-22 15:40:21.248586 libresvip-1.1.2/libresvip/plugins/mtp/mtp.yapsy-plugin
--rw-r--r--   0        0        0      782 2024-02-22 15:40:21.249586 libresvip-1.1.2/libresvip/plugins/mtp/muta_converter.py
--rw-r--r--   0        0        0     7329 2024-05-01 15:16:27.115338 libresvip-1.1.2/libresvip/plugins/mtp/muta_generator.py
--rw-r--r--   0        0        0     5159 2024-05-01 15:02:14.057268 libresvip-1.1.2/libresvip/plugins/mtp/muta_parser.py
--rw-r--r--   0        0        0      495 2024-03-23 15:29:05.938080 libresvip-1.1.2/libresvip/plugins/mtp/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.249586 libresvip-1.1.2/libresvip/plugins/musicxml/__init__.py
--rw-r--r--   0        0        0     1375 2024-02-22 15:40:21.249586 libresvip-1.1.2/libresvip/plugins/musicxml/model.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.251137 libresvip-1.1.2/libresvip/plugins/musicxml/models/__init__.py
--rw-r--r--   0        0        0   375472 2024-02-22 15:40:21.252183 libresvip-1.1.2/libresvip/plugins/musicxml/models/mxml2.py
--rw-r--r--   0        0        0     1577 2024-02-22 15:40:21.253184 libresvip-1.1.2/libresvip/plugins/musicxml/models/xlink.py
--rw-r--r--   0        0        0      118 2024-02-22 15:40:21.253184 libresvip-1.1.2/libresvip/plugins/musicxml/models/xml.py
--rw-r--r--   0        0        0    17317 2024-02-22 15:40:21.253184 libresvip-1.1.2/libresvip/plugins/musicxml/musicxml.yapsy-plugin
--rw-r--r--   0        0        0     1699 2024-04-03 23:14:53.053648 libresvip-1.1.2/libresvip/plugins/musicxml/musicxml_converter.py
--rw-r--r--   0        0        0    14877 2024-02-24 21:21:43.993929 libresvip-1.1.2/libresvip/plugins/musicxml/musicxml_generator.py
--rw-r--r--   0        0        0     6295 2024-02-24 21:21:43.993929 libresvip-1.1.2/libresvip/plugins/musicxml/musicxml_parser.py
--rw-r--r--   0        0        0      125 2024-02-22 15:40:21.255194 libresvip-1.1.2/libresvip/plugins/musicxml/options.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.255194 libresvip-1.1.2/libresvip/plugins/nn/__init__.py
--rw-r--r--   0        0        0     4875 2024-02-22 15:40:21.255194 libresvip-1.1.2/libresvip/plugins/nn/model.py
--rw-r--r--   0        0        0     1068 2024-03-23 15:29:05.939080 libresvip-1.1.2/libresvip/plugins/nn/niaoniao_converter.py
--rw-r--r--   0        0        0     5374 2024-03-23 15:29:05.940080 libresvip-1.1.2/libresvip/plugins/nn/niaoniao_generator.py
--rw-r--r--   0        0        0     3564 2024-03-23 15:29:05.940080 libresvip-1.1.2/libresvip/plugins/nn/niaoniao_parser.py
--rw-r--r--   0        0        0    21285 2024-02-22 15:40:21.256182 libresvip-1.1.2/libresvip/plugins/nn/nn.yapsy-plugin
--rw-r--r--   0        0        0      467 2024-03-23 15:29:05.941583 libresvip-1.1.2/libresvip/plugins/nn/options.py
--rw-r--r--   0        0        0     1008 2024-02-22 15:40:21.257195 libresvip-1.1.2/libresvip/plugins/nn/template.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.257195 libresvip-1.1.2/libresvip/plugins/ppsf/__init__.py
--rw-r--r--   0        0        0     7813 2024-02-22 15:40:21.257195 libresvip-1.1.2/libresvip/plugins/ppsf/legacy_model.py
--rw-r--r--   0        0        0    12763 2024-02-22 15:40:21.258193 libresvip-1.1.2/libresvip/plugins/ppsf/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.942587 libresvip-1.1.2/libresvip/plugins/ppsf/options.py
--rw-r--r--   0        0        0     1931 2024-04-04 15:32:50.252857 libresvip-1.1.2/libresvip/plugins/ppsf/piapro_studio_converter.py
--rw-r--r--   0        0        0     8331 2024-03-09 15:39:33.271989 libresvip-1.1.2/libresvip/plugins/ppsf/piapro_studio_generator.py
--rw-r--r--   0        0        0     6809 2024-02-22 15:40:21.259204 libresvip-1.1.2/libresvip/plugins/ppsf/piapro_studio_legacy_parser.py
--rw-r--r--   0        0        0     5897 2024-03-23 15:29:05.943588 libresvip-1.1.2/libresvip/plugins/ppsf/piapro_studio_nt_parser.py
--rw-r--r--   0        0        0    19426 2024-02-22 15:40:21.260207 libresvip-1.1.2/libresvip/plugins/ppsf/ppsf.yapsy-plugin
--rw-r--r--   0        0        0     3256 2024-02-24 21:21:43.995835 libresvip-1.1.2/libresvip/plugins/ppsf/ppsf_interval_dict.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.260207 libresvip-1.1.2/libresvip/plugins/s5p/__init__.py
--rw-r--r--   0        0        0     6029 2024-04-04 15:32:50.253857 libresvip-1.1.2/libresvip/plugins/s5p/model.py
--rw-r--r--   0        0        0      344 2024-03-23 15:29:09.443412 libresvip-1.1.2/libresvip/plugins/s5p/options.py
--rw-r--r--   0        0        0    52233 2024-02-22 15:40:21.261194 libresvip-1.1.2/libresvip/plugins/s5p/s5p.yapsy-plugin
--rw-r--r--   0        0        0     1045 2024-02-22 15:40:21.261194 libresvip-1.1.2/libresvip/plugins/s5p/synthv_editor_converter.py
--rw-r--r--   0        0        0     5418 2024-04-30 05:04:12.424188 libresvip-1.1.2/libresvip/plugins/s5p/synthv_editor_generator.py
--rw-r--r--   0        0        0    11521 2024-03-23 15:29:09.444396 libresvip-1.1.2/libresvip/plugins/s5p/synthv_editor_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.262203 libresvip-1.1.2/libresvip/plugins/srt/__init__.py
--rw-r--r--   0        0        0     1394 2024-02-22 15:40:21.262203 libresvip-1.1.2/libresvip/plugins/srt/options.py
--rw-r--r--   0        0        0     1285 2024-02-22 15:40:21.263187 libresvip-1.1.2/libresvip/plugins/srt/srt.yapsy-plugin
--rw-r--r--   0        0        0      503 2024-02-22 15:40:21.263187 libresvip-1.1.2/libresvip/plugins/srt/srt_converter.py
--rw-r--r--   0        0        0     2696 2024-02-24 21:21:43.996926 libresvip-1.1.2/libresvip/plugins/srt/srt_generator.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.263187 libresvip-1.1.2/libresvip/plugins/svg/__init__.py
--rw-r--r--   0        0        0     4552 2024-02-22 15:40:21.264194 libresvip-1.1.2/libresvip/plugins/svg/coordinate_helper.py
--rw-r--r--   0        0        0      279 2024-02-22 15:40:21.264194 libresvip-1.1.2/libresvip/plugins/svg/model.py
--rw-r--r--   0        0        0     3009 2024-02-22 15:40:21.264194 libresvip-1.1.2/libresvip/plugins/svg/options.py
--rw-r--r--   0        0        0    15147 2024-02-22 15:40:21.265188 libresvip-1.1.2/libresvip/plugins/svg/svg.yapsy-plugin
--rw-r--r--   0        0        0      568 2024-02-22 15:40:21.265188 libresvip-1.1.2/libresvip/plugins/svg/svg_converter.py
--rw-r--r--   0        0        0     6739 2024-02-22 15:40:21.265188 libresvip-1.1.2/libresvip/plugins/svg/svg_factory.py
--rw-r--r--   0        0        0     2422 2024-02-22 15:40:21.266243 libresvip-1.1.2/libresvip/plugins/svg/svg_generator.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.266243 libresvip-1.1.2/libresvip/plugins/svip/__init__.py
--rw-r--r--   0        0        0    15042 2024-02-22 15:40:21.266243 libresvip-1.1.2/libresvip/plugins/svip/binsvip.yapsy-plugin
--rw-r--r--   0        0        0     1561 2024-04-25 14:59:53.848685 libresvip-1.1.2/libresvip/plugins/svip/binsvip_converter.py
--rw-r--r--   0        0        0    11038 2024-04-04 23:08:50.052929 libresvip-1.1.2/libresvip/plugins/svip/binsvip_generator.py
--rw-r--r--   0        0        0     5944 2024-03-23 15:29:05.947587 libresvip-1.1.2/libresvip/plugins/svip/binsvip_parser.py
--rw-r--r--   0        0        0     1602 2024-04-22 23:56:13.988906 libresvip-1.1.2/libresvip/plugins/svip/models.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.267240 libresvip-1.1.2/libresvip/plugins/svip/msnrbf/__init__.py
--rw-r--r--   0        0        0    19970 2024-02-24 13:23:26.660918 libresvip-1.1.2/libresvip/plugins/svip/msnrbf/binary_models.py
--rw-r--r--   0        0        0      498 2024-03-04 16:48:05.006115 libresvip-1.1.2/libresvip/plugins/svip/msnrbf/constants.py
--rw-r--r--   0        0        0     1341 2024-03-04 16:48:05.007021 libresvip-1.1.2/libresvip/plugins/svip/msnrbf/nrbf_iobase.py
--rw-r--r--   0        0        0     4956 2024-03-04 16:48:05.007021 libresvip-1.1.2/libresvip/plugins/svip/msnrbf/svip_reader.py
--rw-r--r--   0        0        0    23277 2024-02-22 15:40:21.269238 libresvip-1.1.2/libresvip/plugins/svip/msnrbf/svip_writer.py
--rw-r--r--   0        0        0    15021 2024-04-04 15:32:50.256857 libresvip-1.1.2/libresvip/plugins/svip/msnrbf/xstudio_models.py
--rw-r--r--   0        0        0     3393 2024-03-23 15:29:05.948587 libresvip-1.1.2/libresvip/plugins/svip/options.py
--rw-r--r--   0        0        0     1857 2024-02-22 15:40:21.270241 libresvip-1.1.2/libresvip/plugins/svip/singers.json
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.270241 libresvip-1.1.2/libresvip/plugins/svip3/__init__.py
--rw-r--r--   0        0        0      397 2024-02-22 15:40:21.270241 libresvip-1.1.2/libresvip/plugins/svip3/color_pool.py
--rw-r--r--   0        0        0      396 2024-03-04 16:48:05.009732 libresvip-1.1.2/libresvip/plugins/svip3/constants.py
--rw-r--r--   0        0        0    12712 2024-04-26 16:10:27.006657 libresvip-1.1.2/libresvip/plugins/svip3/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.949587 libresvip-1.1.2/libresvip/plugins/svip3/options.py
--rw-r--r--   0        0        0     1588 2024-04-26 15:56:42.775172 libresvip-1.1.2/libresvip/plugins/svip3/singers.json
--rw-r--r--   0        0        0      243 2024-02-22 15:40:21.271242 libresvip-1.1.2/libresvip/plugins/svip3/singers.py
--rw-r--r--   0        0        0    13560 2024-02-22 15:40:21.272276 libresvip-1.1.2/libresvip/plugins/svip3/svip3.yapsy-plugin
--rw-r--r--   0        0        0      782 2024-03-23 15:29:05.950587 libresvip-1.1.2/libresvip/plugins/svip3/svip3_converter.py
--rw-r--r--   0        0        0    11203 2024-04-04 15:32:50.257857 libresvip-1.1.2/libresvip/plugins/svip3/svip3_generator.py
--rw-r--r--   0        0        0     8397 2024-03-23 15:29:05.951587 libresvip-1.1.2/libresvip/plugins/svip3/svip3_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.273244 libresvip-1.1.2/libresvip/plugins/svp/__init__.py
--rw-r--r--   0        0        0      859 2024-02-22 15:40:21.273244 libresvip-1.1.2/libresvip/plugins/svp/constants.py
--rw-r--r--   0        0        0      361 2024-02-22 15:40:21.275243 libresvip-1.1.2/libresvip/plugins/svp/interpolation.py
--rw-r--r--   0        0        0      201 2024-03-14 11:33:30.285334 libresvip-1.1.2/libresvip/plugins/svp/interval_utils.py
--rw-r--r--   0        0        0     1457 2024-02-22 15:40:21.275243 libresvip-1.1.2/libresvip/plugins/svp/lambert_w.py
--rw-r--r--   0        0        0    18008 2024-03-14 13:43:05.687807 libresvip-1.1.2/libresvip/plugins/svp/layer_generator.py
--rw-r--r--   0        0        0    22743 2024-04-04 23:42:44.572812 libresvip-1.1.2/libresvip/plugins/svp/model.py
--rw-r--r--   0        0        0     5769 2024-03-23 15:29:05.952587 libresvip-1.1.2/libresvip/plugins/svp/options.py
--rw-r--r--   0        0        0     9582 2024-03-04 16:48:05.013673 libresvip-1.1.2/libresvip/plugins/svp/param_expression.py
--rw-r--r--   0        0        0     2901 2024-02-22 15:40:21.277240 libresvip-1.1.2/libresvip/plugins/svp/phoneme_categories.json
--rw-r--r--   0        0        0    57860 2024-02-22 15:40:21.278256 libresvip-1.1.2/libresvip/plugins/svp/phoneme_dictionary.json
--rw-r--r--   0        0        0     3281 2024-02-24 21:21:43.999921 libresvip-1.1.2/libresvip/plugins/svp/phoneme_utils.py
--rw-r--r--   0        0        0     3651 2024-02-24 21:21:44.000940 libresvip-1.1.2/libresvip/plugins/svp/pitch_simulator.py
--rw-r--r--   0        0        0      870 2024-02-22 15:40:21.279241 libresvip-1.1.2/libresvip/plugins/svp/pitch_slide.py
--rw-r--r--   0        0        0    41585 2024-02-22 15:40:21.279241 libresvip-1.1.2/libresvip/plugins/svp/svp.yapsy-plugin
--rw-r--r--   0        0        0    21945 2024-03-09 15:39:33.275988 libresvip-1.1.2/libresvip/plugins/svp/synthv_generator.py
--rw-r--r--   0        0        0    29624 2024-03-23 15:29:05.953587 libresvip-1.1.2/libresvip/plugins/svp/synthv_parser.py
--rw-r--r--   0        0        0     1182 2024-04-25 15:00:01.642567 libresvip-1.1.2/libresvip/plugins/svp/synthv_studio_converter.py
--rw-r--r--   0        0        0     7049 2024-03-04 16:48:05.016732 libresvip-1.1.2/libresvip/plugins/svp/track_merge_utils.py
--rw-r--r--   0        0        0        0 2024-04-20 08:41:44.970999 libresvip-1.1.2/libresvip/plugins/tlp/__init__.py
--rw-r--r--   0        0        0     5323 2024-04-30 20:14:39.055539 libresvip-1.1.2/libresvip/plugins/tlp/model.py
--rw-r--r--   0        0        0      325 2024-04-29 22:55:41.750988 libresvip-1.1.2/libresvip/plugins/tlp/options.py
--rw-r--r--   0        0        0      253 2024-04-30 20:13:41.439220 libresvip-1.1.2/libresvip/plugins/tlp/tlp.yapsy-plugin
--rw-r--r--   0        0        0     1016 2024-04-30 20:09:17.799740 libresvip-1.1.2/libresvip/plugins/tlp/tunelab_converter.py
--rw-r--r--   0        0        0     5180 2024-05-05 04:13:14.653996 libresvip-1.1.2/libresvip/plugins/tlp/tunelab_generator.py
--rw-r--r--   0        0        0     5346 2024-05-05 04:32:27.959149 libresvip-1.1.2/libresvip/plugins/tlp/tunelab_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.281548 libresvip-1.1.2/libresvip/plugins/tssln/__init__.py
--rw-r--r--   0        0        0      258 2024-02-22 15:40:21.281548 libresvip-1.1.2/libresvip/plugins/tssln/constants.py
--rw-r--r--   0        0        0    14287 2024-03-04 16:48:05.018348 libresvip-1.1.2/libresvip/plugins/tssln/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.954587 libresvip-1.1.2/libresvip/plugins/tssln/options.py
--rw-r--r--   0        0        0    20418 2024-02-22 15:40:21.283497 libresvip-1.1.2/libresvip/plugins/tssln/tssln.yapsy-plugin
--rw-r--r--   0        0        0     3829 2024-02-24 13:21:27.902046 libresvip-1.1.2/libresvip/plugins/tssln/value_tree.py
--rw-r--r--   0        0        0     1032 2024-02-22 15:40:21.283497 libresvip-1.1.2/libresvip/plugins/tssln/voisona_converter.py
--rw-r--r--   0        0        0     6553 2024-04-04 15:32:50.258857 libresvip-1.1.2/libresvip/plugins/tssln/voisona_generator.py
--rw-r--r--   0        0        0     7550 2024-03-23 15:29:05.955587 libresvip-1.1.2/libresvip/plugins/tssln/voisona_parser.py
--rw-r--r--   0        0        0    12822 2024-05-03 03:24:54.410087 libresvip-1.1.2/libresvip/plugins/tssln/voisona_pitch.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.284496 libresvip-1.1.2/libresvip/plugins/ufdata/__init__.py
--rw-r--r--   0        0        0     1286 2024-04-04 15:32:50.261367 libresvip-1.1.2/libresvip/plugins/ufdata/model.py
--rw-r--r--   0        0        0      125 2024-02-22 15:40:21.285497 libresvip-1.1.2/libresvip/plugins/ufdata/options.py
--rw-r--r--   0        0        0    25204 2024-04-30 20:11:46.826346 libresvip-1.1.2/libresvip/plugins/ufdata/ufdata.yapsy-plugin
--rw-r--r--   0        0        0     1005 2024-04-04 15:32:50.262370 libresvip-1.1.2/libresvip/plugins/ufdata/ufdata_converter.py
--rw-r--r--   0        0        0     3019 2024-03-04 16:48:05.021992 libresvip-1.1.2/libresvip/plugins/ufdata/ufdata_generator.py
--rw-r--r--   0        0        0     4414 2024-04-04 15:32:50.263369 libresvip-1.1.2/libresvip/plugins/ufdata/ufdata_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.287504 libresvip-1.1.2/libresvip/plugins/ust/__init__.py
--rw-r--r--   0        0        0      220 2024-02-22 15:40:21.287504 libresvip-1.1.2/libresvip/plugins/ust/constants.py
--rw-r--r--   0        0        0      859 2024-02-22 15:40:21.288508 libresvip-1.1.2/libresvip/plugins/ust/interpolation.py
--rw-r--r--   0        0        0    17060 2024-03-11 13:13:40.358282 libresvip-1.1.2/libresvip/plugins/ust/model.py
--rw-r--r--   0        0        0      614 2024-04-19 22:30:20.059096 libresvip-1.1.2/libresvip/plugins/ust/options.py
--rw-r--r--   0        0        0     2060 2024-04-04 15:32:50.264367 libresvip-1.1.2/libresvip/plugins/ust/pitch_mode1.py
--rw-r--r--   0        0        0     9626 2024-04-04 15:32:50.265367 libresvip-1.1.2/libresvip/plugins/ust/pitch_mode2.py
--rw-r--r--   0        0        0     1781 2024-02-22 15:40:21.289493 libresvip-1.1.2/libresvip/plugins/ust/rdp_simplification.py
--rw-r--r--   0        0        0     1076 2024-03-04 16:48:05.024002 libresvip-1.1.2/libresvip/plugins/ust/resampling.py
--rw-r--r--   0        0        0     3600 2024-02-22 15:40:21.290497 libresvip-1.1.2/libresvip/plugins/ust/template.py
--rw-r--r--   0        0        0     8187 2024-02-22 15:40:21.291513 libresvip-1.1.2/libresvip/plugins/ust/ust.yapsy-plugin
--rw-r--r--   0        0        0      940 2024-04-19 22:31:18.927764 libresvip-1.1.2/libresvip/plugins/ust/ust_converter.py
--rw-r--r--   0        0        0     4545 2024-03-11 21:42:10.409173 libresvip-1.1.2/libresvip/plugins/ust/ust_generator.py
--rw-r--r--   0        0        0     6093 2024-03-23 15:29:05.958094 libresvip-1.1.2/libresvip/plugins/ust/ust_parser.py
--rw-r--r--   0        0        0     3270 2024-04-05 21:58:38.955510 libresvip-1.1.2/libresvip/plugins/ust/vibrato_param.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.292072 libresvip-1.1.2/libresvip/plugins/ustx/__init__.py
--rw-r--r--   0        0        0     6283 2024-03-04 16:48:05.024934 libresvip-1.1.2/libresvip/plugins/ustx/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.959093 libresvip-1.1.2/libresvip/plugins/ustx/options.py
--rw-r--r--   0        0        0    45293 2024-02-22 15:40:21.294124 libresvip-1.1.2/libresvip/plugins/ustx/ustx.yapsy-plugin
--rw-r--r--   0        0        0     1061 2024-03-12 19:57:09.206525 libresvip-1.1.2/libresvip/plugins/ustx/ustx_converter.py
--rw-r--r--   0        0        0     8246 2024-04-04 23:03:45.113941 libresvip-1.1.2/libresvip/plugins/ustx/ustx_generator.py
--rw-r--r--   0        0        0     7048 2024-03-23 15:29:05.960094 libresvip-1.1.2/libresvip/plugins/ustx/ustx_parser.py
--rw-r--r--   0        0        0     4584 2024-03-11 13:13:40.361335 libresvip-1.1.2/libresvip/plugins/ustx/util.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.295117 libresvip-1.1.2/libresvip/plugins/ustx/utils/__init__.py
--rw-r--r--   0        0        0      407 2024-04-05 21:59:21.996830 libresvip-1.1.2/libresvip/plugins/ustx/utils/lyric_util.py
--rw-r--r--   0        0        0      634 2024-02-24 21:21:44.007536 libresvip-1.1.2/libresvip/plugins/ustx/utils/music_math.py
--rw-r--r--   0        0        0     6102 2024-02-22 15:40:21.296134 libresvip-1.1.2/libresvip/plugins/ustx/utils/time_axis.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.296134 libresvip-1.1.2/libresvip/plugins/vog/__init__.py
--rw-r--r--   0        0        0      766 2024-02-22 15:40:21.297120 libresvip-1.1.2/libresvip/plugins/vog/model.py
--rw-r--r--   0        0        0      359 2024-03-23 15:29:05.960094 libresvip-1.1.2/libresvip/plugins/vog/options.py
--rw-r--r--   0        0        0    63065 2024-02-22 15:40:21.298121 libresvip-1.1.2/libresvip/plugins/vog/vog.yapsy-plugin
--rw-r--r--   0        0        0     1347 2024-03-23 15:29:05.962094 libresvip-1.1.2/libresvip/plugins/vog/vogen_converter.py
--rw-r--r--   0        0        0     1922 2024-03-18 14:02:32.510275 libresvip-1.1.2/libresvip/plugins/vog/vogen_generator.py
--rw-r--r--   0        0        0     1658 2024-02-22 15:40:21.299208 libresvip-1.1.2/libresvip/plugins/vog/vogen_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.299208 libresvip-1.1.2/libresvip/plugins/vpr/__init__.py
--rw-r--r--   0        0        0      434 2024-03-04 16:48:05.027944 libresvip-1.1.2/libresvip/plugins/vpr/constants.py
--rw-r--r--   0        0        0     9840 2024-02-22 15:40:21.300231 libresvip-1.1.2/libresvip/plugins/vpr/model.py
--rw-r--r--   0        0        0     1285 2024-03-23 15:29:05.962094 libresvip-1.1.2/libresvip/plugins/vpr/options.py
--rw-r--r--   0        0        0     4847 2024-03-04 16:48:05.029005 libresvip-1.1.2/libresvip/plugins/vpr/vocaloid_pitch.py
--rw-r--r--   0        0        0    14147 2024-02-22 15:40:21.300231 libresvip-1.1.2/libresvip/plugins/vpr/vpr.yapsy-plugin
--rw-r--r--   0        0        0     1515 2024-04-04 15:32:50.266367 libresvip-1.1.2/libresvip/plugins/vpr/vpr_converter.py
--rw-r--r--   0        0        0    10082 2024-04-04 15:32:50.267366 libresvip-1.1.2/libresvip/plugins/vpr/vpr_generator.py
--rw-r--r--   0        0        0     6440 2024-03-23 15:29:05.963094 libresvip-1.1.2/libresvip/plugins/vpr/vpr_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.302894 libresvip-1.1.2/libresvip/plugins/vshp/__init__.py
--rw-r--r--   0        0        0     5774 2024-02-22 15:40:21.303892 libresvip-1.1.2/libresvip/plugins/vshp/model.py
--rw-r--r--   0        0        0      532 2024-02-22 15:40:21.303892 libresvip-1.1.2/libresvip/plugins/vshp/options.py
--rw-r--r--   0        0        0      351 2024-02-22 15:40:21.304891 libresvip-1.1.2/libresvip/plugins/vshp/utils.py
--rw-r--r--   0        0        0      522 2024-02-22 15:40:21.304891 libresvip-1.1.2/libresvip/plugins/vshp/vocalshifter_converter.py
--rw-r--r--   0        0        0     9778 2024-02-24 21:21:44.008569 libresvip-1.1.2/libresvip/plugins/vshp/vocalshifter_parser.py
--rw-r--r--   0        0        0     9560 2024-03-05 19:32:37.534334 libresvip-1.1.2/libresvip/plugins/vshp/vshp.yapsy-plugin
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.305892 libresvip-1.1.2/libresvip/plugins/vspx/__init__.py
--rw-r--r--   0        0        0    12454 2024-02-24 21:21:44.009521 libresvip-1.1.2/libresvip/plugins/vspx/model.py
--rw-r--r--   0        0        0      325 2024-03-23 15:29:05.965117 libresvip-1.1.2/libresvip/plugins/vspx/options.py
--rw-r--r--   0        0        0     2859 2024-04-03 23:14:53.054645 libresvip-1.1.2/libresvip/plugins/vspx/vocalsharp_converter.py
--rw-r--r--   0        0        0     5428 2024-02-22 15:40:21.307892 libresvip-1.1.2/libresvip/plugins/vspx/vspx.yapsy-plugin
--rw-r--r--   0        0        0     7072 2024-02-24 21:21:44.010521 libresvip-1.1.2/libresvip/plugins/vspx/vspx_generator.py
--rw-r--r--   0        0        0     8035 2024-03-04 16:48:05.031947 libresvip-1.1.2/libresvip/plugins/vspx/vspx_interval_dict.py
--rw-r--r--   0        0        0     5857 2024-03-23 15:29:05.966101 libresvip-1.1.2/libresvip/plugins/vspx/vspx_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.308892 libresvip-1.1.2/libresvip/plugins/vsq/__init__.py
--rw-r--r--   0        0        0      246 2024-03-04 16:48:05.031947 libresvip-1.1.2/libresvip/plugins/vsq/constants.py
--rw-r--r--   0        0        0     1257 2024-03-23 15:29:05.966101 libresvip-1.1.2/libresvip/plugins/vsq/options.py
--rw-r--r--   0        0        0     5055 2024-03-04 16:48:05.032934 libresvip-1.1.2/libresvip/plugins/vsq/vocaloid_pitch.py
--rw-r--r--   0        0        0    49554 2024-02-22 15:40:21.310892 libresvip-1.1.2/libresvip/plugins/vsq/vsq.yapsy-plugin
--rw-r--r--   0        0        0      957 2024-02-22 15:40:21.310892 libresvip-1.1.2/libresvip/plugins/vsq/vsq_converter.py
--rw-r--r--   0        0        0     8510 2024-03-04 16:48:05.033991 libresvip-1.1.2/libresvip/plugins/vsq/vsq_generator.py
--rw-r--r--   0        0        0     8452 2024-03-23 15:29:05.967605 libresvip-1.1.2/libresvip/plugins/vsq/vsq_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.310892 libresvip-1.1.2/libresvip/plugins/vsqx/__init__.py
--rw-r--r--   0        0        0      332 2024-03-04 16:48:05.034998 libresvip-1.1.2/libresvip/plugins/vsqx/constants.py
--rw-r--r--   0        0        0      566 2024-03-23 15:29:05.968632 libresvip-1.1.2/libresvip/plugins/vsqx/enums.py
--rw-r--r--   0        0        0     4400 2024-02-22 15:40:21.312399 libresvip-1.1.2/libresvip/plugins/vsqx/model.py
--rw-r--r--   0        0        0        2 2024-02-22 15:40:21.312399 libresvip-1.1.2/libresvip/plugins/vsqx/models/__init__.py
--rw-r--r--   0        0        0    36025 2024-02-22 15:40:21.313408 libresvip-1.1.2/libresvip/plugins/vsqx/models/vsqx3.py
--rw-r--r--   0        0        0    32059 2024-02-22 15:40:21.313408 libresvip-1.1.2/libresvip/plugins/vsqx/models/vsqx4.py
--rw-r--r--   0        0        0     1078 2024-03-23 15:29:05.969611 libresvip-1.1.2/libresvip/plugins/vsqx/options.py
--rw-r--r--   0        0        0     5138 2024-03-28 15:49:09.959666 libresvip-1.1.2/libresvip/plugins/vsqx/vocaloid_pitch.py
--rw-r--r--   0        0        0    10117 2024-04-04 15:32:50.268367 libresvip-1.1.2/libresvip/plugins/vsqx/vsq3_generator.py
--rw-r--r--   0        0        0    10118 2024-04-04 15:32:50.269366 libresvip-1.1.2/libresvip/plugins/vsqx/vsq4_generator.py
--rw-r--r--   0        0        0    49665 2024-02-22 15:40:21.315408 libresvip-1.1.2/libresvip/plugins/vsqx/vsqx.yapsy-plugin
--rw-r--r--   0        0        0     3216 2024-04-03 23:14:53.055643 libresvip-1.1.2/libresvip/plugins/vsqx/vsqx_converter.py
--rw-r--r--   0        0        0     9672 2024-03-23 15:29:05.970610 libresvip-1.1.2/libresvip/plugins/vsqx/vsqx_parser.py
--rw-r--r--   0        0        0        0 2024-02-22 15:40:21.316410 libresvip-1.1.2/libresvip/plugins/y77/__init__.py
--rw-r--r--   0        0        0      742 2024-02-22 15:40:21.316410 libresvip-1.1.2/libresvip/plugins/y77/model.py
--rw-r--r--   0        0        0      321 2024-03-23 15:29:05.971609 libresvip-1.1.2/libresvip/plugins/y77/options.py
--rw-r--r--   0        0        0    48980 2024-02-22 15:40:21.317409 libresvip-1.1.2/libresvip/plugins/y77/y77.yapsy-plugin
--rw-r--r--   0        0        0     1042 2024-04-04 15:32:50.270964 libresvip-1.1.2/libresvip/plugins/y77/y77_converter.py
--rw-r--r--   0        0        0     3963 2024-03-18 14:02:43.305455 libresvip-1.1.2/libresvip/plugins/y77/y77_generator.py
--rw-r--r--   0        0        0     3190 2024-03-23 15:29:05.973610 libresvip-1.1.2/libresvip/plugins/y77/y77_parser.py
--rw-r--r--   0        0        0        0 2024-04-03 00:40:49.030321 libresvip-1.1.2/libresvip/py.typed
--rw-r--r--   0        0        0   270398 2024-02-22 15:40:21.319450 libresvip-1.1.2/libresvip/res/libresvip.ico
--rw-r--r--   0        0        0    54796 2024-05-06 13:31:51.722284 libresvip-1.1.2/libresvip/res/locales/zh_CN/LC_MESSAGES/libresvip.mo
--rw-r--r--   0        0        0        0 2024-02-24 21:21:44.013149 libresvip-1.1.2/libresvip/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-04-04 15:32:50.277874 libresvip-1.1.2/libresvip/utils/audio.py
--rw-r--r--   0        0        0     2441 2024-03-04 16:48:05.048671 libresvip-1.1.2/libresvip/utils/module_loading.py
--rw-r--r--   0        0        0     3970 2024-03-04 16:48:05.049643 libresvip-1.1.2/libresvip/utils/music_math.py
--rw-r--r--   0        0        0     1129 2024-02-24 21:21:44.014264 libresvip-1.1.2/libresvip/utils/search.py
--rw-r--r--   0        0        0     3309 2024-04-19 22:37:46.159611 libresvip-1.1.2/libresvip/utils/text.py
--rw-r--r--   0        0        0     1627 2024-04-17 18:48:56.821252 libresvip-1.1.2/libresvip/utils/translation.py
--rw-r--r--   0        0        0     1015 2024-04-03 23:14:53.055643 libresvip-1.1.2/libresvip/utils/xmlutils/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-19 21:54:15.974691 libresvip-1.1.2/libresvip/utils/xmlutils/native.py
--rw-r--r--   0        0        0      942 2024-03-12 20:28:45.735172 libresvip-1.1.2/libresvip/utils/yamlutils/__init__.py
--rw-r--r--   0        0        0     2833 2024-03-24 06:01:39.945387 libresvip-1.1.2/libresvip/utils/yamlutils/common.py
--rw-r--r--   0        0        0     3873 2024-03-24 06:01:51.194427 libresvip-1.1.2/libresvip/utils/yamlutils/dumper.py
--rw-r--r--   0        0        0     5052 2024-03-04 16:48:05.053289 libresvip-1.1.2/libresvip/utils/yamlutils/loader.py
--rw-r--r--   0        0        0      152 2024-04-17 14:03:30.170610 libresvip-1.1.2/libresvip/web/__init__.py
--rw-r--r--   0        0        0       97 2024-03-01 21:51:25.393182 libresvip-1.1.2/libresvip/web/__main__.py
--rw-r--r--   0        0        0     2344 2024-03-01 21:51:25.394220 libresvip-1.1.2/libresvip/web/elements.py
--rw-r--r--   0        0        0    96719 2024-04-28 04:40:58.986463 libresvip-1.1.2/libresvip/web/pages.py
--rw-r--r--   0        0        0     5406 2024-05-06 14:07:16.429652 libresvip-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5998 1970-01-01 00:00:00.000000 libresvip-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-02-22 15:40:21.193635 libresvip-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2562 2024-02-22 15:40:21.193635 libresvip-1.1.3/README.md
+-rw-r--r--   0        0        0       87 2024-05-16 12:29:15.828360 libresvip-1.1.3/libresvip/__init__.py
+-rw-r--r--   0        0        0      295 2024-04-04 15:32:50.232340 libresvip-1.1.3/libresvip/cli/__init__.py
+-rw-r--r--   0        0        0       76 2024-02-22 15:40:21.198477 libresvip-1.1.3/libresvip/cli/__main__.py
+-rw-r--r--   0        0        0      213 2024-02-22 15:40:21.198477 libresvip-1.1.3/libresvip/cli/app.py
+-rw-r--r--   0        0        0      180 2024-02-22 15:40:21.198477 libresvip-1.1.3/libresvip/cli/commands/__init__.py
+-rw-r--r--   0        0        0      862 2024-03-04 16:48:04.970405 libresvip-1.1.3/libresvip/cli/commands/conf.py
+-rw-r--r--   0        0        0     6395 2024-03-09 15:39:33.257482 libresvip-1.1.3/libresvip/cli/commands/plugin.py
+-rw-r--r--   0        0        0     9237 2024-04-04 15:32:50.233347 libresvip-1.1.3/libresvip/cli/commands/proj.py
+-rw-r--r--   0        0        0     3231 2024-04-19 22:32:21.141370 libresvip-1.1.3/libresvip/cli/prompt.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.199452 libresvip-1.1.3/libresvip/core/__init__.py
+-rw-r--r--   0        0        0      647 2024-03-10 04:18:39.143052 libresvip-1.1.3/libresvip/core/compat.py
+-rw-r--r--   0        0        0     5142 2024-04-26 03:48:21.746001 libresvip-1.1.3/libresvip/core/config.py
+-rw-r--r--   0        0        0      635 2024-03-02 16:03:26.993803 libresvip-1.1.3/libresvip/core/constants.py
+-rw-r--r--   0        0        0      270 2024-03-04 16:48:04.971414 libresvip-1.1.3/libresvip/core/exceptions.py
+-rw-r--r--   0        0        0        2 2024-02-22 15:40:21.201450 libresvip-1.1.3/libresvip/core/lyric_phoneme/__init__.py
+-rw-r--r--   0        0        0     2988 2024-03-04 16:48:04.972451 libresvip-1.1.3/libresvip/core/lyric_phoneme/chinese/__init__.py
+-rw-r--r--   0        0        0     9449 2024-03-04 16:48:04.973454 libresvip-1.1.3/libresvip/core/lyric_phoneme/chinese/vocaloid_xsampa.py
+-rw-r--r--   0        0        0      464 2024-03-12 17:52:45.770726 libresvip-1.1.3/libresvip/core/lyric_phoneme/japanese/__init__.py
+-rw-r--r--   0        0        0     2789 2024-03-04 16:48:04.974452 libresvip-1.1.3/libresvip/core/lyric_phoneme/japanese/vocaloid_xsampa.py
+-rw-r--r--   0        0        0     1646 2024-02-24 21:21:43.979932 libresvip-1.1.3/libresvip/core/tick_counter.py
+-rw-r--r--   0        0        0     5850 2024-03-04 16:48:04.975456 libresvip-1.1.3/libresvip/core/time_interval.py
+-rw-r--r--   0        0        0     4280 2024-02-24 21:21:43.979932 libresvip-1.1.3/libresvip/core/time_sync.py
+-rw-r--r--   0        0        0     1551 2024-04-04 15:32:50.235346 libresvip-1.1.3/libresvip/core/warning_types.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.203986 libresvip-1.1.3/libresvip/extension/__init__.py
+-rw-r--r--   0        0        0      986 2024-03-09 15:39:33.261482 libresvip-1.1.3/libresvip/extension/base.py
+-rw-r--r--   0        0        0     7583 2024-03-09 15:39:33.262482 libresvip-1.1.3/libresvip/extension/manager.py
+-rw-r--r--   0        0        0     3700 2024-03-09 15:39:33.263482 libresvip-1.1.3/libresvip/extension/meta_info.py
+-rw-r--r--   0        0        0    93928 2024-04-27 16:08:27.372830 libresvip-1.1.3/libresvip/gui/__init__.py
+-rw-r--r--   0        0        0     1135 2024-04-04 15:32:50.237346 libresvip-1.1.3/libresvip/gui/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-04 15:32:50.238347 libresvip-1.1.3/libresvip/gui/models/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-04 15:32:50.238347 libresvip-1.1.3/libresvip/gui/models/base_task.py
+-rw-r--r--   0        0        0     8893 2024-04-26 15:58:39.835740 libresvip-1.1.3/libresvip/gui/models/list_models.py
+-rw-r--r--   0        0        0     7284 2024-04-27 00:43:36.532622 libresvip-1.1.3/libresvip/gui/models/table_models.py
+-rw-r--r--   0        0        0      846 2024-03-26 19:35:54.341234 libresvip-1.1.3/libresvip/gui/modules/__init__.py
+-rw-r--r--   0        0        0      518 2024-03-26 19:35:54.342244 libresvip-1.1.3/libresvip/gui/modules/application.py
+-rw-r--r--   0        0        0      865 2024-02-24 21:21:43.980924 libresvip-1.1.3/libresvip/gui/modules/clipboard.py
+-rw-r--r--   0        0        0     5483 2024-04-25 23:57:25.750197 libresvip-1.1.3/libresvip/gui/modules/config_items.py
+-rw-r--r--   0        0        0      810 2024-02-22 15:40:21.213022 libresvip-1.1.3/libresvip/gui/modules/font_loader.py
+-rw-r--r--   0        0        0     2533 2024-03-04 16:48:04.979510 libresvip-1.1.3/libresvip/gui/modules/frameless_window.py
+-rw-r--r--   0        0        0     8815 2024-03-04 16:48:04.980438 libresvip-1.1.3/libresvip/gui/modules/frameless_window_win32.py
+-rw-r--r--   0        0        0     2218 2024-04-17 18:49:57.998947 libresvip-1.1.3/libresvip/gui/modules/locale_switcher.py
+-rw-r--r--   0        0        0    10138 2024-05-16 13:57:36.350218 libresvip-1.1.3/libresvip/gui/modules/notifier.py
+-rw-r--r--   0        0        0    39784 2024-04-27 01:43:02.793017 libresvip-1.1.3/libresvip/gui/modules/task_manager.py
+-rw-r--r--   0        0        0      390 2024-02-22 15:40:21.215023 libresvip-1.1.3/libresvip/gui/modules/url_opener.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.215023 libresvip-1.1.3/libresvip/gui/modules/vendor/__init__.py
+-rw-r--r--   0        0        0    25262 2024-03-24 06:00:55.521020 libresvip-1.1.3/libresvip/gui/modules/vendor/qasync/__init__.py
+-rw-r--r--   0        0        0      497 2024-03-04 16:48:04.983407 libresvip-1.1.3/libresvip/gui/modules/vendor/qasync/_common.py
+-rw-r--r--   0        0        0     7507 2024-03-04 16:48:04.984405 libresvip-1.1.3/libresvip/gui/modules/vendor/qasync/_unix.py
+-rw-r--r--   0        0        0     9345 2024-03-04 16:48:04.985406 libresvip-1.1.3/libresvip/gui/modules/vendor/qasync/_windows.py
+-rw-r--r--   0        0        0      981 2024-02-22 15:40:21.217025 libresvip-1.1.3/libresvip/gui/modules/win32_constants.py
+-rw-r--r--   0        0        0        0 2024-03-09 15:39:33.266482 libresvip-1.1.3/libresvip/middlewares/pitch_shift/__init__.py
+-rw-r--r--   0        0        0      219 2024-03-09 15:39:33.266482 libresvip-1.1.3/libresvip/middlewares/pitch_shift/options.py
+-rw-r--r--   0        0        0     2136 2024-03-09 15:39:33.267482 libresvip-1.1.3/libresvip/middlewares/pitch_shift/pitch_shift.py
+-rw-r--r--   0        0        0      181 2024-03-09 15:39:33.267482 libresvip-1.1.3/libresvip/middlewares/pitch_shift/pitch_shift.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-03-09 15:39:33.267482 libresvip-1.1.3/libresvip/middlewares/project_zoom/__init__.py
+-rw-r--r--   0        0        0     1009 2024-03-09 15:39:33.267482 libresvip-1.1.3/libresvip/middlewares/project_zoom/options.py
+-rw-r--r--   0        0        0      508 2024-03-09 15:39:33.267482 libresvip-1.1.3/libresvip/middlewares/project_zoom/project_zoom.py
+-rw-r--r--   0        0        0      220 2024-03-09 15:39:33.269050 libresvip-1.1.3/libresvip/middlewares/project_zoom/project_zoom.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-03-09 15:39:33.269050 libresvip-1.1.3/libresvip/middlewares/pronounciation_conversion/__init__.py
+-rw-r--r--   0        0        0      791 2024-03-09 15:39:33.269050 libresvip-1.1.3/libresvip/middlewares/pronounciation_conversion/options.py
+-rw-r--r--   0        0        0     1510 2024-03-09 15:39:33.269050 libresvip-1.1.3/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.py
+-rw-r--r--   0        0        0      270 2024-03-09 15:39:33.269989 libresvip-1.1.3/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-03-09 15:39:33.269989 libresvip-1.1.3/libresvip/middlewares/remove_short_silences/__init__.py
+-rw-r--r--   0        0        0      882 2024-03-09 15:39:33.269989 libresvip-1.1.3/libresvip/middlewares/remove_short_silences/options.py
+-rw-r--r--   0        0        0      953 2024-03-09 15:39:33.270989 libresvip-1.1.3/libresvip/middlewares/remove_short_silences/remove_short_silences.py
+-rw-r--r--   0        0        0      243 2024-03-09 15:39:33.270989 libresvip-1.1.3/libresvip/middlewares/remove_short_silences/remove_short_silences.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-04-17 19:53:22.520237 libresvip-1.1.3/libresvip/middlewares/replace_lyric/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-19 05:00:08.861563 libresvip-1.1.3/libresvip/middlewares/replace_lyric/options.py
+-rw-r--r--   0        0        0     1326 2024-04-27 16:08:27.375841 libresvip-1.1.3/libresvip/middlewares/replace_lyric/replace_lyric.py
+-rw-r--r--   0        0        0      319 2024-04-19 21:12:02.082450 libresvip-1.1.3/libresvip/middlewares/replace_lyric/replace_lyric.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.217025 libresvip-1.1.3/libresvip/model/__init__.py
+-rw-r--r--   0        0        0    10233 2024-05-19 09:55:57.177960 libresvip-1.1.3/libresvip/model/base.py
+-rw-r--r--   0        0        0     1373 2024-03-23 15:29:05.921080 libresvip-1.1.3/libresvip/model/option_mixins.py
+-rw-r--r--   0        0        0     3152 2024-02-24 21:21:43.981935 libresvip-1.1.3/libresvip/model/point.py
+-rw-r--r--   0        0        0     7529 2024-05-03 03:31:10.216309 libresvip-1.1.3/libresvip/model/relative_pitch_curve.py
+-rw-r--r--   0        0        0     7848 2024-03-18 14:03:10.224552 libresvip-1.1.3/libresvip/model/reset_time_axis.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.218004 libresvip-1.1.3/libresvip/plugins/acep/__init__.py
+-rw-r--r--   0        0        0    54700 2024-02-22 15:40:21.219535 libresvip-1.1.3/libresvip/plugins/acep/ace-studio.yapsy-plugin
+-rw-r--r--   0        0        0     1487 2024-02-22 15:40:21.219535 libresvip-1.1.3/libresvip/plugins/acep/ace_curve_utils.py
+-rw-r--r--   0        0        0      949 2024-04-25 14:59:40.397933 libresvip-1.1.3/libresvip/plugins/acep/ace_studio_converter.py
+-rw-r--r--   0        0        0    20088 2024-05-19 05:44:30.560559 libresvip-1.1.3/libresvip/plugins/acep/ace_studio_generator.py
+-rw-r--r--   0        0        0    17695 2024-05-17 23:01:20.660154 libresvip-1.1.3/libresvip/plugins/acep/ace_studio_parser.py
+-rw-r--r--   0        0        0     1620 2024-03-04 16:48:04.991428 libresvip-1.1.3/libresvip/plugins/acep/acep_io.py
+-rw-r--r--   0        0        0     5339 2024-03-04 16:48:04.991428 libresvip-1.1.3/libresvip/plugins/acep/base_pitch_curve.py
+-rw-r--r--   0        0        0      386 2024-02-22 15:40:21.221571 libresvip-1.1.3/libresvip/plugins/acep/color_pool.py
+-rw-r--r--   0        0        0      565 2024-02-24 21:21:43.984931 libresvip-1.1.3/libresvip/plugins/acep/curve_segment_utils.py
+-rw-r--r--   0        0        0    14273 2024-05-17 23:01:16.675271 libresvip-1.1.3/libresvip/plugins/acep/model.py
+-rw-r--r--   0        0        0    11102 2024-04-04 15:32:50.247348 libresvip-1.1.3/libresvip/plugins/acep/options.py
+-rw-r--r--   0        0        0     2518 2024-04-04 15:32:50.248346 libresvip-1.1.3/libresvip/plugins/acep/singers.py
+-rw-r--r--   0        0        0     1215 2024-02-22 15:40:21.223573 libresvip-1.1.3/libresvip/plugins/acep/time_utils.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.223573 libresvip-1.1.3/libresvip/plugins/aisp/__init__.py
+-rw-r--r--   0        0        0     1486 2024-02-22 15:40:21.223573 libresvip-1.1.3/libresvip/plugins/aisp/aisingers_converter.py
+-rw-r--r--   0        0        0     9276 2024-03-04 16:48:04.992962 libresvip-1.1.3/libresvip/plugins/aisp/aisingers_generator.py
+-rw-r--r--   0        0        0     4725 2024-03-23 15:29:05.925080 libresvip-1.1.3/libresvip/plugins/aisp/aisingers_parser.py
+-rw-r--r--   0        0        0    23952 2024-02-22 15:40:21.224550 libresvip-1.1.3/libresvip/plugins/aisp/aisp.yapsy-plugin
+-rw-r--r--   0        0        0     4713 2024-02-22 15:40:21.225582 libresvip-1.1.3/libresvip/plugins/aisp/model.py
+-rw-r--r--   0        0        0      325 2024-04-22 06:45:10.507210 libresvip-1.1.3/libresvip/plugins/aisp/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.225582 libresvip-1.1.3/libresvip/plugins/ccs/__init__.py
+-rw-r--r--   0        0        0    38382 2024-02-22 15:40:21.226575 libresvip-1.1.3/libresvip/plugins/ccs/ccs.yapsy-plugin
+-rw-r--r--   0        0        0     1350 2024-02-22 15:40:21.227574 libresvip-1.1.3/libresvip/plugins/ccs/cevio_converter.py
+-rw-r--r--   0        0        0     8349 2024-04-04 15:32:50.249954 libresvip-1.1.3/libresvip/plugins/ccs/cevio_generator.py
+-rw-r--r--   0        0        0    10117 2024-04-30 12:50:10.287752 libresvip-1.1.3/libresvip/plugins/ccs/cevio_parser.py
+-rw-r--r--   0        0        0    17562 2024-05-09 20:53:19.374299 libresvip-1.1.3/libresvip/plugins/ccs/cevio_pitch.py
+-rw-r--r--   0        0        0      296 2024-02-22 15:40:21.228574 libresvip-1.1.3/libresvip/plugins/ccs/constants.py
+-rw-r--r--   0        0        0    31397 2024-05-07 19:04:39.988623 libresvip-1.1.3/libresvip/plugins/ccs/model.py
+-rw-r--r--   0        0        0      567 2024-03-23 15:29:05.927080 libresvip-1.1.3/libresvip/plugins/ccs/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.229551 libresvip-1.1.3/libresvip/plugins/ds/__init__.py
+-rw-r--r--   0        0        0     6352 2024-02-22 15:40:21.230060 libresvip-1.1.3/libresvip/plugins/ds/dicts/opencpop-extension.txt
+-rw-r--r--   0        0        0     4475 2024-02-22 15:40:21.230241 libresvip-1.1.3/libresvip/plugins/ds/dicts/opencpop-strict.txt
+-rw-r--r--   0        0        0     4468 2024-02-22 15:40:21.230241 libresvip-1.1.3/libresvip/plugins/ds/dicts/opencpop.txt
+-rw-r--r--   0        0        0     2051 2024-02-22 15:40:21.230241 libresvip-1.1.3/libresvip/plugins/ds/diffsinger_converter.py
+-rw-r--r--   0        0        0     1846 2024-02-22 15:40:21.231089 libresvip-1.1.3/libresvip/plugins/ds/diffsinger_generator.py
+-rw-r--r--   0        0        0     5222 2024-03-23 15:29:05.928079 libresvip-1.1.3/libresvip/plugins/ds/diffsinger_parser.py
+-rw-r--r--   0        0        0    31348 2024-02-22 15:40:21.232090 libresvip-1.1.3/libresvip/plugins/ds/ds.yapsy-plugin
+-rw-r--r--   0        0        0     3192 2024-02-22 15:40:21.232090 libresvip-1.1.3/libresvip/plugins/ds/model.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.232090 libresvip-1.1.3/libresvip/plugins/ds/models/__init__.py
+-rw-r--r--   0        0        0     1292 2024-02-22 15:40:21.233090 libresvip-1.1.3/libresvip/plugins/ds/models/ds_note.py
+-rw-r--r--   0        0        0      225 2024-02-22 15:40:21.233090 libresvip-1.1.3/libresvip/plugins/ds/models/ds_param_curve.py
+-rw-r--r--   0        0        0      118 2024-02-22 15:40:21.233090 libresvip-1.1.3/libresvip/plugins/ds/models/ds_param_node.py
+-rw-r--r--   0        0        0     3205 2024-02-22 15:40:21.233090 libresvip-1.1.3/libresvip/plugins/ds/models/ds_project.py
+-rw-r--r--   0        0        0     1984 2024-03-23 15:29:05.929080 libresvip-1.1.3/libresvip/plugins/ds/options.py
+-rw-r--r--   0        0        0      786 2024-02-24 21:21:43.986928 libresvip-1.1.3/libresvip/plugins/ds/phoneme_dict.py
+-rw-r--r--   0        0        0        2 2024-02-22 15:40:21.234069 libresvip-1.1.3/libresvip/plugins/ds/utils/__init__.py
+-rw-r--r--   0        0        0     1452 2024-03-04 16:48:04.996982 libresvip-1.1.3/libresvip/plugins/ds/utils/gender_param_utils.py
+-rw-r--r--   0        0        0      294 2024-04-04 23:42:44.572812 libresvip-1.1.3/libresvip/plugins/ds/utils/lyric_util.py
+-rw-r--r--   0        0        0     6771 2024-04-04 23:06:53.822302 libresvip-1.1.3/libresvip/plugins/ds/utils/note_list_util.py
+-rw-r--r--   0        0        0     1380 2024-02-24 21:21:43.988828 libresvip-1.1.3/libresvip/plugins/ds/utils/pinyin_util.py
+-rw-r--r--   0        0        0     1613 2024-02-24 21:21:43.988828 libresvip-1.1.3/libresvip/plugins/ds/utils/pitch_param_utils.py
+-rw-r--r--   0        0        0     3990 2024-02-22 15:40:21.236071 libresvip-1.1.3/libresvip/plugins/ds/utils/project_util.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.236071 libresvip-1.1.3/libresvip/plugins/dv/__init__.py
+-rw-r--r--   0        0        0    11432 2024-03-04 16:48:04.999015 libresvip-1.1.3/libresvip/plugins/dv/constants.py
+-rw-r--r--   0        0        0      847 2024-02-22 15:40:21.237092 libresvip-1.1.3/libresvip/plugins/dv/deepvocal_converter.py
+-rw-r--r--   0        0        0    10745 2024-02-22 23:04:58.757287 libresvip-1.1.3/libresvip/plugins/dv/deepvocal_pitch.py
+-rw-r--r--   0        0        0     6453 2024-02-22 15:40:21.238069 libresvip-1.1.3/libresvip/plugins/dv/dv.yapsy-plugin
+-rw-r--r--   0        0        0     8519 2024-02-24 21:21:43.989880 libresvip-1.1.3/libresvip/plugins/dv/dv_generator.py
+-rw-r--r--   0        0        0     6800 2024-03-23 15:29:05.930098 libresvip-1.1.3/libresvip/plugins/dv/dv_parser.py
+-rw-r--r--   0        0        0     4927 2024-02-22 15:40:21.239070 libresvip-1.1.3/libresvip/plugins/dv/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.931081 libresvip-1.1.3/libresvip/plugins/dv/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.239070 libresvip-1.1.3/libresvip/plugins/gj/__init__.py
+-rw-r--r--   0        0        0     5113 2024-02-22 15:40:21.239070 libresvip-1.1.3/libresvip/plugins/gj/constants.py
+-rw-r--r--   0        0        0    72345 2024-02-22 15:40:21.240660 libresvip-1.1.3/libresvip/plugins/gj/gjgj.yapsy-plugin
+-rw-r--r--   0        0        0     1120 2024-02-22 15:40:21.240660 libresvip-1.1.3/libresvip/plugins/gj/gjgj_converter.py
+-rw-r--r--   0        0        0    10541 2024-04-04 15:32:50.250856 libresvip-1.1.3/libresvip/plugins/gj/gjgj_generator.py
+-rw-r--r--   0        0        0     8051 2024-03-23 15:29:05.933100 libresvip-1.1.3/libresvip/plugins/gj/gjgj_parser.py
+-rw-r--r--   0        0        0     6172 2024-02-22 15:40:21.241591 libresvip-1.1.3/libresvip/plugins/gj/model.py
+-rw-r--r--   0        0        0      784 2024-03-23 15:29:05.933100 libresvip-1.1.3/libresvip/plugins/gj/options.py
+-rw-r--r--   0        0        0      303 2024-02-22 15:40:21.241591 libresvip-1.1.3/libresvip/plugins/gj/singers.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.241591 libresvip-1.1.3/libresvip/plugins/json/__init__.py
+-rw-r--r--   0        0        0     1225 2024-02-22 15:40:21.242586 libresvip-1.1.3/libresvip/plugins/json/jsonsvip.yapsy-plugin
+-rw-r--r--   0        0        0      965 2024-04-25 14:59:49.047701 libresvip-1.1.3/libresvip/plugins/json/jsonsvip_converter.py
+-rw-r--r--   0        0        0      350 2024-02-22 15:40:21.243587 libresvip-1.1.3/libresvip/plugins/json/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.243587 libresvip-1.1.3/libresvip/plugins/lrc/__init__.py
+-rw-r--r--   0        0        0     1400 2024-02-22 15:40:21.243587 libresvip-1.1.3/libresvip/plugins/lrc/lrc.yapsy-plugin
+-rw-r--r--   0        0        0      484 2024-02-22 15:40:21.244588 libresvip-1.1.3/libresvip/plugins/lrc/lrc_converter.py
+-rw-r--r--   0        0        0     4320 2024-02-24 21:21:43.990884 libresvip-1.1.3/libresvip/plugins/lrc/lrc_generator.py
+-rw-r--r--   0        0        0      670 2024-02-22 15:40:21.244588 libresvip-1.1.3/libresvip/plugins/lrc/model.py
+-rw-r--r--   0        0        0     2391 2024-02-22 15:40:21.244588 libresvip-1.1.3/libresvip/plugins/lrc/options.py
+-rw-r--r--   0        0        0      692 2024-02-22 15:40:21.245587 libresvip-1.1.3/libresvip/plugins/lrc/template.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.245587 libresvip-1.1.3/libresvip/plugins/mid/__init__.py
+-rw-r--r--   0        0        0     1990 2024-02-22 15:40:21.245587 libresvip-1.1.3/libresvip/plugins/mid/constants.py
+-rw-r--r--   0        0        0     5992 2024-02-22 15:40:21.246587 libresvip-1.1.3/libresvip/plugins/mid/mid.yapsy-plugin
+-rw-r--r--   0        0        0      982 2024-02-24 00:53:21.067110 libresvip-1.1.3/libresvip/plugins/mid/midi_converter.py
+-rw-r--r--   0        0        0     6509 2024-03-04 16:48:04.999015 libresvip-1.1.3/libresvip/plugins/mid/midi_generator.py
+-rw-r--r--   0        0        0    12410 2024-04-04 15:32:50.251856 libresvip-1.1.3/libresvip/plugins/mid/midi_parser.py
+-rw-r--r--   0        0        0     2784 2024-03-04 16:48:05.001983 libresvip-1.1.3/libresvip/plugins/mid/midi_pitch.py
+-rw-r--r--   0        0        0      485 2024-02-22 15:40:21.247587 libresvip-1.1.3/libresvip/plugins/mid/note_overlap.py
+-rw-r--r--   0        0        0     3008 2024-03-23 15:29:05.936080 libresvip-1.1.3/libresvip/plugins/mid/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.247587 libresvip-1.1.3/libresvip/plugins/mtp/__init__.py
+-rw-r--r--   0        0        0     5764 2024-02-22 15:40:21.247587 libresvip-1.1.3/libresvip/plugins/mtp/model.py
+-rw-r--r--   0        0        0    63944 2024-02-22 15:40:21.248586 libresvip-1.1.3/libresvip/plugins/mtp/mtp.yapsy-plugin
+-rw-r--r--   0        0        0      782 2024-02-22 15:40:21.249586 libresvip-1.1.3/libresvip/plugins/mtp/muta_converter.py
+-rw-r--r--   0        0        0     7329 2024-05-01 15:16:27.115338 libresvip-1.1.3/libresvip/plugins/mtp/muta_generator.py
+-rw-r--r--   0        0        0     5159 2024-05-01 15:02:14.057268 libresvip-1.1.3/libresvip/plugins/mtp/muta_parser.py
+-rw-r--r--   0        0        0      495 2024-03-23 15:29:05.938080 libresvip-1.1.3/libresvip/plugins/mtp/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.249586 libresvip-1.1.3/libresvip/plugins/musicxml/__init__.py
+-rw-r--r--   0        0        0     1375 2024-02-22 15:40:21.249586 libresvip-1.1.3/libresvip/plugins/musicxml/model.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.251137 libresvip-1.1.3/libresvip/plugins/musicxml/models/__init__.py
+-rw-r--r--   0        0        0   375472 2024-02-22 15:40:21.252183 libresvip-1.1.3/libresvip/plugins/musicxml/models/mxml2.py
+-rw-r--r--   0        0        0     1577 2024-02-22 15:40:21.253184 libresvip-1.1.3/libresvip/plugins/musicxml/models/xlink.py
+-rw-r--r--   0        0        0      118 2024-02-22 15:40:21.253184 libresvip-1.1.3/libresvip/plugins/musicxml/models/xml.py
+-rw-r--r--   0        0        0    17317 2024-02-22 15:40:21.253184 libresvip-1.1.3/libresvip/plugins/musicxml/musicxml.yapsy-plugin
+-rw-r--r--   0        0        0     1699 2024-04-03 23:14:53.053648 libresvip-1.1.3/libresvip/plugins/musicxml/musicxml_converter.py
+-rw-r--r--   0        0        0    14877 2024-02-24 21:21:43.993929 libresvip-1.1.3/libresvip/plugins/musicxml/musicxml_generator.py
+-rw-r--r--   0        0        0     6295 2024-02-24 21:21:43.993929 libresvip-1.1.3/libresvip/plugins/musicxml/musicxml_parser.py
+-rw-r--r--   0        0        0      125 2024-02-22 15:40:21.255194 libresvip-1.1.3/libresvip/plugins/musicxml/options.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.255194 libresvip-1.1.3/libresvip/plugins/nn/__init__.py
+-rw-r--r--   0        0        0     4875 2024-02-22 15:40:21.255194 libresvip-1.1.3/libresvip/plugins/nn/model.py
+-rw-r--r--   0        0        0     1068 2024-03-23 15:29:05.939080 libresvip-1.1.3/libresvip/plugins/nn/niaoniao_converter.py
+-rw-r--r--   0        0        0     5374 2024-03-23 15:29:05.940080 libresvip-1.1.3/libresvip/plugins/nn/niaoniao_generator.py
+-rw-r--r--   0        0        0     3564 2024-03-23 15:29:05.940080 libresvip-1.1.3/libresvip/plugins/nn/niaoniao_parser.py
+-rw-r--r--   0        0        0    21285 2024-02-22 15:40:21.256182 libresvip-1.1.3/libresvip/plugins/nn/nn.yapsy-plugin
+-rw-r--r--   0        0        0      467 2024-03-23 15:29:05.941583 libresvip-1.1.3/libresvip/plugins/nn/options.py
+-rw-r--r--   0        0        0     1008 2024-02-22 15:40:21.257195 libresvip-1.1.3/libresvip/plugins/nn/template.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.257195 libresvip-1.1.3/libresvip/plugins/ppsf/__init__.py
+-rw-r--r--   0        0        0     7813 2024-02-22 15:40:21.257195 libresvip-1.1.3/libresvip/plugins/ppsf/legacy_model.py
+-rw-r--r--   0        0        0    12763 2024-02-22 15:40:21.258193 libresvip-1.1.3/libresvip/plugins/ppsf/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.942587 libresvip-1.1.3/libresvip/plugins/ppsf/options.py
+-rw-r--r--   0        0        0     1931 2024-04-04 15:32:50.252857 libresvip-1.1.3/libresvip/plugins/ppsf/piapro_studio_converter.py
+-rw-r--r--   0        0        0     8331 2024-03-09 15:39:33.271989 libresvip-1.1.3/libresvip/plugins/ppsf/piapro_studio_generator.py
+-rw-r--r--   0        0        0     6809 2024-02-22 15:40:21.259204 libresvip-1.1.3/libresvip/plugins/ppsf/piapro_studio_legacy_parser.py
+-rw-r--r--   0        0        0     5897 2024-03-23 15:29:05.943588 libresvip-1.1.3/libresvip/plugins/ppsf/piapro_studio_nt_parser.py
+-rw-r--r--   0        0        0    19426 2024-02-22 15:40:21.260207 libresvip-1.1.3/libresvip/plugins/ppsf/ppsf.yapsy-plugin
+-rw-r--r--   0        0        0     3256 2024-02-24 21:21:43.995835 libresvip-1.1.3/libresvip/plugins/ppsf/ppsf_interval_dict.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.260207 libresvip-1.1.3/libresvip/plugins/s5p/__init__.py
+-rw-r--r--   0        0        0     6036 2024-05-08 21:54:55.423825 libresvip-1.1.3/libresvip/plugins/s5p/model.py
+-rw-r--r--   0        0        0      344 2024-03-23 15:29:09.443412 libresvip-1.1.3/libresvip/plugins/s5p/options.py
+-rw-r--r--   0        0        0    52233 2024-02-22 15:40:21.261194 libresvip-1.1.3/libresvip/plugins/s5p/s5p.yapsy-plugin
+-rw-r--r--   0        0        0     1045 2024-02-22 15:40:21.261194 libresvip-1.1.3/libresvip/plugins/s5p/synthv_editor_converter.py
+-rw-r--r--   0        0        0     5609 2024-05-08 21:58:19.283039 libresvip-1.1.3/libresvip/plugins/s5p/synthv_editor_generator.py
+-rw-r--r--   0        0        0    11617 2024-05-08 21:58:19.283039 libresvip-1.1.3/libresvip/plugins/s5p/synthv_editor_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.262203 libresvip-1.1.3/libresvip/plugins/srt/__init__.py
+-rw-r--r--   0        0        0     1394 2024-02-22 15:40:21.262203 libresvip-1.1.3/libresvip/plugins/srt/options.py
+-rw-r--r--   0        0        0     1285 2024-02-22 15:40:21.263187 libresvip-1.1.3/libresvip/plugins/srt/srt.yapsy-plugin
+-rw-r--r--   0        0        0      503 2024-02-22 15:40:21.263187 libresvip-1.1.3/libresvip/plugins/srt/srt_converter.py
+-rw-r--r--   0        0        0     2696 2024-02-24 21:21:43.996926 libresvip-1.1.3/libresvip/plugins/srt/srt_generator.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.263187 libresvip-1.1.3/libresvip/plugins/svg/__init__.py
+-rw-r--r--   0        0        0     4552 2024-02-22 15:40:21.264194 libresvip-1.1.3/libresvip/plugins/svg/coordinate_helper.py
+-rw-r--r--   0        0        0      279 2024-02-22 15:40:21.264194 libresvip-1.1.3/libresvip/plugins/svg/model.py
+-rw-r--r--   0        0        0     3009 2024-02-22 15:40:21.264194 libresvip-1.1.3/libresvip/plugins/svg/options.py
+-rw-r--r--   0        0        0    15147 2024-02-22 15:40:21.265188 libresvip-1.1.3/libresvip/plugins/svg/svg.yapsy-plugin
+-rw-r--r--   0        0        0      568 2024-02-22 15:40:21.265188 libresvip-1.1.3/libresvip/plugins/svg/svg_converter.py
+-rw-r--r--   0        0        0     6739 2024-02-22 15:40:21.265188 libresvip-1.1.3/libresvip/plugins/svg/svg_factory.py
+-rw-r--r--   0        0        0     2422 2024-02-22 15:40:21.266243 libresvip-1.1.3/libresvip/plugins/svg/svg_generator.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.266243 libresvip-1.1.3/libresvip/plugins/svip/__init__.py
+-rw-r--r--   0        0        0    15042 2024-02-22 15:40:21.266243 libresvip-1.1.3/libresvip/plugins/svip/binsvip.yapsy-plugin
+-rw-r--r--   0        0        0     1561 2024-04-25 14:59:53.848685 libresvip-1.1.3/libresvip/plugins/svip/binsvip_converter.py
+-rw-r--r--   0        0        0    11038 2024-04-04 23:08:50.052929 libresvip-1.1.3/libresvip/plugins/svip/binsvip_generator.py
+-rw-r--r--   0        0        0     5944 2024-03-23 15:29:05.947587 libresvip-1.1.3/libresvip/plugins/svip/binsvip_parser.py
+-rw-r--r--   0        0        0     1602 2024-04-22 23:56:13.988906 libresvip-1.1.3/libresvip/plugins/svip/models.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.267240 libresvip-1.1.3/libresvip/plugins/svip/msnrbf/__init__.py
+-rw-r--r--   0        0        0    19970 2024-02-24 13:23:26.660918 libresvip-1.1.3/libresvip/plugins/svip/msnrbf/binary_models.py
+-rw-r--r--   0        0        0      498 2024-03-04 16:48:05.006115 libresvip-1.1.3/libresvip/plugins/svip/msnrbf/constants.py
+-rw-r--r--   0        0        0     1341 2024-03-04 16:48:05.007021 libresvip-1.1.3/libresvip/plugins/svip/msnrbf/nrbf_iobase.py
+-rw-r--r--   0        0        0     4956 2024-03-04 16:48:05.007021 libresvip-1.1.3/libresvip/plugins/svip/msnrbf/svip_reader.py
+-rw-r--r--   0        0        0    23277 2024-02-22 15:40:21.269238 libresvip-1.1.3/libresvip/plugins/svip/msnrbf/svip_writer.py
+-rw-r--r--   0        0        0    15021 2024-04-04 15:32:50.256857 libresvip-1.1.3/libresvip/plugins/svip/msnrbf/xstudio_models.py
+-rw-r--r--   0        0        0     3393 2024-03-23 15:29:05.948587 libresvip-1.1.3/libresvip/plugins/svip/options.py
+-rw-r--r--   0        0        0     1857 2024-02-22 15:40:21.270241 libresvip-1.1.3/libresvip/plugins/svip/singers.json
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.270241 libresvip-1.1.3/libresvip/plugins/svip3/__init__.py
+-rw-r--r--   0        0        0      397 2024-02-22 15:40:21.270241 libresvip-1.1.3/libresvip/plugins/svip3/color_pool.py
+-rw-r--r--   0        0        0      396 2024-03-04 16:48:05.009732 libresvip-1.1.3/libresvip/plugins/svip3/constants.py
+-rw-r--r--   0        0        0    12712 2024-04-26 16:10:27.006657 libresvip-1.1.3/libresvip/plugins/svip3/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.949587 libresvip-1.1.3/libresvip/plugins/svip3/options.py
+-rw-r--r--   0        0        0     1647 2024-05-09 20:54:54.690502 libresvip-1.1.3/libresvip/plugins/svip3/singers.json
+-rw-r--r--   0        0        0      243 2024-02-22 15:40:21.271242 libresvip-1.1.3/libresvip/plugins/svip3/singers.py
+-rw-r--r--   0        0        0    13560 2024-02-22 15:40:21.272276 libresvip-1.1.3/libresvip/plugins/svip3/svip3.yapsy-plugin
+-rw-r--r--   0        0        0      782 2024-03-23 15:29:05.950587 libresvip-1.1.3/libresvip/plugins/svip3/svip3_converter.py
+-rw-r--r--   0        0        0    11203 2024-04-04 15:32:50.257857 libresvip-1.1.3/libresvip/plugins/svip3/svip3_generator.py
+-rw-r--r--   0        0        0     8397 2024-03-23 15:29:05.951587 libresvip-1.1.3/libresvip/plugins/svip3/svip3_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.273244 libresvip-1.1.3/libresvip/plugins/svp/__init__.py
+-rw-r--r--   0        0        0      859 2024-02-22 15:40:21.273244 libresvip-1.1.3/libresvip/plugins/svp/constants.py
+-rw-r--r--   0        0        0      361 2024-02-22 15:40:21.275243 libresvip-1.1.3/libresvip/plugins/svp/interpolation.py
+-rw-r--r--   0        0        0      201 2024-03-14 11:33:30.285334 libresvip-1.1.3/libresvip/plugins/svp/interval_utils.py
+-rw-r--r--   0        0        0     1457 2024-02-22 15:40:21.275243 libresvip-1.1.3/libresvip/plugins/svp/lambert_w.py
+-rw-r--r--   0        0        0    18008 2024-03-14 13:43:05.687807 libresvip-1.1.3/libresvip/plugins/svp/layer_generator.py
+-rw-r--r--   0        0        0    22768 2024-05-19 06:28:56.331097 libresvip-1.1.3/libresvip/plugins/svp/model.py
+-rw-r--r--   0        0        0     5769 2024-03-23 15:29:05.952587 libresvip-1.1.3/libresvip/plugins/svp/options.py
+-rw-r--r--   0        0        0     9582 2024-03-04 16:48:05.013673 libresvip-1.1.3/libresvip/plugins/svp/param_expression.py
+-rw-r--r--   0        0        0     2901 2024-02-22 15:40:21.277240 libresvip-1.1.3/libresvip/plugins/svp/phoneme_categories.json
+-rw-r--r--   0        0        0    57860 2024-02-22 15:40:21.278256 libresvip-1.1.3/libresvip/plugins/svp/phoneme_dictionary.json
+-rw-r--r--   0        0        0     3281 2024-02-24 21:21:43.999921 libresvip-1.1.3/libresvip/plugins/svp/phoneme_utils.py
+-rw-r--r--   0        0        0     3651 2024-02-24 21:21:44.000940 libresvip-1.1.3/libresvip/plugins/svp/pitch_simulator.py
+-rw-r--r--   0        0        0      870 2024-02-22 15:40:21.279241 libresvip-1.1.3/libresvip/plugins/svp/pitch_slide.py
+-rw-r--r--   0        0        0    41585 2024-02-22 15:40:21.279241 libresvip-1.1.3/libresvip/plugins/svp/svp.yapsy-plugin
+-rw-r--r--   0        0        0    21945 2024-03-09 15:39:33.275988 libresvip-1.1.3/libresvip/plugins/svp/synthv_generator.py
+-rw-r--r--   0        0        0    29652 2024-05-19 06:30:29.934521 libresvip-1.1.3/libresvip/plugins/svp/synthv_parser.py
+-rw-r--r--   0        0        0     1182 2024-04-25 15:00:01.642567 libresvip-1.1.3/libresvip/plugins/svp/synthv_studio_converter.py
+-rw-r--r--   0        0        0     7049 2024-03-04 16:48:05.016732 libresvip-1.1.3/libresvip/plugins/svp/track_merge_utils.py
+-rw-r--r--   0        0        0        0 2024-04-20 08:41:44.970999 libresvip-1.1.3/libresvip/plugins/tlp/__init__.py
+-rw-r--r--   0        0        0     5364 2024-05-19 09:55:06.091687 libresvip-1.1.3/libresvip/plugins/tlp/model.py
+-rw-r--r--   0        0        0      325 2024-04-29 22:55:41.750988 libresvip-1.1.3/libresvip/plugins/tlp/options.py
+-rw-r--r--   0        0        0      253 2024-04-30 20:13:41.439220 libresvip-1.1.3/libresvip/plugins/tlp/tlp.yapsy-plugin
+-rw-r--r--   0        0        0     1016 2024-04-30 20:09:17.799740 libresvip-1.1.3/libresvip/plugins/tlp/tunelab_converter.py
+-rw-r--r--   0        0        0     5283 2024-05-19 10:00:22.688790 libresvip-1.1.3/libresvip/plugins/tlp/tunelab_generator.py
+-rw-r--r--   0        0        0     8532 2024-05-19 12:17:21.995853 libresvip-1.1.3/libresvip/plugins/tlp/tunelab_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.281548 libresvip-1.1.3/libresvip/plugins/tssln/__init__.py
+-rw-r--r--   0        0        0      258 2024-02-22 15:40:21.281548 libresvip-1.1.3/libresvip/plugins/tssln/constants.py
+-rw-r--r--   0        0        0    14287 2024-03-04 16:48:05.018348 libresvip-1.1.3/libresvip/plugins/tssln/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.954587 libresvip-1.1.3/libresvip/plugins/tssln/options.py
+-rw-r--r--   0        0        0    20418 2024-02-22 15:40:21.283497 libresvip-1.1.3/libresvip/plugins/tssln/tssln.yapsy-plugin
+-rw-r--r--   0        0        0     3829 2024-02-24 13:21:27.902046 libresvip-1.1.3/libresvip/plugins/tssln/value_tree.py
+-rw-r--r--   0        0        0     1032 2024-02-22 15:40:21.283497 libresvip-1.1.3/libresvip/plugins/tssln/voisona_converter.py
+-rw-r--r--   0        0        0     6553 2024-04-04 15:32:50.258857 libresvip-1.1.3/libresvip/plugins/tssln/voisona_generator.py
+-rw-r--r--   0        0        0     8686 2024-05-07 19:56:46.445386 libresvip-1.1.3/libresvip/plugins/tssln/voisona_parser.py
+-rw-r--r--   0        0        0    17668 2024-05-09 20:53:32.087863 libresvip-1.1.3/libresvip/plugins/tssln/voisona_pitch.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.284496 libresvip-1.1.3/libresvip/plugins/ufdata/__init__.py
+-rw-r--r--   0        0        0     1286 2024-04-04 15:32:50.261367 libresvip-1.1.3/libresvip/plugins/ufdata/model.py
+-rw-r--r--   0        0        0      125 2024-02-22 15:40:21.285497 libresvip-1.1.3/libresvip/plugins/ufdata/options.py
+-rw-r--r--   0        0        0    25204 2024-04-30 20:11:46.826346 libresvip-1.1.3/libresvip/plugins/ufdata/ufdata.yapsy-plugin
+-rw-r--r--   0        0        0     1005 2024-04-04 15:32:50.262370 libresvip-1.1.3/libresvip/plugins/ufdata/ufdata_converter.py
+-rw-r--r--   0        0        0     3019 2024-03-04 16:48:05.021992 libresvip-1.1.3/libresvip/plugins/ufdata/ufdata_generator.py
+-rw-r--r--   0        0        0     4414 2024-04-04 15:32:50.263369 libresvip-1.1.3/libresvip/plugins/ufdata/ufdata_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.287504 libresvip-1.1.3/libresvip/plugins/ust/__init__.py
+-rw-r--r--   0        0        0      220 2024-02-22 15:40:21.287504 libresvip-1.1.3/libresvip/plugins/ust/constants.py
+-rw-r--r--   0        0        0      859 2024-02-22 15:40:21.288508 libresvip-1.1.3/libresvip/plugins/ust/interpolation.py
+-rw-r--r--   0        0        0    17060 2024-03-11 13:13:40.358282 libresvip-1.1.3/libresvip/plugins/ust/model.py
+-rw-r--r--   0        0        0      614 2024-04-19 22:30:20.059096 libresvip-1.1.3/libresvip/plugins/ust/options.py
+-rw-r--r--   0        0        0     2060 2024-04-04 15:32:50.264367 libresvip-1.1.3/libresvip/plugins/ust/pitch_mode1.py
+-rw-r--r--   0        0        0     9626 2024-04-04 15:32:50.265367 libresvip-1.1.3/libresvip/plugins/ust/pitch_mode2.py
+-rw-r--r--   0        0        0     1781 2024-02-22 15:40:21.289493 libresvip-1.1.3/libresvip/plugins/ust/rdp_simplification.py
+-rw-r--r--   0        0        0     1076 2024-03-04 16:48:05.024002 libresvip-1.1.3/libresvip/plugins/ust/resampling.py
+-rw-r--r--   0        0        0     3600 2024-02-22 15:40:21.290497 libresvip-1.1.3/libresvip/plugins/ust/template.py
+-rw-r--r--   0        0        0     8187 2024-02-22 15:40:21.291513 libresvip-1.1.3/libresvip/plugins/ust/ust.yapsy-plugin
+-rw-r--r--   0        0        0      940 2024-04-19 22:31:18.927764 libresvip-1.1.3/libresvip/plugins/ust/ust_converter.py
+-rw-r--r--   0        0        0     4545 2024-03-11 21:42:10.409173 libresvip-1.1.3/libresvip/plugins/ust/ust_generator.py
+-rw-r--r--   0        0        0     6093 2024-03-23 15:29:05.958094 libresvip-1.1.3/libresvip/plugins/ust/ust_parser.py
+-rw-r--r--   0        0        0     3270 2024-04-05 21:58:38.955510 libresvip-1.1.3/libresvip/plugins/ust/vibrato_param.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.292072 libresvip-1.1.3/libresvip/plugins/ustx/__init__.py
+-rw-r--r--   0        0        0     6283 2024-03-04 16:48:05.024934 libresvip-1.1.3/libresvip/plugins/ustx/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.959093 libresvip-1.1.3/libresvip/plugins/ustx/options.py
+-rw-r--r--   0        0        0    45293 2024-02-22 15:40:21.294124 libresvip-1.1.3/libresvip/plugins/ustx/ustx.yapsy-plugin
+-rw-r--r--   0        0        0     1061 2024-03-12 19:57:09.206525 libresvip-1.1.3/libresvip/plugins/ustx/ustx_converter.py
+-rw-r--r--   0        0        0     8246 2024-04-04 23:03:45.113941 libresvip-1.1.3/libresvip/plugins/ustx/ustx_generator.py
+-rw-r--r--   0        0        0     7048 2024-03-23 15:29:05.960094 libresvip-1.1.3/libresvip/plugins/ustx/ustx_parser.py
+-rw-r--r--   0        0        0     4584 2024-03-11 13:13:40.361335 libresvip-1.1.3/libresvip/plugins/ustx/util.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.295117 libresvip-1.1.3/libresvip/plugins/ustx/utils/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-05 21:59:21.996830 libresvip-1.1.3/libresvip/plugins/ustx/utils/lyric_util.py
+-rw-r--r--   0        0        0      634 2024-02-24 21:21:44.007536 libresvip-1.1.3/libresvip/plugins/ustx/utils/music_math.py
+-rw-r--r--   0        0        0     6102 2024-02-22 15:40:21.296134 libresvip-1.1.3/libresvip/plugins/ustx/utils/time_axis.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.296134 libresvip-1.1.3/libresvip/plugins/vog/__init__.py
+-rw-r--r--   0        0        0      766 2024-02-22 15:40:21.297120 libresvip-1.1.3/libresvip/plugins/vog/model.py
+-rw-r--r--   0        0        0      359 2024-03-23 15:29:05.960094 libresvip-1.1.3/libresvip/plugins/vog/options.py
+-rw-r--r--   0        0        0    63065 2024-02-22 15:40:21.298121 libresvip-1.1.3/libresvip/plugins/vog/vog.yapsy-plugin
+-rw-r--r--   0        0        0     1347 2024-03-23 15:29:05.962094 libresvip-1.1.3/libresvip/plugins/vog/vogen_converter.py
+-rw-r--r--   0        0        0     1922 2024-03-18 14:02:32.510275 libresvip-1.1.3/libresvip/plugins/vog/vogen_generator.py
+-rw-r--r--   0        0        0     1658 2024-02-22 15:40:21.299208 libresvip-1.1.3/libresvip/plugins/vog/vogen_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.299208 libresvip-1.1.3/libresvip/plugins/vpr/__init__.py
+-rw-r--r--   0        0        0      434 2024-03-04 16:48:05.027944 libresvip-1.1.3/libresvip/plugins/vpr/constants.py
+-rw-r--r--   0        0        0     9840 2024-02-22 15:40:21.300231 libresvip-1.1.3/libresvip/plugins/vpr/model.py
+-rw-r--r--   0        0        0     1285 2024-03-23 15:29:05.962094 libresvip-1.1.3/libresvip/plugins/vpr/options.py
+-rw-r--r--   0        0        0     4847 2024-03-04 16:48:05.029005 libresvip-1.1.3/libresvip/plugins/vpr/vocaloid_pitch.py
+-rw-r--r--   0        0        0    14147 2024-02-22 15:40:21.300231 libresvip-1.1.3/libresvip/plugins/vpr/vpr.yapsy-plugin
+-rw-r--r--   0        0        0     1515 2024-04-04 15:32:50.266367 libresvip-1.1.3/libresvip/plugins/vpr/vpr_converter.py
+-rw-r--r--   0        0        0    10082 2024-04-04 15:32:50.267366 libresvip-1.1.3/libresvip/plugins/vpr/vpr_generator.py
+-rw-r--r--   0        0        0     6440 2024-03-23 15:29:05.963094 libresvip-1.1.3/libresvip/plugins/vpr/vpr_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.302894 libresvip-1.1.3/libresvip/plugins/vshp/__init__.py
+-rw-r--r--   0        0        0     5774 2024-02-22 15:40:21.303892 libresvip-1.1.3/libresvip/plugins/vshp/model.py
+-rw-r--r--   0        0        0      532 2024-02-22 15:40:21.303892 libresvip-1.1.3/libresvip/plugins/vshp/options.py
+-rw-r--r--   0        0        0      351 2024-02-22 15:40:21.304891 libresvip-1.1.3/libresvip/plugins/vshp/utils.py
+-rw-r--r--   0        0        0      522 2024-02-22 15:40:21.304891 libresvip-1.1.3/libresvip/plugins/vshp/vocalshifter_converter.py
+-rw-r--r--   0        0        0     9770 2024-05-12 02:56:26.310999 libresvip-1.1.3/libresvip/plugins/vshp/vocalshifter_parser.py
+-rw-r--r--   0        0        0     9560 2024-03-05 19:32:37.534334 libresvip-1.1.3/libresvip/plugins/vshp/vshp.yapsy-plugin
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.305892 libresvip-1.1.3/libresvip/plugins/vspx/__init__.py
+-rw-r--r--   0        0        0    12444 2024-05-07 19:08:16.999960 libresvip-1.1.3/libresvip/plugins/vspx/model.py
+-rw-r--r--   0        0        0      325 2024-03-23 15:29:05.965117 libresvip-1.1.3/libresvip/plugins/vspx/options.py
+-rw-r--r--   0        0        0     2859 2024-04-03 23:14:53.054645 libresvip-1.1.3/libresvip/plugins/vspx/vocalsharp_converter.py
+-rw-r--r--   0        0        0     5428 2024-02-22 15:40:21.307892 libresvip-1.1.3/libresvip/plugins/vspx/vspx.yapsy-plugin
+-rw-r--r--   0        0        0     7072 2024-02-24 21:21:44.010521 libresvip-1.1.3/libresvip/plugins/vspx/vspx_generator.py
+-rw-r--r--   0        0        0     8035 2024-03-04 16:48:05.031947 libresvip-1.1.3/libresvip/plugins/vspx/vspx_interval_dict.py
+-rw-r--r--   0        0        0     5857 2024-03-23 15:29:05.966101 libresvip-1.1.3/libresvip/plugins/vspx/vspx_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.308892 libresvip-1.1.3/libresvip/plugins/vsq/__init__.py
+-rw-r--r--   0        0        0      246 2024-03-04 16:48:05.031947 libresvip-1.1.3/libresvip/plugins/vsq/constants.py
+-rw-r--r--   0        0        0     1257 2024-03-23 15:29:05.966101 libresvip-1.1.3/libresvip/plugins/vsq/options.py
+-rw-r--r--   0        0        0     5055 2024-03-04 16:48:05.032934 libresvip-1.1.3/libresvip/plugins/vsq/vocaloid_pitch.py
+-rw-r--r--   0        0        0    49554 2024-02-22 15:40:21.310892 libresvip-1.1.3/libresvip/plugins/vsq/vsq.yapsy-plugin
+-rw-r--r--   0        0        0      957 2024-02-22 15:40:21.310892 libresvip-1.1.3/libresvip/plugins/vsq/vsq_converter.py
+-rw-r--r--   0        0        0     8510 2024-03-04 16:48:05.033991 libresvip-1.1.3/libresvip/plugins/vsq/vsq_generator.py
+-rw-r--r--   0        0        0     8932 2024-05-13 23:51:28.744089 libresvip-1.1.3/libresvip/plugins/vsq/vsq_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.310892 libresvip-1.1.3/libresvip/plugins/vsqx/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-04 16:48:05.034998 libresvip-1.1.3/libresvip/plugins/vsqx/constants.py
+-rw-r--r--   0        0        0      566 2024-03-23 15:29:05.968632 libresvip-1.1.3/libresvip/plugins/vsqx/enums.py
+-rw-r--r--   0        0        0     4400 2024-02-22 15:40:21.312399 libresvip-1.1.3/libresvip/plugins/vsqx/model.py
+-rw-r--r--   0        0        0        2 2024-02-22 15:40:21.312399 libresvip-1.1.3/libresvip/plugins/vsqx/models/__init__.py
+-rw-r--r--   0        0        0    36025 2024-02-22 15:40:21.313408 libresvip-1.1.3/libresvip/plugins/vsqx/models/vsqx3.py
+-rw-r--r--   0        0        0    32059 2024-02-22 15:40:21.313408 libresvip-1.1.3/libresvip/plugins/vsqx/models/vsqx4.py
+-rw-r--r--   0        0        0     1078 2024-03-23 15:29:05.969611 libresvip-1.1.3/libresvip/plugins/vsqx/options.py
+-rw-r--r--   0        0        0     6353 2024-05-12 21:40:04.381986 libresvip-1.1.3/libresvip/plugins/vsqx/vocaloid_pitch.py
+-rw-r--r--   0        0        0    10117 2024-04-04 15:32:50.268367 libresvip-1.1.3/libresvip/plugins/vsqx/vsq3_generator.py
+-rw-r--r--   0        0        0    10118 2024-04-04 15:32:50.269366 libresvip-1.1.3/libresvip/plugins/vsqx/vsq4_generator.py
+-rw-r--r--   0        0        0    49665 2024-02-22 15:40:21.315408 libresvip-1.1.3/libresvip/plugins/vsqx/vsqx.yapsy-plugin
+-rw-r--r--   0        0        0     3216 2024-04-03 23:14:53.055643 libresvip-1.1.3/libresvip/plugins/vsqx/vsqx_converter.py
+-rw-r--r--   0        0        0    13947 2024-05-12 21:44:45.964936 libresvip-1.1.3/libresvip/plugins/vsqx/vsqx_parser.py
+-rw-r--r--   0        0        0        0 2024-02-22 15:40:21.316410 libresvip-1.1.3/libresvip/plugins/y77/__init__.py
+-rw-r--r--   0        0        0      742 2024-02-22 15:40:21.316410 libresvip-1.1.3/libresvip/plugins/y77/model.py
+-rw-r--r--   0        0        0      321 2024-03-23 15:29:05.971609 libresvip-1.1.3/libresvip/plugins/y77/options.py
+-rw-r--r--   0        0        0    48980 2024-02-22 15:40:21.317409 libresvip-1.1.3/libresvip/plugins/y77/y77.yapsy-plugin
+-rw-r--r--   0        0        0     1042 2024-04-04 15:32:50.270964 libresvip-1.1.3/libresvip/plugins/y77/y77_converter.py
+-rw-r--r--   0        0        0     3963 2024-03-18 14:02:43.305455 libresvip-1.1.3/libresvip/plugins/y77/y77_generator.py
+-rw-r--r--   0        0        0     3190 2024-03-23 15:29:05.973610 libresvip-1.1.3/libresvip/plugins/y77/y77_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:40:49.030321 libresvip-1.1.3/libresvip/py.typed
+-rw-r--r--   0        0        0   270398 2024-02-22 15:40:21.319450 libresvip-1.1.3/libresvip/res/libresvip.ico
+-rw-r--r--   0        0        0    54799 2024-05-19 09:30:40.522879 libresvip-1.1.3/libresvip/res/locales/zh_CN/LC_MESSAGES/libresvip.mo
+-rw-r--r--   0        0        0        0 2024-02-24 21:21:44.013149 libresvip-1.1.3/libresvip/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-04-04 15:32:50.277874 libresvip-1.1.3/libresvip/utils/audio.py
+-rw-r--r--   0        0        0     2441 2024-03-04 16:48:05.048671 libresvip-1.1.3/libresvip/utils/module_loading.py
+-rw-r--r--   0        0        0     3970 2024-03-04 16:48:05.049643 libresvip-1.1.3/libresvip/utils/music_math.py
+-rw-r--r--   0        0        0     1129 2024-02-24 21:21:44.014264 libresvip-1.1.3/libresvip/utils/search.py
+-rw-r--r--   0        0        0     3309 2024-05-19 06:30:15.423045 libresvip-1.1.3/libresvip/utils/text.py
+-rw-r--r--   0        0        0     1627 2024-04-17 18:48:56.821252 libresvip-1.1.3/libresvip/utils/translation.py
+-rw-r--r--   0        0        0     1015 2024-04-03 23:14:53.055643 libresvip-1.1.3/libresvip/utils/xmlutils/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-19 21:54:15.974691 libresvip-1.1.3/libresvip/utils/xmlutils/native.py
+-rw-r--r--   0        0        0      942 2024-03-12 20:28:45.735172 libresvip-1.1.3/libresvip/utils/yamlutils/__init__.py
+-rw-r--r--   0        0        0     2833 2024-03-24 06:01:39.945387 libresvip-1.1.3/libresvip/utils/yamlutils/common.py
+-rw-r--r--   0        0        0     3873 2024-03-24 06:01:51.194427 libresvip-1.1.3/libresvip/utils/yamlutils/dumper.py
+-rw-r--r--   0        0        0     5052 2024-03-04 16:48:05.053289 libresvip-1.1.3/libresvip/utils/yamlutils/loader.py
+-rw-r--r--   0        0        0      152 2024-04-17 14:03:30.170610 libresvip-1.1.3/libresvip/web/__init__.py
+-rw-r--r--   0        0        0       97 2024-03-01 21:51:25.393182 libresvip-1.1.3/libresvip/web/__main__.py
+-rw-r--r--   0        0        0     2344 2024-03-01 21:51:25.394220 libresvip-1.1.3/libresvip/web/elements.py
+-rw-r--r--   0        0        0    96719 2024-04-28 04:40:58.986463 libresvip-1.1.3/libresvip/web/pages.py
+-rw-r--r--   0        0        0     5415 2024-05-19 13:03:35.055055 libresvip-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5999 1970-01-01 00:00:00.000000 libresvip-1.1.3/PKG-INFO
```

### Comparing `libresvip-1.1.2/LICENSE` & `libresvip-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/README.md` & `libresvip-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/cli/commands/conf.py` & `libresvip-1.1.3/libresvip/cli/commands/conf.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/cli/commands/plugin.py` & `libresvip-1.1.3/libresvip/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/cli/commands/proj.py` & `libresvip-1.1.3/libresvip/cli/commands/proj.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/cli/prompt.py` & `libresvip-1.1.3/libresvip/cli/prompt.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/compat.py` & `libresvip-1.1.3/libresvip/core/compat.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/config.py` & `libresvip-1.1.3/libresvip/core/config.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/constants.py` & `libresvip-1.1.3/libresvip/core/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/lyric_phoneme/chinese/__init__.py` & `libresvip-1.1.3/libresvip/core/lyric_phoneme/chinese/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/lyric_phoneme/chinese/vocaloid_xsampa.py` & `libresvip-1.1.3/libresvip/core/lyric_phoneme/chinese/vocaloid_xsampa.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/lyric_phoneme/japanese/vocaloid_xsampa.py` & `libresvip-1.1.3/libresvip/core/lyric_phoneme/japanese/vocaloid_xsampa.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/tick_counter.py` & `libresvip-1.1.3/libresvip/core/tick_counter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/time_interval.py` & `libresvip-1.1.3/libresvip/core/time_interval.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/time_sync.py` & `libresvip-1.1.3/libresvip/core/time_sync.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/core/warning_types.py` & `libresvip-1.1.3/libresvip/core/warning_types.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/extension/base.py` & `libresvip-1.1.3/libresvip/extension/base.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/extension/manager.py` & `libresvip-1.1.3/libresvip/extension/manager.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/extension/meta_info.py` & `libresvip-1.1.3/libresvip/extension/meta_info.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/__init__.py` & `libresvip-1.1.3/libresvip/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/__main__.py` & `libresvip-1.1.3/libresvip/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/models/list_models.py` & `libresvip-1.1.3/libresvip/gui/models/list_models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/models/table_models.py` & `libresvip-1.1.3/libresvip/gui/models/table_models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/__init__.py` & `libresvip-1.1.3/libresvip/gui/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/application.py` & `libresvip-1.1.3/libresvip/gui/modules/application.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/clipboard.py` & `libresvip-1.1.3/libresvip/gui/modules/clipboard.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/config_items.py` & `libresvip-1.1.3/libresvip/gui/modules/config_items.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/font_loader.py` & `libresvip-1.1.3/libresvip/gui/modules/font_loader.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/frameless_window.py` & `libresvip-1.1.3/libresvip/gui/modules/frameless_window.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/frameless_window_win32.py` & `libresvip-1.1.3/libresvip/gui/modules/frameless_window_win32.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/locale_switcher.py` & `libresvip-1.1.3/libresvip/gui/modules/locale_switcher.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/notifier.py` & `libresvip-1.1.3/libresvip/gui/modules/notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                             elif uname.system == "Darwin":
                                 asset = next(
                                     (
                                         asset
                                         for asset in data["assets"]
                                         if fnmatch.fnmatch(
                                             asset["name"],
-                                            "LibreSVIP-*.macos-*",
+                                            f"LibreSVIP-*.macos-{arch}.dmg",
                                         )
                                     ),
                                     None,
                                 )
                             if asset:
                                 buttons.append(
                                     Button(
```

### Comparing `libresvip-1.1.2/libresvip/gui/modules/task_manager.py` & `libresvip-1.1.3/libresvip/gui/modules/task_manager.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/vendor/qasync/__init__.py` & `libresvip-1.1.3/libresvip/gui/modules/vendor/qasync/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/vendor/qasync/_unix.py` & `libresvip-1.1.3/libresvip/gui/modules/vendor/qasync/_unix.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/vendor/qasync/_windows.py` & `libresvip-1.1.3/libresvip/gui/modules/vendor/qasync/_windows.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/gui/modules/win32_constants.py` & `libresvip-1.1.3/libresvip/gui/modules/win32_constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/middlewares/pitch_shift/pitch_shift.py` & `libresvip-1.1.3/libresvip/middlewares/pitch_shift/pitch_shift.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/middlewares/project_zoom/options.py` & `libresvip-1.1.3/libresvip/middlewares/project_zoom/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/middlewares/pronounciation_conversion/options.py` & `libresvip-1.1.3/libresvip/middlewares/pronounciation_conversion/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.py` & `libresvip-1.1.3/libresvip/middlewares/pronounciation_conversion/pronounciation_conversion.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/middlewares/remove_short_silences/options.py` & `libresvip-1.1.3/libresvip/middlewares/remove_short_silences/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/middlewares/remove_short_silences/remove_short_silences.py` & `libresvip-1.1.3/libresvip/middlewares/remove_short_silences/remove_short_silences.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/middlewares/replace_lyric/replace_lyric.py` & `libresvip-1.1.3/libresvip/middlewares/replace_lyric/replace_lyric.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/model/base.py` & `libresvip-1.1.3/libresvip/model/base.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/model/option_mixins.py` & `libresvip-1.1.3/libresvip/model/option_mixins.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/model/point.py` & `libresvip-1.1.3/libresvip/model/point.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/model/relative_pitch_curve.py` & `libresvip-1.1.3/libresvip/model/relative_pitch_curve.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/model/reset_time_axis.py` & `libresvip-1.1.3/libresvip/model/reset_time_axis.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/ace-studio.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/acep/ace-studio.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/ace_curve_utils.py` & `libresvip-1.1.3/libresvip/plugins/acep/ace_curve_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/ace_studio_converter.py` & `libresvip-1.1.3/libresvip/plugins/acep/ace_studio_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/ace_studio_generator.py` & `libresvip-1.1.3/libresvip/plugins/acep/ace_studio_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,26 +142,27 @@
                 def generate_vocal_pattern() -> None:
                     self.pattern_start = round(
                         max(
                             0,
                             buffer[0].start_pos - 240,
                         )
                     )
+                    self.ace_note_list = []
+                    for note in buffer:
+                        if note.lyric:
+                            self.generate_note(note)
                     vocal_pattern = AcepVocalPattern(
                         pos=self.pattern_start,
                         dur=round(buffer[-1].end_pos) - self.pattern_start,
-                    )
-                    vocal_pattern.notes.extend(
-                        self.generate_note(note) for note in buffer if note.lyric
+                        notes=self.ace_note_list,
                     )
                     vocal_pattern.clip_dur = vocal_pattern.dur
                     buffer.clear()
                     if self.options.breath > 0:
                         self.adjust_breath_tags(vocal_pattern.notes)
-                    self.ace_note_list = vocal_pattern.notes
                     vocal_pattern.parameters = self.generate_params(track.edited_params)
                     ace_vocal_track.patterns.append(vocal_pattern)
 
                 for prev_note, cur_note in zip(track.note_list[:-1], track.note_list[1:]):
                     prev_end = prev_note.end_pos
                     cur_start = cur_note.start_pos
                     if cur_start - prev_end > self.options.split_threshold * TICKS_IN_BEAT > 0:
@@ -206,15 +207,15 @@
                 continue
             actual_breath = min((notes[i].pos - notes[i - 1].pos) // 2, breath)
             notes[i - 1].dur = min(
                 notes[i - 1].dur, notes[i].pos - notes[i - 1].pos - actual_breath
             )
             notes[i].br_len -= actual_breath
 
-    def generate_note(self, note: Note, pinyin: Optional[str] = None) -> AcepNote:
+    def generate_note(self, note: Note, pinyin: Optional[str] = None) -> None:
         if self.options.lyric_language == AcepLyricsLanguage.CHINESE and not pinyin:
             pinyin = next(iter(get_pinyin_series(note.lyric)), None)
         ace_note = AcepNote(
             pos=round(note.start_pos) - self.pattern_start,
             pitch=note.key_number,
             lyric=note.lyric,
             language=self.options.lyric_language,
@@ -230,24 +231,33 @@
                     tick_to_second(note.start_pos, self.ace_tempo_list)
                     - note.edited_phones.head_length_in_secs
                 )
                 phone_start_in_ticks = second_to_tick(phone_start_in_secs, self.ace_tempo_list)
                 ace_note.head_consonants = [round(note.start_pos - phone_start_in_ticks)]
             elif self.options.default_consonant_length:
                 ace_note.head_consonants = [self.options.default_consonant_length]
+        elif self.options.lyric_language == AcepLyricsLanguage.ENGLISH and self.ace_note_list:
+            ace_note.pronunciation = "-"
+            last_ace_note = self.ace_note_list[-1]
+            lyric, sep, index = last_ace_note.lyric.partition("#")
+            if sep == "#" and index.isdigit():
+                ace_note.lyric = f"{lyric}#{int(index) + 1}"
+            else:
+                last_ace_note.lyric = f"{lyric}#1"
+                ace_note.lyric = f"{lyric}#2"
         else:
             ace_note.lyric = ace_note.pronunciation = "-"
 
         if note.head_tag == "V" and self.options.breath > 0:
             breath_start_in_secs = (
                 tick_to_second(note.start_pos, self.ace_tempo_list) - self.options.breath / 1000
             )
             breath_start_in_ticks = second_to_tick(breath_start_in_secs, self.ace_tempo_list)
             ace_note.br_len = round(note.start_pos - breath_start_in_ticks)
-        return ace_note
+        self.ace_note_list.append(ace_note)
 
     @staticmethod
     def linear_transform(
         lower_bound: float, middle_value: float, upper_bound: float
     ) -> Callable[[float], float]:
         def transform(x: float) -> float:
             if x >= 0:
```

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/ace_studio_parser.py` & `libresvip-1.1.3/libresvip/plugins/acep/ace_studio_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/acep_io.py` & `libresvip-1.1.3/libresvip/plugins/acep/acep_io.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/base_pitch_curve.py` & `libresvip-1.1.3/libresvip/plugins/acep/base_pitch_curve.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/curve_segment_utils.py` & `libresvip-1.1.3/libresvip/plugins/acep/curve_segment_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/model.py` & `libresvip-1.1.3/libresvip/plugins/acep/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/options.py` & `libresvip-1.1.3/libresvip/plugins/acep/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/singers.py` & `libresvip-1.1.3/libresvip/plugins/acep/singers.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/acep/time_utils.py` & `libresvip-1.1.3/libresvip/plugins/acep/time_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/aisp/aisingers_converter.py` & `libresvip-1.1.3/libresvip/plugins/aisp/aisingers_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/aisp/aisingers_generator.py` & `libresvip-1.1.3/libresvip/plugins/aisp/aisingers_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/aisp/aisingers_parser.py` & `libresvip-1.1.3/libresvip/plugins/aisp/aisingers_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/aisp/aisp.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/aisp/aisp.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/aisp/model.py` & `libresvip-1.1.3/libresvip/plugins/aisp/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ccs/ccs.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/ccs/ccs.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ccs/cevio_converter.py` & `libresvip-1.1.3/libresvip/plugins/ccs/cevio_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ccs/cevio_generator.py` & `libresvip-1.1.3/libresvip/plugins/ccs/cevio_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ccs/cevio_parser.py` & `libresvip-1.1.3/libresvip/plugins/ccs/cevio_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ccs/cevio_pitch.py` & `libresvip-1.1.3/libresvip/plugins/ccs/cevio_pitch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 import dataclasses
+import functools
 import itertools
 import math
-from typing import NamedTuple, Optional
+from typing import NamedTuple, Optional, cast
 
 import more_itertools
+import portion
 
 from libresvip.core.tick_counter import shift_tempo_list
+from libresvip.core.time_interval import PiecewiseIntervalDict
+from libresvip.core.time_sync import TimeSynchronizer
 from libresvip.core.warning_types import show_warning
 from libresvip.model.base import ParamCurve, Points, SongTempo
 from libresvip.model.point import Point
 from libresvip.utils.music_math import hz2midi, midi2hz
 from libresvip.utils.search import find_last_index
 from libresvip.utils.translation import gettext_lazy as _
 
@@ -59,29 +63,46 @@
         return length + MIN_DATA_LENGTH
 
 
 def pitch_from_cevio_track(data: CeVIOTrackPitchData) -> Optional[ParamCurve]:
     converted_points = [Point.start_point()]
     current_value = -100
 
+    synchronizer = TimeSynchronizer(data.tempos)
+    vibrato_amplitude_interval_dict = build_cevio_param_interval_dict(
+        data.vibrato_amplitude_events, synchronizer, data.tick_prefix
+    )
+    vibrato_value_interval_dict = build_cevio_wave_interval_dict(
+        data.vibrato_frequency_events, synchronizer, data.tick_prefix
+    )
+
     events_normalized = shape_events(
         normalize_to_tick(append_ending_points(data.events), data.tempos, data.tick_prefix)
     )
 
     next_pos = None
     for event in events_normalized:
-        pos = event.idx - data.tick_prefix
+        pos = int(cast(float, event.idx)) - data.tick_prefix
+        secs = synchronizer.get_actual_secs_from_ticks(pos)
         length = event.repeat
         try:
             value = round(hz2midi(math.e**event.value) * 100) if event.value is not None else -100
             if value != current_value or next_pos != pos:
                 converted_points.append(Point(x=round(pos), y=value))
                 if value == -100:
                     converted_points.append(Point(x=round(pos), y=value))
                 current_value = value
+            secs_step = synchronizer.get_duration_secs_from_ticks(pos, pos + 5)
+            for pos_x in range(pos, int(cast(float, pos + length)), 5):
+                if value_diff := vibrato_value_interval_dict.get(secs):
+                    value_diff *= vibrato_amplitude_interval_dict.get(secs, 1)
+                    converted_points.append(Point(x=pos_x, y=round(value + value_diff)))
+                else:
+                    break
+                secs += secs_step
         except OverflowError:
             show_warning(_("Pitch value is out of bounds"))
         next_pos = pos + length
     converted_points.append(Point.end_point())
 
     return ParamCurve(points=Points(root=converted_points)) if len(converted_points) > 2 else None
 
@@ -181,14 +202,101 @@
             last_pos, last_tick_pos, last_bpm = result[-1]
             ticks_in_time_unit = TIME_UNIT_AS_TICKS_PER_BPM * last_bpm
             new_pos = last_pos + (tempo.position - last_tick_pos) / ticks_in_time_unit
             result.append((int(new_pos), tempo.position, tempo.bpm))
     return result
 
 
+def vibrato_curve(value: float, shift: float, omega: float, phase: float) -> float:
+    return math.sin(omega * (value - shift) + phase)
+
+
+def build_cevio_param_interval_dict(
+    events: list[CeVIOParamEvent], synchronizer: TimeSynchronizer, tick_prefix: int
+) -> PiecewiseIntervalDict:
+    param_interval_dict = PiecewiseIntervalDict()
+    for continuous_part in more_itertools.split_before(
+        events,
+        lambda event: event.idx is not None,
+    ):
+        for prev_event, next_event in more_itertools.windowed(
+            more_itertools.prepend(
+                None,
+                normalize_to_tick(
+                    append_ending_points(continuous_part), synchronizer.tempo_list, tick_prefix
+                ),
+            ),
+            2,
+        ):
+            next_start = synchronizer.get_actual_secs_from_ticks(next_event.idx - tick_prefix)
+            if (
+                prev_event is not None
+                and (
+                    prev_end := synchronizer.get_actual_secs_from_ticks(
+                        prev_event.idx + (prev_event.repeat or 1) - tick_prefix
+                    )
+                )
+                and prev_end < next_start
+            ):
+                param_interval_dict[portion.closedopen(prev_end, next_start)] = next_event.value
+            param_interval_dict[
+                portion.closedopen(
+                    next_start,
+                    synchronizer.get_actual_secs_from_ticks(
+                        next_event.idx + (next_event.repeat or 1) - tick_prefix
+                    ),
+                )
+            ] = next_event.value
+    return param_interval_dict
+
+
+def build_cevio_wave_interval_dict(
+    events: list[CeVIOParamEvent], synchronizer: TimeSynchronizer, tick_prefix: int
+) -> PiecewiseIntervalDict:
+    param_interval_dict = PiecewiseIntervalDict()
+    omega = math.tau * 6
+    for continuous_part in more_itertools.split_before(
+        events,
+        lambda event: event.idx is not None,
+    ):
+        phase = 0.0
+        for prev_event, next_event in more_itertools.windowed(
+            more_itertools.prepend(
+                None,
+                normalize_to_tick(
+                    append_ending_points(continuous_part), synchronizer.tempo_list, tick_prefix
+                ),
+            ),
+            2,
+        ):
+            next_start = synchronizer.get_actual_secs_from_ticks(next_event.idx - tick_prefix)
+            next_end = synchronizer.get_actual_secs_from_ticks(
+                next_event.idx + (next_event.repeat or 1) - tick_prefix
+            )
+            if (
+                prev_event is not None
+                and (
+                    prev_end := synchronizer.get_actual_secs_from_ticks(
+                        prev_event.idx + (prev_event.repeat or 1) - tick_prefix
+                    )
+                )
+                and prev_end < next_start
+            ):
+                prev_start = synchronizer.get_actual_secs_from_ticks(prev_event.idx - tick_prefix)
+                param_interval_dict[portion.closedopen(prev_end, next_start)] = vibrato_curve(
+                    prev_end, prev_start, omega, phase
+                )
+            omega = math.tau * (next_event.value or 6)
+            param_interval_dict[portion.closedopen(next_start, next_end)] = functools.partial(
+                vibrato_curve, shift=next_start, omega=omega, phase=phase
+            )
+            phase += (next_end - next_start) * omega
+    return param_interval_dict
+
+
 def generate_for_cevio(
     pitch: ParamCurve, tempos: list[SongTempo], tick_prefix: int
 ) -> Optional[CeVIOTrackPitchData]:
     events_with_full_params = []
     for i, this_point in enumerate(pitch.points.root):
         next_point = pitch.points[i + 1] if i + 1 < len(pitch.points) else None
         end_tick = next_point.x - tick_prefix if next_point else None
@@ -320,8 +428,8 @@
                 new_events.append(event._replace(idx=None))
             else:
                 new_events.append(event)
     return new_events
 
 
 def remove_redundant_repeat(events: list[CeVIOParamEvent]) -> list[CeVIOParamEvent]:
-    return [event if event.repeat != 1 else event._replace(repeat=None) for event in events]
+    return [event if event.repeat > 1 else event._replace(repeat=None) for event in events]
```

### Comparing `libresvip-1.1.2/libresvip/plugins/ccs/model.py` & `libresvip-1.1.3/libresvip/plugins/ccs/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -801,16 +801,16 @@
     data: list[Union[CeVIOData, float, Decimal, int]] = field(
         default_factory=list,
         metadata={
             "name": "Data",
             "type": "Element",
         },
     )
-    no_data: Optional[list[CeVIONoData]] = field(
-        default=None,
+    no_data: list[CeVIONoData] = field(
+        default_factory=list,
         metadata={
             "name": "NoData",
             "type": "Element",
         },
     )
```

### Comparing `libresvip-1.1.2/libresvip/plugins/ccs/options.py` & `libresvip-1.1.3/libresvip/plugins/ccs/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/dicts/opencpop-extension.txt` & `libresvip-1.1.3/libresvip/plugins/ds/dicts/opencpop-extension.txt`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/dicts/opencpop-strict.txt` & `libresvip-1.1.3/libresvip/plugins/ds/dicts/opencpop-strict.txt`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/dicts/opencpop.txt` & `libresvip-1.1.3/libresvip/plugins/ds/dicts/opencpop.txt`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/diffsinger_converter.py` & `libresvip-1.1.3/libresvip/plugins/ds/diffsinger_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/diffsinger_generator.py` & `libresvip-1.1.3/libresvip/plugins/ds/diffsinger_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/diffsinger_parser.py` & `libresvip-1.1.3/libresvip/plugins/ds/diffsinger_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/ds.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/ds/ds.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/model.py` & `libresvip-1.1.3/libresvip/plugins/ds/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/models/ds_note.py` & `libresvip-1.1.3/libresvip/plugins/ds/models/ds_note.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/models/ds_project.py` & `libresvip-1.1.3/libresvip/plugins/ds/models/ds_project.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/options.py` & `libresvip-1.1.3/libresvip/plugins/ds/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/phoneme_dict.py` & `libresvip-1.1.3/libresvip/plugins/ds/phoneme_dict.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/utils/gender_param_utils.py` & `libresvip-1.1.3/libresvip/plugins/ds/utils/gender_param_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/utils/note_list_util.py` & `libresvip-1.1.3/libresvip/plugins/ds/utils/note_list_util.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/utils/pinyin_util.py` & `libresvip-1.1.3/libresvip/plugins/ds/utils/pinyin_util.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/utils/pitch_param_utils.py` & `libresvip-1.1.3/libresvip/plugins/ds/utils/pitch_param_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ds/utils/project_util.py` & `libresvip-1.1.3/libresvip/plugins/ds/utils/project_util.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/dv/constants.py` & `libresvip-1.1.3/libresvip/plugins/dv/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/dv/deepvocal_converter.py` & `libresvip-1.1.3/libresvip/plugins/dv/deepvocal_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/dv/deepvocal_pitch.py` & `libresvip-1.1.3/libresvip/plugins/dv/deepvocal_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/dv/dv.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/dv/dv.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/dv/dv_generator.py` & `libresvip-1.1.3/libresvip/plugins/dv/dv_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/dv/dv_parser.py` & `libresvip-1.1.3/libresvip/plugins/dv/dv_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/dv/model.py` & `libresvip-1.1.3/libresvip/plugins/dv/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/gj/constants.py` & `libresvip-1.1.3/libresvip/plugins/gj/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/gj/gjgj.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/gj/gjgj.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/gj/gjgj_converter.py` & `libresvip-1.1.3/libresvip/plugins/gj/gjgj_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/gj/gjgj_generator.py` & `libresvip-1.1.3/libresvip/plugins/gj/gjgj_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/gj/gjgj_parser.py` & `libresvip-1.1.3/libresvip/plugins/gj/gjgj_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/gj/model.py` & `libresvip-1.1.3/libresvip/plugins/gj/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/gj/options.py` & `libresvip-1.1.3/libresvip/plugins/gj/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/json/jsonsvip.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/json/jsonsvip.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/json/jsonsvip_converter.py` & `libresvip-1.1.3/libresvip/plugins/json/jsonsvip_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/lrc/lrc.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/lrc/lrc.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/lrc/lrc_generator.py` & `libresvip-1.1.3/libresvip/plugins/lrc/lrc_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/lrc/model.py` & `libresvip-1.1.3/libresvip/plugins/lrc/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/lrc/options.py` & `libresvip-1.1.3/libresvip/plugins/lrc/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/lrc/template.py` & `libresvip-1.1.3/libresvip/plugins/lrc/template.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mid/constants.py` & `libresvip-1.1.3/libresvip/plugins/mid/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mid/mid.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/mid/mid.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mid/midi_converter.py` & `libresvip-1.1.3/libresvip/plugins/mid/midi_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mid/midi_generator.py` & `libresvip-1.1.3/libresvip/plugins/mid/midi_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mid/midi_parser.py` & `libresvip-1.1.3/libresvip/plugins/mid/midi_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mid/midi_pitch.py` & `libresvip-1.1.3/libresvip/plugins/mid/midi_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mid/options.py` & `libresvip-1.1.3/libresvip/plugins/mid/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mtp/model.py` & `libresvip-1.1.3/libresvip/plugins/mtp/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mtp/mtp.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/mtp/mtp.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mtp/muta_converter.py` & `libresvip-1.1.3/libresvip/plugins/mtp/muta_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mtp/muta_generator.py` & `libresvip-1.1.3/libresvip/plugins/mtp/muta_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/mtp/muta_parser.py` & `libresvip-1.1.3/libresvip/plugins/mtp/muta_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/musicxml/model.py` & `libresvip-1.1.3/libresvip/plugins/musicxml/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/musicxml/models/mxml2.py` & `libresvip-1.1.3/libresvip/plugins/musicxml/models/mxml2.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/musicxml/models/xlink.py` & `libresvip-1.1.3/libresvip/plugins/musicxml/models/xlink.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/musicxml/musicxml.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/musicxml/musicxml.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/musicxml/musicxml_converter.py` & `libresvip-1.1.3/libresvip/plugins/musicxml/musicxml_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/musicxml/musicxml_generator.py` & `libresvip-1.1.3/libresvip/plugins/musicxml/musicxml_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/musicxml/musicxml_parser.py` & `libresvip-1.1.3/libresvip/plugins/musicxml/musicxml_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/nn/model.py` & `libresvip-1.1.3/libresvip/plugins/nn/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/nn/niaoniao_converter.py` & `libresvip-1.1.3/libresvip/plugins/nn/niaoniao_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/nn/niaoniao_generator.py` & `libresvip-1.1.3/libresvip/plugins/nn/niaoniao_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/nn/niaoniao_parser.py` & `libresvip-1.1.3/libresvip/plugins/nn/niaoniao_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/nn/nn.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/nn/nn.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/nn/template.py` & `libresvip-1.1.3/libresvip/plugins/nn/template.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ppsf/legacy_model.py` & `libresvip-1.1.3/libresvip/plugins/ppsf/legacy_model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ppsf/model.py` & `libresvip-1.1.3/libresvip/plugins/ppsf/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ppsf/piapro_studio_converter.py` & `libresvip-1.1.3/libresvip/plugins/ppsf/piapro_studio_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ppsf/piapro_studio_generator.py` & `libresvip-1.1.3/libresvip/plugins/ppsf/piapro_studio_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ppsf/piapro_studio_legacy_parser.py` & `libresvip-1.1.3/libresvip/plugins/ppsf/piapro_studio_legacy_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ppsf/piapro_studio_nt_parser.py` & `libresvip-1.1.3/libresvip/plugins/ppsf/piapro_studio_nt_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ppsf/ppsf.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/ppsf/ppsf.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ppsf/ppsf_interval_dict.py` & `libresvip-1.1.3/libresvip/plugins/ppsf/ppsf_interval_dict.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/s5p/model.py` & `libresvip-1.1.3/libresvip/plugins/s5p/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,19 +126,19 @@
     )
     def serialize_points(self, points: S5pPoints, _info: FieldSerializationInfo) -> list[float]:
         return list(chain.from_iterable(points.root))
 
 
 class S5pTrack(BaseModel):
     name: str
-    db_name: str = Field(..., alias="dbName")
+    db_name: str = Field("", alias="dbName")
     color: str = "15e879"
-    display_order: int = Field(..., alias="displayOrder")
+    display_order: int = Field(0, alias="displayOrder")
     db_defaults: S5pDbDefaults = Field(default_factory=S5pDbDefaults, alias="dbDefaults")
-    notes: list[S5pNote] = Field(default_factory=list)
+    notes: list[Optional[S5pNote]] = Field(default_factory=list)
     gs_events: None = Field(None, alias="gsEvents")
     mixer: S5pTrackMixer = Field(default_factory=S5pTrackMixer)
     parameters: S5pParameters = Field(default_factory=S5pParameters)
 
 
 class S5pInstrumental(BaseModel):
     filename: str = ""
```

### Comparing `libresvip-1.1.2/libresvip/plugins/s5p/s5p.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/s5p/s5p.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/s5p/synthv_editor_converter.py` & `libresvip-1.1.3/libresvip/plugins/s5p/synthv_editor_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/s5p/synthv_editor_generator.py` & `libresvip-1.1.3/libresvip/plugins/s5p/synthv_editor_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,21 @@
                     mixer=track_mixer,
                 )
                 if track.edited_params is not None:
                     s5p_track.parameters = self.generate_parameters(
                         track.edited_params, track.note_list
                     )
                 tracks.append(s5p_track)
+        if not tracks:
+            tracks.append(
+                S5pTrack(
+                    name="Unnamed Track",
+                    notes=[None],
+                )
+            )
         return tracks
 
     def generate_notes(self, note_list: list[Note]) -> list[S5pNote]:
         return [
             S5pNote(
                 lyric=note.lyric,
                 onset=note.start_pos * TICK_RATE,
```

### Comparing `libresvip-1.1.2/libresvip/plugins/s5p/synthv_editor_parser.py` & `libresvip-1.1.3/libresvip/plugins/s5p/synthv_editor_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import functools
 import math
 import operator
 import pathlib
-from typing import cast
+from typing import Optional, cast
 
 import more_itertools
 import portion
 import sortedcontainers
 
 from libresvip.core.constants import DEFAULT_BPM
 from libresvip.core.time_interval import PiecewiseIntervalDict
@@ -129,19 +129,23 @@
             mute=mixer.instrumental_muted,
             volume=self.parse_volume(mixer.gain_instrumental_decibel),
             title=pathlib.Path(track.filename).name,
             audio_file_path=track.filename,
             offset=round(self.synchronizer.get_actual_ticks_from_secs(track.offset)),
         )
 
-    def parse_notes(self, s5p_notes: list[S5pNote], db_defaults: S5pDbDefaults) -> list[Note]:
+    def parse_notes(
+        self, s5p_notes: list[Optional[S5pNote]], db_defaults: S5pDbDefaults
+    ) -> list[Note]:
         self.vibrato_value_interval_dict = PiecewiseIntervalDict()
         self.vibrato_coef_interval_dict = PiecewiseIntervalDict()
         notes = []
         for s5p_note in s5p_notes:
+            if s5p_note is None:
+                continue
             note = Note(
                 key_number=s5p_note.pitch,
                 start_pos=round(s5p_note.onset / TICK_RATE),
                 length=round(s5p_note.duration / TICK_RATE),
                 lyric=s5p_note.lyric.lstrip(".").replace(" ", "") or db_defaults.lyric,
                 pronunciation=s5p_note.comment
                 if s5p_note.lyric.startswith(".") and s5p_note.comment
```

### Comparing `libresvip-1.1.2/libresvip/plugins/srt/options.py` & `libresvip-1.1.3/libresvip/plugins/srt/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/srt/srt.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/srt/srt.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/srt/srt_generator.py` & `libresvip-1.1.3/libresvip/plugins/srt/srt_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svg/coordinate_helper.py` & `libresvip-1.1.3/libresvip/plugins/svg/coordinate_helper.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svg/options.py` & `libresvip-1.1.3/libresvip/plugins/svg/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svg/svg.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/svg/svg.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svg/svg_converter.py` & `libresvip-1.1.3/libresvip/plugins/svg/svg_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svg/svg_factory.py` & `libresvip-1.1.3/libresvip/plugins/svg/svg_factory.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svg/svg_generator.py` & `libresvip-1.1.3/libresvip/plugins/svg/svg_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/binsvip.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/svip/binsvip.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/binsvip_converter.py` & `libresvip-1.1.3/libresvip/plugins/svip/binsvip_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/binsvip_generator.py` & `libresvip-1.1.3/libresvip/plugins/svip/binsvip_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/binsvip_parser.py` & `libresvip-1.1.3/libresvip/plugins/svip/binsvip_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/models.py` & `libresvip-1.1.3/libresvip/plugins/svip/models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/msnrbf/binary_models.py` & `libresvip-1.1.3/libresvip/plugins/svip/msnrbf/binary_models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/msnrbf/nrbf_iobase.py` & `libresvip-1.1.3/libresvip/plugins/svip/msnrbf/nrbf_iobase.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/msnrbf/svip_reader.py` & `libresvip-1.1.3/libresvip/plugins/svip/msnrbf/svip_reader.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/msnrbf/svip_writer.py` & `libresvip-1.1.3/libresvip/plugins/svip/msnrbf/svip_writer.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/msnrbf/xstudio_models.py` & `libresvip-1.1.3/libresvip/plugins/svip/msnrbf/xstudio_models.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/options.py` & `libresvip-1.1.3/libresvip/plugins/svip/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip/singers.json` & `libresvip-1.1.3/libresvip/plugins/svip/singers.json`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip3/model.py` & `libresvip-1.1.3/libresvip/plugins/svip3/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip3/singers.json` & `libresvip-1.1.3/libresvip/plugins/svip3/singers.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'5e89d107-29f3-48e6-83b8-129bcca0fedf'": "'福姬彩华'"}*

```diff
@@ -4,14 +4,15 @@
     "090591a5-d535-4f16-b38a-849f971c0fa0": "\u6d77\u8389",
     "15452046-bd99-45b9-9fa5-14aeabe64052": "\u827e\u5c14\u6cd5",
     "31aceb85-c488-40cb-8745-8aaf63d9d8d5": "\u6d77\u5ddd",
     "4884b6a0-ab3d-4428-9a83-981e9b54d92b": "\u5c0f\u5802\u59b9",
     "4cf3650e-b017-4b04-be90-0b5625d889c8": "\u5f90\u68a6\u751c",
     "51c83781-5fa9-4bb6-bb35-76e64cf7b433": "\u5d14\u74a8",
     "540cdf30-d97b-488a-81c6-c56ad862b676": "\u82e5\u6eaa",
+    "5e89d107-29f3-48e6-83b8-129bcca0fedf": "\u798f\u59ec\u5f69\u534e",
     "74ec9910-ddd5-4f31-a1b2-e109fc555720": "\u6797\u5a67\u6021",
     "75805007-db40-4125-a22e-87742c6d3e65": "\u6d1b\u5929\u4f9d",
     "78bd36f6-7fd5-48e6-99f6-7d1b87fbf341": "\u65f6\u8427\u7136",
     "7d0c0cfc-00b3-4dca-b7b0-d20b634b531a": "\u5c0f\u51b0",
     "8643d5b2-e103-4b96-9358-81f7d4d89474": "\u6d1b\u5e0c",
     "8fc502e1-28a6-490e-824f-987772ea48ff": "\u767d\u5c7f\u5ddd",
     "9ccee3dd-9019-445f-a1cd-c51426162bd3": "\u9648\u5b50\u6e1d",
```

### Comparing `libresvip-1.1.2/libresvip/plugins/svip3/svip3.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/svip3/svip3.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip3/svip3_converter.py` & `libresvip-1.1.3/libresvip/plugins/svip3/svip3_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip3/svip3_generator.py` & `libresvip-1.1.3/libresvip/plugins/svip3/svip3_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svip3/svip3_parser.py` & `libresvip-1.1.3/libresvip/plugins/svip3/svip3_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/constants.py` & `libresvip-1.1.3/libresvip/plugins/svp/constants.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/lambert_w.py` & `libresvip-1.1.3/libresvip/plugins/svp/lambert_w.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/layer_generator.py` & `libresvip-1.1.3/libresvip/plugins/svp/layer_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/model.py` & `libresvip-1.1.3/libresvip/plugins/svp/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,15 +416,15 @@
         return self.model_copy(deep=True, update={"onset": self.onset + blick_offset})
 
     def __xor__(self, pitch_offset: int) -> SVNote:
         return self.model_copy(deep=True, update={"pitch": self.pitch + pitch_offset})
 
     @staticmethod
     def normalize_lyric(lyric: str) -> str:
-        return symbols_blacklist.cleanse_text(lyric).strip()
+        return symbols_blacklist.cleanse_text("-" if lyric == "+" else lyric).strip()
 
     @classmethod
     def normalize_phoneme(cls, note: Note) -> str:
         if note.pronunciation:
             return note.pronunciation
         elif (hanzi := re.search(rf"[{zhon.hanzi.characters}]+", note.lyric)) is not None:
             return hanzi[0]
```

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/options.py` & `libresvip-1.1.3/libresvip/plugins/svp/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/param_expression.py` & `libresvip-1.1.3/libresvip/plugins/svp/param_expression.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/phoneme_categories.json` & `libresvip-1.1.3/libresvip/plugins/svp/phoneme_categories.json`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/phoneme_dictionary.json` & `libresvip-1.1.3/libresvip/plugins/svp/phoneme_dictionary.json`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/phoneme_utils.py` & `libresvip-1.1.3/libresvip/plugins/svp/phoneme_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/pitch_simulator.py` & `libresvip-1.1.3/libresvip/plugins/svp/pitch_simulator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/pitch_slide.py` & `libresvip-1.1.3/libresvip/plugins/svp/pitch_slide.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/svp.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/svp/svp.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/synthv_generator.py` & `libresvip-1.1.3/libresvip/plugins/svp/synthv_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/synthv_parser.py` & `libresvip-1.1.3/libresvip/plugins/svp/synthv_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dataclasses
+import operator
 import re
 from collections.abc import Callable
 from functools import partial, reduce
 from typing import Optional, cast
 
 from libresvip.core.constants import DEFAULT_BPM
 from libresvip.core.tick_counter import shift_beat_list, shift_tempo_list
@@ -652,15 +653,15 @@
                             self.parse_note_list(group.notes, sv_ref.database),
                             self.parse_params(
                                 group.parameters, group.notes, sv_track.main_group.parameters
                             ),
                             self.first_bar_tick,
                         )
                         merged_group.notes.extend(group.notes)
-                        merged_group.notes.sort(key=lambda n: n.onset)
+                        merged_group.notes.sort(key=operator.attrgetter("onset"))
             svip_track = singing_track
         svip_track.title = sv_track.name
         svip_track.mute = sv_track.mixer.mute
         svip_track.solo = sv_track.mixer.solo
         svip_track.pan = sv_track.mixer.pan
         svip_track.volume = self.parse_volume(sv_track.mixer.gain_decibel)
         return svip_track
```

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/synthv_studio_converter.py` & `libresvip-1.1.3/libresvip/plugins/svp/synthv_studio_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/svp/track_merge_utils.py` & `libresvip-1.1.3/libresvip/plugins/svp/track_merge_utils.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/tlp/model.py` & `libresvip-1.1.3/libresvip/plugins/tlp/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
 
 class TuneLabNote(BaseModel):
     pos: float
     dur: float
     pitch: int
     lyric: str
+    pronunciation: Optional[str] = None
     phonemes: list[TuneLabPhoneme] = Field(default_factory=list)
     properties: dict[str, Any] = Field(default_factory=dict)
 
 
 class TuneLabVibrato(BaseModel):
     pos: float
     dur: float
```

### Comparing `libresvip-1.1.2/libresvip/plugins/tlp/tunelab_converter.py` & `libresvip-1.1.3/libresvip/plugins/tlp/tunelab_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/tlp/tunelab_generator.py` & `libresvip-1.1.3/libresvip/plugins/tlp/tunelab_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,19 @@
     def generate_volume(volume: float) -> float:
         return max(ratio_to_db(max(volume, 0.01)), -70) if volume > 0 else -70
 
     @staticmethod
     def generate_notes(note_list: list[Note]) -> list[TuneLabNote]:
         return [
             TuneLabNote(
-                pos=note.start_pos, dur=note.length, pitch=note.key_number, lyric=note.lyric
+                pos=note.start_pos,
+                dur=note.length,
+                pitch=note.key_number,
+                lyric=note.lyric,
+                pronunciation=note.pronunciation,
             )
             for note in note_list
         ]
 
     def generate_pitch(self, pitch: ParamCurve) -> list[TuneLabPoints]:
         return [
             TuneLabPoints(
```

### Comparing `libresvip-1.1.2/libresvip/plugins/tlp/tunelab_parser.py` & `libresvip-1.1.3/libresvip/plugins/vspx/vspx_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,145 +1,154 @@
 import dataclasses
+from typing import Optional, Union
 
-import more_itertools
-
+from libresvip.core.time_sync import TimeSynchronizer
 from libresvip.model.base import (
     InstrumentalTrack,
     Note,
+    ParamCurve,
+    Points,
     Project,
     SingingTrack,
     SongTempo,
     TimeSignature,
-    Track,
 )
 from libresvip.model.point import Point
-from libresvip.utils.music_math import db_to_float, ratio_to_db
 
 from .model import (
-    TuneLabAudioPart,
-    TuneLabMidiPart,
-    TuneLabNote,
-    TuneLabPoints,
-    TuneLabProject,
-    TuneLabTempo,
-    TuneLabTimeSignature,
-    TuneLabTrack,
+    PIT,
+    VocalSharpBeat,
+    VocalSharpDefaultTrill,
+    VocalSharpMonoTrack,
+    VocalSharpNote,
+    VocalSharpNoteTrack,
+    VocalSharpProject,
+    VocalSharpStereoTrack,
+    VocalSharpTempo,
 )
 from .options import InputOptions
+from .vspx_interval_dict import BasePitchCurve
 
 
 @dataclasses.dataclass
-class TuneLabParser:
+class VocalSharpParser:
     options: InputOptions
+    default_trill: Optional[VocalSharpDefaultTrill] = None
+    synchronizer: TimeSynchronizer = dataclasses.field(init=False)
     first_bar_length: int = dataclasses.field(init=False)
 
-    def parse_project(self, project: TuneLabProject) -> Project:
-        time_signature_list = self.parse_time_signatures(project.time_signatures)
-        self.first_bar_length = round(time_signature_list[0].bar_length())
-        tempo_list = self.parse_tempos(project.tempos)
+    def parse_project(self, vspx_project: VocalSharpProject) -> Project:
+        self.default_trill = vspx_project.project.default_trill
+        time_signatures = self.parse_time_signatures(vspx_project.project.beat)
+        self.first_bar_length = round(time_signatures[0].bar_length())
+        tempos = self.parse_tempos(vspx_project.project.tempo)
+        self.synchronizer = TimeSynchronizer(tempos)
+        singing_tracks = self.parse_singing_tracks(
+            [
+                track
+                for track in vspx_project.project.tracks
+                if isinstance(track, VocalSharpNoteTrack)
+            ]
+        )
+        instrumental_tracks = self.parse_instrumental_tracks(
+            [
+                track
+                for track in vspx_project.project.tracks
+                if isinstance(track, (VocalSharpMonoTrack, VocalSharpStereoTrack))
+            ]
+        )
         return Project(
-            song_tempo_list=tempo_list,
-            time_signature_list=time_signature_list,
-            track_list=self.parse_tracks(project.tracks),
+            time_signature_list=time_signatures,
+            song_tempo_list=tempos,
+            track_list=singing_tracks + instrumental_tracks,
         )
 
-    def parse_time_signatures(
-        self, time_signatures: list[TuneLabTimeSignature]
-    ) -> list[TimeSignature]:
+    def parse_time_signatures(self, beat_list: list[VocalSharpBeat]) -> list[TimeSignature]:
         return [
             TimeSignature(
-                bar_index=time_signature.bar_index,
-                numerator=time_signature.numerator,
-                denominator=time_signature.denominator,
+                bar_index=beat.bar_index,
+                numerator=beat.beat_per_bar,
+                denominator=beat.bar_divide,
             )
-            for time_signature in time_signatures
+            for beat in beat_list
         ]
 
-    def parse_tempos(self, tempos: list[TuneLabTempo]) -> list[SongTempo]:
-        return [SongTempo(position=int(tempo.pos), bpm=tempo.bpm) for tempo in tempos]
+    def parse_tempos(self, tempo_list: list[VocalSharpTempo]) -> list[SongTempo]:
+        return [
+            SongTempo(
+                position=tempo.pos,
+                bpm=tempo.bpm,
+            )
+            for tempo in tempo_list
+        ]
 
-    def parse_tracks(self, tracks: list[TuneLabTrack]) -> list[Track]:
-        track_list = []
-        for track in tracks:
-            for part in track.parts:
-                if isinstance(part, TuneLabAudioPart) and self.options.import_instrumental_track:
-                    track_list.append(
-                        InstrumentalTrack(
-                            audio_file_path=part.path,
-                            title=part.name,
-                            offset=int(part.pos),
-                            volume=self.parse_volume(track.gain),
-                            pan=track.pan,
-                            mute=track.mute,
-                            solo=track.solo,
-                        )
-                    )
-                elif isinstance(part, TuneLabMidiPart) and len(part.notes):
-                    if (
-                        len(track_list)
-                        and isinstance(track_list[-1], SingingTrack)
-                        and (
-                            not track_list[-1].note_list
-                            or track_list[-1].note_list[-1].end_pos <= int(part.pos)
-                        )
-                    ):
-                        singing_track = track_list[-1]
-                    else:
-                        singing_track = SingingTrack(
-                            title=part.name,
-                            volume=self.parse_volume(track.gain),
-                            pan=track.pan,
-                            mute=track.mute,
-                            solo=track.solo,
-                        )
-                        track_list.append(singing_track)
-                    singing_track.note_list.extend(self.parse_notes(part.notes, int(part.pos)))
-                    if self.options.import_pitch and (
-                        pitch_points := self.parse_pitch(part.pitch, int(part.pos))
-                    ):
-                        singing_track.edited_params.pitch.points.root.extend(pitch_points)
-        return track_list
-
-    @staticmethod
-    def parse_volume(gain: float) -> float:
-        if gain >= 0:
-            return min(gain / (ratio_to_db(4)) + 1.0, 2.0)
-        else:
-            return db_to_float(gain)
+    def parse_singing_tracks(self, track_list: list[VocalSharpNoteTrack]) -> list[SingingTrack]:
+        tracks = []
+        for track in track_list:
+            singing_track = SingingTrack(
+                title=track.name,
+                mute=track.is_mute == "True",
+                solo=track.is_solo == "True",
+                ai_singer_name=track.singer,
+                note_list=self.parse_notes(track.note),
+            )
+            if self.options.import_pitch:
+                singing_track.edited_params.pitch = self.parse_pitch(track)
+            tracks.append(singing_track)
+        return tracks
 
-    @staticmethod
-    def parse_notes(notes: list[TuneLabNote], offset: int) -> list[Note]:
+    def parse_notes(self, note_list: list[VocalSharpNote]) -> list[Note]:
         return [
             Note(
-                start_pos=tlp_note.pos + offset,
-                length=tlp_note.dur,
-                key_number=tlp_note.pitch,
-                lyric=tlp_note.lyric,
+                start_pos=note.pos,
+                length=note.duration,
+                key_number=note.key_number,
+                lyric=note.lyric,
+                pronunciation=note.lyric,
             )
-            for tlp_note in notes
+            for note in note_list
         ]
 
-    def parse_pitch(self, pitch: list[TuneLabPoints], offset: int) -> list[Point]:
-        points: list[Point] = []
-        for pitch_part in pitch:
-            for is_first, is_last, tlp_point in more_itertools.mark_ends(pitch_part.root):
-                if is_first:
-                    points.append(
+    def parse_pitch(self, note_track: VocalSharpNoteTrack) -> ParamCurve:
+        base_pitch_curve = BasePitchCurve(note_track, self.default_trill, self.synchronizer)
+        pitch_points = [Point.start_point()]
+        prev_tick = None
+        for vspx_point in note_track.parameter.points:
+            if isinstance(vspx_point, PIT):
+                cur_tick = vspx_point.time + self.first_bar_length
+                if prev_tick is None:
+                    pitch_points.append(Point(x=cur_tick, y=-100))
+                elif vspx_point.time - prev_tick > 1:
+                    pitch_points.append(Point(x=prev_tick, y=-100))
+                    pitch_points.append(Point(x=cur_tick, y=-100))
+                vspx_point_secs = self.synchronizer.get_actual_secs_from_ticks(vspx_point.time)
+                if (base_key := base_pitch_curve.semitone_value_at(vspx_point_secs)) is not None:
+                    pitch_points.append(
                         Point(
-                            x=int(tlp_point.pos) + offset + self.first_bar_length,
-                            y=-100,
+                            x=cur_tick,
+                            y=round(base_key * 100 + vspx_point.value),
                         )
                     )
-                points.append(
-                    Point(
-                        x=int(tlp_point.pos) + offset + self.first_bar_length,
-                        y=round(tlp_point.value * 100),
-                    )
-                )
-                if is_last:
-                    points.append(
-                        Point(
-                            x=points[-1].x,
-                            y=-100,
-                        )
+                prev_tick = cur_tick
+        if len(pitch_points) > 1:
+            pitch_points.append(Point(x=pitch_points[-1].x, y=-100))
+        pitch_points.append(Point.end_point())
+        if len(pitch_points) <= 2:
+            pitch_points.clear()
+        return ParamCurve(points=Points(root=pitch_points))
+
+    def parse_instrumental_tracks(
+        self, track_list: list[Union[VocalSharpMonoTrack, VocalSharpStereoTrack]]
+    ) -> list[InstrumentalTrack]:
+        tracks = []
+        if self.options.import_instrumental_track:
+            for track in track_list:
+                for i, sequence in enumerate(track.sequences):
+                    instrumental_track = InstrumentalTrack(
+                        title=sequence.name or f"{track.name} {i + 1}",
+                        mute=track.is_mute == "True",
+                        solo=track.is_solo == "True",
+                        offset=sequence.pos,
+                        audio_file_path=sequence.path,
                     )
-        return points
+                    tracks.append(instrumental_track)
+        return tracks
```

### Comparing `libresvip-1.1.2/libresvip/plugins/tssln/model.py` & `libresvip-1.1.3/libresvip/plugins/tssln/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/tssln/tssln.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/tssln/tssln.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/tssln/value_tree.py` & `libresvip-1.1.3/libresvip/plugins/tssln/value_tree.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/tssln/voisona_converter.py` & `libresvip-1.1.3/libresvip/plugins/tssln/voisona_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/tssln/voisona_generator.py` & `libresvip-1.1.3/libresvip/plugins/tssln/voisona_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/tssln/voisona_parser.py` & `libresvip-1.1.3/libresvip/plugins/tssln/voisona_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -139,34 +139,55 @@
                         )
                     )
         tempos = shift_tempo_list(tempos, tick_prefix)
         voisona_track_pitch_data = None
         if track.plugin_data.state_information.parameter is not None:
             for parameter in track.plugin_data.state_information.parameter:
                 if parameter.log_f0 is not None:
-                    for curve in parameter.log_f0:
-                        pitch_data_nodes: list[VoiSonaPointData] = curve.data
-                        pitch_datas = [
-                            pitch_data
-                            for data_node in pitch_data_nodes
-                            if (pitch_data := self.parse_pitch_data(data_node))
-                        ]
-                        voisona_track_pitch_data = VoiSonaTrackPitchData(
-                            events=pitch_datas, tempos=tempos, tick_prefix=tick_prefix
-                        )
+                    pitch_data_nodes: list[VoiSonaPointData] = sum(
+                        (curve.data for curve in parameter.log_f0), []
+                    )
+                    vibrato_amplitude_nodes: list[VoiSonaPointData] = sum(
+                        (curve.data for curve in parameter.vib_amp or []), []
+                    )
+                    vibrato_frequency_nodes: list[VoiSonaPointData] = sum(
+                        (curve.data for curve in parameter.vib_frq or []), []
+                    )
+                    pitch_datas = [
+                        pitch_data
+                        for data_node in pitch_data_nodes
+                        if (pitch_data := self.parse_param_data(data_node))
+                    ]
+                    vibrato_amplitude_data = [
+                        vibrato_amplitude
+                        for vibrato_amplitude_node in vibrato_amplitude_nodes
+                        if (vibrato_amplitude := self.parse_param_data(vibrato_amplitude_node))
+                    ]
+                    vibrato_frequency_data = [
+                        vibrato_frequency
+                        for vibrato_frequency_node in vibrato_frequency_nodes
+                        if (vibrato_frequency := self.parse_param_data(vibrato_frequency_node))
+                    ]
+                    voisona_track_pitch_data = VoiSonaTrackPitchData(
+                        events=pitch_datas,
+                        tempos=tempos,
+                        tick_prefix=tick_prefix,
+                        vibrato_amplitude_events=vibrato_amplitude_data,
+                        vibrato_frequency_events=vibrato_frequency_data,
+                    )
         time_signatures = shift_beat_list(time_signatures, 1)
         singing_track = SingingTrack(title=track.name, note_list=notes)
         if (
             self.options.import_pitch
             and voisona_track_pitch_data is not None
             and (pitch := pitch_from_voisona_track(voisona_track_pitch_data)) is not None
         ):
             singing_track.edited_params.pitch = pitch
         return singing_track, tempos, time_signatures
 
     @staticmethod
-    def parse_pitch_data(data_element: VoiSonaPointData) -> Optional[VoiSonaParamEvent]:
+    def parse_param_data(data_element: VoiSonaPointData) -> Optional[VoiSonaParamEvent]:
         value = float(data_element.value) if data_element.value is not None else None
         if value is not None:
             index = data_element.index or None
             repeat = data_element.repeat or None
             return VoiSonaParamEvent(idx=index, repeat=repeat, value=value)
```

### Comparing `libresvip-1.1.2/libresvip/plugins/tssln/voisona_pitch.py` & `libresvip-1.1.3/libresvip/plugins/tssln/voisona_pitch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 import dataclasses
+import functools
 import itertools
 import math
-from typing import NamedTuple, Optional
+from typing import NamedTuple, Optional, cast
 
 import more_itertools
+import portion
 
 from libresvip.core.tick_counter import shift_tempo_list
+from libresvip.core.time_interval import PiecewiseIntervalDict
+from libresvip.core.time_sync import TimeSynchronizer
 from libresvip.core.warning_types import show_warning
 from libresvip.model.base import ParamCurve, Points, SongTempo
 from libresvip.model.point import Point
 from libresvip.utils.music_math import hz2midi, midi2hz
 from libresvip.utils.search import find_last_index
 from libresvip.utils.translation import gettext_lazy as _
 
@@ -43,43 +47,62 @@
 
 
 @dataclasses.dataclass
 class VoiSonaTrackPitchData:
     events: list[VoiSonaParamEvent]
     tempos: list[SongTempo]
     tick_prefix: int
+    vibrato_amplitude_events: list[VoiSonaParamEvent] = dataclasses.field(default_factory=list)
+    vibrato_frequency_events: list[VoiSonaParamEvent] = dataclasses.field(default_factory=list)
 
     @property
     def length(self) -> int:
         last_has_index = find_last_index(self.events, lambda event: event.idx is not None)
         length = self.events[last_has_index].idx + sum(
             event.repeat or 1 for event in self.events[last_has_index:]
         )
         return length + MIN_DATA_LENGTH
 
 
 def pitch_from_voisona_track(data: VoiSonaTrackPitchData) -> Optional[ParamCurve]:
     converted_points = [Point.start_point()]
     current_value = -100
 
+    synchronizer = TimeSynchronizer(data.tempos)
+    vibrato_amplitude_interval_dict = build_voisona_param_interval_dict(
+        data.vibrato_amplitude_events, synchronizer, data.tick_prefix
+    )
+    vibrato_value_interval_dict = build_voisona_wave_interval_dict(
+        data.vibrato_frequency_events, synchronizer, data.tick_prefix
+    )
+
     events_normalized = shape_events(
         normalize_to_tick(append_ending_points(data.events), data.tempos, data.tick_prefix)
     )
 
     next_pos = None
     for event in events_normalized:
-        pos = event.idx - data.tick_prefix
+        pos = int(cast(float, event.idx)) - data.tick_prefix
+        secs = synchronizer.get_actual_secs_from_ticks(pos)
         length = event.repeat
         try:
             value = round(hz2midi(math.e**event.value) * 100) if event.value is not None else -100
             if value != current_value or next_pos != pos:
                 converted_points.append(Point(x=round(pos), y=value))
                 if value == -100:
                     converted_points.append(Point(x=round(pos), y=value))
                 current_value = value
+            secs_step = synchronizer.get_duration_secs_from_ticks(pos, pos + 5)
+            for pos_x in range(pos, int(cast(float, pos + length)), 5):
+                if value_diff := vibrato_value_interval_dict.get(secs):
+                    value_diff *= vibrato_amplitude_interval_dict.get(secs, 1)
+                    converted_points.append(Point(x=pos_x, y=round(value + value_diff)))
+                else:
+                    break
+                secs += secs_step
         except OverflowError:
             show_warning(_("Pitch value is out of bounds"))
         next_pos = pos + length
     converted_points.append(Point.end_point())
 
     return ParamCurve(points=Points(root=converted_points)) if len(converted_points) > 2 else None
 
@@ -179,14 +202,101 @@
             last_pos, last_tick_pos, last_bpm = result[-1]
             ticks_in_time_unit = TIME_UNIT_AS_TICKS_PER_BPM * last_bpm
             new_pos = last_pos + (tempo.position - last_tick_pos) / ticks_in_time_unit
             result.append((int(new_pos), tempo.position, tempo.bpm))
     return result
 
 
+def vibrato_curve(value: float, shift: float, omega: float, phase: float) -> float:
+    return math.sin(omega * (value - shift) + phase)
+
+
+def build_voisona_param_interval_dict(
+    events: list[VoiSonaParamEvent], synchronizer: TimeSynchronizer, tick_prefix: int
+) -> PiecewiseIntervalDict:
+    param_interval_dict = PiecewiseIntervalDict()
+    for continuous_part in more_itertools.split_before(
+        events,
+        lambda event: event.idx is not None,
+    ):
+        for prev_event, next_event in more_itertools.windowed(
+            more_itertools.prepend(
+                None,
+                normalize_to_tick(
+                    append_ending_points(continuous_part), synchronizer.tempo_list, tick_prefix
+                ),
+            ),
+            2,
+        ):
+            next_start = synchronizer.get_actual_secs_from_ticks(next_event.idx - tick_prefix)
+            if (
+                prev_event is not None
+                and (
+                    prev_end := synchronizer.get_actual_secs_from_ticks(
+                        prev_event.idx + (prev_event.repeat or 1) - tick_prefix
+                    )
+                )
+                and prev_end < next_start
+            ):
+                param_interval_dict[portion.closedopen(prev_end, next_start)] = next_event.value
+            param_interval_dict[
+                portion.closedopen(
+                    next_start,
+                    synchronizer.get_actual_secs_from_ticks(
+                        next_event.idx + (next_event.repeat or 1) - tick_prefix
+                    ),
+                )
+            ] = next_event.value
+    return param_interval_dict
+
+
+def build_voisona_wave_interval_dict(
+    events: list[VoiSonaParamEvent], synchronizer: TimeSynchronizer, tick_prefix: int
+) -> PiecewiseIntervalDict:
+    param_interval_dict = PiecewiseIntervalDict()
+    omega = math.tau * 6
+    for continuous_part in more_itertools.split_before(
+        events,
+        lambda event: event.idx is not None,
+    ):
+        phase = 0.0
+        for prev_event, next_event in more_itertools.windowed(
+            more_itertools.prepend(
+                None,
+                normalize_to_tick(
+                    append_ending_points(continuous_part), synchronizer.tempo_list, tick_prefix
+                ),
+            ),
+            2,
+        ):
+            next_start = synchronizer.get_actual_secs_from_ticks(next_event.idx - tick_prefix)
+            next_end = synchronizer.get_actual_secs_from_ticks(
+                next_event.idx + (next_event.repeat or 1) - tick_prefix
+            )
+            if (
+                prev_event is not None
+                and (
+                    prev_end := synchronizer.get_actual_secs_from_ticks(
+                        prev_event.idx + (prev_event.repeat or 1) - tick_prefix
+                    )
+                )
+                and prev_end < next_start
+            ):
+                prev_start = synchronizer.get_actual_secs_from_ticks(prev_event.idx - tick_prefix)
+                param_interval_dict[portion.closedopen(prev_end, next_start)] = vibrato_curve(
+                    prev_end, prev_start, omega, phase
+                )
+            omega = math.tau * (next_event.value or 6)
+            param_interval_dict[portion.closedopen(next_start, next_end)] = functools.partial(
+                vibrato_curve, shift=next_start, omega=omega, phase=phase
+            )
+            phase += (next_end - next_start) * omega
+    return param_interval_dict
+
+
 def generate_for_voisona(
     pitch: ParamCurve, tempos: list[SongTempo], tick_prefix: int
 ) -> Optional[VoiSonaTrackPitchData]:
     events_with_full_params = []
     for i, this_point in enumerate(pitch.points.root):
         next_point = pitch.points[i + 1] if i + 1 < len(pitch.points) else None
         end_tick = next_point.x - tick_prefix if next_point else None
```

### Comparing `libresvip-1.1.2/libresvip/plugins/ufdata/model.py` & `libresvip-1.1.3/libresvip/plugins/ufdata/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ufdata/ufdata.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/ufdata/ufdata.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ufdata/ufdata_converter.py` & `libresvip-1.1.3/libresvip/plugins/ufdata/ufdata_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ufdata/ufdata_generator.py` & `libresvip-1.1.3/libresvip/plugins/ufdata/ufdata_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ufdata/ufdata_parser.py` & `libresvip-1.1.3/libresvip/plugins/ufdata/ufdata_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/interpolation.py` & `libresvip-1.1.3/libresvip/plugins/ust/interpolation.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/model.py` & `libresvip-1.1.3/libresvip/plugins/ust/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/options.py` & `libresvip-1.1.3/libresvip/plugins/ust/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/pitch_mode1.py` & `libresvip-1.1.3/libresvip/plugins/ust/pitch_mode1.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/pitch_mode2.py` & `libresvip-1.1.3/libresvip/plugins/ust/pitch_mode2.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/rdp_simplification.py` & `libresvip-1.1.3/libresvip/plugins/ust/rdp_simplification.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/resampling.py` & `libresvip-1.1.3/libresvip/plugins/ust/resampling.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/template.py` & `libresvip-1.1.3/libresvip/plugins/ust/template.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/ust.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/ust/ust.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/ust_converter.py` & `libresvip-1.1.3/libresvip/plugins/ust/ust_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/ust_generator.py` & `libresvip-1.1.3/libresvip/plugins/ust/ust_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/ust_parser.py` & `libresvip-1.1.3/libresvip/plugins/ust/ust_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ust/vibrato_param.py` & `libresvip-1.1.3/libresvip/plugins/ust/vibrato_param.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ustx/model.py` & `libresvip-1.1.3/libresvip/plugins/ustx/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ustx/ustx.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/ustx/ustx.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ustx/ustx_converter.py` & `libresvip-1.1.3/libresvip/plugins/ustx/ustx_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ustx/ustx_generator.py` & `libresvip-1.1.3/libresvip/plugins/ustx/ustx_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ustx/ustx_parser.py` & `libresvip-1.1.3/libresvip/plugins/ustx/ustx_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ustx/util.py` & `libresvip-1.1.3/libresvip/plugins/ustx/util.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ustx/utils/music_math.py` & `libresvip-1.1.3/libresvip/plugins/ustx/utils/music_math.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/ustx/utils/time_axis.py` & `libresvip-1.1.3/libresvip/plugins/ustx/utils/time_axis.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vog/model.py` & `libresvip-1.1.3/libresvip/plugins/vog/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vog/vog.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/vog/vog.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vog/vogen_converter.py` & `libresvip-1.1.3/libresvip/plugins/vog/vogen_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vog/vogen_generator.py` & `libresvip-1.1.3/libresvip/plugins/vog/vogen_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vog/vogen_parser.py` & `libresvip-1.1.3/libresvip/plugins/vog/vogen_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vpr/model.py` & `libresvip-1.1.3/libresvip/plugins/vpr/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vpr/options.py` & `libresvip-1.1.3/libresvip/plugins/vpr/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vpr/vocaloid_pitch.py` & `libresvip-1.1.3/libresvip/plugins/vpr/vocaloid_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vpr/vpr.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/vpr/vpr.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vpr/vpr_converter.py` & `libresvip-1.1.3/libresvip/plugins/vpr/vpr_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vpr/vpr_generator.py` & `libresvip-1.1.3/libresvip/plugins/vpr/vpr_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vpr/vpr_parser.py` & `libresvip-1.1.3/libresvip/plugins/vpr/vpr_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vshp/model.py` & `libresvip-1.1.3/libresvip/plugins/vshp/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vshp/options.py` & `libresvip-1.1.3/libresvip/plugins/vshp/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vshp/vocalshifter_converter.py` & `libresvip-1.1.3/libresvip/plugins/vshp/vocalshifter_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vshp/vocalshifter_parser.py` & `libresvip-1.1.3/libresvip/plugins/vshp/vocalshifter_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import dataclasses
 import math
 import pathlib
 from collections.abc import Callable
 
-from construct import Container
-
 from libresvip.core.constants import DEFAULT_CHINESE_LYRIC
 from libresvip.core.time_sync import TimeSynchronizer
 from libresvip.model.base import (
     InstrumentalTrack,
     Note,
     ParamCurve,
     Params,
@@ -25,25 +23,25 @@
     VocalShifterLabel,
     VocalShifterNote,
     VocalShifterPatternData,
     VocalShifterPatternMetadata,
     VocalShifterPatternType,
     VocalShifterProjectData,
     VocalShifterProjectMetadata,
+    VocalShifterTrackMetadata,
 )
 from .options import InputOptions
 from .utils import ansi2unicode
 
 
 @dataclasses.dataclass
 class VocalShifterParser:
     options: InputOptions
     synchronizer: TimeSynchronizer = dataclasses.field(init=False)
     tick_rate: float = dataclasses.field(init=False)
-    track_index2metadata: dict[int, Container] = dataclasses.field(default_factory=dict)
 
     def parse_project(self, vshp_proj: VocalShifterProjectData) -> Project:
         project = Project(
             song_tempo_list=self.parse_tempo(vshp_proj.project_metadata),
             time_signature_list=self.parse_time_signature(vshp_proj.project_metadata),
         )
         project.track_list = self.parse_track_list(vshp_proj)
@@ -69,54 +67,60 @@
                 numerator=vshp_metadata.numerator,
                 denominator=vshp_metadata.denominator,
             )
         ]
 
     def parse_track_list(self, vshp_proj: VocalShifterProjectData) -> list[Track]:
         track_list = []
-        for i, track_metadata in enumerate(vshp_proj.track_metadatas):
-            self.track_index2metadata[i + 1] = track_metadata
         for pattern_metadata, pattern_data in zip(
             vshp_proj.pattern_metadatas, vshp_proj.pattern_datas
         ):
             if (
                 pattern_data.header.pattern_type == VocalShifterPatternType.WAVE
                 and not self.options.wave_to_singing
             ):
-                track = self.parse_instrumental_track(pattern_metadata, pattern_data)
+                track = self.parse_instrumental_track(
+                    pattern_metadata,
+                    pattern_data,
+                    vshp_proj.track_metadatas[pattern_metadata.track_index],
+                )
             else:
-                track = self.parse_singing_track(pattern_metadata, pattern_data)
+                track = self.parse_singing_track(
+                    pattern_metadata,
+                    pattern_data,
+                    vshp_proj.track_metadatas[pattern_metadata.track_index],
+                )
             track_list.append(track)
         return track_list
 
     def parse_instrumental_track(
         self,
         pattern_metadata: VocalShifterPatternMetadata,
         pattern_data: VocalShifterPatternData,
+        track_metadata: VocalShifterTrackMetadata,
     ) -> InstrumentalTrack:
         sample_rate = pattern_data.header.sample_rate
         sample_offset = pattern_metadata.offset_samples + pattern_metadata.offset_correction
         offset_in_seconds = sample_offset / sample_rate
         offset_in_ticks = self.synchronizer.get_actual_ticks_from_secs(offset_in_seconds)
-        track_metadata = self.track_index2metadata[pattern_metadata.track_index]
         return InstrumentalTrack(
             audio_file_path=ansi2unicode(pattern_metadata.path_and_ext.split(b"\x00")[0]),
             offset=offset_in_ticks,
             solo=track_metadata.solo,
             mute=track_metadata.mute,
             volume=track_metadata.volume,
             pan=track_metadata.pan,
         )
 
     def parse_singing_track(
         self,
         pattern_metadata: VocalShifterPatternMetadata,
         pattern_data: VocalShifterPatternData,
+        track_metadata: VocalShifterTrackMetadata,
     ) -> SingingTrack:
-        track_metadata = self.track_index2metadata[pattern_metadata.track_index]
         file_path = pathlib.Path(ansi2unicode(pattern_metadata.path_and_ext.split(b"\x00")[0]))
         track = SingingTrack(
             title=file_path.stem,
             solo=track_metadata.solo,
             mute=track_metadata.mute,
             volume=track_metadata.volume,
             pan=track_metadata.pan,
```

### Comparing `libresvip-1.1.2/libresvip/plugins/vshp/vshp.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/vshp/vshp.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vspx/model.py` & `libresvip-1.1.3/libresvip/plugins/vspx/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
     trill: Optional[VocalSharpTrill] = field(
         default=None,
         metadata={
             "name": "trill",
             "type": "Element",
         },
     )
-    syllable: Optional[list[VocalSharpSyllable]] = field(
+    syllable: list[VocalSharpSyllable] = field(
         default_factory=list,
         metadata={
             "name": "Syllable",
             "type": "Element",
         },
     )
```

### Comparing `libresvip-1.1.2/libresvip/plugins/vspx/vocalsharp_converter.py` & `libresvip-1.1.3/libresvip/plugins/vspx/vocalsharp_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vspx/vspx.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/vspx/vspx.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vspx/vspx_generator.py` & `libresvip-1.1.3/libresvip/plugins/vspx/vspx_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vspx/vspx_interval_dict.py` & `libresvip-1.1.3/libresvip/plugins/vspx/vspx_interval_dict.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsq/options.py` & `libresvip-1.1.3/libresvip/plugins/vsq/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsq/vocaloid_pitch.py` & `libresvip-1.1.3/libresvip/plugins/vsq/vocaloid_pitch.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsq/vsq.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/vsq/vsq.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsq/vsq_converter.py` & `libresvip-1.1.3/libresvip/plugins/vsq/vsq_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsq/vsq_generator.py` & `libresvip-1.1.3/libresvip/plugins/vsq/vsq_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsq/vsq_parser.py` & `libresvip-1.1.3/libresvip/plugins/vsq/vsq_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,28 @@
 
     def parse_track(self, text: str, track_index: int, tick_prefix: int) -> SingingTrack:
         vsq_track = configparser.ConfigParser()
         try:
             vsq_track.read_string(text)
         except configparser.Error:
             vsq_track.read_string(text.rsplit("\n", 1)[0])
+        singer_name = ""
+        if (
+            singer_icon_key := next(
+                (
+                    value.get("iconhandle")
+                    for key, value in vsq_track.items()
+                    if key.startswith("ID#") and value.get("type") == "Singer"
+                ),
+                None,
+            )
+        ) is not None:
+            singer_name = vsq_track.get(singer_icon_key, "ids", fallback="")
         singing_track = SingingTrack(
+            ai_singer_name=singer_name,
             title=vsq_track.get("Common", "Name", fallback=f"Track {track_index}"),
             note_list=self.parse_notes(vsq_track, tick_prefix)
             if vsq_track.has_section("EventList")
             else [],
         )
         if self.options.import_pitch and (
             pitch := self.parse_pitch(vsq_track, singing_track.note_list, tick_prefix)
```

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/enums.py` & `libresvip-1.1.3/libresvip/plugins/vsqx/enums.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/model.py` & `libresvip-1.1.3/libresvip/plugins/vsqx/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/models/vsqx3.py` & `libresvip-1.1.3/libresvip/plugins/vsqx/models/vsqx3.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/models/vsqx4.py` & `libresvip-1.1.3/libresvip/plugins/vsqx/models/vsqx4.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/options.py` & `libresvip-1.1.3/libresvip/plugins/vsqx/options.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/vocaloid_pitch.py` & `libresvip-1.1.3/libresvip/plugins/vsqx/vocaloid_pitch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import math
 from dataclasses import dataclass
 from typing import Optional
 
+from libresvip.core.time_interval import PiecewiseIntervalDict
+from libresvip.core.time_sync import TimeSynchronizer
 from libresvip.model.base import Note, ParamCurve
 from libresvip.model.point import Point
 from libresvip.model.relative_pitch_curve import RelativePitchCurve
 from libresvip.utils.music_math import clamp
 
 from .constants import (
     DEFAULT_PITCH_BEND_SENSITIVITY,
@@ -25,15 +27,18 @@
     start_pos: int
     pit: list[ControllerEvent]
     pbs: list[ControllerEvent]
 
 
 def pitch_from_vocaloid_parts(
     data_by_parts: list[VocaloidPartPitchData],
+    synchronizer: TimeSynchronizer,
     note_list: list[Note],
+    vibrato_rate_interval_dict: PiecewiseIntervalDict,
+    vibrato_depth_interval_dict: PiecewiseIntervalDict,
     first_bar_length: int,
     lower_bound: int,
     upper_bound: int,
 ) -> Optional[ParamCurve]:
     pitch_raw_data_by_part = []
     for part in data_by_parts:
         pit = part.pit
@@ -71,21 +76,40 @@
         )
         if first_invalid_index_in_previous is None:
             pitch_raw_data += list(element.items())
         else:
             pitch_raw_data = pitch_raw_data[:first_invalid_index_in_previous] + list(
                 element.items()
             )
-    data = [
-        Point(
-            x=pos,
-            y=round((value / (PITCH_MAX_VALUE if value > 0 else (PITCH_MAX_VALUE + 1))) * 100),
+    data = []
+    prev_pos = None
+    value = None
+    for pos, pitch in pitch_raw_data:
+        pos_secs = synchronizer.get_actual_secs_from_ticks(pos)
+        if prev_pos is not None and value is not None:
+            for interp_pos in range(prev_pos + 5, pos, 5):
+                interp_pos_secs = synchronizer.get_actual_secs_from_ticks(interp_pos)
+                if interp_value_diff := vibrato_rate_interval_dict.get(interp_pos_secs, 0):
+                    interp_value_diff *= vibrato_depth_interval_dict.get(interp_pos_secs, 64)
+                data.append(
+                    Point(
+                        x=interp_pos,
+                        y=value + round(interp_value_diff),
+                    )
+                )
+        value = round((pitch / (PITCH_MAX_VALUE if pitch > 0 else (PITCH_MAX_VALUE + 1))) * 100)
+        if value_diff := vibrato_rate_interval_dict.get(pos_secs, 0):
+            value_diff *= vibrato_depth_interval_dict.get(pos_secs, 64)
+        data.append(
+            Point(
+                x=pos,
+                y=value + round(value_diff),
+            )
         )
-        for pos, value in pitch_raw_data
-    ]
+        prev_pos = pos
     return (
         RelativePitchCurve(first_bar_length, lower_bound, upper_bound).to_absolute(data, note_list)
         if data and note_list
         else None
     )
```

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/vsq3_generator.py` & `libresvip-1.1.3/libresvip/plugins/vsqx/vsq3_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/vsq4_generator.py` & `libresvip-1.1.3/libresvip/plugins/vsqx/vsq4_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/vsqx.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/vsqx/vsqx.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/vsqx_converter.py` & `libresvip-1.1.3/libresvip/plugins/vsqx/vsqx_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/vsqx/vsqx_parser.py` & `libresvip-1.1.3/libresvip/plugins/tlp/tunelab_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,236 +1,211 @@
 import dataclasses
-import pathlib
-from enum import Enum
-from typing import Optional
+import functools
+import math
+import operator
 
-from libresvip.core.constants import DEFAULT_ENGLISH_LYRIC
-from libresvip.core.tick_counter import skip_beat_list, skip_tempo_list
+import more_itertools
+import portion
+
+from libresvip.core.time_interval import PiecewiseIntervalDict
+from libresvip.core.time_sync import TimeSynchronizer
 from libresvip.model.base import (
     InstrumentalTrack,
     Note,
-    ParamCurve,
-    Point,
     Project,
     SingingTrack,
     SongTempo,
     TimeSignature,
+    Track,
 )
+from libresvip.model.point import Point
+from libresvip.utils.music_math import db_to_float, ratio_to_db
 
-from .constants import BPM_RATE
 from .model import (
-    Vsq3ParameterNames,
-    Vsq4ParameterNames,
-    Vsqx,
-    VsqxMasterTrack,
-    VsqxMusicalPart,
-    VsqxNote,
-    VsqxTempoList,
-    VsqxTimeSigList,
-    VsqxVsTrackList,
-    VsqxVsUnitList,
-    VsqxVVoice,
-    VsqxWavPartList,
-    VsqxWavUnitList,
+    TuneLabAudioPart,
+    TuneLabMidiPart,
+    TuneLabNote,
+    TuneLabPoints,
+    TuneLabProject,
+    TuneLabTempo,
+    TuneLabTimeSignature,
+    TuneLabTrack,
+    TuneLabVibrato,
 )
 from .options import InputOptions
-from .vocaloid_pitch import (
-    ControllerEvent,
-    VocaloidPartPitchData,
-    pitch_from_vocaloid_parts,
-)
 
 
 @dataclasses.dataclass
-class VsqxParser:
+class TuneLabParser:
     options: InputOptions
-    src_path: pathlib.Path
-    param_names: type[Enum] = dataclasses.field(init=False)
     first_bar_length: int = dataclasses.field(init=False)
-    pc2voice: dict[int, VsqxVVoice] = dataclasses.field(default_factory=dict)
+    synchronizer: TimeSynchronizer = dataclasses.field(init=False)
 
-    def parse_project(self, vsqx_project: Vsqx) -> Project:
-        if vsqx_project.Meta.name == "vsq3":
-            self.param_names = Vsq3ParameterNames
-        elif vsqx_project.Meta.name == "vsq4":
-            self.param_names = Vsq4ParameterNames
-        master_track: VsqxMasterTrack = vsqx_project.master_track
-        tick_prefix, time_signatures = self.parse_time_signatures(
-            master_track.time_sig, master_track.pre_measure
-        )
-        tempos = self.parse_tempos(master_track.tempo, tick_prefix)
-        for v_voice in vsqx_project.v_voice_table.v_voice:
-            if v_voice.v_pc is not None:
-                self.pc2voice[v_voice.v_pc] = v_voice
-        singing_tracks = self.parse_singing_tracks(
-            vsqx_project.vs_track, vsqx_project.mixer.vs_unit, tick_prefix, master_track.pre_measure
-        )
-        wav_parts: VsqxWavPartList = []
-        wav_units: VsqxWavUnitList = []
-        if vsqx_project.mono_track is not None:
-            wav_parts += vsqx_project.mono_track.wav_part
-            wav_units += [vsqx_project.mixer.mono_unit] * len(vsqx_project.mono_track.wav_part)  # type: ignore[list-item]
-        if vsqx_project.stereo_track is not None:
-            wav_parts += vsqx_project.stereo_track.wav_part
-            wav_units += [vsqx_project.mixer.stereo_unit] * len(vsqx_project.stereo_track.wav_part)  # type: ignore[list-item]
-        instrumental_tracks = self.parse_instrumental_tracks(wav_parts, wav_units, tick_prefix)
+    def parse_project(self, project: TuneLabProject) -> Project:
+        time_signature_list = self.parse_time_signatures(project.time_signatures)
+        self.first_bar_length = round(time_signature_list[0].bar_length())
+        tempo_list = self.parse_tempos(project.tempos)
+        self.synchronizer = TimeSynchronizer(tempo_list)
         return Project(
-            song_tempo_list=tempos,
-            time_signature_list=time_signatures,
-            track_list=singing_tracks + instrumental_tracks,
+            song_tempo_list=tempo_list,
+            time_signature_list=time_signature_list,
+            track_list=self.parse_tracks(project.tracks),
         )
 
     def parse_time_signatures(
-        self, time_signatures: VsqxTimeSigList, measure_prefix: int
-    ) -> tuple[int, list[TimeSignature]]:
-        time_signature_list = [
+        self, time_signatures: list[TuneLabTimeSignature]
+    ) -> list[TimeSignature]:
+        return [
             TimeSignature(
-                numerator=time_sig.nume,
-                denominator=time_sig.denomi,
-                bar_index=time_sig.pos_mes,
+                bar_index=time_signature.bar_index,
+                numerator=time_signature.numerator,
+                denominator=time_signature.denominator,
             )
-            for time_sig in time_signatures
+            for time_signature in time_signatures
         ]
-        tick_prefix = 0
-        measure = 0
-        for time_sig in time_signature_list:
-            measure_diff = time_sig.bar_index - measure
-            tick_prefix += measure_diff * round(time_sig.bar_length())
-            measure += time_sig.bar_index
-        measure_diff = measure_prefix - measure
-        tick_prefix += measure_diff * round(time_signature_list[-1].bar_length())
-        self.first_bar_length = round(time_signature_list[0].bar_length())
-        return int(tick_prefix), skip_beat_list(time_signature_list, measure_prefix)
 
-    def parse_tempos(self, tempos: VsqxTempoList, tick_prefix: int) -> list[SongTempo]:
-        tempo_list = [
-            SongTempo(
-                position=tempo.pos_tick,
-                bpm=tempo.bpm / BPM_RATE,
+    def parse_tempos(self, tempos: list[TuneLabTempo]) -> list[SongTempo]:
+        return [SongTempo(position=int(tempo.pos), bpm=tempo.bpm) for tempo in tempos]
+
+    def parse_tracks(self, tracks: list[TuneLabTrack]) -> list[Track]:
+        track_list = []
+        for track in tracks:
+            for part in track.parts:
+                if isinstance(part, TuneLabAudioPart) and self.options.import_instrumental_track:
+                    track_list.append(
+                        InstrumentalTrack(
+                            audio_file_path=part.path,
+                            title=part.name,
+                            offset=int(part.pos),
+                            volume=self.parse_volume(track.gain),
+                            pan=track.pan,
+                            mute=track.mute,
+                            solo=track.solo,
+                        )
+                    )
+                elif isinstance(part, TuneLabMidiPart) and len(part.notes):
+                    if (
+                        len(track_list)
+                        and isinstance(track_list[-1], SingingTrack)
+                        and (
+                            not track_list[-1].note_list
+                            or track_list[-1].note_list[-1].end_pos <= int(part.pos)
+                        )
+                    ):
+                        singing_track = track_list[-1]
+                    else:
+                        singing_track = SingingTrack(
+                            title=part.name,
+                            volume=self.parse_volume(track.gain),
+                            pan=track.pan,
+                            mute=track.mute,
+                            solo=track.solo,
+                        )
+                        track_list.append(singing_track)
+                    singing_track.note_list.extend(self.parse_notes(part.notes, int(part.pos)))
+                    if self.options.import_pitch:
+                        vibrato_base_interval_dict, vibrato_envelope_interval_dict = (
+                            self.parse_vibrato(part)
+                        )
+                        if pitch_points := self.parse_pitch(
+                            part.pitch,
+                            int(part.pos),
+                            vibrato_base_interval_dict,
+                            vibrato_envelope_interval_dict,
+                        ):
+                            singing_track.edited_params.pitch.points.root.extend(pitch_points)
+        return track_list
+
+    @staticmethod
+    def parse_volume(gain: float) -> float:
+        if gain >= 0:
+            return min(gain / (ratio_to_db(4)) + 1.0, 2.0)
+        else:
+            return db_to_float(gain)
+
+    @staticmethod
+    def parse_notes(notes: list[TuneLabNote], offset: int) -> list[Note]:
+        return [
+            Note(
+                start_pos=tlp_note.pos + offset,
+                length=tlp_note.dur,
+                key_number=tlp_note.pitch,
+                lyric=tlp_note.lyric,
+                pronunciation=tlp_note.pronunciation,
             )
-            for tempo in tempos
+            for tlp_note in notes
         ]
-        return skip_tempo_list(tempo_list, tick_prefix)
 
-    def parse_singing_tracks(
-        self,
-        vs_tracks: VsqxVsTrackList,
-        vs_units: VsqxVsUnitList,
-        tick_prefix: int,
-        measure_prefix: int,
-    ) -> list[SingingTrack]:
-        singing_tracks = []
-        for vs_track, vs_unit in zip(vs_tracks, vs_units):
-            singing_track = SingingTrack(
-                title=vs_track.track_name, mute=vs_unit.mute, solo=vs_unit.solo
+    @staticmethod
+    def vibrato_value(seconds: float, vibrato_start: float, vibrato: TuneLabVibrato) -> float:
+        return (
+            math.sin(math.pi * (2 * (seconds - vibrato_start) * vibrato.frequency - vibrato.phase))
+            * vibrato.amplitude
+        )
+
+    def parse_vibrato(
+        self, part: TuneLabMidiPart
+    ) -> tuple[PiecewiseIntervalDict, PiecewiseIntervalDict]:
+        vibrato_base_interval_dict = PiecewiseIntervalDict()
+        vibrato_envelope_interval_dict = PiecewiseIntervalDict()
+        for vibrato in part.vibratos:
+            vibrato_start = self.synchronizer.get_actual_secs_from_ticks(int(vibrato.pos))
+            vibrato_end = self.synchronizer.get_actual_secs_from_ticks(
+                int(vibrato.pos + vibrato.dur)
+            )
+            vibrato_base_interval_dict[portion.closed(vibrato_start, vibrato_end)] = (
+                functools.partial(self.vibrato_value, vibrato_start=vibrato_start, vibrato=vibrato)
             )
-            for musical_part in vs_track.musical_part:
-                note_list = self.parse_notes(musical_part.note, musical_part.pos_tick - tick_prefix)
-                singing_track.note_list.extend(note_list)
-                if (
-                    not singing_track.ai_singer_name
-                    and musical_part.singer
-                    and (v_voice := self.pc2voice.get(musical_part.singer[0].v_pc))
-                    and v_voice.v_voice_name is not None
-                ):
-                    singing_track.ai_singer_name = v_voice.v_voice_name
-                if self.options.import_pitch and (
-                    pitch := self.parse_pitch(
-                        musical_part,
-                        note_list,
-                        tick_prefix,
+        if part.automations is not None and part.automations.vibrato_envelope is not None:
+            for value, ticks_group in more_itertools.groupby_transform(
+                part.automations.vibrato_envelope.values.root,
+                keyfunc=operator.attrgetter("value"),
+                valuefunc=operator.attrgetter("pos"),
+            ):
+                ticks_group = list(ticks_group)
+                group_start = self.synchronizer.get_actual_secs_from_ticks(int(ticks_group[0]))
+                group_end = self.synchronizer.get_actual_secs_from_ticks(int(ticks_group[-1] + 5))
+                vibrato_envelope_interval_dict[
+                    portion.closedopen(
+                        group_start,
+                        group_end,
                     )
-                ):
-                    singing_track.edited_params.pitch.points.extend(pitch.points)
-            if len(singing_track.edited_params.pitch.points.root):
-                singing_track.edited_params.pitch.points.root.insert(0, Point.start_point())
-                singing_track.edited_params.pitch.points.root.append(Point.end_point())
-            singing_tracks.append(singing_track)
-        return singing_tracks
-
-    def parse_notes(self, vsqx_notes: list[VsqxNote], tick_offset: int) -> list[Note]:
-        prev_vsqx_note = None
-        note_list: list[Note] = []
-        for vsqx_note in vsqx_notes:
-            if prev_vsqx_note and vsqx_note.lyric.startswith("EVEC("):
-                note_list[-1].length += vsqx_note.dur_tick
-                continue
-            elif vsqx_note.phnms is None or vsqx_note.phnms.value not in ["Asp", "Sil", "?"]:
-                note = Note(
-                    start_pos=vsqx_note.pos_tick + tick_offset,
-                    length=vsqx_note.dur_tick,
-                    lyric=(vsqx_note.lyric or DEFAULT_ENGLISH_LYRIC).lower(),
-                    pronunciation=vsqx_note.phnms.value
-                    if (vsqx_note.phnms is not None and vsqx_note.phnms.lock == 1)
-                    else None,
-                    key_number=vsqx_note.note_num,
-                )
-                if (
-                    prev_vsqx_note is not None
-                    and prev_vsqx_note.phnms is not None
-                    and prev_vsqx_note.pos_tick + prev_vsqx_note.dur_tick == vsqx_note.pos_tick
-                    and prev_vsqx_note.phnms.value == "Sil"
-                ):
-                    note.head_tag = "0"
-                note_list.append(note)
-            prev_vsqx_note = vsqx_note
-        return note_list
+                ] = max(value + 1, 0)
+        return vibrato_base_interval_dict, vibrato_envelope_interval_dict
 
     def parse_pitch(
-        self, musical_part: VsqxMusicalPart, note_list: list[Note], tick_offset: int
-    ) -> Optional[ParamCurve]:
-        pitch_data = VocaloidPartPitchData(
-            start_pos=musical_part.pos_tick - tick_offset,
-            pit=[
-                ControllerEvent(
-                    pos=music_control.pos_tick,
-                    value=music_control.attr.value,
-                )
-                for music_control in musical_part.m_ctrl
-                if music_control.attr.type_param_attr_id == self.param_names.PIT.value
-                and music_control.attr.value is not None
-            ],
-            pbs=[
-                ControllerEvent(
-                    pos=music_control.pos_tick,
-                    value=music_control.attr.value,
-                )
-                for music_control in musical_part.m_ctrl
-                if music_control.attr.type_param_attr_id == self.param_names.PBS.value
-                and music_control.attr.value is not None
-            ],
-        )
-        return pitch_from_vocaloid_parts(
-            [pitch_data],
-            note_list,
-            self.first_bar_length,
-            musical_part.pos_tick - tick_offset,
-            musical_part.pos_tick + musical_part.play_time - tick_offset,
-        )
-
-    def parse_instrumental_tracks(
         self,
-        wav_parts: VsqxWavPartList,
-        wav_units: VsqxWavUnitList,
-        tick_prefix: int,
-    ) -> list[InstrumentalTrack]:
-        instrumental_tracks = []
-        if self.options.import_instrumental_track:
-            for wav_part, wav_unit in zip(wav_parts, wav_units):
-                if pathlib.Path(wav_part.file_path).is_absolute():
-                    wav_path_str = wav_part.file_path
-                elif (
-                    wav_path := self.src_path.with_suffix(".wavparts") / wav_part.file_path
-                ).exists():
-                    wav_path_str = str(wav_path)
-                else:
-                    continue
-                instrumental_tracks.append(
-                    InstrumentalTrack(
-                        title=wav_part.part_name,
-                        audio_file_path=wav_path_str,
-                        offset=wav_part.pos_tick - tick_prefix,
-                        mute=wav_unit.mute,
-                        solo=wav_unit.solo,
+        pitch: list[TuneLabPoints],
+        offset: int,
+        vibrato_base_interval_dict: PiecewiseIntervalDict,
+        vibrato_envelope_interval_dict: PiecewiseIntervalDict,
+    ) -> list[Point]:
+        points: list[Point] = []
+        for pitch_part in pitch:
+            for is_first, is_last, tlp_point in more_itertools.mark_ends(pitch_part.root):
+                pitch_pos = int(tlp_point.pos) + offset
+                if is_first:
+                    points.append(
+                        Point(
+                            x=pitch_pos + self.first_bar_length,
+                            y=-100,
+                        )
+                    )
+                pitch_secs = self.synchronizer.get_actual_secs_from_ticks(pitch_pos)
+                pitch_value = tlp_point.value
+                if (vibrato_value := vibrato_base_interval_dict.get(pitch_secs)) is not None:
+                    vibrato_value *= vibrato_envelope_interval_dict.get(pitch_secs, 1)
+                    pitch_value += vibrato_value
+                points.append(
+                    Point(
+                        x=pitch_pos + self.first_bar_length,
+                        y=round(pitch_value * 100),
                     )
                 )
-        return instrumental_tracks
+                if is_last:
+                    points.append(
+                        Point(
+                            x=points[-1].x,
+                            y=-100,
+                        )
+                    )
+        return points
```

### Comparing `libresvip-1.1.2/libresvip/plugins/y77/model.py` & `libresvip-1.1.3/libresvip/plugins/y77/model.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/y77/y77.yapsy-plugin` & `libresvip-1.1.3/libresvip/plugins/y77/y77.yapsy-plugin`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/y77/y77_converter.py` & `libresvip-1.1.3/libresvip/plugins/y77/y77_converter.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/y77/y77_generator.py` & `libresvip-1.1.3/libresvip/plugins/y77/y77_generator.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/plugins/y77/y77_parser.py` & `libresvip-1.1.3/libresvip/plugins/y77/y77_parser.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/res/libresvip.ico` & `libresvip-1.1.3/libresvip/res/libresvip.ico`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/res/locales/zh_CN/LC_MESSAGES/libresvip.mo` & `libresvip-1.1.3/libresvip/res/locales/zh_CN/LC_MESSAGES/libresvip.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  libresvip\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-05-06 21:06+0800\n"
-"PO-Revision-Date: 2024-05-06 13:31+0000\n"
+"PO-Revision-Date: 2024-05-18 03:49+0000\n"
 "Last-Translator: \n"
 "Language: zh_CN\n"
 "Language-Team: Chinese Simplified\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -668,15 +668,15 @@
 msgid "File successfully converted"
 msgstr "此文件已成功转换"
 
 msgid "Fill short rests"
 msgstr "填充短休止符"
 
 msgid "Flags"
-msgstr "标记"
+msgstr "修饰符"
 
 msgid "Folder Presets"
 msgstr "文件夹预设"
 
 msgid "For Chinese and Japanese Lyrics"
 msgstr "仅限中文及日文歌词"
```

### Comparing `libresvip-1.1.2/libresvip/utils/audio.py` & `libresvip-1.1.3/libresvip/utils/audio.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/module_loading.py` & `libresvip-1.1.3/libresvip/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/music_math.py` & `libresvip-1.1.3/libresvip/utils/music_math.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/search.py` & `libresvip-1.1.3/libresvip/utils/search.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/text.py` & `libresvip-1.1.3/libresvip/utils/text.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/translation.py` & `libresvip-1.1.3/libresvip/utils/translation.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/xmlutils/__init__.py` & `libresvip-1.1.3/libresvip/utils/xmlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/xmlutils/native.py` & `libresvip-1.1.3/libresvip/utils/xmlutils/native.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/yamlutils/__init__.py` & `libresvip-1.1.3/libresvip/utils/yamlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/yamlutils/common.py` & `libresvip-1.1.3/libresvip/utils/yamlutils/common.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/yamlutils/dumper.py` & `libresvip-1.1.3/libresvip/utils/yamlutils/dumper.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/utils/yamlutils/loader.py` & `libresvip-1.1.3/libresvip/utils/yamlutils/loader.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/web/elements.py` & `libresvip-1.1.3/libresvip/web/elements.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/libresvip/web/pages.py` & `libresvip-1.1.3/libresvip/web/pages.py`

 * *Files identical despite different names*

### Comparing `libresvip-1.1.2/pyproject.toml` & `libresvip-1.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -35,67 +35,67 @@
     "jinja2<4.0.0,>=3.1.4",
     "loguru<1.0.0,>=0.7.2",
     "mido-fix<2.0.0,>=1.2.12",
     "more-itertools<11.0.0,>=10.2.0",
     "omegaconf<3.0.0,>=2.3.0",
     "packaging<24.1,>=24.0",
     "parsimonious<0.11.0,>=0.10.0",
-    "platformdirs<5.0.0,>=4.2.1",
+    "platformdirs<5.0.0,>=4.2.2",
     "portion<3.0.0,>=2.4.2",
     "proto-plus<2.0.0,>=1.23.0",
     "pydantic<3.0.0,>=2.7.1",
     "pydantic-extra-types<3.0.0,>=2.7.0",
     "pymediainfo<7.0.0,>=6.1.0",
     "pypinyin<1.0.0,>=0.51.0",
     "retrie<1.0.0,>=0.3.1",
     "rich<14.0.0,>=13.7.1",
     "srt<4.0.0,>=3.5.3",
     "typer-slim<1.0.0,>=0.12.3",
     "wanakana-python<2.0.0,>=1.2.2",
-    "xsdata<24.5,>=24.4",
+    "xsdata<24.6,>=24.5",
     "zhon<3.0.0,>=2.0.2",
     "zstandard<0.23.0,>=0.22.0; platform_python_implementation == \"CPython\"",
     "zstd<2.0.0,>=1.5.5.1; platform_python_implementation == \"PyPy\"",
 ]
 name = "libresvip"
 dynamic = []
 description = "Universal Converter for Singing Voice Projects"
 readme = "README.md"
-version = "1.1.2"
+version = "1.1.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/SoulMelody/LibreSVIP"
 documentation = "https://soulmelody.github.io/LibreSVIP"
 
 [project.optional-dependencies]
 ujson = [
-    "ujson>=5.9.0",
+    "ujson>=5.10.0",
 ]
 upath = [
     "universal-pathlib<1.0.0,>=0.2.2",
 ]
 ruamel_yaml = [
     "ruamel.yaml>=0.18.6",
 ]
 lxml = [
-    "lxml>=5.2.1",
+    "lxml>=5.2.2",
 ]
 webui = [
-    "nicegui>=1.4.24",
+    "nicegui>=1.4.25",
     "pywebview>=5.1",
     "libresvip[upath]",
 ]
 desktop = [
     "pyside6<6.8.0,>=6.6.3.1,!=6.7.0",
     "fonticon-materialdesignicons7>=7.2.96",
     "httpx>=0.27.0",
-    "desktop-notifier>=3.5.6; platform_python_implementation == \"CPython\"",
+    "desktop-notifier>=4.0.0; platform_python_implementation == \"CPython\"",
     "libresvip[upath]",
 ]
 
 [project.scripts]
 libresvip-cli = "libresvip.cli.__main__:app"
 libresvip-web = "libresvip.web.__main__:main"
 
@@ -105,42 +105,42 @@
 [tool.pdm.version]
 source = "file"
 path = "libresvip/__init__.py"
 
 [tool.pdm.dev-dependencies]
 code_gen = [
     "datamodel-code-generator>=0.25.6",
-    "gapic-generator>=1.17.1",
+    "gapic-generator>=1.18.0",
     "click-default-group>=1.2.4",
     "docformatter>=1.7.5",
     "toposort>=1.10",
 ]
 i18n = [
     "translate-toolkit>=3.13.0",
     "babel>=2.15.0",
 ]
 linting = [
-    "pre-commit>=3.7.0",
-    "ruff>=0.4.3",
+    "pre-commit>=3.7.1",
+    "ruff>=0.4.4",
     "mypy>=1.10.0",
-    "sourcery>=1.16.0",
+    "sourcery>=1.18.0",
     "proto-plus-stubs>=0.7.0",
     "types-parsimonious>=0.10.0.20240331",
     "types-pyyaml>=6.0.12.20240311",
-    "types-ujson>=5.9.0.0",
+    "types-ujson>=5.10.0.20240515",
     "types-zstd>=1.5.0.20240311; platform_python_implementation == \"PyPy\"",
 ]
 packaging = [
     "cx-Freeze>=7.0.0",
-    "nuitka>=2.2.1",
+    "nuitka>=2.2.3",
     "pyinstaller>=6.6.0",
     "shellingham<2.0.0,>=1.5.4",
 ]
 docs = [
-    "mkdocs-material<10.0.0,>=9.5.21",
+    "mkdocs-material<10.0.0,>=9.5.23",
 ]
 test = [
     "pytest>=8.2.0",
     "pytest-datadir>=1.5.0",
 ]
 
 [tool.pdm.build]
```

### Comparing `libresvip-1.1.2/PKG-INFO` & `libresvip-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libresvip
-Version: 1.1.2
+Version: 1.1.3
 Summary: Universal Converter for Singing Voice Projects
 Author-Email: SoulMelody <yjxrtzyx@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
@@ -36,41 +36,41 @@
 Requires-Dist: jinja2<4.0.0,>=3.1.4
 Requires-Dist: loguru<1.0.0,>=0.7.2
 Requires-Dist: mido-fix<2.0.0,>=1.2.12
 Requires-Dist: more-itertools<11.0.0,>=10.2.0
 Requires-Dist: omegaconf<3.0.0,>=2.3.0
 Requires-Dist: packaging<24.1,>=24.0
 Requires-Dist: parsimonious<0.11.0,>=0.10.0
-Requires-Dist: platformdirs<5.0.0,>=4.2.1
+Requires-Dist: platformdirs<5.0.0,>=4.2.2
 Requires-Dist: portion<3.0.0,>=2.4.2
 Requires-Dist: proto-plus<2.0.0,>=1.23.0
 Requires-Dist: pydantic<3.0.0,>=2.7.1
 Requires-Dist: pydantic-extra-types<3.0.0,>=2.7.0
 Requires-Dist: pymediainfo<7.0.0,>=6.1.0
 Requires-Dist: pypinyin<1.0.0,>=0.51.0
 Requires-Dist: retrie<1.0.0,>=0.3.1
 Requires-Dist: rich<14.0.0,>=13.7.1
 Requires-Dist: srt<4.0.0,>=3.5.3
 Requires-Dist: typer-slim<1.0.0,>=0.12.3
 Requires-Dist: wanakana-python<2.0.0,>=1.2.2
-Requires-Dist: xsdata<24.5,>=24.4
+Requires-Dist: xsdata<24.6,>=24.5
 Requires-Dist: zhon<3.0.0,>=2.0.2
 Requires-Dist: zstandard<0.23.0,>=0.22.0; platform_python_implementation == "CPython"
 Requires-Dist: zstd<2.0.0,>=1.5.5.1; platform_python_implementation == "PyPy"
-Requires-Dist: ujson>=5.9.0; extra == "ujson"
+Requires-Dist: ujson>=5.10.0; extra == "ujson"
 Requires-Dist: universal-pathlib<1.0.0,>=0.2.2; extra == "upath"
 Requires-Dist: ruamel.yaml>=0.18.6; extra == "ruamel-yaml"
-Requires-Dist: lxml>=5.2.1; extra == "lxml"
-Requires-Dist: nicegui>=1.4.24; extra == "webui"
+Requires-Dist: lxml>=5.2.2; extra == "lxml"
+Requires-Dist: nicegui>=1.4.25; extra == "webui"
 Requires-Dist: pywebview>=5.1; extra == "webui"
 Requires-Dist: libresvip[upath]; extra == "webui"
 Requires-Dist: pyside6!=6.7.0,<6.8.0,>=6.6.3.1; extra == "desktop"
 Requires-Dist: fonticon-materialdesignicons7>=7.2.96; extra == "desktop"
 Requires-Dist: httpx>=0.27.0; extra == "desktop"
-Requires-Dist: desktop-notifier>=3.5.6; platform_python_implementation == "CPython" and extra == "desktop"
+Requires-Dist: desktop-notifier>=4.0.0; platform_python_implementation == "CPython" and extra == "desktop"
 Requires-Dist: libresvip[upath]; extra == "desktop"
 Provides-Extra: ujson
 Provides-Extra: upath
 Provides-Extra: ruamel-yaml
 Provides-Extra: lxml
 Provides-Extra: webui
 Provides-Extra: desktop
```

