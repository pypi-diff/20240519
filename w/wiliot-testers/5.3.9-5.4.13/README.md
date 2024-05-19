# Comparing `tmp/wiliot-testers-5.3.9.tar.gz` & `tmp/wiliot-testers-5.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-testers-5.3.9.tar", last modified: Sun Feb 11 08:59:18 2024, max compression
+gzip compressed data, was "wiliot-testers-5.4.13.tar", last modified: Sun May 19 06:54:21 2024, max compression
```

## Comparing `wiliot-testers-5.3.9.tar` & `wiliot-testers-5.4.13.tar`

### file list

```diff
@@ -1,139 +1,155 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)    10658 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10154 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7595 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      332 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2138 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.044051 wiliot-testers-5.3.9/wiliot_testers/
--rw-rw-rw-   0 root         (0) root         (0)    10654 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/API_README.md
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.048051 wiliot-testers-5.3.9/wiliot_testers/calibration_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/calibration_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20924 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/calibration_test/calibration_test.py
--rw-rw-rw-   0 root         (0) root         (0)    25311 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/calibration_test/calibration_test_by_tbp.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.048051 wiliot-testers-5.3.9/wiliot_testers/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/config/equipment_config.json
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/config/unusable_inlays.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.048051 wiliot-testers-5.3.9/wiliot_testers/docs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    72970 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/docs/tester_api_flow.pdf
--rw-rw-rw-   0 root         (0) root         (0)     4818 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/docs/wiliot_logo.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.048051 wiliot-testers-5.3.9/wiliot_testers/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/examples/wiliot_tester_example.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.048051 wiliot-testers-5.3.9/wiliot_testers/offline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.048051 wiliot-testers-5.3.9/wiliot_testers/offline/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6173 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/configs/global_vars_and_enums.py
--rw-rw-rw-   0 root         (0) root         (0)    14239 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/configs/moh_instruction.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/configs/tests_suites.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.048051 wiliot-testers-5.3.9/wiliot_testers/offline/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18396 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/modules/offline_log.py
--rw-rw-rw-   0 root         (0) root         (0)    49951 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/modules/offline_printing_and_validation.py
--rw-rw-rw-   0 root         (0) root         (0)    19361 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/modules/offline_tag_testing.py
--rw-rw-rw-   0 root         (0) root         (0)    51764 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/modules/offline_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    45066 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/offline_main.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/run_barcode_testing.bat
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/run_offline_tester.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.052051 wiliot-testers-5.3.9/wiliot_testers/offline/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4708 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/utils/barcode_test.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/utils/env_install.bat
--rw-rw-rw-   0 root         (0) root         (0)     9005 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/utils/env_install.py
--rw-rw-rw-   0 root         (0) root         (0)     3624 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/utils/offline_log_editing.py
--rw-rw-rw-   0 root         (0) root         (0)     8729 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/offline/utils/tadbik_r2r_controller.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.052051 wiliot-testers-5.3.9/wiliot_testers/partners/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/partners/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.052051 wiliot-testers-5.3.9/wiliot_testers/partners/avery_dennison/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/partners/avery_dennison/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.052051 wiliot-testers-5.3.9/wiliot_testers/partners/avery_dennison/configs/
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/partners/avery_dennison/configs/test_suite_example.json
--rw-rw-rw-   0 root         (0) root         (0)    27489 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/partners/avery_dennison/simple_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/partners/avery_dennison/test_upload_get_AD.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.052051 wiliot-testers-5.3.9/wiliot_testers/sample/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42685 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/com_connect.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.052051 wiliot-testers-5.3.9/wiliot_testers/sample/configs/
--rw-rw-rw-   0 root         (0) root         (0)      121 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/configs/.default_surfaces.json
--rw-rw-rw-   0 root         (0) root         (0)     2364 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/configs/.default_test_configs.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12210 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/configs_gui.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/get_temperature_sensor_name.py
--rw-rw-rw-   0 root         (0) root         (0)    37369 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/sample_chamber.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/sample_test.bat
--rw-rw-rw-   0 root         (0) root         (0)    87954 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/sample_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.052051 wiliot-testers-5.3.9/wiliot_testers/sample/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22413 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/com_connect.ui
--rw-rw-rw-   0 root         (0) root         (0)     1153 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/comm.gif
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/configs.gif
--rw-rw-rw-   0 root         (0) root         (0)    18323 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/configs.ui
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/edit.gif
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/refresh.gif
--rw-rw-rw-   0 root         (0) root         (0)     3213 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/reset.png
--rw-rw-rw-   0 root         (0) root         (0)    23842 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/sample_test.ui
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/save.png
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sample/utils/wiliot3.gif
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/wiliot_testers/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4373 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sensors/get_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4449 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sensors/get_temperature.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/sensors/light_sensor_calibration.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/wiliot_testers/system_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/system_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    45287 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/system_test/harvester_test.py
--rw-rw-rw-   0 root         (0) root         (0)    73280 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/system_test/system_test_example.py
--rw-rw-rw-   0 root         (0) root         (0)    58430 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/test_equipment.py
--rw-rw-rw-   0 root         (0) root         (0)    66254 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/tester_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/upload_testers_data.bat
--rw-rw-rw-   0 root         (0) root         (0)    15882 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/upload_testers_data_to_cloud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/wiliot_testers/utils/
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/utils/Install PPFP.bat
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6048 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)    10217 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/utils/ppfp_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     8840 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/utils/upload_to_cloud_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4729 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/utils/wiliot_external_ids.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-02-11 08:59:17.000000 wiliot-testers-5.3.9/wiliot_testers/version.py
--rw-rw-rw-   0 root         (0) root         (0)    11339 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/wiliot_tester_log.py
--rw-rw-rw-   0 root         (0) root         (0)    19055 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/wiliot_tester_tag_result.py
--rw-rw-rw-   0 root         (0) root         (0)    65894 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/wiliot_tester_tag_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/wiliot_testers/yield_tester/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/wiliot_testers/yield_tester/arduino_counter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/arduino_counter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/arduino_counter/arduino_counter.ino
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/wiliot_testers/yield_tester/configs/
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/configs/.default_configs.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1394 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/configs/inlay_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4573 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/count_thread.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/from_listener_log_to_csv.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/run_yield_tester.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/wiliot_testers/yield_tester/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/simulation/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/wiliot_testers/yield_tester/simulation/gw_arduino_simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/simulation/gw_arduino_simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2186 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/simulation/gw_arduino_simulation/gw_arduino_simulation.ino
--rw-rw-rw-   0 root         (0) root         (0)     4662 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/simulation/yield_simulation_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5894 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/trigger_miss_catcher.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.056051 wiliot-testers-5.3.9/wiliot_testers/yield_tester/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4217 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/utils/get_arduino_ports.py
--rw-rw-rw-   0 root         (0) root         (0)    61768 2024-02-11 08:59:02.000000 wiliot-testers-5.3.9/wiliot_testers/yield_tester/yield_tester.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-11 08:59:18.048051 wiliot-testers-5.3.9/wiliot_testers.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    10658 2024-02-11 08:59:17.000000 wiliot-testers-5.3.9/wiliot_testers.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4689 2024-02-11 08:59:17.000000 wiliot-testers-5.3.9/wiliot_testers.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-11 08:59:17.000000 wiliot-testers-5.3.9/wiliot_testers.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-11 08:59:17.000000 wiliot-testers-5.3.9/wiliot_testers.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-02-11 08:59:17.000000 wiliot-testers-5.3.9/wiliot_testers.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-11 08:59:17.000000 wiliot-testers-5.3.9/wiliot_testers.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.069631 wiliot-testers-5.4.13/
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    11857 2024-05-19 06:54:21.069631 wiliot-testers-5.4.13/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11352 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7595 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      332 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-19 06:54:21.069631 wiliot-testers-5.4.13/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2140 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.053631 wiliot-testers-5.4.13/wiliot_testers/
+-rw-rw-rw-   0 root         (0) root         (0)    10654 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/API_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.053631 wiliot-testers-5.4.13/wiliot_testers/association_tester/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/association_tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4011 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/association_tester/association_and_verification_tester.py
+-rw-rw-rw-   0 root         (0) root         (0)    12561 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/association_tester/association_module.py
+-rw-rw-rw-   0 root         (0) root         (0)    12927 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/association_tester/performance_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     5836 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/association_tester/r2r_component.py
+-rw-rw-rw-   0 root         (0) root         (0)     5211 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/association_tester/scanner_component.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.053631 wiliot-testers-5.4.13/wiliot_testers/calibration_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/calibration_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20924 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/calibration_test/calibration_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    25311 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/calibration_test/calibration_test_by_tbp.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.053631 wiliot-testers-5.4.13/wiliot_testers/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/config/equipment_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/config/unusable_inlays.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.053631 wiliot-testers-5.4.13/wiliot_testers/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    72970 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/docs/tester_api_flow.pdf
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/docs/wiliot_logo.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.053631 wiliot-testers-5.4.13/wiliot_testers/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/examples/wiliot_tester_example.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.057631 wiliot-testers-5.4.13/wiliot_testers/offline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.057631 wiliot-testers-5.4.13/wiliot_testers/offline/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6698 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/configs/global_vars_and_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)    14229 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/configs/moh_instruction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/configs/tests_suites.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.057631 wiliot-testers-5.4.13/wiliot_testers/offline/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18992 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/modules/offline_log.py
+-rw-rw-rw-   0 root         (0) root         (0)    49983 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/modules/offline_printing_and_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/modules/offline_r2r_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    25924 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/modules/offline_tag_testing.py
+-rw-rw-rw-   0 root         (0) root         (0)    52795 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/modules/offline_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    46605 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/offline_main.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/run_barcode_testing.bat
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/run_offline_tester.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.057631 wiliot-testers-5.4.13/wiliot_testers/offline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4708 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/utils/barcode_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/utils/env_install.bat
+-rw-rw-rw-   0 root         (0) root         (0)     9005 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/utils/env_install.py
+-rw-rw-rw-   0 root         (0) root         (0)     3624 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/utils/offline_log_editing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8729 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/offline/utils/tadbik_r2r_controller.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.057631 wiliot-testers-5.4.13/wiliot_testers/partners/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/partners/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.057631 wiliot-testers-5.4.13/wiliot_testers/partners/simple_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/partners/simple_test/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.057631 wiliot-testers-5.4.13/wiliot_testers/partners/simple_test/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/partners/simple_test/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/partners/simple_test/configs/test_suite_example.json
+-rw-rw-rw-   0 root         (0) root         (0)    27489 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/partners/simple_test/simple_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4527 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/partners/simple_test/test_upload_get_results.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.061631 wiliot-testers-5.4.13/wiliot_testers/sample/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43810 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/com_connect.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.061631 wiliot-testers-5.4.13/wiliot_testers/sample/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/configs/.default_surfaces.json
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/configs/.default_test_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12355 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/configs_gui.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.061631 wiliot-testers-5.4.13/wiliot_testers/sample/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9235 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/modules/resolve_packets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10003 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/modules/wiliot_sample_tag_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    37368 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/sample_chamber.py
+-rw-rw-rw-   0 root         (0) root         (0)     8533 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/sample_slim.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/sample_test.bat
+-rw-rw-rw-   0 root         (0) root         (0)    69664 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/sample_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.061631 wiliot-testers-5.4.13/wiliot_testers/sample/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22446 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/com_connect.ui
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/comm.gif
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/configs.gif
+-rw-rw-rw-   0 root         (0) root         (0)    18347 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/configs.ui
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/edit.gif
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/refresh.gif
+-rw-rw-rw-   0 root         (0) root         (0)     3213 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/reset.png
+-rw-rw-rw-   0 root         (0) root         (0)    23899 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/sample_test.ui
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/save.png
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sample/utils/wiliot3.gif
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.065631 wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/config_attenuators.bat
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/config_attenuators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4373 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/get_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/get_temperature.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/get_temperature_sensor_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4740 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/light_sensor_calibration.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.065631 wiliot-testers-5.4.13/wiliot_testers/system_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/system_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19659 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/system_test/beacon_power_calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)    45361 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/system_test/harvester_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    73280 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/system_test/system_test_example.py
+-rw-rw-rw-   0 root         (0) root         (0)    60553 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/test_equipment.py
+-rw-rw-rw-   0 root         (0) root         (0)    66254 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/tester_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/upload_testers_data.bat
+-rw-rw-rw-   0 root         (0) root         (0)    15882 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/upload_testers_data_to_cloud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.065631 wiliot-testers-5.4.13/wiliot_testers/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/utils/Install PPFP.bat
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6048 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    10217 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/utils/ppfp_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     8840 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/utils/upload_to_cloud_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4729 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/utils/wiliot_external_ids.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-19 06:54:20.000000 wiliot-testers-5.4.13/wiliot_testers/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    11313 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/wiliot_tester_log.py
+-rw-rw-rw-   0 root         (0) root         (0)    19095 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/wiliot_tester_tag_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    66533 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/wiliot_tester_tag_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.065631 wiliot-testers-5.4.13/wiliot_testers/yield_tester/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.065631 wiliot-testers-5.4.13/wiliot_testers/yield_tester/arduino_counter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/arduino_counter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/arduino_counter/arduino_counter.ino
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.065631 wiliot-testers-5.4.13/wiliot_testers/yield_tester/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/configs/.default_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/configs/inlay_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/from_listener_log_to_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/run_yield_tester.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.065631 wiliot-testers-5.4.13/wiliot_testers/yield_tester/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/simulation/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.065631 wiliot-testers-5.4.13/wiliot_testers/yield_tester/simulation/gw_arduino_simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/simulation/gw_arduino_simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2186 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/simulation/gw_arduino_simulation/gw_arduino_simulation.ino
+-rw-rw-rw-   0 root         (0) root         (0)     4662 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/simulation/yield_simulation_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5894 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/trigger_miss_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.065631 wiliot-testers-5.4.13/wiliot_testers/yield_tester/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4217 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/utils/get_arduino_ports.py
+-rw-rw-rw-   0 root         (0) root         (0)    59396 2024-05-19 06:54:04.000000 wiliot-testers-5.4.13/wiliot_testers/yield_tester/yield_tester.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 06:54:21.053631 wiliot-testers-5.4.13/wiliot_testers.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11857 2024-05-19 06:54:20.000000 wiliot-testers-5.4.13/wiliot_testers.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5510 2024-05-19 06:54:20.000000 wiliot-testers-5.4.13/wiliot_testers.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-19 06:54:20.000000 wiliot-testers-5.4.13/wiliot_testers.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-19 06:54:20.000000 wiliot-testers-5.4.13/wiliot_testers.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-05-19 06:54:20.000000 wiliot-testers-5.4.13/wiliot_testers.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-19 06:54:20.000000 wiliot-testers-5.4.13/wiliot_testers.egg-info/top_level.txt
```

### Comparing `wiliot-testers-5.3.9/.gitignore` & `wiliot-testers-5.4.13/.gitignore`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/LICENSE` & `wiliot-testers-5.4.13/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/PKG-INFO` & `wiliot-testers-5.4.13/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-testers
-Version: 5.3.9
+Version: 5.4.13
 Summary: A library for interacting with Wiliot's Testers app
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,48 @@
 * [Yield Tester](wiliot_testers/yield_tester/yield_tester.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 5.4.13:
+-----------------
+    
+* tester SDK:
+    * raise exception if bad gateway configuration occurs
+    * even if test stopped by the user, first update and analyze results and then exit the test
+    * if fail bin was set outside the test, all functions should be updated accordingly
+    
+* sensors and hardware:
+    * improve light sensor calibration
+    * added a script to configure attenuator
+    * added beacons power calibration for chambers
+    
+* test equipment:
+    * improve chamber handling
+    * add more options to work with Cognex scanner
+    
+* offline tester
+    * added support for GW gpio new functionalities and control PLC using GW only
+    * added support to more external sensors
+    * added support to handle duplication if tag was not printed yet
+    * added support to label missing label case
+    
+* sample test
+    * new architecture for sample test including adding sample test sdk class based on the tester sdk.
+    * added a resolver class to get external id from packet based on api key
+    
+    
+* yield-tester:
+    * add support to clout wafer matrix using the GW and not Arduino.
+    * update graph and labels
+    * fix bug in temperature calculation
+
+
 Version 5.3.9:
 -----------------
 * offline tester: HOTFIX for running without printing
 
 Version 5.3.8:
 -----------------
 * offline tester: HOTFIX for printer communication
```

### Comparing `wiliot-testers-5.3.9/README.md` & `wiliot-testers-5.4.13/wiliot_testers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: wiliot-testers
+Version: 5.4.13
+Summary: A library for interacting with Wiliot's Testers app
+Home-page: UNKNOWN
+Author: Wiliot
+Author-email: support@wiliot.com
+License: MIT
+Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyWiliot: wiliot-testers #
 
 wiliot-testers is a python library for accessing Wiliot's Testers scripts
 
 ## Public Library
 
 ### MAC Installation
@@ -40,14 +57,48 @@
 * [Yield Tester](wiliot_testers/yield_tester/yield_tester.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 5.4.13:
+-----------------
+    
+* tester SDK:
+    * raise exception if bad gateway configuration occurs
+    * even if test stopped by the user, first update and analyze results and then exit the test
+    * if fail bin was set outside the test, all functions should be updated accordingly
+    
+* sensors and hardware:
+    * improve light sensor calibration
+    * added a script to configure attenuator
+    * added beacons power calibration for chambers
+    
+* test equipment:
+    * improve chamber handling
+    * add more options to work with Cognex scanner
+    
+* offline tester
+    * added support for GW gpio new functionalities and control PLC using GW only
+    * added support to more external sensors
+    * added support to handle duplication if tag was not printed yet
+    * added support to label missing label case
+    
+* sample test
+    * new architecture for sample test including adding sample test sdk class based on the tester sdk.
+    * added a resolver class to get external id from packet based on api key
+    
+    
+* yield-tester:
+    * add support to clout wafer matrix using the GW and not Arduino.
+    * update graph and labels
+    * fix bug in temperature calculation
+
+
 Version 5.3.9:
 -----------------
 * offline tester: HOTFIX for running without printing
 
 Version 5.3.8:
 -----------------
 * offline tester: HOTFIX for printer communication
@@ -230,7 +281,9 @@
 Version 4.0.0:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
 for more information please read 'wiliot' package's release notes
+
+
```

### Comparing `wiliot-testers-5.3.9/bitbucket-pipelines.yml` & `wiliot-testers-5.4.13/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/setup.py` & `wiliot-testers-5.4.13/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,22 +31,22 @@
                  install_requires=[
                      'setuptools_scm',
                      'pyserial',
                      'yoctopuce',
                      'pandas',
                      'numpy<2',
                      'pyqtgraph',
-                     'PySimpleGUI',
+                     'PySimpleGUI<5',
                      'matplotlib',
                      'PyQt5-sip<12.13.0',
                      'PyQt5<5.15.10',
                      'pygubu==0.16',
                      'appdirs',
                      'pillow',
-                     'wiliot-api>=4.7.1',
-                     'wiliot-core>=5.4.3',
-                     'wiliot-tools>=4.4.4'
+                     'wiliot-api>=4.8.2',
+                     'wiliot-core>=5.5.8',
+                     'wiliot-tools>=4.5.4'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                  include_package_data=True,
                  )
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/API_README.md` & `wiliot-testers-5.4.13/wiliot_testers/API_README.md`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/__init__.py` & `wiliot-testers-5.4.13/wiliot_testers/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/calibration_test/calibration_test.py` & `wiliot-testers-5.4.13/wiliot_testers/calibration_test/calibration_test.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/calibration_test/calibration_test_by_tbp.py` & `wiliot-testers-5.4.13/wiliot_testers/calibration_test/calibration_test_by_tbp.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/docs/tester_api_flow.pdf` & `wiliot-testers-5.4.13/wiliot_testers/docs/tester_api_flow.pdf`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/docs/wiliot_logo.png` & `wiliot-testers-5.4.13/wiliot_testers/docs/wiliot_logo.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/examples/wiliot_tester_example.py` & `wiliot-testers-5.4.13/wiliot_testers/examples/wiliot_tester_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/configs/global_vars_and_enums.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/configs/global_vars_and_enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,18 +93,25 @@
     R2R_PULSE_DURATION = 50  # msec
     MAX_R2R_WAIT_TIME = 90  # being on the safe side since r2r can wait max 99 seconds
     EVENT_WAIT_TIME = 20  # the max time to wait for an event
     MIN_WAIT_TIME = 2  # time to wait for post run validation validation if stop is set
     MAX_TIME_BETWEEN_TESTS = 5  # the max time between the r2r movement and receiving the next trigger
     MAX_MAIN_STATES = 80
     PRINTER_90_DEG_WAIT_TIME = 1  # time to wait for the printer if running without scanning
-    PRINTER_90_DEG_WAIT_LSL = 0.5  # time to wait for the printer between getting PRC (print complete ack) and line selection
     TRIGGER_TYPE = 5  # relevant only for Cognex, 0: Single (external), 1: Presentation (internal), 2: Manual (button), 3: Burst (external), 4: Self (internal), 5: Continuous (external)
     R2R_START_OFFSET = 1    # When starting run then its starting from 1 and not 0
 
 
 # Configurations for offline_tag_testing.py
 class TagTestingDefaults:
     TIMEOUT_FOR_MISSING_LABEL = 5
-    TIME_BETWEEN_TEST_PRINTING = 2
+    TIME_BETWEEN_TEST_PRINTING = 3
     ENABLE_MISSING_LABEL = False
     MAX_MISSING_LABEL_ENGINEERING = 30
+    EVENT_WAIT_TIME = 1.5  # relevant only if GW control R2R: time to wait till printing and validation are done
+    MAX_R2R_WAIT_TIME = PrintingAndValidationDefaults.MAX_R2R_WAIT_TIME
+    POST_RUN_WAIT_TIME = 5  # relevant only if GW control R2R: time to wait for post run validation validation if stop is set
+    R2R_PULSE_DURATION = 50  # relevant only if GW control R2R: milliseconds
+    START_STOP_GPIO = 'P0.31'  # relevant only if GW control R2R
+    PASS_PULSE_GPIO = 'P0.29'  # relevant only if GW control R2R
+    FAIL_PULSE_GPIO = 'P0.30'  # relevant only if GW control R2R
+    MISSING_LABEL_GPIO = 'P1.00'  # relevant only if GW control R2R
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/configs/moh_instruction.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/configs/moh_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             "Please disconnect and reconnect Arduino and click continue after 5 second is alive"
         ],
         "Ru": [
             "Пожалуйста, отключите и снова подключите контроллер - "
             "Arduino и нажмите продолжить через 5 секунд после его включения"
         ],
         "He": [
-            "אנא נתק וחבר מחדש את הבקר - הארדואינו ולחץ על המשך 5 שניות לאחר שנדלק"
+            "אנא נתק וחבר מחדש את הבקר ה-Arduino ולחץ על המשך 5 שניות לאחר שנדלק"
         ]
     },
 
     "General Error": {
         "En": [
             "* Please make sure there are no empty tags after printer. If there are, please replace with faulty tags",
             "* If running with scanner, please make sure all passed tags were scanned by the scanner. "
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/configs/tests_suites.json` & `wiliot-testers-5.4.13/wiliot_testers/offline/configs/tests_suites.json`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/modules/offline_log.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/modules/offline_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 """
 
 import os
 import datetime
 import logging
 
 from wiliot_core import InlayTypes, WiliotDir
+
+from wiliot_testers.test_equipment import YoctoSensor
 from wiliot_testers.wiliot_tester_log import dict_to_csv, WiliotTesterLog
 from wiliot_testers.wiliot_tester_tag_test import TesterName
 from wiliot_testers.wiliot_tester_tag_result import ConversionTypes, SurfaceTypes, FailureCodes
 from wiliot_testers.utils.get_version import get_version
 from wiliot_testers.offline.modules.offline_printing_and_validation import ValidatedBin
 
 
@@ -177,25 +179,25 @@
                          'print_pass_job_name': self.log_config['passJobName'] if is_printing else '',
                          'printing_format': self.log_config['printingFormat'] if is_printing else '',
                          'external_id_prefix': self.log_config['stringBeforeCounter'] if is_printing else '',
                          'external_id_suffix_init_value': self.log_config['firstPrintingValue'] if is_printing else '',
                          'gw_version': gw_version,
                          'py_wiliot_version': get_version(),
                          'owner_id': 'wiliot-ops',
-                         'temperature_sensor_enable': self.log_config['temperatureSensorEnable'],
+                         'sensors_enable': self.log_config['sensorsEnable'],
                          'ttfp_avg': float('nan'),
                          'user_config_dict': self.log_config}
 
         self.test_data = {'common_run_name': common_run_name, 'tag_run_location': 0,
                           'total_test_duration': None,
                           'status_offline': False, 'fail_bin': FailureCodes.NONE.value,
                           'fail_bin_str': FailureCodes.NONE.name,
                           'external_id': '',
                           'label_validated': ValidatedBin.UNTESTED.name, 'trigger_time': None,
-                          'test_num': 0, 'temperature_sensor': float(-1),
+                          'test_num': 0,
                           'tag_reel_location': self.tag_reel_location}
 
         self.packet_headers_default = \
             ['common_run_name', 'tag_run_location', 'tag_reel_location', 'test_num', 'external_id', 'time_from_start',
              'raw_packet', 'rssi',
              'packet_status', 'adv_address', 'selected_tag', 'is_test_pass', 'status_offline', 'fail_bin',
              'fail_bin_str',
@@ -203,15 +205,15 @@
              'sprinkler_counter_min', 'sprinkler_counter_max', 'tbp_mean', 'tbp_std', 'tbp_min', 'tbp_max',
              'tbp_num_vals',
              'per_mean', 'per_std', 'rssi_mean', 'rssi_std', 'rssi_min', 'rssi_max', 'ttfp', 'rx_rate_normalized',
              'rx_rate', 'total_test_duration', 'test_start_time', 'trigger_time',
              'test_end_time', 'label_validated', 'rx_channel', 'energizing_pattern', 'time_profile',
              'decrypted_packet_type',
              'group_id', 'flow_ver', 'test_mode', 'en', 'type', 'data_uid', 'nonce', 'enc_uid', 'mic', 'enc_payload',
-             'gw_packet', 'stat_param', 'temperature_sensor']
+             'gw_packet', 'stat_param', 'temperature_sensor', 'humidity_sensor', 'light_intensity_sensor']
 
         self.update_run_data()
         self.update_packets_data(only_titles=True)
 
     def update_run_data(self, res=None, save_to_csv=True):
         if res is not None:
             test_info = res.get_test_info()
@@ -250,15 +252,16 @@
                             'total_test_duration': self.test_data['total_test_duration'],
                             'status_offline': self.test_data['status_offline'],
                             'fail_bin': self.test_data['fail_bin'], 'fail_bin_str': self.test_data['fail_bin_str'],
                             'external_id': None,
                             'label_validated': self.test_data['label_validated'],
                             'test_num': self.test_data['test_num'],
                             'trigger_time': self.test_data['trigger_time'], 'packet_status': None,
-                            'temperature_sensor': float(-1)}
+                            'temperature_sensor': float('nan'), 'humidity_sensor': float('nan'),
+                            'light_intensity_sensor': float('nan')}
             if summary is None:
                 default_sum = {'is_test_pass': None, 'selected_tag': None, 'test_start_time': None,
                                'test_end_time': None, 'test_status': None, 'rx_channel': None,
                                'energizing_pattern': None, 'time_profile': None, 'num_packets': 0,
                                'num_cycles': 0, 'sprinkler_counter_mean': None, 'sprinkler_counter_std': None,
                                'sprinkler_counter_min': None, 'sprinkler_counter_max': None, 'tbp_mean': None,
                                'tbp_std': None, 'tbp_min': None, 'tbp_max': None, 'tbp_num_vals': None,
@@ -283,21 +286,30 @@
                 fail_bin = FailureCodes.GW_ERROR.name
             self.test_data['fail_bin'] = FailureCodes[fail_bin].value
             self.test_data['fail_bin_str'] = fail_bin
             self.test_data['trigger_time'] = res.get_trigger_time()
 
             test_info = res.get_test_info()
             self.test_data['tag_run_location'] = test_info['tag_run_location']
+
+            # Include new sensor readings in the test data
             self.test_data['tag_reel_location'] = test_info['tag_reel_location']
             self.test_data['external_id'] = test_info['external_id'] \
                 if 'external_id' in test_info.keys() and self.test_data['status_offline'] == 1 else ''
             self.test_data['label_validated'] = test_info['validated'] \
                 if 'validated' in test_info.keys() else ValidatedBin.UNTESTED.name
             self.test_data['temperature_sensor'] = test_info['temperature_sensor'] \
-                if 'temperature_sensor' in test_info.keys() else float(-1)
+                if 'temperature_sensor' in test_info.keys() else float('nan')
+            self.test_data['humidity_sensor'] = test_info['humidity_sensor'] \
+                if 'humidity_sensor' in test_info.keys() else float('nan')
+            self.test_data['light_intensity_sensor'] = test_info['light_sensor'] \
+                if 'light_sensor' in test_info.keys() else float('nan')
+
+            if len(res) == 0:
+                save_default_packet_data()
 
             for i, r in enumerate(res):
                 self.test_data['test_num'] = i
                 r_sum = r.get_summary()
 
                 # add packets info:
                 if r.all_packets.size():
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/modules/offline_printing_and_validation.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/modules/offline_printing_and_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,20 @@
    (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
    (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 """
 
 from queue import Queue
 import socket
 from wiliot_testers.tester_utils import open_json_cache
-from wiliot_testers.offline.modules.offline_utils import R2rGpio, ConfigDefaults, get_printed_value, \
+from wiliot_testers.offline.modules.offline_utils import ConfigDefaults, get_printed_value, \
     get_print_user_config_file, DefaultGUIValues
 from wiliot_testers.test_equipment import BarcodeScanner, CognexDataMan
 from wiliot_testers.wiliot_tester_tag_result import FailureCodes, WiliotTesterTagResultList
 from wiliot_testers.offline.configs.global_vars_and_enums import PrintingAndValidationDefaults, ASTRIX
+from wiliot_testers.offline.modules.offline_r2r_controller import R2R
 
 import os
 import json
 import time
 import logging
 from threading import Event
 import datetime
@@ -121,60 +122,70 @@
     # odd values are bad
     MISMATCH = 3  # ex id/black square not as expected (should be a different ex.id or black square)
     NO_READ = 1  # expect to read ex id, but no success reading it
     ERROR = 99
 
 
 class PrintingAndValidation(object):
-    def __init__(self, test_start_event, test_end_event, stop_app_event, moh_object, test_object,
-                 exception_queue, tag_results_queue, log_obj=None, user_config=None, gw_version=''):
+    def __init__(self, test_start_event, test_end_event, validation_end_event, stop_app_event, moh_object, test_object,
+                 exception_queue, tag_results_queue, log_obj=None, user_config=None, gw_version='',
+                 get_duplicated_tags=None):
         """
 
         @param test_start_event: event is set when tag is under test
         @type test_start_event: Event
         @param test_end_event: event is set when tag test was completed
+        @type validation_end_event: Event
+        @param validation_end_event: event is set when validation ends if GW move R2R
         @type test_end_event: Event
         @param moh_object: an object contains all functions related to MOH event, Manual Operation Handling
         @type moh_object: Object
         @param test_object: an object contains all functions related to test parameters
         @type test_object: TestParameters
         @param exception_queue: queue for all exceptions, handled in the main class
         @type exception_queue: Queue
         @param tag_results_queue: queue for tag test results, sent from the tag test class
         @type tag_results_queue: Queue
         @param user_config: all user configuration inputs
         @type user_config: dict or None
         """
         self.test_start_event = test_start_event
         self.test_end_event = test_end_event
+        self.validation_end_event = validation_end_event
         self.stop_app_event = stop_app_event
         self.exception_q = exception_queue
         self.tag_results_q = tag_results_queue
         self.end_of_test_tags = []
         self.moh = moh_object
         self.test = test_object
         self.logger = logging.getLogger(log_obj.get_logger_name())
         self.is_print = user_config['toPrint'].lower() == 'yes'
         self.is_scanner = user_config['QRRead'].lower() == 'yes'
-        self.is_r2r = user_config['isR2R'].lower() == 'yes' if 'isR2R' in user_config else True
+        self.is_r2r = user_config['isR2R'].lower() == 'yes' and user_config['typeR2R'].lower() == 'arduino'
+        self.get_duplicated_tags = get_duplicated_tags
+        self.change_tag_to_duplicated = []
+
         self.last_state = ValidationStates.IDLE
         self.tag_run_location = -1
         self.external_id_counter = 0
         self.tag_result_to_validate = None
 
         self.is_init = False
+        self.r2r = None
+        self.r2r_counter_func = None
         try:
             self.printer = Printer(is_print=self.is_print,
                                    exception_queue=exception_queue,
                                    logger_name=log_obj.get_logger_name(),
                                    printing_config=log_obj.get_log_config())
-
-            self.r2r = R2R(is_r2r=self.is_r2r,
-                           exception_queue=exception_queue,
-                           logger_name=log_obj.get_logger_name())
+            if self.is_r2r:
+                self.r2r = R2R(exception_queue=exception_queue,
+                               logger_name=log_obj.get_logger_name(),
+                               exc_obj=R2RException)
+                self.r2r_counter_func = self.r2r.get_counter
 
             self.scanner = Scanner(is_scanner=self.is_scanner,
                                    exception_queue=exception_queue,
                                    logger_name=log_obj.get_logger_name(),
                                    scanning_config=user_config,
                                    is_print=self.is_print)
 
@@ -203,23 +214,32 @@
                 self.exception_q.put(PrintingAndValidationException(f'init: queues: {e}').__str__(), block=False)
             return
 
         # move to the first tag:
         try:
             if self.is_print:
                 self.set_next_printing_type(False)
-            self.r2r.move_to_the_first_tag()
+            if self.is_r2r:
+                self.r2r.move_to_the_first_tag()
         except Exception as e:
             if isinstance(e, PrintingAndValidationException):
                 self.exception_q.put(f'init: move to the first tag: {e}', block=False)
             else:
                 self.exception_q.put(PrintingAndValidationException(f'init: move to the first tag: {e}').__str__(),
                                      block=False)
             return
 
+    def get_r2r_counter(self):
+        if self.r2r_counter_func is None:
+            return 0
+        return self.r2r_counter_func()
+
+    def set_r2r_counter_func(self, r2r_counter_func=None):
+        self.r2r_counter_func = r2r_counter_func
+
     def init_validation_q(self):
         if self.is_scanner:
             q_size = self.scanner.scanning_config['QRoffset']
         elif self.is_print:
             q_size = self.printer.printing_config['printOffset'] + PrintingAndValidationDefaults.QUEUE_VALIDATION_OFFSET
         else:
             q_size = 1  # No validation is needed
@@ -234,20 +254,21 @@
         else:
             q_size = 0  # No Printing is needed
         self.printing_type_q = Queue(maxsize=q_size)
         if q_size == 0:
             return
 
         for k in range(q_size - offset_printing):
-            self.printing_type_q.put(False, block=False)
+            self.printing_type_q.put({'adva': '', 'status': False}, block=False)
 
     def run(self):
         state = ValidationStates.IDLE
         next_tag_status = False
         self.printer.reset_printer_ack()
+        start_test_time = time.time()
 
         while True:
             time.sleep(0)
             try:
                 state = self.update_state(state)
                 self.logger.info(f'PrintingAndValidation: start state {state}')
                 if state == ValidationStates.STOP:
@@ -260,53 +281,56 @@
 
                 elif state == ValidationStates.WAIT_START:
                     # wait till event start_testing is set
                     self.wait_for_new_event(event=self.test_start_event,
                                             time_to_wait=PrintingAndValidationDefaults.EVENT_WAIT_TIME)
 
                 elif state == ValidationStates.START_TEST:
-                    # Stop R2R if long test
+                    start_test_time = time.time()
+
                     self.tag_run_location += 1
                     self.logger.info(f'{ASTRIX} PrintingAndValidation: START_TEST: '
                                      f'new tag location {self.tag_run_location} {ASTRIX}')
-                    if self.is_r2r and \
-                            self.test.get_total_test_time() > PrintingAndValidationDefaults.MAX_R2R_WAIT_TIME:
-                        self.r2r.send_stop_to_r2r()
+                    # Stop R2R if long test
+                    if self.is_r2r:
+                        if self.test.get_total_test_time() > PrintingAndValidationDefaults.MAX_R2R_WAIT_TIME:
+                            self.r2r.send_stop_to_r2r()
 
                 elif state == ValidationStates.PRE_VALIDATION:
                     # Validation
                     self.tag_result_to_validate = None
                     if self.validation_q.full() or self.stop_app_event.is_set():
                         self.tag_result_to_validate = self.validation_q.get(block=False)
+                        self.handle_duplication_before_validation()
+                        self.add_external_id_to_tag_results()
                     else:
                         self.logger.info('PrintingAndValidation: PRE_VALIDATION: Waiting for the first tag to arrive')
 
                 elif state == ValidationStates.VALIDATION:
                     if self.tag_result_to_validate is not None:
                         self.validation(self.tag_result_to_validate)
 
                 elif state == ValidationStates.PRINTER_ACK:
                     if self.need_to_check_printer_ack():
                         is_ack = self.printer.get_printing_ack()
                         if not is_ack:
                             raise PrinterException('did not get printing acknowledgement (PRC)')
 
                 elif state == ValidationStates.SET_NEXT_PRINT:
-                    if self.is_print and not self.printer.printing_during_movement:
-                        time.sleep(PrintingAndValidationDefaults.PRINTER_90_DEG_WAIT_LSL)
                     # select next printing type
                     if self.is_print:
                         if self.printing_type_q.empty():
                             self.logger.info(
                                 'PrintingAndValidation: SET_NEXT_PRINT: set next printing to False since queue empty')
                             next_tag_status = False
                             self.logger.info('PrintingAndValidation: SET_NEXT_PRINT: '
                                              'set printing type to false since queue is empty')
                         else:
-                            next_tag_status = self.printing_type_q.get(block=False)
+                            next_tag_to_print = self.printing_type_q.get(block=False)
+                            next_tag_status = self.handle_duplication_before_printing(next_tag_to_print)
                         self.set_next_printing_type(next_tag_status)
 
                 elif state == ValidationStates.WAIT_END:
                     # wait till event end_of_testing is set
                     self.wait_for_new_event(
                         event=self.test_end_event,
                         time_to_wait=self.test.get_total_test_time() + PrintingAndValidationDefaults.EVENT_WAIT_TIME)
@@ -318,23 +342,30 @@
                             self.logger.info(f'Empty tag_results_q during {state}')
                             self.add_end_of_test_tags()
 
                     else:
                         cur_tag_to_print = self.tag_results_q.get(timeout=0.1, block=False)
                         cur_tag_to_print.set_test_info({'tag_run_location': self.tag_run_location,
                                                         'tag_reel_location': self.get_tag_reel_location()})
-                        self.add_external_id_to_tag_results(tag_result_to_validate=cur_tag_to_print)
                         self.validation_q.put(cur_tag_to_print, block=False)
                         if self.is_print:
-                            self.printing_type_q.put(cur_tag_to_print.is_all_tests_passed(), block=False)
+                            self.printing_type_q.put({'adva': cur_tag_to_print.check_and_get_selected_tag_id(),
+                                                      'status': cur_tag_to_print.is_all_tests_passed()}, block=False)
 
                 elif state == ValidationStates.NEXT_TAG:
+                    if self.is_print and not self.printer.printing_during_movement:
+                        dt = time.time() - start_test_time
+                        if dt < PrintingAndValidationDefaults.PRINTER_90_DEG_WAIT_TIME:
+                            time.sleep(PrintingAndValidationDefaults.PRINTER_90_DEG_WAIT_TIME - dt)
                     # send signal to the r2r to move
                     self.printer.reset_printer_ack()
-                    self.r2r.move_r2r(is_pass=next_tag_status)
+                    if self.is_r2r:
+                        self.r2r.move_r2r(is_pass=next_tag_status)
+                    else:
+                        self.validation_end_event.set()
 
                 elif state == ValidationStates.LOG_DATA:
                     # log data
                     if self.tag_result_to_validate is not None:
                         self.log_data(self.tag_result_to_validate)
                         self.tag_result_to_validate = None
                     if self.is_print:
@@ -398,29 +429,49 @@
         elif state == ValidationStates.NEXT_TAG:
             state = ValidationStates.LOG_DATA
         elif state == ValidationStates.LOG_DATA:
             state = ValidationStates.WAIT_START
 
         return state
 
+    def handle_duplication_before_printing(self, next_tag):
+        is_tag_passed = False
+        if not next_tag['status']:
+            return is_tag_passed
+
+        duplication_list = self.get_duplicated_tags()
+        if next_tag['adva'] != '' and next_tag['adva'] in duplication_list:
+            self.change_tag_to_duplicated.append(next_tag['adva'])
+            self.logger.info(f'changing printing tag {next_tag["adva"]} to fail due to duplication')
+            return is_tag_passed
+
+        is_tag_passed = True
+        return is_tag_passed
+
+    def handle_duplication_before_validation(self):
+        selected_tag = self.tag_result_to_validate.check_and_get_selected_tag_id()
+        if selected_tag in self.change_tag_to_duplicated:
+            self.tag_result_to_validate.set_total_fail_bin(FailureCodes.DUPLICATION_OFFLINE)
+            self.logger.info(f'changing tag {selected_tag} to duplication fail bin')
+
     def need_to_check_printer_ack(self):
         return self.is_print and self.is_scanner and self.printer.printing_config['enablePrinterAck'].lower() == 'yes'
 
-    def add_external_id_to_tag_results(self, tag_result_to_validate):
+    def add_external_id_to_tag_results(self):
         expected_external_id = ''
         configs = self.data_logging.get_log_config()
         if self.is_print:
-            if tag_result_to_validate.is_all_tests_passed():
+            if self.tag_result_to_validate.is_all_tests_passed():
                 expected_external_id = self.printer.get_expected_external_id(counter=self.external_id_counter)
                 self.external_id_counter += 1
             else:
                 expected_external_id = ''
                 if configs['printingFormat'] == 'prePrint':
                     self.external_id_counter += 1
-            tag_result_to_validate.set_test_info({'external_id': expected_external_id})
+            self.tag_result_to_validate.set_test_info({'external_id': expected_external_id})
             self.logger.info(f'PrintingAndValidation: assigned external id {expected_external_id}')
         return expected_external_id
 
     def get_validation_q_size(self):
         return self.validation_q.qsize()
 
     def get_validation_q_maxsize(self):
@@ -460,15 +511,17 @@
                     self.printer.set_printing_type(is_tag_passed=is_pass)
                 except Exception as e:
                     raise PrinterException(f'set_next_printing_type: {e}')
 
     def wait_for_new_event(self, event, time_to_wait):
         t_start = datetime.datetime.now()
         while not event.is_set():
-            if self.stop_app_event.is_set():
+            if not self.is_r2r and self.stop_app_event.is_set():
+                self.logger.info('stop application during waiting for event while r2r is controlled by gateway')
+            elif self.stop_app_event.is_set():
                 self.logger.info('stop application during waiting for event')
                 time.sleep(PrintingAndValidationDefaults.MIN_WAIT_TIME)
                 break
             elif self.moh.get_manual_operation_is_needed():
                 self.wait_for_moh()
                 t_start = datetime.datetime.now()
             event.wait(0.1)
@@ -514,15 +567,15 @@
                 is_validated = ValidatedBin.NO_READ
                 hw_exc = f' [{e}]'
 
         elif self.is_print and not self.is_scanner:
             # get_status from printer
             if not self.printer.printing_during_movement:
                 time.sleep(PrintingAndValidationDefaults.PRINTER_90_DEG_WAIT_TIME)
-            status = self.printer.get_printer_status(counter=self.r2r.get_counter(),
+            status = self.printer.get_printer_status(counter=self.get_r2r_counter(),
                                                      is_pass=expected_result.is_all_tests_passed())
             if status:
                 is_validated = ValidatedBin.PRINT_ACK_ONLY
             else:
                 is_validated = ValidatedBin.MISMATCH
 
         elif not self.is_print and self.is_scanner:
@@ -542,15 +595,17 @@
         self.data_logging.update_run_data(res=new_tag_results)
 
     def add_end_of_test_tags(self):
         if self.is_print:
             dummy_dict = {'tag_run_location': self.tag_run_location,
                           'tag_reel_location': self.get_tag_reel_location(),
                           'fail_bin': FailureCodes.END_OF_TEST.value,
-                          'fail_bin_str': FailureCodes.END_OF_TEST.name}
+                          'fail_bin_str': FailureCodes.END_OF_TEST.name,
+                          'trigger_time': None, 'total_test_duration': None,
+                          'label_validated': 'UNTESTED'}
             self.end_of_test_tags.append(dummy_dict)
 
     def add_end_of_test_to_log(self):
         for dummy_tag in self.end_of_test_tags:
             # Update only packet data
             self.data_logging.update_default_test_data(dummy_tag)
             self.data_logging.update_packets_data()
@@ -577,15 +632,15 @@
         if self.end_of_test_tags:
             self.add_end_of_test_to_log()
         if self.printer.enable:
             self.update_printer_configs()
             self.printer.exit()
         if self.scanner.enable:
             self.scanner.exit()
-        if self.r2r.enable:
+        if self.is_r2r:
             self.r2r.exit()
 
 
 class Printer(object):
     def __init__(self, is_print, exception_queue, logger_name, printing_config=None):
         """
 
@@ -711,20 +766,18 @@
         elif parts[1] == '4':  # (Offline)
             res = self.query(self.set_state_command('3'))
             if res == 'ACK':
                 return
         e = 'Printer failed to switch to running mode'
         raise PrinterException(f'set_printer_to_running: {e}')
 
-    def query(self, cmd, ignore_printer_ack=True):
+    def query(self, cmd):
         """Send the input cmd string via TCPIP Socket
         @type cmd: str
         @param cmd: command to send to printer
-        @type ignore_printer_ack: bool
-        @param ignore_printer_ack: if True, ack printer msg is ignored (PRC)
         @return: the reply string
         """
         cmd_str = cmd.strip('\r\n')
         self.logger.info(f'Sent command to printer: {cmd_str}')
         self.printer_socket.send(cmd.encode())
         values = self.read(cmd=cmd)
         if 'PRC' in values:
@@ -1038,83 +1091,7 @@
         return validated_status
 
     def exit(self):
         try:
             self.scanner.close_port()
         except Exception as e:
             self.logger.warning(f'Could not exit scanner due to: {e}')
-
-
-class R2R(object):
-    def __init__(self, is_r2r, exception_queue, logger_name):
-        """
-
-        @param exception_queue:
-        @type exception_queue: Queue
-        @param logger_name:
-        @type logger_name: str
-        """
-        self.exception_queue = exception_queue
-        self.logger = logging.getLogger(logger_name)
-        self.counter = 0
-
-        self.enable = True
-        if not is_r2r:
-            self.logger.info('R2R is disable')
-            self.enable = False
-            return
-
-        self.is_running = False
-        try:
-            self.gpio = R2rGpio(logger_name=logger_name)
-        except Exception as e:
-            raise R2RException(f'init: could not connect to arduino: {e}')
-
-    def reconnect(self):
-        status = self.gpio.reconnect()
-        if not status:
-            raise R2RException(f'reconnect: could not connect to arduino')
-
-    def move_to_the_first_tag(self):
-        self.send_start_to_r2r()
-        self.move_r2r(is_pass=False)
-
-    def send_start_to_r2r(self):
-        self.gpio.gpio_state(PrintingAndValidationDefaults.START_STOP_GPIO, "ON")
-        self.logger.info('R2R: PC send start to R2R')
-        self.is_running = True
-
-    def send_stop_to_r2r(self):
-        self.gpio.gpio_state(PrintingAndValidationDefaults.START_STOP_GPIO, "OFF")
-        self.logger.info('R2R: PC send stop to R2R')
-        self.is_running = False
-
-    def move_r2r(self, is_pass):
-        if not self.is_running:
-            self.send_start_to_r2r()
-        gpio = PrintingAndValidationDefaults.PASS_PULSE_GPIO \
-            if is_pass else PrintingAndValidationDefaults.FAIL_PULSE_GPIO
-        self.gpio.pulse(gpio, PrintingAndValidationDefaults.R2R_PULSE_DURATION)
-        self.logger.info(f'{ASTRIX} R2R: PC send {"pass" if is_pass else "fail"} to R2R {ASTRIX}')
-        self.counter += 1
-
-    def enable_missing_label(self, is_enable):
-        gpio_on_off = 'ON' if is_enable else 'OFF'
-        self.gpio.gpio_state(PrintingAndValidationDefaults.MISSING_LABEL_GPIO, gpio_on_off)
-        self.logger.info(f'R2R: PC send {"enable" if is_enable else "disable"} missing label msg to R2R')
-
-    def end_of_run(self):
-        self.send_stop_to_r2r()
-        self.enable_missing_label(is_enable=False)
-
-    def get_counter(self):
-        return self.counter
-
-    def reset_counter(self):
-        self.counter = 0
-
-    def exit(self):
-        try:
-            self.send_stop_to_r2r()
-            self.gpio.__del__()
-        except Exception as e:
-            self.logger.warning(f'Could not exit R2R due to: {e}')
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/modules/offline_tag_testing.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/modules/offline_tag_testing.py`

 * *Files 19% similar despite different names*

```diff
@@ -58,27 +58,34 @@
    (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 """
 
 import logging
 import time
 import numpy as np
 from enum import Enum
+
 from wiliot_testers.wiliot_tester_tag_test import WiliotTesterTagTest
 from wiliot_testers.wiliot_tester_tag_result import FailureCodes, WiliotTesterTagResultList
-from wiliot_testers.test_equipment import Attenuator, YoctoTemperatureSensor
+from wiliot_testers.test_equipment import Attenuator, YoctoSensor
 from wiliot_core import InlayTypes, WiliotGateway
 from wiliot_testers.offline.configs.global_vars_and_enums import TagTestingDefaults
+from wiliot_testers.offline.modules.offline_r2r_controller import R2R
 
 
 class TagTestingException(Exception):
     def __init__(self, msg):
         self.message = msg
         super().__init__(f'TagTesting Exception: {self.message}')
 
 
+class R2RException(TagTestingException):
+    def __init__(self, msg):
+        super().__init__(f'R2R: {msg}')
+
+
 class MissingLabelException(TagTestingException):
     def __init__(self, msg):
         super().__init__(f'Missing Label: {msg}')
 
 
 class AttenuatorException(TagTestingException):
     def __init__(self, msg):
@@ -98,37 +105,45 @@
     STOP = 99
     WAIT_MOH = 88
     GET_TRIGGER = 1
     START_TEST = 2
     TAG_TEST = 3
     PROCESS_TEST = 4
     END_TEST = 5
+    WAIT_END = 6
+    NEXT_TAG = 7
 
 
 class TagTesting(object):
-    def __init__(self, test_start_event, test_end_event, stop_app_event, moh_object,
-                 exception_queue, tag_results_queue, log_obj, user_config=None, hw_config=None):
+    def __init__(self, test_start_event, test_end_event, validation_end_event, stop_app_event, moh_object,
+                 exception_queue, tag_results_queue, log_obj, test_object, user_config=None, hw_config=None):
         self.test_start_event = test_start_event
         self.test_end_event = test_end_event
+        self.validation_end_event = validation_end_event
         self.stop_app_event = stop_app_event
         self.exception_q = exception_queue
         self.tag_results_q = tag_results_queue
         self.moh = moh_object
+        self.test = test_object
         self.logger = logging.getLogger(log_obj.get_logger_name())
         self.user_config = user_config
         self.tested = 0
         self.missing_labels = 0
+        self.last_missing_label_location = -1
         self.need_to_manual_trigger = False
         self.all_selected_tags = []
+        self.all_duplicated_tags = []
         self.all_tags = []
         self.is_passed_list = []
         self.ttfp_list = []
         self.last_state = TagStates.IDLE
-        self.is_init = False
+        self.is_r2r = user_config['isR2R'].lower() == 'yes' and user_config['typeR2R'].lower() == 'gateway'
 
+        self.is_init = False
+        self.r2r = None
         try:
             # init gateway:
             self.gw_obj = WiliotGateway(auto_connect=True, logger_name=self.logger.name, is_multi_processes=True,
                                         log_dir_for_multi_processes=log_obj.get_test_folder())
 
             # init tester class
             self.wiliot_tester = WiliotTesterTagTest(
@@ -140,31 +155,40 @@
                 stop_event_trig=self.stop_app_event,
                 inlay=InlayTypes(self.user_config['inlay']))
 
             # init timeout for trigger:
             self.logger.info(f'Maximum time for gw trigger (i.e. missing label) '
                              f'is {TagTestingDefaults.TIMEOUT_FOR_MISSING_LABEL}')
 
+            # init r2r if relevant:
+            if self.is_r2r:
+                self.r2r = R2R(exception_queue=exception_queue,
+                               logger_name=log_obj.get_logger_name(),
+                               exc_obj=R2RException,
+                               gw_obj=self.gw_obj)
+
             # init external hw
             self.attenuator_handle = AttenuatorHandle(logger_name=self.logger.name, exception_q=exception_queue,
                                                       attenuator_configs=hw_config)
-            self.temperature_sensor_handle = TemperatureSensorHandle(logger_name=self.logger.name,
-                                                                     exception_q=exception_queue,
-                                                                     sensor_configs=hw_config)
+            self.sensors_handle = ExternalSensorHandle(logger_name=self.logger.name,
+                                                       exception_q=exception_queue,
+                                                       sensor_configs=hw_config)
             self.is_init = True
 
         except Exception as e:
             if isinstance(e, TagTestingException):
                 self.exception_q.put(f'init: {e}', block=False)
             else:
                 self.exception_q.put(TagTestingException(f'init: {e}').__str__(), block=False)
 
     def run(self):
         tester_res = WiliotTesterTagResultList()  # Empty list
         state = TagStates.IDLE
+        if self.is_r2r:
+            self.r2r.move_to_the_first_tag()
 
         while True:
             time.sleep(0)
             try:
                 state = self.update_state(state)
                 self.logger.info(f'TagTesting: start state {state}')
                 if state == TagStates.GET_TRIGGER:
@@ -179,14 +203,26 @@
 
                 elif state == TagStates.PROCESS_TEST:
                     self.process_test(tester_res=tester_res)
 
                 elif state == TagStates.END_TEST:
                     self.end_test(tester_res=tester_res)
 
+                elif state == TagStates.WAIT_END:
+                    if self.is_r2r:
+                        # wait till event end_of_validation is set
+                        self.wait_for_new_event(
+                            event=self.validation_end_event,
+                            time_to_wait=TagTestingDefaults.EVENT_WAIT_TIME)
+
+                elif state == TagStates.NEXT_TAG:
+                    if self.is_r2r:
+                        # send signal to the r2r to move
+                        self.r2r.move_r2r()
+
                 elif state == TagStates.STOP:
                     self.logger.info('Stop running TagTesting main loop')
                     break
 
                 elif state == TagStates.WAIT_MOH:
                     self.wait_for_moh()
 
@@ -198,31 +234,35 @@
                 else:
                     self.exception_q.put(TagTestingException(f'run: state{state.name}: {e}').__str__(), block=False)
 
                 if state == TagStates.GET_TRIGGER:
                     self.need_to_manual_trigger = True
                 elif state == TagStates.TAG_TEST:
                     tester_res = WiliotTesterTagResultList()
+                    tester_res.set_total_fail_bin(fail_code=FailureCodes.GW_ERROR)
                 elif state == TagStates.PROCESS_TEST:
                     tester_res.set_total_fail_bin(fail_code=FailureCodes.SOFTWARE_GENERAL_ERROR, overwrite=True)
                 elif state == TagStates.END_TEST or state == TagStates.WAIT_MOH:
                     self.logger.warning(f'TagTesting Got exception during {state}: {e}')
+                elif state == TagStates.NEXT_TAG:
+                    state = TagStates.WAIT_END
 
         self.stop()
 
     def update_state(self, state):
         # after MOH was done, continue to the next state
         if state == TagStates.WAIT_MOH:
             state = self.last_state
 
         # when event occurred
         if self.stop_app_event.is_set():
             if state == TagStates.TAG_TEST or state == TagStates.PROCESS_TEST:
                 pass  # finish the cycle
             else:
+                self.last_state = state
                 state = TagStates.STOP
         elif self.moh.get_manual_operation_is_needed():
             self.last_state = state
             state = TagStates.WAIT_MOH
 
         # main flow
         if state == TagStates.IDLE:
@@ -232,56 +272,92 @@
         elif state == TagStates.START_TEST:
             state = TagStates.TAG_TEST
         elif state == TagStates.TAG_TEST:
             state = TagStates.PROCESS_TEST
         elif state == TagStates.PROCESS_TEST:
             state = TagStates.END_TEST
         elif state == TagStates.END_TEST:
+            state = TagStates.WAIT_END
+        elif state == TagStates.WAIT_END:
+            state = TagStates.NEXT_TAG
+        elif state == TagStates.NEXT_TAG:
             state = TagStates.GET_TRIGGER
 
         return state
 
+    def wait_for_new_event(self, event, time_to_wait=TagTestingDefaults.POST_RUN_WAIT_TIME):
+        t_start = time.time()
+        while not event.is_set():
+            if self.stop_app_event.is_set():
+                self.logger.info('Tag Testing: stop application during waiting for event')
+                time.sleep(TagTestingDefaults.POST_RUN_WAIT_TIME)
+                break
+            elif self.moh.get_manual_operation_is_needed():
+                self.wait_for_moh()
+                t_start = time.time()
+            event.wait(0.1)
+            dt = time.time() - t_start
+
+            if dt > time_to_wait and not self.moh.get_manual_operation_is_needed():
+                raise TagTestingException('wait_for_new_event: did not receive ack for '
+                                          'starting/ending tag test')
+        event.clear()
+
+    def update_missing_label_parameters(self):
+        self.missing_labels += 1
+        if self.user_config['sensorOffset'] != '':
+            self.last_missing_label_location = self.tested + int(self.user_config['sensorOffset']) + 1
+            self.logger.info(f'TagTesting: update_missing_label_parameters: '
+                             f'estimate Missing Label at location: {self.last_missing_label_location}')
+
     def get_trigger(self):
         pulse_received = self.wiliot_tester.wait_for_trigger(
             wait_for_gw_trigger=TagTestingDefaults.TIMEOUT_FOR_MISSING_LABEL)
         if not pulse_received:
             while self.moh.get_manual_operation_is_needed():
                 self.wait_for_moh()
                 if self.stop_app_event.is_set():
                     return
                 pulse_received = self.wiliot_tester.wait_for_trigger(
                     wait_for_gw_trigger=TagTestingDefaults.TIMEOUT_FOR_MISSING_LABEL)
                 if pulse_received:
                     break
             if not pulse_received:
-                self.missing_labels += 1
+                self.update_missing_label_parameters()
                 if TagTestingDefaults.ENABLE_MISSING_LABEL and \
                         self.missing_labels < TagTestingDefaults.MAX_MISSING_LABEL_ENGINEERING:
                     self.need_to_manual_trigger = True
                     self.logger.info((f'MISSING LABEL. no trigger was received for '
                                       f'{TagTestingDefaults.TIMEOUT_FOR_MISSING_LABEL} seconds. Continue to test.'))
                     return
 
                 raise MissingLabelException(f'MISSING LABEL. no trigger was received for '
                                             f'{TagTestingDefaults.TIMEOUT_FOR_MISSING_LABEL} seconds')
 
     def start_test(self):
         self.test_start_event.set()
         if self.attenuator_handle.enable:
             self.attenuator_handle.set_dynamic_value()
+        if self.is_r2r:
+            if self.test.get_total_test_time() > TagTestingDefaults.MAX_R2R_WAIT_TIME:
+                self.r2r.send_stop_to_r2r()
+
+    def gw_reset_and_config(self):
+        self.wiliot_tester.gw_reset_and_config()
+        self.wiliot_tester.init_gw_test(is_start_gw_app=False)
 
     def tag_test(self):
+        self.tested += 1
         if not self.is_printing_calibration():
             tester_res = self.wiliot_tester.run(wait_for_gw_trigger=None,
                                                 need_to_manual_trigger=self.need_to_manual_trigger)
         else:
             tester_res = WiliotTesterTagResultList()
             time.sleep(TagTestingDefaults.TIME_BETWEEN_TEST_PRINTING)
 
-        self.tested += 1
         return tester_res
 
     def process_test(self, tester_res):
         is_pass = False
         if self.is_printing_calibration():
             tester_res.set_total_test_status(True)
             is_pass = True
@@ -293,56 +369,71 @@
                 else:
                     is_pass = True
 
             elif selected_tag in self.all_selected_tags:
                 # Duplication
                 tester_res.set_total_fail_bin(FailureCodes.DUPLICATION_OFFLINE)
                 tester_res.set_packet_status(adv_address=selected_tag, status='duplication')
+                self.all_duplicated_tags.append(selected_tag)
                 self.logger.warning(f'DUPLICATION for Adva: {selected_tag}')
             else:
                 # PASS
                 self.all_selected_tags.append(selected_tag)
                 is_pass = True
+        else:
+            if tester_res.get_total_fail_bin() == FailureCodes.NO_RESPONSE.value:
+                self.logger.info(f'TagTesting: process_test: got NO_RESPONSE at location: {self.tested}')
+                if self.last_missing_label_location == self.tested:
+                    tester_res.set_total_fail_bin(FailureCodes.MISSING_LABEL, overwrite=True)
+                    self.logger.info(f'set tag location {self.tested} to MISSING lABEL fail bin')
         if not is_pass:
             self.logger.warning(f'Tag {self.tested} Failed - {tester_res.get_total_fail_bin(as_name=True)}')
         self.all_tags += tester_res.get_test_unique_adva()
         self.all_tags = list(set(self.all_tags))
         self.is_passed_list.append(is_pass)
 
+    def get_all_duplicated_tags(self):
+        return self.all_duplicated_tags
+
     def is_printing_calibration(self):
         return self.user_config['printingFormat'].lower() == 'test' and self.user_config['toPrint'].lower() == 'yes'
 
     @staticmethod
     def calculating_ttfp_avg(ttfp_list):
         ttfp_list_no_nan = [x for x in ttfp_list if not np.isnan(x)]
         if ttfp_list_no_nan:
             return np.mean(ttfp_list_no_nan)
         return float(-1)
 
     def end_test(self, tester_res):
         self.ttfp_list.append(tester_res.get_total_ttfp())
-        test_data = {'temperature_sensor': float(-1),
-                     'tested': self.get_tested(),
+        test_data = {'tested': self.get_tested(),
                      'passed': self.get_passed(),
                      'responded': self.get_responded(),
                      'missing_label': self.get_missing_label_count(),
                      'ttfp_avg': self.calculating_ttfp_avg(self.ttfp_list)}
-        if self.temperature_sensor_handle.enable:
+        if self.sensors_handle.enable:
             try:
-                test_data['temperature_sensor'] = self.temperature_sensor_handle.get_temperature()
+                sensors_out = self.sensors_handle.get_measurement()
+                test_data = {**test_data, **sensors_out}
             except Exception as e:
                 self.logger.warning(f'end test: could not read from sensor due to {e}')
         tester_res.set_test_info(test_info=test_data)
         if self.tag_results_q.full():
             raise TagTestingException('end_test: tag results queue is full - error in offset definition')
         self.tag_results_q.put(tester_res, block=False)
         self.test_end_event.set()
 
     def wait_for_moh(self):
         self.logger.info('TagTesting: wait for manual operation handling')
+        try:
+            if self.is_r2r:
+                self.r2r.send_stop_to_r2r()
+        except Exception as e:
+            self.logger.warning(f'Could not stop R2R during wait for manual operation handling due to {e}')
         while True:
             time.sleep(1)
             if not self.moh.get_manual_operation_is_needed():
                 break
             if self.stop_app_event.is_set():
                 break
 
@@ -361,17 +452,54 @@
     def get_is_passed_list(self):
         return self.is_passed_list.copy()
 
     def get_ttfp_list(self):
         return self.ttfp_list
 
     def stop(self):
+        if self.is_r2r:
+            self.post_run_validation()
+            self.r2r.exit()
         self.wiliot_tester.exit_tag_test()
         self.logger.info('TagTesting Thread is done')
 
+    def post_run_validation(self):
+        self.logger.info('TagTesting: start post run validation...')
+        if self.last_state == TagStates.WAIT_END:
+            stage = 'move'  # wait, move, trigger
+        elif self.last_state == TagStates.GET_TRIGGER:
+            stage = 'trigger'  # wait, move, trigger
+        else:
+            stage = 'wait'  # wait, move, trigger
+        while True:
+            if stage == 'wait':
+                time.sleep(TagTestingDefaults.TIME_BETWEEN_TEST_PRINTING)
+                self.validation_end_event.wait(TagTestingDefaults.POST_RUN_WAIT_TIME)
+                if not self.validation_end_event.is_set():
+                    break
+                stage = 'move'
+            elif stage == 'move':
+                self.validation_end_event.clear()
+                self.r2r.move_r2r()
+                gw_answer = self.gw_obj.read_specific_message(msg="Start Production Line GW",
+                                                              read_timeout=TagTestingDefaults.EVENT_WAIT_TIME)
+                self.logger.info(f'TagTesting: post_run_validation: gw rsp: {gw_answer}')
+                stage = 'trigger'
+
+            elif stage == 'trigger':
+                self.test_start_event.set()
+                self.gw_obj.stop_gw_app()
+                self.test_end_event.set()
+                stage = 'wait'
+
+            else:
+                raise Exception(f'TagTesting: post_run_validation: stage is not supported: {stage}')
+
+        self.logger.info('TagTesting: end post run validation')
+
     def get_gw_version(self):
         return self.wiliot_tester.get_gw_version()
 
 
 class AttenuatorHandle(object):
     def __init__(self, logger_name, exception_q, attenuator_configs=None):
         self.logger = logging.getLogger(logger_name)
@@ -404,35 +532,51 @@
             raise AttenuatorException(f'AttenuatorHandle Exception: set_value: failed to set attenuation value '
                                       f'(expected: {attenuator_val}, current: {set_attn_status})')
 
     def set_dynamic_value(self):
         pass
 
 
-class TemperatureSensorHandle(object):
+class ExternalSensorHandle(object):
     def __init__(self, logger_name, exception_q, sensor_configs=None):
         self.logger = logging.getLogger(logger_name)
         self.exception_q = exception_q
+        self.sensor_configs = sensor_configs
+
         self.enable = True
-        if sensor_configs is None or sensor_configs['temperatureSensorEnable'].lower() == 'no':
-            self.logger.info('Temperature Sensor is disable')
+        if sensor_configs is None or self.sensor_configs['sensorsEnable'].lower() == 'no':
+            self.logger.info('External Sensors measurement is disable')
             self.enable = False
             return
 
-        self.sensor_configs = sensor_configs
+        self.sensor = None
+        self.sensor_measurements = []
         try:
-            self.temp_sensor = YoctoTemperatureSensor()
-            self.temp_sensor.connect()
-            sensor_name = self.temp_sensor.get_sensor_name()
-            self.logger.info(f'Connected to temperature sensor: {sensor_name}')
+            self.connect()
         except Exception as e:
-            raise SensorException(f'TemperatureSensorHandle Exception: init: {e}')
+            raise SensorException(f'ExternalSensorHandle Exception: init: {e}')
 
-    def get_temperature(self):
-        try:
-            cur_temp = self.temp_sensor.get_temperature()
-            self.logger.info(f'Measured temperature from sensor: {cur_temp}')
-            if cur_temp == float('nan'):
-                self.logger.warning('TemperatureSensorHandle: Could not measure temperature from sensor')
-            return cur_temp
-        except Exception as e:
-            raise Exception(f'SENSOR: TemperatureSensorHandle Exception: get_temperature: {e}')
+    def connect(self):
+        self.sensor = YoctoSensor(self.logger)
+        if self.sensor.temperature_sensor is not None:
+            self.logger.info(f'Connected to temperature sensor')
+            self.sensor_measurements.append({'name': 'temperature', 'func': self.sensor.get_temperature})
+        if self.sensor.humidity_sensor is not None:
+            self.logger.info(f'Connected to humidity sensor')
+            self.sensor_measurements.append({'name': 'humidity', 'func': self.sensor.get_humidity})
+        if self.sensor.light_sensor is not None:
+            self.logger.info(f'Connected to light sensor')
+            self.sensor_measurements.append({'name': 'light', 'func': self.sensor.get_light})
+
+    def get_measurement(self):
+        meas_out = {}
+        for meas in self.sensor_measurements:
+            try:
+                cur_value = meas['func']()
+                if cur_value == float('nan') or (isinstance(cur_value, int) and cur_value == 0):
+                    self.logger.warning(f'ExternalSensorHandle: Could not measure {meas["name"]} from sensor')
+                else:
+                    self.logger.info(f'Measured {meas["name"]} from sensor: {cur_value}')
+                    meas_out[f'{meas["name"]}_sensor'] = cur_value
+            except Exception as e:
+                raise SensorException(f'ExternalSensorHandle: get_measurement: {e}')
+        return meas_out
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/modules/offline_utils.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/modules/offline_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,18 @@
         self.printer_defaults = {'TCP_IP': '192.168.6.61', 'TCP_PORT': '3003', 'TCP_BUFFER': '128',
                                  'enableLineSelection': 'Yes', 'enablePrinterAck': 'No',
                                  'printingDuringMovement': 'Yes'}
         self.single_band_gw_defaults = {'energizingPattern': '18', 'timeProfile': '3,7', 'txPower': '3',
                                         'rssiThreshold': '90', 'plDelay': '150'}
         self.dual_band_gw_defaults = {'energizingPattern': '18', 'secondEnergizingPattern': '52', 'timeProfile': '5,10',
                                       'txPower': '3', 'rssiThreshold': '90', 'plDelay': '100'}
-        self.external_hw = {"temperatureSensorEnable": "No",
+        self.external_hw = {"sensorsEnable": "No",
                             "AutoAttenuatorEnable": "No", "attnComport": "AUTO", "attnval": "0",
-                            "scannerType": "rtscan"}
+                            "scannerType": "rtscan",
+                            "isR2R": "yes", "typeR2R": "arduino"}
 
     def get_printer_defaults(self):
         return self.printer_defaults
 
     def get_single_band_gw_defaults(self):
         return self.single_band_gw_defaults
 
@@ -118,14 +119,15 @@
                 'testName': 'Ble_Test_Only', 'inlay': InlayTypes.TIKI_099.value,
                 'desiredTags': '9999999', 'desiredPass': '9999999',
                 'surface': SurfaceTypes.AIR.value,
                 'conversion': ConversionTypes.STANDARD.value,
                 'Environment': 'production', 'OwnerId': 'wiliot-ops', 'operator': '',
                 'QRRead': 'No', 'QRcomport': 'COM3', 'QRoffset': '2',
                 'QRtimeout': '200',
+                'sensorOffset': '',
                 'comments': '', 'maxFailStop': '50', 'maxYieldStop': '40',
                 'pass_response_diff': '100', 'pass_response_diff_offset': '9999'}
         elif gui_type == 'Test':
             self.default_gui_values = {'passJobName': 'BARCODE_8', 'passJobNum': 2, 'sgtin': '',
                                        'stringBeforeCounter': '',
                                        'reelNumManually': 'test', 'firstPrintingValue': '0', 'tagLocation': '0',
                                        'tag_reel_location': '0'}
@@ -342,21 +344,25 @@
                   SimGUI.InputCombo(('Yes', 'No'), visible=True, default_value=gui_inputs_values["QRRead"],
                                     key='QRRead')],
                  [SimGUI.Text('QR ComPort: ', size=(40, 1), visible=True),
                   SimGUI.Spin(values=[i for i in range(1, 15)], initial_value=(
                       int(gui_inputs_values['QRcomport'][-1]) if len(str(gui_inputs_values['QRcomport'])) > 1 else int(
                           gui_inputs_values['QRcomport'])),
                               size=(6, 1), key='QRcomport')],
-                 [SimGUI.Text('QR offset (tags between GW and QR scanner):', size=(40, 1), visible=True),
+                 [SimGUI.Text('QR offset (tags between coupler and QR scanner):', size=(40, 1), visible=True),
                   SimGUI.Spin(values=[i for i in range(1, 10)], initial_value=int(gui_inputs_values['QRoffset']),
                               size=(6, 1), key='QRoffset')],
                  [SimGUI.Text('QR Timeout:', size=(40, 1), visible=True),
                   SimGUI.Spin(values=[i for i in range(100, 1000, 100)],
                               initial_value=int(gui_inputs_values['QRtimeout']),
-                              size=(6, 1), key='QRtimeout')]
+                              size=(6, 1), key='QRtimeout')],
+                 [SimGUI.Text('Label Detection Sensor offset (tags between sensor and coupler):', size=(40, 1),
+                              visible=True),
+                  SimGUI.Spin(values=[i for i in range(1, 50)], initial_value=gui_inputs_values['sensorOffset'],
+                              size=(6, 1), key='sensorOffset')],
                  ]
 
     stop_conditiona_tab = [
         [SimGUI.Text('Ignore stop conditions', size=(40, 1)),
          SimGUI.Checkbox('', default=False, key='ignoreStop',
                          disabled=False, visible=True)],
         [SimGUI.Text('Max failed tags in a row:', size=(40, 1)),
@@ -400,14 +406,22 @@
 
         elif event.startswith(EXTEND_KEY):
             window[EXTEND_KEY].update(visible=not window[EXTEND_KEY].visible)
             window[EXTEND_KEY + '-BUTTON-'].update(
                 window[EXTEND_KEY].metadata[0] if window[EXTEND_KEY].visible else window[EXTEND_KEY].metadata[1])
 
         elif event == 'Submit':
+            if int(values['printOffset']) == 0:
+                SimGUI.popup_error('Offset Value 0 is not valid', keep_on_top=True)
+                values['printOffset'] = '1'
+                continue
+            if values['sensorOffset'] != '' and not str(values['sensorOffset']).isnumeric():
+                SimGUI.popup_error('Label Detection Sensor offset MUST be integer or empty',  keep_on_top=True)
+                values['sensorOffset'] = ''
+                continue
             # make sure user input is legit
             reel_name_ver = False
             if int(values['printOffset']) != int(gui_inputs_values['printOffset']):
                 # popup warning message:
                 change_in_printing_offset = \
                     SimGUI.popup_ok_cancel('Are you sure you want to change the printing offset?\n'
                                            '(old value:{}, new value: {})?\n'.format(gui_inputs_values['printOffset'],
@@ -418,37 +432,36 @@
                     SimGUI.popup('printing offset was NOT change and equals to {}'.format(values['printOffset']),
                                  button_type='ok', font=14)
 
             if ' ' in values['batchName'] or '/' in values['batchName'] or '\\' in values['batchName']:
                 print("Reel name could not contain spaces, '\\' or '/'\nplease fix it and press Submit")
                 continue
 
+            try:
+                int(values['desiredTags'])
+                int(values['desiredPass'])
+            except Exception as e:
+                print("the following values should be numbers (integer): "
+                      "desiredTags, desiredPass (and should not be smaller than 2")
+                continue
+            yes_no = ['Yes', 'No']
+            if values['toPrint'] not in yes_no:
+                print("the following values should be 'Yes' or 'No': toPrint")
+                continue
+            if values['Environment'] == 'production' and values['toPrint'].lower() == 'yes':
+                reel_name_ver = check_structure(values['batchName'])
             else:
-                try:
-                    int(values['desiredTags'])
-                    int(values['desiredPass'])
-                except Exception:
-                    print("the following values should be numbers (integer): packetThreshold,"
-                          "desiredTags, desiredPass (and should not be smaller than 2")
-                    continue
-                yes_no = ['Yes', 'No']
-                if values['toPrint'] not in yes_no:
-                    print("the following values should be 'Yes' or 'No': toPrint")
-                    continue
-                if values['Environment'] == 'production' and values['toPrint'].lower() == 'yes':
-                    reel_name_ver = check_structure(values['batchName'])
-                else:
-                    reel_name_ver = True
+                reel_name_ver = True
 
-                if reel_name_ver:
-                    break
-                else:
-                    SimGUI.popup('Reel name error \n Reel name should be: <6 uppercase alphanumeric chars>.'
-                                 '<2 integers minimum 01 maximum 25>_<upper case char minimum A maximum F>',
-                                 button_type='ok', font=14)
+            if reel_name_ver:
+                break
+            else:
+                SimGUI.popup('Reel name error \n Reel name should be: <6 uppercase alphanumeric chars>.'
+                             '<2 integers minimum 01 maximum 25>_<upper case char minimum A maximum F>',
+                             button_type='ok', font=14)
 
         elif event == 'Advanced Calibration':
             # calib_val = True
             # break
             window.hide()
             calib_values = open_calibration_config()
             window.un_hide()
@@ -514,24 +527,33 @@
 def printing_process_of_test_and_sgtin(window, printing_format, gui_inputs_values, is_new_reel=True):
     """
     A function that does all the work of the printing process
     """
     reel_number = ''
     pass_job_name = None
     is_ok = True
+    original_p_format = printing_format
     while True:
         event, values = window.read()
-        if printing_format != 'Test':
-            pass_job_name = values['passJobName']
+        pass_job_name = values['passJobName']
+
         if event == SimGUI.WINDOW_CLOSED or event is None:
             is_ok = False
             break
 
-        if event == 'Submit':
+        if event == 'Submit' or event == 'Check first print':
+            reel_number = ''
             try:
+                if original_p_format == 'Test':
+                    printing_format_list = [k for k, v in PRINT_FORMAT_TO_PASS_JOB_NAME.items() if v == pass_job_name]
+                    if len(printing_format_list) != 1:
+                        raise Exception(f'specified unsupported pass job name while Printing format sis Test: '
+                                        f'{pass_job_name}')
+                    printing_format = printing_format_list[0]
+
                 if printing_format == 'prePrint':
                     if 'T' not in values['firstFullExternalId']:
                         window['-OUTPUT-'].update(
                             'scanned external id must contains the char T')
                         continue
                     external_id_list = values['firstFullExternalId'].split('T')
                     if len(external_id_list) != 2:
@@ -598,41 +620,42 @@
                                                      keep_on_top=True)
                 if sure_to_submit.lower() == 'no':
                     window['-OUTPUT-'].update('')
                     continue
                 else:
                     window['-OUTPUT-'].update('The first tag printing value will be:\n' + first_print)
 
+        if event == 'Check first print':
+            continue
+
         break
 
     v = {'passJobName': pass_job_name, 'digitsInCounter': TAG_COUNTER_DIGITS, 'passJobNum': PASS_JOB_NUM,
          'firstPrintingValue': values['firstPrintingValue'], 'tagLocation': values['firstPrintingValue'],
-         'tag_reel_location': gui_inputs_values['tag_reel_location']}
+         'tag_reel_location': gui_inputs_values['tag_reel_location'],
+         'stringBeforeCounter': reel_number}
 
     data_to_save = {'passJobName': pass_job_name,
                     'passJobNum': PASS_JOB_NUM,
                     'sgtin': values['sgtinNumManually'] if 'sgtinNumManually' in values else '',
                     'reelNumManually': values['reelNumManually'],
                     'firstPrintingValue': values['firstPrintingValue'],
                     'tagLocation': values['firstPrintingValue'],
-                    'tag_reel_location': gui_inputs_values['tag_reel_location']}
+                    'tag_reel_location': gui_inputs_values['tag_reel_location'],
+                    'stringBeforeCounter': reel_number}
 
-    if printing_format == 'Test':
-        v['stringBeforeCounter'] = \
-            values['sgtinNumManually'] if 'sgtinNumManually' in values else '' + values['reelNumManually']
+    if original_p_format == 'Test':
         v['failJobName'] = pass_job_name
     else:
-        v['stringBeforeCounter'] = reel_number
         v['failJobName'] = 'line_'
-        v['printingFormat'] = printing_format
-        data_to_save['stringBeforeCounter'] = reel_number
-        data_to_save['printingFormat'] = printing_format
+        v['printingFormat'] = original_p_format
+        data_to_save['printingFormat'] = original_p_format
 
     folder_name = 'configs'
-    file_name = get_print_user_config_file(printing_format)
+    file_name = get_print_user_config_file(original_p_format)
     f = open(os.path.join(folder_name, file_name), "w")
     json.dump(data_to_save, f)
     f.close()
     return v, is_ok
 
 
 def get_print_user_config_file(printing_format):
@@ -657,29 +680,27 @@
         reel_num = 'test_test_test_test_X_test'
         gui_inputs_values['sgtin'] = reel_num[:22]
         gui_inputs_values['reelNumManually'] = reel_num[22:]
         gui_inputs_values['firstPrintingValue'] = '0'
         gui_inputs_values['tagLocation'] = '0'
         gui_inputs_values['tag_reel_location'] = '0'
 
-    layout = [[SimGUI.Text('Job to print for pass and fail:'),
+    layout = [[SimGUI.Text('Job to print for pass:'),
                SimGUI.InputCombo(('SGTIN_only', 'SGTIN_QR', 'BARCODE_8', 'devkit_TEO', 'devkit_TIKI', 'empty'),
                                  default_value=gui_inputs_values['passJobName'], key='passJobName')],
-              [SimGUI.Text('pass line number:'),
-               SimGUI.Input(gui_inputs_values['passJobNum'], key='passJobNum')],
               [SimGUI.Text("What is the first counter number?")],
               [SimGUI.Input(gui_inputs_values['firstPrintingValue'], key='firstPrintingValue')],
-              [SimGUI.Checkbox('Insert reel number manually?', default=False, key='isManually')],
-              [SimGUI.Text("For manual mode only - what is the sgtin number?", key='sgtinNumManuallyText'),
+              [SimGUI.Text("For QR code - what is the sgtin number?", key='sgtinNumManuallyText'),
                SimGUI.Input(gui_inputs_values['sgtin'], key='sgtinNumManually')],
-              [SimGUI.Text("For manual mode only - what is the reel number?", key='reelNumManuallyText'),
+              [SimGUI.Text("For Barcode code - what is the reel number?", key='reelNumManuallyText'),
                SimGUI.Input(gui_inputs_values['reelNumManually'], key='reelNumManually')],
               [SimGUI.Text(size=(60, 3), key='-OUTPUT-')],
               [SimGUI.Text("*Tags in this run will not be serialized")],
-              [SimGUI.Button('Check first print'), SimGUI.Button('Submit', button_color=('white', '#0e6251'))]]
+              [SimGUI.Button('Check first print'),
+               SimGUI.Button('Submit', button_color=('white', '#0e6251'))]]
     window = SimGUI.Window('Printing Test', layout, keep_on_top=True)
     wanted_v, wanted_is_ok = printing_process_of_test_and_sgtin(window, printing_format, gui_inputs_values)
     window.close()
     return wanted_v, wanted_is_ok
 
 
 def printing_sgtin_window(env='', owner_id='wiliot-ops', printing_format='SGTIN'):
@@ -1042,14 +1063,15 @@
                 self.s.close()
                 logging.warning(f"Failed to close connection to {self.comport} - Please restart connection")
                 reconnect_success = False
         return reconnect_success
 
 
 if __name__ == '__main__':
+    s = printing_test_window()
     a = printing_sgtin_window(env='prod', owner_id='wiliot-ops', printing_format='prePrint')
     rsp = get_reel_name_from_cloud_api(env='test', owner_id='wiliot-ops', printing_format='Barcode')
 
     open_session(['Single Band', 'Dual Band'])
     printing_test_window()
     printing_sgtin_window(env='test', printing_format='Barcode')
     printing_sgtin_window(env='test', printing_format='SGTIN')
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/offline_main.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/offline_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     sig = pyqtSignal(str)
 
     def __init__(self, test_config_path=None, *args, **kwargs):
 
         # init communication between classes
         self.test_start_event = threading.Event()
         self.test_end_event = threading.Event()
+        self.validation_end_event = threading.Event()
         self.stop_app_event = threading.Event()
         self.exception_q = Queue(maxsize=MainDefaults.MAX_QUEUE_SIZE)
         self.tag_results_queue = Queue(maxsize=MainDefaults.MAX_QUEUE_SIZE)
 
         # init test parameters including tests suites
         self.test_parameters = TestParameters()
 
@@ -161,15 +162,17 @@
         self.test_logger.update_log_config({**self.external_hw_config, **self.print_config})
 
         # run application
         self.tag_testing = None
         self.print_log_validation = None
         self.tag_testing_thread = None
         self.print_log_validation_thread = None
-        self.moh_obj = ManualOperationHandle(exception_queue=self.exception_q, logger_name=self.logger.name)
+        self.r2r_obj = None
+        self.moh_obj = ManualOperationHandle(exception_queue=self.exception_q, logger_name=self.logger.name,
+                                             is_gw_r2r=False)
         self.gw_version = ''
         self.run_app()
 
         # run GUI:
         self.tested = None
         self.text_box = None
         self.data_line = None
@@ -216,48 +219,64 @@
 
         return tag_print_config
 
     def run_app(self):
         # init all classes
         self.tag_testing = TagTesting(test_start_event=self.test_start_event,
                                       test_end_event=self.test_end_event,
+                                      validation_end_event=self.validation_end_event,
                                       stop_app_event=self.stop_app_event,
                                       moh_object=self.moh_obj,
                                       exception_queue=self.exception_q,
                                       tag_results_queue=self.tag_results_queue,
                                       log_obj=self.test_logger,
+                                      test_object=self.test_parameters,
                                       user_config=self.user_config,
                                       hw_config=self.external_hw_config)
         if not self.tag_testing.is_init:
             err = self.moh_obj.get_all_exceptions()
             raise Exception(f'Got the following errors during TagTesting init:\n{err}')
-
+        self.moh_obj.set_is_gw_r2r(self.tag_testing.is_r2r)
         self.print_log_validation = PrintingAndValidation(test_start_event=self.test_start_event,
                                                           test_end_event=self.test_end_event,
+                                                          validation_end_event=self.validation_end_event,
                                                           stop_app_event=self.stop_app_event,
                                                           moh_object=self.moh_obj,
                                                           exception_queue=self.exception_q,
                                                           tag_results_queue=self.tag_results_queue,
                                                           log_obj=self.test_logger,
                                                           test_object=self.test_parameters,
                                                           user_config=self.user_config,
-                                                          gw_version=self.tag_testing.get_gw_version())
+                                                          gw_version=self.tag_testing.get_gw_version(),
+                                                          get_duplicated_tags=self.tag_testing.get_all_duplicated_tags)
         if not self.print_log_validation.is_init:
             err = self.moh_obj.get_all_exceptions()
             raise Exception(f'Got the following errors during PrintingAndValidation init:\n{err}')
+        # set r2r counter:
+        self.r2r_obj = self.tag_testing.r2r if self.tag_testing.is_r2r else self.print_log_validation.r2r
+        self.set_r2r_configuration()
 
         # open threads for all classes
         self.tag_testing_thread = threading.Thread(target=self.tag_testing.run)
         self.print_log_validation_thread = threading.Thread(target=self.print_log_validation.run)
 
         self.tag_testing_thread.start()
         self.print_log_validation_thread.start()
 
         self.gw_version = self.tag_testing.get_gw_version()
 
+    def set_r2r_configuration(self):
+        if self.tag_testing.is_r2r:
+            self.print_log_validation.set_r2r_counter_func(self.tag_testing.r2r.get_counter)
+            # update instruction strings
+            for lan in moh_instruction[MohType.ARDUINO_ERROR.value].keys():
+                moh_instruction[MohType.ARDUINO_ERROR.value][lan] = \
+                    [s.replace('Arduino', 'Gateway') for s in moh_instruction[MohType.ARDUINO_ERROR.value][lan]]
+            self.logger.info('Gateway working instead of Arduino')
+
     @pyqtSlot(str)
     def append_debug(self, string):
         self.text_box.appendPlainText(string)  # +'\n')
 
     def open_ui(self, wiliot_ver, gw_version):
         """
         opens the run main GUI that will present the run data and gives to the user ability to Stop/Continue/Pause
@@ -411,26 +430,26 @@
             return True
         return False
 
     @staticmethod
     def calculate_yield_over_time(is_passed_list):
         yield_over_time = \
             [sum(is_passed_list[x - MainDefaults.CALCULATE_ON:x]) / MainDefaults.CALCULATE_ON * 100
-                           for x in range(MainDefaults.CALCULATE_ON, len(is_passed_list), MainDefaults.CALCULATE_INTERVAL)]
+             for x in range(MainDefaults.CALCULATE_ON, len(is_passed_list), MainDefaults.CALCULATE_INTERVAL)]
         return yield_over_time
 
     def gui_run(self):
 
         try:
 
             if self.stop_app_event.is_set():
                 self.exit()
                 return
 
-            tested = self.tag_testing.get_tested()
+            tested = self.tag_testing.get_tested() - 1
             passed = self.tag_testing.get_passed()
             is_passed_list = self.tag_testing.get_is_passed_list()
             responded = self.tag_testing.get_responded()
             missing_labels = self.tag_testing.get_missing_label_count()
             self.reel_label.setText("Reel Name: " + self.test_logger.get_reel_name())
 
             if tested == 0:
@@ -476,15 +495,15 @@
             continue_run = False
             if exceptions_status['moh_type'] == MohType.MISSING_LABEL:
                 is_end_of_run = self.end_of_run_pop_up()
             if not is_end_of_run:
                 continue_run = \
                     self.moh_obj.moh_pop_up(
                         moh_type=exceptions_status['moh_type'],
-                                                       error_code=exceptions_status['error_code'],
+                        error_code=exceptions_status['error_code'],
                         msg=exceptions_status['exception_str'],
                         scan_again_func=self.print_log_validation.update_scanning_results_after_exception
                         if self.print_log_validation.is_scanner else None)
             self.restart_run_after_moh(continue_run)
             exceptions_status = self.moh_obj.handle_exceptions()
 
             if not continue_run:
@@ -494,21 +513,22 @@
         self.moh_obj.set_moh_is_needed(False)
         self.update_timer.start()
 
     def restart_run_after_moh(self, continue_run):
         self.logger.info('Start the run after MOH')
         is_print = self.user_config['toPrint'].lower() == 'yes'
         is_scanner = self.user_config['QRRead'].lower() == 'yes'
-        is_r2r = self.user_config['isR2R'].lower() == 'yes' if 'isR2R' in self.user_config else True
+        is_r2r = self.user_config['isR2R'].lower() == 'yes'
         try:
+            self.tag_testing.gw_reset_and_config()
             if is_r2r:
-                self.print_log_validation.r2r.reconnect()
-                self.print_log_validation.r2r.send_start_to_r2r()
+                self.r2r_obj.reconnect()
+                self.r2r_obj.send_start_to_r2r()
                 if not continue_run:
-                    self.print_log_validation.r2r.end_of_run()
+                    self.r2r_obj.end_of_run()
             if is_print:
                 self.print_log_validation.printer.init_printer_hw_connection()
             if is_scanner:
                 self.print_log_validation.scanner.reconnect()
 
         except Exception as e:
             self.exception_q.put(f'Main Exception: run: state{MainStates.RESTART_AFTER_MOH.name}: {e}', block=False)
@@ -609,16 +629,18 @@
             self.logger.info('Waiting for Printing Log and Validation thread to stop all processes...')
             self.print_log_validation_thread.join()
             self.logger.info('Printing Log and Validation thread was done')
 
     def exit(self):
         self.stop_app_event.set()
         try:
-            if self.print_log_validation.get_validation_q_maxsize() > 1:
-                self.timed_popup('Finishing validation process - wait until all tags will be verified', 20)
+            offset_size = self.print_log_validation.get_validation_q_maxsize()
+            if offset_size > 1:
+                self.timed_popup(msg='Finishing validation process - wait until all tags will be verified',
+                                 wait_time=offset_size * 5)
             self.stop_app()
             self.moh_obj.get_all_exceptions()
             self.upload_data_to_cloud_and_summary()
         except Exception as e:
             self.logger.warning(f'Main: exit: Got Exception during upload data: [{e}]\n'
                                 f'please make sure data was uploaded')
         self.update_timer.stop()
@@ -718,36 +740,40 @@
         external_hw_config_path = os.path.join(self.dir_config, 'test_configs.json')
         external_hw_config_values = open_json_cache(self.dir_config, external_hw_config_path,
                                                     config_defaults.get_external_hw_defaults())
         return {**printer_config_values, **external_hw_config_values}
 
 
 class ManualOperationHandle(object):
-    def __init__(self, exception_queue, logger_name):
+    def __init__(self, exception_queue, logger_name, is_gw_r2r):
         """
 
         @param exception_queue:
         @type exception_queue: Queue
         """
         self.exception_q = exception_queue
         self.logger = logging.getLogger(logger_name)
         self.is_moh_needed = False
+        self.is_gw_r2r = is_gw_r2r
         self.critical_moh_types = []
         self.set_critical_errors()
 
     def set_critical_errors(self):
         self.critical_moh_types = [MohType.GENERAL_ERROR, MohType.FILES_ERROR, MohType.STOP_CRITERIA,
                                    MohType.NO_PRINTER_ACK]
 
     def get_manual_operation_is_needed(self):
         return self.is_moh_needed or not self.exception_q.empty()
 
     def set_moh_is_needed(self, is_needed):
         self.is_moh_needed = is_needed
 
+    def set_is_gw_r2r(self, is_r2r):
+        self.is_gw_r2r = is_r2r
+
     @staticmethod
     def error_code_to_moh(error_code):
         if compare_error_code(error_code, ErrorCode.TagTesting.value, 0) and \
                 compare_error_code(error_code, TagStates.GET_TRIGGER.value, 2):
             moh_type = MohType.MISSING_LABEL
         elif compare_error_code(error_code, ErrorCode.Main.value, 0) and \
                 compare_error_code(error_code, MainStates.STOP_CRITERIA.value, 2):
@@ -830,17 +856,19 @@
         language_code = MainDefaults.DEFAULT_LANGUAGE    # Default to English
         instructions_str = moh_instruction[moh_type.value][language_code] \
             if moh_type.value in moh_instruction and language_code in moh_instruction[moh_type.value] \
             else ['error instructions are not available']
 
         button_layout = [
             [Sg.Button(lang_code, key=lang_name, size=(3, 1)) for lang_name, lang_code in lang_map.items()]]
-
+        moh_name = moh_type.value
+        if self.is_gw_r2r:
+            moh_name = moh_name.replace('Arduino', 'Gateway')
         layout = [[Sg.Text('Manual Handling is Needed!', font=(font, font_size), justification='center')],
-                  [Sg.Text(moh_type.value, font=(font, font_size), justification='center')],
+                  [Sg.Text(moh_name, font=(font, font_size), justification='center')],
                   [Sg.Text('')],
                   [Sg.Text(f'Instructions:', key='Instructions', font=(font, font_size, 'bold underline '))],
                   *button_layout,
                   [Sg.Text('\n'.join(instructions_str), font=(font, font_size, 'bold'), key='-INSTRUCTIONS-',
                            justification='right' if language_code == 'he' else 'left')],
                   [Sg.Text('')],
                   [Sg.Text(f'ErrorCode:{error_code}', font=(font, font_size), justification='center')],
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/utils/barcode_test.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/utils/barcode_test.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/utils/env_install.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/utils/env_install.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/utils/offline_log_editing.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/utils/offline_log_editing.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/offline/utils/tadbik_r2r_controller.py` & `wiliot-testers-5.4.13/wiliot_testers/offline/utils/tadbik_r2r_controller.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/partners/avery_dennison/simple_test.py` & `wiliot-testers-5.4.13/wiliot_testers/partners/simple_test/simple_test.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/partners/avery_dennison/test_upload_get_AD.py` & `wiliot-testers-5.4.13/wiliot_testers/partners/simple_test/test_upload_get_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import PySimpleGUI as sg
 import threading
 from wiliot_testers.utils.ppfp_tool import DataPullGUI
-from wiliot_testers.partners.avery_dennison.simple_test import SimpleTest
+from wiliot_testers.partners.simple_test.simple_test import SimpleTest
 
-OWNER_ID = 'averydennison_rfid'
+OWNER_ID = ''
 
 
 def custom_progress_bar(window, title, total_time, shared_status):
     layout = [[sg.Text(title, key='-STATUS-')],
               [sg.ProgressBar(total_time, orientation='h', size=(20, 20), key='-PROGRESS-')],
               [sg.Cancel()]]
 
@@ -65,15 +65,15 @@
         [sg.Text('Test Name', visible=False), sg.InputText(key='cloud_test_name', visible=False)],
         [sg.Text('Output Directory', visible=False), sg.InputText(key='cloud_output_dir', visible=False)],
         [sg.Button('Get Results')]]
 
     layout = [
         [sg.Column(left_layout), sg.VSeparator(), sg.Column(right_layout)]]
 
-    window = sg.Window('AD GUI', layout, size=(450, 250))
+    window = sg.Window('GUI', layout, size=(450, 250))
 
     shared_status = {'test_complete': False, 'test': None, 'upload_complete': False}
 
     while True:
         event, values = window.read()
         if event == sg.WIN_CLOSED:
             break
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/com_connect.py` & `wiliot-testers-5.4.13/wiliot_testers/sample/com_connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,19 +53,20 @@
 #     FOR ANY LOSS OF USE OR DATA OR BUSINESS INTERRUPTION, AND/OR FOR ANY ECONOMIC LOSS
 #     (SUCH AS LOST PROFITS, REVENUE, ANTICIPATED SAVINGS). THE FOREGOING SHALL APPLY:
 #     (A) HOWEVER CAUSED AND REGARDLESS OF THE THEORY OR BASIS LIABILITY, WHETHER IN
 #     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
+import os.path
 from threading import Thread
 import logging
 import threading
 from tkinter import *
-from serial import tools
+import serial.tools.list_ports
 import pygubu
 from os.path import abspath
 from json import dump
 from os.path import join, dirname
 from wiliot_testers.test_equipment import *
 from wiliot_core import WiliotGateway, ActionType, DataType
 from wiliot_testers.sample.configs_gui import CONFIGS_DIR
@@ -73,27 +74,27 @@
 barcodeMutex = threading.Lock()
 
 CONNECT_HW = 'Connect HW'
 GO = 'Go'
 CONTINUE = 'Continue'
 READ = 'Read'
 FINISH = 'Finish'
-SEND = 'Send'
 
 ADD = 'ADD'
 REMOVE = 'REMOVE'
 
 GW_CANCEL = '!reset'
 
 # gateway
 GW_VERSION = 'Gateway version: '
 GW_AVAILABLE_VERSION = 'Available Version: '
 
 # attenuator
 ATTENUATION = 'atten'
+ATTENUATION_PARAMS = ['attenBle', 'attenLoRa']
 
 BLE = 'Ble'
 LORA = 'LoRa'
 
 BARCODES = 'Barcodes'
 ATTENUATORS = 'Atten'
 CHAMBERS = 'Chambers'
@@ -129,24 +130,27 @@
     chambers_to_close = []
     gw_latest_version = ['']
     gw_update_status = 'disabled'
     start_time = 0
     temperature_sensor_readings = []
     all_sensors = []
     ttk = None
+    logger_dir = ''
 
-    def __init__(self, top_builder=None, new_tag_func=None, update_go=None, default_dict=None, logger=None):
+    def __init__(self, top_builder=None, new_tag_func=None, update_go=None, default_dict=None, logger=None,
+                 logger_dir=None, tk_frame=None):
         '''
         Constructor
         '''
-        self.gateway = WiliotGateway(logger_name='sample')
+        self.logger_dir = logger_dir
         self.top_builder = top_builder
         self.add_tag_to_test = new_tag_func
         self.update_go_state = update_go
         self.default_dict = default_dict
+        self.tk_frame = tk_frame
         if logger is None:
             self.logger = logging.getLogger('sample')
         else:
             self.logger = logger
 
     def __del__(self):
         if self.gateway is not None and self.is_gw_serial_open():
@@ -165,50 +169,47 @@
         self.chambers_serials = {}
 
         for com_port, atten in self.atten_serials.items():
             if atten != None and 'serial' in atten.keys() and atten['serial'] != None and atten:
                 atten['serial'].GetActiveTE().close_port()
         self.atten_serials = {}
 
-    def gui(self, ttk_frame=None):
+    def gui(self):
         self.builder = builder = pygubu.Builder()
         ui_file = join(abspath(dirname(__file__)), 'utils', 'com_connect.ui')
         self.builder.add_from_file(ui_file)
 
         img_path = join(abspath(dirname(__file__)), '')
         builder.add_resource_path(img_path)
         img_path = join(abspath(dirname(__file__)), 'utils')
         builder.add_resource_path(img_path)
 
-        self.ttk = ttk_frame
+        if self.tk_frame is not None:
+            self.ttk = Toplevel(self.tk_frame)
+        else:
+            self.ttk = Tk()
 
         self.ttk.title("ComConnect")
 
         self.mainwindow = self.builder.get_object('mainwindow', self.ttk)
 
         self.builder.connect_callbacks(self)
         self.isGui = True
-        self.find_com_ports()
+        self.find_com_ports_cb()
         self.set_gui_defaults()
 
         self.ttk.protocol("WM_DELETE_WINDOW", self.close)
         self.ttk.lift()
         self.ttk.attributes("-topmost", True)
         self.ttk.attributes("-topmost", False)
 
         # self.set_gui_defaults()
 
         self.ttk.mainloop()
 
-    def find_com_ports(self, *args):
-        com_ports = serial_ports()
-        available_ports = [com_port for com_port in com_ports if com_port not in self.used_ports]
-
-        self.update_com_gui(available_ports, com_ports)
-
     def set_gui_defaults(self):
 
         if self.serials_connected(CHAMBERS):
             self.builder.get_object('connect_chambers').configure(text='Disconnect')
             self.builder.get_object('chosenChambers')['state'] = 'disabled'
             self.builder.get_object('availableChambers')['state'] = 'disabled'
             self.builder.get_object('chambers_up')['state'] = 'disabled'
@@ -325,18 +326,17 @@
         else:
             self.builder.get_object(f'connect_atten').configure(text='Connect')
             self.builder.get_object(f'attenComLoRa')['state'] = 'normal'
             self.builder.get_object(f'attenComBle')['state'] = 'normal'
 
     def choose_com_ports(self):
         default_dict = self.default_dict
-        com_ports = [s.device for s in tools.list_ports.comports()]
+        com_ports = [comport.device for comport in serial.tools.list_ports.comports()]
         if len(com_ports) == 0:
-            com_ports = [s.name for s in tools.list_ports.comports()]
-
+            com_ports = [s.name for s in serial.tools.list_ports.comports()]
         if 'gw' in default_dict.keys() and default_dict['gw'] in com_ports:
             self.gw_com_port = [default_dict['gw']]
             self.used_ports.append(default_dict['gw'])
         else:
             self.gw_com_port = ['']
             self.missing_com_port = True
         if 'atten' in default_dict.keys() and BLE in default_dict['atten'].keys() and default_dict['atten'][BLE] \
@@ -378,59 +378,39 @@
         if 'chambers' in default_dict.keys():
             missing_chambers = [chamber for chamber in default_dict['chambers'] if chamber not in com_ports]
         if any(missing_barcodes + missing_chambers):
             self.missing_com_port = True
 
         return self.missing_com_port
 
-    def choose_gw(self, *args):
-        if len(self.gw_com_port) > 0 and self.gw_com_port[0] != '':
-            self.used_ports.pop(self.used_ports.index(self.gw_com_port[0]))
-        self.gw_com_port = [self.builder.get_object('gwCom').get()]
-        self.used_ports.append(self.gw_com_port[0])
-
-    def choose_ble_atten(self, *args):
-        ble_com = self.builder.get_object('attenComBle').get()
-        ble_last_com = [com for com, item in self.atten_serials.items() if item['type'] == BLE]
-        if len(ble_last_com) > 0:
-            self.atten_serials.pop(ble_last_com[0])
-            self.used_ports.pop(self.used_ports.index(ble_last_com[0]))
-        if ble_com.strip() != '':
-            self.atten_serials[ble_com] = {}
-            self.atten_serials[ble_com]['type'] = BLE
-            self.atten_serials[ble_com]['serial'] = None
-            self.used_ports.append(ble_com)
-
-    def choose_lora_atten(self, *args):
-        lora_com = self.builder.get_object('attenComLoRa').get()
-        lora_last_com = [com for com, item in self.atten_serials.items() if item['type'] == LORA]
-        if len(lora_last_com) > 0:
-            self.atten_serials.pop(lora_last_com[0])
-            self.used_ports.pop(self.used_ports.index(lora_last_com[0]))
-        if lora_com.strip() != '':
-            self.atten_serials[lora_com] = {}
-            self.atten_serials[lora_com]['type'] = LORA
-            self.atten_serials[lora_com]['serial'] = None
-            self.used_ports.append(lora_com)
+    def init_gw(self):
+        return WiliotGateway(logger_name=self.logger.name, is_multi_processes=True,
+                             mp_reset_time_upon_gw_start=True,
+                             np_max_packet_in_buffer_before_error=10,
+                             log_dir_for_multi_processes=self.logger_dir)
 
     def connect_all(self, gui=True):
+        if self.gateway is None:
+            self.gateway = self.init_gw()
         if not self.is_gw_serial_open():
             success = self.connect_gw(gui)
             if not success:
                 return
         if not self.serials_connected(ATTENUATORS):
             self.connect_atten(gui)
         if not self.serials_connected(BARCODES):
             self.connect_barcodes(gui)
         if not self.serials_connected(CHAMBERS):
             self.connect_chambers(gui)
         self.connect_temperature_sensor()
         self.hwConnected = True
 
     def connect_gw(self, gui=True, disconnect=False):
+        if self.gateway is None:
+            self.gateway = self.init_gw()
         if not self.is_gw_serial_open() and not disconnect:
             if len(self.gw_com_port) == 0 or self.gw_com_port[0].strip() == '':
                 self.popup_message('No default com port for GW, please choose GW com port.', title='Error', log='error')
                 return False
             com_port = self.gw_com_port[0]
             self.gateway.open_port(port=com_port, baud=921600)
             if self.is_gw_serial_open():
@@ -520,15 +500,15 @@
                 try:
                     self.builder.get_object(f'chosen{obj}')['state'] = 'disabled'
                     self.builder.get_object(f'available{obj}')['state'] = 'disabled'
                     self.builder.get_object(f'add{obj}')['state'] = 'disabled'
                 except:
                     pass
         if gui:
-            self.find_com_ports()
+            self.find_com_ports_cb()
         # self.update_go_state()
         return is_connected
 
     def open_serials(self, obj, serials):
         threads = []
         for com_port, com_serial in serials.items():
             if 'barcode' in obj.lower():
@@ -563,41 +543,25 @@
             self.enable_hw_connected()
         if self.isGui:
             self.isGui = False
             self.ttk.destroy()
         return self.hwConnected
 
     def save(self):
-        # default_dict = {}
-        # if isfile(join(CONFIGS_DIR, '.defaults.json')):
-        #     with open(join(CONFIGS_DIR, '.defaults.json'), 'r') as defaultComs:
-        #         default_dict = load(defaultComs)
         self.default_dict['gw'] = self.gw_com_port[0]
         self.default_dict['atten'] = {}
         for com_port, atten in self.atten_serials.items():
             self.default_dict['atten'][atten['type']] = com_port
         self.default_dict['barcodes'] = list(self.barcodes_serials.keys())
         self.default_dict['chambers'] = list(self.chambers_serials.keys())
         with open(join(CONFIGS_DIR, '.defaults.json'), 'w+') as defaultComs:
             dump(dict(self.default_dict), defaultComs, indent=4)
 
         self.logger.info(f'Com ports saved successfully.')
 
-    def focus_barcode_available(self, *args):
-        self.focus_available(BARCODES)
-
-    def focus_barcode_chosen(self, *args):
-        self.focus_chosen(BARCODES)
-
-    def focus_chamber_available(self, *args):
-        self.focus_available(CHAMBERS)
-
-    def focus_chamber_chosen(self, *args):
-        self.focus_chosen(CHAMBERS)
-
     def focus_available(self, obj):
         self.builder.get_object(f'add{obj}').configure(text='>')
         setattr(self, f'{obj.lower()}_state', ADD)
 
     def focus_chosen(self, obj):
         self.builder.get_object(f'add{obj}').configure(text='<')
         setattr(self, f'{obj.lower()}_state', REMOVE)
@@ -607,19 +571,19 @@
         if getattr(self, f'{BARCODES.lower()}_state') == ADD:
             com_chosen = self.builder.get_object(f'available{BARCODES}').get(ACTIVE)
             try:
                 temp_barcode = BarcodeScanner(com_port=com_chosen)
             except Exception as e:
                 self.popup_message(f'Could NOT connect. {e}', title='Error', log='error')
         self.add(BARCODES)
-        self.find_com_ports()
+        self.find_com_ports_cb()
 
     def add_chamber(self):
         self.add(CHAMBERS)
-        self.find_com_ports()
+        self.find_com_ports_cb()
 
     def add(self, obj):
         if getattr(self, f'{obj.lower()}_state') == ADD:
             sending = self.builder.get_object(f'available{obj}')
             receiving = self.builder.get_object(f'chosen{obj}')
         else:
             sending = self.builder.get_object(f'chosen{obj}')
@@ -737,55 +701,55 @@
             # if com_port.strip()=='':
             #     connected_serials += 1
         if connected_serials > 0 and connected_serials == len(serials.keys()):
             return True
         else:
             return False
 
-    def get_data(self, actionType=ActionType.ALL_SAMPLE, dataType=DataType.PACKET_LIST):
-        return self.gateway.get_packets(action_type=actionType, data_type=dataType)
-
     def read_barcode(self, scanner_index=0, close_chamber=False, add_to_test=False, n_try=5):
+        full_data, reel_id, gtin = None, None, None
         if len(list(self.barcodes_serials.values())) == 0:
             self.logger.error('Trying to read barcode but no scanner were connected')
             return None, None
         scanner = list(self.barcodes_serials.values())[scanner_index]
         for i in range(n_try):
             full_data, cur_id, reel_id, gtin = scanner.scan_ext_id()
             if full_data is None and cur_id is None and reel_id is None and full_data is None:
                 continue
             break
 
-        cur_id = cur_id if cur_id is not None else full_data
         reel_id = reel_id if reel_id is not None else full_data
         gtin = gtin if gtin is not None else ''
         if reel_id is not None:
             self.reel_id = reel_id
             self.gtin = gtin
-        if cur_id is None:
+        if full_data is None:
             barcodeMutex.acquire()
             if close_chamber:
                 self.barcode_error.append(scanner_index)
             barcodeMutex.release()
             return None, None
 
         if not close_chamber:
             reel_id_obj = self.top_builder.tkvariables.get('reelId')
             reel_id_obj.set(self.reel_id)
 
         else:
-            success = self.add_tag_to_test(cur_id, reel_id, scanner_index=scanner_index, add_to_test=add_to_test)
+            success = self.add_tag_to_test(full_data, reel_id, scanner_index=scanner_index, add_to_test=add_to_test)
             if success:
                 self.chambers_to_close.append(scanner_index)
 
-        return cur_id, reel_id
+        return full_data, gtin + reel_id
+
+    def get_all_scanners_index(self):
+        return list(range(len(self.barcodes_serials.values())))
 
     def read_scanners_barcodes(self, indexes=()):
         if len(indexes) == 0:
-            indexes = list(range(len(self.barcodes_serials.values())))
+            indexes = self.get_all_scanners_index()
         scanner_threads = []
         self.barcode_error = []
         self.chambers_to_close = []
 
         for i in indexes:
             t = threading.Thread(target=self.read_barcode, args=(i, True, True))
             scanner_threads.append(t)
@@ -794,38 +758,48 @@
             t = scanner_threads[i]
             t.join()
 
         read_message = ''
         title = 'Warning'
         font = 18
         if len(self.barcode_error) > 0:
-            read_message += f'Error reading external ID from chambers {self.barcode_error}, try repositioning the tags.\n'
+            read_message += f'Error reading external ID from chambers {self.barcode_error},' \
+                            f' try repositioning the tags.\n'
             title = 'Error'
             font = 16
 
         if len(self.chambers_to_close) > 0:
             read_message += f'Chambers are closing!!\nWatch your hands!!!'
 
-        popupThread = threading.Thread(target=self.popup_message,
-                                       args=(read_message, title, ("Helvetica", font), title.lower()))
-        popupThread.start()
-        popupThread.join()
+        self.popup_message(read_message, title, ("Helvetica", font), title.lower())
 
         if len(self.chambers_to_close) > 0:
             self.close_chambers(self.chambers_to_close)
 
         self.update_go_state()
 
     def enable_hw_connected(self):
         self.top_builder.get_object('read_qr')['state'] = 'normal'
         self.top_builder.get_object('reelId')['state'] = 'normal'
         if self.top_builder.tkvariables.get('go').get() == CONNECT_HW:
             self.top_builder.tkvariables.get('go').set(READ)
             self.top_builder.get_object('go')['state'] = 'disabled'
 
+    def set_attenuation(self, params):
+        for com_port, atten in self.atten_serials.items():  # BLE and/or Lora
+            try:
+                value = params[atten['type'].lower() + 'Attenuation']
+                attenuation = atten['serial'].GetActiveTE().Setattn(float(value))
+                self.logger.info(f"{atten['type']} Attenuation set to: {str(attenuation).strip()}")
+            except Exception as e:
+                err = f"{atten['type']} Attenuator error: try reconnect the attenuator [{e}].\n" \
+                      f"or params are not correct: {params.keys()}: [{e}]"
+                self.logger.error(err)
+                raise Exception(err)
+
     def send_gw_app(self, params):
         str_rsp = []
         self.gateway.reset_buffer()
         self.gateway.clear_rsp_str_input_q()
 
         self.gateway.reset_start_time()
 
@@ -879,14 +853,16 @@
     def get_gtin(self):
         return self.gtin
 
     def get_reel_external(self):
         return self.gtin + self.reel_id
 
     def is_gw_serial_open(self):
+        if self.gateway is None:
+            return False
         serial_open, _, _ = self.gateway.get_connection_status()
         return serial_open
 
     def is_gw_data_available(self):
         return self.gateway.is_data_available()
 
     def is_gui_opened(self):
@@ -975,7 +951,57 @@
             popup.destroy()
 
         label = Label(popup, text=msg, font=font)
         label.pack(side="top", fill="x", padx=10, pady=10)
         b1 = Button(popup, text="Okay", command=popup_exit)
         b1.pack(padx=10, pady=10)
         popup.mainloop()
+
+    # ############## GUI Callbacks  #######################
+
+    def find_com_ports_cb(self, *args):
+        com_ports = serial_ports()
+        available_ports = [com_port for com_port in com_ports if com_port not in self.used_ports]
+
+        self.update_com_gui(available_ports, com_ports)
+
+    def focus_barcode_available_cb(self, *args):
+        self.focus_available(BARCODES)
+
+    def focus_barcode_chosen_cb(self, *args):
+        self.focus_chosen(BARCODES)
+
+    def focus_chamber_available_cb(self, *args):
+        self.focus_available(CHAMBERS)
+
+    def focus_chamber_chosen_cb(self, *args):
+        self.focus_chosen(CHAMBERS)
+
+    def choose_gw_cb(self, *args):
+        if len(self.gw_com_port) > 0 and self.gw_com_port[0] != '':
+            self.used_ports.pop(self.used_ports.index(self.gw_com_port[0]))
+        self.gw_com_port = [self.builder.get_object('gwCom').get()]
+        self.used_ports.append(self.gw_com_port[0])
+
+    def choose_ble_atten_cb(self, *args):
+        ble_com = self.builder.get_object('attenComBle').get()
+        ble_last_com = [com for com, item in self.atten_serials.items() if item['type'] == BLE]
+        if len(ble_last_com) > 0:
+            self.atten_serials.pop(ble_last_com[0])
+            self.used_ports.pop(self.used_ports.index(ble_last_com[0]))
+        if ble_com.strip() != '':
+            self.atten_serials[ble_com] = {}
+            self.atten_serials[ble_com]['type'] = BLE
+            self.atten_serials[ble_com]['serial'] = None
+            self.used_ports.append(ble_com)
+
+    def choose_lora_atten_cb(self, *args):
+        lora_com = self.builder.get_object('attenComLoRa').get()
+        lora_last_com = [com for com, item in self.atten_serials.items() if item['type'] == LORA]
+        if len(lora_last_com) > 0:
+            self.atten_serials.pop(lora_last_com[0])
+            self.used_ports.pop(self.used_ports.index(lora_last_com[0]))
+        if lora_com.strip() != '':
+            self.atten_serials[lora_com] = {}
+            self.atten_serials[lora_com]['type'] = LORA
+            self.atten_serials[lora_com]['serial'] = None
+            self.used_ports.append(lora_com)
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/configs/.default_test_configs.json` & `wiliot-testers-5.4.13/wiliot_testers/sample/configs/.default_test_configs.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9882352941176471%*

 * *Differences: {"'TIKI_LORA'": "{'attenLoRa': '24.5', 'EmulateSurface': 'simulate cardboard', "*

 * *                "'EmulateSurfaceValue': 923000}"}*

```diff
@@ -68,18 +68,19 @@
         "testTime": "90",
         "test_responding_min": "",
         "test_tbp_max": "",
         "test_tbp_min": "",
         "test_valid_tbp": ""
     },
     "TIKI_LORA": {
-        "EmulateSurface": "no simulation",
+        "EmulateSurface": "simulate cardboard",
+        "EmulateSurfaceValue": 923000,
         "antennaType": "TIKI",
         "attenBle": "17",
-        "attenLoRa": "25",
+        "attenLoRa": "24.5",
         "channel": "37",
         "pattern": "50",
         "sleep": "0",
         "tOn": "8",
         "tTotal": "20",
         "tag_tbp_max": "",
         "tag_tbp_min": "",
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/configs_gui.py` & `wiliot-testers-5.4.13/wiliot_testers/sample/configs_gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,206 +55,209 @@
 #     (A) HOWEVER CAUSED AND REGARDLESS OF THE THEORY OR BASIS LIABILITY, WHETHER IN
 #     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 from shutil import copyfile
 from os import makedirs
-import logging
 import pygubu
+from tkinter import Tk, Toplevel
 from os.path import join, abspath, dirname, isfile, isdir
 from json import dump, load
 from copy import deepcopy
 from wiliot_core import WiliotDir
 from wiliot_testers.utils.get_version import get_version
 
+TESTER_NAME = 'sample'
 VER = get_version()
 MEASURED = {'button': 'Measured', 'label': '[meter]'}
 MANUAL = {'button': 'Manual', 'label': '[db]'}
 DEFAULT_EMULATED_SURFACE = 'no simulation'
 
-wiliot_env = WiliotDir()
-sample_test_dir = abspath(join(wiliot_env.get_common_dir(), 'sample_test'))
+wiliot_dir = WiliotDir()
+wiliot_dir.create_tester_dir(TESTER_NAME)
+sample_test_dir = wiliot_dir.get_tester_dir(TESTER_NAME)
 OUTPUT_DIR = abspath(join(sample_test_dir, 'logs'))
 CONFIGS_DIR = abspath(join(sample_test_dir, 'configs'))
 if not isdir(abspath(join(OUTPUT_DIR))):
     makedirs(abspath(join(OUTPUT_DIR)))
 if not isdir(abspath(join(CONFIGS_DIR))):
     makedirs(abspath(join(CONFIGS_DIR)))
 
 
 class ConfigsGui(object):
-    '''
-    classdocs
-    '''
-    isGui = False
+    is_gui = False
     atten_cur_mode = MANUAL
     test_config = ''
     config = ''
-    configsDict = {}
+    configs_test = {}
     paramDict = {}
     defaultConfigsDict = {}
-    defaultSurfacesDict = {}
+    default_surfaces = {}
     all_configs_fields = []
+    builder = None
+    ttk = None
+    mainwindow = None
     
-    def __init__(self, top_builder=None):
-        '''
-        Constructor
-        '''
+    def __init__(self, top_builder=None, tk_frame=None):
         self.top_builder = top_builder
+        self.tk_frame = tk_frame
         self.config_path = abspath(join(dirname(__file__), 'configs', '.default_test_configs.json'))
         if isfile(self.config_path):
             with open(self.config_path, 'r') as jsonFile:
-                self.configsDict = load(jsonFile)
-                if len(self.configsDict):
-                    self.all_configs_fields = list(self.configsDict[next(iter(self.configsDict))].keys())
+                self.configs_test = load(jsonFile)
+                if len(self.configs_test):
+                    self.all_configs_fields = list(self.configs_test[next(iter(self.configs_test))].keys())
             self.fix_antenna_type()
 
         with open(abspath(join(dirname(__file__), 'configs', '.default_surfaces.json')), 'r') as jsonFile:
-            self.defaultSurfacesDict = load(jsonFile)
+            self.default_surfaces = load(jsonFile)
 
         self.copy_config_file()
 
     def copy_config_file(self):
         copyfile(self.config_path, abspath(join(CONFIGS_DIR, f'.default_test_configs(ViewOnly)_{VER}.json')))
 
-    def gui(self, ttk_frame=None):
+    def gui(self):
         self.builder = builder = pygubu.Builder()
         ui_file = abspath(join(abspath(dirname(__file__)), 'utils', 'configs.ui'))
         self.builder.add_from_file(ui_file)
         
         img_path = abspath(join(abspath(dirname(__file__)), ''))
         builder.add_resource_path(img_path)
         img_path = abspath(join(abspath(dirname(__file__)), 'utils'))
         builder.add_resource_path(img_path)
-        
-        self.ttk = ttk_frame
-        
+
+        if self.tk_frame is not None:
+            self.ttk = Toplevel(self.tk_frame)
+        else:
+            self.ttk = Tk()
+
         self.ttk.title("Sample Test Configs")
         
         self.mainwindow = self.builder.get_object('mainwindow', self.ttk)
         
         self.builder.connect_callbacks(self)
         
-        self.ttk.protocol("WM_DELETE_WINDOW", self.close)
+        self.ttk.protocol("WM_DELETE_WINDOW", self.close_cb)
         self.ttk.lift()
         self.ttk.attributes("-topmost", True)
         self.ttk.attributes("-topmost", False)
         
         self.set_gui_defaults()
         
-        self.isGui = True
+        self.is_gui = True
         self.ttk.mainloop()
     
     def set_gui_defaults(self):
-        temp_dict = deepcopy(self.configsDict)
+        temp_dict = deepcopy(self.configs_test)
         self.builder.get_object('configsList')['values'] = [key for key, item in temp_dict.items()
                                                             if isinstance(item, dict)]
         if temp_dict.get(self.config):
             self.builder.get_object('configsList').set(self.config)
             self.top_builder.tkvariables.get('testTime').set(temp_dict[self.config]['testTime'])
             self.builder.get_object('EmulateSurface')['values'] = tuple(
-                self.defaultSurfacesDict['EmulateSurface'].keys())
+                self.default_surfaces['EmulateSurface'].keys())
             self.builder.get_object('EmulateSurface').set(DEFAULT_EMULATED_SURFACE)
             self.builder.get_object('antennaType')['values'] = ['TEO', 'TIKI']
             for param, value in temp_dict[self.config].items():
                 if self.builder.tkvariables.get(param) is not None:
                     self.builder.tkvariables.get(param).set(value)
                 else:
                     pass
         self.builder.get_object('save')['state'] = 'normal'
     
     def fix_antenna_type(self):
-        tempDict = deepcopy(self.configsDict)
+        tempDict = deepcopy(self.configs_test)
         for config, params in tempDict.items():
             if 'antennaType' in params.keys() and params['antennaType']:
                 fixedAntenna = 'TIKI' if params['antennaType'].lower() in ['dual', 'tiki'] else 'TEO'
-                self.configsDict[config]['antennaType'] = fixedAntenna
-    
-    def atten_mode(self):
-        self.atten_cur_mode = MEASURED if self.atten_cur_mode == MANUAL else MANUAL
-        self.builder.tkvariables.get('atten_mode').set(self.atten_cur_mode['button'])
-        ble_label = self.builder.tkvariables.get('attenBleLabel')
-        ble_label.set(ble_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
-        lora_label = self.builder.tkvariables.get('attenLoRaLabel')
-        lora_label.set(lora_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
-    
-    def close(self):
-        self.isGui = False
-        self.ttk.destroy()
-    
+                self.configs_test[config]['antennaType'] = fixedAntenna
+
     def is_gui_opened(self):
-        return self.isGui
+        return self.is_gui
     
     def get_params(self):
         return self.paramDict
     
     def get_configs(self):
-        temp_dict = deepcopy(self.configsDict)
+        temp_dict = deepcopy(self.configs_test)
         return temp_dict
     
     def set_params(self, test_config):
-        if test_config not in self.configsDict.keys():
-            config_options = list(self.configsDict.keys())
+        if test_config not in self.configs_test.keys():
+            config_options = list(self.configs_test.keys())
             test_config = config_options[0]
-        self.paramDict = self.configsDict[test_config].copy()
-        if 'EmulateSurface' in self.configsDict[test_config].keys():
-            surface = self.configsDict[test_config]['EmulateSurface']
-            self.paramDict['EmulateSurfaceValue'] = self.defaultSurfacesDict['EmulateSurface'][surface]
+        self.paramDict = self.configs_test[test_config].copy()
+        if 'EmulateSurface' in self.configs_test[test_config].keys():
+            surface = self.configs_test[test_config]['EmulateSurface']
+            self.paramDict['EmulateSurfaceValue'] = self.configs_test[test_config]['EmulateSurfaceValue'] = \
+                self.default_surfaces['EmulateSurface'][surface]
         self.top_builder.tkvariables.get('testTime').set(self.paramDict['testTime'])
     
     def set_default_config(self, test_config):
         self.test_config = test_config
         self.config = test_config
-    
-    def config_select(self, *args):
-        self.config = config = self.builder.get_object('configsList').get()
-        self.builder.get_object('save')['state'] = 'normal'
-        self.top_builder.get_object('test_config').set(config)
-        self.reset()
-    
+
     def config_set(self, config):
         self.config = config
         self.set_params(config)
-        if self.isGui:
+        if self.is_gui:
             self.builder.get_object('configsList').set(config)
             self.set_gui_defaults()
         # except BaseException:
         #     pass
-    
-    def save(self):
+
+    # ############## GUI Callbacks  #######################
+
+    def choose_antenna_type_cb(self, *args):
+        antenna = self.builder.tkvariables.get('antennaType').get()
+        antenna = 'TIKI' if antenna.lower() in ['dual', 'tiki'] else 'TEO'
+        self.builder.tkvariables.get('antennaType').set(antenna)
+
+    def reset_cb(self):
+        def_dict = deepcopy(self.defaultConfigsDict)
+        self.configs_test.update(def_dict)
+        self.set_gui_defaults()
+
+    def atten_mode_cb(self):
+        self.atten_cur_mode = MEASURED if self.atten_cur_mode == MANUAL else MANUAL
+        self.builder.tkvariables.get('atten_mode').set(self.atten_cur_mode['button'])
+        ble_label = self.builder.tkvariables.get('attenBleLabel')
+        ble_label.set(ble_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
+        lora_label = self.builder.tkvariables.get('attenLoRaLabel')
+        lora_label.set(lora_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
+
+    def close_cb(self):
+        self.is_gui = False
+        self.ttk.destroy()
+
+    def save_cb(self):
         self.config = config = self.builder.get_object('configsList').get()
 
-        if config not in self.configsDict.keys():
-            self.configsDict[config] = {}
+        if config not in self.configs_test.keys():
+            self.configs_test[config] = {}
 
         for param in self.all_configs_fields:
             value = self.builder.tkvariables.get(param)
             if value is not None:
-                self.configsDict[config][param] = value.get()
+                self.configs_test[config][param] = value.get()
             else:
-                self.configsDict[config][param] = ''
-        self.builder.get_object('configsList')['values'] = [key for key, item in self.configsDict.items()
+                self.configs_test[config][param] = ''
+        self.builder.get_object('configsList')['values'] = [key for key, item in self.configs_test.items()
                                                             if isinstance(item, dict)]
-        self.top_builder.get_object('test_config')['values'] = [key for key, item in self.configsDict.items()
+        self.top_builder.get_object('test_config')['values'] = [key for key, item in self.configs_test.items()
                                                                 if isinstance(item, dict)]
         self.top_builder.get_object('test_config').set(config)
-        
+
         with open(self.config_path, 'w+') as jsonFile:
-            dump(self.configsDict, jsonFile, indent=4)
+            dump(self.configs_test, jsonFile, indent=4)
         self.copy_config_file()
 
         self.set_params(config)
         print(f'{config} configuration saved successfully.')
-    
-    def reset(self):
-        def_dict = deepcopy(self.defaultConfigsDict)
-        self.configsDict.update(def_dict)
-        self.set_gui_defaults()
-    
-    def test_time_update(self, *args):
-        self.top_builder.tkvariables.get('testTime').set(self.builder.tkvariables.get('testTime').get())
-    
-    def choose_antenna_type(self, *args):
-        antenna = self.builder.tkvariables.get('antennaType').get()
-        antenna = 'TIKI' if antenna.lower() in ['dual', 'tiki'] else 'TEO'
-        self.builder.tkvariables.get('antennaType').set(antenna)
+
+    def config_select_cb(self, *args):
+        self.config = config = self.builder.get_object('configsList').get()
+        self.builder.get_object('save')['state'] = 'normal'
+        self.top_builder.get_object('test_config').set(config)
+        self.reset_cb()
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/get_temperature_sensor_name.py` & `wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/get_temperature_sensor_name.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/sample_chamber.py` & `wiliot-testers-5.4.13/wiliot_testers/sample/sample_chamber.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,14 @@
                     self.selected_test_suite = convert_test_suite()
 
             with open(abspath(join(config_dir, '.default_surfaces.json')), 'r') as defaultSurfaces:
                 surface_configs = json.load(defaultSurfaces)
                 self.default_freq = surface_configs['EmulateSurface'].get('no simulation', {})
                 self.surface_freq_shift = surface_configs['EmulateSurface'].get(self.surface, {})
 
-
         except Exception as e:
             if logger is not None:
                 logger.logger.error(f'Could not read configs: {e}')
             raise Exception(e)
 
         return logger
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/sample_test.py` & `wiliot-testers-5.4.13/wiliot_testers/sample/sample_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -53,209 +53,142 @@
 #     FOR ANY LOSS OF USE OR DATA OR BUSINESS INTERRUPTION, AND/OR FOR ANY ECONOMIC LOSS
 #     (SUCH AS LOST PROFITS, REVENUE, ANTICIPATED SAVINGS). THE FOREGOING SHALL APPLY:
 #     (A) HOWEVER CAUSED AND REGARDLESS OF THE THEORY OR BASIS LIABILITY, WHETHER IN
 #     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
-import json
-import logging
+import threading
 import tkinter
-from tkinter.font import Font
-
 import numpy
-from os import remove
 from os import makedirs, mkdir
 from tkinter import *
 from tkinter import ttk
 from tkinter import messagebox
+import pandas as pd
 import pygubu
-from threading import Thread, Lock
+from threading import Thread
 from time import sleep
 import time
-import csv
 import datetime
-from wiliot_testers.sample.configs_gui import ConfigsGui, OUTPUT_DIR, CONFIGS_DIR
-from wiliot_testers.sample.com_connect import ComConnect, GO, CONTINUE, CONNECT_HW, READ, SEND
-from traceback import print_exc
 from json import load, dump
-import argparse
-import sys
-from os.path import isfile, abspath, dirname, join, isdir, exists
+from os.path import isfile, abspath, dirname, join
+from enum import Enum
+
+from wiliot_core import InlayTypes
+from wiliot_testers.sample.configs_gui import ConfigsGui, OUTPUT_DIR, CONFIGS_DIR, TESTER_NAME
+from wiliot_testers.sample.com_connect import ComConnect, GO, CONTINUE, CONNECT_HW, READ
 from wiliot_testers.utils.get_version import get_version
-from wiliot_testers.tester_utils \
-    import setLogger, changeFileHandler, removeFileHandler, CsvLog, HeaderType, TesterName, StreamToLogger
-from wiliot_core import TagCollection, PacketList
-from wiliot_core import check_user_config_is_ok, InlayTypes, WiliotDir
-from wiliot_api import ManufacturingClient
 from wiliot_testers.config.unusable_inlays import UnusableInlayTypes
 from wiliot_testers.utils.upload_to_cloud_api import *
-from wiliot_testers.utils.wiliot_external_ids import is_external_id_valid
-from enum import Enum
 from wiliot_testers.wiliot_tester_tag_result import FailBinSample
+from wiliot_testers.wiliot_tester_log import WiliotTesterLog, dict_to_csv
+from wiliot_testers.sample.sample_slim import SampleRun, TagStatus
 
-addToDictMutex = Lock()
-calibMutex = Lock()
-recvDataMutex = Lock()
-timerMutex = Lock()
-mutex = Lock()
+RESOLVE_OWNER_ID = 'wiliot-ops'
+RESOLVE_ENV = 'prod'
 
+SEND = 'Send'
 STOP = 'Stop'
 FINISH = 'Finish'
-
-RAW = 'raw'
-TIME = 'time'
-
-DEF_NUM_OF_TAGS = 2
-
-CLOUD_TIMEOUT_POST = 10
-CLOUD_TIMEOUT_RESOLVE = 2
-
-SGTIN_PREFIX_DEFAULT = '(01)00850027865010(21)'
-
 RSSI_THR_DEFAULT = 80
-
-
-class SettingModeOptions(Enum):
-    SEND = 'Send to Cloud'
-    SEND_TEST = 'Send to Cloud [TEST]'
-    OFFLINE = 'Offline Mode'
-    CALIB = 'Test Calibration'
-    CALIB_OFFLINE = 'Test Calibration [OFFLINE]'
-
-
-class SampleException(Exception):
-    pass
+TIME_BETWEEN_CALIB_RUNS = 5  # seconds
+TAG_COUNTER_LEN = 4
 
 
 class FailureCodeSampleTest(Enum):
     NONE = 0
     PASS = 1  # Pass
     NO_RESPONSE = 3
     NO_TBP = 5
     HIGH_TBP_AVG = 7
     NOT_COMPLETED = 9
 
 
 class SampleTest(object):
-    goButtonState = CONNECT_HW
-    stopButtonState = STOP
-    client = None
-    comConnect = None
-    configsGui = None
-    comTtk = None
-    configsTtk = None
+    stop_event = threading.Event()
+    sample_run_obj = None
+    go_button_state = CONNECT_HW
+    stop_button_state = STOP
+    com_connect = None
+    configs_gui = None
     testBarcodesThread = None
-    finishThread = None
-    finishTestThread = None
+    finish_thread = None
     closeChambersThread = None
-    gatewayDataThread = None
-    timerThread = None
-    testFinished = True
+    timer_thread = None
     post_data = True
-    wiliotTags = False
-    forceCloseRequested = False
+    force_close_requested = False
     closeRequested = False
-    testGo = False
-    stopTimer = False
     closeListener = False
     is_test_pass = False
-    testConfig = ''
+    test_configs = ''
     reel_id = ''
-    gtin = ''
-    testDir = ''
     owner = ''
     station_name = ''
     pywiliot_version = ''
-    testTime = 0
-    # tagsCount = 0
-    testStartTime = 0
+    test_time = 0
     sleep = 0
     cur_atten = 0
     test_num = 0
-    defaultDict = {}
-    dataBaseDict = {}
-    runDataDict = {}
-    params = {}
-    test_barcodes = {}
-    barcodes_read = {}
-    tagsFinished = {}
-    packets_dict = {}
-    bad_advas = []
-    advas_dict = {}
-    total_bad_advas = []
-    add_to_dict_threads = []
-    unknown_packets = PacketList()
+    default_config = {}
+    run_data = {}
+    all_tags_in_test = {}
+    all_results = pd.DataFrame()
+    results_df = pd.DataFrame()
+    tags_under_test = {}
     antenna = ''
     low = 0
     high = 0
     step = 1
     n_repetitions = 1
-    logger = logging.getLogger('sample')
-
-    # numOfTags = ''
-    multiTag = TagCollection()
-
-    def __init__(self, calib=None, environment='prod', post_data=True, offline=False):
+    logger = logging.getLogger(TESTER_NAME)
 
+    def __init__(self):
+        global SEND
         self.test_is_running = False
         self.set_logger()
-        self.calib = calib
-        self.offline = offline
-        self.offline_tag_index = 0
-        self.environment = environment
-        self.post_data = post_data
-        if self.offline:
-            self.post_data = False
+        self.calib = False
+        self.offline = False
+        self.environment = 'prod'
+        self.post_data = True
 
         self.pywiliot_version = get_version()
         self.logger.info(f'PyWiliot version: {self.pywiliot_version}')
 
-        if isfile(abspath(join(CONFIGS_DIR, '.defaults.json'))):
-            with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'r') as defaultComs:
-                self.defaultDict = load(defaultComs)
+        defaults_file_path = abspath(join(CONFIGS_DIR, '.defaults.json'))
+        defaults_old_file_path = abspath(join(dirname(dirname(CONFIGS_DIR)),
+                                              'common', 'sample_test', 'configs', '.defaults.json'))
+        if isfile(defaults_file_path):
+            with open(defaults_file_path, 'r') as defaults:
+                self.default_config = load(defaults)
+        elif isfile(defaults_old_file_path):
+            with open(defaults_old_file_path, 'r') as defaults:
+                self.default_config = load(defaults)
 
         self.popup_login()
+        if self.calib or self.offline:
+            SEND = 'Log'
+            self.post_data = False
 
         self.builder = builder = pygubu.Builder()
+        self.ttk = Tk()
 
-        self.comConnect = ComConnect(top_builder=builder, new_tag_func=self.add_tag_to_test,
-                                     update_go=self.update_go_state, default_dict=self.defaultDict, logger=self.logger)
+        self.com_connect = ComConnect(top_builder=builder, new_tag_func=self.add_tag_to_test,
+                                      update_go=self.update_go_state, default_dict=self.default_config,
+                                      logger=self.logger,
+                                      logger_dir=self.log_obj.log_path, tk_frame=self.ttk)
         self.update_data()
-        if not self.offline:
-            _, api_key, is_success = check_user_config_is_ok(env='prod', owner_id=self.owner)
-            if not is_success:
-                self.logger.warning('invalid User credential')
-                return
-            self.client = ManufacturingClient(api_key=api_key, logger_='root', env='prod')
-        self.configsGui = ConfigsGui(top_builder=builder)
+        self.configs_gui = ConfigsGui(top_builder=builder, tk_frame=self.ttk)
         self.logger.info(f'Sample test is up and running')
-        self.ttk = Tk()
-        self.var_option = tkinter.IntVar(0)
 
     def set_logger(self):
-        formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s: %(message)s', '%Y-%m-%d %H:%M:%S')
-        stream_handler = logging.StreamHandler()
-        stream_handler.setLevel(logging.DEBUG)
-        stream_handler.setFormatter(formatter)
-        wiliot_dir = WiliotDir()
-        logger_path = abspath(join(wiliot_dir.get_wiliot_root_app_dir(), 'sample_test'))
-        if not isdir(logger_path):
-            os.mkdir(logger_path)
-        logger_path = abspath(join(logger_path, 'logs'))
-        if not isdir(logger_path):
-            os.mkdir(logger_path)
-        logger_name = 'sample_test_{}.log'.format(datetime.datetime.now().strftime('%Y%m%d_%H%M%S'))
-        self.logger_path = abspath(join(logger_path, logger_name))
-        file_handler = logging.FileHandler(self.logger_path, mode='a')
-        file_formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
-        file_handler.setFormatter(file_formatter)
-        self.logger.addHandler(file_handler)
-        self.logger.addHandler(stream_handler)
-        self.logger.setLevel(logging.INFO)
+        run_name = 'sample_' + datetime.datetime.now().strftime('%d%m%y_%H%M%S')
+        self.log_obj = WiliotTesterLog(run_name=run_name)
+        self.log_obj.set_logger(tester_name=TESTER_NAME)
+        self.logger = self.log_obj.logger
 
     def gui(self):
         self.logger.info(f'Sample test setting the GUI')
         self.set_gui()
         self.logger.info(f'Sample test GUI is running')
         self.ttk.mainloop()
 
@@ -269,1257 +202,748 @@
         self.builder.add_resource_path(img_path)
 
         self.ttk.title("Wiliot Sample Test")
         self.mainWindow = self.builder.get_object('mainwindow', self.ttk)
         self.ttk.protocol("WM_DELETE_WINDOW", self.close)
         self.builder.connect_callbacks(self)
 
-        self.builder.get_object('reelId').bind("<Key>", self.get_reel_id)
+        self.builder.get_object('reelId').bind("<Key>", self.get_reel_id_cb)
         list_box = self.builder.get_object('scanned')
         scrollbar = self.builder.get_object('scrollbar1')
         list_box.configure(yscrollcommand=scrollbar.set)
         scrollbar.configure(command=list_box.yview)
         self.builder.get_object('scrollbar1').set(self.builder.get_object('scanned').index(ACTIVE),
                                                   self.builder.get_object('scanned').index(END))
         self.logger.info(f'checking available serial connection')
-        self.comConnect.choose_com_ports()
+        self.com_connect.choose_com_ports()
         self.logger.info(f'setting up gui defaults')
         self.set_gui_defaults()
 
         self.builder.connect_callbacks(self)
 
         self.settings_combobox = self.builder.get_object('settings_combobox', self.ttk)
-        self.settings_combobox.configure(values=[v.value for v in SettingModeOptions])
-        self.settings_combobox.set(SettingModeOptions.SEND.value)
-        self.settings_combobox.bind('<<ComboboxSelected>>', self.on_dropdown_change)
-
-    def on_dropdown_change(self, event=None):
-
-        selected_label = self.settings_combobox.get()
-
-        self.post_data = False
-        self.calib = False
-        self.offline = False
+        self.settings_combobox.configure(values=['prod', 'test', 'dev'])
+        self.settings_combobox.set('prod')
+        self.settings_combobox.bind('<<ComboboxSelected>>', self.on_env_change_cb)
+
+    def init_test(self):
+        all_config = {'run': self.default_config,
+                      'test': self.configs_gui.configs_test}
+        test_cloud_config = {'is_online': not self.offline, 'owner_id': RESOLVE_OWNER_ID, 'env': RESOLVE_ENV}
+        self.stop_event.clear()
+        self.sample_run_obj = SampleRun(tags_in_test=list(self.tags_under_test.keys()),
+                                        selected_test=self.test_configs,
+                                        all_configs=all_config,
+                                        cloud_config=test_cloud_config,
+                                        gw_obj=self.com_connect.gateway,
+                                        stop_event=self.stop_event,
+                                        inlay=self.run_data['inlay'],
+                                        logger_name=self.logger.name)
+
+    def init_data_log(self):
+        test_name = self.builder.get_object('testName').get()
+        makedirs(abspath(join(OUTPUT_DIR, test_name)), exist_ok=True)
+        self.test_data_dir = abspath(join(OUTPUT_DIR, test_name, self.run_data['timestamp']))
+        mkdir(self.test_data_dir)
+        self.test_num = 0
+
+    def tag_test(self):
+        # init:
+        self.init_test()
+        self.com_connect.read_temperature_sensor()  # read temperature
+        # start timer
+        self.timer_thread = Thread(target=self.timer_count_down, args=())
+        self.timer_thread.start()
+        # start run:
+        self.com_connect.set_attenuation(self.run_data)
+        self.sample_run_obj.run()
+        # end of run
+        self.end_test()
+
+    def end_test(self):
+        self.stop_event.set()
+        self.com_connect.read_temperature_sensor()  # read temperature
 
-        if selected_label in [SettingModeOptions.SEND.value, SettingModeOptions.SEND_TEST.value]:  # Send to Cloud
-            self.post_data = True
-            self.logger.info('Send to cloud was changed to True')
-        elif selected_label == SettingModeOptions.CALIB.value:  # Test Calibration
-            self.calib = True
-            self.logger.info('Calibration mode was changed to True')
-        elif selected_label == SettingModeOptions.OFFLINE.value:  # Offline Mode
-            self.offline = True
-            self.logger.info('Offline mode was changed to True')
-        elif selected_label == SettingModeOptions.CALIB_OFFLINE.value:  # Offline Mode
-            self.offline = True
-            self.calib = True
-            self.logger.info('Calibration + Offline mode were changed to True')
-
-        # Update the environment
-        self.environment = 'prod' if selected_label != SettingModeOptions.SEND_TEST.value else 'test'
-        self.logger.info(f'Environment set to {self.environment}')
-
-    def choose_param(self, *args):
-        var = args[0].widget['style'].split('.')[0]
-        if self.builder.tkvariables.get(var) is not None:
-            value = self.builder.get_object(var).get()
-            if var not in self.defaultDict.keys():
-                self.defaultDict[var] = []
-            if value in self.defaultDict[var]:
-                self.defaultDict[var].pop(self.defaultDict[var].index(value))
-            self.defaultDict[var].insert(0, value)
-
-    def go(self):
-        if self.finishThread is not None and self.finishThread.is_alive():
-            self.finishThread.join()
-        self.goButtonState = goButtonState = self.builder.tkvariables.get('go').get()
-        self.builder.get_object('stop')['state'] = 'disabled'
-        self.builder.get_object('settings_combobox')['state'] = 'disabled'
-        self.update_params_state(state='disabled', group=GO)
-        self.builder.get_variable('forceGo').set('0')
-        recvDataMutex.acquire()
-        self.forceCloseRequested = False
-        recvDataMutex.release()
-        if goButtonState == CONNECT_HW:
-            self.connectThread = Thread(target=self.connect_all, args=([False]))
-            self.connectThread.start()
-        elif goButtonState == READ:
-            self.builder.get_object('settings_combobox')['state'] = 'disabled'
-            if self.stopButtonState == SEND:
-                self.remove_barcodes()
-                self.stopButtonState = FINISH
-                self.builder.tkvariables.get('stop').set(FINISH)
-            indexes = self.get_missing_ids_chambers()
-            if self.offline:
-                self.update_go_state()
-            else:
-                self.testBarcodesThread = Thread(target=self.read_scanners_barcodes, args=([indexes]))
-                self.testBarcodesThread.start()
-        elif goButtonState == GO:
-            self.numOfPackets = 0
-            self.offline_tag_index = 0
-            self.multiTag = TagCollection()
-            self.total_bad_advas = []
-            self.bad_advas = []
-            self.advas_dict = {}
-            self.builder.tkvariables.get('stop').set(STOP)
-            self.stopButtonState = STOP
-            # self.numOfTags = int(self.builder.tkvariables.get('numTags').get())
-            self.testId = testId = time.time()
-            self.testName = testName = self.builder.get_object('testName').get()
-            # self.operator = operator = self.builder.get_object('operator').get()
-            if not isdir(abspath(join(OUTPUT_DIR, testName))):
-                makedirs(abspath(join(OUTPUT_DIR, testName)))
-            self.testDir = testDir = datetime.datetime.fromtimestamp(testId).strftime('%d%m%y_%H%M%S')
-            mkdir(abspath(join(OUTPUT_DIR, testName, testDir)))
-            self.common_run_name = common_run_name = self.reel_id + '_' + testDir
-            self.test_log_file = abspath(join(OUTPUT_DIR, testName, testDir, f'{common_run_name}.log'))
-            changeFileHandler(self.logger, self.test_log_file, append_handler=True)
-            self.logger.info(f'Starts new test: {common_run_name}')
-            removeFileHandler(self.logger, self.logger_path)
-            self.update_params()
-            self.testStartTime = time.time()
-            self.comConnect.read_temperature_sensor()  # read temperature
-            if self.calib:
-                self.calibModeThread = Thread(target=self.calib_thread, args=())
-                self.calibModeThread.start()
-                self.calibModeThread.join()
-                self.calibModeThread = Thread(target=self.calib_mode, args=())
-                self.calibModeThread.start()
-            else:
-                self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
-                self.sendCommandThread.start()
-
-        elif goButtonState == CONTINUE:
-            self.builder.tkvariables.get('stop').set(STOP)
-            self.stopButtonState = STOP
-            self.total_bad_advas.append(x for x in self.bad_advas if x not in self.total_bad_advas)
-            self.bad_advas = []
-            self.advas_dict = {}
-            self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
-            self.sendCommandThread.start()
-
-    def calib_thread(self):
-        self.popup_calib()
+        if not self.calib:
+            self.builder.get_object('stop')['state'] = 'disabled'
+            self.iteration_finished()
+        elif self.calib:
+            self.post_process_iteration()
+            self.calib_mode_clean_barcodes()
 
     def read_scanners_barcodes(self, indexes):
-        self.comConnect.read_scanners_barcodes(indexes)
-        # self.update_params_state(state='normal', group=CONTINUE)
+        self.com_connect.read_scanners_barcodes(indexes)
 
     def connect_all(self, gui=True):
-        self.comConnect.connect_all(gui=gui)
-        self.builder.tkvariables.get('go').set(READ)
-        # self.update_params_state(state='normal', group=READ)
-        self.builder.get_object('read_qr')['state'] = 'normal'
-        self.builder.get_object('reelId')['state'] = 'normal'
-        self.builder.get_object('connect')['state'] = 'normal'
+        self.com_connect.connect_all(gui=gui)
+        if self.com_connect.hwConnected:
+            self.builder.tkvariables.get('go').set(READ)
+            self.builder.get_object('read_qr')['state'] = 'normal'
+            self.builder.get_object('reelId')['state'] = 'normal'
+            self.builder.get_object('connect')['state'] = 'normal'
+        else:
+            self.builder.tkvariables.get('go').set(CONNECT_HW)
+            self.builder.get_object('go')['state'] = 'normal'
+            self.builder.get_object('connect')['state'] = 'normal'
 
     def add_tag_to_test(self, cur_id, reel_id, scanner_index=0, add_to_test=False):
-        mutex.acquire()
-        if cur_id not in self.test_barcodes.keys() and cur_id not in self.barcodes_read.keys() and add_to_test:
-            self.barcodes_read[cur_id] = {'chamber': scanner_index,
-                                          'packets': [],
-                                          'reel': self.reel_id,
-                                          'ext ID': cur_id,
-                                          'ttfp': -1,
-                                          'tbp': -1,
-                                          'rssi': -1,
-                                          'adv_address': [],
-                                          'packetList': PacketList()}
-            # self.test_barcodes[cur_id] = scanner_index
+        same_reel_id = self.reel_id == reel_id or (self.reel_id[-TAG_COUNTER_LEN:] == reel_id
+                                                   if len(self.reel_id) > TAG_COUNTER_LEN else False)
+        if self.reel_id != '' and not same_reel_id and not self.calib:
+            do_test = popup_yes_no(f'Tag {cur_id} has a reel id different from test reel {self.reel_id}, '
+                                   f'are you sure you want to include it in the test?')
+            if not do_test:
+                return False
+
+        if add_to_test:
+            if cur_id in self.tags_under_test.keys():
+                self.com_connect.popup_message(f'Tag {cur_id} in chamber {scanner_index} already read in '
+                                               f'another chamber: {self.tags_under_test[cur_id]["chamber"]}',
+                                               title='Warning',
+                                               log='warning')
+                return False
+
+            if cur_id in self.all_tags_in_test.keys() and not self.calib:
+                retest = popup_yes_no(f'Tag {cur_id} was already tested, are you sure you want to re-test the tag?')
+                if not retest:
+                    return False
+            # add tag to test
+            self.tags_under_test[cur_id] = {'chamber': scanner_index}
             self.builder.get_object('scanned').insert(END, f'{cur_id}, {scanner_index}')
-            mutex.release()
-        else:
-            mutex.release()
-            self.comConnect.popup_message(f'Tag {cur_id} in chamber {scanner_index} already read.', title='Warning',
-                                          log='warning')
-            return False
-
-        if self.reel_id != '' and self.reel_id != reel_id and self.wiliotTags:
-            self.comConnect.popup_message('Tag reel different from test reel.', title='Warning', log='error')
 
         return True
 
     def update_go_state(self, force_go=False):
-        if (self.comConnect.get_num_of_barcode_scanners() == len(self.barcodes_read.keys()) or force_go) and \
-                len(self.test_barcodes.keys()) > 0:
-            self.builder.tkvariables.get('go').set(CONTINUE)
-            self.update_params_state(state='normal', group=CONTINUE)
-        elif self.comConnect.get_num_of_barcode_scanners() == len(self.barcodes_read.keys()) or force_go:
-            self.builder.tkvariables.get('go').set(GO)
-            self.update_params_state(state='normal', group=GO)
+        if self.com_connect.get_num_of_barcode_scanners() == len(self.tags_under_test.keys()) or force_go:
+            if len(self.all_tags_in_test.keys()) == 0:
+                self.builder.tkvariables.get('go').set(GO)
+                self.update_params_state(state='normal', group=GO)
+            else:
+                self.builder.tkvariables.get('go').set(CONTINUE)
+                self.update_params_state(state='normal', group=CONTINUE)
         else:
             self.builder.tkvariables.get('go').set(READ)
             self.update_params_state(state='normal', group=READ)
-        # self.top_builder.get_object('go')['state'] = 'normal'
 
     def get_missing_ids_chambers(self):
-        indexes = list(range(self.comConnect.get_num_of_barcode_scanners()))
-        if len(self.barcodes_read.keys()) > 0:
-            used_indexes = [barcode['chamber'] for barcode in self.barcodes_read.values()]
+        indexes = list(range(self.com_connect.get_num_of_barcode_scanners()))
+        if len(self.tags_under_test.keys()) > 0:
+            used_indexes = [barcode['chamber'] for barcode in self.tags_under_test.values()]
             indexes = [index for index in indexes if index not in used_indexes]
         return indexes
 
-    def force_go(self):
-        """
-        enable go in the GUI even if some of the chambers are empty
-        """
-        if self.builder.get_variable('forceGo').get() == '1':
-            self.builder.get_object('forceGo')['state'] = 'disabled'
-            self.builder.get_object('stop')['state'] = 'disabled'
-            self.builder.get_object('go')['state'] = 'disabled'
-            self.builder.get_object('add')['state'] = 'disabled'
-            self.builder.get_object('remove')['state'] = 'disabled'
-            self.builder.get_object('settings_combobox')['state'] = 'disabled'
-            if self.closeChambersThread is not None and self.closeChambersThread.is_alive():
-                self.closeChambersThread.join()
-            self.closeChambersThread = Thread(target=self.force_go_close_chambers, args=())
-            self.closeChambersThread.start()
-        else:
-            self.update_go_state()
-
     def force_go_close_chambers(self):
         indexes = self.get_missing_ids_chambers()
-        self.comConnect.close_chambers(indexes)
+        self.com_connect.close_chambers(indexes)
         self.update_go_state(force_go=True)
         self.builder.get_object('forceGo')['state'] = 'normal'
         self.builder.get_object('stop')['state'] = 'normal'
         self.builder.get_object('go')['state'] = 'normal'
 
+    def wait_between_calib_runs(self):
+        self.logger.info(f'wait between calib test for {TIME_BETWEEN_CALIB_RUNS} seconds')
+        t_start = time.time()
+        dt = time.time() - t_start
+        while dt < TIME_BETWEEN_CALIB_RUNS:
+            dt = time.time() - t_start
+            if self.force_close_requested:
+                break
+            sleep(0.200)
+        self.logger.info('continue to the next calib stage')
+
     def calib_mode(self):
-        self.testFinished = False
-        attenuations = numpy.arange(float(self.low), float(self.high) + float(self.step), float(self.step))
+        attenuation_list = numpy.arange(float(self.low), float(self.high) + float(self.step), float(self.step))
         n_rep = int(self.n_repetitions)
-        for i in attenuations:
-            if self.forceCloseRequested:
+        for i, atten in enumerate(attenuation_list):
+            if self.force_close_requested:
                 break
             for j in range(n_rep):
-                calibMutex.acquire()
-                self.total_num_of_unique = 0
-                self.offline_tag_index = 0
-                self.avg_unique = 1
-                self.cur_atten = i
-                self.test_num = j
-                self.advas_dict = {}
-                self.tagsFinished = {}
-                self.testGo = True
+                self.cur_atten = atten
+                self.test_num = (i * n_rep) + j
                 if self.antenna.lower() == 'ble':
-                    self.params['attenBle'] = self.cur_atten
-                    self.dataBaseDict['attenBle[db]'] = self.cur_atten
+                    self.run_data['bleAttenuation'] = self.cur_atten
                 elif self.antenna.lower() == 'lora':
-                    self.dataBaseDict['attenLoRa[db]'] = self.cur_atten
-                    self.params['attenLoRa'] = self.cur_atten
-                self.dataBaseDict['testNum'] = self.test_num
-                self.params['testNum'] = self.test_num
-
-                self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
-                self.sendCommandThread.start()
-                self.sendCommandThread.join()
-                sleep(5)
-                if self.forceCloseRequested:
-                    break
+                    self.run_data['loraAttenuation'] = self.cur_atten
 
-        calibMutex.acquire()
-        self.calib_mode_post_process()
-        self.comConnect.open_chambers()
-        # self.builder.tkvariables.get('numTags').set(0)
-        # self.builder.tkvariables.get('go').set(READ)
-        # self.test_barcodes = {}
-        # self.builder.get_object('connect')['state'] = 'normal'
-        # self.builder.get_object('read_qr')['state'] = 'normal'
-        calibMutex.release()
-        self.finish_test(post_data=False, reset_tester=True, post_process=False)
-        self.comConnect.popup_message('Sample Test - Calib Mode Finished running.', title='Info', log='info')
-
-    def calib_mode_post_process(self):
-        common_run_name = self.reel_id + '_' + self.testDir
-        unique_valid = []
-        full_test_dir = abspath(join(OUTPUT_DIR, self.testName, self.testDir))
-        is_first = True
-        for atten, runData in self.packets_dict.items():
-            for extId, data in runData.items():
-                if data['packetList'].size() > 0:
-                    packet_df = data['packetList'].get_df(add_sprinkler_info=True)
-                    packet_df.insert(loc=len(packet_df.columns), column='status', value='PASSED')
-                    packet_df.insert(loc=len(packet_df.columns), column='attenuation', value=float(atten.split('_')[0]))
-                    packet_df.insert(loc=len(packet_df.columns), column='test_num', value=int(atten.split('_')[1]))
-                    packet_df.insert(loc=len(packet_df.columns), column='external_id', value=extId)
-                    packet_df.insert(loc=len(packet_df.columns), column='chamber', value=data['chamber'])
-                    data['packetList'].export_packet_df(
-                        packet_df=packet_df,
-                        path=abspath(join(full_test_dir, f'{common_run_name}@packets_data_calib_mode.csv')),
-                        append=not is_first)
-                    is_first = False
-
-                unique_valid.append({
-                    'adv_address': data['adv_address'],
-                    'tbp': data['tbp'],
-                    'ttfp': data['ttfp'],
-                    'ext ID': data['ext ID'],
-                    'reel': data['reel'],
-                    'attenuation': float(atten.split('_')[0]),
-                    'test_num': int(atten.split('_')[1]),
-                    'chamber': data['chamber']
-                })
-
-        if len(unique_valid):
-            with open(abspath(join(full_test_dir, f'{common_run_name}@unique_data.csv')), 'w+',
-                      newline='') as new_tagsCsv:
-                writer = csv.DictWriter(new_tagsCsv, fieldnames=list(unique_valid[0].keys()))
-                writer.writeheader()
-                writer.writerows(unique_valid)
+                self.tag_test()
 
-        self.barcodes_read = {}
-        self.test_barcodes = {}
-        self.builder.get_object('scanned').delete(0, END)
+                self.wait_between_calib_runs()
+                if self.force_close_requested:
+                    break
+
+        self.com_connect.open_chambers()
+        self.finish()
+        self.com_connect.popup_message('Sample Test - Calib Mode Finished running.', title='Info', log='info')
 
     def calib_mode_clean_barcodes(self):
-        old_barcodes = self.barcodes_read.copy()
-        self.barcodes_read = {}
-        self.test_barcodes = {}
+        old_barcodes = self.tags_under_test.copy()
+        self.tags_under_test = {}
+        self.all_tags_in_test = {}
         self.builder.get_object('scanned').delete(0, END)
-        for tag in old_barcodes.values():
-            self.add_tag_to_test(tag['ext ID'], tag['reel'], tag['chamber'], add_to_test=True)
-
-    def stop(self):
-        """
-        stop the test and run post process
-        """
-        if self.stopButtonState == STOP:
-            self.forceCloseRequested = True
-
-        elif self.stopButtonState == FINISH:
-            # self.numOfTags = len(self.test_barcodes.keys())
-            # self.finishThread = Thread(target=self.iteration_finished, args=([True]))
-            # self.finishThread.start()
-            self.builder.get_object('scanned').delete(0, END)
-            self.builder.tkvariables.get('stop').set(SEND)
-            self.stopButtonState = SEND
-            for barcode in list(self.test_barcodes.keys()):
-                self.builder.get_object('scanned').insert(END, barcode)
-
-        elif self.stopButtonState == SEND:
-            if not self.is_test_completed() and 'controlLimits' in self.defaultDict.keys():
-                control_limits = self.defaultDict['controlLimits'][self.defaultDict['controlLimitsTestNum']]
-                self.update_values_for_control_limits(control_limits=control_limits)
-                is_pass, fail_str, complete_sub_test, fail_bin = self.check_control_limits()
-                self.reset_values_for_control_limits(control_limits=control_limits)
-                if not is_pass or not complete_sub_test:
-                    send_anyway = popup_yes_no(f'Test was FAILED!! are you sure you want to finish the test and '
-                                               f'send data to the cloud?')
-                    if not send_anyway:
-                        self.logger.info('User decide to keep testing')
-                        return
-            self.builder.get_object('go')['state'] = 'disabled'
-            self.builder.get_object('stop')['state'] = 'disabled'
-            self.builder.get_object('forceGo')['state'] = 'disabled'
-            self.builder.get_object('add')['state'] = 'disabled'
-            self.builder.get_object('remove')['state'] = 'disabled'
-            self.finishThread = Thread(target=self.finish, args=())
-            self.finishThread.start()
-
-    def add(self):
-        """
-        add manually tag to the list
-        """
-        new_tag = self.builder.tkvariables.get('addTag').get()
-        if (self.builder.tkvariables.get('stop').get() != SEND or len(new_tag.split(',')) == 2) and not \
-                new_tag.split(',')[0].strip() in self.barcodes_read.keys():
-            # self.builder.get_object('scanned').insert(END, new_tag)
-            # self.barcodes_read[new_tag.split(',')[0].strip()] = new_tag.split(',')[1].strip()
-            if self.builder.tkvariables.get('stop').get() == SEND:
-                self.builder.get_object('scanned').delete(0, END)
-                self.remove_barcodes()
-                self.stopButtonState = FINISH
-                self.builder.tkvariables.get('stop').set(FINISH)
-
-            if len(new_tag.split(',')) < 2:
-                self.comConnect.popup_message(f'Missing chamber index, add chamber index after a comma.', title='Error',
-                                              log='error')
-                return
-            cur_id = new_tag.split(',')[0].strip()
-            scan_index = int(new_tag.split(',')[1].strip())
-            if 0 < self.comConnect.get_num_of_barcode_scanners() < (scan_index + 1):
-                self.comConnect.popup_message(f'Chamber number {scan_index} not exists.', title='Error', log='error')
-                return
-
-            barcodes = self.builder.get_object('scanned').get(0, END)
-            if any([barcode for barcode in barcodes if int(barcode.split()[1].strip()) == scan_index]):
-                self.comConnect.popup_message(f'Chamber {scan_index} tag already scanned.', title='Error', log='error')
-                return
-            # logger.info(scan_index)
-
-            self.builder.tkvariables.get('addTag').set('')
-            popup_thread = Thread(target=self.comConnect.popup_message,
-                                  args=('Chambers are closing!!\nWatch your hands!!!',
-                                        'Warning', ("Helvetica", 18), 'warning'))
-            popup_thread.start()
-            popup_thread.join()
-            self.add_tag_to_test(cur_id, self.reel_id, scan_index, add_to_test=True)
-            chambers = self.comConnect.get_chambers()
-            if len(chambers) > scan_index and chambers[scan_index] is not None:
-                chambers[scan_index].close_chamber()
-            self.update_go_state()
-        else:
-            self.builder.get_object('scanned').insert(END, new_tag)
-            self.builder.tkvariables.get('addTag').set('')
-
-    def remove(self):
-        """
-        remove tag read from the list
-        """
-        tag = self.builder.get_object('scanned').get(ACTIVE)
-        tags = list(self.builder.get_object('scanned').get(0, END))
-        tag_index = tags.index(tag)
-        self.builder.get_object('scanned').delete(tag_index, tag_index)
-        tags.pop(tag_index)
-        self.builder.tkvariables.get('addTag').set(tag)
-        if self.stopButtonState != SEND:
-            self.barcodes_read.pop(tag.split(',')[0].strip())
-            self.comConnect.open_chambers(indexes=[int(tag.split(',')[1].strip())])
-            self.update_go_state()
+        for ex_id, tag in old_barcodes.items():
+            self.add_tag_to_test(ex_id, ex_id.split('T')[0], tag['chamber'], add_to_test=True)
 
     def update_params_state(self, state='disabled', group=GO):
-        if state == 'disabled' or group == READ:
+        if group == READ:
             self.builder.get_object('connect')['state'] = state
 
-            if len(self.test_barcodes.keys()) == 0:
+            if len(self.all_tags_in_test.keys()) == 0:
                 self.builder.get_object('read_qr')['state'] = state
                 self.builder.get_object('reelId')['state'] = state
 
             if self.reel_id != '':
                 self.builder.get_object('go')['state'] = state
                 self.builder.get_object('add')['state'] = state
                 self.builder.get_object('remove')['state'] = state
                 self.builder.get_object('addTag')['state'] = state
                 self.builder.get_object('stop')['state'] = state
                 self.builder.get_object('forceGo')['state'] = state
             self.builder.get_object('settings_combobox')['state'] = state
 
-        if state == 'disabled' or group == GO:
-            self.builder.get_object('configs')['state'] = state
-            self.builder.get_object('test_config')['state'] = state
-            self.builder.get_object('testName')['state'] = state
-            self.builder.get_object('operator')['state'] = state
-            self.builder.get_object('inlay')['state'] = state
-            self.builder.get_object('surface')['state'] = state
-            self.builder.get_object('settings_combobox')['state'] = state
+        if group in [GO, CONNECT_HW, CONTINUE]:
+            if group in [GO, CONTINUE]:
+                self.builder.get_object('go')['state'] = state
+                self.builder.get_object('connect')['state'] = state
+
+            if group == GO:
+                self.builder.get_object('configs')['state'] = state
+
+            if group in [GO, CONNECT_HW]:
+                self.builder.get_object('test_config')['state'] = state
+                self.builder.get_object('testName')['state'] = state
+                self.builder.get_object('operator')['state'] = state
+                self.builder.get_object('inlay')['state'] = state
+                self.builder.get_object('surface')['state'] = state
+                self.builder.get_object('settings_combobox')['state'] = state
+                if self.reel_id != '':
+                    self.builder.get_object('stop')['state'] = state
 
-        if state == 'disabled' or group == CONTINUE or group == GO:
-            self.builder.get_object('connect')['state'] = state
-            self.builder.get_object('go')['state'] = state
             self.builder.get_object('add')['state'] = state
             self.builder.get_object('remove')['state'] = state
             self.builder.get_object('addTag')['state'] = state
             self.builder.get_object('settings_combobox')['state'] = state
             self.builder.get_object('forceGo')['state'] = 'disabled'
 
-            if len(self.test_barcodes.keys()) == 0:
+            if len(self.all_tags_in_test.keys()) == 0:
                 self.builder.get_object('read_qr')['state'] = state
                 self.builder.get_object('reelId')['state'] = state
 
-        if state == 'disabled':
-            self.builder.get_object('read_qr')['state'] = state
-            self.builder.get_object('reelId')['state'] = state
-
     def set_gui_defaults(self):
-        configs = self.configsGui.get_configs()
+        configs = self.configs_gui.get_configs()
         self.builder.get_object('test_config')['values'] = \
             [key for key, item in configs.items() if isinstance(item, dict)]
 
-        if 'testName' in self.defaultDict.keys():
-            self.builder.get_object('testName')['values'] = self.defaultDict['testName']
-            self.builder.get_object('testName').set(self.defaultDict['testName'][0])
-
-        if 'operator' in self.defaultDict.keys():
-            self.builder.get_object('operator')['values'] = self.defaultDict['operator']
-            self.builder.get_object('operator').set(self.defaultDict['operator'][0])
+        if 'testName' in self.default_config.keys():
+            self.builder.get_object('testName')['values'] = self.default_config['testName']
+            self.builder.get_object('testName').set(self.default_config['testName'][0])
+
+        if 'operator' in self.default_config.keys():
+            self.builder.get_object('operator')['values'] = self.default_config['operator']
+            self.builder.get_object('operator').set(self.default_config['operator'][0])
 
         self.builder.get_object('inlay')['values'] = tuple(
             name for name in InlayTypes._member_names_ if name not in UnusableInlayTypes.__members__)
-        if 'inlay' in self.defaultDict.keys():
-            self.builder.get_object('inlay').set(self.defaultDict['inlay'][0])
+        if 'inlay' in self.default_config.keys():
+            self.builder.get_object('inlay').set(self.default_config['inlay'][0])
 
-        if 'surface' in self.defaultDict.keys():
-            self.builder.get_object('surface')['values'] = self.defaultDict['surface']
-            self.builder.get_object('surface').set(self.defaultDict['surface'][0])
-        if 'tester_hw' in self.defaultDict.keys():
+        if 'surface' in self.default_config.keys():
+            self.builder.get_object('surface')['values'] = self.default_config['surface']
+            self.builder.get_object('surface').set(self.default_config['surface'][0])
+        if 'tester_hw' in self.default_config.keys():
             self.builder.get_object('tester_hw_ver')['state'] = 'enabled'
             self.builder.get_object('tester_hw_ver').delete(0, END)
-            self.builder.get_object('tester_hw_ver').insert(0, self.defaultDict['tester_hw']['version'])
+            self.builder.get_object('tester_hw_ver').insert(0, self.default_config['tester_hw']['version'])
             self.builder.get_object('tester_hw_ver')['state'] = 'disabled'
             self.builder.get_object('tester_hw_desc')['state'] = 'enabled'
             self.builder.get_object('tester_hw_desc').delete(0, END)
-            self.builder.get_object('tester_hw_desc').insert(0, self.defaultDict['tester_hw']['description'])
+            self.builder.get_object('tester_hw_desc').insert(0, self.default_config['tester_hw']['description'])
             self.builder.get_object('tester_hw_desc')['state'] = 'disabled'
-        # if 'numOfTags' in self.defaultDict.keys():
-        # self.builder.tkvariables.get('numTags').set(self.defaultDict['numOfTags'])
+        # if 'numOfTags' in self.default_config.keys():
+        # self.builder.tkvariables.get('numTags').set(self.default_config['numOfTags'])
         # else:
         # self.builder.tkvariables.get('numTags').set(DEF_NUM_OF_TAGS)
         self.builder.tkvariables.get('numTags').set(0)
+        self.builder.get_object('go')['state'] = 'normal'
+        self.builder.tkvariables.get('go').set(CONNECT_HW)
+        self.builder.get_object('stop')['state'] = 'normal'
+        self.builder.tkvariables.get('stop').set(STOP)
+        self.builder.get_object('stop')['state'] = 'disabled'
+        self.builder.tkvariables.get('reelId').set('')
+        self.update_params_state(group=CONNECT_HW)
 
-        if 'config' in self.defaultDict.keys():
-            self.testConfig = self.defaultDict['config']
-        else:
-            self.testConfig = ''
-        self.builder.get_object('test_config').set(self.testConfig)
-        self.configsGui.set_default_config(self.testConfig)
-        self.configsGui.set_params(self.testConfig)
-
-    def open_configs(self):
-        """
-        open Configs GUI
-        """
-        if self.configsGui is not None and not self.configsGui.is_gui_opened():
-            self.configsTtk = Toplevel(self.ttk)
-            self.ttk.eval(f'tk::PlaceWindow {str(self.configsTtk)} center')
-            self.configsGui.gui(self.configsTtk)
-
-    def test_config(self, *args):
-        """
-        update the configs in Configs module according to the main GUI
-        """
-        self.configsGui.config_set(self.builder.get_object('test_config').get())
-
-    def open_com_ports(self):
-        """
-        open ComConnect GUI
-        """
-        if self.comConnect is not None and not self.comConnect.is_gui_opened():
-            self.comTtk = Toplevel(self.ttk)
-            self.ttk.eval(f'tk::PlaceWindow {str(self.comTtk)} center')
-            self.comConnect.gui(self.comTtk)
-
-    def read_qr(self):
-        barcode, reel = self.comConnect.read_barcode()
-        if barcode is None:
-            read_qr_thread = Thread(target=self.comConnect.popup_message, args=(
-                [f'Error reading external ID, try repositioning the tag.', 'Error', ("Helvetica", 10), 'error']))
-            read_qr_thread.start()
-            read_qr_thread.join()
-            if not self.calib:
-                return
-
-        if reel is not None:
-            reel_id = self.builder.tkvariables.get('reelId')
-            reel_id.set(reel)
-            self.reel_id = reel
-
-        if 'config' in self.defaultDict.keys():
-            self.testConfig = self.defaultDict['config']
+        if 'config' in self.default_config.keys():
+            self.test_configs = self.default_config['config']
         else:
-            self.testConfig = []
-
-        self.builder.get_object('reelId').unbind("<Key>")
-        self.update_params_state(state='normal', group=GO)
-        self.builder.get_object('forceGo')['state'] = 'normal'
-
-    def get_reel_id(self, *args):
-        reel = self.builder.tkvariables.get('reelId').get()
-        if reel.strip() != '' and (str(args[0].type) != 'KeyPress' or args[0].keysym == 'Return'):
-            self.reel_id = reel
-            self.update_params_state(state='normal', group=GO)
-            self.builder.get_object('reelId').unbind("<Key>")
-            self.builder.get_object('forceGo')['state'] = 'normal'
+            self.test_configs = ''
+        self.builder.get_object('test_config').set(self.test_configs)
+        self.configs_gui.set_default_config(self.test_configs)
+        self.configs_gui.set_params(self.test_configs)
 
     def update_params(self):
-        self.runDataDict = {}
-        self.dataBaseDict = {}
-        self.params = params = self.configsGui.get_params()
-        self.testConfig = self.defaultDict['config'] = self.builder.get_object('test_config').get()
-
-        self.dataBaseDict['timestamp'] = datetime.datetime.fromtimestamp(self.testId).strftime('%d/%m/%y %H:%M:%S')
-        self.dataBaseDict['tested'] = self.builder.get_object('numTags').get()
-        self.dataBaseDict['channel'] = params['channel']
-        self.dataBaseDict['externalId'] = self.comConnect.get_reel_external()
+        self.run_data = {}
+        params = self.configs_gui.get_params()
+        self.test_configs = self.default_config['config'] = self.builder.get_object('test_config').get()
+
+        self.run_data['timestamp'] = datetime.datetime.now().strftime('%d%m%y_%H%M%S')
+        self.common_run_name = self.reel_id + '_' + self.run_data['timestamp']
         if 'sleep' in params.keys():
             self.sleep = int(params['sleep'])
         else:
             self.sleep = 0
-        self.testTime = float(params['testTime'])
+        self.test_time = float(params['testTime'])
 
-        self.runDataDict['runStartTime'] = self.dataBaseDict['runStartTime'] = time.strftime('%d/%m/%y %H:%M:%S')
-        self.runDataDict['antennaType'] = self.dataBaseDict['antennaType'] = params['antennaType']
-        self.runDataDict['bleAttenuation'] = self.dataBaseDict['attenBle[db]'] = params['attenBle']
-        self.runDataDict['loraAttenuation'] = self.dataBaseDict['attenLoRa[db]'] = params['attenLoRa']
-        self.runDataDict['energizingPattern'] = self.dataBaseDict['energizing'] = params['pattern']
-        self.runDataDict['testTime'] = self.dataBaseDict['testTime[sec]'] = params['testTime']
-        self.runDataDict['inlay'] = self.dataBaseDict['inlay'] = self.builder.get_object('inlay').get()
-        self.runDataDict['surface'] = self.dataBaseDict['surface'] = self.builder.get_object('surface').get()
-        self.runDataDict['testerStationName'] = self.station_name
-        self.runDataDict['commonRunName'] = self.common_run_name
-        self.runDataDict['testerType'] = 'sample'
-        self.runDataDict['gwVersion'] = self.dataBaseDict['gwVersion'] = self.comConnect.get_gw_version()
-        self.runDataDict['operator'] = self.dataBaseDict['operator'] = self.builder.get_object('operator').get()
-        self.runDataDict['pyWiliotVersion'] = self.dataBaseDict['pyWiliotVersion'] = self.pywiliot_version
-        self.runDataDict['testTimeProfilePeriod'] = self.dataBaseDict['testTimeProfilePeriod'] = params['tTotal']
-        self.runDataDict['testTimeProfileOnTime'] = self.dataBaseDict['testTimeProfileOnTime'] = params['tOn']
-        self.runDataDict['numChambers'] = self.dataBaseDict[
-            'numChambers'] = self.comConnect.get_num_of_barcode_scanners()
-        self.runDataDict['timeProfile'] = '[{}, {}]'.format(params['tOn'], params['tTotal'])
-        self.runDataDict['txPower'] = 'max'
+        self.run_data['runStartTime'] = time.strftime('%d/%m/%y %H:%M:%S')
+        self.run_data['antennaType'] = params['antennaType']
+        self.run_data['bleAttenuation'] = params['attenBle']
+        self.run_data['loraAttenuation'] = params['attenLoRa']
+        self.run_data['energizingPattern'] = params['pattern']
+        self.run_data['testTime'] = params['testTime']
+        self.run_data['inlay'] = self.builder.get_object('inlay').get()
+        self.run_data['surface'] = self.builder.get_object('surface').get()
+        self.run_data['testerStationName'] = self.station_name
+        self.run_data['commonRunName'] = self.common_run_name
+        self.run_data['testerType'] = 'sample'
+        self.run_data['gwVersion'] = self.com_connect.get_gw_version()
+        self.run_data['operator'] = self.builder.get_object('operator').get()
+        self.run_data['pyWiliotVersion'] = str(self.pywiliot_version)
+        self.run_data['testTimeProfilePeriod'] = params['tTotal']
+        self.run_data['testTimeProfileOnTime'] = params['tOn']
+        self.run_data['numChambers'] = self.com_connect.get_num_of_barcode_scanners()
+        self.run_data['timeProfile'] = '[{}, {}]'.format(params['tOn'], params['tTotal'])
+        self.run_data['txPower'] = 'max'
 
-        if 'controlLimits' in self.defaultDict.keys():
+        if 'controlLimits' in self.default_config.keys():
             self.logger.info('reset control limits')
-            self.runDataDict['controlLimits'] = self.defaultDict['controlLimits'].copy()
-            self.defaultDict['controlLimitsTestNum'] = 0
-            self.params['tag_tbp_min'] = self.defaultDict['controlLimits'][0]['tag_tbp_min']
-            self.params['tag_tbp_max'] = self.defaultDict['controlLimits'][0]['tag_tbp_max']
+            self.run_data['controlLimits'] = self.default_config['controlLimits'].copy()
+            self.default_config['controlLimitsTestNum'] = 0
+            self.run_data['tag_tbp_min'] = self.default_config['controlLimits'][0]['tag_tbp_min']
+            self.run_data['tag_tbp_max'] = self.default_config['controlLimits'][0]['tag_tbp_max']
+        else:
+            self.run_data['tag_tbp_min'] = params['tag_tbp_min']
+            self.run_data['tag_tbp_max'] = params['tag_tbp_max']
 
-        if 'rssiThresholdSW' in self.defaultDict.keys():
+        if 'rssiThresholdSW' in self.default_config.keys():
             try:
-                self.params['rssi_threshold'] = int(self.defaultDict['rssiThresholdSW'])
+                self.run_data['rssi_threshold'] = int(self.default_config['rssiThresholdSW'])
             except Exception as e:
                 self.logger.warning(f'could not convert "rssiThresholdSW" field in ,default to number: '
-                                    f'{self.defaultDict["rssiThresholdSW"]} due to {e}. '
+                                    f'{self.default_config["rssiThresholdSW"]} due to {e}. '
                                     f'rssi threshold is set to default: {RSSI_THR_DEFAULT}')
         else:
-            self.params['rssi_threshold'] = self.defaultDict['rssiThresholdSW'] = RSSI_THR_DEFAULT
+            self.run_data['rssi_threshold'] = self.default_config['rssiThresholdSW'] = RSSI_THR_DEFAULT
 
-        self.runDataDict['hwVersion'] = self.defaultDict['tester_hw']['version'] \
-            if 'tester_hw' in self.defaultDict.keys() else ''
-        self.runDataDict['sub1gFrequency'] = params['EmulateSurfaceValue']
+        self.run_data['hwVersion'] = self.default_config['tester_hw']['version'] \
+            if 'tester_hw' in self.default_config.keys() else ''
+        self.run_data['sub1gFrequency'] = params['EmulateSurfaceValue']
 
         self.update_data()
 
-    def send_gw_commands(self):
-        """
-        send commands to the GW and start the packet listener
-        """
-        if self.sleep > 0:
-            for i in range(self.sleep):
-                sleep(1)
-                if i % 3 == 0:
-                    print('.', end='')
-            print()
-        self.recv_data_from_gw()
-        self.testFinished = False
-
-    def stop_state(self):
-        self.builder.get_object('stop')['state'] = 'normal'
-
-    def recv_data_from_gw(self):
-        self.tagsFinished = {}
-        self.testGo = True
-        self.startTime = self.comConnect.get_gw_time()
-        self.logger.info(f'Tags in the test: {",".join(list(self.barcodes_read.keys()))}')
-        gw_passed = self.comConnect.send_gw_app(self.params)
-        if not gw_passed:
-            self.comConnect.popup_message(f'Error sending GW commands.', 'Error', ("Helvetica", 10), 'error')
-            self.update_params_state(state='normal', group=CONTINUE)
-            return
-        self.gatewayDataThread = Thread(target=self.stop_state(), args=())
-        self.gatewayDataThread.start()
-        last_time = time.time()
-        self.targetTime = last_time + self.testTime
-        if self.timerThread is not None:
-            self.timerThread.join()
-        self.timerThread = Thread(target=self.timer_count_down, args=([self.targetTime]))
-        self.timerThread.start()
-        self.sync_thread = Thread(target=self.threads_sync, args=())
-        self.sync_thread.start()
-        packets_list = PacketList()
-        recvDataMutex.acquire()
-        while True:
-            sleep(0.001)
-            try:
-                if self.closeListener:
-                    self.logger.info("DataHandlerProcess Stop")
-                    break
-
-                if self.comConnect.is_gw_data_available():
-
-                    gw_data = self.comConnect.get_data()
-
-                    packets_list.__add__(gw_data)
-
-                    cur_time = time.time()
-                    if cur_time - last_time > 2 and len(packets_list) > 0:
-                        temp_thread = Thread(target=self.add_to_packet_dict, args=([packets_list]))
-                        # temp_thread.start()
-                        addToDictMutex.acquire()
-                        self.add_to_dict_threads.append(temp_thread)
-                        addToDictMutex.release()
-                        packets_list = PacketList()
-                        last_time = cur_time
-
-            except BaseException:
-                print_exc()
-                pass
-        self.comConnect.read_temperature_sensor()  # read temperature
-        self.comConnect.cancel_gw_commands()
-        timerMutex.acquire()
-        self.stopTimer = True
-        timerMutex.release()
-        # self.tagsCount += len(self.barcodes_read.keys())
-        recvDataMutex.release()
-        self.sync_thread.join()
-        self.closeListener = False
-        if not self.calib:
-            self.builder.get_object('stop')['state'] = 'disabled'
-            self.finishIterThread = Thread(target=self.iteration_finished, args=())
-            self.finishIterThread.start()
-        elif self.calib:
-            self.handle_unknown_packets()
-            self.unknown_packets = PacketList()
-            self.post_process_iteration()
-
-            self.packets_dict[f'{self.cur_atten}_{self.test_num}'] = {}
-            self.packets_dict[f'{self.cur_atten}_{self.test_num}'].update(self.barcodes_read)
-            self.calib_mode_clean_barcodes()
-            calibMutex.release()
-
-    def threads_sync(self):
-        while not self.closeRequested and not self.forceCloseRequested and time.time() < self.targetTime:
-            if len(self.add_to_dict_threads) > 0:
-                addToDictMutex.acquire()
-                thread = self.add_to_dict_threads.pop()
-                addToDictMutex.release()
-                thread.start()
-                thread.join()
-            sleep(0.1)
-        self.closeRequested = False
-        self.closeListener = True
-        self.add_to_dict_threads = []
-
-    def timer_count_down(self, target_time):
+    def timer_count_down(self):
         """
         count down the test time
         """
-        while True:
-            if self.stopTimer:
-                timerMutex.acquire()
-                self.stopTimer = False
-                timerMutex.release()
+        target_time = time.time() + self.test_time
+        dt = int(target_time - time.time())
+        while dt > 0:
+            if self.stop_event.is_set():
                 break
-            timer = int(target_time - time.time())
-            update_timer_thread = Thread(target=self.update_timer, args=([timer]))
-            update_timer_thread.start()
-            update_timer_thread.join()
+            dt = int(target_time - time.time())
+            self.builder.tkvariables.get('testTime').set(str(dt))
             sleep(1)
-        self.builder.tkvariables.get('testTime').set(str(int(self.testTime)))
 
-    def update_timer(self, timer):
-        """
-        update timer value in the GUI
-        :type timer: int
-        :param timer: remaining time to the test
-        """
-        self.builder.tkvariables.get('testTime').set(str(timer))
+        self.stop_event.set()
+        self.builder.tkvariables.get('testTime').set(str(int(self.test_time)))
 
-    def add_to_packet_dict(self, packets, post_run=False):
-        self.process_packets(packets, post_run=post_run)
+    def end_test_popup_calculation(self, df):
+        """
 
-    def check_rssi_threshold(self, packet_rssi):
-        packet_rssi_list = packet_rssi.tolist()
-        if not isinstance(packet_rssi_list, list):
-            packet_rssi_list = [packet_rssi_list]
-        return any([rssi <= self.params['rssi_threshold'] for rssi in packet_rssi_list])
+        @param df:
+        @type df: pd.Dataframe
+        @return:
+        @rtype:
+        """
+        all_answered = len(df[df['resolve_status'] == TagStatus.NO_RESPONSE]) == 0
+        several_adva = []
+        if 'adva_dup' in df.columns:
+            several_adva = df.loc[df['adva_dup'], 'external_id'].unique()
+        bad_adva = df['external_id'].loc[
+            df['resolve_status'].isin([TagStatus.OUT_VALID, TagStatus.OUT_INVALID])].unique()
 
-    def process_packets(self, packets, post_run=False):
-        for packet in packets:
-            ext_id = ''
-            adv_address = packet.packet_data['adv_address']
-            self.numOfPackets += 1
+        warning_msg = '' if all_answered or len(bad_adva) == 0 else 'Serialization warning!\n'
+        warning_msg += f'ADVA warning in tags: {several_adva}\n' if len(several_adva) else ''
+        bg_color = 'yellow' if warning_msg else None
 
-            if not self.check_rssi_threshold(packet.gw_data['rssi']):
-                self.logger.info(f'packet: {packet.get_packet_string()} was ignore due to high rssi')
-                continue
+        avg_tbp = self.get_clean_tbp(df['tbp_min'].unique()).mean()
+        avg_ttfp = pd.Series(df['ttfp'].unique()).mean()
 
-            if adv_address in [x['adv_address'] for x in self.bad_advas]:
-                continue
+        avg_tbp = avg_tbp if pd.isnull(avg_tbp) else avg_tbp.item()
+        avg_ttfp = avg_ttfp if pd.isnull(avg_ttfp) else avg_ttfp.item()
 
-            elif adv_address in self.advas_dict.keys() and self.advas_dict[adv_address] is not None:
-                ext_id = self.advas_dict[adv_address]
+        return warning_msg, bg_color, avg_tbp, avg_ttfp
 
-            else:
-                print(packet.get_packet_string())
-                full_data, success, is_valid = self.get_packet_ext_id(packet)
+    def end_test_popup(self):
+        warning_msg, bg_color, avg_tbp, avg_ttfp = self.end_test_popup_calculation(self.results_df)
 
-                if not success:
-                    if not post_run:
-                        self.unknown_packets.append(packet)
-                        if adv_address not in self.advas_dict.keys():
-                            self.logger.error(
-                                f'Could not get external ID for adv_address {adv_address} '
-                                f'from the cloud - saving data for post process')
-                        self.advas_dict[adv_address] = None
-                    else:
-                        self.logger.error(
-                            f'Could not get external ID for adv_address {adv_address} '
-                            f'from the cloud - dumping packet')
-                    continue
-
-                ext_id = full_data['barcode'] if full_data['barcode'] in self.barcodes_read.keys() else full_data[
-                    'cur_id']
-                if ext_id is not None and ext_id not in self.barcodes_read.keys():
-                    self.logger.info(
-                        f'Tag with adv_address {adv_address} and external ID {full_data["cur_id"]} '
-                        f'detected but not belong to the test.')
-                    self.bad_advas.append({'adv_address': adv_address, 'external_id': full_data["cur_id"],
-                                           'is_valid': is_valid})
-                    continue
-
-                self.advas_dict[adv_address] = ext_id
-
-                if adv_address not in self.barcodes_read[ext_id]['adv_address']:
-                    self.logger.info(
-                        f'New Tag detected with adv_address {adv_address} and external ID {full_data["cur_id"]}.')
-                    self.barcodes_read[ext_id]['adv_address'].append(adv_address)
-
-            self.barcodes_read[ext_id]['packets'].append(packet.get_packet_string())
-            self.barcodes_read[ext_id]['packetList'].append(packet.copy())
-
-            if self.barcodes_read[ext_id]['packetList'].get_statistics()['tbp_min'] > 0 and not post_run:
-                self.tagsFinished[ext_id] = True
-
-            if len(self.tagsFinished.keys()) >= len(self.barcodes_read.keys()) and not post_run:
-                self.closeRequested = True
-
-    def iteration_finished(self, force_finish=False):
-        self.testGo = False
-        self.handle_unknown_packets()
-        avg_tbp, avg_ttfp = self.post_process_iteration()
-        self.test_barcodes = dict(list(self.test_barcodes.items()) + list(self.barcodes_read.items()))
-        self.comConnect.open_chambers()
-
-        all_answered = all([False for ext_id in self.barcodes_read.values() if len(ext_id['packets']) == 0])
-        dup_adva = [extId for extId, tag in self.barcodes_read.items() if len(tag['adv_address']) > 1]
-        adva_warning = len(dup_adva) > 0
-        serial_warning = '' if all_answered or len(self.bad_advas) == 0 else 'Serialization warning!\n'
-        serial_warning = serial_warning if not adva_warning else serial_warning + f'ADVA warning in tags: {dup_adva}\n'
-        bg_color = None if all_answered or len(self.bad_advas) == 0 else 'yellow'
-        bg_color = bg_color if not adva_warning else 'yellow'
-        stat = ''
-        if avg_ttfp != 0:
+        if pd.notnull(avg_ttfp):
             stat = f'Average TTFP: {avg_ttfp:.3f} [sec]\n' + \
                    f'Average TBP: {avg_tbp:.3f} [msec]'
         else:
             stat = 'No packets received'
 
-        self.finish_test()
-
-        # read_tags = ''
-        # if self.tagsCount < self.numOfTags and not force_finish:
         read_tags = '\nReplace tags and click on "Read"'
 
-        finishThread = Thread(target=self.comConnect.popup_message, args=(f'{serial_warning}'
-                                                                          f'{stat}'
-                                                                          f'{read_tags}',
-                                                                          'info',
-                                                                          ("Helvetica", 10),
-                                                                          'info',
-                                                                          bg_color))
-        finishThread.start()
-        finishThread.join()
+        self.com_connect.popup_message(msg=f'{warning_msg}{stat}{read_tags}',
+                                       title='end test info',
+                                       font=("Helvetica", 10),
+                                       bg=bg_color)
+
+    def iteration_finished(self):
+        self.post_process_iteration()
+
+        self.all_tags_in_test = {**self.all_tags_in_test, **self.tags_under_test}
+        self.com_connect.open_chambers()
+
+        self.end_test_popup()
+        self.finish_test()
 
         self.update_params_state(state='normal', group=READ)
 
-        self.builder.tkvariables.get('numTags').set(len(self.test_barcodes.keys()))
+        self.builder.tkvariables.get('numTags').set(len(self.all_tags_in_test.keys()))
         self.builder.tkvariables.get('addTag').set('')
         self.builder.get_object('connect')['state'] = 'normal'
         self.builder.get_object('scanned').delete(0, END)
         self.builder.tkvariables.get('go').set(READ)
         self.builder.tkvariables.get('stop').set(FINISH)
-        self.stopButtonState = FINISH
+        self.stop_button_state = FINISH
 
-        self.barcodes_read = {}
-        self.unknown_packets = PacketList()
+        self.reset_test_data()
+
+    def reset_test_data(self):
+        self.tags_under_test = {}
+        self.results_df = pd.DataFrame()
 
     def remove_barcodes(self):
         final_barcodes = self.builder.get_object('scanned').get(0, END)
         self.builder.get_object('scanned').delete(0, END)
-        test_barcodes = list(self.test_barcodes.keys()).copy()
+        test_barcodes = list(self.all_tags_in_test.keys()).copy()
         for barcode in test_barcodes:
             if barcode not in final_barcodes:
-                self.test_barcodes.pop(barcode)
+                self.all_tags_in_test.pop(barcode)
 
     def finish(self):
         self.remove_barcodes()
-        self.finish_test(True, True)
-        # self.finishTestThread = Thread(target=self.finish_test, args=([True, True]))
-        # self.finishTestThread.start()
-
-    def handle_unknown_packets(self):
-        if self.unknown_packets.size() > 0:
-            self.logger.info(f'Start handling unknown packets.')
-            self.process_packets(self.unknown_packets, post_run=True)
+        self.finish_test(post_data=not self.calib, reset_tester=True, post_process=True)
 
-    def post_process_iteration(self):
-        tbp_count = 0
-        ttfp_count = 0
-        ttfp_avg = 0
-        tbp_avg = 0
-
-        for extId, tag in self.barcodes_read.items():
-            stat = tag['packetList'].get_statistics()
-            if 'ttfp' in stat.keys():
-                tbp = stat['tbp_min']
-                tbp = tbp if type(tbp).__name__ != 'str' else -1
-                if tbp != -1:
-                    tbp_avg = ((tbp_avg * tbp_count) + tbp) / (tbp_count + 1)
-                    tbp_count += 1
-
-                ttfp = stat['ttfp']
-                ttfp_avg = ((ttfp_avg * ttfp_count) + ttfp) / (ttfp_count + 1)
-                ttfp_count += 1
-                self.barcodes_read[extId]['tbp'] = int(tbp)
-                self.barcodes_read[extId]['ttfp'] = ttfp
+    def is_valid_tbp(self, tbp):
+        if self.run_data['tag_tbp_min'] != '' and self.run_data['tag_tbp_max'] != '':
+            is_pass = int(self.run_data['tag_tbp_min']) < tbp < int(self.run_data['tag_tbp_max'])
+        elif pd.isnull(tbp):
+            is_pass = False
+        else:
+            is_pass = tbp != -1
+        return is_pass
 
-                self.barcodes_read[extId]['rssi'] = float(stat["rssi_mean"])
+    def get_temperature_avg(self, chamber):
+        if pd.isnull(chamber):
+            return float('nan')
+        if chamber < len(self.com_connect.temperature_sensor_readings):
+            all_reading_temp = self.com_connect.temperature_sensor_readings[int(chamber)]
+        else:
+            all_reading_temp = []
+        return numpy.nanmean(all_reading_temp) if len(all_reading_temp) else float('nan')
 
-        return tbp_avg, ttfp_avg
+    def post_process_iteration(self):
+        self.results_df = self.sample_run_obj.get_test_results()
+        # check if there are no response tags:
+        all_received_tags = [] if self.results_df.empty else self.results_df['external_id'].unique()
+        all_not_responded_tags = [{'external_id': ex_id,
+                                   'resolve_status': TagStatus.NO_RESPONSE,
+                                   'adv_address': '', 'raw_packet': '', 'gw_packet': '',
+                                   'time_from_start': float('nan'),
+                                   'tbp_min': float('nan'), 'rssi_mean': float('nan'),
+                                   'ttfp': float('nan'), 'tbp':float('nan'), 'rssi': float('nan')}
+                                  for ex_id in self.tags_under_test.keys() if
+                                  ex_id not in all_received_tags]
+        self.results_df = pd.concat([self.results_df, pd.DataFrame(all_not_responded_tags)], ignore_index=True)
+        tags_results = self.results_df.groupby('external_id').agg(
+            adva_dup=('adv_address', lambda x: len(x.unique()) > 1),
+            tag_status=('resolve_status', 'first'),
+            tag_ttfp=('ttfp', 'first'),
+            tag_tbp=('tbp_min', 'first'),
+            tag_rssi=('rssi_mean', 'first')
+        )
+        # check pass/fail:
+        tags_results['valid_tbp'] = tags_results['tag_tbp'].apply(lambda x: self.is_valid_tbp(x))
+        tags_results['is_pass'] = (~tags_results['adva_dup']) & (tags_results['valid_tbp']) & (
+                tags_results['tag_status'] == TagStatus.INSIDE_TEST)
+        tags_results.reset_index(inplace=True)
+
+        # calc fail bin
+        tag_status_count = tags_results['tag_status'].value_counts()
+        test_status = {}
+        for name in dir(TagStatus):
+            if not name.startswith('_'):
+                stat = getattr(TagStatus, name)
+                test_status[stat] = tag_status_count.loc[stat] if stat in tag_status_count.index else 0
+
+        fail_bins = tags_results.apply(lambda x: self.calc_tag_state(x, test_status), axis=1)
+        tags_results['fail_bin'] = [f_bin.name for f_bin in fail_bins]
+        tags_results['state(tbp_exists:0,no_tbp:-1,no_ttfp:-2,dup_adv_address:-3)'] = [
+            f_bin.value for f_bin in fail_bins]
+
+        # add chamber and reel data:
+        chambers = [{'external_id': ex_id, 'chamber': self.tags_under_test[ex_id]['chamber']}
+                    for ex_id in self.tags_under_test.keys()]
+        tags_results = pd.merge(tags_results, pd.DataFrame(chambers), on='external_id', how='outer')
+        tags_results['reel'] = tags_results['external_id'].apply(lambda x: x[:-5])
+
+        # get temperature:
+        tags_results['temperature_from_sensor'] = tags_results['chamber'].apply(lambda x: self.get_temperature_avg(x))
+        # add test params
+        tags_results['test_num'] = self.test_num
+        tags_results['attenuation_ble'] = self.run_data['bleAttenuation']
+        tags_results['attenuation_lora'] = self.run_data['loraAttenuation']
+
+        self.update_tags_data(tags_results)
+        # add results
+        self.results_df = pd.merge(self.results_df, tags_results, on='external_id')
+
+        # update all test results
+        self.all_results = pd.concat([self.all_results, self.results_df], ignore_index=True)
 
     def update_values_for_control_limits(self, control_limits):
-        self.params['test_tbp_min'] = control_limits['test_tbp_min']
-        self.params['test_tbp_max'] = control_limits['test_tbp_max']
-        self.params['test_responding_min'] = control_limits['test_responding_min']
-        self.params['test_valid_tbp'] = control_limits['test_valid_tbp']
+        self.run_data['test_tbp_min'] = control_limits['test_tbp_min']
+        self.run_data['test_tbp_max'] = control_limits['test_tbp_max']
+        self.run_data['test_responding_min'] = control_limits['test_responding_min']
+        self.run_data['test_valid_tbp'] = control_limits['test_valid_tbp']
 
     def reset_values_for_control_limits(self, control_limits):
-        self.params['tag_tbp_min'] = control_limits['tag_tbp_min']
-        self.params['tag_tbp_max'] = control_limits['tag_tbp_max']
-        self.params['test_tbp_min'] = ''
-        self.params['test_tbp_max'] = ''
-        self.params['test_responding_min'] = ''
-        self.params['test_valid_tbp'] = ''
+        self.run_data['tag_tbp_min'] = int(control_limits['tag_tbp_min'])
+        self.run_data['tag_tbp_max'] = int(control_limits['tag_tbp_max'])
+        self.run_data['test_tbp_min'] = ''
+        self.run_data['test_tbp_max'] = ''
+        self.run_data['test_responding_min'] = ''
+        self.run_data['test_valid_tbp'] = ''
 
     def update_control_limits(self, reset_test=False):
         next_test = False
-        if 'controlLimits' in self.defaultDict.keys():
+        if 'controlLimits' in self.default_config.keys():
             self.logger.info(f'Check control limits for pre-defined phased-test:'
-                             f'\nnumber of tested:{self.dataBaseDict["tested"]}')
-            if reset_test and self.defaultDict['controlLimitsTestNum'] < len(self.defaultDict['controlLimits']) - 1:
-                self.defaultDict['controlLimitsTestNum'] += 1
-                self.logger.info(f'move to the next test: {self.defaultDict["controlLimitsTestNum"]}')
+                             f'\nnumber of tested:{self.run_data["tested"]}')
+            if reset_test and \
+                    self.default_config['controlLimitsTestNum'] < len(self.default_config['controlLimits']) - 1:
+                self.default_config['controlLimitsTestNum'] += 1
+                self.logger.info(f'move to the next test: {self.default_config["controlLimitsTestNum"]}')
 
-            control_limits = self.defaultDict['controlLimits'][self.defaultDict['controlLimitsTestNum']]
+            control_limits = self.default_config['controlLimits'][self.default_config['controlLimitsTestNum']]
 
             if reset_test:
                 self.reset_values_for_control_limits(control_limits=control_limits)
 
-            elif self.dataBaseDict['tested'] >= int(control_limits['n_tags']):
+            elif self.run_data['tested'] >= int(control_limits['n_tags']):
                 self.update_values_for_control_limits(control_limits=control_limits)
                 next_test = True
         return next_test
 
     def is_test_completed(self):
         completed = True
-        if 'controlLimits' in self.defaultDict.keys():
-            control_limits = self.defaultDict['controlLimits'][-1]
-            if self.dataBaseDict['tested'] < int(control_limits['n_tags']):
+        if 'controlLimits' in self.default_config.keys():
+            control_limits = self.default_config['controlLimits'][-1]
+            if self.run_data['tested'] < int(control_limits['n_tags']):
                 completed = False
         return completed
 
     def check_control_limits(self):
         complete_sub_test = self.update_control_limits(reset_test=False)
         is_pass = True
         fail_str = ''
         fail_bin = FailureCodeSampleTest.PASS
 
-        if self.params['test_responding_min'] != '':
-            if float(self.dataBaseDict['responding[%]'].replace('%', '')) < float(self.params['test_responding_min']):
+        if self.run_data.get('test_responding_min') and self.run_data.get('test_responding_min') != '':
+            if float(self.run_data.get('responding[%]').replace('%', '')) < float(self.run_data.get('test_responding_min')):
                 is_pass = False
                 fail_str += 'Failed % responding test. '
                 if fail_bin == FailureCodeSampleTest.PASS:
                     fail_bin = FailureCodeSampleTest.NO_RESPONSE
-        if self.params['test_valid_tbp'] != '':
-            if float(self.dataBaseDict['validTbp[%]'].replace('%', '')) < float(self.params['test_valid_tbp']):
+        if self.run_data.get('test_valid_tbp') and self.run_data.get('test_valid_tbp') != '':
+
+            if float(self.run_data.get('validTbp[%]').replace('%', '')) < float(
+                    self.run_data.get('test_valid_tbp', 'nan')):
                 is_pass = False
                 fail_str += 'Failed % from the responded tags with valid tbp avg test. '
                 if fail_bin == FailureCodeSampleTest.PASS:
                     fail_bin = FailureCodeSampleTest.NO_TBP
-        if self.params['test_tbp_min'] != '' and self.params['test_tbp_max'] != '':
-            if not int(self.params['test_tbp_min']) < float(
-                    self.runDataDict['tbpAvg']) < int(self.params['test_tbp_max']):
+        if ((self.run_data.get('test_tbp_min') and self.run_data.get('test_tbp_min') != '')
+                and (self.run_data.get('test_tbp_max') and self.run_data.get('test_tbp_max') != '')):
+
+            if not int(self.run_data.get('test_tbp_min')) < float(
+                    self.run_data.get('tbpAvg', 'nan')) < int(self.run_data.get('test_tbp_max')):
                 is_pass = False
                 fail_str += 'Failed tbp avg test. '
                 if fail_bin == FailureCodeSampleTest.PASS:
                     fail_bin = FailureCodeSampleTest.HIGH_TBP_AVG
 
         return is_pass, fail_str, complete_sub_test, fail_bin
 
     def finish_test(self, post_data=False, reset_tester=False, post_process=True):
         if post_process:
-            pass_barcodes = self.post_process()
+            self.post_process()
             pass_fail, fail_str, complete_sub_test, fail_bin = self.check_control_limits()
             if complete_sub_test and not pass_fail:
                 self.update_control_limits(reset_test=True)
 
-            dup_adva = [extId for extId, tag in self.test_barcodes.items() if len(tag['adv_address']) > 1]
+            warning_msg, bg_color, avg_tbp, avg_ttfp = self.end_test_popup_calculation(self.all_results)
 
-            all_answered = all([False for ext_id in self.test_barcodes.values() if len(ext_id['packets']) == 0])
-            serial_warning = (not all_answered) and len(self.total_bad_advas) != 0
-            adva_warning = len(dup_adva) > 0
-            serial_warning = '' if not serial_warning else 'Serialization warning!\n'
-            serial_warning = serial_warning \
-                if not adva_warning else serial_warning + f'ADVA warning in tags: {dup_adva}\n'
-            bg_color = 'green'
-            if 'controlLimits' not in self.defaultDict.keys():
-                bg_color = 'green' if not (serial_warning or adva_warning) else 'yellow'
+            if 'controlLimits' not in self.default_config.keys():
+                bg_color = 'green' if bg_color is None else bg_color
             bg_color = bg_color if pass_fail else 'red'
             pass_fail_str = 'Passed' if pass_fail else 'Failed'
 
-            if 'controlLimits' in self.defaultDict.keys():
+            if 'controlLimits' in self.default_config.keys():
                 if reset_tester and not complete_sub_test:
                     # user click on finish but test was not completed:
                     if fail_bin == FailureCodeSampleTest.PASS:
                         fail_bin = FailureCodeSampleTest.NOT_COMPLETED
                         pass_fail = False
                         pass_fail_str = 'Failed'
                         bg_color = 'red'
                 if complete_sub_test and not reset_tester:
                     new_test_pass_str = 'SUCCESSFULLY COMPLETED THE TEST! please move to the next reel'
                     last_stage = self.is_test_completed()
                     new_test_fail_str = 'FAILED CURRENT TEST STAGE,' + \
                                         ' failed the reel' if last_stage else ' please continue to test the reel'
                     if not last_stage and not pass_fail:
                         bg_color = 'yellow'
-                    self.comConnect.popup_message(f'Test {self.common_run_name} has {pass_fail_str}\n' +
-                                                  f'{fail_str}\n' +
-                                                  f'{new_test_pass_str if pass_fail else new_test_fail_str}'
-                                                  f'\n' +
-                                                  f'{serial_warning}'
-                                                  f'Fail bin: {fail_bin.value}:{fail_bin.name}', title='Finished test',
-                                                  bg=bg_color,
-                                                  log='info')
+
+                    if not self.calib:
+                        self.com_connect.popup_message(f'Test {self.common_run_name} has {pass_fail_str}\n' +
+                                                       f'{fail_str}\n' +
+                                                       f'{new_test_pass_str if pass_fail else new_test_fail_str}'
+                                                       f'\n' +
+                                                       f'{warning_msg}'
+                                                       f'Fail bin: {fail_bin.value}:{fail_bin.name}',
+                                                       title='Finished test',
+                                                       bg=bg_color,
+                                                       log='info')
             self.is_test_pass = pass_fail
 
             if reset_tester:
-                self.comConnect.popup_message(f'Test {self.common_run_name} has {pass_fail_str}\n' +
-                                              f'{fail_str}\n' +
-                                              f'{serial_warning}' +
-                                              f'Fail bin: {fail_bin.value}:{fail_bin.name}\n' +
-                                              f'Average TTFP: {self.dataBaseDict["ttfpAvg"]} [sec]\n' +
-                                              f'Average TBP: {self.dataBaseDict["tbpAvg"]} [msec]\n' +
-                                              f'STD TBP: {self.dataBaseDict["tbpStd"]} [msec]\n' +
-                                              f'Yield: {self.dataBaseDict["passed[%]"]}', title='Finished test',
-                                              bg=bg_color,
-                                              log='info')
+                if not self.calib:
+                    self.com_connect.popup_message(f'Test {self.common_run_name} has {pass_fail_str}\n' +
+                                                   f'{fail_str}\n' +
+                                                   f'{warning_msg}' +
+                                                   f'Fail bin: {fail_bin.value}:{fail_bin.name}\n' +
+                                                   f'Average TTFP: {self.run_data["ttfpAvg"]} [sec]\n' +
+                                                   f'Average TBP: {self.run_data["tbpAvg"]} [msec]\n' +
+                                                   f'STD TBP: {self.run_data["tbpStd"]} [msec]\n' +
+                                                   f'Yield: {self.run_data["passed[%]"]}', title='Finished test',
+                                                   bg=bg_color,
+                                                   log='info')
                 self.update_control_limits(reset_test=True)
 
             # log data:
-            self.runDataDict['testStatus'] = pass_fail
-            self.runDataDict['failBin'] = str(fail_bin.value) + str(self.defaultDict['controlLimitsTestNum']) \
-                if 'controlLimitsTestNum' in self.defaultDict.keys() else ''
-            self.runDataDict['failBinStr'] = fail_bin.name
+            self.run_data['testStatus'] = pass_fail
+            self.run_data['failBin'] = str(fail_bin.value) + str(self.default_config['controlLimitsTestNum']) \
+                if 'controlLimitsTestNum' in self.default_config.keys() else ''
+            self.run_data['failBinStr'] = fail_bin.name
 
             self.files_and_cloud(post_data)
 
         if reset_tester:
-            # self.tagsCount = 0
-            self.builder.get_object('reelId').bind("<Key>", self.get_reel_id)
-            self.builder.tkvariables.get('numTags').set(0)
+            self.reset_app_data()
             self.builder.tkvariables.get('go').set(READ)
-            self.testFinished = True
-            self.packets_dict = {}
-            self.test_barcodes = {}
-            self.barcodes_read = {}
-            self.reel_id = ''
-            self.gtin = ''
-            self.builder.tkvariables.get('reelId').set('')
-
-            changeFileHandler(self.logger, self.logger_path, file_mode='a+', append_handler=True)
-            self.logger.info(f'Test {self.common_run_name} ended.')
-            removeFileHandler(self.logger, self.test_log_file)
-            self.update_params_state(state='normal', group=READ)
-            self.builder.tkvariables.get('stop').set(STOP)
             self.builder.get_object('stop')['state'] = 'disabled'
+            self.update_params_state(group=READ, state='normal')
 
-        if self.offline:
-            self.offline_tag_index = 0
+    def reset_app_data(self):
+        self.all_results = pd.DataFrame()
+        self.builder.get_object('reelId').bind("<Key>", self.get_reel_id_cb)
+        self.set_gui_defaults()
 
-    def update_run_data(self, run_data_path):
-        if exists(run_data_path):
-            remove(run_data_path)
-
-        run_csv = CsvLog(HeaderType.RUN, run_data_path, tester_type=TesterName.SAMPLE)
-        run_csv.open_csv()
-        run_csv.append_dict_as_row([self.runDataDict])
-
-    def calc_tag_state(self, data):
-        if len(data['packetList']):
-            if len(data['adv_address']) > 1:
+        self.all_tags_in_test = {}
+        self.tags_under_test = {}
+        self.reel_id = ''
+
+    def update_run_data(self):
+        run_data_path = abspath(join(self.test_data_dir, f'{self.common_run_name}@run_data.csv'))
+        dict_to_csv(dict_in=self.run_data, path=run_data_path)
+        self.logger.info(f'updated run data at {run_data_path}')
+        return run_data_path
+
+    def update_packets_data(self):
+        packets_data_path = abspath(join(self.test_data_dir, f'{self.common_run_name}@packets_data.csv'))
+        if self.results_df.empty:
+            return packets_data_path
+
+        self.results_df.insert(loc=len(self.results_df.columns), column='encryptedPacket',
+                               value=self.results_df['raw_packet'] + self.results_df['gw_packet'])
+
+        self.results_df.rename(columns={'time_from_start': 'time',
+                                        'external_id': 'externalId',
+                                        'is_pass': 'status'}, inplace=True)
+        df_to_save = self.results_df[['encryptedPacket', 'time', 'externalId', 'reel',
+                                      'adv_address', 'state(tbp_exists:0,no_tbp:-1,no_ttfp:-2,dup_adv_address:-3)',
+                                      'fail_bin', 'status', 'chamber', 'tbp', 'rssi',
+                                      'temperature_from_sensor', 'test_num',
+                                      'attenuation_ble', 'attenuation_lora']]
+        df_to_save.insert(0, 'commonRunName', self.common_run_name)
+        df_to_save.to_csv(packets_data_path, index=False, mode='w' if self.test_num == 0 else 'a',
+                          header=self.test_num == 0)
+        self.logger.info(f'updated packets data at {packets_data_path}')
+        return packets_data_path
+
+    def update_tags_data(self, df_to_save):
+        tags_data_path = abspath(join(self.test_data_dir, f'{self.common_run_name}@tags_data.csv'))
+        df_to_save.to_csv(tags_data_path, index=False, mode='w' if self.test_num == 0 else 'a',
+                          header=self.test_num == 0)
+        self.logger.info(f'updated tags data at {tags_data_path}')
+
+    @staticmethod
+    def calc_tag_state(data, test_status):
+        if data['tag_status'] == TagStatus.INSIDE_TEST:
+            if data['adva_dup']:
                 tag_state = FailBinSample.ADVA_DUPLICATION
-            elif data['ttfp'] == -1:
+            elif pd.isnull(data['tag_ttfp']):
                 tag_state = FailBinSample.NO_TTFP
-            elif data['tbp'] == -1:
+            elif data['tag_tbp'] == -1:
                 tag_state = FailBinSample.NO_TBP
             else:
                 tag_state = FailBinSample.TBP_EXISTS
         else:
-            if len(self.bad_advas) == 0:
+            if (test_status[TagStatus.OUT_VALID] + test_status[TagStatus.OUT_INVALID]) == 0:
                 tag_state = FailBinSample.NO_TTFP
-            elif any(b['is_valid'] for b in self.bad_advas):
+            elif test_status[TagStatus.OUT_VALID] > 0:
                 tag_state = FailBinSample.UNDETERMINED_ERROR
-            elif len(self.bad_advas) == sum([len(tag['packetList']) == 0 for tag in self.test_barcodes.values()]):
+            elif test_status[TagStatus.OUT_INVALID] == test_status[TagStatus.NO_RESPONSE]:
                 tag_state = FailBinSample.NO_SERIALIZATION
             else:
                 tag_state = FailBinSample.UNDETERMINED_ERROR
 
         return tag_state
 
     def files_and_cloud(self, post_data=False):
-        self.runDataDict['runEndTime'] = self.dataBaseDict['runEndTime'] = time.strftime('%d/%m/%y %H:%M:%S')
-        self.runDataDict['uploadToCloud'] = post_data and self.post_data
-        run_data_path = abspath(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@run_data.csv'))
-
-        self.update_run_data(run_data_path)
-
-        tags_data_path = abspath(
-            join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@packets_data.csv'))
-        if exists(tags_data_path):
-            remove(tags_data_path)
-        packets_csv = CsvLog(header_type=HeaderType.PACKETS, path=tags_data_path, tester_type=TesterName.SAMPLE)
-        packets_csv.open_csv()
-
-        for extId, data in self.test_barcodes.items():
-            if data['chamber'] < len(self.comConnect.temperature_sensor_readings):
-                all_reading_temp = self.comConnect.temperature_sensor_readings[data['chamber']]
-            else:
-                all_reading_temp = []
-            temperature_from_sensor = numpy.mean(all_reading_temp) if len(all_reading_temp) else float('nan')
-            tag_state = self.calc_tag_state(data)
-            if data['packetList'].packet_list.size > 0:
-                for sprinkler in data['packetList'].packet_list:
-                    for i in range(sprinkler.gw_data['gw_packet'].size):
-                        if sprinkler.gw_data["time_from_start"].size > 1:
-                            time_from_start = sprinkler.gw_data["time_from_start"][i]
-                        else:
-                            time_from_start = sprinkler.gw_data["time_from_start"].item()
-                        tag_row = {'commonRunName': self.common_run_name,
-                                   'encryptedPacket': sprinkler.get_packet_string(i),
-                                   'time': time_from_start,
-                                   'externalId': extId,
-                                   'reel': data['reel'], 'ttfp': data['ttfp'], 'tbp': data['tbp'],
-                                   'adv_address': data['adv_address'],
-                                   'state(tbp_exists:0,no_tbp:-1,no_ttfp:-2,dup_adv_address:-3)': tag_state.value,
-                                   'fail_bin': tag_state.name,
-                                   'status': data['status'], 'chamber': data['chamber'],
-                                   'temperature_from_sensor': temperature_from_sensor
-                                   }
-
-                        packets_csv.append_dict_as_row([tag_row])
-            else:  # add no response tags
-                tag_row = {'commonRunName': self.common_run_name,
-                           'encryptedPacket': '',
-                           'time': float('nan'),
-                           'externalId': extId,
-                           'reel': self.reel_id, 'ttfp': float('nan'), 'tbp': None,
-                           'adv_address': '',
-                           'state(tbp_exists:0,no_tbp:-1,no_ttfp:-2,dup_adv_address:-3)': tag_state.value,
-                           'fail_bin':tag_state.name,
-                           'status': False, 'chamber': None,
-                           'temperature_from_sensor': float('nan')
-                           }
-                packets_csv.append_dict_as_row([tag_row])
-
-        with open(abspath(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@configs_data.csv')),
-                  'w+', newline='') as newCsv:
-            writer = csv.DictWriter(newCsv, fieldnames=self.dataBaseDict.keys())
-            writer.writeheader()
-            writer.writerows([self.dataBaseDict])
-
-        with open(abspath(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@tags_data.csv')),
-                  'w+', newline='') as newCsv:
-            ids_dict = self.test_barcodes
-            tags = []
-            for extId, tag in ids_dict.items():
-                tag_state = self.calc_tag_state(tag)
-                if tag['chamber'] < len(self.comConnect.temperature_sensor_readings):
-                    all_reading_temp = self.comConnect.temperature_sensor_readings[tag['chamber']]
-                else:
-                    all_reading_temp = []
-                temperature_from_sensor = numpy.mean(all_reading_temp) if len(all_reading_temp) else float('nan')
-                temp_dict = {}
-                temp_dict['chamber'] = tag['chamber']
-                temp_dict['reel'] = tag['reel']
-                temp_dict['ext_id'] = extId
-                temp_dict['ttfp'] = tag['ttfp']
-                temp_dict['tbp'] = tag['tbp']
-                temp_dict['adv_address'] = tag['adv_address']
-                temp_dict['state(tbp_exists:0,no_tbp:-1,no_ttfp:-2,dup_adv_address:-3)'] = tag_state.value
-                temp_dict['fail_bin'] = tag_state.name
-                temp_dict['status'] = tag['status']
-                temp_dict['testName'] = self.testName
-                temp_dict['rssi'] = tag['rssi']
-                temp_dict['temperature_from_sensor'] = temperature_from_sensor
-
-                tags.append(temp_dict)
-
-            writer = csv.DictWriter(newCsv, fieldnames=tags[0].keys())
-            writer.writeheader()
-            writer.writerows(tags)
+        self.run_data['runEndTime'] = time.strftime('%d/%m/%y %H:%M:%S')
+        self.run_data['uploadToCloud'] = post_data and self.post_data
+
+        run_data_path = self.update_run_data()
+        packets_data_path = self.update_packets_data()
 
         if post_data and self.post_data:
-            post_success = self.post_to_cloud(run_data_path, tags_data_path, environment=self.environment)
+            post_success = self.post_to_cloud(run_data_path, packets_data_path, environment=self.environment)
             if post_success:
                 self.logger.info('files were uploaded!')
+                self.com_connect.popup_message(f'The following files were uploaded:\n' +
+                                               f'{self.common_run_name}@run_data.csv\n' +
+                                               f'{self.common_run_name}@packets_data.csv', log='info')
             else:
-                self.comConnect.popup_message(f'Failed uploading run and/or tags data, Upload manually:\n' +
-                                              f'{self.common_run_name}@run_data.csv\n' +
-                                              f'{self.common_run_name}@packets_data.csv', log='warning')
-                self.runDataDict['uploadToCloud'] = False
-                self.update_run_data(run_data_path)
-
-    def get_packet_ext_id(self, packet):
-        """
-        get external ID of a tag by sending an example packet to the cloud.
-        :type packet: Packet
-        :param packet: contains the raw and time of the packet.
-        :return: external ID of the tag, and the external ID parsed when it's wiliot tag.
-        """
-        full_data = {'barcode': None, 'cur_id': None, 'reel_id': None, 'gtin': None}
-        success = False
-        is_valid = False
-        if self.offline:
-            success = True
-            is_valid = True
-            if self.offline_tag_index <= len(self.barcodes_read.keys()) and len(self.barcodes_read.keys()) > 0:
-                full_data['cur_id'] = list(self.barcodes_read.keys())[self.offline_tag_index - 1]
-            else:
-                print(f'discard {packet.get_packet_string()} since too many tags detected')
-            full_data['reel_id'] = self.reel_id
-            if len(self.reel_id) < 4:
-                print('reel id smaller than 4 char assuming barcode format')
-                full_data['gtin'] = ''
-            else:
-                print('according to reel id length, assuming sgtin format')
-                full_data['gtin'] = SGTIN_PREFIX_DEFAULT
-            full_data['barcode'] = full_data['gtin'] + full_data['reel_id'] + 'T' + full_data['cur_id']
-            self.offline_tag_index += 1
-            return full_data, success, is_valid
-
-        packet_payload = packet.get_payload()
-
-        res = self.client.resolve_payload(payload=packet_payload, owner_id=self.owner, verbose=True)
-        if 'externalId' in res.keys():
-            if res['externalId'] != 'unknown':
-                full_data['barcode'] = res['externalId']
-                full_data['cur_id'] = full_data['reel_id'] = full_data['gtin'] = full_data['barcode']
-                try:
-                    is_valid = is_external_id_valid(full_data['barcode'])
-                    if is_valid:
-                        if ')' in full_data['barcode']:
-                            tag_data = full_data['barcode'].split(')')[2]
-                            full_data['gtin'] = ')'.join(full_data['barcode'].split(')')[:2]) + ')'
-                        elif len(full_data['barcode']) >= len(SGTIN_PREFIX_DEFAULT):  # gtin without parenthesis
-                            full_data['gtin'] = full_data['barcode'][0:18]
-                            tag_data = full_data['barcode'][18:]
-                        else:  # barcode or an other type with no prefix
-                            full_data['gtin'] = ''
-                            tag_data = full_data['barcode']
-
-                        full_data['cur_id'] = tag_data.split('T')[1].strip("' ")
-                        full_data['reel_id'] = tag_data.split('T')[0].strip("' ")
-                    success = True
-                except Exception as e:
-                    success = False
-                    print('got invalid external id: {} with exception: {}'.format(res, e))
-        return full_data, success, is_valid
+                self.com_connect.popup_message(f'Failed uploading run and/or tags data, Upload manually:\n' +
+                                               f'{self.common_run_name}@run_data.csv\n' +
+                                               f'{self.common_run_name}@packets_data.csv', log='warning')
+                self.run_data['uploadToCloud'] = False
+                self.update_run_data()
 
     def post_to_cloud(self, run_data_file_path, packets_data_file_path, environment='test/'):
         """
         post file to the cloud
         :type run_data_file_path: string
         :param run_data_file_path: the path to the uploaded run data file
         :type packets_data_file_path: string
@@ -1542,138 +966,86 @@
                                           is_path=True,
                                           env=environment,
                                           owner_id=self.owner,
                                           logger_='sample')
             first_iter = False
 
         if not success:
-            self.comConnect.popup_message(
-                f'Run upload failed. Check exception error at the console and check Internet connection is available and upload logs manually.',
+            self.com_connect.popup_message(
+                f'Run upload failed. Check exception error at the console and check Internet connection is available'
+                f' and upload logs manually.',
                 title='Upload Error',
                 log='error')
 
         return success
 
+    @staticmethod
+    def get_clean_tbp(tbp_arr):
+        mask = tbp_arr == -1
+        tbp_arr = tbp_arr[~mask]
+        return pd.Series(tbp_arr)
+
     def post_process(self):
-        tbp_arr = []
-        ttfp_arr = []
-        rssi_arr = []
-        status_arr = []
-        for extId, tag in self.test_barcodes.items():
-            status_temp = False
-            if tag['tbp'] != -1:
-                tbp_arr.append(tag['tbp'])
-                if self.params['tag_tbp_min'] != '' and self.params['tag_tbp_max'] != '':
-                    if int(self.params['tag_tbp_min']) < tag['tbp'] < int(self.params['tag_tbp_max']):
-                        status_temp = True
-                    else:
-                        status_temp = False
-                else:
-                    status_temp = True
-
-            if tag['ttfp'] != -1:
-                ttfp_arr.append(tag['ttfp'])
-            if tag['rssi'] != -1:
-                rssi_arr.append(tag['rssi'])
-            if len(tag['adv_address']) != 1:
-                status_temp = False
-            tag['status'] = status_temp
-            status_arr.append(status_temp)
-
-        pass_barcodes = [extId for extId, is_pass in zip(self.test_barcodes.keys(), status_arr) if is_pass]
-        tested_barcodes = len(self.test_barcodes.keys())
-        num_of_answered = len(ttfp_arr)
-        num_of_pass = len(pass_barcodes)
-        self.dataBaseDict['packets'] = self.numOfPackets
-        self.dataBaseDict['tested'] = self.runDataDict['tested'] = tested_barcodes
-        self.dataBaseDict['responded'] = self.runDataDict['responded'] = num_of_answered
-        self.dataBaseDict['passed'] = self.runDataDict['passed'] = num_of_pass
-        self.dataBaseDict['responding[%]'] = self.runDataDict['responding[%]'] = self.runDataDict['yield'] = \
-            f'{float((num_of_answered / tested_barcodes) * 100) if tested_barcodes > 0 else 0}%'
-        self.dataBaseDict['passed[%]'] = self.runDataDict[
-            'passed[%]'] = f'{float((num_of_pass / tested_barcodes) * 100 if tested_barcodes > 0 else 0)}%'
-        self.dataBaseDict['validTbp[%]'] = self.runDataDict[
-            'validTbp[%]'] = f'{float((num_of_pass / num_of_answered) * 100 if num_of_answered > 0 else 0)}%'
-        # calc ttfp
-        avg_ttfp = sum(ttfp_arr) / len(ttfp_arr) if len(ttfp_arr) > 0 else -1
-        ttfp_arr = ttfp_arr if len(ttfp_arr) > 0 else [-1]
 
-        self.dataBaseDict['ttfpStd'] = f'{numpy.std(ttfp_arr):.3f}'
-        self.runDataDict['ttfpAvg'] = self.dataBaseDict['ttfpAvg'] = f'{avg_ttfp:.3f}'
-        self.dataBaseDict['ttfpMin'] = f'{min(ttfp_arr):.3f}'
-        self.runDataDict['maxTtfp'] = self.dataBaseDict['ttfpMax'] = f'{max(ttfp_arr):.3f}'
+        # calc ttfp
+        avg_ttfp = self.all_results.groupby('external_id')['ttfp'].unique().apply(lambda x: x[-1]).mean()
+        max_ttfp = self.all_results.groupby('external_id')['ttfp'].unique().apply(lambda x: x[-1]).max()
+        self.run_data['ttfpAvg'] = f'{avg_ttfp:.3f}'
+        self.run_data['maxTtfp'] = f'{max_ttfp:.3f}'
 
         # calc tbp
-        avg_tbp = sum(tbp_arr) / len(tbp_arr) if len(tbp_arr) > 0 else -1
-        tbp_arr = tbp_arr if len(tbp_arr) > 0 else [-1]
-
-        self.runDataDict['tbpStd'] = self.dataBaseDict['tbpStd'] = f'{numpy.std(tbp_arr):.3f}'
-        self.runDataDict['tbpAvg'] = self.dataBaseDict['tbpAvg'] = f'{avg_tbp:.3f}'
-        self.dataBaseDict['tbpMin'] = f'{min(tbp_arr):.3f}'
-        self.dataBaseDict['tbpMax'] = f'{max(tbp_arr):.3f}'
-
-        avg_rssi = sum(rssi_arr) / len(rssi_arr) if len(rssi_arr) > 0 else -1
-        rssi_arr = rssi_arr if len(rssi_arr) > 0 else [-1]
-
-        self.runDataDict['rssiAvg'] = self.dataBaseDict['rssiAvg'] = str(avg_rssi)
-
-        return pass_barcodes
-
-    def reset(self):
-        """
-        reset the tester (fully available only when running from bat file)
-        """
-        global RESET
-        RESET = False
-        self.comConnect.cancel_gw_commands()
-        if popup_yes_no(f'Reset Sample test?'):
-            try:
-                self.comConnect.close()
-                self.comConnect.__del__()
-                self.remove_barcodes()
-
-                self.ttk.destroy()
-                RESET = True
-            except Exception as e:
-                print(f'could not reset due to: {e}')
-                exit(1)
-        else:
-            pass
+        all_tbp = self.get_clean_tbp(self.all_results.groupby('external_id')['tbp_min'].unique().apply(lambda x: x[-1]))
+        avg_tbp = all_tbp.mean()
+        std_tbp = all_tbp.std()
+        self.run_data['tbpStd'] = f'{std_tbp:.3f}'
+        self.run_data['tbpAvg'] = f'{avg_tbp:.3f}'
+
+        # rssi
+        avg_rssi = self.all_results.groupby('external_id')['rssi_mean'].unique().apply(lambda x: x[-1]).mean()
+        self.run_data['rssiAvg'] = str(avg_rssi)
+
+        n_tested = len(self.all_tags_in_test.keys())
+        n_answered = len(self.all_results.loc[
+                             self.all_results['resolve_status'] == TagStatus.INSIDE_TEST, 'external_id'].unique())
+        n_pass = sum([self.is_valid_tbp(x) for ex_id,x in zip(all_tbp.index,all_tbp.values)
+                      if ex_id in self.all_tags_in_test.keys()])
+
+        self.run_data['tested'] = n_tested
+        self.run_data['responded'] = n_answered
+        self.run_data['passed'] = n_pass
+        self.run_data['responding[%]'] = f'{float((n_answered / n_tested) * 100) if n_tested > 0 else 0}%'
+        self.run_data['passed[%]'] = f'{float((n_pass / n_tested) * 100 if n_tested > 0 else 0)}%'
+        self.run_data['yield'] = self.run_data['responding[%]']
+        self.run_data['validTbp[%]'] = f'{float((n_pass / n_answered) * 100 if n_answered > 0 else 0)}%'
 
     def close(self):
         """
         close the gui and destroy the test
         """
         try:
-            self.comConnect.close()
-            self.comConnect.gateway.exit_gw_api()
+            self.com_connect.close()
+            self.com_connect.gateway.exit_gw_api()
             self.ttk.destroy()
         except Exception as e:
             print(e)
             exit(1)
 
     def update_data(self):
         """
         update station name and owner in json file, for future usage.
         """
-        # temp_coms = {}
-        # if isfile(join(CONFIGS_DIR, '.defaults.json')):
-        #     with open(join(CONFIGS_DIR, '.defaults.json'), 'r') as defaultComs:
-        #         temp_coms = load(defaultComs)
-        # temp_coms.update(self.defaultDict)
-        temp_coms = self.comConnect.get_default_dict()
         if self.station_name.strip() != '':
-            temp_coms['stationName'] = self.station_name
-        if self.testConfig != '':
-            temp_coms['config'] = self.testConfig
+            self.default_config['stationName'] = self.station_name
+        if self.test_configs != '':
+            self.default_config['config'] = self.test_configs
         if self.calib:
-            temp_coms[f'{self.antenna}_calib'] = {'low': self.low, 'high': self.high, 'step': self.step}
+            self.default_config[f'{self.antenna}_calib'] = {'low': self.low, 'high': self.high, 'step': self.step}
 
         with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'w+') as defaultComs:
-            dump(temp_coms, defaultComs, indent=4)
+            dump(self.default_config, defaultComs, indent=4)
 
     def popup_login(self):
         """
         popup to insert fusion auth credentials, and choosing owner.
         """
         default_font = ("Helvetica", 10)
         popup = Tk()
@@ -1688,52 +1060,72 @@
                 exit(1)
 
         popup.protocol("WM_DELETE_WINDOW", quit_tester)
 
         def ok():
             self.owner = c1.get()
             self.station_name = e3.get()
+            self.calib = c_calib.get() == 'yes'
+            self.offline = c_cloud.get() == 'no'
             popup.destroy()
 
-        l1 = Label(popup, text='Choose owner and station name:', font=default_font)
+        l1 = Label(popup, text='Run configuration:', font=default_font)
         l1.grid(row=2, column=0, padx=10, pady=10, columnspan=3)
+
+        l3 = Label(popup, text='Online Mode (Cloud connection):', font=default_font)
+        l3.grid(row=5, column=0, padx=10, pady=10)
+        c_cloud = ttk.Combobox(popup, state='normal')
+        c_cloud.grid(row=5, column=1, padx=10, pady=15)
+        c_cloud['values'] = ['yes', 'no']
+        c_cloud.set('yes')
+
+        l3 = Label(popup, text='Calibration Mode:', font=default_font)
+        l3.grid(row=4, column=0, padx=10, pady=10)
+        c_calib = ttk.Combobox(popup, state='normal')
+        c_calib.grid(row=4, column=1, padx=10, pady=15)
+        c_calib['values'] = ['yes', 'no']
+        c_calib.set('no')
+
         l4 = Label(popup, text='Owner:', font=default_font)
         l4.grid(row=6, column=0, padx=10, pady=10)
         c1 = ttk.Combobox(popup, state='normal')
         c1.grid(row=6, column=1, padx=10, pady=15)
+
         l5 = Label(popup, text='Station Name:', font=default_font)
         l5.grid(row=7, column=0, padx=10, pady=10)
         e3 = Entry(popup)
-        if 'stationName' in self.defaultDict.keys():
-            e3.insert(0, self.defaultDict['stationName'])
+        if 'stationName' in self.default_config.keys():
+            e3.insert(0, self.default_config['stationName'])
         e3.grid(row=7, column=1, padx=10, pady=5)
         b3 = Button(popup, text="OK", command=ok, height=1, width=10)
         b3.grid(row=8, column=1, padx=10, pady=10)
 
-        if 'owner' in self.defaultDict.keys():
-            owner_id_list = self.defaultDict['owner'] \
-                if isinstance(self.defaultDict['owner'], list) else [self.defaultDict['owner']]
+        if 'owner' in self.default_config.keys():
+            owner_id_list = self.default_config['owner'] \
+                if isinstance(self.default_config['owner'], list) else [self.default_config['owner']]
         else:
             owner_id_list = ['']
         c1['values'] = owner_id_list
-        c1.set(owner_id_list[-1])
+        c1.set(self.default_config.get('selected_owner', owner_id_list[-1]))
 
         popup.mainloop()
 
+        # update configs:
+        self.default_config['selected_owner'] = self.owner
         if self.owner not in owner_id_list:
             owner_id_list.append(self.owner)
             owner_id_list = [o for o in owner_id_list if o != '']
-            self.defaultDict['owner'] = owner_id_list
-            with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'w+') as defaultComs:
-                dump(self.defaultDict, defaultComs, indent=4)
+            self.default_config['owner'] = owner_id_list
+            with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'w+') as defaults:
+                dump(self.default_config, defaults, indent=4)
 
     def update_default_dict(self, field, value):
         antenna = self.antenna.lower()
-        if f'{antenna}_calib' in self.defaultDict.keys():
-            self.defaultDict[f'{antenna}_calib'][field] = value
+        if f'{antenna}_calib' in self.default_config.keys():
+            self.default_config[f'{antenna}_calib'][field] = value
 
     def popup_calib(self):
         """
         popup to choose calib mode parameters
         """
         default_font = ("Helvetica", 10)
         popup = Tk()
@@ -1747,21 +1139,21 @@
         def ok():
             self.low = e2.get()
             self.high = e3.get()
             self.step = e4.get()
             self.n_repetitions = e5.get()
             # save the dictionary back to the file
             with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'w') as defaultComs:
-                dump(self.defaultDict, defaultComs)
+                dump(self.default_config, defaultComs)
             popup.destroy()
 
         def update_antenna_params(*args):
             self.antenna = antenna = c2.get().lower()
-            if f'{antenna}_calib' in self.defaultDict.keys():
-                antennaDict = self.defaultDict[f'{antenna}_calib']
+            if f'{antenna}_calib' in self.default_config.keys():
+                antennaDict = self.default_config[f'{antenna}_calib']
                 e2.delete(0, END)
                 e3.delete(0, END)
                 e4.delete(0, END)
                 e5.delete(0, END)
                 e2.insert(0, antennaDict['low'])
                 e3.insert(0, antennaDict['high'])
                 e4.insert(0, antennaDict['step'])
@@ -1798,14 +1190,287 @@
         b1 = Button(popup, text="Quit", command=quit_calib, height=1, width=10)
         b1.grid(row=7, column=0, padx=10, pady=10)
         b2 = Button(popup, text="Ok", command=ok, height=1, width=10)
         b2.grid(row=7, column=1, padx=10, pady=10)
 
         popup.mainloop()
 
+    # ############## GUI Callbacks  #######################
+
+    def go_cb(self):
+        if self.finish_thread is not None and self.finish_thread.is_alive():
+            self.logger.info('wait for finish process to be done')
+            self.finish_thread.join()
+        self.go_button_state = self.builder.tkvariables.get('go').get()
+        self.builder.get_object('stop')['state'] = 'disabled'
+        self.builder.get_object('settings_combobox')['state'] = 'disabled'
+
+        self.update_params_state(state='disabled', group=GO)
+        self.builder.get_variable('forceGo').set('0')
+        self.force_close_requested = False
+        if self.go_button_state == CONNECT_HW:
+            self.connect_thread = Thread(target=self.connect_all, args=([False]))
+            self.connect_thread.start()
+        elif self.go_button_state == READ:
+            self.builder.get_object('settings_combobox')['state'] = 'disabled'
+            if self.stop_button_state == SEND:
+                self.remove_barcodes()
+                self.stop_button_state = FINISH
+                self.builder.tkvariables.get('stop').set(FINISH)
+            indexes = self.get_missing_ids_chambers()
+            test_barcodes_thread = Thread(target=self.read_scanners_barcodes, args=([indexes]))
+            test_barcodes_thread.start()
+        elif self.go_button_state == GO:
+            # calib data:
+            if self.calib:
+                pop_calib_th = Thread(target=self.popup_calib, args=())
+                pop_calib_th.start()
+                pop_calib_th.join()
+
+            self.update_params()
+
+            self.builder.get_object('stop')['state'] = 'normal'
+            self.builder.tkvariables.get('stop').set(STOP)
+            self.stop_button_state = STOP
+            # create a dir for log
+            self.init_data_log()
+
+            if self.calib:
+                self.calib_mode_thread = Thread(target=self.calib_mode, args=())
+                self.calib_mode_thread.start()
+            else:
+                self.tag_test_thread = Thread(target=self.tag_test, args=())
+                self.tag_test_thread.start()
+
+        elif self.go_button_state == CONTINUE:
+            self.builder.tkvariables.get('stop').set(STOP)
+            self.stop_button_state = STOP
+            self.test_num += 1
+
+            self.tag_test_thread.join(timeout=1)
+            if self.tag_test_thread.is_alive():
+                raise Exception('tag thread test still running - the applicaiton needs restart')
+
+            self.tag_test_thread = Thread(target=self.tag_test, args=())
+            self.tag_test_thread.start()
+
+    def choose_param_cb(self, *args):
+        var = args[0].widget['style'].split('.')[0]
+        if self.builder.tkvariables.get(var) is not None:
+            value = self.builder.get_object(var).get()
+            if var not in self.default_config.keys():
+                self.default_config[var] = []
+            if value in self.default_config[var]:
+                self.default_config[var].pop(self.default_config[var].index(value))
+            self.default_config[var].insert(0, value)
+
+    def reset_cb(self):
+        """
+        reset the tester (fully available only when running from bat file)
+        """
+        if popup_yes_no(f'Reset Sample test?'):
+            try:
+                self.com_connect.close()
+                self.com_connect.__del__()
+                self.remove_barcodes()
+                self.com_connect.choose_com_ports()
+                self.reset_app_data()
+            except Exception as e:
+                print(f'could not reset due to: {e}')
+                exit(1)
+        else:
+            pass
+
+    def stop_cb(self):
+        """
+        stop the test and run post process
+        """
+        if self.stop_button_state == STOP:
+            self.force_close_requested = True
+            self.stop_event.set()
+
+        elif self.stop_button_state == FINISH:
+            self.builder.get_object('scanned').delete(0, END)
+            self.builder.tkvariables.get('stop').set(SEND)
+            self.stop_button_state = SEND
+            for barcode in list(self.all_tags_in_test.keys()):
+                self.builder.get_object('scanned').insert(END, barcode)
+
+        elif self.stop_button_state == SEND:
+            if not self.is_test_completed() and 'controlLimits' in self.default_config.keys():
+                control_limits = self.default_config['controlLimits'][self.default_config['controlLimitsTestNum']]
+                self.update_values_for_control_limits(control_limits=control_limits)
+                is_pass, fail_str, complete_sub_test, fail_bin = self.check_control_limits()
+                self.reset_values_for_control_limits(control_limits=control_limits)
+                if not is_pass or not complete_sub_test:
+                    send_anyway = popup_yes_no(f'Test was FAILED!! are you sure you want to finish the test and '
+                                               f'send data to the cloud?')
+                    if not send_anyway:
+                        self.logger.info('User decide to keep testing')
+                        return
+            self.builder.get_object('go')['state'] = 'disabled'
+            self.builder.get_object('stop')['state'] = 'disabled'
+            self.builder.get_object('forceGo')['state'] = 'disabled'
+            self.builder.get_object('add')['state'] = 'disabled'
+            self.builder.get_object('remove')['state'] = 'disabled'
+            self.finish_thread = Thread(target=self.finish, args=())
+            self.finish_thread.start()
+
+    def add_cb(self):
+        """
+        add manually tag to the list
+        """
+        new_tag = self.builder.tkvariables.get('addTag').get()
+        if self.builder.tkvariables.get('stop').get() != SEND or len(new_tag.split(',')) == 2:
+            new_tag_id = self.get_external_id_from_monitor(new_tag)
+            if new_tag_id in self.tags_under_test.keys():
+                retest = popup_yes_no(f'Tag {new_tag_id} was already tested, are you sure you want to re-test the tag?')
+                if not retest:
+                    self.builder.tkvariables.get('addTag').set('')
+                    return
+
+            if self.builder.tkvariables.get('stop').get() == SEND:
+                self.builder.get_object('scanned').delete(0, END)
+                self.remove_barcodes()
+                self.stop_button_state = FINISH
+                self.builder.tkvariables.get('stop').set(FINISH)
+
+            if len(new_tag.split(',')) < 2:
+                self.com_connect.popup_message(f'Missing chamber index, add chamber index after a comma.',
+                                               title='Error',
+                                               log='error')
+                return
+            scan_index = int(new_tag.split(',')[1].strip())
+            if 0 < self.com_connect.get_num_of_barcode_scanners() < (scan_index + 1):
+                self.com_connect.popup_message(f'Chamber number {scan_index} not exists.', title='Error', log='error')
+                return
+
+            barcodes = self.builder.get_object('scanned').get(0, END)
+            if any([barcode for barcode in barcodes if int(barcode.split()[1].strip()) == scan_index]):
+                self.com_connect.popup_message(f'Chamber {scan_index} tag already scanned.', title='Error', log='error')
+                return
+            # logger.info(scan_index)
+
+            self.builder.tkvariables.get('addTag').set('')
+            added_to_test = self.add_tag_to_test(new_tag_id, self.reel_id, scan_index, add_to_test=True)
+            if added_to_test:
+                popup_thread = Thread(target=self.com_connect.popup_message,
+                                      args=('Chambers are closing!!\nWatch your hands!!!',
+                                            'Warning', ("Helvetica", 18), 'warning'))
+                popup_thread.start()
+                popup_thread.join()
+                chambers = self.com_connect.get_chambers()
+                if len(chambers) > scan_index and chambers[scan_index] is not None:
+                    chambers[scan_index].close_chamber()
+            self.update_go_state()
+        else:
+            self.builder.get_object('scanned').insert(END, new_tag)
+            self.builder.tkvariables.get('addTag').set('')
+
+    def remove_cb(self):
+        """
+        remove tag read from the list
+        """
+        tag = self.builder.get_object('scanned').get(ACTIVE)
+        tags = list(self.builder.get_object('scanned').get(0, END))
+        tag_index = tags.index(tag)
+        self.builder.get_object('scanned').delete(tag_index, tag_index)
+        tags.pop(tag_index)
+        self.builder.tkvariables.get('addTag').set(tag)
+        if self.stop_button_state != SEND:
+            self.tags_under_test.pop(self.get_external_id_from_monitor(tag))
+            self.com_connect.open_chambers(indexes=[int(tag.split(',')[1].strip())])
+            self.update_go_state()
+
+    def get_external_id_from_monitor(self, tag_str):
+        external_id = tag_str.split(',')[0].strip()
+        external_id = f'{self.reel_id}T{external_id}' if len(external_id) == TAG_COUNTER_LEN else external_id
+        return external_id
+
+    def open_configs_cb(self):
+        """
+        open Configs GUI
+        """
+        if self.configs_gui is not None and not self.configs_gui.is_gui_opened():
+            self.configs_gui.gui()
+
+    def test_config_cb(self, *args):
+        """
+        update the configs in Configs module according to the main GUI
+        """
+        self.configs_gui.config_set(self.builder.get_object('test_config').get())
+
+    def open_com_ports_cb(self):
+        """
+        open ComConnect GUI
+        """
+        if self.com_connect is not None and not self.com_connect.is_gui_opened():
+            self.com_connect.gui()
+
+    def read_qr_cb(self):
+        indexes = self.com_connect.get_all_scanners_index()
+        barcode, reel = None, None
+        for i in indexes:
+            barcode, reel = self.com_connect.read_barcode(scanner_index=i)
+            if barcode is not None:
+                break
+
+        if barcode is None:
+            read_qr_thread = Thread(target=self.com_connect.popup_message, args=(
+                [f'Error reading external ID, try repositioning the tag.', 'Error', ("Helvetica", 10), 'error']))
+            read_qr_thread.start()
+            read_qr_thread.join()
+            if not self.calib:
+                return
+
+        if reel is not None:
+            reel_id = self.builder.tkvariables.get('reelId')
+            reel_id.set(reel)
+            self.reel_id = reel
+
+        if 'config' in self.default_config.keys():
+            self.test_configs = self.default_config['config']
+        else:
+            self.test_configs = ''
+
+        self.builder.get_object('reelId').unbind("<Key>")
+        self.update_params_state(state='normal', group=GO)
+        self.builder.get_object('forceGo')['state'] = 'normal'
+
+    def get_reel_id_cb(self, *args):
+        reel = self.builder.tkvariables.get('reelId').get()
+        if reel.strip() != '' and (str(args[0].type) != 'KeyPress' or args[0].keysym == 'Return'):
+            self.reel_id = reel
+            self.update_params_state(state='normal', group=GO)
+            self.builder.get_object('reelId').unbind("<Key>")
+            self.builder.get_object('forceGo')['state'] = 'normal'
+
+    def force_go_cb(self):
+        """
+        enable go in the GUI even if some of the chambers are empty
+        """
+        if self.builder.get_variable('forceGo').get() == '1':
+            self.builder.get_object('forceGo')['state'] = 'disabled'
+            self.builder.get_object('stop')['state'] = 'disabled'
+            self.builder.get_object('go')['state'] = 'disabled'
+            self.builder.get_object('add')['state'] = 'disabled'
+            self.builder.get_object('remove')['state'] = 'disabled'
+            self.builder.get_object('settings_combobox')['state'] = 'disabled'
+            if self.closeChambersThread is not None and self.closeChambersThread.is_alive():
+                self.closeChambersThread.join()
+            self.closeChambersThread = Thread(target=self.force_go_close_chambers, args=())
+            self.closeChambersThread.start()
+        else:
+            self.update_go_state()
+
+    def on_env_change_cb(self, event=None):
+
+        self.environment = self.settings_combobox.get()
+        self.logger.info(f'Environment set to {self.environment}')
+
 
 def popup_yes_no(question, tk_frame=None):
     if tk_frame is None:
         root = Tk()
         root.eval(f'tk::PlaceWindow {str(root)} center')
     else:
         root = tk_frame
@@ -1814,52 +1479,10 @@
     root.destroy()
     if result == 'yes':
         return True
     else:
         return False
 
 
-def float_precision(num, prec=2):
-    dot_pos = str(num).index('.')
-    first_idx = [i for i in range(len(str(num))) if str(num)[i] != '0' and str(num)[i] != '.']
-    first_idx = first_idx[0] if first_idx[0] > 0 else first_idx[0] + 1
-    after_dot = first_idx - dot_pos + prec
-    if after_dot > 0:
-        eval_str = '{:.%sf}' % (str(first_idx - dot_pos + prec))
-    else:
-        eval_str = '{:.0f}'
-    return float(eval_str.format(num))
-
-
 if __name__ == '__main__':
-    global RESET
-    RESET = False
-    parser = argparse.ArgumentParser(description='Run PixieParser')
-    parser.add_argument('-c', '--calib', help='Calibration mode', default=False, action='store_true')
-    parser.add_argument('-e', '--environment', help='Environment: test or not', default='prod')
-    parser.add_argument('-p', '--post_data', help='Post data to the cloud', default=True)
-    parser.add_argument('-o', '--offline', help='Offline mode', default=False, action='store_true')
-    args = parser.parse_args()
-    calib = args.calib
-    post_data = args.post_data
-    offline = args.offline
-
-    # Run the UI
-    # calib = True
-    # offline = True
-    if calib:
-        print(f'Sample Test - calibration mode active.')
-    if offline:
-        print(f'Sample Test - offline mode active.')
-    app_folder = abspath(join(dirname(__file__), '../wiliot_testers'))
-    is_first_run = True
-    while is_first_run or RESET:
-        is_first_run = False
-        try:
-            RESET = False
-            sampleTest = SampleTest(calib=calib, environment=args.environment, post_data=post_data,
-                                    offline=offline)
-            sampleTest.gui()
-        except BaseException:
-            print_exc()
-            exit(0)
-            break
+    sampleTest = SampleTest()
+    sampleTest.gui()
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/com_connect.ui` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/com_connect.ui`

 * *Files 1% similar despite different names*

#### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/com_connect.ui` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/com_connect.ui`

```diff
@@ -37,16 +37,16 @@
           <property id="0" name="pad" type="col">0</property>
           <property id="0" name="weight" type="col">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="gwCom">
-        <bind add="True" handler="choose_gw" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
-        <bind add="True" handler="find_com_ports" sequence="&lt;FocusIn&gt;"/>
+        <bind add="True" handler="choose_gw_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="True" handler="find_com_ports_cb" sequence="&lt;FocusIn&gt;"/>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="padx">10</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">2</property>
         </layout>
@@ -79,16 +79,16 @@
           <property id="0" name="pad" type="col">0</property>
           <property id="0" name="weight" type="col">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="attenComBle">
-        <bind add="True" handler="choose_ble_atten" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
-        <bind add="True" handler="find_com_ports" sequence="&lt;FocusIn&gt;"/>
+        <bind add="True" handler="choose_ble_atten_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="True" handler="find_com_ports_cb" sequence="&lt;FocusIn&gt;"/>
         <layout manager="grid">
           <property name="column">6</property>
           <property name="padx">10</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">2</property>
         </layout>
@@ -146,16 +146,16 @@
           <property name="propagate">True</property>
           <property name="row">3</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="attenComLoRa">
-        <bind add="True" handler="choose_lora_atten" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
-        <bind add="True" handler="find_com_ports" sequence="&lt;FocusIn&gt;"/>
+        <bind add="True" handler="choose_lora_atten_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="True" handler="find_com_ports_cb" sequence="&lt;FocusIn&gt;"/>
         <layout manager="grid">
           <property name="column">6</property>
           <property name="propagate">True</property>
           <property name="row">3</property>
         </layout>
       </object>
     </child>
@@ -217,15 +217,15 @@
           <property name="propagate">True</property>
           <property name="row">8</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="tk.Listbox" id="availableBarcodes">
-        <bind add="True" handler="focus_barcode_available" sequence="&lt;FocusIn&gt;"/>
+        <bind add="True" handler="focus_barcode_available_cb" sequence="&lt;FocusIn&gt;"/>
         <layout manager="grid">
           <property name="column">0</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">9</property>
         </layout>
@@ -241,15 +241,15 @@
           <property name="propagate">True</property>
           <property name="row">9</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="tk.Listbox" id="chosenBarcodes">
-        <bind add="True" handler="focus_barcode_chosen" sequence="&lt;FocusIn&gt;"/>
+        <bind add="True" handler="focus_barcode_chosen_cb" sequence="&lt;FocusIn&gt;"/>
         <layout manager="grid">
           <property name="column">2</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">9</property>
         </layout>
@@ -283,15 +283,15 @@
           <property name="row">9</property>
           <property name="sticky">se</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="tk.Listbox" id="availableChambers">
-        <bind add="True" handler="focus_chamber_available" sequence="&lt;FocusIn&gt;"/>
+        <bind add="True" handler="focus_chamber_available_cb" sequence="&lt;FocusIn&gt;"/>
         <layout manager="grid">
           <property name="column">5</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">9</property>
         </layout>
@@ -309,15 +309,15 @@
           <property name="propagate">True</property>
           <property name="row">9</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="tk.Listbox" id="chosenChambers">
-        <bind add="True" handler="focus_chamber_chosen" sequence="&lt;FocusIn&gt;"/>
+        <bind add="True" handler="focus_chamber_chosen_cb" sequence="&lt;FocusIn&gt;"/>
         <layout manager="grid">
           <property name="column">7</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">9</property>
         </layout>
@@ -394,15 +394,15 @@
           <property id="0" name="pad" type="col">0</property>
           <property id="0" name="weight" type="col">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="refresh">
-        <property cbtype="simple" name="command" type="command">find_com_ports</property>
+        <property cbtype="simple" name="command" type="command">find_com_ports_cb</property>
         <property name="image">refresh.gif</property>
         <property name="text" translatable="yes">refresh</property>
         <layout manager="grid">
           <property name="column">0</property>
           <property name="padx">10</property>
           <property name="pady">10</property>
           <property name="propagate">True</property>
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/comm.gif` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/comm.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/configs.gif` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/configs.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/configs.ui` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/configs.ui`

 * *Files 0% similar despite different names*

#### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/configs.ui` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/configs.ui`

```diff
@@ -19,30 +19,30 @@
           <property name="propagate">True</property>
           <property name="row">1</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="configsList">
-        <bind add="True" handler="config_select" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
-        <bind add="" handler="config_select" sequence="&lt;FocusOut&gt;"/>
+        <bind add="True" handler="config_select_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="" handler="config_select_cb" sequence="&lt;FocusOut&gt;"/>
         <layout manager="grid">
           <property name="column">2</property>
           <property name="columnspan">3</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">1</property>
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="save">
-        <property cbtype="simple" name="command" type="command">save</property>
+        <property cbtype="simple" name="command" type="command">save_cb</property>
         <property name="image">save.png</property>
         <property name="text" translatable="yes">Save</property>
         <layout manager="grid">
           <property name="column">5</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
@@ -217,16 +217,16 @@
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="antennaType">
         <property name="textvariable">string:antennaType</property>
         <property name="values">TEO TIKI</property>
-        <bind add="" handler="choose_antenna_type" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
-        <bind add="" handler="choose_antenna_type" sequence="&lt;FocusOut&gt;"/>
+        <bind add="" handler="choose_antenna_type_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="" handler="choose_antenna_type_cb" sequence="&lt;FocusOut&gt;"/>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="propagate">True</property>
           <property name="row">10</property>
         </layout>
       </object>
     </child>
@@ -331,15 +331,15 @@
           <property name="propagate">True</property>
           <property name="row">3</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="atten_mode">
-        <property cbtype="simple" name="command" type="command">atten_mode</property>
+        <property cbtype="simple" name="command" type="command">atten_mode_cb</property>
         <property name="text" translatable="yes">Measured</property>
         <property name="textvariable">string:atten_mode</property>
         <layout manager="grid">
           <property name="column">6</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
@@ -422,29 +422,29 @@
           <property name="row">20</property>
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="reset">
-        <property cbtype="simple" name="command" type="command">reset</property>
+        <property cbtype="simple" name="command" type="command">reset_cb</property>
         <property name="text" translatable="yes">Reset</property>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">22</property>
           <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="close">
-        <property cbtype="simple" name="command" type="command">close</property>
+        <property cbtype="simple" name="command" type="command">close_cb</property>
         <property name="text" translatable="yes">Close</property>
         <layout manager="grid">
           <property name="column">5</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">22</property>
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/reset.png` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/reset.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/sample_test.ui` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/sample_test.ui`

 * *Files 1% similar despite different names*

#### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/sample_test.ui` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/sample_test.ui`

```diff
@@ -41,15 +41,15 @@
           <property name="row">1</property>
           <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="connect">
-        <property cbtype="simple" name="command" type="command">open_com_ports</property>
+        <property cbtype="simple" name="command" type="command">open_com_ports_cb</property>
         <property name="image">comm.gif</property>
         <property name="text" translatable="yes">connect</property>
         <layout manager="grid">
           <property name="column">2</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
@@ -81,15 +81,15 @@
           <property name="propagate">True</property>
           <property name="row">2</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="read_qr">
-        <property cbtype="simple" name="command" type="command">read_qr</property>
+        <property cbtype="simple" name="command" type="command">read_qr_cb</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">Read QR</property>
         <layout manager="grid">
           <property name="column">2</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
@@ -109,15 +109,15 @@
       </object>
     </child>
     <child>
       <object class="ttk.Entry" id="reelId">
         <property name="state">disabled</property>
         <property name="textvariable">string:reelId</property>
         <property name="width">35</property>
-        <bind add="" handler="get_reel_id" sequence="&lt;FocusOut&gt;"/>
+        <bind add="" handler="get_reel_id_cb" sequence="&lt;FocusOut&gt;"/>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">3</property>
           <property id="3" name="weight" type="row">0</property>
@@ -137,27 +137,27 @@
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="test_config">
         <property name="state">disabled</property>
         <property name="textvariable">string:test_config</property>
-        <bind add="True" handler="test_config" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="True" handler="test_config_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">7</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="configs">
-        <property cbtype="simple" name="command" type="command">open_configs</property>
+        <property cbtype="simple" name="command" type="command">open_configs_cb</property>
         <property name="image">configs.gif</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">Configs</property>
         <layout manager="grid">
           <property name="column">2</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
@@ -239,16 +239,16 @@
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="testName">
         <property name="state">disabled</property>
         <property name="style">testName.TCombobox</property>
         <property name="textvariable">string:testName</property>
-        <bind add="True" handler="choose_param" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
-        <bind add="True" handler="choose_param" sequence="&lt;FocusOut&gt;"/>
+        <bind add="True" handler="choose_param_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="True" handler="choose_param_cb" sequence="&lt;FocusOut&gt;"/>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">12</property>
         </layout>
@@ -265,16 +265,16 @@
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="operator">
         <property name="state">disabled</property>
         <property name="style">operator.TCombobox</property>
         <property name="textvariable">string:operator</property>
-        <bind add="True" handler="choose_param" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
-        <bind add="True" handler="choose_param" sequence="&lt;FocusOut&gt;"/>
+        <bind add="True" handler="choose_param_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="True" handler="choose_param_cb" sequence="&lt;FocusOut&gt;"/>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">13</property>
         </layout>
@@ -293,16 +293,16 @@
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="inlay">
         <property name="state">disabled</property>
         <property name="style">inlay.TCombobox</property>
         <property name="textvariable">string:inlay</property>
-        <bind add="True" handler="choose_param" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
-        <bind add="True" handler="choose_param" sequence="&lt;FocusOut&gt;"/>
+        <bind add="True" handler="choose_param_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="True" handler="choose_param_cb" sequence="&lt;FocusOut&gt;"/>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">15</property>
         </layout>
@@ -321,16 +321,16 @@
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="surface">
         <property name="state">disabled</property>
         <property name="style">surface.TCombobox</property>
         <property name="textvariable">string:surface</property>
-        <bind add="" handler="choose_param" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
-        <bind add="" handler="choose_param" sequence="&lt;FocusOut&gt;"/>
+        <bind add="" handler="choose_param_cb" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
+        <bind add="" handler="choose_param_cb" sequence="&lt;FocusOut&gt;"/>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
           <property name="row">16</property>
         </layout>
@@ -385,15 +385,15 @@
           <property name="row">19</property>
           <property name="sticky">nsw</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="remove">
-        <property cbtype="simple" name="command" type="command">remove</property>
+        <property cbtype="simple" name="command" type="command">remove_cb</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">-</property>
         <property name="width">2</property>
         <layout manager="grid">
           <property name="column">2</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
@@ -424,15 +424,15 @@
           <property name="propagate">True</property>
           <property name="row">20</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="add">
-        <property cbtype="simple" name="command" type="command">add</property>
+        <property cbtype="simple" name="command" type="command">add_cb</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">+</property>
         <property name="width">2</property>
         <layout manager="grid">
           <property name="column">2</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
@@ -452,30 +452,30 @@
           <property name="row">21</property>
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Checkbutton" id="forceGo">
-        <property cbtype="simple" name="command" type="command">force_go</property>
+        <property cbtype="simple" name="command" type="command">force_go_cb</property>
         <property name="offvalue">0</property>
         <property name="onvalue">1</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">Force Go</property>
         <property name="variable">string:forceGo</property>
         <layout manager="grid">
           <property name="column">0</property>
           <property name="propagate">True</property>
           <property name="row">22</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="go">
-        <property cbtype="simple" name="command" type="command">go</property>
+        <property cbtype="simple" name="command" type="command">go_cb</property>
         <property name="text" translatable="yes">Connect HW</property>
         <property name="textvariable">string:go</property>
         <layout manager="grid">
           <property name="column">0</property>
           <property name="columnspan">3</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
@@ -498,15 +498,15 @@
           <property name="sticky">ew</property>
           <property id="0" name="pad" type="col">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="stop">
-        <property cbtype="simple" name="command" type="command">stop</property>
+        <property cbtype="simple" name="command" type="command">stop_cb</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">Stop</property>
         <property name="textvariable">string:stop</property>
         <layout manager="grid">
           <property name="column">0</property>
           <property name="columnspan">3</property>
           <property name="padx">5</property>
@@ -515,15 +515,15 @@
           <property name="row">26</property>
           <property id="0" name="pad" type="col">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="reset">
-        <property cbtype="simple" name="command" type="command">reset</property>
+        <property cbtype="simple" name="command" type="command">reset_cb</property>
         <property name="image">reset.png</property>
         <property name="text" translatable="yes">reset</property>
         <layout manager="grid">
           <property name="column">0</property>
           <property name="padx">5</property>
           <property name="pady">5</property>
           <property name="propagate">True</property>
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sample/utils/wiliot3.gif` & `wiliot-testers-5.4.13/wiliot_testers/sample/utils/wiliot3.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sensors/get_light.py` & `wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/get_light.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/sensors/get_temperature.py` & `wiliot-testers-5.4.13/wiliot_testers/sensors_and_hardware/get_temperature.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/system_test/harvester_test.py` & `wiliot-testers-5.4.13/wiliot_testers/system_test/harvester_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,16 +56,21 @@
 #     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 '''
 Eduard Tatievski
 '''
+import re
+import sys
+import threading
 
 import matplotlib.pyplot as plt
+from wiliot_core import PacketList
+
 from wiliot_testers.calibration_test.calibration_test_by_tbp import *
 from wiliot_core.packet_data import packet_list, packet, tag_collection
 from wiliot_testers.test_equipment import Attenuator, EquipmentError
 from wiliot_testers.wiliot_tester_log import *
 import PySimpleGUI as SimGUI
 import os
 import pathlib
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/system_test/system_test_example.py` & `wiliot-testers-5.4.13/wiliot_testers/system_test/system_test_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/test_equipment.py` & `wiliot-testers-5.4.13/wiliot_testers/test_equipment.py`

 * *Files 2% similar despite different names*

```diff
@@ -813,2840 +813,2973 @@
 000032c0: 735f 6c69 7374 203d 2073 6572 6961 6c5f  s_list = serial_
 000032d0: 706f 7274 7328 290a 2020 2020 2020 2020  ports().        
 000032e0: 2020 2020 2020 2020 666f 7220 706f 7274          for port
 000032f0: 2069 6e20 706f 7274 735f 6c69 7374 3a0a   in ports_list:.
 00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003310: 2020 2020 7365 6c66 2e63 6f6d 706f 7274      self.comport
 00003320: 203d 2070 6f72 740a 2020 2020 2020 2020   = port.        
-00003330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003340: 2e73 203d 2073 6572 6961 6c2e 5365 7269  .s = serial.Seri
-00003350: 616c 2873 656c 662e 636f 6d70 6f72 742c  al(self.comport,
-00003360: 2073 656c 662e 6261 7564 7261 7465 2c20   self.baudrate, 
-00003370: 7469 6d65 6f75 743d 302e 3529 0a20 2020  timeout=0.5).   
-00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003390: 2073 6c65 6570 2831 290a 2020 2020 2020   sleep(1).      
-000033a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000033b0: 6c66 2e73 2e66 6c75 7368 496e 7075 7428  lf.s.flushInput(
-000033c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000033d0: 2020 2020 2020 7365 6c66 2e73 2e66 6c75        self.s.flu
-000033e0: 7368 4f75 7470 7574 2829 0a20 2020 2020  shOutput().     
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003400: 6c65 6570 2830 2e31 290a 2020 2020 2020  leep(0.1).      
-00003410: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00003420: 5475 726e 2074 6865 2063 6f6e 736f 6c65  Turn the console
-00003430: 206f 6666 0a20 2020 2020 2020 2020 2020   off.           
-00003440: 2020 2020 2020 2020 2073 656c 662e 732e           self.s.
-00003450: 7772 6974 6528 2243 4f4e 534f 4c45 2044  write("CONSOLE D
-00003460: 4953 4142 4c45 5c72 5c6e 222e 656e 636f  ISABLE\r\n".enco
-00003470: 6465 2829 290a 2020 2020 2020 2020 2020  de()).          
-00003480: 2020 2020 2020 2020 2020 2320 466c 7573            # Flus
-00003490: 6820 7468 6520 6275 6666 6572 730a 2020  h the buffers.  
-000034a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034b0: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
-000034c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034d0: 2073 656c 662e 732e 666c 7573 6828 290a   self.s.flush().
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034f0: 2020 2020 7365 6c66 2e73 2e66 6c75 7368      self.s.flush
-00003500: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
-00003510: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003520: 2e73 2e66 6c75 7368 4f75 7470 7574 2829  .s.flushOutput()
-00003530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003540: 2020 2020 2073 656c 662e 732e 7772 6974       self.s.writ
-00003550: 6528 222a 4944 4e3f 5c72 5c6e 222e 656e  e("*IDN?\r\n".en
-00003560: 636f 6465 2829 290a 2020 2020 2020 2020  code()).        
+00003330: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00003340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003350: 2020 2020 2020 2020 2073 656c 662e 7320           self.s 
+00003360: 3d20 7365 7269 616c 2e53 6572 6961 6c28  = serial.Serial(
+00003370: 7365 6c66 2e63 6f6d 706f 7274 2c20 7365  self.comport, se
+00003380: 6c66 2e62 6175 6472 6174 652c 2074 696d  lf.baudrate, tim
+00003390: 656f 7574 3d30 2e35 290a 2020 2020 2020  eout=0.5).      
+000033a0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+000033b0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+000033c0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+000033d0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000033e0: 6e74 2866 2763 6f75 6c64 206e 6f74 2063  nt(f'could not c
+000033f0: 6f6e 6e65 6374 207b 7365 6c66 2e63 6f6d  onnect {self.com
+00003400: 706f 7274 7d2c 2074 7279 2061 6e6f 7468  port}, try anoth
+00003410: 6572 2070 6f72 7420 6475 6520 746f 3b20  er port due to; 
+00003420: 7b65 7d27 290a 2020 2020 2020 2020 2020  {e}').          
+00003430: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00003440: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+00003450: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+00003460: 2831 290a 2020 2020 2020 2020 2020 2020  (1).            
+00003470: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
+00003480: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
+00003490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034a0: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
+000034b0: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+000034c0: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
+000034d0: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
+000034e0: 2020 2020 2020 2020 2320 5475 726e 2074          # Turn t
+000034f0: 6865 2063 6f6e 736f 6c65 206f 6666 0a20  he console off. 
+00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003510: 2020 2073 656c 662e 732e 7772 6974 6528     self.s.write(
+00003520: 2243 4f4e 534f 4c45 2044 4953 4142 4c45  "CONSOLE DISABLE
+00003530: 5c72 5c6e 222e 656e 636f 6465 2829 290a  \r\n".encode()).
+00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003550: 2020 2020 2320 466c 7573 6820 7468 6520      # Flush the 
+00003560: 6275 6666 6572 730a 2020 2020 2020 2020  buffers.        
 00003570: 2020 2020 2020 2020 2020 2020 736c 6565              slee
 00003580: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
-00003590: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000035a0: 6c66 2e73 2e69 6e5f 7761 6974 696e 6720  lf.s.in_waiting 
-000035b0: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
-000035c0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-000035d0: 7020 3d20 7365 6c66 2e73 2e72 6561 646c  p = self.s.readl
-000035e0: 696e 6528 292e 6465 636f 6465 2822 7574  ine().decode("ut
-000035f0: 662d 3822 290a 2020 2020 2020 2020 2020  f-8").          
-00003600: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003620: 2020 2020 2020 2020 7265 7370 203d 2027          resp = '
-00003630: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00003640: 2020 2020 2020 7365 6c66 2e6d 6f64 656c        self.model
-00003650: 203d 2072 6573 700a 2020 2020 2020 2020   = resp.        
-00003660: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00003670: 2241 6572 6f66 6c65 7822 2069 6e20 7265  "Aeroflex" in re
-00003680: 7370 293a 0a20 2020 2020 2020 2020 2020  sp):.           
-00003690: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000036a0: 6e74 2827 466f 756e 6420 2720 2b20 7265  nt('Found ' + re
-000036b0: 7370 2e73 7472 6970 2827 5c72 5c6e 2729  sp.strip('\r\n')
-000036c0: 202b 2027 206f 6e20 706f 7274 3a20 2720   + ' on port: ' 
-000036d0: 2b20 706f 7274 290a 2020 2020 2020 2020  + port).        
+00003590: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000035a0: 732e 666c 7573 6828 290a 2020 2020 2020  s.flush().      
+000035b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000035c0: 6c66 2e73 2e66 6c75 7368 496e 7075 7428  lf.s.flushInput(
+000035d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000035e0: 2020 2020 2020 7365 6c66 2e73 2e66 6c75        self.s.flu
+000035f0: 7368 4f75 7470 7574 2829 0a20 2020 2020  shOutput().     
+00003600: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003610: 656c 662e 732e 7772 6974 6528 222a 4944  elf.s.write("*ID
+00003620: 4e3f 5c72 5c6e 222e 656e 636f 6465 2829  N?\r\n".encode()
+00003630: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003640: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
+00003650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003660: 2020 2020 2069 6620 7365 6c66 2e73 2e69       if self.s.i
+00003670: 6e5f 7761 6974 696e 6720 3e20 313a 0a20  n_waiting > 1:. 
+00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003690: 2020 2020 2020 2072 6573 7020 3d20 7365         resp = se
+000036a0: 6c66 2e73 2e72 6561 646c 696e 6528 292e  lf.s.readline().
+000036b0: 6465 636f 6465 2822 7574 662d 3822 290a  decode("utf-8").
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
 000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036f0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-00003700: 2020 2020 2020 2020 2020 656c 6966 2027            elif '
-00003710: 3833 3131 2720 696e 2072 6573 7020 6f72  8311' in resp or
-00003720: 2027 3833 3331 2720 696e 2072 6573 703a   '8331' in resp:
-00003730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003740: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00003750: 466f 756e 6420 2720 2b20 7265 7370 2e73  Found ' + resp.s
-00003760: 7472 6970 2827 5c72 5c6e 2729 202b 2027  trip('\r\n') + '
-00003770: 206f 6e20 706f 7274 3a20 2720 2b20 706f   on port: ' + po
-00003780: 7274 290a 2020 2020 2020 2020 2020 2020  rt).            
-00003790: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000037a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037b0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-000037c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000037d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000037e0: 662e 7320 3d20 7365 7269 616c 2e53 6572  f.s = serial.Ser
-000037f0: 6961 6c28 636f 6d70 6f72 742c 2073 656c  ial(comport, sel
-00003800: 662e 6261 7564 7261 7465 2c20 7469 6d65  f.baudrate, time
-00003810: 6f75 743d 302e 3529 0a20 2020 2020 2020  out=0.5).       
-00003820: 2020 2020 2020 2020 2073 6c65 6570 2831           sleep(1
-00003830: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003840: 2020 7365 6c66 2e73 2e77 7269 7465 2822    self.s.write("
-00003850: 434f 4e53 4f4c 4520 4449 5341 424c 455c  CONSOLE DISABLE\
-00003860: 725c 6e22 2e65 6e63 6f64 6528 2929 0a20  r\n".encode()). 
-00003870: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00003880: 2046 6c75 7368 2074 6865 2062 7566 6665   Flush the buffe
-00003890: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
-000038a0: 2020 2073 656c 662e 732e 666c 7573 6828     self.s.flush(
-000038b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000038c0: 2020 7365 6c66 2e73 2e66 6c75 7368 496e    self.s.flushIn
-000038d0: 7075 7428 290a 2020 2020 2020 2020 2020  put().          
-000038e0: 2020 2020 2020 7365 6c66 2e73 2e66 6c75        self.s.flu
-000038f0: 7368 4f75 7470 7574 2829 0a20 2020 2020  shOutput().     
-00003900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003910: 5175 6572 7928 222a 4944 4e3f 5c72 5c6e  Query("*IDN?\r\n
-00003920: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00003930: 2020 2072 6573 7020 3d20 7365 6c66 2e51     resp = self.Q
-00003940: 7565 7279 2822 2a49 444e 3f5c 725c 6e22  uery("*IDN?\r\n"
-00003950: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003960: 2020 7365 6c66 2e6d 6f64 656c 203d 2072    self.model = r
-00003970: 6573 700a 2020 2020 2020 2020 2020 2020  esp.            
-00003980: 2020 2020 6966 2028 2241 6572 6f66 6c65      if ("Aerofle
-00003990: 7822 2069 6e20 7265 7370 2920 6f72 2028  x" in resp) or (
-000039a0: 2234 3230 3522 2069 6e20 7265 7370 293a  "4205" in resp):
-000039b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000039c0: 2020 2020 2070 7269 6e74 2827 466f 756e       print('Foun
-000039d0: 6420 2720 2b20 7265 7370 2e73 7472 6970  d ' + resp.strip
-000039e0: 2827 5c72 5c6e 2729 202b 2027 206f 6e20  ('\r\n') + ' on 
-000039f0: 706f 7274 3a20 2720 2b20 636f 6d70 6f72  port: ' + compor
-00003a00: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-00003a10: 2020 2065 6c69 6620 2738 3331 3127 2069     elif '8311' i
-00003a20: 6e20 7265 7370 206f 7220 2738 3333 3127  n resp or '8331'
-00003a30: 2069 6e20 7265 7370 3a0a 2020 2020 2020   in resp:.      
-00003a40: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00003a50: 696e 7428 2746 6f75 6e64 2027 202b 2072  int('Found ' + r
-00003a60: 6573 702e 7374 7269 7028 275c 725c 6e27  esp.strip('\r\n'
-00003a70: 2920 2b20 2720 6f6e 2070 6f72 743a 2027  ) + ' on port: '
-00003a80: 202b 2063 6f6d 706f 7274 290a 2020 2020   + comport).    
-00003a90: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00003aa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003ab0: 2020 2020 2020 7365 6c66 2e63 6c6f 7365        self.close
-00003ac0: 5f70 6f72 7428 290a 2020 2020 2020 2020  _port().        
-00003ad0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003ae0: 7428 2741 6572 6f66 6c65 7820 4174 7465  t('Aeroflex Atte
-00003af0: 6e75 6174 6f72 206e 6f74 2066 6f75 6e64  nuator not found
-00003b00: 206f 6e20 7365 6c65 6374 6564 2070 6f72   on selected por
-00003b10: 742c 2063 6865 636b 2063 6f6e 6e65 6374  t, check connect
-00003b20: 696f 6e27 2c20 6669 6c65 3d73 7973 2e73  ion', file=sys.s
-00003b30: 7464 6572 7229 0a0a 2020 2020 2020 2020  tderr)..        
-00003b40: 6465 6620 5772 6974 6528 7365 6c66 2c20  def Write(self, 
-00003b50: 636d 642c 2077 6169 743d 4661 6c73 6529  cmd, wait=False)
-00003b60: 3a0a 2020 2020 2020 2020 2020 2020 2222  :.            ""
-00003b70: 2253 656e 6420 7468 6520 696e 7075 7420  "Send the input 
-00003b80: 636d 6420 7374 7269 6e67 2076 6961 2043  cmd string via C
-00003b90: 4f4d 2053 6f63 6b65 7422 2222 0a20 2020  OM Socket""".   
-00003ba0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00003bb0: 2e73 2e69 734f 7065 6e28 293a 0a20 2020  .s.isOpen():.   
-00003bc0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00003bd0: 730a 2020 2020 2020 2020 2020 2020 656c  s.            el
-00003be0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00003bf0: 2020 2020 7365 6c66 2e73 2e6f 7065 6e28      self.s.open(
-00003c00: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00003c10: 6c66 2e73 2e66 6c75 7368 496e 7075 7428  lf.s.flushInput(
-00003c20: 290a 2020 2020 2020 2020 2020 2020 736c  ).            sl
-00003c30: 6565 7028 3129 0a20 2020 2020 2020 2020  eep(1).         
-00003c40: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00003c50: 2020 2020 2020 2020 7365 6c66 2e73 2e77          self.s.w
-00003c60: 7269 7465 2873 7472 2e65 6e63 6f64 6528  rite(str.encode(
-00003c70: 636d 6429 290a 2020 2020 2020 2020 2020  cmd)).          
-00003c80: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
-00003c90: 2020 2320 436f 6d6d 616e 6473 206d 6179    # Commands may
-00003ca0: 2062 6520 6c6f 7374 2077 6865 6e20 7772   be lost when wr
-00003cb0: 6974 696e 6720 746f 6f20 6661 7374 0a0a  iting too fast..
-00003cc0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00003cd0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-00003ce0: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
-00003cf0: 2020 2020 2023 2073 656c 662e 732e 636c       # self.s.cl
-00003d00: 6f73 6528 290a 0a20 2020 2020 2020 2064  ose()..        d
-00003d10: 6566 2051 7565 7279 2873 656c 662c 2063  ef Query(self, c
-00003d20: 6d64 293a 0a20 2020 2020 2020 2020 2020  md):.           
-00003d30: 2022 2222 5365 6e64 2074 6865 2069 6e70   """Send the inp
-00003d40: 7574 2063 6d64 2073 7472 696e 6720 7669  ut cmd string vi
-00003d50: 6120 434f 4d20 536f 636b 6574 2061 6e64  a COM Socket and
-00003d60: 2072 6574 7572 6e20 7468 6520 7265 706c   return the repl
-00003d70: 7920 7374 7269 6e67 2222 220a 2020 2020  y string""".    
-00003d80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003d90: 732e 6973 4f70 656e 2829 3a0a 2020 2020  s.isOpen():.    
-00003da0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00003db0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00003dc0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00003dd0: 2020 2073 656c 662e 732e 6f70 656e 2829     self.s.open()
-00003de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003df0: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
-00003e00: 2020 2020 2020 2020 2320 7365 6c66 2e73          # self.s
-00003e10: 2e66 6c75 7368 496e 7075 7428 290a 2020  .flushInput().  
-00003e20: 2020 2020 2020 2020 2020 736c 6565 7028            sleep(
-00003e30: 3129 0a20 2020 2020 2020 2020 2020 2074  1).            t
-00003e40: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00003e50: 2020 2020 7365 6c66 2e73 2e77 7269 7465      self.s.write
-00003e60: 2863 6d64 2e65 6e63 6f64 6528 2929 0a20  (cmd.encode()). 
-00003e70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003e80: 6c65 6570 2830 2e31 290a 2020 2020 2020  leep(0.1).      
-00003e90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00003ea0: 662e 732e 696e 5f77 6169 7469 6e67 203e  f.s.in_waiting >
-00003eb0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00003ec0: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
-00003ed0: 656c 662e 732e 7265 6164 6c69 6e65 2829  elf.s.readline()
-00003ee0: 2e64 6563 6f64 6528 2275 7466 2d38 2229  .decode("utf-8")
-00003ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00003f10: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00003f20: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
-00003f30: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00003f40: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-00003f50: 2727 0a20 2020 2020 2020 2020 2020 2023  ''.            #
-00003f60: 2073 656c 662e 732e 636c 6f73 6528 290a   self.s.close().
-00003f70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003f80: 726e 2064 6174 610a 0a20 2020 2020 2020  rn data..       
-00003f90: 2064 6566 2063 6c6f 7365 5f70 6f72 7428   def close_port(
-00003fa0: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
-00003fb0: 2020 2069 6620 7365 6c66 2e73 2069 7320     if self.s is 
-00003fc0: 6e6f 7420 4e6f 6e65 2061 6e64 2073 656c  not None and sel
-00003fd0: 662e 732e 6973 4f70 656e 2829 3a0a 2020  f.s.isOpen():.  
-00003fe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003ff0: 6c66 2e73 2e63 6c6f 7365 2829 0a0a 2020  lf.s.close()..  
-00004000: 2020 2020 2020 6465 6620 6973 5f6f 7065        def is_ope
-00004010: 6e28 7365 6c66 2c20 6368 6563 6b5f 706f  n(self, check_po
-00004020: 7274 3d46 616c 7365 293a 0a20 2020 2020  rt=False):.     
-00004030: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00004040: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00004050: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004060: 2063 6865 636b 5f70 6f72 743a 0a20 2020   check_port:.   
-00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004080: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00004090: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000040a0: 6c66 2e51 7565 7279 2822 2a49 444e 3f5c  lf.Query("*IDN?\
-000040b0: 725c 6e22 290a 2020 2020 2020 2020 2020  r\n").          
-000040c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000040d0: 7370 203d 2073 656c 662e 5175 6572 7928  sp = self.Query(
-000040e0: 222a 4944 4e3f 5c72 5c6e 2229 0a20 2020  "*IDN?\r\n").   
-000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004100: 2020 2020 2073 656c 662e 6d6f 6465 6c20       self.model 
-00004110: 3d20 7265 7370 0a20 2020 2020 2020 2020  = resp.         
-00004120: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004130: 6620 2822 4165 726f 666c 6578 2220 696e  f ("Aeroflex" in
-00004140: 2072 6573 7029 3a0a 2020 2020 2020 2020   resp):.        
+000036f0: 2020 7265 7370 203d 2027 270a 2020 2020    resp = ''.    
+00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003710: 7365 6c66 2e6d 6f64 656c 203d 2072 6573  self.model = res
+00003720: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+00003730: 2020 2020 2020 6966 2028 2241 6572 6f66        if ("Aerof
+00003740: 6c65 7822 2069 6e20 7265 7370 293a 0a20  lex" in resp):. 
+00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003760: 2020 2020 2020 2070 7269 6e74 2827 466f         print('Fo
+00003770: 756e 6420 2720 2b20 7265 7370 2e73 7472  und ' + resp.str
+00003780: 6970 2827 5c72 5c6e 2729 202b 2027 206f  ip('\r\n') + ' o
+00003790: 6e20 706f 7274 3a20 2720 2b20 706f 7274  n port: ' + port
+000037a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000037b0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037d0: 2020 2020 656c 6966 2027 3833 3131 2720      elif '8311' 
+000037e0: 696e 2072 6573 7020 6f72 2027 3833 3331  in resp or '8331
+000037f0: 2720 696e 2072 6573 703a 0a20 2020 2020  ' in resp:.     
+00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003810: 2020 2070 7269 6e74 2827 466f 756e 6420     print('Found 
+00003820: 2720 2b20 7265 7370 2e73 7472 6970 2827  ' + resp.strip('
+00003830: 5c72 5c6e 2729 202b 2027 206f 6e20 706f  \r\n') + ' on po
+00003840: 7274 3a20 2720 2b20 706f 7274 290a 2020  rt: ' + port).  
+00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003860: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003880: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00003890: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000038a0: 2020 2020 2020 2073 656c 662e 7320 3d20         self.s = 
+000038b0: 7365 7269 616c 2e53 6572 6961 6c28 636f  serial.Serial(co
+000038c0: 6d70 6f72 742c 2073 656c 662e 6261 7564  mport, self.baud
+000038d0: 7261 7465 2c20 7469 6d65 6f75 743d 302e  rate, timeout=0.
+000038e0: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
+000038f0: 2020 2073 6c65 6570 2831 290a 2020 2020     sleep(1).    
+00003900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003910: 2e73 2e77 7269 7465 2822 434f 4e53 4f4c  .s.write("CONSOL
+00003920: 4520 4449 5341 424c 455c 725c 6e22 2e65  E DISABLE\r\n".e
+00003930: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
+00003940: 2020 2020 2020 2020 2023 2046 6c75 7368           # Flush
+00003950: 2074 6865 2062 7566 6665 7273 0a20 2020   the buffers.   
+00003960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003970: 662e 732e 666c 7573 6828 290a 2020 2020  f.s.flush().    
+00003980: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003990: 2e73 2e66 6c75 7368 496e 7075 7428 290a  .s.flushInput().
+000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039b0: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
+000039c0: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+000039d0: 2020 2020 2073 656c 662e 5175 6572 7928       self.Query(
+000039e0: 222a 4944 4e3f 5c72 5c6e 2229 0a20 2020  "*IDN?\r\n").   
+000039f0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00003a00: 7020 3d20 7365 6c66 2e51 7565 7279 2822  p = self.Query("
+00003a10: 2a49 444e 3f5c 725c 6e22 290a 2020 2020  *IDN?\r\n").    
+00003a20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003a30: 2e6d 6f64 656c 203d 2072 6573 700a 2020  .model = resp.  
+00003a40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003a50: 2028 2241 6572 6f66 6c65 7822 2069 6e20   ("Aeroflex" in 
+00003a60: 7265 7370 2920 6f72 2028 2234 3230 3522  resp) or ("4205"
+00003a70: 2069 6e20 7265 7370 293a 0a20 2020 2020   in resp):.     
+00003a80: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003a90: 7269 6e74 2827 466f 756e 6420 2720 2b20  rint('Found ' + 
+00003aa0: 7265 7370 2e73 7472 6970 2827 5c72 5c6e  resp.strip('\r\n
+00003ab0: 2729 202b 2027 206f 6e20 706f 7274 3a20  ') + ' on port: 
+00003ac0: 2720 2b20 636f 6d70 6f72 7429 0a20 2020  ' + comport).   
+00003ad0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00003ae0: 6620 2738 3331 3127 2069 6e20 7265 7370  f '8311' in resp
+00003af0: 206f 7220 2738 3333 3127 2069 6e20 7265   or '8331' in re
+00003b00: 7370 3a0a 2020 2020 2020 2020 2020 2020  sp:.            
+00003b10: 2020 2020 2020 2020 7072 696e 7428 2746          print('F
+00003b20: 6f75 6e64 2027 202b 2072 6573 702e 7374  ound ' + resp.st
+00003b30: 7269 7028 275c 725c 6e27 2920 2b20 2720  rip('\r\n') + ' 
+00003b40: 6f6e 2070 6f72 743a 2027 202b 2063 6f6d  on port: ' + com
+00003b50: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
+00003b60: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b80: 7365 6c66 2e63 6c6f 7365 5f70 6f72 7428  self.close_port(
+00003b90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003ba0: 2020 2020 2020 7072 696e 7428 2741 6572        print('Aer
+00003bb0: 6f66 6c65 7820 4174 7465 6e75 6174 6f72  oflex Attenuator
+00003bc0: 206e 6f74 2066 6f75 6e64 206f 6e20 7365   not found on se
+00003bd0: 6c65 6374 6564 2070 6f72 742c 2063 6865  lected port, che
+00003be0: 636b 2063 6f6e 6e65 6374 696f 6e27 2c20  ck connection', 
+00003bf0: 6669 6c65 3d73 7973 2e73 7464 6572 7229  file=sys.stderr)
+00003c00: 0a0a 2020 2020 2020 2020 6465 6620 5772  ..        def Wr
+00003c10: 6974 6528 7365 6c66 2c20 636d 642c 2077  ite(self, cmd, w
+00003c20: 6169 743d 4661 6c73 6529 3a0a 2020 2020  ait=False):.    
+00003c30: 2020 2020 2020 2020 2222 2253 656e 6420          """Send 
+00003c40: 7468 6520 696e 7075 7420 636d 6420 7374  the input cmd st
+00003c50: 7269 6e67 2076 6961 2043 4f4d 2053 6f63  ring via COM Soc
+00003c60: 6b65 7422 2222 0a20 2020 2020 2020 2020  ket""".         
+00003c70: 2020 2069 6620 7365 6c66 2e73 2e69 734f     if self.s.isO
+00003c80: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
+00003c90: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00003ca0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00003cb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003cc0: 6c66 2e73 2e6f 7065 6e28 290a 2020 2020  lf.s.open().    
+00003cd0: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
+00003ce0: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
+00003cf0: 2020 2020 2020 2020 736c 6565 7028 3129          sleep(1)
+00003d00: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00003d10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003d20: 2020 7365 6c66 2e73 2e77 7269 7465 2873    self.s.write(s
+00003d30: 7472 2e65 6e63 6f64 6528 636d 6429 290a  tr.encode(cmd)).
+00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d50: 736c 6565 7028 302e 3129 2020 2320 436f  sleep(0.1)  # Co
+00003d60: 6d6d 616e 6473 206d 6179 2062 6520 6c6f  mmands may be lo
+00003d70: 7374 2077 6865 6e20 7772 6974 696e 6720  st when writing 
+00003d80: 746f 6f20 6661 7374 0a0a 2020 2020 2020  too fast..      
+00003d90: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00003da0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00003db0: 7373 0a20 2020 2020 2020 2020 2020 2023  ss.            #
+00003dc0: 2073 656c 662e 732e 636c 6f73 6528 290a   self.s.close().
+00003dd0: 0a20 2020 2020 2020 2064 6566 2051 7565  .        def Que
+00003de0: 7279 2873 656c 662c 2063 6d64 293a 0a20  ry(self, cmd):. 
+00003df0: 2020 2020 2020 2020 2020 2022 2222 5365             """Se
+00003e00: 6e64 2074 6865 2069 6e70 7574 2063 6d64  nd the input cmd
+00003e10: 2073 7472 696e 6720 7669 6120 434f 4d20   string via COM 
+00003e20: 536f 636b 6574 2061 6e64 2072 6574 7572  Socket and retur
+00003e30: 6e20 7468 6520 7265 706c 7920 7374 7269  n the reply stri
+00003e40: 6e67 2222 220a 2020 2020 2020 2020 2020  ng""".          
+00003e50: 2020 6966 2073 656c 662e 732e 6973 4f70    if self.s.isOp
+00003e60: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
+00003e70: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00003e80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00003e90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003ea0: 662e 732e 6f70 656e 2829 0a20 2020 2020  f.s.open().     
+00003eb0: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+00003ec0: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
+00003ed0: 2020 2320 7365 6c66 2e73 2e66 6c75 7368    # self.s.flush
+00003ee0: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
+00003ef0: 2020 2020 736c 6565 7028 3129 0a20 2020      sleep(1).   
+00003f00: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00003f10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003f20: 6c66 2e73 2e77 7269 7465 2863 6d64 2e65  lf.s.write(cmd.e
+00003f30: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
+00003f40: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
+00003f50: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
+00003f60: 2020 2020 6966 2073 656c 662e 732e 696e      if self.s.in
+00003f70: 5f77 6169 7469 6e67 203e 2030 3a0a 2020  _waiting > 0:.  
+00003f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f90: 2020 6461 7461 203d 2073 656c 662e 732e    data = self.s.
+00003fa0: 7265 6164 6c69 6e65 2829 2e64 6563 6f64  readline().decod
+00003fb0: 6528 2275 7466 2d38 2229 0a20 2020 2020  e("utf-8").     
+00003fc0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003fe0: 2020 2020 2064 6174 6120 3d20 2727 0a20       data = ''. 
+00003ff0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00004000: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00004010: 2020 2064 6174 6120 3d20 2727 0a20 2020     data = ''.   
+00004020: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00004030: 732e 636c 6f73 6528 290a 2020 2020 2020  s.close().      
+00004040: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
+00004050: 610a 0a20 2020 2020 2020 2064 6566 2063  a..        def c
+00004060: 6c6f 7365 5f70 6f72 7428 7365 6c66 293a  lose_port(self):
+00004070: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004080: 7365 6c66 2e73 2069 7320 6e6f 7420 4e6f  self.s is not No
+00004090: 6e65 2061 6e64 2073 656c 662e 732e 6973  ne and self.s.is
+000040a0: 4f70 656e 2829 3a0a 2020 2020 2020 2020  Open():.        
+000040b0: 2020 2020 2020 2020 7365 6c66 2e73 2e63          self.s.c
+000040c0: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
+000040d0: 6465 6620 6973 5f6f 7065 6e28 7365 6c66  def is_open(self
+000040e0: 2c20 6368 6563 6b5f 706f 7274 3d46 616c  , check_port=Fal
+000040f0: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
+00004100: 2069 6620 7365 6c66 2e73 2069 7320 6e6f   if self.s is no
+00004110: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00004120: 2020 2020 2020 2020 6966 2063 6865 636b          if check
+00004130: 5f70 6f72 743a 0a20 2020 2020 2020 2020  _port:.         
+00004140: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
 00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004160: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004180: 2020 2020 2020 2020 656c 6966 2027 3833          elif '83
-00004190: 3131 2720 696e 2072 6573 7020 6f72 2027  11' in resp or '
-000041a0: 3833 3331 2720 696e 2072 6573 703a 0a20  8331' in resp:. 
-000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000041d0: 6e20 5472 7565 0a20 2020 2020 2020 2020  n True.         
-000041e0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-000041f0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00004200: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004210: 636c 6f73 655f 706f 7274 2829 0a20 2020  close_port().   
-00004220: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00004230: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00004240: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00004250: 6c66 2e73 2e69 734f 7065 6e28 290a 2020  lf.s.isOpen().  
-00004260: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00004270: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
-00004280: 6465 6620 5365 7461 7474 6e28 7365 6c66  def Setattn(self
-00004290: 2c20 6174 746e 293a 0a20 2020 2020 2020  , attn):.       
-000042a0: 2020 2020 2063 6d64 203d 2022 4154 544e       cmd = "ATTN
-000042b0: 207b 3a2e 3266 7d5c 725c 6e22 2e66 6f72   {:.2f}\r\n".for
-000042c0: 6d61 7428 6174 746e 290a 2020 2020 2020  mat(attn).      
-000042d0: 2020 2020 2020 7365 6c66 2e57 7269 7465        self.Write
-000042e0: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
-000042f0: 2020 7661 6c75 6520 3d20 7365 6c66 2e47    value = self.G
-00004300: 6574 6174 746e 2829 0a20 2020 2020 2020  etattn().       
-00004310: 2020 2020 2076 616c 7565 203d 2066 6c6f       value = flo
-00004320: 6174 2876 616c 7565 290a 2020 2020 2020  at(value).      
-00004330: 2020 2020 2020 6966 2076 616c 7565 2021        if value !
-00004340: 3d20 6174 746e 3a0a 2020 2020 2020 2020  = attn:.        
-00004350: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00004360: 4572 726f 7220 7365 7474 696e 6720 6174  Error setting at
-00004370: 7465 6e75 6174 696f 6e3a 206e 6577 203a  tenuation: new :
-00004380: 207b 6174 746e 7d20 6375 7272 656e 743a   {attn} current:
-00004390: 207b 7661 6c75 657d 2729 0a20 2020 2020   {value}').     
-000043a0: 2020 2020 2020 2072 6574 7572 6e20 7661         return va
-000043b0: 6c75 650a 0a20 2020 2020 2020 2064 6566  lue..        def
-000043c0: 2047 6574 6174 746e 2873 656c 6629 3a0a   Getattn(self):.
-000043d0: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
-000043e0: 3d20 2241 5454 4e3f 5c72 5c6e 220a 2020  = "ATTN?\r\n".  
-000043f0: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
-00004400: 3d20 7365 6c66 2e51 7565 7279 2863 6d64  = self.Query(cmd
-00004410: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00004420: 7475 726e 2076 616c 7565 0a0a 0a63 6c61  turn value...cla
-00004430: 7373 2054 6573 636f 6d3a 0a20 2020 2022  ss Tescom:.    "
-00004440: 2222 0a20 2020 2043 6f6e 7472 6f6c 2054  "".    Control T
-00004450: 4553 434f 4d20 7465 7374 696e 6720 6368  ESCOM testing ch
-00004460: 616d 6265 7273 0a20 2020 2022 2222 0a20  ambers.    """. 
-00004470: 2020 206f 7065 6e5f 636d 6420 3d20 6227     open_cmd = b'
-00004480: 4f50 454e 5c72 270a 2020 2020 636c 6f73  OPEN\r'.    clos
-00004490: 655f 636d 6420 3d20 6227 434c 4f53 455c  e_cmd = b'CLOSE\
-000044a0: 7227 0a20 2020 2063 6f6d 5f70 6f72 745f  r'.    com_port_
-000044b0: 6f62 6a20 3d20 4e6f 6e65 0a20 2020 206d  obj = None.    m
-000044c0: 6f64 656c 735f 6c69 7374 203d 205b 2754  odels_list = ['T
-000044d0: 432d 3530 3634 4327 2c20 2754 412d 3730  C-5064C', 'TA-70
-000044e0: 3131 4150 272c 2027 5443 2d35 3036 3341  11AP', 'TC-5063A
-000044f0: 272c 2027 5443 2d35 3937 3043 5027 5d0a  ', 'TC-5970CP'].
-00004500: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00004510: 5f28 7365 6c66 2c20 706f 7274 3d4e 6f6e  _(self, port=Non
-00004520: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00004530: 2e70 6f72 7420 3d20 706f 7274 0a20 2020  .port = port.   
-00004540: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00004550: 2020 2020 2020 6966 2070 6f72 7420 6973        if port is
-00004560: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00004570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004580: 636f 6e6e 6563 7428 706f 7274 290a 0a20  connect(port).. 
-00004590: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-000045a0: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
-000045b0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000045c0: 6529 0a20 2020 2020 2020 2020 2020 2070  e).            p
-000045d0: 7269 6e74 2822 5465 7363 6f6d 202d 2043  rint("Tescom - C
-000045e0: 6f6e 6e65 6374 696f 6e20 6661 696c 6564  onnection failed
-000045f0: 2229 0a0a 2020 2020 6465 6620 636f 6e6e  ")..    def conn
-00004600: 6563 7428 7365 6c66 2c20 706f 7274 293a  ect(self, port):
-00004610: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004620: 2020 2020 203a 7061 7261 6d20 706f 7274       :param port
-00004630: 3a20 636f 6d20 706f 7274 2074 6f20 636f  : com port to co
-00004640: 6e6e 6563 740a 2020 2020 2020 2020 3a72  nnect.        :r
-00004650: 6574 7572 6e3a 2063 6f6d 2070 6f72 7420  eturn: com port 
-00004660: 6f62 6a0a 2020 2020 2020 2020 2222 220a  obj.        """.
-00004670: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00004680: 2020 2020 2020 2020 2063 6f6d 5f70 6f72           com_por
-00004690: 745f 6f62 6a20 3d20 7365 6c66 2e63 6f6d  t_obj = self.com
-000046a0: 5f70 6f72 745f 6f62 6a20 3d20 7365 7269  _port_obj = seri
-000046b0: 616c 2e53 6572 6961 6c28 706f 7274 3d70  al.Serial(port=p
-000046c0: 6f72 742c 2062 6175 6472 6174 653d 3936  ort, baudrate=96
-000046d0: 3030 2c20 7469 6d65 6f75 743d 3129 0a20  00, timeout=1). 
-000046e0: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-000046f0: 6d5f 706f 7274 5f6f 626a 2069 7320 6e6f  m_port_obj is no
-00004700: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00004710: 2020 2020 2020 2020 7365 6c66 2e64 6f6f          self.doo
-00004720: 725f 636d 6420 3d20 4e6f 6e65 0a20 2020  r_cmd = None.   
-00004730: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00004740: 662e 636f 6d5f 706f 7274 5f6f 626a 2e77  f.com_port_obj.w
-00004750: 7269 7465 2862 274d 4f44 454c 3f5c 7227  rite(b'MODEL?\r'
-00004760: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004770: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
-00004780: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00004790: 656c 203d 2073 7472 2873 656c 662e 636f  el = str(self.co
-000047a0: 6d5f 706f 7274 5f6f 626a 2e72 6561 6428  m_port_obj.read(
-000047b0: 3134 2929 0a20 2020 2020 2020 2020 2020  14)).           
-000047c0: 2020 2020 2070 6172 7473 203d 205b 7020       parts = [p 
-000047d0: 666f 7220 7020 696e 206d 6f64 656c 2e73  for p in model.s
-000047e0: 706c 6974 2822 2722 295d 0a20 2020 2020  plit("'")].     
-000047f0: 2020 2020 2020 2020 2020 2070 6172 7473             parts
-00004800: 203d 205b 7020 666f 7220 7020 696e 2070   = [p for p in p
-00004810: 6172 7473 5b31 5d2e 7370 6c69 7428 2220  arts[1].split(" 
-00004820: 2229 5d0a 2020 2020 2020 2020 2020 2020  ")].            
-00004830: 2020 2020 7365 6c66 2e6d 6f64 656c 203d      self.model =
-00004840: 2070 6172 7473 5b30 5d0a 2020 2020 2020   parts[0].      
-00004850: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00004860: 2873 656c 662e 6d6f 6465 6c29 203e 2030  (self.model) > 0
-00004870: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004880: 2020 2020 2020 7072 696e 7428 2252 4620        print("RF 
-00004890: 6368 616d 6265 7220 636f 6e6e 6563 7465  chamber connecte
-000048a0: 6420 746f 2070 6f72 7420 2220 2b20 7374  d to port " + st
-000048b0: 7228 706f 7274 2929 0a20 2020 2020 2020  r(port)).       
-000048c0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000048d0: 6e74 2822 5465 7363 6f6d 202d 2043 6861  nt("Tescom - Cha
-000048e0: 6d62 6572 206d 6f64 656c 3a22 2c20 7365  mber model:", se
-000048f0: 6c66 2e6d 6f64 656c 290a 2020 2020 2020  lf.model).      
-00004900: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 7072 696e 7428 2254 6573 636f      print("Tesco
-00004930: 6d20 2d20 4572 726f 7221 204e 6f20 6368  m - Error! No ch
-00004940: 616d 6265 7220 666f 756e 6422 290a 2020  amber found").  
-00004950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004960: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00004970: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00004980: 2e6d 6f64 656c 2069 6e20 7365 6c66 2e6d  .model in self.m
-00004990: 6f64 656c 735f 6c69 7374 3a0a 2020 2020  odels_list:.    
-000049a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049b0: 7365 6c66 2e64 6f6f 725f 636d 6420 3d20  self.door_cmd = 
-000049c0: 6227 444f 4f52 3f5c 7227 0a20 2020 2020  b'DOOR?\r'.     
-000049d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000049e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000049f0: 2020 2020 2073 656c 662e 646f 6f72 5f63       self.door_c
-00004a00: 6d64 203d 2062 274c 4944 3f5c 7227 0a20  md = b'LID?\r'. 
-00004a10: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00004160: 2020 2020 2020 2020 7365 6c66 2e51 7565          self.Que
+00004170: 7279 2822 2a49 444e 3f5c 725c 6e22 290a  ry("*IDN?\r\n").
+00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004190: 2020 2020 2020 2020 7265 7370 203d 2073          resp = s
+000041a0: 656c 662e 5175 6572 7928 222a 4944 4e3f  elf.Query("*IDN?
+000041b0: 5c72 5c6e 2229 0a20 2020 2020 2020 2020  \r\n").         
+000041c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000041d0: 656c 662e 6d6f 6465 6c20 3d20 7265 7370  elf.model = resp
+000041e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041f0: 2020 2020 2020 2020 2069 6620 2822 4165           if ("Ae
+00004200: 726f 666c 6578 2220 696e 2072 6573 7029  roflex" in resp)
+00004210: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004220: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00004230: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+00004240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004250: 2020 656c 6966 2027 3833 3131 2720 696e    elif '8311' in
+00004260: 2072 6573 7020 6f72 2027 3833 3331 2720   resp or '8331' 
+00004270: 696e 2072 6573 703a 0a20 2020 2020 2020  in resp:.       
+00004280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004290: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+000042a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000042b0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042d0: 2020 2020 2073 656c 662e 636c 6f73 655f       self.close_
+000042e0: 706f 7274 2829 0a20 2020 2020 2020 2020  port().         
+000042f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00004300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004310: 2072 6574 7572 6e20 7365 6c66 2e73 2e69   return self.s.i
+00004320: 734f 7065 6e28 290a 2020 2020 2020 2020  sOpen().        
+00004330: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00004340: 0a0a 2020 2020 2020 2020 6465 6620 5365  ..        def Se
+00004350: 7461 7474 6e28 7365 6c66 2c20 6174 746e  tattn(self, attn
+00004360: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00004370: 6d64 203d 2022 4154 544e 207b 3a2e 3266  md = "ATTN {:.2f
+00004380: 7d5c 725c 6e22 2e66 6f72 6d61 7428 6174  }\r\n".format(at
+00004390: 746e 290a 2020 2020 2020 2020 2020 2020  tn).            
+000043a0: 7365 6c66 2e57 7269 7465 2863 6d64 290a  self.Write(cmd).
+000043b0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+000043c0: 6520 3d20 7365 6c66 2e47 6574 6174 746e  e = self.Getattn
+000043d0: 2829 0a20 2020 2020 2020 2020 2020 2076  ().            v
+000043e0: 616c 7565 203d 2066 6c6f 6174 2876 616c  alue = float(val
+000043f0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00004400: 6966 2076 616c 7565 2021 3d20 6174 746e  if value != attn
+00004410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004420: 2020 7072 696e 7428 6627 4572 726f 7220    print(f'Error 
+00004430: 7365 7474 696e 6720 6174 7465 6e75 6174  setting attenuat
+00004440: 696f 6e3a 206e 6577 203a 207b 6174 746e  ion: new : {attn
+00004450: 7d20 6375 7272 656e 743a 207b 7661 6c75  } current: {valu
+00004460: 657d 2729 0a20 2020 2020 2020 2020 2020  e}').           
+00004470: 2072 6574 7572 6e20 7661 6c75 650a 0a20   return value.. 
+00004480: 2020 2020 2020 2064 6566 2047 6574 6174         def Getat
+00004490: 746e 2873 656c 6629 3a0a 2020 2020 2020  tn(self):.      
+000044a0: 2020 2020 2020 636d 6420 3d20 2241 5454        cmd = "ATT
+000044b0: 4e3f 5c72 5c6e 220a 2020 2020 2020 2020  N?\r\n".        
+000044c0: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
+000044d0: 2e51 7565 7279 2863 6d64 290a 2020 2020  .Query(cmd).    
+000044e0: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+000044f0: 616c 7565 0a0a 0a63 6c61 7373 2054 6573  alue...class Tes
+00004500: 636f 6d3a 0a20 2020 2022 2222 0a20 2020  com:.    """.   
+00004510: 2043 6f6e 7472 6f6c 2054 4553 434f 4d20   Control TESCOM 
+00004520: 7465 7374 696e 6720 6368 616d 6265 7273  testing chambers
+00004530: 0a20 2020 2022 2222 0a20 2020 206f 7065  .    """.    ope
+00004540: 6e5f 636d 6420 3d20 6227 4f50 454e 5c72  n_cmd = b'OPEN\r
+00004550: 270a 2020 2020 636c 6f73 655f 636d 6420  '.    close_cmd 
+00004560: 3d20 6227 434c 4f53 455c 7227 0a20 2020  = b'CLOSE\r'.   
+00004570: 2063 6f6d 5f70 6f72 745f 6f62 6a20 3d20   com_port_obj = 
+00004580: 4e6f 6e65 0a20 2020 206d 6f64 656c 735f  None.    models_
+00004590: 6c69 7374 203d 205b 2754 432d 3530 3634  list = ['TC-5064
+000045a0: 4327 2c20 2754 412d 3730 3131 4150 272c  C', 'TA-7011AP',
+000045b0: 2027 5443 2d35 3036 3341 272c 2027 5443   'TC-5063A', 'TC
+000045c0: 2d35 3937 3043 5027 5d0a 0a20 2020 2064  -5970CP']..    d
+000045d0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000045e0: 2c20 706f 7274 3d4e 6f6e 6529 3a0a 2020  , port=None):.  
+000045f0: 2020 2020 2020 7365 6c66 2e70 6f72 7420        self.port 
+00004600: 3d20 706f 7274 0a20 2020 2020 2020 2074  = port.        t
+00004610: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00004620: 6966 2070 6f72 7420 6973 206e 6f74 204e  if port is not N
+00004630: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00004640: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
+00004650: 7428 706f 7274 290a 0a20 2020 2020 2020  t(port)..       
+00004660: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00004670: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+00004680: 2020 2020 7072 696e 7428 6529 0a20 2020      print(e).   
+00004690: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+000046a0: 5465 7363 6f6d 202d 2043 6f6e 6e65 6374  Tescom - Connect
+000046b0: 696f 6e20 6661 696c 6564 2229 0a0a 2020  ion failed")..  
+000046c0: 2020 6465 6620 636f 6e6e 6563 7428 7365    def connect(se
+000046d0: 6c66 2c20 706f 7274 293a 0a20 2020 2020  lf, port):.     
+000046e0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+000046f0: 7061 7261 6d20 706f 7274 3a20 636f 6d20  param port: com 
+00004700: 706f 7274 2074 6f20 636f 6e6e 6563 740a  port to connect.
+00004710: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00004720: 2063 6f6d 2070 6f72 7420 6f62 6a0a 2020   com port obj.  
+00004730: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00004740: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00004750: 2020 2063 6f6d 5f70 6f72 745f 6f62 6a20     com_port_obj 
+00004760: 3d20 7365 6c66 2e63 6f6d 5f70 6f72 745f  = self.com_port_
+00004770: 6f62 6a20 3d20 7365 7269 616c 2e53 6572  obj = serial.Ser
+00004780: 6961 6c28 706f 7274 3d70 6f72 742c 2062  ial(port=port, b
+00004790: 6175 6472 6174 653d 3936 3030 2c20 7469  audrate=9600, ti
+000047a0: 6d65 6f75 743d 3129 0a20 2020 2020 2020  meout=1).       
+000047b0: 2020 2020 2069 6620 636f 6d5f 706f 7274       if com_port
+000047c0: 5f6f 626a 2069 7320 6e6f 7420 4e6f 6e65  _obj is not None
+000047d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000047e0: 2020 7365 6c66 2e64 6f6f 725f 636d 6420    self.door_cmd 
+000047f0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00004800: 2020 2020 2020 2073 656c 662e 636f 6d5f         self.com_
+00004810: 706f 7274 5f6f 626a 2e77 7269 7465 2862  port_obj.write(b
+00004820: 274d 4f44 454c 3f5c 7227 290a 2020 2020  'MODEL?\r').    
+00004830: 2020 2020 2020 2020 2020 2020 736c 6565              slee
+00004840: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
+00004850: 2020 2020 2020 206d 6f64 656c 203d 2073         model = s
+00004860: 7472 2873 656c 662e 636f 6d5f 706f 7274  tr(self.com_port
+00004870: 5f6f 626a 2e72 6561 6428 3134 2929 0a20  _obj.read(14)). 
+00004880: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00004890: 6172 7473 203d 205b 7020 666f 7220 7020  arts = [p for p 
+000048a0: 696e 206d 6f64 656c 2e73 706c 6974 2822  in model.split("
+000048b0: 2722 295d 0a20 2020 2020 2020 2020 2020  '")].           
+000048c0: 2020 2020 2070 6172 7473 203d 205b 7020       parts = [p 
+000048d0: 666f 7220 7020 696e 2070 6172 7473 5b31  for p in parts[1
+000048e0: 5d2e 7370 6c69 7428 2220 2229 5d0a 2020  ].split(" ")].  
+000048f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004900: 6c66 2e6d 6f64 656c 203d 2070 6172 7473  lf.model = parts
+00004910: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00004920: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+00004930: 6d6f 6465 6c29 203e 2030 3a0a 2020 2020  model) > 0:.    
+00004940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004950: 7072 696e 7428 2252 4620 6368 616d 6265  print("RF chambe
+00004960: 7220 636f 6e6e 6563 7465 6420 746f 2070  r connected to p
+00004970: 6f72 7420 2220 2b20 7374 7228 706f 7274  ort " + str(port
+00004980: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00004990: 2020 2020 2020 2070 7269 6e74 2822 5465         print("Te
+000049a0: 7363 6f6d 202d 2043 6861 6d62 6572 206d  scom - Chamber m
+000049b0: 6f64 656c 3a22 2c20 7365 6c66 2e6d 6f64  odel:", self.mod
+000049c0: 656c 290a 2020 2020 2020 2020 2020 2020  el).            
+000049d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000049e0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000049f0: 696e 7428 2254 6573 636f 6d20 2d20 4572  int("Tescom - Er
+00004a00: 726f 7221 2043 6861 6d62 6572 2069 7320  ror! Chamber is 
+00004a10: 6e6f 7420 7265 7370 6f6e 6469 6e67 2229  not responding")
 00004a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004a30: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-00004a40: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00004a50: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
-00004a60: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
-00004a70: 696e 7428 6529 0a20 2020 2020 2020 2020  int(e).         
-00004a80: 2020 2070 7269 6e74 2866 2254 6573 636f     print(f"Tesco
-00004a90: 6d20 2d20 436f 756c 6420 6e6f 7420 636f  m - Could not co
-00004aa0: 6e6e 6563 7420 746f 2070 6f72 7420 7b70  nnect to port {p
-00004ab0: 6f72 747d 2064 7565 2074 6f20 7b65 7d22  ort} due to {e}"
-00004ac0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00004ad0: 7475 726e 204e 6f6e 650a 0a20 2020 2064  turn None..    d
-00004ae0: 6566 2063 6c6f 7365 5f70 6f72 7428 7365  ef close_port(se
-00004af0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00004b00: 0a20 2020 2020 2020 2063 6c6f 7365 7320  .        closes 
-00004b10: 636f 6d20 706f 7274 0a20 2020 2020 2020  com port.       
-00004b20: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
-00004b30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00004b40: 6c66 2e63 6f6d 5f70 6f72 745f 6f62 6a2e  lf.com_port_obj.
-00004b50: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
-00004b60: 2020 2020 7072 696e 7428 2252 4620 6368      print("RF ch
-00004b70: 616d 6265 7220 6469 7363 6f6e 6e65 6374  amber disconnect
-00004b80: 6564 2066 726f 6d20 706f 7274 3a20 2220  ed from port: " 
-00004b90: 2b20 7374 7228 7365 6c66 2e70 6f72 7429  + str(self.port)
-00004ba0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00004bb0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00004bc0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00004bd0: 6e74 2822 436f 756c 6420 6e6f 7420 6469  nt("Could not di
-00004be0: 7363 6f6e 6e65 6374 2229 0a0a 2020 2020  sconnect")..    
-00004bf0: 6465 6620 6f70 656e 5f63 6861 6d62 6572  def open_chamber
-00004c00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00004c10: 2222 220a 2020 2020 2020 2020 6f70 656e  """.        open
-00004c20: 7320 6368 616d 6265 720a 2020 2020 2020  s chamber.      
-00004c30: 2020 3a72 6574 7572 6e3a 2022 4f4b 2220    :return: "OK" 
-00004c40: 6966 2063 6f6d 6d61 6e64 2077 6173 2073  if command was s
-00004c50: 7563 6365 7373 6675 6c0a 2020 2020 2020  uccessful.      
-00004c60: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00004c70: 2073 656c 662e 6973 5f64 6f6f 725f 6f70   self.is_door_op
-00004c80: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
-00004c90: 2020 7072 696e 7428 2243 6861 6d62 6572    print("Chamber
-00004ca0: 2069 7320 6f70 656e 2229 0a20 2020 2020   is open").     
-00004cb0: 2020 2020 2020 2072 6574 7572 6e20 274f         return 'O
-00004cc0: 4b27 0a20 2020 2020 2020 2074 7279 3a0a  K'.        try:.
-00004cd0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00004ce0: 7428 6622 4368 616d 6265 7220 7b73 656c  t(f"Chamber {sel
-00004cf0: 662e 706f 7274 7d20 6973 206f 7065 6e69  f.port} is openi
-00004d00: 6e67 2229 0a20 2020 2020 2020 2020 2020  ng").           
-00004d10: 2073 656c 662e 636f 6d5f 706f 7274 5f6f   self.com_port_o
-00004d20: 626a 2e72 6573 6574 5f69 6e70 7574 5f62  bj.reset_input_b
-00004d30: 7566 6665 7228 290a 2020 2020 2020 2020  uffer().        
-00004d40: 2020 2020 7365 6c66 2e63 6f6d 5f70 6f72      self.com_por
-00004d50: 745f 6f62 6a2e 7265 7365 745f 6f75 7470  t_obj.reset_outp
-00004d60: 7574 5f62 7566 6665 7228 290a 2020 2020  ut_buffer().    
-00004d70: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
-00004d80: 5f70 6f72 745f 6f62 6a2e 7772 6974 6528  _port_obj.write(
-00004d90: 7365 6c66 2e6f 7065 6e5f 636d 6429 0a20  self.open_cmd). 
-00004da0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00004db0: 2027 270a 2020 2020 2020 2020 2020 2020   ''.            
-00004dc0: 7761 6974 5f63 6f75 6e74 6572 203d 2030  wait_counter = 0
-00004dd0: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
-00004de0: 6c65 2027 4f4b 2720 6e6f 7420 696e 2072  le 'OK' not in r
-00004df0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00004e00: 2020 2020 6966 2077 6169 745f 636f 756e      if wait_coun
-00004e10: 7465 7220 3e3d 2031 353a 0a20 2020 2020  ter >= 15:.     
-00004e20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004e30: 6169 7365 2045 7863 6570 7469 6f6e 2866  aise Exception(f
-00004e40: 2245 7272 6f72 2069 6e20 6f70 656e 696e  "Error in openin
-00004e50: 6720 6368 616d 6265 7220 7b73 656c 662e  g chamber {self.
-00004e60: 706f 7274 7d22 290a 2020 2020 2020 2020  port}").        
-00004e70: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-00004e80: 6c66 2e63 6f6d 5f70 6f72 745f 6f62 6a2e  lf.com_port_obj.
-00004e90: 7265 6164 2831 3429 2e64 6563 6f64 6528  read(14).decode(
-00004ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004eb0: 2020 2020 2027 7574 662d 3827 292e 7570       'utf-8').up
-00004ec0: 7065 7228 292e 7273 7472 6970 2827 5c72  per().rstrip('\r
-00004ed0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00004ee0: 2020 2069 6620 6c65 6e28 7374 7228 7265     if len(str(re
-00004ef0: 7329 2920 3e20 303a 0a20 2020 2020 2020  s)) > 0:.       
-00004f00: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00004f10: 6e74 2866 2743 6861 6d62 6572 207b 7365  nt(f'Chamber {se
-00004f20: 6c66 2e70 6f72 747d 2073 7461 7475 733a  lf.port} status:
-00004f30: 2027 202b 2073 7472 2872 6573 2929 0a20   ' + str(res)). 
-00004f40: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00004f50: 6169 745f 636f 756e 7465 7220 2b3d 2031  ait_counter += 1
-00004f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004f70: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
-00004f80: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00004f90: 656c 662e 6973 5f64 6f6f 725f 6f70 656e  elf.is_door_open
-00004fa0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00004fb0: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
-00004fc0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00004fd0: 2020 2020 2020 2020 2066 227b 7365 6c66           f"{self
-00004fe0: 2e70 6f72 747d 2044 6f6f 7220 7374 6174  .port} Door stat
-00004ff0: 7573 2064 6f65 736e 2774 206d 6174 6368  us doesn't match
-00005000: 2063 6f6d 6d61 6e64 2073 656e 7421 2229   command sent!")
-00005010: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00005020: 6e74 2866 2243 6861 6d62 6572 207b 7365  nt(f"Chamber {se
-00005030: 6c66 2e70 6f72 747d 2069 7320 6f70 656e  lf.port} is open
-00005040: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-00005050: 6574 7572 6e20 274f 4b27 0a20 2020 2020  eturn 'OK'.     
-00005060: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00005070: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
-00005080: 2020 2020 2020 7072 696e 7428 6529 0a20        print(e). 
-00005090: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000050a0: 6e20 2246 4149 4c22 0a0a 2020 2020 6465  n "FAIL"..    de
-000050b0: 6620 636c 6f73 655f 6368 616d 6265 7228  f close_chamber(
-000050c0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000050d0: 2222 0a20 2020 2020 2020 2063 6c6f 7365  "".        close
-000050e0: 7320 6368 616d 6265 720a 2020 2020 2020  s chamber.      
-000050f0: 2020 3a72 6574 7572 6e3a 2022 4f4b 2220    :return: "OK" 
-00005100: 6966 2063 6f6d 6d61 6e64 2077 6173 2073  if command was s
-00005110: 7563 6365 7373 6675 6c0a 2020 2020 2020  uccessful.      
-00005120: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00005130: 2073 656c 662e 6973 5f64 6f6f 725f 636c   self.is_door_cl
-00005140: 6f73 6564 2829 3a0a 2020 2020 2020 2020  osed():.        
-00005150: 2020 2020 7072 696e 7428 2243 6861 6d62      print("Chamb
-00005160: 6572 2063 6c6f 7365 6422 290a 2020 2020  er closed").    
-00005170: 2020 2020 2020 2020 7265 7475 726e 2027          return '
-00005180: 4f4b 270a 2020 2020 2020 2020 7472 793a  OK'.        try:
-00005190: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-000051a0: 6e74 2866 2243 4841 4d42 4552 207b 7365  nt(f"CHAMBER {se
-000051b0: 6c66 2e70 6f72 747d 2049 5320 434c 4f53  lf.port} IS CLOS
-000051c0: 494e 472c 2043 4c45 4152 2048 414e 4453  ING, CLEAR HANDS
-000051d0: 2121 2122 290a 2020 2020 2020 2020 2020  !!!").          
-000051e0: 2020 736c 6565 7028 3229 0a20 2020 2020    sleep(2).     
-000051f0: 2020 2020 2020 2073 656c 662e 636f 6d5f         self.com_
-00005200: 706f 7274 5f6f 626a 2e77 7269 7465 2873  port_obj.write(s
-00005210: 656c 662e 636c 6f73 655f 636d 6429 0a20  elf.close_cmd). 
-00005220: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00005230: 2027 270a 2020 2020 2020 2020 2020 2020   ''.            
-00005240: 7761 6974 5f63 6f75 6e74 6572 203d 2030  wait_counter = 0
-00005250: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
-00005260: 6c65 2027 5245 4144 5927 206e 6f74 2069  le 'READY' not i
-00005270: 6e20 7265 733a 0a20 2020 2020 2020 2020  n res:.         
-00005280: 2020 2020 2020 2069 6620 7761 6974 5f63         if wait_c
-00005290: 6f75 6e74 6572 203e 3d20 353a 0a20 2020  ounter >= 5:.   
-000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052b0: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-000052c0: 2866 2263 6861 6d62 6572 207b 7365 6c66  (f"chamber {self
-000052d0: 2e70 6f72 747d 2073 7461 7475 7320 6973  .port} status is
-000052e0: 204e 4f54 2072 6561 6479 2229 0a20 2020   NOT ready").   
-000052f0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00005300: 203d 2073 656c 662e 636f 6d5f 706f 7274   = self.com_port
-00005310: 5f6f 626a 2e72 6561 6428 3134 292e 6465  _obj.read(14).de
-00005320: 636f 6465 280a 2020 2020 2020 2020 2020  code(.          
-00005330: 2020 2020 2020 2020 2020 2775 7466 2d38            'utf-8
-00005340: 2729 2e75 7070 6572 2829 2e72 7374 7269  ').upper().rstri
-00005350: 7028 275c 7227 290a 2020 2020 2020 2020  p('\r').        
-00005360: 2020 2020 2020 2020 6966 2027 4552 5227          if 'ERR'
-00005370: 2069 6e20 7265 7320 6f72 2027 5245 4144   in res or 'READ
-00005380: 5927 2069 6e20 7265 7320 6f72 2027 4f4b  Y' in res or 'OK
-00005390: 2720 696e 2072 6573 3a0a 2020 2020 2020  ' in res:.      
-000053a0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000053b0: 696e 7428 6627 4368 616d 6265 7220 7b73  int(f'Chamber {s
-000053c0: 656c 662e 706f 7274 7d20 7374 6174 7573  elf.port} status
-000053d0: 3a20 2720 2b20 7374 7228 7265 7329 290a  : ' + str(res)).
-000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00005400: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00005410: 6627 4368 616d 6265 7220 7b73 656c 662e  f'Chamber {self.
-00005420: 706f 7274 7d20 6469 6420 6e6f 7420 616e  port} did not an
-00005430: 7377 6572 6564 3a20 7b72 6573 7d27 202b  swered: {res}' +
-00005440: 2073 7472 2872 6573 2929 0a20 2020 2020   str(res)).     
-00005450: 2020 2020 2020 2020 2020 2069 6620 2745             if 'E
-00005460: 5252 2720 696e 2072 6573 3a0a 2020 2020  RR' in res:.    
-00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005480: 7265 7475 726e 2022 4641 494c 220a 2020  return "FAIL".  
-00005490: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-000054a0: 6974 5f63 6f75 6e74 6572 202b 3d20 310a  it_counter += 1.
-000054b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054c0: 736c 6565 7028 302e 3129 0a20 2020 2020  sleep(0.1).     
-000054d0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-000054e0: 6c66 2e69 735f 646f 6f72 5f63 6c6f 7365  lf.is_door_close
-000054f0: 6428 293a 0a20 2020 2020 2020 2020 2020  d():.           
-00005500: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00005510: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-00005520: 2020 2020 2020 2020 2020 6622 7b73 656c            f"{sel
-00005530: 662e 706f 7274 7d20 446f 6f72 2073 7461  f.port} Door sta
-00005540: 7475 7320 646f 6573 6e27 7420 6d61 7463  tus doesn't matc
-00005550: 6820 636f 6d6d 616e 6420 7365 6e74 2122  h command sent!"
-00005560: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00005570: 696e 7428 6622 4368 616d 6265 7220 7b73  int(f"Chamber {s
-00005580: 656c 662e 706f 7274 7d20 636c 6f73 6564  elf.port} closed
-00005590: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-000055a0: 6574 7572 6e20 274f 4b27 0a20 2020 2020  eturn 'OK'.     
-000055b0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000055c0: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
-000055d0: 2020 2020 2020 7072 696e 7428 6622 4572        print(f"Er
-000055e0: 726f 7220 696e 2063 6c6f 7369 6e67 2063  ror in closing c
-000055f0: 6861 6d62 6572 207b 7365 6c66 2e70 6f72  hamber {self.por
-00005600: 747d 2c20 6475 6520 746f 207b 657d 2229  t}, due to {e}")
-00005610: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00005620: 7572 6e20 2246 4149 4c22 0a0a 2020 2020  urn "FAIL"..    
-00005630: 6465 6620 6973 5f63 6f6e 6e65 6374 6564  def is_connected
-00005640: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00005650: 6966 2073 656c 662e 636f 6d5f 706f 7274  if self.com_port
-00005660: 5f6f 626a 2069 7320 4e6f 6e65 3a0a 2020  _obj is None:.  
-00005670: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00005680: 2046 616c 7365 0a20 2020 2020 2020 2072   False.        r
-00005690: 6574 7572 6e20 7365 6c66 2e63 6f6d 5f70  eturn self.com_p
-000056a0: 6f72 745f 6f62 6a2e 6973 4f70 656e 2829  ort_obj.isOpen()
-000056b0: 0a0a 2020 2020 6465 6620 6765 745f 7374  ..    def get_st
-000056c0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000056d0: 2020 2073 7461 7465 203d 2027 270a 2020     state = ''.  
-000056e0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000056f0: 2020 2020 2020 2073 656c 662e 636f 6d5f         self.com_
-00005700: 706f 7274 5f6f 626a 2e72 6573 6574 5f69  port_obj.reset_i
-00005710: 6e70 7574 5f62 7566 6665 7228 290a 2020  nput_buffer().  
-00005720: 2020 2020 2020 2020 2020 736c 6565 7028            sleep(
-00005730: 302e 3129 0a20 2020 2020 2020 2020 2020  0.1).           
-00005740: 2069 6620 7365 6c66 2e64 6f6f 725f 636d   if self.door_cm
-00005750: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
-00005760: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00005770: 6e20 7374 6174 650a 2020 2020 2020 2020  n state.        
-00005780: 2020 2020 7365 6c66 2e63 6f6d 5f70 6f72      self.com_por
-00005790: 745f 6f62 6a2e 7772 6974 6528 7365 6c66  t_obj.write(self
-000057a0: 2e64 6f6f 725f 636d 6429 0a20 2020 2020  .door_cmd).     
-000057b0: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
-000057c0: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
-000057d0: 6174 6520 3d20 7365 6c66 2e63 6f6d 5f70  ate = self.com_p
-000057e0: 6f72 745f 6f62 6a2e 7265 6164 2831 3429  ort_obj.read(14)
-000057f0: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-00005800: 2e75 7070 6572 2829 2e72 7374 7269 7028  .upper().rstrip(
-00005810: 275c 7227 290a 2020 2020 2020 2020 6578  '\r').        ex
-00005820: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00005830: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-00005840: 2070 7269 6e74 2866 2743 6f75 6c64 206e   print(f'Could n
-00005850: 6f74 2063 6f6d 6d75 6e69 6361 7465 2077  ot communicate w
-00005860: 6974 6820 6368 616d 6265 7220 6475 6520  ith chamber due 
-00005870: 746f 207b 657d 2e20 706c 6561 7365 2063  to {e}. please c
-00005880: 6865 636b 2063 6861 6d62 6572 2063 6f6e  heck chamber con
-00005890: 6e65 6374 696f 6e27 290a 2020 2020 2020  nection').      
-000058a0: 2020 7265 7475 726e 2073 7461 7465 0a0a    return state..
-000058b0: 2020 2020 6465 6620 6973 5f64 6f6f 725f      def is_door_
-000058c0: 6f70 656e 2873 656c 6629 3a0a 2020 2020  open(self):.    
-000058d0: 2020 2020 7374 6174 6520 3d20 7365 6c66      state = self
-000058e0: 2e67 6574 5f73 7461 7465 2829 0a20 2020  .get_state().   
-000058f0: 2020 2020 2069 6620 274f 5045 4e27 2069       if 'OPEN' i
-00005900: 6e20 7374 6174 653a 0a20 2020 2020 2020  n state:.       
-00005910: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00005920: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005930: 4661 6c73 650a 0a20 2020 2064 6566 2069  False..    def i
-00005940: 735f 646f 6f72 5f63 6c6f 7365 6428 7365  s_door_closed(se
-00005950: 6c66 293a 0a20 2020 2020 2020 2073 7461  lf):.        sta
-00005960: 7465 203d 2073 656c 662e 6765 745f 7374  te = self.get_st
-00005970: 6174 6528 290a 2020 2020 2020 2020 6966  ate().        if
-00005980: 2027 434c 4f53 4527 2069 6e20 7374 6174   'CLOSE' in stat
-00005990: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000059a0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-000059b0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-000059c0: 0a0a 636c 6173 7320 4261 7263 6f64 6553  ..class BarcodeS
-000059d0: 6361 6e6e 6572 3a0a 2020 2020 6465 6620  canner:.    def 
-000059e0: 5f5f 696e 6974 5f5f 2873 656c 662c 2063  __init__(self, c
-000059f0: 6f6d 5f70 6f72 743a 2073 7472 203d 204e  om_port: str = N
-00005a00: 6f6e 652c 2062 6175 645f 7261 7465 3a20  one, baud_rate: 
-00005a10: 696e 7420 3d20 3131 3532 3030 2c20 636f  int = 115200, co
-00005a20: 6e66 6967 3a20 626f 6f6c 203d 2054 7275  nfig: bool = Tru
-00005a30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00005a40: 2020 2020 6c6f 675f 7479 7065 3a20 7374      log_type: st
-00005a50: 7220 3d20 274e 4f5f 4c4f 4727 2c20 7772  r = 'NO_LOG', wr
-00005a60: 6974 655f 746f 5f6c 6f67 3a20 626f 6f6c  ite_to_log: bool
-00005a70: 203d 2046 616c 7365 2c20 7469 6d65 6f75   = False, timeou
-00005a80: 743a 2073 7472 203d 2027 3130 3030 272c  t: str = '1000',
-00005a90: 206c 6f67 5f6e 616d 653a 2073 7472 203d   log_name: str =
-00005aa0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00005ab0: 2222 220a 2020 2020 2020 2020 496e 6974  """.        Init
-00005ac0: 6961 6c69 7a65 2074 6865 2051 5253 6361  ialize the QRSca
-00005ad0: 6e6e 6572 206f 626a 6563 742e 0a20 2020  nner object..   
-00005ae0: 2020 2020 2044 6174 6173 6865 6574 3a0a       Datasheet:.
-00005af0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00005b00: 6364 6e2e 7274 7363 616e 2e6e 6574 2f77  cdn.rtscan.net/w
-00005b10: 702d 636f 6e74 656e 742f 7570 6c6f 6164  p-content/upload
-00005b20: 732f 3230 3232 2f30 362f 5573 6572 5f4d  s/2022/06/User_M
-00005b30: 616e 7561 6c5f 5254 3231 345f 5254 3231  anual_RT214_RT21
-00005b40: 375f 5254 3233 355f 5254 3234 305f 3230  7_RT235_RT240_20
-00005b50: 3232 2e30 355f 312e 302e 362e 7064 660a  22.05_1.0.6.pdf.
-00005b60: 2020 2020 2020 2020 466f 7220 7468 6520          For the 
-00005b70: 6669 7273 7420 7573 652c 2079 6f75 2077  first use, you w
-00005b80: 696c 6c20 6e65 6564 2074 6f20 7363 616e  ill need to scan
-00005b90: 2033 2062 6172 636f 6465 2074 6f20 696e   3 barcode to in
-00005ba0: 6974 6961 6c20 636f 6d70 6f72 7420 636f  itial comport co
-00005bb0: 6e6e 6563 7469 6f6e 3a0a 2020 2020 2020  nnection:.      
-00005bc0: 2020 6874 7470 733a 2f2f 7769 6c69 6f74    https://wiliot
-00005bd0: 2e61 746c 6173 7369 616e 2e6e 6574 2f77  .atlassian.net/w
-00005be0: 696b 692f 7370 6163 6573 2f46 572f 7061  iki/spaces/FW/pa
-00005bf0: 6765 732f 3235 3636 3032 3934 3037 2f52  ges/2566029407/R
-00005c00: 5473 6361 6e2b 4261 7263 6f64 652b 5363  Tscan+Barcode+Sc
-00005c10: 616e 6e65 720a 2020 2020 2020 2020 4070  anner.        @p
-00005c20: 6172 616d 2063 6f6d 3a0a 2020 2020 2020  aram com:.      
-00005c30: 2020 4074 7970 6520 636f 6d3a 0a20 2020    @type com:.   
-00005c40: 2020 2020 2040 7061 7261 6d20 6261 7564       @param baud
-00005c50: 3a0a 2020 2020 2020 2020 4074 7970 6520  :.        @type 
-00005c60: 6261 7564 3a0a 2020 2020 2020 2020 4070  baud:.        @p
-00005c70: 6172 616d 2063 6f6e 6669 673a 0a20 2020  aram config:.   
-00005c80: 2020 2020 2040 7479 7065 2063 6f6e 6669       @type confi
-00005c90: 673a 0a20 2020 2020 2020 2040 7061 7261  g:.        @para
-00005ca0: 6d20 6c6f 675f 7479 7065 3a0a 2020 2020  m log_type:.    
-00005cb0: 2020 2020 4074 7970 6520 6c6f 675f 7479      @type log_ty
-00005cc0: 7065 3a0a 2020 2020 2020 2020 4070 6172  pe:.        @par
-00005cd0: 616d 2077 7269 7465 5f74 6f5f 6c6f 673a  am write_to_log:
-00005ce0: 0a20 2020 2020 2020 2040 7479 7065 2077  .        @type w
-00005cf0: 7269 7465 5f74 6f5f 6c6f 673a 0a20 2020  rite_to_log:.   
-00005d00: 2020 2020 2040 7061 7261 6d20 7469 6d65       @param time
-00005d10: 6f75 743a 0a20 2020 2020 2020 2040 7479  out:.        @ty
-00005d20: 7065 2074 696d 656f 7574 3a0a 2020 2020  pe timeout:.    
-00005d30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00005d40: 7365 6c66 2e70 7265 6669 7820 3d20 277e  self.prefix = '~
-00005d50: 0130 3030 3040 270a 2020 2020 2020 2020  .0000@'.        
-00005d60: 7365 6c66 2e73 7566 6669 7820 3d20 273b  self.suffix = ';
-00005d70: 0327 0a20 2020 2020 2020 2073 656c 662e  .'.        self.
-00005d80: 636f 6d5f 706f 7274 203d 2063 6f6d 5f70  com_port = com_p
-00005d90: 6f72 740a 2020 2020 2020 2020 7365 6c66  ort.        self
-00005da0: 2e73 6572 6961 6c5f 636f 6e6e 6563 7469  .serial_connecti
-00005db0: 6f6e 203d 204e 6f6e 650a 2020 2020 2020  on = None.      
-00005dc0: 2020 7365 6c66 2e64 6576 6963 655f 7369    self.device_si
-00005dd0: 676e 6174 7572 6520 3d20 224e 4c53 2d4e  gnature = "NLS-N
-00005de0: 3122 0a20 2020 2020 2020 2073 656c 662e  1".        self.
-00005df0: 6c6f 675f 7479 7065 203d 206c 6f67 5f74  log_type = log_t
-00005e00: 7970 650a 2020 2020 2020 2020 7365 6c66  ype.        self
-00005e10: 2e77 7269 7465 5f74 6f5f 6c6f 6720 3d20  .write_to_log = 
-00005e20: 7772 6974 655f 746f 5f6c 6f67 0a20 2020  write_to_log.   
-00005e30: 2020 2020 2073 656c 662e 7367 7469 6e5f       self.sgtin_
-00005e40: 6c65 6e67 7468 203d 2033 310a 0a20 2020  length = 31..   
-00005e50: 2020 2020 2069 6620 6c6f 675f 6e61 6d65       if log_name
-00005e60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00005e70: 2020 2020 2020 7365 6c66 2e71 725f 6c6f        self.qr_lo
-00005e80: 6767 6572 203d 206c 6f67 6769 6e67 2e67  gger = logging.g
-00005e90: 6574 4c6f 6767 6572 2827 5152 4c6f 6767  etLogger('QRLogg
-00005ea0: 6572 2729 0a20 2020 2020 2020 2065 6c73  er').        els
-00005eb0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00005ec0: 656c 662e 7172 5f6c 6f67 6765 7220 3d20  elf.qr_logger = 
-00005ed0: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
-00005ee0: 7228 6c6f 675f 6e61 6d65 290a 0a20 2020  r(log_name)..   
-00005ef0: 2020 2020 2069 6620 636f 6d5f 706f 7274       if com_port
-00005f00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00005f10: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
-00005f20: 7065 6e5f 706f 7274 2863 6f6d 5f70 6f72  pen_port(com_por
-00005f30: 742c 2062 6175 645f 7261 7465 3d62 6175  t, baud_rate=bau
-00005f40: 645f 7261 7465 2c20 636f 6e66 6967 3d63  d_rate, config=c
-00005f50: 6f6e 6669 672c 2074 696d 656f 7574 3d74  onfig, timeout=t
-00005f60: 696d 656f 7574 290a 2020 2020 2020 2020  imeout).        
-00005f70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00005f80: 2020 7365 6c66 2e61 7574 6f5f 636f 6e6e    self.auto_conn
-00005f90: 6563 7428 7469 6d65 6f75 743d 7469 6d65  ect(timeout=time
-00005fa0: 6f75 7429 0a0a 2020 2020 2020 2020 6966  out)..        if
-00005fb0: 2073 656c 662e 7772 6974 655f 746f 5f6c   self.write_to_l
-00005fc0: 6f67 3a0a 2020 2020 2020 2020 2020 2020  og:.            
-00005fd0: 7365 6c66 2e63 7265 6174 655f 6c6f 675f  self.create_log_
-00005fe0: 6669 6c65 2829 0a0a 2020 2020 6465 6620  file()..    def 
-00005ff0: 6372 6561 7465 5f6c 6f67 5f66 696c 6528  create_log_file(
-00006000: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00006010: 2222 0a20 2020 2020 2020 2043 7265 6174  "".        Creat
-00006020: 6520 6120 6c6f 6720 6669 6c65 2e0a 2020  e a log file..  
-00006030: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006040: 2020 7769 6c69 6f74 5f64 6972 203d 2057    wiliot_dir = W
-00006050: 696c 696f 7444 6972 2829 0a20 2020 2020  iliotDir().     
-00006060: 2020 2077 696c 696f 745f 6469 722e 6372     wiliot_dir.cr
-00006070: 6561 7465 5f64 6972 2827 5152 5f73 6361  eate_dir('QR_sca
-00006080: 6e27 290a 2020 2020 2020 2020 6170 705f  n').        app_
-00006090: 6469 7220 3d20 7769 6c69 6f74 5f64 6972  dir = wiliot_dir
-000060a0: 2e67 6574 5f77 696c 696f 745f 726f 6f74  .get_wiliot_root
-000060b0: 5f61 7070 5f64 6972 2829 0a20 2020 2020  _app_dir().     
-000060c0: 2020 206c 6f67 5f64 6972 203d 206f 732e     log_dir = os.
-000060d0: 7061 7468 2e6a 6f69 6e28 6170 705f 6469  path.join(app_di
-000060e0: 722c 2027 5152 5f73 6361 6e27 290a 2020  r, 'QR_scan').  
-000060f0: 2020 2020 2020 6966 206e 6f74 206f 732e        if not os.
-00006100: 7061 7468 2e65 7869 7374 7328 6c6f 675f  path.exists(log_
-00006110: 6469 7229 3a0a 2020 2020 2020 2020 2020  dir):.          
-00006120: 2020 6f73 2e6d 616b 6564 6972 7328 6c6f    os.makedirs(lo
-00006130: 675f 6469 7229 0a0a 2020 2020 2020 2020  g_dir)..        
-00006140: 6375 7272 656e 745f 7469 6d65 203d 2064  current_time = d
-00006150: 6174 6574 696d 652e 6e6f 7728 292e 7374  atetime.now().st
-00006160: 7266 7469 6d65 2822 2559 2d25 6d2d 2564  rftime("%Y-%m-%d
-00006170: 5f25 482d 254d 2d25 5322 290a 2020 2020  _%H-%M-%S").    
-00006180: 2020 2020 7365 6c66 2e6c 6f67 5f66 696c      self.log_fil
-00006190: 656e 616d 6520 3d20 6f73 2e70 6174 682e  ename = os.path.
-000061a0: 6a6f 696e 286c 6f67 5f64 6972 2c20 6622  join(log_dir, f"
-000061b0: 5152 5f72 6561 645f 6c6f 675f 7b63 7572  QR_read_log_{cur
-000061c0: 7265 6e74 5f74 696d 657d 2e6c 6f67 2229  rent_time}.log")
-000061d0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
-000061e0: 656e 2873 656c 662e 6c6f 675f 6669 6c65  en(self.log_file
-000061f0: 6e61 6d65 2c20 2777 2729 2061 7320 663a  name, 'w') as f:
-00006200: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
-00006210: 7269 7465 2822 4c6f 6720 6669 6c65 2063  rite("Log file c
-00006220: 7265 6174 6564 2e5c 6e22 290a 0a20 2020  reated.\n")..   
-00006230: 2064 6566 2061 7574 6f5f 636f 6e6e 6563   def auto_connec
-00006240: 7428 7365 6c66 2c20 6261 7564 5f72 6174  t(self, baud_rat
-00006250: 653a 2069 6e74 203d 2031 3135 3230 302c  e: int = 115200,
-00006260: 2063 6f6e 6669 673a 2062 6f6f 6c20 3d20   config: bool = 
-00006270: 5472 7565 2c20 7469 6d65 6f75 743a 2073  True, timeout: s
-00006280: 7472 203d 2027 3130 3030 2729 3a0a 2020  tr = '1000'):.  
-00006290: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000062a0: 2020 4175 746f 6d61 7469 6361 6c6c 7920    Automatically 
-000062b0: 636f 6e6e 6563 7420 746f 2074 6865 2043  connect to the C
-000062c0: 4f4d 2070 6f72 742e 0a20 2020 2020 2020  OM port..       
-000062d0: 2022 2222 0a20 2020 2020 2020 2063 6f6d   """.        com
-000062e0: 5f70 6f72 7420 3d20 7365 6c66 2e66 696e  _port = self.fin
-000062f0: 645f 636f 6d5f 706f 7274 2862 6175 645f  d_com_port(baud_
-00006300: 7261 7465 290a 2020 2020 2020 2020 6966  rate).        if
-00006310: 2063 6f6d 5f70 6f72 7420 6973 206e 6f74   com_port is not
-00006320: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006330: 2020 2073 656c 662e 6f70 656e 5f70 6f72     self.open_por
-00006340: 7428 636f 6d5f 706f 7274 2c20 6261 7564  t(com_port, baud
-00006350: 5f72 6174 652c 2063 6f6e 6669 672c 2074  _rate, config, t
-00006360: 696d 656f 7574 3d74 696d 656f 7574 290a  imeout=timeout).
-00006370: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00006380: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
-00006390: 725f 6c6f 6767 6572 2e65 7272 6f72 2822  r_logger.error("
-000063a0: 4e6f 2073 7569 7461 626c 6520 434f 4d20  No suitable COM 
-000063b0: 706f 7274 2066 6f75 6e64 2e22 290a 2020  port found.").  
-000063c0: 2020 2020 2020 2020 2020 7379 732e 6578            sys.ex
-000063d0: 6974 2831 290a 0a20 2020 2064 6566 2069  it(1)..    def i
-000063e0: 735f 7274 7363 616e 5f72 7432 3335 2873  s_rtscan_rt235(s
-000063f0: 656c 662c 2063 6f6d 5f70 6f72 743a 2073  elf, com_port: s
-00006400: 7472 2c20 6261 7564 5f72 6174 653a 2069  tr, baud_rate: i
-00006410: 6e74 203d 2031 3135 3230 3029 202d 3e20  nt = 115200) -> 
-00006420: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00006430: 220a 2020 2020 2020 2020 4368 6563 6b20  ".        Check 
-00006440: 6966 2074 6865 2064 6576 6963 6520 6973  if the device is
-00006450: 2052 5473 6361 6e20 5254 3233 352e 0a20   RTscan RT235.. 
-00006460: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00006470: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00006480: 2020 2020 7769 7468 2073 6572 6961 6c2e      with serial.
-00006490: 5365 7269 616c 2863 6f6d 5f70 6f72 742c  Serial(com_port,
-000064a0: 2062 6175 645f 7261 7465 2c20 7469 6d65   baud_rate, time
-000064b0: 6f75 743d 3129 2061 7320 7365 723a 0a20  out=1) as ser:. 
-000064c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000064d0: 6572 2e77 7269 7465 2873 7472 2e65 6e63  er.write(str.enc
-000064e0: 6f64 6528 7365 6c66 2e70 7265 6669 7820  ode(self.prefix 
-000064f0: 2b20 2251 5259 5044 4e22 202b 2073 656c  + "QRYPDN" + sel
-00006500: 662e 7375 6666 6978 2929 0a20 2020 2020  f.suffix)).     
-00006510: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-00006520: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
-00006530: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00006540: 2073 6572 2e72 6561 645f 616c 6c28 292e   ser.read_all().
-00006550: 6465 636f 6465 2829 0a20 2020 2020 2020  decode().       
-00006560: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00006570: 7365 6c66 2e64 6576 6963 655f 7369 676e  self.device_sign
-00006580: 6174 7572 6520 696e 2072 6573 706f 6e73  ature in respons
-00006590: 650a 2020 2020 2020 2020 6578 6365 7074  e.        except
-000065a0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-000065b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000065c0: 662e 7172 5f6c 6f67 6765 722e 6572 726f  f.qr_logger.erro
-000065d0: 7228 6622 4572 726f 7220 696e 2069 735f  r(f"Error in is_
-000065e0: 7274 7363 616e 5f72 7432 3335 3a20 7b65  rtscan_rt235: {e
-000065f0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00006600: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
-00006610: 2020 6465 6620 6669 6e64 5f63 6f6d 5f70    def find_com_p
-00006620: 6f72 7428 7365 6c66 2c20 6261 7564 5f72  ort(self, baud_r
-00006630: 6174 653a 2069 6e74 203d 2031 3135 3230  ate: int = 11520
-00006640: 3029 202d 3e20 7374 723a 0a20 2020 2020  0) -> str:.     
-00006650: 2020 2022 2222 0a20 2020 2020 2020 2046     """.        F
-00006660: 696e 6420 7468 6520 434f 4d20 706f 7274  ind the COM port
-00006670: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00006680: 2020 2020 2020 636f 6d5f 706f 7274 7320        com_ports 
-00006690: 3d20 7365 7269 616c 5f70 6f72 7473 2829  = serial_ports()
-000066a0: 0a20 2020 2020 2020 2066 6f72 2063 6f6d  .        for com
-000066b0: 5f70 6f72 7420 696e 2063 6f6d 5f70 6f72  _port in com_por
-000066c0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-000066d0: 6966 2073 656c 662e 6973 5f72 7473 6361  if self.is_rtsca
-000066e0: 6e5f 7274 3233 3528 636f 6d5f 706f 7274  n_rt235(com_port
-000066f0: 2c20 6261 7564 5f72 6174 6529 3a0a 2020  , baud_rate):.  
-00006700: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00006710: 7475 726e 2063 6f6d 5f70 6f72 740a 2020  turn com_port.  
-00006720: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00006730: 650a 0a20 2020 2064 6566 206f 7065 6e5f  e..    def open_
-00006740: 706f 7274 2873 656c 662c 2063 6f6d 5f70  port(self, com_p
-00006750: 6f72 743a 2073 7472 2c20 6261 7564 5f72  ort: str, baud_r
-00006760: 6174 653a 2069 6e74 203d 2031 3135 3230  ate: int = 11520
-00006770: 302c 2063 6f6e 6669 673a 2062 6f6f 6c20  0, config: bool 
-00006780: 3d20 5472 7565 2c20 7469 6d65 6f75 743a  = True, timeout:
-00006790: 2073 7472 203d 2027 3130 3030 2729 3a0a   str = '1000'):.
-000067a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000067b0: 2020 2020 4f70 656e 2074 6865 2043 4f4d      Open the COM
-000067c0: 2070 6f72 742e 0a20 2020 2020 2020 2022   port..        "
-000067d0: 2222 0a20 2020 2020 2020 2074 7279 3a0a  "".        try:.
-000067e0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000067f0: 6f74 2073 656c 662e 6973 5f72 7473 6361  ot self.is_rtsca
-00006800: 6e5f 7274 3233 3528 636f 6d5f 706f 7274  n_rt235(com_port
-00006810: 2c20 6261 7564 5f72 6174 6529 3a0a 2020  , baud_rate):.  
-00006820: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00006830: 6973 6520 4578 6365 7074 696f 6e28 6627  ise Exception(f'
-00006840: 7b63 6f6d 5f70 6f72 747d 2069 7320 6e6f  {com_port} is no
-00006850: 7420 6120 6261 7263 6f64 6520 7363 616e  t a barcode scan
-00006860: 6e65 7227 290a 2020 2020 2020 2020 2020  ner').          
-00006870: 2020 7365 6c66 2e73 6572 6961 6c5f 636f    self.serial_co
-00006880: 6e6e 6563 7469 6f6e 203d 2073 6572 6961  nnection = seria
-00006890: 6c2e 5365 7269 616c 2863 6f6d 5f70 6f72  l.Serial(com_por
-000068a0: 742c 2062 6175 645f 7261 7465 2c20 7469  t, baud_rate, ti
-000068b0: 6d65 6f75 743d 2869 6e74 2874 696d 656f  meout=(int(timeo
-000068c0: 7574 2920 2b20 3530 2920 2f20 3130 3030  ut) + 50) / 1000
-000068d0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-000068e0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-000068f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006900: 662e 636c 6f73 655f 706f 7274 2829 0a20  f.close_port(). 
-00006910: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00006920: 2045 7863 6570 7469 6f6e 2866 2743 6f75   Exception(f'Cou
-00006930: 6c64 206e 6f74 2063 6f6e 6e65 6374 2074  ld not connect t
-00006940: 6f20 7b63 6f6d 5f70 6f72 747d 3a20 7b65  o {com_port}: {e
-00006950: 7d27 290a 0a20 2020 2020 2020 2069 6620  }')..        if 
-00006960: 7365 6c66 2e73 6572 6961 6c5f 636f 6e6e  self.serial_conn
-00006970: 6563 7469 6f6e 2069 7320 6e6f 7420 4e6f  ection is not No
-00006980: 6e65 2061 6e64 2073 656c 662e 6c6f 675f  ne and self.log_
-00006990: 7479 7065 2021 3d20 274e 4f5f 4c4f 4727  type != 'NO_LOG'
-000069a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000069b0: 6c66 2e71 725f 6c6f 6767 6572 2e69 6e66  lf.qr_logger.inf
-000069c0: 6f28 6627 4261 7263 6f64 6520 7363 616e  o(f'Barcode scan
-000069d0: 6e65 7220 287b 636f 6d5f 706f 7274 7d29  ner ({com_port})
-000069e0: 2063 6f6e 6e65 6374 6564 2e27 290a 2020   connected.').  
-000069f0: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-00006a00: 7365 7269 616c 5f63 6f6e 6e65 6374 696f  serial_connectio
-00006a10: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-00006a20: 2020 2020 2020 2073 656c 662e 7172 5f6c         self.qr_l
-00006a30: 6f67 6765 722e 6572 726f 7228 6627 4261  ogger.error(f'Ba
-00006a40: 7263 6f64 6520 7363 616e 6e65 7220 2d20  rcode scanner - 
-00006a50: 5072 6f62 6c65 6d20 636f 6e6e 6563 7469  Problem connecti
-00006a60: 6e67 207b 636f 6d5f 706f 7274 7d27 290a  ng {com_port}').
-00006a70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006a80: 726e 0a0a 2020 2020 2020 2020 7365 6c66  rn..        self
-00006a90: 2e63 6f6d 5f70 6f72 7420 3d20 636f 6d5f  .com_port = com_
-00006aa0: 706f 7274 0a20 2020 2020 2020 2073 656c  port.        sel
-00006ab0: 662e 7365 7269 616c 5f63 6f6e 6e65 6374  f.serial_connect
-00006ac0: 696f 6e2e 7772 6974 6554 696d 656f 7574  ion.writeTimeout
-00006ad0: 203d 2030 2e35 2020 2320 7772 6974 6520   = 0.5  # write 
-00006ae0: 7469 6d65 6f75 742e 0a20 2020 2020 2020  timeout..       
-00006af0: 2069 6620 636f 6e66 6967 3a0a 2020 2020   if config:.    
-00006b00: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00006b10: 6669 6775 7265 2874 696d 655f 6f75 743d  figure(time_out=
-00006b20: 7469 6d65 6f75 7429 0a0a 2020 2020 6465  timeout)..    de
-00006b30: 6620 636c 6f73 655f 706f 7274 2873 656c  f close_port(sel
-00006b40: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-00006b50: 2020 2020 2020 2020 436c 6f73 6520 7468          Close th
-00006b60: 6520 434f 4d20 706f 7274 2e0a 2020 2020  e COM port..    
-00006b70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006b80: 6966 2073 656c 662e 7365 7269 616c 5f63  if self.serial_c
-00006b90: 6f6e 6e65 6374 696f 6e20 6973 206e 6f74  onnection is not
-00006ba0: 204e 6f6e 6520 616e 6420 7365 6c66 2e73   None and self.s
-00006bb0: 6572 6961 6c5f 636f 6e6e 6563 7469 6f6e  erial_connection
-00006bc0: 2e69 734f 7065 6e28 293a 0a20 2020 2020  .isOpen():.     
-00006bd0: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
-00006be0: 616c 5f63 6f6e 6e65 6374 696f 6e2e 636c  al_connection.cl
-00006bf0: 6f73 6528 290a 0a20 2020 2064 6566 2069  ose()..    def i
-00006c00: 735f 6f70 656e 2873 656c 6629 202d 3e20  s_open(self) -> 
-00006c10: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00006c20: 220a 2020 2020 2020 2020 4368 6563 6b20  ".        Check 
-00006c30: 6966 2074 6865 2043 4f4d 2070 6f72 7420  if the COM port 
-00006c40: 6973 206f 7065 6e2e 0a20 2020 2020 2020  is open..       
-00006c50: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
-00006c60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00006c70: 7320 3d20 7365 6c66 2e6d 616e 7561 6c5f  s = self.manual_
-00006c80: 636f 6e66 6967 7572 6528 5b27 5152 5950  configure(['QRYP
-00006c90: 444e 275d 290a 2020 2020 2020 2020 2020  DN']).          
-00006ca0: 2020 6966 2027 4e4c 532d 4e31 2720 696e    if 'NLS-N1' in
-00006cb0: 2073 7472 2872 6573 293a 0a20 2020 2020   str(res):.     
-00006cc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00006cd0: 6e20 5472 7565 0a20 2020 2020 2020 2020  n True.         
-00006ce0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00006cf0: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-00006d00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006d10: 726e 2046 616c 7365 0a0a 2020 2020 6465  rn False..    de
-00006d20: 6620 636f 6e66 6967 7572 6528 7365 6c66  f configure(self
-00006d30: 2c20 696c 6c5f 7363 6e3d 2731 272c 2061  , ill_scn='1', a
-00006d40: 6d6c 5f65 6e61 3d27 3127 2c20 6772 625f  ml_ena='1', grb_
-00006d50: 656e 613d 2730 272c 2067 7262 5f76 6c6c  ena='0', grb_vll
-00006d60: 3d27 3227 2c20 6174 735f 656e 613d 2730  ='2', ats_ena='0
-00006d70: 272c 2061 7473 5f64 7572 3d27 3336 3030  ', ats_dur='3600
-00006d80: 3027 2c20 7363 6e5f 6d6f 643d 2730 272c  0', scn_mod='0',
-00006d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006da0: 2020 2070 7762 5f65 6e61 3d27 3027 2c20     pwb_ena='0', 
-00006db0: 7272 6472 5f65 6e3d 2731 272c 2067 7264  rrdr_en='1', grd
-00006dc0: 5f65 6e61 3d27 3027 2c20 6772 645f 6475  _ena='0', grd_du
-00006dd0: 723d 2731 272c 2074 696d 655f 6f75 743d  r='1', time_out=
-00006de0: 2731 3027 2c20 6261 645f 6d73 675f 656e  '10', bad_msg_en
-00006df0: 3d54 7275 652c 2073 796d 626f 6c6f 6769  =True, symbologi
-00006e00: 6573 3d4e 6f6e 6529 3a0a 2020 2020 2020  es=None):.      
-00006e10: 2020 2727 270a 2020 2020 2020 2020 696c    '''.        il
-00006e20: 6c5f 7363 6e20 2d20 696c 6c75 6d69 6e61  l_scn - illumina
-00006e30: 7469 6f6e 3a20 2020 2020 2020 2020 302d  tion:         0-
-00006e40: 6f66 662c 2031 2d6e 6f72 6d61 6c2c 2032  off, 1-normal, 2
-00006e50: 2d61 6c77 6179 7320 6f6e 0a20 2020 2020  -always on.     
-00006e60: 2020 2061 6d6c 5f65 6e61 202d 2061 696d     aml_ena - aim
-00006e70: 696e 673a 2020 2020 2020 2020 2020 2020  ing:            
-00006e80: 2020 2030 2d6f 6666 2c20 312d 6e6f 726d     0-off, 1-norm
-00006e90: 616c 2c20 322d 616c 7761 7973 206f 6e0a  al, 2-always on.
-00006ea0: 2020 2020 2020 2020 7077 625f 656e 6120          pwb_ena 
-00006eb0: 2d20 706f 7765 7220 6f6e 2062 6565 7020  - power on beep 
-00006ec0: 2020 2020 2020 2020 302d 6f66 662c 2031          0-off, 1
-00006ed0: 2d6f 6e0a 2020 2020 2020 2020 6772 625f  -on.        grb_
-00006ee0: 656e 6120 2d20 676f 6f64 2072 6561 6420  ena - good read 
-00006ef0: 6265 6570 2020 2020 2020 2020 302d 6f66  beep        0-of
-00006f00: 662c 2031 2d6f 6e0a 2020 2020 2020 2020  f, 1-on.        
-00006f10: 6772 645f 656e 6120 2d20 676f 6f64 2072  grd_ena - good r
-00006f20: 6561 6420 656e 6162 6c65 2020 2020 2020  ead enable      
-00006f30: 302d 6f66 662c 2031 2d6f 6e0a 2020 2020  0-off, 1-on.    
-00006f40: 2020 2020 6772 645f 6475 7220 2d20 676f      grd_dur - go
-00006f50: 6f64 2072 6561 6420 6475 7261 7469 6f6e  od read duration
-00006f60: 2020 2020 312d 3336 3030 3020 5b6d 7365      1-36000 [mse
-00006f70: 635d 0a20 2020 2020 2020 2061 7473 5f65  c].        ats_e
-00006f80: 6e61 202d 2061 7574 6f20 736c 6565 7020  na - auto sleep 
-00006f90: 2020 2020 2020 2020 2020 2030 2d64 6973             0-dis
-00006fa0: 6162 6c65 2c20 312d 656e 6162 6c65 0a20  able, 1-enable. 
-00006fb0: 2020 2020 2020 2061 7473 5f64 7572 202d         ats_dur -
-00006fc0: 2073 6c65 6570 2064 7572 6174 696f 6e20   sleep duration 
-00006fd0: 2020 2020 2020 2031 2d33 3630 3030 205b         1-36000 [
-00006fe0: 7365 635d 0a20 2020 2020 2020 2072 7264  sec].        rrd
-00006ff0: 725f 656e 202d 2052 6572 6561 6420 7265  r_en - Reread re
-00007000: 7365 7420 2020 2020 2020 2020 2030 2d6f  set          0-o
-00007010: 6666 2c20 312d 6f6e 0a20 2020 2020 2020  ff, 1-on.       
-00007020: 2073 636e 5f6d 6f64 202d 2073 6361 6e20   scn_mod - scan 
-00007030: 6d6f 6465 2020 2020 2020 2020 2020 2020  mode            
-00007040: 2030 2d6c 6576 656c 206d 6f64 652c 2032   0-level mode, 2
-00007050: 2d73 656e 7365 206d 6f64 652c 2033 2d63  -sense mode, 3-c
-00007060: 6f6e 7469 6e75 6f75 7320 6d6f 6465 2c20  ontinuous mode, 
-00007070: 372d 6261 7463 6820 6d6f 6465 0a20 2020  7-batch mode.   
-00007080: 2020 2020 2073 796d 626f 6c6f 6769 6573       symbologies
-00007090: 202d 2061 206c 6973 7420 6f66 2073 7472   - a list of str
-000070a0: 696e 6773 2072 6570 7265 7365 6e74 696e  ings representin
-000070b0: 6720 7468 6520 7379 6d62 6f6c 6f67 6965  g the symbologie
-000070c0: 7320 746f 2065 6e61 626c 652c 2065 2e67  s to enable, e.g
-000070d0: 2e20 5b27 5152 272c 2027 5044 4634 3137  . ['QR', 'PDF417
-000070e0: 272c 2027 4541 4e31 3327 5d0a 0a20 2020  ', 'EAN13']..   
-000070f0: 2020 2020 204c 6576 656c 204d 6f64 653a       Level Mode:
-00007100: 0a20 2020 2020 2020 2049 6e20 7468 6973  .        In this
-00007110: 206d 6f64 652c 2074 6865 2073 6361 6e6e   mode, the scann
-00007120: 6572 2077 6169 7473 2066 6f72 2061 2074  er waits for a t
-00007130: 7269 6767 6572 2070 756c 6c20 746f 2061  rigger pull to a
-00007140: 6374 6976 6174 6520 6120 6465 636f 6465  ctivate a decode
-00007150: 2073 6573 7369 6f6e 2e20 5468 6520 6465   session. The de
-00007160: 636f 6465 2073 6573 7369 6f6e 2063 6f6e  code session con
-00007170: 7469 6e75 6573 2075 6e74 696c 2061 2062  tinues until a b
-00007180: 6172 636f 6465 2069 7320 6465 636f 6465  arcode is decode
-00007190: 6420 6f72 2079 6f75 2072 656c 6561 7365  d or you release
-000071a0: 2074 6865 2074 7269 6767 6572 2e0a 2020   the trigger..  
-000071b0: 2020 2020 2020 436f 6d6d 616e 6420 7472        Command tr
-000071c0: 6967 6765 7220 6d6f 6465 3a0a 2020 2020  igger mode:.    
-000071d0: 2020 2020 5468 6973 206d 6f64 6520 7265      This mode re
-000071e0: 7175 6972 6573 2079 6f75 2074 6f20 7365  quires you to se
-000071f0: 6e64 2061 2063 6f6d 6d61 6e64 2028 3142  nd a command (1B
-00007200: 2033 3120 696e 2068 6578 2920 746f 2061   31 in hex) to a
-00007210: 6374 6976 6174 6520 6120 6465 636f 6465  ctivate a decode
-00007220: 2073 6573 7369 6f6e 2e0a 0a20 2020 2020   session...     
-00007230: 2020 2053 656e 7365 204d 6f64 653a 0a20     Sense Mode:. 
-00007240: 2020 2020 2020 2049 6e20 7468 6973 206d         In this m
-00007250: 6f64 652c 2074 6865 2073 6361 6e6e 6572  ode, the scanner
-00007260: 2061 6374 6976 6174 6573 2061 2064 6563   activates a dec
-00007270: 6f64 6520 7365 7373 696f 6e20 6576 6572  ode session ever
-00007280: 7920 7469 6d65 2069 7420 6465 7465 6374  y time it detect
-00007290: 7320 6120 6261 7263 6f64 6520 7072 6573  s a barcode pres
-000072a0: 656e 7465 6420 746f 2069 742e 2054 6865  ented to it. The
-000072b0: 2064 6563 6f64 6520 7365 7373 696f 6e20   decode session 
-000072c0: 636f 6e74 696e 7565 7320 756e 7469 6c20  continues until 
-000072d0: 6120 6261 7263 6f64 6520 6973 2064 6563  a barcode is dec
-000072e0: 6f64 6564 206f 7220 7468 6520 6465 636f  oded or the deco
-000072f0: 6465 2073 6573 7369 6f6e 2074 696d 656f  de session timeo
-00007300: 7574 2065 7870 6972 6573 2e20 596f 7520  ut expires. You 
-00007310: 6361 6e20 6164 6a75 7374 2074 6865 2073  can adjust the s
-00007320: 656e 7369 7469 7669 7479 2061 6e64 2072  ensitivity and r
-00007330: 6572 6561 6420 7469 6d65 6f75 7420 746f  eread timeout to
-00007340: 2061 766f 6964 2075 6e64 6573 6972 6564   avoid undesired
-00007350: 2072 6572 6561 6469 6e67 206f 6620 7468   rereading of th
-00007360: 6520 7361 6d65 2062 6172 636f 6465 2069  e same barcode i
-00007370: 6e20 6120 6769 7665 6e20 7065 7269 6f64  n a given period
-00007380: 206f 6620 7469 6d65 2e20 596f 7520 6361   of time. You ca
-00007390: 6e20 616c 736f 2061 646a 7573 7420 7468  n also adjust th
-000073a0: 6520 696d 6167 6520 7374 6162 696c 697a  e image stabiliz
-000073b0: 6174 696f 6e20 7469 6d65 6f75 7420 746f  ation timeout to
-000073c0: 2067 6976 6520 7468 6520 7363 616e 6e65   give the scanne
-000073d0: 7220 7469 6d65 2074 6f20 6164 6170 7420  r time to adapt 
-000073e0: 746f 2061 6d62 6965 6e74 2065 6e76 6972  to ambient envir
-000073f0: 6f6e 6d65 6e74 2061 6674 6572 2069 7420  onment after it 
-00007400: 6465 636f 6465 7320 6120 6261 7263 6f64  decodes a barcod
-00007410: 6520 616e 6420 e280 9c6c 6f6f 6b73 e280  e and ...looks..
-00007420: 9d20 666f 7220 616e 6f74 6865 722e 0a0a  . for another...
-00007430: 2020 2020 2020 2020 436f 6e74 696e 756f          Continuo
-00007440: 7573 204d 6f64 653a 0a20 2020 2020 2020  us Mode:.       
-00007450: 2049 6e20 7468 6973 206d 6f64 652c 2074   In this mode, t
-00007460: 6865 2073 6361 6e6e 6572 2061 7574 6f6d  he scanner autom
-00007470: 6174 6963 616c 6c79 2073 7461 7274 7320  atically starts 
-00007480: 6f6e 6520 6465 636f 6465 2073 6573 7369  one decode sessi
-00007490: 6f6e 2061 6674 6572 2061 6e6f 7468 6572  on after another
-000074a0: 2e20 546f 2073 7573 7065 6e64 2f72 6573  . To suspend/res
-000074b0: 756d 6520 6261 7263 6f64 6520 7265 6164  ume barcode read
-000074c0: 696e 672c 2073 696d 706c 7920 7072 6573  ing, simply pres
-000074d0: 7320 7468 6520 7472 6967 6765 722e 2059  s the trigger. Y
-000074e0: 6f75 2063 616e 2061 646a 7573 7420 7468  ou can adjust th
-000074f0: 6520 7265 7265 6164 2074 696d 656f 7574  e reread timeout
-00007500: 2074 6f20 6176 6f69 6420 756e 6465 7369   to avoid undesi
-00007510: 7265 6420 7265 7265 6164 696e 6720 6f66  red rereading of
-00007520: 2074 6865 2073 616d 6520 6261 7263 6f64   the same barcod
-00007530: 6520 696e 2061 2067 6976 656e 2070 6572  e in a given per
-00007540: 696f 6420 6f66 2074 696d 652e 204e 6f74  iod of time. Not
-00007550: 6520 7468 6174 2077 6865 6e20 7377 6974  e that when swit
-00007560: 6368 696e 6720 746f 2074 6869 7320 6d6f  ching to this mo
-00007570: 6465 2062 7920 7363 616e 6e69 6e67 2074  de by scanning t
-00007580: 6865 2043 6f6e 7469 6e75 6f75 7320 4d6f  he Continuous Mo
-00007590: 6465 2062 6172 636f 6465 2c20 7468 6520  de barcode, the 
-000075a0: 7363 616e 6e65 7220 7769 6c6c 2073 746f  scanner will sto
-000075b0: 7020 6261 7263 6f64 6520 7265 6164 696e  p barcode readin
-000075c0: 6720 666f 7220 3320 7365 636f 6e64 7320  g for 3 seconds 
-000075d0: 6265 666f 7265 2073 7461 7274 696e 6720  before starting 
-000075e0: 7363 616e 6e69 6e67 2063 6f6e 7469 6e75  scanning continu
-000075f0: 6f75 736c 792e 0a0a 2020 2020 2020 2020  ously...        
-00007600: 4261 7463 6820 4d6f 6465 3a0a 2020 2020  Batch Mode:.    
-00007610: 2020 2020 496e 2074 6869 7320 6d6f 6465      In this mode
-00007620: 2c20 6120 7472 6967 6765 7220 7075 6c6c  , a trigger pull
-00007630: 2061 6374 6976 6174 6573 2061 2072 6f75   activates a rou
-00007640: 6e64 206f 6620 6d75 6c74 6970 6c65 2064  nd of multiple d
-00007650: 6563 6f64 6520 7365 7373 696f 6e73 2e20  ecode sessions. 
-00007660: 5468 6520 726f 756e 6420 6f66 206d 756c  The round of mul
-00007670: 7469 706c 6520 7363 616e 7320 636f 6e74  tiple scans cont
-00007680: 696e 7565 7320 756e 7469 6c20 796f 7520  inues until you 
-00007690: 7265 6c65 6173 6520 7468 6520 7472 6967  release the trig
-000076a0: 6765 722e 2052 6572 6561 6469 6e67 2074  ger. Rereading t
-000076b0: 6865 2073 616d 6520 6261 7263 6f64 6520  he same barcode 
-000076c0: 6973 206e 6f74 2061 6c6c 6f77 6564 2069  is not allowed i
-000076d0: 6e20 7468 6520 7361 6d65 2072 6f75 6e64  n the same round
-000076e0: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-000076f0: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
-00007700: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00007710: 3d20 7b27 494c 4c53 434e 273a 2069 6c6c  = {'ILLSCN': ill
-00007720: 5f73 636e 2c20 2741 4d4c 454e 4127 3a20  _scn, 'AMLENA': 
-00007730: 616d 6c5f 656e 612c 2027 4752 4245 4e41  aml_ena, 'GRBENA
-00007740: 273a 2067 7262 5f65 6e61 2c20 2741 5453  ': grb_ena, 'ATS
-00007750: 454e 4127 3a20 6174 735f 656e 612c 0a20  ENA': ats_ena,. 
-00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007770: 2027 4e47 5245 4e41 273a 2027 3127 2069   'NGRENA': '1' i
-00007780: 6620 6261 645f 6d73 675f 656e 2065 6c73  f bad_msg_en els
-00007790: 6520 2730 272c 0a20 2020 2020 2020 2020  e '0',.         
-000077a0: 2020 2020 2020 2020 2027 4752 4256 4c4c           'GRBVLL
-000077b0: 273a 2067 7262 5f76 6c6c 2c20 2741 5453  ': grb_vll, 'ATS
-000077c0: 4455 5227 3a20 6174 735f 6475 722c 2027  DUR': ats_dur, '
-000077d0: 5343 4e4d 4f44 273a 2073 636e 5f6d 6f64  SCNMOD': scn_mod
-000077e0: 2c20 2752 5244 5245 4e27 3a20 7272 6472  , 'RRDREN': rrdr
-000077f0: 5f65 6e2c 2027 4752 4445 4e41 273a 2067  _en, 'GRDENA': g
-00007800: 7264 5f65 6e61 2c0a 2020 2020 2020 2020  rd_ena,.        
-00007810: 2020 2020 2020 2020 2020 2747 5244 4455            'GRDDU
-00007820: 5227 3a20 6772 645f 6475 722c 0a20 2020  R': grd_dur,.   
-00007830: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00007840: 5057 4245 4e41 273a 2070 7762 5f65 6e61  PWBENA': pwb_ena
-00007850: 2c20 274f 5254 5345 5427 3a20 7469 6d65  , 'ORTSET': time
-00007860: 5f6f 7574 7d0a 2020 2020 2020 2020 7061  _out}.        pa
-00007870: 7261 6d73 203d 205b 6b65 7920 2b20 7661  rams = [key + va
-00007880: 6c75 6520 666f 7220 6b65 792c 2076 616c  lue for key, val
-00007890: 7565 2069 6e20 7061 7261 6d73 2e69 7465  ue in params.ite
-000078a0: 6d73 2829 5d0a 0a20 2020 2020 2020 2069  ms()]..        i
-000078b0: 6620 7379 6d62 6f6c 6f67 6965 7320 6973  f symbologies is
-000078c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000078d0: 2020 2020 2020 2066 6f72 2073 796d 626f         for symbo
-000078e0: 6c6f 6779 2069 6e20 7379 6d62 6f6c 6f67  logy in symbolog
-000078f0: 6965 733a 0a20 2020 2020 2020 2020 2020  ies:.           
-00007900: 2020 2020 2070 6172 616d 732e 6170 7065       params.appe
-00007910: 6e64 2827 5359 4d42 5f27 202b 2073 796d  nd('SYMB_' + sym
-00007920: 626f 6c6f 6779 202b 2027 3127 290a 0a20  bology + '1').. 
-00007930: 2020 2020 2020 2074 2c20 6973 5375 6363         t, isSucc
-00007940: 6573 7320 3d20 7365 6c66 2e6d 616e 7561  ess = self.manua
-00007950: 6c5f 636f 6e66 6967 7572 6528 7061 7261  l_configure(para
-00007960: 6d73 290a 2020 2020 2020 2020 6966 2069  ms).        if i
-00007970: 7353 7563 6365 7373 2061 6e64 2073 656c  sSuccess and sel
-00007980: 662e 6c6f 675f 7479 7065 2021 3d20 274e  f.log_type != 'N
-00007990: 4f5f 4c4f 4727 3a0a 2020 2020 2020 2020  O_LOG':.        
-000079a0: 2020 2020 7365 6c66 2e71 725f 6c6f 6767      self.qr_logg
-000079b0: 6572 2e69 6e66 6f28 6627 4261 7263 6f64  er.info(f'Barcod
-000079c0: 6520 7363 616e 6e65 7220 287b 7365 6c66  e scanner ({self
-000079d0: 2e63 6f6d 5f70 6f72 747d 2920 636f 6e66  .com_port}) conf
-000079e0: 6967 7572 6564 2073 7563 6365 7373 6675  igured successfu
-000079f0: 6c6c 792e 2729 0a20 2020 2020 2020 2065  lly.').        e
-00007a00: 6c69 6620 6e6f 7420 6973 5375 6363 6573  lif not isSucces
-00007a10: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00007a20: 656c 662e 7172 5f6c 6f67 6765 722e 6572  elf.qr_logger.er
-00007a30: 726f 7228 6627 4261 7263 6f64 6520 7363  ror(f'Barcode sc
-00007a40: 616e 6e65 7220 287b 7365 6c66 2e63 6f6d  anner ({self.com
-00007a50: 5f70 6f72 747d 2920 636f 6e66 6967 7572  _port}) configur
-00007a60: 6174 696f 6e20 6661 696c 6564 2e27 290a  ation failed.').
-00007a70: 0a20 2020 2064 6566 2072 6573 746f 7265  .    def restore
-00007a80: 5f61 6c6c 5f66 6163 746f 7279 5f64 6566  _all_factory_def
-00007a90: 6175 6c74 7328 7365 6c66 293a 0a20 2020  aults(self):.   
-00007aa0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00007ab0: 2052 6573 746f 7265 2061 6c6c 2066 6163   Restore all fac
-00007ac0: 746f 7279 2064 6566 6175 6c74 732e 0a20  tory defaults.. 
-00007ad0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007ae0: 2020 2073 6c65 6570 2830 2e31 290a 2020     sleep(0.1).  
-00007af0: 2020 2020 2020 7061 7261 6d73 203d 207b        params = {
-00007b00: 2746 4143 4445 4627 3a20 2727 7d0a 2020  'FACDEF': ''}.  
-00007b10: 2020 2020 2020 7061 7261 6d73 203d 205b        params = [
-00007b20: 6b65 7920 2b20 7661 6c75 6520 666f 7220  key + value for 
-00007b30: 6b65 792c 2076 616c 7565 2069 6e20 7061  key, value in pa
-00007b40: 7261 6d73 2e69 7465 6d73 2829 5d0a 2020  rams.items()].  
-00007b50: 2020 2020 2020 742c 2069 7353 7563 6365        t, isSucce
-00007b60: 7373 203d 2073 656c 662e 6d61 6e75 616c  ss = self.manual
-00007b70: 5f63 6f6e 6669 6775 7265 2870 6172 616d  _configure(param
-00007b80: 7329 0a20 2020 2020 2020 2069 6620 6973  s).        if is
-00007b90: 5375 6363 6573 7320 616e 6420 7365 6c66  Success and self
-00007ba0: 2e6c 6f67 5f74 7970 6520 213d 2027 4e4f  .log_type != 'NO
-00007bb0: 5f4c 4f47 273a 0a20 2020 2020 2020 2020  _LOG':.         
-00007bc0: 2020 2073 656c 662e 7172 5f6c 6f67 6765     self.qr_logge
-00007bd0: 722e 696e 666f 2866 2742 6172 636f 6465  r.info(f'Barcode
-00007be0: 2073 6361 6e6e 6572 2028 7b73 656c 662e   scanner ({self.
-00007bf0: 636f 6d5f 706f 7274 7d29 2072 6573 746f  com_port}) resto
-00007c00: 7265 6420 6661 6374 6f72 7920 6465 6661  red factory defa
-00007c10: 756c 7420 7375 6363 6573 7366 756c 6c79  ult successfully
-00007c20: 2e27 290a 2020 2020 2020 2020 656c 6966  .').        elif
-00007c30: 206e 6f74 2069 7353 7563 6365 7373 3a0a   not isSuccess:.
-00007c40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007c50: 2e71 725f 6c6f 6767 6572 2e65 7272 6f72  .qr_logger.error
-00007c60: 2866 2742 6172 636f 6465 2073 6361 6e6e  (f'Barcode scann
-00007c70: 6572 2028 7b73 656c 662e 636f 6d5f 706f  er ({self.com_po
-00007c80: 7274 7d29 2072 6573 746f 7265 6420 6661  rt}) restored fa
-00007c90: 6374 6f72 7920 6465 6661 756c 7420 6661  ctory default fa
-00007ca0: 696c 6564 2e27 290a 0a20 2020 2064 6566  iled.')..    def
-00007cb0: 206d 616e 7561 6c5f 636f 6e66 6967 7572   manual_configur
-00007cc0: 6528 7365 6c66 2c20 7061 7261 6d73 293a  e(self, params):
-00007cd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007ce0: 2020 2020 204d 616e 7561 6c6c 7920 636f       Manually co
-00007cf0: 6e66 6967 7572 6520 7468 6520 7363 616e  nfigure the scan
-00007d00: 6e65 722e 0a20 2020 2020 2020 2022 2222  ner..        """
-00007d10: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00007d20: 7269 616c 5f63 6f6e 6e65 6374 696f 6e2e  rial_connection.
-00007d30: 666c 7573 6849 6e70 7574 2829 0a20 2020  flushInput().   
-00007d40: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
-00007d50: 5f63 6f6e 6e65 6374 696f 6e2e 666c 7573  _connection.flus
-00007d60: 684f 7574 7075 7428 290a 2020 2020 2020  hOutput().      
-00007d70: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
-00007d80: 2020 2020 2062 6164 5f6d 7367 203d 2027       bad_msg = '
-00007d90: 3436 3064 3061 2720 2023 2034 3620 3d20  460d0a'  # 46 = 
-00007da0: 462c 2023 3064 203d 202f 7220 2330 6120  F, #0d = /r #0a 
-00007db0: 3d20 2f6e 202d 3e20 6d65 616e 7320 7468  = /n -> means th
-00007dc0: 6174 2065 7665 7279 2065 7272 6f72 206f  at every error o
-00007dd0: 7220 6465 636f 6e64 696e 6720 7469 6d65  r deconding time
-00007de0: 6f75 7420 7769 6c6c 2073 656e 6420 7468  out will send th
-00007df0: 6520 6d65 7373 6167 6520 462f 722f 6e20  e message F/r/n 
-00007e00: 2d3e 2077 696c 6c20 6265 2074 7261 6e73  -> will be trans
-00007e10: 6c61 7465 6420 6279 2073 6572 6961 6c20  lated by serial 
-00007e20: 6c69 6220 6173 2046 3c4e 6577 4c69 6e65  lib as F<NewLine
-00007e30: 3e0a 2020 2020 2020 2020 656e 7465 725f  >.        enter_
-00007e40: 7365 7475 705f 6d6f 6465 203d 2027 5345  setup_mode = 'SE
-00007e50: 5455 5045 3127 0a20 2020 2020 2020 2065  TUPE1'.        e
-00007e60: 7869 745f 7365 7475 705f 6d6f 6465 203d  xit_setup_mode =
-00007e70: 2027 5345 5455 5045 3027 0a20 2020 2020   'SETUPE0'.     
-00007e80: 2020 2023 2045 6e74 6572 2073 6574 7570     # Enter setup
-00007e90: 206d 6f64 650a 2020 2020 2020 2020 7365   mode.        se
-00007ea0: 6c66 2e73 6572 6961 6c5f 636f 6e6e 6563  lf.serial_connec
-00007eb0: 7469 6f6e 2e77 7269 7465 2873 7472 2e65  tion.write(str.e
-00007ec0: 6e63 6f64 6528 7365 6c66 2e70 7265 6669  ncode(self.prefi
-00007ed0: 7820 2b20 656e 7465 725f 7365 7475 705f  x + enter_setup_
-00007ee0: 6d6f 6465 202b 2073 656c 662e 7375 6666  mode + self.suff
-00007ef0: 6978 2929 0a20 2020 2020 2020 2023 2049  ix)).        # I
-00007f00: 6e73 6572 7420 636f 6e66 6967 7572 6174  nsert configurat
-00007f10: 696f 6e0a 2020 2020 2020 2020 636f 6e66  ion.        conf
-00007f20: 6967 7320 3d20 7365 6c66 2e70 7265 6669  igs = self.prefi
-00007f30: 7820 2b20 273b 272e 6a6f 696e 2870 6172  x + ';'.join(par
-00007f40: 616d 7329 202b 2073 656c 662e 7375 6666  ams) + self.suff
-00007f50: 6978 0a20 2020 2020 2020 2073 656c 662e  ix.        self.
-00007f60: 7365 7269 616c 5f63 6f6e 6e65 6374 696f  serial_connectio
-00007f70: 6e2e 7772 6974 6528 7374 722e 656e 636f  n.write(str.enco
-00007f80: 6465 2863 6f6e 6669 6773 2929 0a20 2020  de(configs)).   
-00007f90: 2020 2020 2069 6620 274e 4752 454e 4131       if 'NGRENA1
-00007fa0: 2720 696e 2070 6172 616d 733a 0a20 2020  ' in params:.   
-00007fb0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00007fc0: 7269 616c 5f63 6f6e 6e65 6374 696f 6e2e  rial_connection.
-00007fd0: 7772 6974 6528 0a20 2020 2020 2020 2020  write(.         
-00007fe0: 2020 2020 2020 2073 7472 2e65 6e63 6f64         str.encod
-00007ff0: 6528 7365 6c66 2e70 7265 6669 7820 2b20  e(self.prefix + 
-00008000: 274e 4752 5345 5427 202b 2062 6164 5f6d  'NGRSET' + bad_m
-00008010: 7367 202b 2073 656c 662e 7375 6666 6978  sg + self.suffix
-00008020: 2929 2020 2320 5365 7420 6d65 7373 6167  ))  # Set messag
-00008030: 6520 746f 2065 6d70 7479 0a20 2020 2020  e to empty.     
-00008040: 2020 2069 6620 2753 434e 4d4f 4432 2720     if 'SCNMOD2' 
-00008050: 696e 2070 6172 616d 733a 0a20 2020 2020  in params:.     
-00008060: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
-00008070: 616c 5f63 6f6e 6e65 6374 696f 6e2e 7772  al_connection.wr
-00008080: 6974 6528 0a20 2020 2020 2020 2020 2020  ite(.           
-00008090: 2020 2020 2073 7472 2e65 6e63 6f64 6528       str.encode(
-000080a0: 7365 6c66 2e70 7265 6669 7820 2b20 2753  self.prefix + 'S
-000080b0: 454e 4c56 4c35 2720 2b20 6261 645f 6d73  ENLVL5' + bad_ms
-000080c0: 6720 2b20 7365 6c66 2e73 7566 6669 7829  g + self.suffix)
-000080d0: 2920 2023 2053 6574 2073 656e 7369 7469  )  # Set sensiti
-000080e0: 7669 7479 2074 6f20 6869 6768 2031 2d32  vity to high 1-2
-000080f0: 300a 2020 2020 2020 2020 2320 4578 6974  0.        # Exit
-00008100: 2073 6574 7570 206d 6f64 650a 2020 2020   setup mode.    
-00008110: 2020 2020 7365 6c66 2e73 6572 6961 6c5f      self.serial_
-00008120: 636f 6e6e 6563 7469 6f6e 2e77 7269 7465  connection.write
-00008130: 2873 7472 2e65 6e63 6f64 6528 7365 6c66  (str.encode(self
-00008140: 2e70 7265 6669 7820 2b20 6578 6974 5f73  .prefix + exit_s
-00008150: 6574 7570 5f6d 6f64 6520 2b20 7365 6c66  etup_mode + self
-00008160: 2e73 7566 6669 7829 290a 2020 2020 2020  .suffix)).      
-00008170: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
-00008180: 2020 2020 2074 2c20 6973 5375 6363 6573       t, isSucces
-00008190: 7320 3d20 7365 6c66 2e74 7269 6767 6572  s = self.trigger
-000081a0: 5f73 746f 705f 7365 7474 696e 6773 2829  _stop_settings()
-000081b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000081c0: 742c 2069 7353 7563 6365 7373 0a0a 2020  t, isSuccess..  
-000081d0: 2020 6465 6620 7363 616e 2873 656c 6629    def scan(self)
-000081e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000081f0: 2020 2020 2020 5363 616e 2074 6865 2051        Scan the Q
-00008200: 5220 636f 6465 2e0a 2020 2020 2020 2020  R code..        
-00008210: 2222 220a 2020 2020 2020 2020 7420 3d20  """.        t = 
-00008220: 4e6f 6e65 0a20 2020 2020 2020 2074 7279  None.        try
-00008230: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008240: 6c66 2e73 6572 6961 6c5f 636f 6e6e 6563  lf.serial_connec
-00008250: 7469 6f6e 2e77 7269 7465 2862 225c 7831  tion.write(b"\x1
-00008260: 625c 7833 3122 290a 2020 2020 2020 2020  b\x31").        
-00008270: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00008280: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00008290: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
-000082a0: 6f6e 2866 2753 6361 6e6e 6572 3a20 4572  on(f'Scanner: Er
-000082b0: 726f 7220 7365 6e64 696e 6720 6d65 7373  ror sending mess
-000082c0: 6167 6520 7468 726f 7567 6820 5541 5254  age through UART
-000082d0: 2d20 4368 6563 6b20 636f 6e6e 6563 7469  - Check connecti
-000082e0: 6f6e 207b 657d 2729 0a20 2020 2020 2020  on {e}').       
-000082f0: 2073 7461 7274 5f74 696d 6520 3d20 6461   start_time = da
-00008300: 7465 7469 6d65 2e6e 6f77 2829 0a20 2020  tetime.now().   
-00008310: 2020 2020 2074 203d 2073 656c 662e 7365       t = self.se
-00008320: 7269 616c 5f63 6f6e 6e65 6374 696f 6e2e  rial_connection.
-00008330: 7265 6164 6c69 6e65 2829 0a20 2020 2020  readline().     
-00008340: 2020 2065 6e64 5f74 696d 6520 3d20 6461     end_time = da
-00008350: 7465 7469 6d65 2e6e 6f77 2829 0a20 2020  tetime.now().   
-00008360: 2020 2020 2065 6c61 7073 6564 5f74 696d       elapsed_tim
-00008370: 655f 6d73 203d 2028 656e 645f 7469 6d65  e_ms = (end_time
-00008380: 202d 2073 7461 7274 5f74 696d 6529 2e74   - start_time).t
-00008390: 6f74 616c 5f73 6563 6f6e 6473 2829 202a  otal_seconds() *
-000083a0: 2031 3030 300a 2020 2020 2020 2020 7265   1000.        re
-000083b0: 7475 726e 2074 2c20 656c 6170 7365 645f  turn t, elapsed_
-000083c0: 7469 6d65 5f6d 730a 0a20 2020 2064 6566  time_ms..    def
-000083d0: 2073 6361 6e5f 616e 645f 666c 7573 6828   scan_and_flush(
-000083e0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000083f0: 2222 0a20 2020 2020 2020 2053 6361 6e20  "".        Scan 
-00008400: 7468 6520 5152 2063 6f64 6520 616e 6420  the QR code and 
-00008410: 666c 7573 6820 7468 6520 6275 6666 6572  flush the buffer
-00008420: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00008430: 2020 2020 2020 6465 6620 636c 6561 6e5f        def clean_
-00008440: 7363 616e 5f66 2869 6e70 7574 5f73 6361  scan_f(input_sca
-00008450: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-00008460: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00008470: 2020 2020 2064 6563 6f64 6564 5f73 6361       decoded_sca
-00008480: 6e20 3d20 696e 7075 745f 7363 616e 2e64  n = input_scan.d
-00008490: 6563 6f64 6528 290a 2020 2020 2020 2020  ecode().        
-000084a0: 2020 2020 2020 2020 7374 7269 7070 6564          stripped
-000084b0: 5f73 6361 6e20 3d20 6465 636f 6465 645f  _scan = decoded_
-000084c0: 7363 616e 2e73 7472 6970 2829 0a20 2020  scan.strip().   
-000084d0: 2020 2020 2020 2020 2020 2020 2063 6c65               cle
-000084e0: 616e 5f73 7472 203d 2073 7472 6970 7065  an_str = strippe
-000084f0: 645f 7363 616e 2e72 6570 6c61 6365 2827  d_scan.replace('
-00008500: 5c72 5c6e 272c 2027 2729 2e72 6570 6c61  \r\n', '').repla
-00008510: 6365 2827 5c78 3036 272c 2027 2729 2e72  ce('\x06', '').r
-00008520: 6570 6c61 6365 2827 5c78 3031 272c 2027  eplace('\x01', '
-00008530: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00008540: 2020 2072 6574 7572 6e20 636c 6561 6e5f     return clean_
-00008550: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-00008560: 6578 6365 7074 2055 6e69 636f 6465 4465  except UnicodeDe
-00008570: 636f 6465 4572 726f 723a 0a20 2020 2020  codeError:.     
-00008580: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008590: 6e20 4e6f 6e65 0a0a 2020 2020 2020 2020  n None..        
-000085a0: 6966 2073 656c 662e 7365 7269 616c 5f63  if self.serial_c
-000085b0: 6f6e 6e65 6374 696f 6e20 6973 204e 6f6e  onnection is Non
-000085c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000085d0: 656c 662e 7172 5f6c 6f67 6765 722e 6572  elf.qr_logger.er
-000085e0: 726f 7228 2245 7272 6f72 3a20 5365 7269  ror("Error: Seri
-000085f0: 616c 206f 626a 6563 7420 6e6f 7420 696e  al object not in
-00008600: 6974 6961 6c69 7a65 6422 290a 2020 2020  itialized").    
-00008610: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00008620: 6f6e 650a 0a20 2020 2020 2020 2073 6361  one..        sca
-00008630: 6e6e 6564 2c20 656c 6170 7365 645f 7469  nned, elapsed_ti
-00008640: 6d65 5f6d 7320 3d20 7365 6c66 2e73 6361  me_ms = self.sca
-00008650: 6e28 290a 0a20 2020 2020 2020 2069 6620  n()..        if 
-00008660: 7363 616e 6e65 643a 0a20 2020 2020 2020  scanned:.       
-00008670: 2020 2020 2063 6c65 616e 5f73 6361 6e20       clean_scan 
-00008680: 3d20 636c 6561 6e5f 7363 616e 5f66 2873  = clean_scan_f(s
-00008690: 6361 6e6e 6564 290a 2020 2020 2020 2020  canned).        
-000086a0: 2020 2020 6966 2063 6c65 616e 5f73 6361      if clean_sca
-000086b0: 6e20 3d3d 2027 4627 3a0a 2020 2020 2020  n == 'F':.      
-000086c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000086d0: 204e 6f6e 652c 2065 6c61 7073 6564 5f74   None, elapsed_t
-000086e0: 696d 655f 6d73 0a20 2020 2020 2020 2020  ime_ms.         
-000086f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00008700: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008710: 636c 6561 6e5f 7363 616e 2c20 656c 6170  clean_scan, elap
-00008720: 7365 645f 7469 6d65 5f6d 730a 0a20 2020  sed_time_ms..   
-00008730: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008740: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00008750: 735f 6f70 656e 2829 3a0a 2020 2020 2020  s_open():.      
-00008760: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00008770: 6572 6961 6c5f 636f 6e6e 6563 7469 6f6e  erial_connection
-00008780: 2e72 6573 6574 5f69 6e70 7574 5f62 7566  .reset_input_buf
-00008790: 6665 7228 290a 2020 2020 2020 2020 2020  fer().          
-000087a0: 2020 2020 2020 7365 6c66 2e73 6572 6961        self.seria
-000087b0: 6c5f 636f 6e6e 6563 7469 6f6e 2e72 6573  l_connection.res
-000087c0: 6574 5f6f 7574 7075 745f 6275 6666 6572  et_output_buffer
-000087d0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000087e0: 2020 2073 6c65 6570 2830 2e31 290a 2020     sleep(0.1).  
-000087f0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00008800: 616e 6e65 642c 2065 6c61 7073 6564 5f74  anned, elapsed_t
-00008810: 696d 655f 6d73 203d 2073 656c 662e 7363  ime_ms = self.sc
-00008820: 616e 2829 0a20 2020 2020 2020 2020 2020  an().           
-00008830: 2020 2020 2069 6620 7363 616e 6e65 643a       if scanned:
-00008840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008850: 2020 2020 2063 6c65 616e 5f73 6361 6e20       clean_scan 
-00008860: 3d20 636c 6561 6e5f 7363 616e 5f66 2873  = clean_scan_f(s
-00008870: 6361 6e6e 6564 290a 2020 2020 2020 2020  canned).        
-00008880: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00008890: 6c65 616e 5f73 6361 6e20 3d3d 2027 4627  lean_scan == 'F'
-000088a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000088b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000088c0: 204e 6f6e 652c 2065 6c61 7073 6564 5f74   None, elapsed_t
-000088d0: 696d 655f 6d73 0a20 2020 2020 2020 2020  ime_ms.         
-000088e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000088f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008900: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008910: 636c 6561 6e5f 7363 616e 2c20 656c 6170  clean_scan, elap
-00008920: 7365 645f 7469 6d65 5f6d 730a 2020 2020  sed_time_ms.    
-00008930: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00008940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008950: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
-00008960: 7074 696f 6e28 2745 7272 6f72 2072 6561  ption('Error rea
-00008970: 6469 6e67 2062 6172 636f 6465 2064 6174  ding barcode dat
-00008980: 6120 2d20 5365 7269 616c 2070 726f 626c  a - Serial probl
-00008990: 656d 2729 0a20 2020 2020 2020 2020 2020  em').           
-000089a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000089b0: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
-000089c0: 6570 7469 6f6e 2827 4572 726f 7220 696e  eption('Error in
-000089d0: 2053 6361 6e6e 6572 2053 6572 6961 6c20   Scanner Serial 
-000089e0: 636f 6e6e 6563 7469 6f6e 2729 0a0a 2020  connection')..  
-000089f0: 2020 6465 6620 7363 616e 5f65 7874 5f69    def scan_ext_i
-00008a00: 6428 7365 6c66 2c20 6e65 6564 5f74 6f5f  d(self, need_to_
-00008a10: 7472 6967 6765 723d 5472 7565 293a 0a20  trigger=True):. 
-00008a20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00008a30: 2020 2053 6361 6e20 7468 6520 6578 7465     Scan the exte
-00008a40: 726e 616c 2049 442e 0a20 2020 2020 2020  rnal ID..       
-00008a50: 2040 7061 7261 6d20 6e65 6564 5f74 6f5f   @param need_to_
-00008a60: 7472 6967 6765 7220 746f 206b 6565 7020  trigger to keep 
-00008a70: 7361 6d65 2062 6568 6176 696f 7220 6173  same behavior as
-00008a80: 2074 6865 2043 6f67 6e65 780a 2020 2020   the Cognex.    
-00008a90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008aa0: 6261 7263 6f64 655f 7265 6164 203d 2027  barcode_read = '
-00008ab0: 270a 2020 2020 2020 2020 7374 6172 745f  '.        start_
-00008ac0: 7469 6d65 203d 2074 696d 6528 290a 2020  time = time().  
-00008ad0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00008ae0: 2020 2020 2020 2062 6172 636f 6465 5f72         barcode_r
-00008af0: 6561 642c 2065 6c61 7073 6564 5f74 696d  ead, elapsed_tim
-00008b00: 655f 6d73 203d 2073 656c 662e 7363 616e  e_ms = self.scan
-00008b10: 5f61 6e64 5f66 6c75 7368 2829 0a20 2020  _and_flush().   
-00008b20: 2020 2020 2020 2020 2069 6620 6261 7263           if barc
-00008b30: 6f64 655f 7265 6164 2069 7320 4e6f 6e65  ode_read is None
-00008b40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008b50: 2020 7265 7475 726e 204e 6f6e 652c 204e    return None, N
-00008b60: 6f6e 652c 204e 6f6e 652c 204e 6f6e 650a  one, None, None.
-00008b70: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00008b80: 2062 6172 636f 6465 5f72 6561 6420 3d3d   barcode_read ==
-00008b90: 2027 273a 0a20 2020 2020 2020 2020 2020   '':.           
-00008ba0: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00008bb0: 7469 6f6e 2827 4572 726f 7220 696e 2053  tion('Error in S
-00008bc0: 6361 6e6e 6572 2053 6572 6961 6c20 636f  canner Serial co
-00008bd0: 6e6e 6563 7469 6f6e 2729 0a20 2020 2020  nnection').     
-00008be0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00008bf0: 2020 2020 2020 2020 2020 2020 2066 756c               ful
-00008c00: 6c5f 6461 7461 2c20 6375 725f 6964 2c20  l_data, cur_id, 
-00008c10: 7265 656c 5f69 642c 2067 7469 6e20 3d20  reel_id, gtin = 
-00008c20: 7365 6c66 2e72 6561 645f 6261 7263 6f64  self.read_barcod
-00008c30: 6528 6261 7263 6f64 655f 7265 6164 290a  e(barcode_read).
-00008c40: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00008c50: 656c 662e 7772 6974 655f 746f 5f6c 6f67  elf.write_to_log
-00008c60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008c70: 2020 7769 7468 206f 7065 6e28 7365 6c66    with open(self
-00008c80: 2e6c 6f67 5f66 696c 656e 616d 652c 2027  .log_filename, '
-00008c90: 6127 2920 6173 2066 3a0a 2020 2020 2020  a') as f:.      
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00008cb0: 6d65 7374 616d 7020 3d20 6461 7465 7469  mestamp = dateti
-00008cc0: 6d65 2e6e 6f77 2829 2e73 7472 6674 696d  me.now().strftim
-00008cd0: 6528 2225 592d 256d 2d25 6420 2548 3a25  e("%Y-%m-%d %H:%
-00008ce0: 4d3a 2553 2229 0a20 2020 2020 2020 2020  M:%S").         
-00008cf0: 2020 2020 2020 2020 2020 206c 6f67 5f6d             log_m
-00008d00: 6573 7361 6765 203d 2066 227b 7469 6d65  essage = f"{time
-00008d10: 7374 616d 707d 202d 207b 6675 6c6c 5f64  stamp} - {full_d
-00008d20: 6174 617d 202d 2045 6c61 7073 6564 2054  ata} - Elapsed T
-00008d30: 696d 653a 207b 656c 6170 7365 645f 7469  ime: {elapsed_ti
-00008d40: 6d65 5f6d 733a 2e32 667d 206d 735c 6e22  me_ms:.2f} ms\n"
-00008d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008d60: 2020 2020 2066 2e77 7269 7465 286c 6f67       f.write(log
-00008d70: 5f6d 6573 7361 6765 290a 0a20 2020 2020  _message)..     
-00008d80: 2020 2020 2020 2072 6574 7572 6e20 6675         return fu
-00008d90: 6c6c 5f64 6174 612c 2063 7572 5f69 642c  ll_data, cur_id,
-00008da0: 2072 6565 6c5f 6964 2c20 6774 696e 0a20   reel_id, gtin. 
-00008db0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00008dc0: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
-00008dd0: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
-00008de0: 725f 6c6f 6767 6572 2e65 7272 6f72 2866  r_logger.error(f
-00008df0: 277b 657d 202d 2043 6865 636b 2063 6f6e  '{e} - Check con
-00008e00: 6e65 6374 696f 6e27 290a 2020 2020 2020  nection').      
-00008e10: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
-00008e20: 7074 696f 6e28 6627 7b65 7d20 2d20 4368  ption(f'{e} - Ch
-00008e30: 6563 6b20 636f 6e6e 6563 7469 6f6e 2729  eck connection')
-00008e40: 0a0a 2020 2020 6465 6620 7265 6164 5f62  ..    def read_b
-00008e50: 6172 636f 6465 2873 656c 662c 2062 6172  arcode(self, bar
-00008e60: 636f 6465 5f72 6561 6429 3a0a 2020 2020  code_read):.    
-00008e70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008e80: 5265 6164 2074 6865 2062 6172 636f 6465  Read the barcode
-00008e90: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00008ea0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00008eb0: 2020 2020 2020 2069 6620 2728 3031 2927         if '(01)'
-00008ec0: 2069 6e20 6261 7263 6f64 655f 7265 6164   in barcode_read
-00008ed0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008ee0: 2020 6261 7263 6f64 6573 203d 2062 6172    barcodes = bar
-00008ef0: 636f 6465 5f72 6561 642e 7370 6c69 7428  code_read.split(
-00008f00: 2228 3031 2922 290a 2020 2020 2020 2020  "(01)").        
-00008f10: 2020 2020 2020 2020 666f 7220 692c 2073          for i, s
-00008f20: 696e 676c 655f 6261 7263 6f64 6520 696e  ingle_barcode in
-00008f30: 2065 6e75 6d65 7261 7465 2862 6172 636f   enumerate(barco
-00008f40: 6465 735b 313a 5d2c 2031 293a 0a20 2020  des[1:], 1):.   
-00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f60: 2066 756c 6c5f 6461 7461 203d 2066 2228   full_data = f"(
-00008f70: 3031 297b 7369 6e67 6c65 5f62 6172 636f  01){single_barco
-00008f80: 6465 7d22 0a20 2020 2020 2020 2020 2020  de}".           
-00008f90: 2020 2020 2020 2020 2067 7469 6e20 3d20           gtin = 
-00008fa0: 2729 272e 6a6f 696e 2866 756c 6c5f 6461  ')'.join(full_da
-00008fb0: 7461 2e73 706c 6974 2827 2927 295b 3a32  ta.split(')')[:2
-00008fc0: 5d29 202b 2027 2927 0a20 2020 2020 2020  ]) + ')'.       
-00008fd0: 2020 2020 2020 2020 2020 2020 2074 6167               tag
-00008fe0: 5f64 6174 6120 3d20 6675 6c6c 5f64 6174  _data = full_dat
-00008ff0: 612e 7370 6c69 7428 2729 2729 5b32 5d0a  a.split(')')[2].
-00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009010: 2020 2020 6375 725f 6964 203d 2074 6167      cur_id = tag
-00009020: 5f64 6174 612e 7370 6c69 7428 2754 2729  _data.split('T')
-00009030: 5b31 5d2e 7374 7269 7028 2227 2022 292e  [1].strip("' ").
-00009040: 7370 6c69 7428 2728 2729 5b30 5d0a 2020  split('(')[0].  
-00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009060: 2020 7265 656c 5f69 6420 3d20 7461 675f    reel_id = tag_
-00009070: 6461 7461 2e73 706c 6974 2827 5427 295b  data.split('T')[
-00009080: 305d 2e73 7472 6970 2822 2720 2229 0a0a  0].strip("' ")..
-00009090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090a0: 2020 2020 6966 2066 756c 6c5f 6461 7461      if full_data
-000090b0: 2061 6e64 2063 7572 5f69 6420 616e 6420   and cur_id and 
-000090c0: 7265 656c 5f69 6420 616e 6420 6774 696e  reel_id and gtin
-000090d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000090e0: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
-000090f0: 725f 6c6f 6767 6572 2e69 6e66 6f28 0a20  r_logger.info(. 
-00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009110: 2020 2020 2020 2020 2020 2066 2757 696c             f'Wil
-00009120: 696f 7420 5152 2064 6574 6563 7465 6420  iot QR detected 
-00009130: 4754 696e 3a20 7b67 7469 6e7d 2c20 5265  GTin: {gtin}, Re
-00009140: 656c 3a20 7b72 6565 6c5f 6964 7d2c 2049  el: {reel_id}, I
-00009150: 443a 7b63 7572 5f69 647d 2729 0a20 2020  D:{cur_id}').   
-00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009170: 2020 2020 2072 6574 7572 6e20 6675 6c6c       return full
-00009180: 5f64 6174 612c 2063 7572 5f69 642c 2072  _data, cur_id, r
-00009190: 6565 6c5f 6964 2c20 6774 696e 0a20 2020  eel_id, gtin.   
-000091a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000091b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000091c0: 756c 6c5f 6461 7461 203d 2063 7572 5f69  ull_data = cur_i
-000091d0: 6420 3d20 7265 656c 5f69 6420 3d20 6774  d = reel_id = gt
-000091e0: 696e 203d 2062 6172 636f 6465 5f72 6561  in = barcode_rea
-000091f0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00009200: 2020 6774 696e 5f76 616c 203d 2054 7275    gtin_val = Tru
-00009210: 6520 6966 206c 656e 2866 756c 6c5f 6461  e if len(full_da
-00009220: 7461 2920 3d3d 2073 656c 662e 7367 7469  ta) == self.sgti
-00009230: 6e5f 6c65 6e67 7468 2065 6c73 6520 4661  n_length else Fa
-00009240: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00009250: 2020 2020 6966 2067 7469 6e5f 7661 6c3a      if gtin_val:
-00009260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009270: 2020 2020 2063 7572 5f69 6420 3d20 6675       cur_id = fu
-00009280: 6c6c 5f64 6174 612e 7370 6c69 7428 2754  ll_data.split('T
-00009290: 2729 5b31 5d2e 7374 7269 7028 2227 2022  ')[1].strip("' "
-000092a0: 292e 7370 6c69 7428 2728 2729 5b30 5d0a  ).split('(')[0].
-000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092c0: 2020 2020 7265 656c 5f69 6420 3d20 6675      reel_id = fu
-000092d0: 6c6c 5f64 6174 612e 7370 6c69 7428 2754  ll_data.split('T
-000092e0: 2729 5b30 5d2e 7374 7269 7028 2227 2022  ')[0].strip("' "
-000092f0: 295b 2d34 3a5d 0a20 2020 2020 2020 2020  )[-4:].         
-00009300: 2020 2020 2020 2020 2020 2067 7469 6e20             gtin 
-00009310: 3d20 6675 6c6c 5f64 6174 612e 7370 6c69  = full_data.spli
-00009320: 7428 2754 2729 5b30 5d2e 7374 7269 7028  t('T')[0].strip(
-00009330: 2227 2022 295b 3a2d 345d 0a20 2020 2020  "' ")[:-4].     
-00009340: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00009350: 656c 662e 7172 5f6c 6f67 6765 722e 696e  elf.qr_logger.in
-00009360: 666f 2827 5769 6c69 6f74 2051 5220 6465  fo('Wiliot QR de
-00009370: 7465 6374 6564 2047 5469 6e3a 207b 7d2c  tected GTin: {},
-00009380: 2052 6565 6c3a 207b 7d2c 2049 443a 7b7d   Reel: {}, ID:{}
-00009390: 272e 666f 726d 6174 2867 7469 6e2c 2063  '.format(gtin, c
-000093a0: 7572 5f69 642c 2072 6565 6c5f 6964 2929  ur_id, reel_id))
-000093b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000093c0: 2020 2020 2072 6574 7572 6e20 6675 6c6c       return full
-000093d0: 5f64 6174 612c 2063 7572 5f69 642c 2072  _data, cur_id, r
-000093e0: 6565 6c5f 6964 2c20 6774 696e 0a20 2020  eel_id, gtin.   
-000093f0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00009400: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00009410: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00009420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009430: 2020 2020 6966 2066 756c 6c5f 6461 7461      if full_data
-00009440: 203d 3d20 2746 273a 0a20 2020 2020 2020   == 'F':.       
-00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009460: 2020 2020 2073 656c 662e 7172 5f6c 6f67       self.qr_log
-00009470: 6765 722e 696e 666f 2827 4e6f 2062 6172  ger.info('No bar
-00009480: 636f 6465 2064 6574 6563 7465 6420 2d20  code detected - 
-00009490: 4465 636f 6469 6e67 2074 696d 656f 7574  Decoding timeout
-000094a0: 2072 6561 6368 6564 2729 0a20 2020 2020   reached').     
-000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-000094d0: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  ne, None, None, 
-000094e0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-000094f0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00009500: 6620 6675 6c6c 5f64 6174 6120 3d3d 2027  f full_data == '
-00009510: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00009520: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009530: 6169 7365 2045 7863 6570 7469 6f6e 2827  aise Exception('
-00009540: 5072 6f62 6c65 6d20 7769 7468 2062 6172  Problem with bar
-00009550: 636f 6465 2073 6361 6e6e 6572 2729 0a20  code scanner'). 
-00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009570: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00009580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009590: 2020 2020 2020 2020 2063 7572 5f69 6420           cur_id 
-000095a0: 3d20 6675 6c6c 5f64 6174 612e 7370 6c69  = full_data.spli
-000095b0: 7428 2754 2729 5b31 5d0a 2020 2020 2020  t('T')[1].      
-000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095d0: 2020 2020 2020 7265 656c 5f69 6420 3d20        reel_id = 
-000095e0: 6675 6c6c 5f64 6174 612e 7370 6c69 7428  full_data.split(
-000095f0: 2754 2729 5b30 5d0a 2020 2020 2020 2020  'T')[0].        
-00009600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009610: 2020 2020 6774 696e 203d 2027 270a 2020      gtin = ''.  
+00004a30: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00004a40: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00004a50: 656c 662e 6d6f 6465 6c20 696e 2073 656c  elf.model in sel
+00004a60: 662e 6d6f 6465 6c73 5f6c 6973 743a 0a20  f.models_list:. 
+00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a80: 2020 2073 656c 662e 646f 6f72 5f63 6d64     self.door_cmd
+00004a90: 203d 2062 2744 4f4f 523f 5c72 270a 2020   = b'DOOR?\r'.  
+00004aa0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00004ab0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00004ac0: 2020 2020 2020 2020 7365 6c66 2e64 6f6f          self.doo
+00004ad0: 725f 636d 6420 3d20 6227 4c49 443f 5c72  r_cmd = b'LID?\r
+00004ae0: 270a 2020 2020 2020 2020 2020 2020 656c  '.            el
+00004af0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00004b00: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+00004b10: 696f 6e0a 2020 2020 2020 2020 6578 6365  ion.        exce
+00004b20: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00004b30: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+00004b40: 2070 7269 6e74 2865 290a 2020 2020 2020   print(e).      
+00004b50: 2020 2020 2020 7072 696e 7428 6622 5465        print(f"Te
+00004b60: 7363 6f6d 202d 2043 6f75 6c64 206e 6f74  scom - Could not
+00004b70: 2063 6f6e 6e65 6374 2074 6f20 706f 7274   connect to port
+00004b80: 207b 706f 7274 7d20 6475 6520 746f 207b   {port} due to {
+00004b90: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
+00004ba0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00004bb0: 2020 6465 6620 636c 6f73 655f 706f 7274    def close_port
+00004bc0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004bd0: 2222 220a 2020 2020 2020 2020 636c 6f73  """.        clos
+00004be0: 6573 2063 6f6d 2070 6f72 740a 2020 2020  es com port.    
+00004bf0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004c00: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00004c10: 2073 656c 662e 636f 6d5f 706f 7274 5f6f   self.com_port_o
+00004c20: 626a 2e63 6c6f 7365 2829 0a20 2020 2020  bj.close().     
+00004c30: 2020 2020 2020 2070 7269 6e74 2822 5246         print("RF
+00004c40: 2063 6861 6d62 6572 2064 6973 636f 6e6e   chamber disconn
+00004c50: 6563 7465 6420 6672 6f6d 2070 6f72 743a  ected from port:
+00004c60: 2022 202b 2073 7472 2873 656c 662e 706f   " + str(self.po
+00004c70: 7274 2929 0a20 2020 2020 2020 2065 7863  rt)).        exc
+00004c80: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00004c90: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00004ca0: 7072 696e 7428 2243 6f75 6c64 206e 6f74  print("Could not
+00004cb0: 2064 6973 636f 6e6e 6563 7422 290a 0a20   disconnect").. 
+00004cc0: 2020 2064 6566 206f 7065 6e5f 6368 616d     def open_cham
+00004cd0: 6265 7228 7365 6c66 293a 0a20 2020 2020  ber(self):.     
+00004ce0: 2020 2022 2222 0a20 2020 2020 2020 206f     """.        o
+00004cf0: 7065 6e73 2063 6861 6d62 6572 0a20 2020  pens chamber.   
+00004d00: 2020 2020 203a 7265 7475 726e 3a20 224f       :return: "O
+00004d10: 4b22 2069 6620 636f 6d6d 616e 6420 7761  K" if command wa
+00004d20: 7320 7375 6363 6573 7366 756c 0a20 2020  s successful.   
+00004d30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00004d40: 2069 6620 7365 6c66 2e69 735f 646f 6f72   if self.is_door
+00004d50: 5f6f 7065 6e28 293a 0a20 2020 2020 2020  _open():.       
+00004d60: 2020 2020 2070 7269 6e74 2822 4368 616d       print("Cham
+00004d70: 6265 7220 6973 206f 7065 6e22 290a 2020  ber is open").  
+00004d80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00004d90: 2027 4f4b 270a 2020 2020 2020 2020 7472   'OK'.        tr
+00004da0: 793a 0a20 2020 2020 2020 2020 2020 2070  y:.            p
+00004db0: 7269 6e74 2866 2243 6861 6d62 6572 207b  rint(f"Chamber {
+00004dc0: 7365 6c66 2e70 6f72 747d 2069 7320 6f70  self.port} is op
+00004dd0: 656e 696e 6722 290a 2020 2020 2020 2020  ening").        
+00004de0: 2020 2020 7365 6c66 2e63 6f6d 5f70 6f72      self.com_por
+00004df0: 745f 6f62 6a2e 7265 7365 745f 696e 7075  t_obj.reset_inpu
+00004e00: 745f 6275 6666 6572 2829 0a20 2020 2020  t_buffer().     
+00004e10: 2020 2020 2020 2073 656c 662e 636f 6d5f         self.com_
+00004e20: 706f 7274 5f6f 626a 2e72 6573 6574 5f6f  port_obj.reset_o
+00004e30: 7574 7075 745f 6275 6666 6572 2829 0a20  utput_buffer(). 
+00004e40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004e50: 636f 6d5f 706f 7274 5f6f 626a 2e77 7269  com_port_obj.wri
+00004e60: 7465 2873 656c 662e 6f70 656e 5f63 6d64  te(self.open_cmd
+00004e70: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00004e80: 7320 3d20 2727 0a20 2020 2020 2020 2020  s = ''.         
+00004e90: 2020 2077 6169 745f 636f 756e 7465 7220     wait_counter 
+00004ea0: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
+00004eb0: 6966 2073 656c 662e 646f 6f72 5f63 6d64  if self.door_cmd
+00004ec0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00004ed0: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+00004ee0: 696c 6520 274f 4b27 206e 6f74 2069 6e20  ile 'OK' not in 
+00004ef0: 7265 733a 0a20 2020 2020 2020 2020 2020  res:.           
+00004f00: 2020 2020 2020 2020 2069 6620 7761 6974           if wait
+00004f10: 5f63 6f75 6e74 6572 203e 3d20 3135 3a0a  _counter >= 15:.
+00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f30: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+00004f40: 6365 7074 696f 6e28 6622 4572 726f 7220  ception(f"Error 
+00004f50: 696e 206f 7065 6e69 6e67 2063 6861 6d62  in opening chamb
+00004f60: 6572 207b 7365 6c66 2e70 6f72 747d 2229  er {self.port}")
+00004f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f80: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+00004f90: 636f 6d5f 706f 7274 5f6f 626a 2e72 6561  com_port_obj.rea
+00004fa0: 6428 3134 292e 6465 636f 6465 280a 2020  d(14).decode(.  
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fc0: 2020 2020 2020 2775 7466 2d38 2729 2e75        'utf-8').u
+00004fd0: 7070 6572 2829 2e72 7374 7269 7028 275c  pper().rstrip('\
+00004fe0: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
+00004ff0: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+00005000: 7472 2872 6573 2929 203e 2030 3a0a 2020  tr(res)) > 0:.  
+00005010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005020: 2020 2020 2020 7072 696e 7428 6627 4368        print(f'Ch
+00005030: 616d 6265 7220 7b73 656c 662e 706f 7274  amber {self.port
+00005040: 7d20 7374 6174 7573 3a20 2720 2b20 7374  } status: ' + st
+00005050: 7228 7265 7329 290a 2020 2020 2020 2020  r(res)).        
+00005060: 2020 2020 2020 2020 2020 2020 7761 6974              wait
+00005070: 5f63 6f75 6e74 6572 202b 3d20 310a 2020  _counter += 1.  
+00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005090: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
+000050a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000050b0: 6e6f 7420 7365 6c66 2e69 735f 646f 6f72  not self.is_door
+000050c0: 5f6f 7065 6e28 293a 0a20 2020 2020 2020  _open():.       
+000050d0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+000050e0: 7365 2045 7863 6570 7469 6f6e 280a 2020  se Exception(.  
+000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005100: 2020 2020 2020 6622 7b73 656c 662e 706f        f"{self.po
+00005110: 7274 7d20 446f 6f72 2073 7461 7475 7320  rt} Door status 
+00005120: 646f 6573 6e27 7420 6d61 7463 6820 636f  doesn't match co
+00005130: 6d6d 616e 6420 7365 6e74 2122 290a 2020  mmand sent!").  
+00005140: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00005150: 6622 4368 616d 6265 7220 7b73 656c 662e  f"Chamber {self.
+00005160: 706f 7274 7d20 6973 206f 7065 6e22 290a  port} is open").
+00005170: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00005180: 726e 2027 4f4b 270a 2020 2020 2020 2020  rn 'OK'.        
+00005190: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+000051a0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+000051b0: 2020 2070 7269 6e74 2865 290a 2020 2020     print(e).    
+000051c0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
+000051d0: 4641 494c 220a 0a20 2020 2064 6566 2063  FAIL"..    def c
+000051e0: 6c6f 7365 5f63 6861 6d62 6572 2873 656c  lose_chamber(sel
+000051f0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00005200: 2020 2020 2020 2020 636c 6f73 6573 2063          closes c
+00005210: 6861 6d62 6572 0a20 2020 2020 2020 203a  hamber.        :
+00005220: 7265 7475 726e 3a20 224f 4b22 2069 6620  return: "OK" if 
+00005230: 636f 6d6d 616e 6420 7761 7320 7375 6363  command was succ
+00005240: 6573 7366 756c 0a20 2020 2020 2020 2022  essful.        "
+00005250: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+00005260: 6c66 2e69 735f 646f 6f72 5f63 6c6f 7365  lf.is_door_close
+00005270: 6428 293a 0a20 2020 2020 2020 2020 2020  d():.           
+00005280: 2070 7269 6e74 2822 4368 616d 6265 7220   print("Chamber 
+00005290: 636c 6f73 6564 2229 0a20 2020 2020 2020  closed").       
+000052a0: 2020 2020 2072 6574 7572 6e20 274f 4b27       return 'OK'
+000052b0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+000052c0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000052d0: 6622 4348 414d 4245 5220 7b73 656c 662e  f"CHAMBER {self.
+000052e0: 706f 7274 7d20 4953 2043 4c4f 5349 4e47  port} IS CLOSING
+000052f0: 2c20 434c 4541 5220 4841 4e44 5321 2121  , CLEAR HANDS!!!
+00005300: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00005310: 6c65 6570 2832 290a 2020 2020 2020 2020  leep(2).        
+00005320: 2020 2020 7365 6c66 2e63 6f6d 5f70 6f72      self.com_por
+00005330: 745f 6f62 6a2e 7772 6974 6528 7365 6c66  t_obj.write(self
+00005340: 2e63 6c6f 7365 5f63 6d64 290a 2020 2020  .close_cmd).    
+00005350: 2020 2020 2020 2020 7265 7320 3d20 2727          res = ''
+00005360: 0a20 2020 2020 2020 2020 2020 2077 6169  .            wai
+00005370: 745f 636f 756e 7465 7220 3d20 300a 2020  t_counter = 0.  
+00005380: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00005390: 662e 646f 6f72 5f63 6d64 2069 7320 6e6f  f.door_cmd is no
+000053a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000053b0: 2020 2020 2020 2020 7768 696c 6520 2752          while 'R
+000053c0: 4541 4459 2720 6e6f 7420 696e 2072 6573  EADY' not in res
+000053d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000053e0: 2020 2020 2020 6966 2077 6169 745f 636f        if wait_co
+000053f0: 756e 7465 7220 3e3d 2035 3a0a 2020 2020  unter >= 5:.    
+00005400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005410: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+00005420: 696f 6e28 6622 6368 616d 6265 7220 7b73  ion(f"chamber {s
+00005430: 656c 662e 706f 7274 7d20 7374 6174 7573  elf.port} status
+00005440: 2069 7320 4e4f 5420 7265 6164 7922 290a   is NOT ready").
+00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005460: 2020 2020 7265 7320 3d20 7365 6c66 2e63      res = self.c
+00005470: 6f6d 5f70 6f72 745f 6f62 6a2e 7265 6164  om_port_obj.read
+00005480: 2831 3429 2e64 6563 6f64 6528 0a20 2020  (14).decode(.   
+00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054a0: 2020 2020 2027 7574 662d 3827 292e 7570       'utf-8').up
+000054b0: 7065 7228 292e 7273 7472 6970 2827 5c72  per().rstrip('\r
+000054c0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+000054d0: 2020 2020 2020 2069 6620 2745 5252 2720         if 'ERR' 
+000054e0: 696e 2072 6573 206f 7220 2752 4541 4459  in res or 'READY
+000054f0: 2720 696e 2072 6573 206f 7220 274f 4b27  ' in res or 'OK'
+00005500: 2069 6e20 7265 733a 0a20 2020 2020 2020   in res:.       
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 2070 7269 6e74 2866 2743 6861 6d62 6572   print(f'Chamber
+00005530: 207b 7365 6c66 2e70 6f72 747d 2073 7461   {self.port} sta
+00005540: 7475 733a 2027 202b 2073 7472 2872 6573  tus: ' + str(res
+00005550: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00005560: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 2020 2020 2070 7269 6e74 2866 2743 6861       print(f'Cha
+00005590: 6d62 6572 207b 7365 6c66 2e70 6f72 747d  mber {self.port}
+000055a0: 2064 6964 206e 6f74 2061 6e73 7765 7265   did not answere
+000055b0: 643a 207b 7265 737d 2720 2b20 7374 7228  d: {res}' + str(
+000055c0: 7265 7329 290a 2020 2020 2020 2020 2020  res)).          
+000055d0: 2020 2020 2020 2020 2020 6966 2027 4552            if 'ER
+000055e0: 5227 2069 6e20 7265 733a 0a20 2020 2020  R' in res:.     
+000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005600: 2020 2072 6574 7572 6e20 2246 4149 4c22     return "FAIL"
+00005610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005620: 2020 2020 2077 6169 745f 636f 756e 7465       wait_counte
+00005630: 7220 2b3d 2031 0a20 2020 2020 2020 2020  r += 1.         
+00005640: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+00005650: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
+00005660: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00005670: 662e 6973 5f64 6f6f 725f 636c 6f73 6564  f.is_door_closed
+00005680: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00005690: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+000056a0: 6365 7074 696f 6e28 0a20 2020 2020 2020  ception(.       
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056c0: 2066 227b 7365 6c66 2e70 6f72 747d 2044   f"{self.port} D
+000056d0: 6f6f 7220 7374 6174 7573 2064 6f65 736e  oor status doesn
+000056e0: 2774 206d 6174 6368 2063 6f6d 6d61 6e64  't match command
+000056f0: 2073 656e 7421 2229 0a20 2020 2020 2020   sent!").       
+00005700: 2020 2020 2070 7269 6e74 2866 2243 6861       print(f"Cha
+00005710: 6d62 6572 207b 7365 6c66 2e70 6f72 747d  mber {self.port}
+00005720: 2063 6c6f 7365 6422 290a 2020 2020 2020   closed").      
+00005730: 2020 2020 2020 7265 7475 726e 2027 4f4b        return 'OK
+00005740: 270a 2020 2020 2020 2020 6578 6365 7074  '.        except
+00005750: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00005760: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00005770: 6e74 2866 2245 7272 6f72 2069 6e20 636c  nt(f"Error in cl
+00005780: 6f73 696e 6720 6368 616d 6265 7220 7b73  osing chamber {s
+00005790: 656c 662e 706f 7274 7d2c 2064 7565 2074  elf.port}, due t
+000057a0: 6f20 7b65 7d22 290a 2020 2020 2020 2020  o {e}").        
+000057b0: 2020 2020 7265 7475 726e 2022 4641 494c      return "FAIL
+000057c0: 220a 0a20 2020 2064 6566 2069 735f 636f  "..    def is_co
+000057d0: 6e6e 6563 7465 6428 7365 6c66 293a 0a20  nnected(self):. 
+000057e0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000057f0: 6f6d 5f70 6f72 745f 6f62 6a20 6973 204e  om_port_obj is N
+00005800: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00005810: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00005820: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00005830: 662e 636f 6d5f 706f 7274 5f6f 626a 2e69  f.com_port_obj.i
+00005840: 734f 7065 6e28 290a 0a20 2020 2064 6566  sOpen()..    def
+00005850: 2067 6574 5f73 7461 7465 2873 656c 6629   get_state(self)
+00005860: 3a0a 2020 2020 2020 2020 7374 6174 6520  :.        state 
+00005870: 3d20 2727 0a20 2020 2020 2020 2072 7370  = ''.        rsp
+00005880: 203d 2027 270a 2020 2020 2020 2020 7472   = ''.        tr
+00005890: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+000058a0: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
+000058b0: 2e72 6573 6574 5f69 6e70 7574 5f62 7566  .reset_input_buf
+000058c0: 6665 7228 290a 2020 2020 2020 2020 2020  fer().          
+000058d0: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
+000058e0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000058f0: 2e64 6f6f 725f 636d 6420 6973 204e 6f6e  .door_cmd is Non
+00005900: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00005910: 2020 2072 6574 7572 6e20 7374 6174 650a     return state.
+00005920: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005930: 2e63 6f6d 5f70 6f72 745f 6f62 6a2e 7772  .com_port_obj.wr
+00005940: 6974 6528 7365 6c66 2e64 6f6f 725f 636d  ite(self.door_cm
+00005950: 6429 0a20 2020 2020 2020 2020 2020 2073  d).            s
+00005960: 6c65 6570 2830 2e31 290a 2020 2020 2020  leep(0.1).      
+00005970: 2020 2020 2020 7273 7020 3d20 7365 6c66        rsp = self
+00005980: 2e63 6f6d 5f70 6f72 745f 6f62 6a2e 7265  .com_port_obj.re
+00005990: 6164 2831 3429 0a20 2020 2020 2020 2020  ad(14).         
+000059a0: 2020 2073 7461 7465 203d 2072 7370 2e64     state = rsp.d
+000059b0: 6563 6f64 6528 2775 7466 2d38 2729 2e75  ecode('utf-8').u
+000059c0: 7070 6572 2829 2e72 7374 7269 7028 275c  pper().rstrip('\
+000059d0: 7227 290a 2020 2020 2020 2020 6578 6365  r').        exce
+000059e0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+000059f0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00005a00: 7269 6e74 2866 2743 6f75 6c64 206e 6f74  rint(f'Could not
+00005a10: 2063 6f6d 6d75 6e69 6361 7465 2077 6974   communicate wit
+00005a20: 6820 6368 616d 6265 7220 6475 6520 746f  h chamber due to
+00005a30: 207b 657d 2e20 476f 7420 7265 7370 6f6e   {e}. Got respon
+00005a40: 7365 3a7b 7273 707d 2e20 706c 6561 7365  se:{rsp}. please
+00005a50: 2063 6865 636b 2063 6861 6d62 6572 2063   check chamber c
+00005a60: 6f6e 6e65 6374 696f 6e27 290a 2020 2020  onnection').    
+00005a70: 2020 2020 7265 7475 726e 2073 7461 7465      return state
+00005a80: 0a0a 2020 2020 6465 6620 6973 5f64 6f6f  ..    def is_doo
+00005a90: 725f 6f70 656e 2873 656c 6629 3a0a 2020  r_open(self):.  
+00005aa0: 2020 2020 2020 7374 6174 6520 3d20 7365        state = se
+00005ab0: 6c66 2e67 6574 5f73 7461 7465 2829 0a20  lf.get_state(). 
+00005ac0: 2020 2020 2020 2069 6620 274f 5045 4e27         if 'OPEN'
+00005ad0: 2069 6e20 7374 6174 653a 0a20 2020 2020   in state:.     
+00005ae0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00005af0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00005b00: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00005b10: 2069 735f 646f 6f72 5f63 6c6f 7365 6428   is_door_closed(
+00005b20: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00005b30: 7461 7465 203d 2073 656c 662e 6765 745f  tate = self.get_
+00005b40: 7374 6174 6528 290a 2020 2020 2020 2020  state().        
+00005b50: 6966 2027 434c 4f53 4527 2069 6e20 7374  if 'CLOSE' in st
+00005b60: 6174 653a 0a20 2020 2020 2020 2020 2020  ate:.           
+00005b70: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00005b80: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00005b90: 650a 0a0a 636c 6173 7320 4261 7263 6f64  e...class Barcod
+00005ba0: 6553 6361 6e6e 6572 3a0a 2020 2020 6465  eScanner:.    de
+00005bb0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00005bc0: 2063 6f6d 5f70 6f72 743a 2073 7472 203d   com_port: str =
+00005bd0: 204e 6f6e 652c 2062 6175 645f 7261 7465   None, baud_rate
+00005be0: 3a20 696e 7420 3d20 3131 3532 3030 2c20  : int = 115200, 
+00005bf0: 636f 6e66 6967 3a20 626f 6f6c 203d 2054  config: bool = T
+00005c00: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00005c10: 2020 2020 2020 6c6f 675f 7479 7065 3a20        log_type: 
+00005c20: 7374 7220 3d20 274e 4f5f 4c4f 4727 2c20  str = 'NO_LOG', 
+00005c30: 7772 6974 655f 746f 5f6c 6f67 3a20 626f  write_to_log: bo
+00005c40: 6f6c 203d 2046 616c 7365 2c20 7469 6d65  ol = False, time
+00005c50: 6f75 743a 2073 7472 203d 2027 3130 3030  out: str = '1000
+00005c60: 272c 206c 6f67 5f6e 616d 653a 2073 7472  ', log_name: str
+00005c70: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00005c80: 2020 2222 220a 2020 2020 2020 2020 496e    """.        In
+00005c90: 6974 6961 6c69 7a65 2074 6865 2051 5253  itialize the QRS
+00005ca0: 6361 6e6e 6572 206f 626a 6563 742e 0a20  canner object.. 
+00005cb0: 2020 2020 2020 2044 6174 6173 6865 6574         Datasheet
+00005cc0: 3a0a 2020 2020 2020 2020 6874 7470 733a  :.        https:
+00005cd0: 2f2f 6364 6e2e 7274 7363 616e 2e6e 6574  //cdn.rtscan.net
+00005ce0: 2f77 702d 636f 6e74 656e 742f 7570 6c6f  /wp-content/uplo
+00005cf0: 6164 732f 3230 3232 2f30 362f 5573 6572  ads/2022/06/User
+00005d00: 5f4d 616e 7561 6c5f 5254 3231 345f 5254  _Manual_RT214_RT
+00005d10: 3231 375f 5254 3233 355f 5254 3234 305f  217_RT235_RT240_
+00005d20: 3230 3232 2e30 355f 312e 302e 362e 7064  2022.05_1.0.6.pd
+00005d30: 660a 2020 2020 2020 2020 466f 7220 7468  f.        For th
+00005d40: 6520 6669 7273 7420 7573 652c 2079 6f75  e first use, you
+00005d50: 2077 696c 6c20 6e65 6564 2074 6f20 7363   will need to sc
+00005d60: 616e 2033 2062 6172 636f 6465 2074 6f20  an 3 barcode to 
+00005d70: 696e 6974 6961 6c20 636f 6d70 6f72 7420  initial comport 
+00005d80: 636f 6e6e 6563 7469 6f6e 3a0a 2020 2020  connection:.    
+00005d90: 2020 2020 6874 7470 733a 2f2f 7769 6c69      https://wili
+00005da0: 6f74 2e61 746c 6173 7369 616e 2e6e 6574  ot.atlassian.net
+00005db0: 2f77 696b 692f 7370 6163 6573 2f46 572f  /wiki/spaces/FW/
+00005dc0: 7061 6765 732f 3235 3636 3032 3934 3037  pages/2566029407
+00005dd0: 2f52 5473 6361 6e2b 4261 7263 6f64 652b  /RTscan+Barcode+
+00005de0: 5363 616e 6e65 720a 2020 2020 2020 2020  Scanner.        
+00005df0: 4070 6172 616d 2063 6f6d 3a0a 2020 2020  @param com:.    
+00005e00: 2020 2020 4074 7970 6520 636f 6d3a 0a20      @type com:. 
+00005e10: 2020 2020 2020 2040 7061 7261 6d20 6261         @param ba
+00005e20: 7564 3a0a 2020 2020 2020 2020 4074 7970  ud:.        @typ
+00005e30: 6520 6261 7564 3a0a 2020 2020 2020 2020  e baud:.        
+00005e40: 4070 6172 616d 2063 6f6e 6669 673a 0a20  @param config:. 
+00005e50: 2020 2020 2020 2040 7479 7065 2063 6f6e         @type con
+00005e60: 6669 673a 0a20 2020 2020 2020 2040 7061  fig:.        @pa
+00005e70: 7261 6d20 6c6f 675f 7479 7065 3a0a 2020  ram log_type:.  
+00005e80: 2020 2020 2020 4074 7970 6520 6c6f 675f        @type log_
+00005e90: 7479 7065 3a0a 2020 2020 2020 2020 4070  type:.        @p
+00005ea0: 6172 616d 2077 7269 7465 5f74 6f5f 6c6f  aram write_to_lo
+00005eb0: 673a 0a20 2020 2020 2020 2040 7479 7065  g:.        @type
+00005ec0: 2077 7269 7465 5f74 6f5f 6c6f 673a 0a20   write_to_log:. 
+00005ed0: 2020 2020 2020 2040 7061 7261 6d20 7469         @param ti
+00005ee0: 6d65 6f75 743a 0a20 2020 2020 2020 2040  meout:.        @
+00005ef0: 7479 7065 2074 696d 656f 7574 3a0a 2020  type timeout:.  
+00005f00: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00005f10: 2020 7365 6c66 2e70 7265 6669 7820 3d20    self.prefix = 
+00005f20: 277e 0130 3030 3040 270a 2020 2020 2020  '~.0000@'.      
+00005f30: 2020 7365 6c66 2e73 7566 6669 7820 3d20    self.suffix = 
+00005f40: 273b 0327 0a20 2020 2020 2020 2073 656c  ';.'.        sel
+00005f50: 662e 636f 6d5f 706f 7274 203d 2063 6f6d  f.com_port = com
+00005f60: 5f70 6f72 740a 2020 2020 2020 2020 7365  _port.        se
+00005f70: 6c66 2e73 6572 6961 6c5f 636f 6e6e 6563  lf.serial_connec
+00005f80: 7469 6f6e 203d 204e 6f6e 650a 2020 2020  tion = None.    
+00005f90: 2020 2020 7365 6c66 2e64 6576 6963 655f      self.device_
+00005fa0: 7369 676e 6174 7572 6520 3d20 224e 4c53  signature = "NLS
+00005fb0: 2d4e 3122 0a20 2020 2020 2020 2073 656c  -N1".        sel
+00005fc0: 662e 6c6f 675f 7479 7065 203d 206c 6f67  f.log_type = log
+00005fd0: 5f74 7970 650a 2020 2020 2020 2020 7365  _type.        se
+00005fe0: 6c66 2e77 7269 7465 5f74 6f5f 6c6f 6720  lf.write_to_log 
+00005ff0: 3d20 7772 6974 655f 746f 5f6c 6f67 0a20  = write_to_log. 
+00006000: 2020 2020 2020 2073 656c 662e 7367 7469         self.sgti
+00006010: 6e5f 6c65 6e67 7468 203d 2033 310a 0a20  n_length = 31.. 
+00006020: 2020 2020 2020 2069 6620 6c6f 675f 6e61         if log_na
+00006030: 6d65 2069 7320 4e6f 6e65 3a0a 2020 2020  me is None:.    
+00006040: 2020 2020 2020 2020 7365 6c66 2e71 725f          self.qr_
+00006050: 6c6f 6767 6572 203d 206c 6f67 6769 6e67  logger = logging
+00006060: 2e67 6574 4c6f 6767 6572 2827 5152 4c6f  .getLogger('QRLo
+00006070: 6767 6572 2729 0a20 2020 2020 2020 2065  gger').        e
+00006080: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00006090: 2073 656c 662e 7172 5f6c 6f67 6765 7220   self.qr_logger 
+000060a0: 3d20 6c6f 6767 696e 672e 6765 744c 6f67  = logging.getLog
+000060b0: 6765 7228 6c6f 675f 6e61 6d65 290a 0a20  ger(log_name).. 
+000060c0: 2020 2020 2020 2069 6620 636f 6d5f 706f         if com_po
+000060d0: 7274 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rt is not None:.
+000060e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000060f0: 2e6f 7065 6e5f 706f 7274 2863 6f6d 5f70  .open_port(com_p
+00006100: 6f72 742c 2062 6175 645f 7261 7465 3d62  ort, baud_rate=b
+00006110: 6175 645f 7261 7465 2c20 636f 6e66 6967  aud_rate, config
+00006120: 3d63 6f6e 6669 672c 2074 696d 656f 7574  =config, timeout
+00006130: 3d74 696d 656f 7574 290a 2020 2020 2020  =timeout).      
+00006140: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00006150: 2020 2020 7365 6c66 2e61 7574 6f5f 636f      self.auto_co
+00006160: 6e6e 6563 7428 7469 6d65 6f75 743d 7469  nnect(timeout=ti
+00006170: 6d65 6f75 7429 0a0a 2020 2020 2020 2020  meout)..        
+00006180: 6966 2073 656c 662e 7772 6974 655f 746f  if self.write_to
+00006190: 5f6c 6f67 3a0a 2020 2020 2020 2020 2020  _log:.          
+000061a0: 2020 7365 6c66 2e63 7265 6174 655f 6c6f    self.create_lo
+000061b0: 675f 6669 6c65 2829 0a0a 2020 2020 6465  g_file()..    de
+000061c0: 6620 6372 6561 7465 5f6c 6f67 5f66 696c  f create_log_fil
+000061d0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000061e0: 2022 2222 0a20 2020 2020 2020 2043 7265   """.        Cre
+000061f0: 6174 6520 6120 6c6f 6720 6669 6c65 2e0a  ate a log file..
+00006200: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006210: 2020 2020 7769 6c69 6f74 5f64 6972 203d      wiliot_dir =
+00006220: 2057 696c 696f 7444 6972 2829 0a20 2020   WiliotDir().   
+00006230: 2020 2020 2077 696c 696f 745f 6469 722e       wiliot_dir.
+00006240: 6372 6561 7465 5f64 6972 2827 5152 5f73  create_dir('QR_s
+00006250: 6361 6e27 290a 2020 2020 2020 2020 6170  can').        ap
+00006260: 705f 6469 7220 3d20 7769 6c69 6f74 5f64  p_dir = wiliot_d
+00006270: 6972 2e67 6574 5f77 696c 696f 745f 726f  ir.get_wiliot_ro
+00006280: 6f74 5f61 7070 5f64 6972 2829 0a20 2020  ot_app_dir().   
+00006290: 2020 2020 206c 6f67 5f64 6972 203d 206f       log_dir = o
+000062a0: 732e 7061 7468 2e6a 6f69 6e28 6170 705f  s.path.join(app_
+000062b0: 6469 722c 2027 5152 5f73 6361 6e27 290a  dir, 'QR_scan').
+000062c0: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
+000062d0: 732e 7061 7468 2e65 7869 7374 7328 6c6f  s.path.exists(lo
+000062e0: 675f 6469 7229 3a0a 2020 2020 2020 2020  g_dir):.        
+000062f0: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
+00006300: 6c6f 675f 6469 7229 0a0a 2020 2020 2020  log_dir)..      
+00006310: 2020 6375 7272 656e 745f 7469 6d65 203d    current_time =
+00006320: 2064 6174 6574 696d 652e 6e6f 7728 292e   datetime.now().
+00006330: 7374 7266 7469 6d65 2822 2559 2d25 6d2d  strftime("%Y-%m-
+00006340: 2564 5f25 482d 254d 2d25 5322 290a 2020  %d_%H-%M-%S").  
+00006350: 2020 2020 2020 7365 6c66 2e6c 6f67 5f66        self.log_f
+00006360: 696c 656e 616d 6520 3d20 6f73 2e70 6174  ilename = os.pat
+00006370: 682e 6a6f 696e 286c 6f67 5f64 6972 2c20  h.join(log_dir, 
+00006380: 6622 5152 5f72 6561 645f 6c6f 675f 7b63  f"QR_read_log_{c
+00006390: 7572 7265 6e74 5f74 696d 657d 2e6c 6f67  urrent_time}.log
+000063a0: 2229 0a20 2020 2020 2020 2077 6974 6820  ").        with 
+000063b0: 6f70 656e 2873 656c 662e 6c6f 675f 6669  open(self.log_fi
+000063c0: 6c65 6e61 6d65 2c20 2777 2729 2061 7320  lename, 'w') as 
+000063d0: 663a 0a20 2020 2020 2020 2020 2020 2066  f:.            f
+000063e0: 2e77 7269 7465 2822 4c6f 6720 6669 6c65  .write("Log file
+000063f0: 2063 7265 6174 6564 2e5c 6e22 290a 0a20   created.\n").. 
+00006400: 2020 2064 6566 2061 7574 6f5f 636f 6e6e     def auto_conn
+00006410: 6563 7428 7365 6c66 2c20 6261 7564 5f72  ect(self, baud_r
+00006420: 6174 653a 2069 6e74 203d 2031 3135 3230  ate: int = 11520
+00006430: 302c 2063 6f6e 6669 673a 2062 6f6f 6c20  0, config: bool 
+00006440: 3d20 5472 7565 2c20 7469 6d65 6f75 743a  = True, timeout:
+00006450: 2073 7472 203d 2027 3130 3030 2729 3a0a   str = '1000'):.
+00006460: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006470: 2020 2020 4175 746f 6d61 7469 6361 6c6c      Automaticall
+00006480: 7920 636f 6e6e 6563 7420 746f 2074 6865  y connect to the
+00006490: 2043 4f4d 2070 6f72 742e 0a20 2020 2020   COM port..     
+000064a0: 2020 2022 2222 0a20 2020 2020 2020 2063     """.        c
+000064b0: 6f6d 5f70 6f72 7420 3d20 7365 6c66 2e66  om_port = self.f
+000064c0: 696e 645f 636f 6d5f 706f 7274 2862 6175  ind_com_port(bau
+000064d0: 645f 7261 7465 290a 2020 2020 2020 2020  d_rate).        
+000064e0: 6966 2063 6f6d 5f70 6f72 7420 6973 206e  if com_port is n
+000064f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00006500: 2020 2020 2073 656c 662e 6f70 656e 5f70       self.open_p
+00006510: 6f72 7428 636f 6d5f 706f 7274 2c20 6261  ort(com_port, ba
+00006520: 7564 5f72 6174 652c 2063 6f6e 6669 672c  ud_rate, config,
+00006530: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+00006540: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00006550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006560: 2e71 725f 6c6f 6767 6572 2e65 7272 6f72  .qr_logger.error
+00006570: 2822 4e6f 2073 7569 7461 626c 6520 434f  ("No suitable CO
+00006580: 4d20 706f 7274 2066 6f75 6e64 2e22 290a  M port found.").
+00006590: 2020 2020 2020 2020 2020 2020 7379 732e              sys.
+000065a0: 6578 6974 2831 290a 0a20 2020 2064 6566  exit(1)..    def
+000065b0: 2069 735f 7274 7363 616e 5f72 7432 3335   is_rtscan_rt235
+000065c0: 2873 656c 662c 2063 6f6d 5f70 6f72 743a  (self, com_port:
+000065d0: 2073 7472 2c20 6261 7564 5f72 6174 653a   str, baud_rate:
+000065e0: 2069 6e74 203d 2031 3135 3230 3029 202d   int = 115200) -
+000065f0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00006600: 2222 220a 2020 2020 2020 2020 4368 6563  """.        Chec
+00006610: 6b20 6966 2074 6865 2064 6576 6963 6520  k if the device 
+00006620: 6973 2052 5473 6361 6e20 5254 3233 352e  is RTscan RT235.
+00006630: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006640: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00006650: 2020 2020 2020 7769 7468 2073 6572 6961        with seria
+00006660: 6c2e 5365 7269 616c 2863 6f6d 5f70 6f72  l.Serial(com_por
+00006670: 742c 2062 6175 645f 7261 7465 2c20 7469  t, baud_rate, ti
+00006680: 6d65 6f75 743d 3129 2061 7320 7365 723a  meout=1) as ser:
+00006690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000066a0: 2073 6572 2e77 7269 7465 2873 7472 2e65   ser.write(str.e
+000066b0: 6e63 6f64 6528 7365 6c66 2e70 7265 6669  ncode(self.prefi
+000066c0: 7820 2b20 2251 5259 5044 4e22 202b 2073  x + "QRYPDN" + s
+000066d0: 656c 662e 7375 6666 6978 2929 0a20 2020  elf.suffix)).   
+000066e0: 2020 2020 2020 2020 2020 2020 2073 6c65               sle
+000066f0: 6570 2830 2e31 290a 2020 2020 2020 2020  ep(0.1).        
+00006700: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00006710: 203d 2073 6572 2e72 6561 645f 616c 6c28   = ser.read_all(
+00006720: 292e 6465 636f 6465 2829 0a20 2020 2020  ).decode().     
+00006730: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006740: 6e20 7365 6c66 2e64 6576 6963 655f 7369  n self.device_si
+00006750: 676e 6174 7572 6520 696e 2072 6573 706f  gnature in respo
+00006760: 6e73 650a 2020 2020 2020 2020 6578 6365  nse.        exce
+00006770: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00006780: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00006790: 656c 662e 7172 5f6c 6f67 6765 722e 6572  elf.qr_logger.er
+000067a0: 726f 7228 6622 4572 726f 7220 696e 2069  ror(f"Error in i
+000067b0: 735f 7274 7363 616e 5f72 7432 3335 3a20  s_rtscan_rt235: 
+000067c0: 7b65 7d22 290a 2020 2020 2020 2020 2020  {e}").          
+000067d0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+000067e0: 2020 2020 6465 6620 6669 6e64 5f63 6f6d      def find_com
+000067f0: 5f70 6f72 7428 7365 6c66 2c20 6261 7564  _port(self, baud
+00006800: 5f72 6174 653a 2069 6e74 203d 2031 3135  _rate: int = 115
+00006810: 3230 3029 202d 3e20 7374 723a 0a20 2020  200) -> str:.   
+00006820: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00006830: 2046 696e 6420 7468 6520 434f 4d20 706f   Find the COM po
+00006840: 7274 2e0a 2020 2020 2020 2020 2222 220a  rt..        """.
+00006850: 2020 2020 2020 2020 636f 6d5f 706f 7274          com_port
+00006860: 7320 3d20 7365 7269 616c 5f70 6f72 7473  s = serial_ports
+00006870: 2829 0a20 2020 2020 2020 2066 6f72 2063  ().        for c
+00006880: 6f6d 5f70 6f72 7420 696e 2063 6f6d 5f70  om_port in com_p
+00006890: 6f72 7473 3a0a 2020 2020 2020 2020 2020  orts:.          
+000068a0: 2020 6966 2073 656c 662e 6973 5f72 7473    if self.is_rts
+000068b0: 6361 6e5f 7274 3233 3528 636f 6d5f 706f  can_rt235(com_po
+000068c0: 7274 2c20 6261 7564 5f72 6174 6529 3a0a  rt, baud_rate):.
+000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068e0: 7265 7475 726e 2063 6f6d 5f70 6f72 740a  return com_port.
+000068f0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00006900: 6f6e 650a 0a20 2020 2064 6566 206f 7065  one..    def ope
+00006910: 6e5f 706f 7274 2873 656c 662c 2063 6f6d  n_port(self, com
+00006920: 5f70 6f72 743a 2073 7472 2c20 6261 7564  _port: str, baud
+00006930: 5f72 6174 653a 2069 6e74 203d 2031 3135  _rate: int = 115
+00006940: 3230 302c 2063 6f6e 6669 673a 2062 6f6f  200, config: boo
+00006950: 6c20 3d20 5472 7565 2c20 7469 6d65 6f75  l = True, timeou
+00006960: 743a 2073 7472 203d 2027 3130 3030 2729  t: str = '1000')
+00006970: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00006980: 2020 2020 2020 4f70 656e 2074 6865 2043        Open the C
+00006990: 4f4d 2070 6f72 742e 0a20 2020 2020 2020  OM port..       
+000069a0: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
+000069b0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000069c0: 206e 6f74 2073 656c 662e 6973 5f72 7473   not self.is_rts
+000069d0: 6361 6e5f 7274 3233 3528 636f 6d5f 706f  can_rt235(com_po
+000069e0: 7274 2c20 6261 7564 5f72 6174 6529 3a0a  rt, baud_rate):.
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+00006a10: 6627 7b63 6f6d 5f70 6f72 747d 2069 7320  f'{com_port} is 
+00006a20: 6e6f 7420 6120 6261 7263 6f64 6520 7363  not a barcode sc
+00006a30: 616e 6e65 7227 290a 2020 2020 2020 2020  anner').        
+00006a40: 2020 2020 7365 6c66 2e73 6572 6961 6c5f      self.serial_
+00006a50: 636f 6e6e 6563 7469 6f6e 203d 2073 6572  connection = ser
+00006a60: 6961 6c2e 5365 7269 616c 2863 6f6d 5f70  ial.Serial(com_p
+00006a70: 6f72 742c 2062 6175 645f 7261 7465 2c20  ort, baud_rate, 
+00006a80: 7469 6d65 6f75 743d 2869 6e74 2874 696d  timeout=(int(tim
+00006a90: 656f 7574 2920 2b20 3530 2920 2f20 3130  eout) + 50) / 10
+00006aa0: 3030 290a 2020 2020 2020 2020 6578 6365  00).        exce
+00006ab0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00006ac0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00006ad0: 656c 662e 636c 6f73 655f 706f 7274 2829  elf.close_port()
+00006ae0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00006af0: 7365 2045 7863 6570 7469 6f6e 2866 2743  se Exception(f'C
+00006b00: 6f75 6c64 206e 6f74 2063 6f6e 6e65 6374  ould not connect
+00006b10: 2074 6f20 7b63 6f6d 5f70 6f72 747d 3a20   to {com_port}: 
+00006b20: 7b65 7d27 290a 0a20 2020 2020 2020 2069  {e}')..        i
+00006b30: 6620 7365 6c66 2e73 6572 6961 6c5f 636f  f self.serial_co
+00006b40: 6e6e 6563 7469 6f6e 2069 7320 6e6f 7420  nnection is not 
+00006b50: 4e6f 6e65 2061 6e64 2073 656c 662e 6c6f  None and self.lo
+00006b60: 675f 7479 7065 2021 3d20 274e 4f5f 4c4f  g_type != 'NO_LO
+00006b70: 4727 3a0a 2020 2020 2020 2020 2020 2020  G':.            
+00006b80: 7365 6c66 2e71 725f 6c6f 6767 6572 2e69  self.qr_logger.i
+00006b90: 6e66 6f28 6627 4261 7263 6f64 6520 7363  nfo(f'Barcode sc
+00006ba0: 616e 6e65 7220 287b 636f 6d5f 706f 7274  anner ({com_port
+00006bb0: 7d29 2063 6f6e 6e65 6374 6564 2e27 290a  }) connected.').
+00006bc0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+00006bd0: 662e 7365 7269 616c 5f63 6f6e 6e65 6374  f.serial_connect
+00006be0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+00006bf0: 2020 2020 2020 2020 2073 656c 662e 7172           self.qr
+00006c00: 5f6c 6f67 6765 722e 6572 726f 7228 6627  _logger.error(f'
+00006c10: 4261 7263 6f64 6520 7363 616e 6e65 7220  Barcode scanner 
+00006c20: 2d20 5072 6f62 6c65 6d20 636f 6e6e 6563  - Problem connec
+00006c30: 7469 6e67 207b 636f 6d5f 706f 7274 7d27  ting {com_port}'
+00006c40: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00006c50: 7475 726e 0a0a 2020 2020 2020 2020 7365  turn..        se
+00006c60: 6c66 2e63 6f6d 5f70 6f72 7420 3d20 636f  lf.com_port = co
+00006c70: 6d5f 706f 7274 0a20 2020 2020 2020 2073  m_port.        s
+00006c80: 656c 662e 7365 7269 616c 5f63 6f6e 6e65  elf.serial_conne
+00006c90: 6374 696f 6e2e 7772 6974 6554 696d 656f  ction.writeTimeo
+00006ca0: 7574 203d 2030 2e35 2020 2320 7772 6974  ut = 0.5  # writ
+00006cb0: 6520 7469 6d65 6f75 742e 0a20 2020 2020  e timeout..     
+00006cc0: 2020 2069 6620 636f 6e66 6967 3a0a 2020     if config:.  
+00006cd0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00006ce0: 6f6e 6669 6775 7265 2874 696d 655f 6f75  onfigure(time_ou
+00006cf0: 743d 7469 6d65 6f75 7429 0a0a 2020 2020  t=timeout)..    
+00006d00: 6465 6620 636c 6f73 655f 706f 7274 2873  def close_port(s
+00006d10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00006d20: 220a 2020 2020 2020 2020 436c 6f73 6520  ".        Close 
+00006d30: 7468 6520 434f 4d20 706f 7274 2e0a 2020  the COM port..  
+00006d40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00006d50: 2020 6966 2073 656c 662e 7365 7269 616c    if self.serial
+00006d60: 5f63 6f6e 6e65 6374 696f 6e20 6973 206e  _connection is n
+00006d70: 6f74 204e 6f6e 6520 616e 6420 7365 6c66  ot None and self
+00006d80: 2e73 6572 6961 6c5f 636f 6e6e 6563 7469  .serial_connecti
+00006d90: 6f6e 2e69 734f 7065 6e28 293a 0a20 2020  on.isOpen():.   
+00006da0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00006db0: 7269 616c 5f63 6f6e 6e65 6374 696f 6e2e  rial_connection.
+00006dc0: 636c 6f73 6528 290a 0a20 2020 2064 6566  close()..    def
+00006dd0: 2069 735f 6f70 656e 2873 656c 6629 202d   is_open(self) -
+00006de0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00006df0: 2222 220a 2020 2020 2020 2020 4368 6563  """.        Chec
+00006e00: 6b20 6966 2074 6865 2043 4f4d 2070 6f72  k if the COM por
+00006e10: 7420 6973 206f 7065 6e2e 0a20 2020 2020  t is open..     
+00006e20: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
+00006e30: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00006e40: 7265 7320 3d20 7365 6c66 2e6d 616e 7561  res = self.manua
+00006e50: 6c5f 636f 6e66 6967 7572 6528 5b27 5152  l_configure(['QR
+00006e60: 5950 444e 275d 290a 2020 2020 2020 2020  YPDN']).        
+00006e70: 2020 2020 6966 2027 4e4c 532d 4e31 2720      if 'NLS-N1' 
+00006e80: 696e 2073 7472 2872 6573 293a 0a20 2020  in str(res):.   
+00006e90: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00006ea0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00006eb0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00006ec0: 650a 2020 2020 2020 2020 6578 6365 7074  e.        except
+00006ed0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00006ee0: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+00006ef0: 6465 6620 636f 6e66 6967 7572 6528 7365  def configure(se
+00006f00: 6c66 2c20 696c 6c5f 7363 6e3d 2731 272c  lf, ill_scn='1',
+00006f10: 2061 6d6c 5f65 6e61 3d27 3127 2c20 6772   aml_ena='1', gr
+00006f20: 625f 656e 613d 2730 272c 2067 7262 5f76  b_ena='0', grb_v
+00006f30: 6c6c 3d27 3227 2c20 6174 735f 656e 613d  ll='2', ats_ena=
+00006f40: 2730 272c 2061 7473 5f64 7572 3d27 3336  '0', ats_dur='36
+00006f50: 3030 3027 2c20 7363 6e5f 6d6f 643d 2730  000', scn_mod='0
+00006f60: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00006f70: 2020 2020 2070 7762 5f65 6e61 3d27 3027       pwb_ena='0'
+00006f80: 2c20 7272 6472 5f65 6e3d 2731 272c 2067  , rrdr_en='1', g
+00006f90: 7264 5f65 6e61 3d27 3027 2c20 6772 645f  rd_ena='0', grd_
+00006fa0: 6475 723d 2731 272c 2074 696d 655f 6f75  dur='1', time_ou
+00006fb0: 743d 2731 3027 2c20 6261 645f 6d73 675f  t='10', bad_msg_
+00006fc0: 656e 3d54 7275 652c 2073 796d 626f 6c6f  en=True, symbolo
+00006fd0: 6769 6573 3d4e 6f6e 6529 3a0a 2020 2020  gies=None):.    
+00006fe0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00006ff0: 696c 6c5f 7363 6e20 2d20 696c 6c75 6d69  ill_scn - illumi
+00007000: 6e61 7469 6f6e 3a20 2020 2020 2020 2020  nation:         
+00007010: 302d 6f66 662c 2031 2d6e 6f72 6d61 6c2c  0-off, 1-normal,
+00007020: 2032 2d61 6c77 6179 7320 6f6e 0a20 2020   2-always on.   
+00007030: 2020 2020 2061 6d6c 5f65 6e61 202d 2061       aml_ena - a
+00007040: 696d 696e 673a 2020 2020 2020 2020 2020  iming:          
+00007050: 2020 2020 2030 2d6f 6666 2c20 312d 6e6f       0-off, 1-no
+00007060: 726d 616c 2c20 322d 616c 7761 7973 206f  rmal, 2-always o
+00007070: 6e0a 2020 2020 2020 2020 7077 625f 656e  n.        pwb_en
+00007080: 6120 2d20 706f 7765 7220 6f6e 2062 6565  a - power on bee
+00007090: 7020 2020 2020 2020 2020 302d 6f66 662c  p         0-off,
+000070a0: 2031 2d6f 6e0a 2020 2020 2020 2020 6772   1-on.        gr
+000070b0: 625f 656e 6120 2d20 676f 6f64 2072 6561  b_ena - good rea
+000070c0: 6420 6265 6570 2020 2020 2020 2020 302d  d beep        0-
+000070d0: 6f66 662c 2031 2d6f 6e0a 2020 2020 2020  off, 1-on.      
+000070e0: 2020 6772 645f 656e 6120 2d20 676f 6f64    grd_ena - good
+000070f0: 2072 6561 6420 656e 6162 6c65 2020 2020   read enable    
+00007100: 2020 302d 6f66 662c 2031 2d6f 6e0a 2020    0-off, 1-on.  
+00007110: 2020 2020 2020 6772 645f 6475 7220 2d20        grd_dur - 
+00007120: 676f 6f64 2072 6561 6420 6475 7261 7469  good read durati
+00007130: 6f6e 2020 2020 312d 3336 3030 3020 5b6d  on    1-36000 [m
+00007140: 7365 635d 0a20 2020 2020 2020 2061 7473  sec].        ats
+00007150: 5f65 6e61 202d 2061 7574 6f20 736c 6565  _ena - auto slee
+00007160: 7020 2020 2020 2020 2020 2020 2030 2d64  p            0-d
+00007170: 6973 6162 6c65 2c20 312d 656e 6162 6c65  isable, 1-enable
+00007180: 0a20 2020 2020 2020 2061 7473 5f64 7572  .        ats_dur
+00007190: 202d 2073 6c65 6570 2064 7572 6174 696f   - sleep duratio
+000071a0: 6e20 2020 2020 2020 2031 2d33 3630 3030  n        1-36000
+000071b0: 205b 7365 635d 0a20 2020 2020 2020 2072   [sec].        r
+000071c0: 7264 725f 656e 202d 2052 6572 6561 6420  rdr_en - Reread 
+000071d0: 7265 7365 7420 2020 2020 2020 2020 2030  reset          0
+000071e0: 2d6f 6666 2c20 312d 6f6e 0a20 2020 2020  -off, 1-on.     
+000071f0: 2020 2073 636e 5f6d 6f64 202d 2073 6361     scn_mod - sca
+00007200: 6e20 6d6f 6465 2020 2020 2020 2020 2020  n mode          
+00007210: 2020 2030 2d6c 6576 656c 206d 6f64 652c     0-level mode,
+00007220: 2032 2d73 656e 7365 206d 6f64 652c 2033   2-sense mode, 3
+00007230: 2d63 6f6e 7469 6e75 6f75 7320 6d6f 6465  -continuous mode
+00007240: 2c20 372d 6261 7463 6820 6d6f 6465 0a20  , 7-batch mode. 
+00007250: 2020 2020 2020 2073 796d 626f 6c6f 6769         symbologi
+00007260: 6573 202d 2061 206c 6973 7420 6f66 2073  es - a list of s
+00007270: 7472 696e 6773 2072 6570 7265 7365 6e74  trings represent
+00007280: 696e 6720 7468 6520 7379 6d62 6f6c 6f67  ing the symbolog
+00007290: 6965 7320 746f 2065 6e61 626c 652c 2065  ies to enable, e
+000072a0: 2e67 2e20 5b27 5152 272c 2027 5044 4634  .g. ['QR', 'PDF4
+000072b0: 3137 272c 2027 4541 4e31 3327 5d0a 0a20  17', 'EAN13'].. 
+000072c0: 2020 2020 2020 204c 6576 656c 204d 6f64         Level Mod
+000072d0: 653a 0a20 2020 2020 2020 2049 6e20 7468  e:.        In th
+000072e0: 6973 206d 6f64 652c 2074 6865 2073 6361  is mode, the sca
+000072f0: 6e6e 6572 2077 6169 7473 2066 6f72 2061  nner waits for a
+00007300: 2074 7269 6767 6572 2070 756c 6c20 746f   trigger pull to
+00007310: 2061 6374 6976 6174 6520 6120 6465 636f   activate a deco
+00007320: 6465 2073 6573 7369 6f6e 2e20 5468 6520  de session. The 
+00007330: 6465 636f 6465 2073 6573 7369 6f6e 2063  decode session c
+00007340: 6f6e 7469 6e75 6573 2075 6e74 696c 2061  ontinues until a
+00007350: 2062 6172 636f 6465 2069 7320 6465 636f   barcode is deco
+00007360: 6465 6420 6f72 2079 6f75 2072 656c 6561  ded or you relea
+00007370: 7365 2074 6865 2074 7269 6767 6572 2e0a  se the trigger..
+00007380: 2020 2020 2020 2020 436f 6d6d 616e 6420          Command 
+00007390: 7472 6967 6765 7220 6d6f 6465 3a0a 2020  trigger mode:.  
+000073a0: 2020 2020 2020 5468 6973 206d 6f64 6520        This mode 
+000073b0: 7265 7175 6972 6573 2079 6f75 2074 6f20  requires you to 
+000073c0: 7365 6e64 2061 2063 6f6d 6d61 6e64 2028  send a command (
+000073d0: 3142 2033 3120 696e 2068 6578 2920 746f  1B 31 in hex) to
+000073e0: 2061 6374 6976 6174 6520 6120 6465 636f   activate a deco
+000073f0: 6465 2073 6573 7369 6f6e 2e0a 0a20 2020  de session...   
+00007400: 2020 2020 2053 656e 7365 204d 6f64 653a       Sense Mode:
+00007410: 0a20 2020 2020 2020 2049 6e20 7468 6973  .        In this
+00007420: 206d 6f64 652c 2074 6865 2073 6361 6e6e   mode, the scann
+00007430: 6572 2061 6374 6976 6174 6573 2061 2064  er activates a d
+00007440: 6563 6f64 6520 7365 7373 696f 6e20 6576  ecode session ev
+00007450: 6572 7920 7469 6d65 2069 7420 6465 7465  ery time it dete
+00007460: 6374 7320 6120 6261 7263 6f64 6520 7072  cts a barcode pr
+00007470: 6573 656e 7465 6420 746f 2069 742e 2054  esented to it. T
+00007480: 6865 2064 6563 6f64 6520 7365 7373 696f  he decode sessio
+00007490: 6e20 636f 6e74 696e 7565 7320 756e 7469  n continues unti
+000074a0: 6c20 6120 6261 7263 6f64 6520 6973 2064  l a barcode is d
+000074b0: 6563 6f64 6564 206f 7220 7468 6520 6465  ecoded or the de
+000074c0: 636f 6465 2073 6573 7369 6f6e 2074 696d  code session tim
+000074d0: 656f 7574 2065 7870 6972 6573 2e20 596f  eout expires. Yo
+000074e0: 7520 6361 6e20 6164 6a75 7374 2074 6865  u can adjust the
+000074f0: 2073 656e 7369 7469 7669 7479 2061 6e64   sensitivity and
+00007500: 2072 6572 6561 6420 7469 6d65 6f75 7420   reread timeout 
+00007510: 746f 2061 766f 6964 2075 6e64 6573 6972  to avoid undesir
+00007520: 6564 2072 6572 6561 6469 6e67 206f 6620  ed rereading of 
+00007530: 7468 6520 7361 6d65 2062 6172 636f 6465  the same barcode
+00007540: 2069 6e20 6120 6769 7665 6e20 7065 7269   in a given peri
+00007550: 6f64 206f 6620 7469 6d65 2e20 596f 7520  od of time. You 
+00007560: 6361 6e20 616c 736f 2061 646a 7573 7420  can also adjust 
+00007570: 7468 6520 696d 6167 6520 7374 6162 696c  the image stabil
+00007580: 697a 6174 696f 6e20 7469 6d65 6f75 7420  ization timeout 
+00007590: 746f 2067 6976 6520 7468 6520 7363 616e  to give the scan
+000075a0: 6e65 7220 7469 6d65 2074 6f20 6164 6170  ner time to adap
+000075b0: 7420 746f 2061 6d62 6965 6e74 2065 6e76  t to ambient env
+000075c0: 6972 6f6e 6d65 6e74 2061 6674 6572 2069  ironment after i
+000075d0: 7420 6465 636f 6465 7320 6120 6261 7263  t decodes a barc
+000075e0: 6f64 6520 616e 6420 e280 9c6c 6f6f 6b73  ode and ...looks
+000075f0: e280 9d20 666f 7220 616e 6f74 6865 722e  ... for another.
+00007600: 0a0a 2020 2020 2020 2020 436f 6e74 696e  ..        Contin
+00007610: 756f 7573 204d 6f64 653a 0a20 2020 2020  uous Mode:.     
+00007620: 2020 2049 6e20 7468 6973 206d 6f64 652c     In this mode,
+00007630: 2074 6865 2073 6361 6e6e 6572 2061 7574   the scanner aut
+00007640: 6f6d 6174 6963 616c 6c79 2073 7461 7274  omatically start
+00007650: 7320 6f6e 6520 6465 636f 6465 2073 6573  s one decode ses
+00007660: 7369 6f6e 2061 6674 6572 2061 6e6f 7468  sion after anoth
+00007670: 6572 2e20 546f 2073 7573 7065 6e64 2f72  er. To suspend/r
+00007680: 6573 756d 6520 6261 7263 6f64 6520 7265  esume barcode re
+00007690: 6164 696e 672c 2073 696d 706c 7920 7072  ading, simply pr
+000076a0: 6573 7320 7468 6520 7472 6967 6765 722e  ess the trigger.
+000076b0: 2059 6f75 2063 616e 2061 646a 7573 7420   You can adjust 
+000076c0: 7468 6520 7265 7265 6164 2074 696d 656f  the reread timeo
+000076d0: 7574 2074 6f20 6176 6f69 6420 756e 6465  ut to avoid unde
+000076e0: 7369 7265 6420 7265 7265 6164 696e 6720  sired rereading 
+000076f0: 6f66 2074 6865 2073 616d 6520 6261 7263  of the same barc
+00007700: 6f64 6520 696e 2061 2067 6976 656e 2070  ode in a given p
+00007710: 6572 696f 6420 6f66 2074 696d 652e 204e  eriod of time. N
+00007720: 6f74 6520 7468 6174 2077 6865 6e20 7377  ote that when sw
+00007730: 6974 6368 696e 6720 746f 2074 6869 7320  itching to this 
+00007740: 6d6f 6465 2062 7920 7363 616e 6e69 6e67  mode by scanning
+00007750: 2074 6865 2043 6f6e 7469 6e75 6f75 7320   the Continuous 
+00007760: 4d6f 6465 2062 6172 636f 6465 2c20 7468  Mode barcode, th
+00007770: 6520 7363 616e 6e65 7220 7769 6c6c 2073  e scanner will s
+00007780: 746f 7020 6261 7263 6f64 6520 7265 6164  top barcode read
+00007790: 696e 6720 666f 7220 3320 7365 636f 6e64  ing for 3 second
+000077a0: 7320 6265 666f 7265 2073 7461 7274 696e  s before startin
+000077b0: 6720 7363 616e 6e69 6e67 2063 6f6e 7469  g scanning conti
+000077c0: 6e75 6f75 736c 792e 0a0a 2020 2020 2020  nuously...      
+000077d0: 2020 4261 7463 6820 4d6f 6465 3a0a 2020    Batch Mode:.  
+000077e0: 2020 2020 2020 496e 2074 6869 7320 6d6f        In this mo
+000077f0: 6465 2c20 6120 7472 6967 6765 7220 7075  de, a trigger pu
+00007800: 6c6c 2061 6374 6976 6174 6573 2061 2072  ll activates a r
+00007810: 6f75 6e64 206f 6620 6d75 6c74 6970 6c65  ound of multiple
+00007820: 2064 6563 6f64 6520 7365 7373 696f 6e73   decode sessions
+00007830: 2e20 5468 6520 726f 756e 6420 6f66 206d  . The round of m
+00007840: 756c 7469 706c 6520 7363 616e 7320 636f  ultiple scans co
+00007850: 6e74 696e 7565 7320 756e 7469 6c20 796f  ntinues until yo
+00007860: 7520 7265 6c65 6173 6520 7468 6520 7472  u release the tr
+00007870: 6967 6765 722e 2052 6572 6561 6469 6e67  igger. Rereading
+00007880: 2074 6865 2073 616d 6520 6261 7263 6f64   the same barcod
+00007890: 6520 6973 206e 6f74 2061 6c6c 6f77 6564  e is not allowed
+000078a0: 2069 6e20 7468 6520 7361 6d65 2072 6f75   in the same rou
+000078b0: 6e64 2e0a 2020 2020 2020 2020 2727 270a  nd..        '''.
+000078c0: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
+000078d0: 3129 0a20 2020 2020 2020 2070 6172 616d  1).        param
+000078e0: 7320 3d20 7b27 494c 4c53 434e 273a 2069  s = {'ILLSCN': i
+000078f0: 6c6c 5f73 636e 2c20 2741 4d4c 454e 4127  ll_scn, 'AMLENA'
+00007900: 3a20 616d 6c5f 656e 612c 2027 4752 4245  : aml_ena, 'GRBE
+00007910: 4e41 273a 2067 7262 5f65 6e61 2c20 2741  NA': grb_ena, 'A
+00007920: 5453 454e 4127 3a20 6174 735f 656e 612c  TSENA': ats_ena,
+00007930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007940: 2020 2027 4e47 5245 4e41 273a 2027 3127     'NGRENA': '1'
+00007950: 2069 6620 6261 645f 6d73 675f 656e 2065   if bad_msg_en e
+00007960: 6c73 6520 2730 272c 0a20 2020 2020 2020  lse '0',.       
+00007970: 2020 2020 2020 2020 2020 2027 4752 4256             'GRBV
+00007980: 4c4c 273a 2067 7262 5f76 6c6c 2c20 2741  LL': grb_vll, 'A
+00007990: 5453 4455 5227 3a20 6174 735f 6475 722c  TSDUR': ats_dur,
+000079a0: 2027 5343 4e4d 4f44 273a 2073 636e 5f6d   'SCNMOD': scn_m
+000079b0: 6f64 2c20 2752 5244 5245 4e27 3a20 7272  od, 'RRDREN': rr
+000079c0: 6472 5f65 6e2c 2027 4752 4445 4e41 273a  dr_en, 'GRDENA':
+000079d0: 2067 7264 5f65 6e61 2c0a 2020 2020 2020   grd_ena,.      
+000079e0: 2020 2020 2020 2020 2020 2020 2747 5244              'GRD
+000079f0: 4455 5227 3a20 6772 645f 6475 722c 0a20  DUR': grd_dur,. 
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 2027 5057 4245 4e41 273a 2070 7762 5f65   'PWBENA': pwb_e
+00007a20: 6e61 2c20 274f 5254 5345 5427 3a20 7469  na, 'ORTSET': ti
+00007a30: 6d65 5f6f 7574 7d0a 2020 2020 2020 2020  me_out}.        
+00007a40: 7061 7261 6d73 203d 205b 6b65 7920 2b20  params = [key + 
+00007a50: 7661 6c75 6520 666f 7220 6b65 792c 2076  value for key, v
+00007a60: 616c 7565 2069 6e20 7061 7261 6d73 2e69  alue in params.i
+00007a70: 7465 6d73 2829 5d0a 0a20 2020 2020 2020  tems()]..       
+00007a80: 2069 6620 7379 6d62 6f6c 6f67 6965 7320   if symbologies 
+00007a90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007aa0: 2020 2020 2020 2020 2066 6f72 2073 796d           for sym
+00007ab0: 626f 6c6f 6779 2069 6e20 7379 6d62 6f6c  bology in symbol
+00007ac0: 6f67 6965 733a 0a20 2020 2020 2020 2020  ogies:.         
+00007ad0: 2020 2020 2020 2070 6172 616d 732e 6170         params.ap
+00007ae0: 7065 6e64 2827 5359 4d42 5f27 202b 2073  pend('SYMB_' + s
+00007af0: 796d 626f 6c6f 6779 202b 2027 3127 290a  ymbology + '1').
+00007b00: 0a20 2020 2020 2020 2074 2c20 6973 5375  .        t, isSu
+00007b10: 6363 6573 7320 3d20 7365 6c66 2e6d 616e  ccess = self.man
+00007b20: 7561 6c5f 636f 6e66 6967 7572 6528 7061  ual_configure(pa
+00007b30: 7261 6d73 290a 2020 2020 2020 2020 6966  rams).        if
+00007b40: 2069 7353 7563 6365 7373 2061 6e64 2073   isSuccess and s
+00007b50: 656c 662e 6c6f 675f 7479 7065 2021 3d20  elf.log_type != 
+00007b60: 274e 4f5f 4c4f 4727 3a0a 2020 2020 2020  'NO_LOG':.      
+00007b70: 2020 2020 2020 7365 6c66 2e71 725f 6c6f        self.qr_lo
+00007b80: 6767 6572 2e69 6e66 6f28 6627 4261 7263  gger.info(f'Barc
+00007b90: 6f64 6520 7363 616e 6e65 7220 287b 7365  ode scanner ({se
+00007ba0: 6c66 2e63 6f6d 5f70 6f72 747d 2920 636f  lf.com_port}) co
+00007bb0: 6e66 6967 7572 6564 2073 7563 6365 7373  nfigured success
+00007bc0: 6675 6c6c 792e 2729 0a20 2020 2020 2020  fully.').       
+00007bd0: 2065 6c69 6620 6e6f 7420 6973 5375 6363   elif not isSucc
+00007be0: 6573 733a 0a20 2020 2020 2020 2020 2020  ess:.           
+00007bf0: 2073 656c 662e 7172 5f6c 6f67 6765 722e   self.qr_logger.
+00007c00: 6572 726f 7228 6627 4261 7263 6f64 6520  error(f'Barcode 
+00007c10: 7363 616e 6e65 7220 287b 7365 6c66 2e63  scanner ({self.c
+00007c20: 6f6d 5f70 6f72 747d 2920 636f 6e66 6967  om_port}) config
+00007c30: 7572 6174 696f 6e20 6661 696c 6564 2e27  uration failed.'
+00007c40: 290a 0a20 2020 2064 6566 2072 6573 746f  )..    def resto
+00007c50: 7265 5f61 6c6c 5f66 6163 746f 7279 5f64  re_all_factory_d
+00007c60: 6566 6175 6c74 7328 7365 6c66 293a 0a20  efaults(self):. 
+00007c70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00007c80: 2020 2052 6573 746f 7265 2061 6c6c 2066     Restore all f
+00007c90: 6163 746f 7279 2064 6566 6175 6c74 732e  actory defaults.
+00007ca0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007cb0: 2020 2020 2073 6c65 6570 2830 2e31 290a       sleep(0.1).
+00007cc0: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+00007cd0: 207b 2746 4143 4445 4627 3a20 2727 7d0a   {'FACDEF': ''}.
+00007ce0: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+00007cf0: 205b 6b65 7920 2b20 7661 6c75 6520 666f   [key + value fo
+00007d00: 7220 6b65 792c 2076 616c 7565 2069 6e20  r key, value in 
+00007d10: 7061 7261 6d73 2e69 7465 6d73 2829 5d0a  params.items()].
+00007d20: 2020 2020 2020 2020 742c 2069 7353 7563          t, isSuc
+00007d30: 6365 7373 203d 2073 656c 662e 6d61 6e75  cess = self.manu
+00007d40: 616c 5f63 6f6e 6669 6775 7265 2870 6172  al_configure(par
+00007d50: 616d 7329 0a20 2020 2020 2020 2069 6620  ams).        if 
+00007d60: 6973 5375 6363 6573 7320 616e 6420 7365  isSuccess and se
+00007d70: 6c66 2e6c 6f67 5f74 7970 6520 213d 2027  lf.log_type != '
+00007d80: 4e4f 5f4c 4f47 273a 0a20 2020 2020 2020  NO_LOG':.       
+00007d90: 2020 2020 2073 656c 662e 7172 5f6c 6f67       self.qr_log
+00007da0: 6765 722e 696e 666f 2866 2742 6172 636f  ger.info(f'Barco
+00007db0: 6465 2073 6361 6e6e 6572 2028 7b73 656c  de scanner ({sel
+00007dc0: 662e 636f 6d5f 706f 7274 7d29 2072 6573  f.com_port}) res
+00007dd0: 746f 7265 6420 6661 6374 6f72 7920 6465  tored factory de
+00007de0: 6661 756c 7420 7375 6363 6573 7366 756c  fault successful
+00007df0: 6c79 2e27 290a 2020 2020 2020 2020 656c  ly.').        el
+00007e00: 6966 206e 6f74 2069 7353 7563 6365 7373  if not isSuccess
+00007e10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007e20: 6c66 2e71 725f 6c6f 6767 6572 2e65 7272  lf.qr_logger.err
+00007e30: 6f72 2866 2742 6172 636f 6465 2073 6361  or(f'Barcode sca
+00007e40: 6e6e 6572 2028 7b73 656c 662e 636f 6d5f  nner ({self.com_
+00007e50: 706f 7274 7d29 2072 6573 746f 7265 6420  port}) restored 
+00007e60: 6661 6374 6f72 7920 6465 6661 756c 7420  factory default 
+00007e70: 6661 696c 6564 2e27 290a 0a20 2020 2064  failed.')..    d
+00007e80: 6566 206d 616e 7561 6c5f 636f 6e66 6967  ef manual_config
+00007e90: 7572 6528 7365 6c66 2c20 7061 7261 6d73  ure(self, params
+00007ea0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00007eb0: 2020 2020 2020 204d 616e 7561 6c6c 7920         Manually 
+00007ec0: 636f 6e66 6967 7572 6520 7468 6520 7363  configure the sc
+00007ed0: 616e 6e65 722e 0a20 2020 2020 2020 2022  anner..        "
+00007ee0: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00007ef0: 7365 7269 616c 5f63 6f6e 6e65 6374 696f  serial_connectio
+00007f00: 6e2e 666c 7573 6849 6e70 7574 2829 0a20  n.flushInput(). 
+00007f10: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00007f20: 616c 5f63 6f6e 6e65 6374 696f 6e2e 666c  al_connection.fl
+00007f30: 7573 684f 7574 7075 7428 290a 2020 2020  ushOutput().    
+00007f40: 2020 2020 736c 6565 7028 302e 3129 0a20      sleep(0.1). 
+00007f50: 2020 2020 2020 2062 6164 5f6d 7367 203d         bad_msg =
+00007f60: 2027 3436 3064 3061 2720 2023 2034 3620   '460d0a'  # 46 
+00007f70: 3d20 462c 2023 3064 203d 202f 7220 2330  = F, #0d = /r #0
+00007f80: 6120 3d20 2f6e 202d 3e20 6d65 616e 7320  a = /n -> means 
+00007f90: 7468 6174 2065 7665 7279 2065 7272 6f72  that every error
+00007fa0: 206f 7220 6465 636f 6e64 696e 6720 7469   or deconding ti
+00007fb0: 6d65 6f75 7420 7769 6c6c 2073 656e 6420  meout will send 
+00007fc0: 7468 6520 6d65 7373 6167 6520 462f 722f  the message F/r/
+00007fd0: 6e20 2d3e 2077 696c 6c20 6265 2074 7261  n -> will be tra
+00007fe0: 6e73 6c61 7465 6420 6279 2073 6572 6961  nslated by seria
+00007ff0: 6c20 6c69 6220 6173 2046 3c4e 6577 4c69  l lib as F<NewLi
+00008000: 6e65 3e0a 2020 2020 2020 2020 656e 7465  ne>.        ente
+00008010: 725f 7365 7475 705f 6d6f 6465 203d 2027  r_setup_mode = '
+00008020: 5345 5455 5045 3127 0a20 2020 2020 2020  SETUPE1'.       
+00008030: 2065 7869 745f 7365 7475 705f 6d6f 6465   exit_setup_mode
+00008040: 203d 2027 5345 5455 5045 3027 0a20 2020   = 'SETUPE0'.   
+00008050: 2020 2020 2023 2045 6e74 6572 2073 6574       # Enter set
+00008060: 7570 206d 6f64 650a 2020 2020 2020 2020  up mode.        
+00008070: 7365 6c66 2e73 6572 6961 6c5f 636f 6e6e  self.serial_conn
+00008080: 6563 7469 6f6e 2e77 7269 7465 2873 7472  ection.write(str
+00008090: 2e65 6e63 6f64 6528 7365 6c66 2e70 7265  .encode(self.pre
+000080a0: 6669 7820 2b20 656e 7465 725f 7365 7475  fix + enter_setu
+000080b0: 705f 6d6f 6465 202b 2073 656c 662e 7375  p_mode + self.su
+000080c0: 6666 6978 2929 0a20 2020 2020 2020 2023  ffix)).        #
+000080d0: 2049 6e73 6572 7420 636f 6e66 6967 7572   Insert configur
+000080e0: 6174 696f 6e0a 2020 2020 2020 2020 636f  ation.        co
+000080f0: 6e66 6967 7320 3d20 7365 6c66 2e70 7265  nfigs = self.pre
+00008100: 6669 7820 2b20 273b 272e 6a6f 696e 2870  fix + ';'.join(p
+00008110: 6172 616d 7329 202b 2073 656c 662e 7375  arams) + self.su
+00008120: 6666 6978 0a20 2020 2020 2020 2073 656c  ffix.        sel
+00008130: 662e 7365 7269 616c 5f63 6f6e 6e65 6374  f.serial_connect
+00008140: 696f 6e2e 7772 6974 6528 7374 722e 656e  ion.write(str.en
+00008150: 636f 6465 2863 6f6e 6669 6773 2929 0a20  code(configs)). 
+00008160: 2020 2020 2020 2069 6620 274e 4752 454e         if 'NGREN
+00008170: 4131 2720 696e 2070 6172 616d 733a 0a20  A1' in params:. 
+00008180: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008190: 7365 7269 616c 5f63 6f6e 6e65 6374 696f  serial_connectio
+000081a0: 6e2e 7772 6974 6528 0a20 2020 2020 2020  n.write(.       
+000081b0: 2020 2020 2020 2020 2073 7472 2e65 6e63           str.enc
+000081c0: 6f64 6528 7365 6c66 2e70 7265 6669 7820  ode(self.prefix 
+000081d0: 2b20 274e 4752 5345 5427 202b 2062 6164  + 'NGRSET' + bad
+000081e0: 5f6d 7367 202b 2073 656c 662e 7375 6666  _msg + self.suff
+000081f0: 6978 2929 2020 2320 5365 7420 6d65 7373  ix))  # Set mess
+00008200: 6167 6520 746f 2065 6d70 7479 0a20 2020  age to empty.   
+00008210: 2020 2020 2069 6620 2753 434e 4d4f 4432       if 'SCNMOD2
+00008220: 2720 696e 2070 6172 616d 733a 0a20 2020  ' in params:.   
+00008230: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00008240: 7269 616c 5f63 6f6e 6e65 6374 696f 6e2e  rial_connection.
+00008250: 7772 6974 6528 0a20 2020 2020 2020 2020  write(.         
+00008260: 2020 2020 2020 2073 7472 2e65 6e63 6f64         str.encod
+00008270: 6528 7365 6c66 2e70 7265 6669 7820 2b20  e(self.prefix + 
+00008280: 2753 454e 4c56 4c35 2720 2b20 6261 645f  'SENLVL5' + bad_
+00008290: 6d73 6720 2b20 7365 6c66 2e73 7566 6669  msg + self.suffi
+000082a0: 7829 2920 2023 2053 6574 2073 656e 7369  x))  # Set sensi
+000082b0: 7469 7669 7479 2074 6f20 6869 6768 2031  tivity to high 1
+000082c0: 2d32 300a 2020 2020 2020 2020 2320 4578  -20.        # Ex
+000082d0: 6974 2073 6574 7570 206d 6f64 650a 2020  it setup mode.  
+000082e0: 2020 2020 2020 7365 6c66 2e73 6572 6961        self.seria
+000082f0: 6c5f 636f 6e6e 6563 7469 6f6e 2e77 7269  l_connection.wri
+00008300: 7465 2873 7472 2e65 6e63 6f64 6528 7365  te(str.encode(se
+00008310: 6c66 2e70 7265 6669 7820 2b20 6578 6974  lf.prefix + exit
+00008320: 5f73 6574 7570 5f6d 6f64 6520 2b20 7365  _setup_mode + se
+00008330: 6c66 2e73 7566 6669 7829 290a 2020 2020  lf.suffix)).    
+00008340: 2020 2020 736c 6565 7028 302e 3129 0a20      sleep(0.1). 
+00008350: 2020 2020 2020 2074 2c20 6973 5375 6363         t, isSucc
+00008360: 6573 7320 3d20 7365 6c66 2e74 7269 6767  ess = self.trigg
+00008370: 6572 5f73 746f 705f 7365 7474 696e 6773  er_stop_settings
+00008380: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00008390: 6e20 742c 2069 7353 7563 6365 7373 0a0a  n t, isSuccess..
+000083a0: 2020 2020 6465 6620 7363 616e 2873 656c      def scan(sel
+000083b0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+000083c0: 2020 2020 2020 2020 5363 616e 2074 6865          Scan the
+000083d0: 2051 5220 636f 6465 2e0a 2020 2020 2020   QR code..      
+000083e0: 2020 2222 220a 2020 2020 2020 2020 7420    """.        t 
+000083f0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2074  = None.        t
+00008400: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00008410: 7365 6c66 2e73 6572 6961 6c5f 636f 6e6e  self.serial_conn
+00008420: 6563 7469 6f6e 2e77 7269 7465 2862 225c  ection.write(b"\
+00008430: 7831 625c 7833 3122 290a 2020 2020 2020  x1b\x31").      
+00008440: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00008450: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00008460: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00008470: 7469 6f6e 2866 2753 6361 6e6e 6572 3a20  tion(f'Scanner: 
+00008480: 4572 726f 7220 7365 6e64 696e 6720 6d65  Error sending me
+00008490: 7373 6167 6520 7468 726f 7567 6820 5541  ssage through UA
+000084a0: 5254 2d20 4368 6563 6b20 636f 6e6e 6563  RT- Check connec
+000084b0: 7469 6f6e 207b 657d 2729 0a20 2020 2020  tion {e}').     
+000084c0: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
+000084d0: 6461 7465 7469 6d65 2e6e 6f77 2829 0a20  datetime.now(). 
+000084e0: 2020 2020 2020 2074 203d 2073 656c 662e         t = self.
+000084f0: 7365 7269 616c 5f63 6f6e 6e65 6374 696f  serial_connectio
+00008500: 6e2e 7265 6164 6c69 6e65 2829 0a20 2020  n.readline().   
+00008510: 2020 2020 2065 6e64 5f74 696d 6520 3d20       end_time = 
+00008520: 6461 7465 7469 6d65 2e6e 6f77 2829 0a20  datetime.now(). 
+00008530: 2020 2020 2020 2065 6c61 7073 6564 5f74         elapsed_t
+00008540: 696d 655f 6d73 203d 2028 656e 645f 7469  ime_ms = (end_ti
+00008550: 6d65 202d 2073 7461 7274 5f74 696d 6529  me - start_time)
+00008560: 2e74 6f74 616c 5f73 6563 6f6e 6473 2829  .total_seconds()
+00008570: 202a 2031 3030 300a 2020 2020 2020 2020   * 1000.        
+00008580: 7265 7475 726e 2074 2c20 656c 6170 7365  return t, elapse
+00008590: 645f 7469 6d65 5f6d 730a 0a20 2020 2064  d_time_ms..    d
+000085a0: 6566 2073 6361 6e5f 616e 645f 666c 7573  ef scan_and_flus
+000085b0: 6828 7365 6c66 293a 0a20 2020 2020 2020  h(self):.       
+000085c0: 2022 2222 0a20 2020 2020 2020 2053 6361   """.        Sca
+000085d0: 6e20 7468 6520 5152 2063 6f64 6520 616e  n the QR code an
+000085e0: 6420 666c 7573 6820 7468 6520 6275 6666  d flush the buff
+000085f0: 6572 2e0a 2020 2020 2020 2020 2222 220a  er..        """.
+00008600: 2020 2020 2020 2020 6465 6620 636c 6561          def clea
+00008610: 6e5f 7363 616e 5f66 2869 6e70 7574 5f73  n_scan_f(input_s
+00008620: 6361 6e29 3a0a 2020 2020 2020 2020 2020  can):.          
+00008630: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00008640: 2020 2020 2020 2064 6563 6f64 6564 5f73         decoded_s
+00008650: 6361 6e20 3d20 696e 7075 745f 7363 616e  can = input_scan
+00008660: 2e64 6563 6f64 6528 290a 2020 2020 2020  .decode().      
+00008670: 2020 2020 2020 2020 2020 7374 7269 7070            stripp
+00008680: 6564 5f73 6361 6e20 3d20 6465 636f 6465  ed_scan = decode
+00008690: 645f 7363 616e 2e73 7472 6970 2829 0a20  d_scan.strip(). 
+000086a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000086b0: 6c65 616e 5f73 7472 203d 2073 7472 6970  lean_str = strip
+000086c0: 7065 645f 7363 616e 2e72 6570 6c61 6365  ped_scan.replace
+000086d0: 2827 5c72 5c6e 272c 2027 2729 2e72 6570  ('\r\n', '').rep
+000086e0: 6c61 6365 2827 5c78 3036 272c 2027 2729  lace('\x06', '')
+000086f0: 2e72 6570 6c61 6365 2827 5c78 3031 272c  .replace('\x01',
+00008700: 2027 2729 0a20 2020 2020 2020 2020 2020   '').           
+00008710: 2020 2020 2072 6574 7572 6e20 636c 6561       return clea
+00008720: 6e5f 7374 720a 2020 2020 2020 2020 2020  n_str.          
+00008730: 2020 6578 6365 7074 2055 6e69 636f 6465    except Unicode
+00008740: 4465 636f 6465 4572 726f 723a 0a20 2020  DecodeError:.   
+00008750: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00008760: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+00008770: 2020 6966 2073 656c 662e 7365 7269 616c    if self.serial
+00008780: 5f63 6f6e 6e65 6374 696f 6e20 6973 204e  _connection is N
+00008790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000087a0: 2073 656c 662e 7172 5f6c 6f67 6765 722e   self.qr_logger.
+000087b0: 6572 726f 7228 2245 7272 6f72 3a20 5365  error("Error: Se
+000087c0: 7269 616c 206f 626a 6563 7420 6e6f 7420  rial object not 
+000087d0: 696e 6974 6961 6c69 7a65 6422 290a 2020  initialized").  
+000087e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000087f0: 204e 6f6e 650a 0a20 2020 2020 2020 2073   None..        s
+00008800: 6361 6e6e 6564 2c20 656c 6170 7365 645f  canned, elapsed_
+00008810: 7469 6d65 5f6d 7320 3d20 7365 6c66 2e73  time_ms = self.s
+00008820: 6361 6e28 290a 0a20 2020 2020 2020 2069  can()..        i
+00008830: 6620 7363 616e 6e65 643a 0a20 2020 2020  f scanned:.     
+00008840: 2020 2020 2020 2063 6c65 616e 5f73 6361         clean_sca
+00008850: 6e20 3d20 636c 6561 6e5f 7363 616e 5f66  n = clean_scan_f
+00008860: 2873 6361 6e6e 6564 290a 2020 2020 2020  (scanned).      
+00008870: 2020 2020 2020 6966 2063 6c65 616e 5f73        if clean_s
+00008880: 6361 6e20 3d3d 2027 4627 3a0a 2020 2020  can == 'F':.    
+00008890: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000088a0: 726e 204e 6f6e 652c 2065 6c61 7073 6564  rn None, elapsed
+000088b0: 5f74 696d 655f 6d73 0a20 2020 2020 2020  _time_ms.       
+000088c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000088d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000088e0: 6e20 636c 6561 6e5f 7363 616e 2c20 656c  n clean_scan, el
+000088f0: 6170 7365 645f 7469 6d65 5f6d 730a 0a20  apsed_time_ms.. 
+00008900: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00008910: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00008920: 2e69 735f 6f70 656e 2829 3a0a 2020 2020  .is_open():.    
+00008930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008940: 2e73 6572 6961 6c5f 636f 6e6e 6563 7469  .serial_connecti
+00008950: 6f6e 2e72 6573 6574 5f69 6e70 7574 5f62  on.reset_input_b
+00008960: 7566 6665 7228 290a 2020 2020 2020 2020  uffer().        
+00008970: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
+00008980: 6961 6c5f 636f 6e6e 6563 7469 6f6e 2e72  ial_connection.r
+00008990: 6573 6574 5f6f 7574 7075 745f 6275 6666  eset_output_buff
+000089a0: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
+000089b0: 2020 2020 2073 6c65 6570 2830 2e31 290a       sleep(0.1).
+000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089d0: 7363 616e 6e65 642c 2065 6c61 7073 6564  scanned, elapsed
+000089e0: 5f74 696d 655f 6d73 203d 2073 656c 662e  _time_ms = self.
+000089f0: 7363 616e 2829 0a20 2020 2020 2020 2020  scan().         
+00008a00: 2020 2020 2020 2069 6620 7363 616e 6e65         if scanne
+00008a10: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+00008a20: 2020 2020 2020 2063 6c65 616e 5f73 6361         clean_sca
+00008a30: 6e20 3d20 636c 6561 6e5f 7363 616e 5f66  n = clean_scan_f
+00008a40: 2873 6361 6e6e 6564 290a 2020 2020 2020  (scanned).      
+00008a50: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00008a60: 2063 6c65 616e 5f73 6361 6e20 3d3d 2027   clean_scan == '
+00008a70: 4627 3a0a 2020 2020 2020 2020 2020 2020  F':.            
+00008a80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008a90: 726e 204e 6f6e 652c 2065 6c61 7073 6564  rn None, elapsed
+00008aa0: 5f74 696d 655f 6d73 0a20 2020 2020 2020  _time_ms.       
+00008ab0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00008ac0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00008ad0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00008ae0: 6e20 636c 6561 6e5f 7363 616e 2c20 656c  n clean_scan, el
+00008af0: 6170 7365 645f 7469 6d65 5f6d 730a 2020  apsed_time_ms.  
+00008b00: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00008b10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00008b20: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+00008b30: 6365 7074 696f 6e28 2745 7272 6f72 2072  ception('Error r
+00008b40: 6561 6469 6e67 2062 6172 636f 6465 2064  eading barcode d
+00008b50: 6174 6120 2d20 5365 7269 616c 2070 726f  ata - Serial pro
+00008b60: 626c 656d 2729 0a20 2020 2020 2020 2020  blem').         
+00008b70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00008b80: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+00008b90: 7863 6570 7469 6f6e 2827 4572 726f 7220  xception('Error 
+00008ba0: 696e 2053 6361 6e6e 6572 2053 6572 6961  in Scanner Seria
+00008bb0: 6c20 636f 6e6e 6563 7469 6f6e 2729 0a0a  l connection')..
+00008bc0: 2020 2020 6465 6620 7363 616e 5f65 7874      def scan_ext
+00008bd0: 5f69 6428 7365 6c66 2c20 6e65 6564 5f74  _id(self, need_t
+00008be0: 6f5f 7472 6967 6765 723d 5472 7565 293a  o_trigger=True):
+00008bf0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00008c00: 2020 2020 2053 6361 6e20 7468 6520 6578       Scan the ex
+00008c10: 7465 726e 616c 2049 442e 0a20 2020 2020  ternal ID..     
+00008c20: 2020 2040 7061 7261 6d20 6e65 6564 5f74     @param need_t
+00008c30: 6f5f 7472 6967 6765 7220 746f 206b 6565  o_trigger to kee
+00008c40: 7020 7361 6d65 2062 6568 6176 696f 7220  p same behavior 
+00008c50: 6173 2074 6865 2043 6f67 6e65 780a 2020  as the Cognex.  
+00008c60: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00008c70: 2020 6261 7263 6f64 655f 7265 6164 203d    barcode_read =
+00008c80: 2027 270a 2020 2020 2020 2020 7374 6172   ''.        star
+00008c90: 745f 7469 6d65 203d 2074 696d 6528 290a  t_time = time().
+00008ca0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00008cb0: 2020 2020 2020 2020 2062 6172 636f 6465           barcode
+00008cc0: 5f72 6561 642c 2065 6c61 7073 6564 5f74  _read, elapsed_t
+00008cd0: 696d 655f 6d73 203d 2073 656c 662e 7363  ime_ms = self.sc
+00008ce0: 616e 5f61 6e64 5f66 6c75 7368 2829 0a20  an_and_flush(). 
+00008cf0: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
+00008d00: 7263 6f64 655f 7265 6164 2069 7320 4e6f  rcode_read is No
+00008d10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00008d20: 2020 2020 7265 7475 726e 204e 6f6e 652c      return None,
+00008d30: 204e 6f6e 652c 204e 6f6e 652c 204e 6f6e   None, None, Non
+00008d40: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+00008d50: 6966 2062 6172 636f 6465 5f72 6561 6420  if barcode_read 
+00008d60: 3d3d 2027 273a 0a20 2020 2020 2020 2020  == '':.         
+00008d70: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
+00008d80: 6570 7469 6f6e 2827 4572 726f 7220 696e  eption('Error in
+00008d90: 2053 6361 6e6e 6572 2053 6572 6961 6c20   Scanner Serial 
+00008da0: 636f 6e6e 6563 7469 6f6e 2729 0a20 2020  connection').   
+00008db0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00008dc0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00008dd0: 756c 6c5f 6461 7461 2c20 6375 725f 6964  ull_data, cur_id
+00008de0: 2c20 7265 656c 5f69 642c 2067 7469 6e20  , reel_id, gtin 
+00008df0: 3d20 7365 6c66 2e72 6561 645f 6261 7263  = self.read_barc
+00008e00: 6f64 6528 6261 7263 6f64 655f 7265 6164  ode(barcode_read
+00008e10: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00008e20: 2073 656c 662e 7772 6974 655f 746f 5f6c   self.write_to_l
+00008e30: 6f67 3a0a 2020 2020 2020 2020 2020 2020  og:.            
+00008e40: 2020 2020 7769 7468 206f 7065 6e28 7365      with open(se
+00008e50: 6c66 2e6c 6f67 5f66 696c 656e 616d 652c  lf.log_filename,
+00008e60: 2027 6127 2920 6173 2066 3a0a 2020 2020   'a') as f:.    
+00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e80: 7469 6d65 7374 616d 7020 3d20 6461 7465  timestamp = date
+00008e90: 7469 6d65 2e6e 6f77 2829 2e73 7472 6674  time.now().strft
+00008ea0: 696d 6528 2225 592d 256d 2d25 6420 2548  ime("%Y-%m-%d %H
+00008eb0: 3a25 4d3a 2553 2229 0a20 2020 2020 2020  :%M:%S").       
+00008ec0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00008ed0: 5f6d 6573 7361 6765 203d 2066 227b 7469  _message = f"{ti
+00008ee0: 6d65 7374 616d 707d 202d 207b 6675 6c6c  mestamp} - {full
+00008ef0: 5f64 6174 617d 202d 2045 6c61 7073 6564  _data} - Elapsed
+00008f00: 2054 696d 653a 207b 656c 6170 7365 645f   Time: {elapsed_
+00008f10: 7469 6d65 5f6d 733a 2e32 667d 206d 735c  time_ms:.2f} ms\
+00008f20: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
+00008f30: 2020 2020 2020 2066 2e77 7269 7465 286c         f.write(l
+00008f40: 6f67 5f6d 6573 7361 6765 290a 0a20 2020  og_message)..   
+00008f50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008f60: 6675 6c6c 5f64 6174 612c 2063 7572 5f69  full_data, cur_i
+00008f70: 642c 2072 6565 6c5f 6964 2c20 6774 696e  d, reel_id, gtin
+00008f80: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00008f90: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
+00008fa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008fb0: 2e71 725f 6c6f 6767 6572 2e65 7272 6f72  .qr_logger.error
+00008fc0: 2866 277b 657d 202d 2043 6865 636b 2063  (f'{e} - Check c
+00008fd0: 6f6e 6e65 6374 696f 6e27 290a 2020 2020  onnection').    
+00008fe0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+00008ff0: 6365 7074 696f 6e28 6627 7b65 7d20 2d20  ception(f'{e} - 
+00009000: 4368 6563 6b20 636f 6e6e 6563 7469 6f6e  Check connection
+00009010: 2729 0a0a 2020 2020 6465 6620 7265 6164  ')..    def read
+00009020: 5f62 6172 636f 6465 2873 656c 662c 2062  _barcode(self, b
+00009030: 6172 636f 6465 5f72 6561 6429 3a0a 2020  arcode_read):.  
+00009040: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00009050: 2020 5265 6164 2074 6865 2062 6172 636f    Read the barco
+00009060: 6465 2e0a 2020 2020 2020 2020 2222 220a  de..        """.
+00009070: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00009080: 2020 2020 2020 2020 2069 6620 2728 3031           if '(01
+00009090: 2927 2069 6e20 6261 7263 6f64 655f 7265  )' in barcode_re
+000090a0: 6164 3a0a 2020 2020 2020 2020 2020 2020  ad:.            
+000090b0: 2020 2020 6261 7263 6f64 6573 203d 2062      barcodes = b
+000090c0: 6172 636f 6465 5f72 6561 642e 7370 6c69  arcode_read.spli
+000090d0: 7428 2228 3031 2922 290a 2020 2020 2020  t("(01)").      
+000090e0: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
+000090f0: 2073 696e 676c 655f 6261 7263 6f64 6520   single_barcode 
+00009100: 696e 2065 6e75 6d65 7261 7465 2862 6172  in enumerate(bar
+00009110: 636f 6465 735b 313a 5d2c 2031 293a 0a20  codes[1:], 1):. 
+00009120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009130: 2020 2066 756c 6c5f 6461 7461 203d 2066     full_data = f
+00009140: 2228 3031 297b 7369 6e67 6c65 5f62 6172  "(01){single_bar
+00009150: 636f 6465 7d22 0a20 2020 2020 2020 2020  code}".         
+00009160: 2020 2020 2020 2020 2020 2067 7469 6e20             gtin 
+00009170: 3d20 2729 272e 6a6f 696e 2866 756c 6c5f  = ')'.join(full_
+00009180: 6461 7461 2e73 706c 6974 2827 2927 295b  data.split(')')[
+00009190: 3a32 5d29 202b 2027 2927 0a20 2020 2020  :2]) + ')'.     
+000091a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000091b0: 6167 5f64 6174 6120 3d20 6675 6c6c 5f64  ag_data = full_d
+000091c0: 6174 612e 7370 6c69 7428 2729 2729 5b32  ata.split(')')[2
+000091d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000091e0: 2020 2020 2020 6375 725f 6964 203d 2074        cur_id = t
+000091f0: 6167 5f64 6174 612e 7370 6c69 7428 2754  ag_data.split('T
+00009200: 2729 5b31 5d2e 7374 7269 7028 2227 2022  ')[1].strip("' "
+00009210: 292e 7370 6c69 7428 2728 2729 5b30 5d0a  ).split('(')[0].
+00009220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009230: 2020 2020 7265 656c 5f69 6420 3d20 7461      reel_id = ta
+00009240: 675f 6461 7461 2e73 706c 6974 2827 5427  g_data.split('T'
+00009250: 295b 305d 2e73 7472 6970 2822 2720 2229  )[0].strip("' ")
+00009260: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009270: 2020 2020 2020 6966 2066 756c 6c5f 6461        if full_da
+00009280: 7461 2061 6e64 2063 7572 5f69 6420 616e  ta and cur_id an
+00009290: 6420 7265 656c 5f69 6420 616e 6420 6774  d reel_id and gt
+000092a0: 696e 3a0a 2020 2020 2020 2020 2020 2020  in:.            
+000092b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000092c0: 2e71 725f 6c6f 6767 6572 2e69 6e66 6f28  .qr_logger.info(
+000092d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000092e0: 2020 2020 2020 2020 2020 2020 2066 2757               f'W
+000092f0: 696c 696f 7420 5152 2064 6574 6563 7465  iliot QR detecte
+00009300: 6420 4754 696e 3a20 7b67 7469 6e7d 2c20  d GTin: {gtin}, 
+00009310: 5265 656c 3a20 7b72 6565 6c5f 6964 7d2c  Reel: {reel_id},
+00009320: 2049 443a 7b63 7572 5f69 647d 2729 0a20   ID:{cur_id}'). 
+00009330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009340: 2020 2020 2020 2072 6574 7572 6e20 6675         return fu
+00009350: 6c6c 5f64 6174 612c 2063 7572 5f69 642c  ll_data, cur_id,
+00009360: 2072 6565 6c5f 6964 2c20 6774 696e 0a20   reel_id, gtin. 
+00009370: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00009380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009390: 2066 756c 6c5f 6461 7461 203d 2063 7572   full_data = cur
+000093a0: 5f69 6420 3d20 7265 656c 5f69 6420 3d20  _id = reel_id = 
+000093b0: 6774 696e 203d 2062 6172 636f 6465 5f72  gtin = barcode_r
+000093c0: 6561 640a 2020 2020 2020 2020 2020 2020  ead.            
+000093d0: 2020 2020 6774 696e 5f76 616c 203d 2054      gtin_val = T
+000093e0: 7275 6520 6966 206c 656e 2866 756c 6c5f  rue if len(full_
+000093f0: 6461 7461 2920 3d3d 2073 656c 662e 7367  data) == self.sg
+00009400: 7469 6e5f 6c65 6e67 7468 2065 6c73 6520  tin_length else 
+00009410: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00009420: 2020 2020 2020 6966 2067 7469 6e5f 7661        if gtin_va
+00009430: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+00009440: 2020 2020 2020 2063 7572 5f69 6420 3d20         cur_id = 
+00009450: 6675 6c6c 5f64 6174 612e 7370 6c69 7428  full_data.split(
+00009460: 2754 2729 5b31 5d2e 7374 7269 7028 2227  'T')[1].strip("'
+00009470: 2022 292e 7370 6c69 7428 2728 2729 5b30   ").split('(')[0
+00009480: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00009490: 2020 2020 2020 7265 656c 5f69 6420 3d20        reel_id = 
+000094a0: 6675 6c6c 5f64 6174 612e 7370 6c69 7428  full_data.split(
+000094b0: 2754 2729 5b30 5d2e 7374 7269 7028 2227  'T')[0].strip("'
+000094c0: 2022 295b 2d34 3a5d 0a20 2020 2020 2020   ")[-4:].       
+000094d0: 2020 2020 2020 2020 2020 2020 2067 7469               gti
+000094e0: 6e20 3d20 6675 6c6c 5f64 6174 612e 7370  n = full_data.sp
+000094f0: 6c69 7428 2754 2729 5b30 5d2e 7374 7269  lit('T')[0].stri
+00009500: 7028 2227 2022 295b 3a2d 345d 0a20 2020  p("' ")[:-4].   
+00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009520: 2073 656c 662e 7172 5f6c 6f67 6765 722e   self.qr_logger.
+00009530: 696e 666f 2827 5769 6c69 6f74 2051 5220  info('Wiliot QR 
+00009540: 6465 7465 6374 6564 2047 5469 6e3a 207b  detected GTin: {
+00009550: 7d2c 2052 6565 6c3a 207b 7d2c 2049 443a  }, Reel: {}, ID:
+00009560: 7b7d 272e 666f 726d 6174 2867 7469 6e2c  {}'.format(gtin,
+00009570: 2063 7572 5f69 642c 2072 6565 6c5f 6964   cur_id, reel_id
+00009580: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00009590: 2020 2020 2020 2072 6574 7572 6e20 6675         return fu
+000095a0: 6c6c 5f64 6174 612c 2063 7572 5f69 642c  ll_data, cur_id,
+000095b0: 2072 6565 6c5f 6964 2c20 6774 696e 0a20   reel_id, gtin. 
+000095c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000095d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000095e0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009600: 2020 2020 2020 6966 2066 756c 6c5f 6461        if full_da
+00009610: 7461 203d 3d20 2746 273a 0a20 2020 2020  ta == 'F':.     
 00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009630: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
-00009640: 725f 6c6f 6767 6572 2e69 6e66 6f28 2757  r_logger.info('W
-00009650: 696c 696f 7420 5152 2064 6574 6563 7465  iliot QR detecte
-00009660: 6420 5265 656c 3a20 7b7d 2c20 4944 3a7b  d Reel: {}, ID:{
-00009670: 7d27 2e66 6f72 6d61 7428 6375 725f 6964  }'.format(cur_id
-00009680: 2c20 7265 656c 5f69 6429 290a 0a20 2020  , reel_id))..   
-00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096a0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-000096b0: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-000096c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000096d0: 7172 5f6c 6f67 6765 722e 696e 666f 2827  qr_logger.info('
-000096e0: 4e6f 7420 5769 6c69 6f74 2062 6172 636f  Not Wiliot barco
-000096f0: 6465 2729 0a0a 2020 2020 2020 2020 2020  de')..          
-00009700: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009710: 2066 756c 6c5f 6461 7461 2c20 6375 725f   full_data, cur_
-00009720: 6964 2c20 7265 656c 5f69 642c 2067 7469  id, reel_id, gti
-00009730: 6e0a 0a20 2020 2020 2020 2065 7863 6570  n..        excep
-00009740: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00009750: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00009760: 6c66 2e71 725f 6c6f 6767 6572 2e65 7272  lf.qr_logger.err
-00009770: 6f72 2866 2245 7272 6f72 2064 7572 696e  or(f"Error durin
-00009780: 6720 7265 6164 696e 6720 5769 6c69 6f74  g reading Wiliot
-00009790: 2062 6172 636f 6465 3a20 7b65 7d22 290a   barcode: {e}").
-000097a0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000097b0: 6520 4578 6365 7074 696f 6e0a 0a20 2020  e Exception..   
-000097c0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-000097d0: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  , None, None, No
-000097e0: 6e65 0a0a 2020 2020 6465 6620 6175 746f  ne..    def auto
-000097f0: 5f73 6361 6e28 7365 6c66 293a 0a20 2020  _scan(self):.   
-00009800: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00009810: 2041 7574 6f6d 6174 6963 616c 6c79 2073   Automatically s
-00009820: 6361 6e20 7468 6520 5152 2063 6f64 652e  can the QR code.
-00009830: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00009840: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
-00009850: 5f63 6f6e 6e65 6374 696f 6e2e 7772 6974  _connection.writ
-00009860: 6528 6222 5c78 3162 5c78 3332 2229 0a20  e(b"\x1b\x32"). 
-00009870: 2020 2020 2020 2074 203d 2073 656c 662e         t = self.
-00009880: 7365 7269 616c 5f63 6f6e 6e65 6374 696f  serial_connectio
-00009890: 6e2e 7265 6164 5f61 6c6c 2829 0a20 2020  n.read_all().   
-000098a0: 2020 2020 2073 656c 662e 7172 5f6c 6f67       self.qr_log
-000098b0: 6765 722e 696e 666f 2866 2761 7574 6f20  ger.info(f'auto 
-000098c0: 7363 616e 3a20 676f 7420 6d73 6720 7b74  scan: got msg {t
-000098d0: 7d27 290a 2020 2020 2020 2020 7265 7475  }').        retu
-000098e0: 726e 2074 0a0a 2020 2020 6465 6620 7472  rn t..    def tr
-000098f0: 6967 6765 725f 7374 6f70 5f73 6574 7469  igger_stop_setti
-00009900: 6e67 7328 7365 6c66 293a 0a20 2020 2020  ngs(self):.     
-00009910: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
-00009920: 7269 6767 6572 2073 746f 7020 7365 7474  rigger stop sett
-00009930: 696e 6773 2e0a 2020 2020 2020 2020 2222  ings..        ""
-00009940: 220a 2020 2020 2020 2020 736c 6565 7028  ".        sleep(
-00009950: 302e 3035 290a 2020 2020 2020 2020 7420  0.05).        t 
-00009960: 3d20 7365 6c66 2e73 6572 6961 6c5f 636f  = self.serial_co
-00009970: 6e6e 6563 7469 6f6e 2e72 6561 645f 616c  nnection.read_al
-00009980: 6c28 290a 2020 2020 2020 2020 736c 6565  l().        slee
-00009990: 7028 302e 3035 290a 2020 2020 2020 2020  p(0.05).        
-000099a0: 6163 6b73 203d 2073 7472 2874 292e 7370  acks = str(t).sp
-000099b0: 6c69 7428 273b 2729 5b3a 2d31 5d0a 2020  lit(';')[:-1].  
-000099c0: 2020 2020 2020 6973 5375 6363 6573 7320        isSuccess 
-000099d0: 3d20 616c 6c28 5b54 7275 6520 6966 2061  = all([True if a
-000099e0: 636b 2e65 6e64 7377 6974 6828 275c 5c78  ck.endswith('\\x
-000099f0: 3036 2729 2065 6c73 6520 4661 6c73 6520  06') else False 
-00009a00: 666f 7220 6163 6b20 696e 2061 636b 735d  for ack in acks]
-00009a10: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00009a20: 2074 2c20 6973 5375 6363 6573 730a 0a20   t, isSuccess.. 
-00009a30: 2020 2064 6566 2074 7269 6767 6572 5f6f     def trigger_o
-00009a40: 6666 2873 656c 6629 3a0a 2020 2020 2020  ff(self):.      
-00009a50: 2020 2222 220a 2020 2020 2020 2020 746f    """.        to
-00009a60: 206b 6565 7020 7361 6d65 2062 6568 6176   keep same behav
-00009a70: 696f 7220 6173 2074 6865 2043 6f67 6e65  ior as the Cogne
-00009a80: 780a 2020 2020 2020 2020 4072 6574 7572  x.        @retur
-00009a90: 6e3a 0a20 2020 2020 2020 2040 7274 7970  n:.        @rtyp
-00009aa0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00009ab0: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
-00009ac0: 6173 7320 436f 676e 6578 4e65 7477 6f72  ass CognexNetwor
-00009ad0: 6b3a 0a20 2020 2042 4152 434f 4445 5f4c  k:.    BARCODE_L
-00009ae0: 454e 203d 2031 380a 2020 2020 4445 5649  EN = 18.    DEVI
-00009af0: 4345 5f4e 414d 4520 3d20 2742 6172 436f  CE_NAME = 'BarCo
-00009b00: 6465 5265 6164 6572 270a 0a20 2020 2064  deReader'..    d
-00009b10: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00009b20: 2c20 6970 5f61 6464 7265 7373 2c20 706f  , ip_address, po
-00009b30: 7274 3d32 3329 3a0a 0a20 2020 2020 2020  rt=23):..       
-00009b40: 2073 656c 662e 636f 6e6e 6563 7465 6420   self.connected 
-00009b50: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00009b60: 7365 6c66 2e74 6e20 3d20 4e6f 6e65 0a20  self.tn = None. 
-00009b70: 2020 2020 2020 2073 656c 662e 686f 7374         self.host
-00009b80: 203d 2073 7472 2869 705f 6164 6472 6573   = str(ip_addres
-00009b90: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-00009ba0: 706f 7274 203d 2070 6f72 740a 2020 2020  port = port.    
-00009bb0: 2020 2020 7365 6c66 2e64 6576 6963 655f      self.device_
-00009bc0: 6e61 6d65 203d 2027 270a 0a20 2020 2020  name = ''..     
-00009bd0: 2020 2073 656c 662e 6f70 656e 5f70 6f72     self.open_por
-00009be0: 7428 290a 0a20 2020 2064 6566 206f 7065  t()..    def ope
-00009bf0: 6e5f 706f 7274 2873 656c 662c 2063 6f6d  n_port(self, com
-00009c00: 5f70 6f72 743d 4e6f 6e65 2c20 6261 7564  _port=None, baud
-00009c10: 5f72 6174 653d 3131 3532 3030 2c20 7469  _rate=115200, ti
-00009c20: 6d65 6f75 743d 3530 302c 2063 6f6e 6669  meout=500, confi
-00009c30: 673d 4661 6c73 6529 3a0a 2020 2020 2020  g=False):.      
-00009c40: 2020 7365 6c66 2e63 6f6e 6e65 6374 6564    self.connected
-00009c50: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00009c60: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00009c70: 2020 7365 6c66 2e74 6e20 3d20 7465 6c6e    self.tn = teln
-00009c80: 6574 6c69 622e 5465 6c6e 6574 2868 6f73  etlib.Telnet(hos
-00009c90: 743d 7365 6c66 2e68 6f73 742c 2070 6f72  t=self.host, por
-00009ca0: 743d 7365 6c66 2e70 6f72 742c 2074 696d  t=self.port, tim
-00009cb0: 656f 7574 3d31 290a 2020 2020 2020 2020  eout=1).        
-00009cc0: 2020 2020 736c 6565 7028 3129 0a20 2020      sleep(1).   
-00009cd0: 2020 2020 2020 2020 2073 656c 662e 746e           self.tn
-00009ce0: 2e77 7269 7465 2862 277c 7c30 3a31 3233  .write(b'||0:123
-00009cf0: 3e47 4554 2044 4556 4943 452e 4e41 4d45  >GET DEVICE.NAME
-00009d00: 5c72 5c6e 2729 0a20 2020 2020 2020 2020  \r\n').         
-00009d10: 2020 2072 7370 203d 2073 656c 662e 7265     rsp = self.re
-00009d20: 6164 5f72 6573 706f 6e73 6528 290a 2020  ad_response().  
-00009d30: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00009d40: 662e 4445 5649 4345 5f4e 414d 4520 696e  f.DEVICE_NAME in
-00009d50: 2072 7370 3a0a 2020 2020 2020 2020 2020   rsp:.          
-00009d60: 2020 2020 2020 7365 6c66 2e64 6576 6963        self.devic
-00009d70: 655f 6e61 6d65 203d 2072 7370 0a20 2020  e_name = rsp.   
-00009d80: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00009d90: 6e6e 6563 7465 6420 3d20 5472 7565 0a20  nnected = True. 
-00009da0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00009db0: 2866 2743 6f6e 6e65 6374 6564 2074 6f20  (f'Connected to 
-00009dc0: 7b73 656c 662e 6465 7669 6365 5f6e 616d  {self.device_nam
-00009dd0: 657d 2729 0a20 2020 2020 2020 2065 7863  e}').        exc
-00009de0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00009df0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-00009e00: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
-00009e10: 6622 4661 696c 6564 2074 6f20 636f 6e6e  f"Failed to conn
-00009e20: 6563 7420 746f 2054 656e 6574 2073 6f63  ect to Tenet soc
-00009e30: 6b65 743a 207b 657d 2229 0a0a 2020 2020  ket: {e}")..    
-00009e40: 6465 6620 7265 6164 5f72 6573 706f 6e73  def read_respons
-00009e50: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00009e60: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00009e70: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00009e80: 662e 746e 2e72 6561 645f 756e 7469 6c28  f.tn.read_until(
-00009e90: 6227 5c6e 272c 2074 696d 656f 7574 3d31  b'\n', timeout=1
-00009ea0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00009eb0: 2072 6573 706f 6e73 653a 0a20 2020 2020   response:.     
-00009ec0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-00009ed0: 6e73 6520 3d20 7265 7370 6f6e 7365 2e64  nse = response.d
-00009ee0: 6563 6f64 6528 290a 2020 2020 2020 2020  ecode().        
-00009ef0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00009f00: 203d 2072 6573 706f 6e73 652e 7374 7269   = response.stri
-00009f10: 7028 275c 725c 6e27 290a 2020 2020 2020  p('\r\n').      
-00009f20: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009f30: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
-00009f40: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00009f50: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-00009f60: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00009f70: 7469 6f6e 2866 2246 6169 6c65 6420 746f  tion(f"Failed to
-00009f80: 2072 6561 6420 7265 7370 6f6e 7365 3a20   read response: 
-00009f90: 7b65 7d22 290a 2020 2020 2020 2020 7265  {e}").        re
-00009fa0: 7475 726e 2027 270a 0a20 2020 2064 6566  turn ''..    def
-00009fb0: 2072 6561 645f 6261 7463 6828 7365 6c66   read_batch(self
-00009fc0: 2c20 6e5f 6d73 673d 3130 3030 293a 0a20  , n_msg=1000):. 
-00009fd0: 2020 2020 2020 2072 7370 5f6f 7574 203d         rsp_out =
-00009fe0: 205b 5d0a 2020 2020 2020 2020 7273 7020   [].        rsp 
-00009ff0: 3d20 7365 6c66 2e72 6561 645f 7265 7370  = self.read_resp
-0000a000: 6f6e 7365 2829 0a20 2020 2020 2020 206d  onse().        m
-0000a010: 7367 5f63 6f75 6e74 6572 203d 2030 0a20  sg_counter = 0. 
-0000a020: 2020 2020 2020 2077 6869 6c65 206c 656e         while len
-0000a030: 2872 7370 5f6f 7574 2920 3c20 6e5f 6d73  (rsp_out) < n_ms
-0000a040: 6720 616e 6420 7273 7020 213d 2027 2720  g and rsp != '' 
-0000a050: 616e 6420 6d73 675f 636f 756e 7465 7220  and msg_counter 
-0000a060: 3c20 6e5f 6d73 673a 0a20 2020 2020 2020  < n_msg:.       
-0000a070: 2020 2020 2077 6869 6c65 206c 656e 2872       while len(r
-0000a080: 7370 2920 3e3d 2073 656c 662e 4241 5243  sp) >= self.BARC
-0000a090: 4f44 455f 4c45 4e3a 0a20 2020 2020 2020  ODE_LEN:.       
-0000a0a0: 2020 2020 2020 2020 2072 7370 5f6f 7574           rsp_out
-0000a0b0: 2e61 7070 656e 6428 7273 705b 3a73 656c  .append(rsp[:sel
-0000a0c0: 662e 4241 5243 4f44 455f 4c45 4e5d 290a  f.BARCODE_LEN]).
-0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0e0: 7273 7020 3d20 7273 705b 7365 6c66 2e42  rsp = rsp[self.B
-0000a0f0: 4152 434f 4445 5f4c 454e 3a5d 0a20 2020  ARCODE_LEN:].   
-0000a100: 2020 2020 2020 2020 2072 7370 203d 2073           rsp = s
-0000a110: 656c 662e 7265 6164 5f72 6573 706f 6e73  elf.read_respons
-0000a120: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000a130: 6d73 675f 636f 756e 7465 7220 2b3d 2031  msg_counter += 1
-0000a140: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000a150: 206c 6973 7428 7365 7428 7273 705f 6f75   list(set(rsp_ou
-0000a160: 7429 290a 0a20 2020 2064 6566 2074 7269  t))..    def tri
-0000a170: 6767 6572 5f6f 6e28 7365 6c66 2c20 636f  gger_on(self, co
-0000a180: 6e74 696e 756f 7573 6c79 3d54 7275 652c  ntinuously=True,
-0000a190: 2074 7269 6767 6572 5f74 7970 653d 3429   trigger_type=4)
-0000a1a0: 3a0a 2020 2020 2020 2020 2222 220a 0a20  :.        """.. 
-0000a1b0: 2020 2020 2020 2040 7061 7261 6d20 7472         @param tr
-0000a1c0: 6967 6765 725f 7479 7065 3a20 303a 2053  igger_type: 0: S
-0000a1d0: 696e 676c 6520 2865 7874 6572 6e61 6c29  ingle (external)
-0000a1e0: 2c20 313a 2050 7265 7365 6e74 6174 696f  , 1: Presentatio
-0000a1f0: 6e20 2869 6e74 6572 6e61 6c29 2c20 323a  n (internal), 2:
-0000a200: 204d 616e 7561 6c20 2862 7574 746f 6e29   Manual (button)
-0000a210: 2c20 333a 2042 7572 7374 2028 6578 7465  , 3: Burst (exte
-0000a220: 726e 616c 292c 0a20 2020 2020 2020 2020  rnal),.         
-0000a230: 2020 2020 2020 2020 2020 2020 343a 2053              4: S
-0000a240: 656c 6620 2869 6e74 6572 6e61 6c29 2c20  elf (internal), 
-0000a250: 353a 2043 6f6e 7469 6e75 6f75 7320 2865  5: Continuous (e
-0000a260: 7874 6572 6e61 6c29 0a20 2020 2020 2020  xternal).       
-0000a270: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
-0000a280: 5369 6e67 6c65 3a20 4163 7175 6972 6573  Single: Acquires
-0000a290: 2061 2073 696e 676c 6520 696d 6167 6520   a single image 
-0000a2a0: 616e 6420 6174 7465 6d70 7473 2074 6f20  and attempts to 
-0000a2b0: 6465 636f 6465 2061 6e79 2073 796d 626f  decode any symbo
-0000a2c0: 6c20 6974 2063 6f6e 7461 696e 7320 6f72  l it contains or
-0000a2d0: 206d 6f72 6520 7468 616e 206f 6e65 0a20   more than one. 
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2f0: 2020 2020 7379 6d62 6f6c 2069 6e20 6361      symbol in ca
-0000a300: 7365 7320 7768 6572 6520 6d75 6c74 6963  ses where multic
-0000a310: 6f64 6520 6973 2065 6e61 626c 6564 2e20  ode is enabled. 
-0000a320: 5468 6520 7265 6164 6572 2072 656c 6965  The reader relie
-0000a330: 7320 6f6e 2061 6e20 6578 7465 726e 616c  s on an external
-0000a340: 2074 7269 6767 6572 2073 6f75 7263 652e   trigger source.
-0000a350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a360: 2020 2020 2020 2a20 5072 6573 656e 7461        * Presenta
-0000a370: 7469 6f6e 3a20 5265 7065 6174 6564 6c79  tion: Repeatedly
-0000a380: 2073 6361 6e73 2066 6f72 2061 2073 796d   scans for a sym
-0000a390: 626f 6c20 616e 6420 6465 636f 6465 7320  bol and decodes 
-0000a3a0: 6974 2077 6865 6e65 7665 7220 6f6e 6520  it whenever one 
-0000a3b0: 6973 2064 6574 6563 7465 642e 0a20 2020  is detected..   
-0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3d0: 2020 5468 6520 7265 6164 6572 2072 656c    The reader rel
-0000a3e0: 6965 7320 6f6e 2061 6e20 696e 7465 726e  ies on an intern
-0000a3f0: 616c 2074 696d 696e 6720 6d65 6368 616e  al timing mechan
-0000a400: 6973 6d20 746f 2061 6371 7569 7265 2069  ism to acquire i
-0000a410: 6d61 6765 732e 0a20 2020 2020 2020 2020  mages..         
-0000a420: 2020 2020 2020 2020 2020 2020 2a20 4275              * Bu
-0000a430: 7273 743a 2050 6572 666f 726d 7320 6d75  rst: Performs mu
-0000a440: 6c74 6970 6c65 2069 6d61 6765 2061 6371  ltiple image acq
-0000a450: 7569 7369 7469 6f6e 7320 6261 7365 6420  uisitions based 
-0000a460: 6f6e 2061 6e20 6578 7465 726e 616c 2074  on an external t
-0000a470: 7269 6767 6572 2061 6e64 2064 6563 6f64  rigger and decod
-0000a480: 6573 206f 6e65 206f 720a 2020 2020 2020  es one or.      
-0000a490: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000a4a0: 756c 7469 706c 6520 7379 6d62 6f6c 7320  ultiple symbols 
-0000a4b0: 6170 7065 6172 696e 6720 696e 2074 6865  appearing in the
-0000a4c0: 2073 6571 7565 6e63 6520 6f66 2069 6d61   sequence of ima
-0000a4d0: 6765 732e 0a20 2020 2020 2020 2020 2020  ges..           
-0000a4e0: 2020 2020 2020 2020 2020 2a20 5365 6c66            * Self
-0000a4f0: 3a20 5369 6d69 6c61 7220 746f 2050 7265  : Similar to Pre
-0000a500: 7365 6e74 6174 696f 6e20 6d6f 6465 2069  sentation mode i
-0000a510: 6e20 7468 6174 2074 6865 2072 6561 6465  n that the reade
-0000a520: 7220 7065 7270 6574 7561 6c6c 7920 7363  r perpetually sc
-0000a530: 616e 7320 666f 7220 7379 6d62 6f6c 7320  ans for symbols 
-0000a540: 616e 6420 6465 636f 6465 730a 2020 2020  and decodes.    
-0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2074 6865 6d20 6561 6368 2074 696d 6520   them each time 
-0000a570: 6f6e 6520 6973 2064 6574 6563 7465 642e  one is detected.
-0000a580: 2055 6e6c 696b 6520 5072 6573 656e 7461   Unlike Presenta
-0000a590: 7469 6f6e 206d 6f64 652c 2068 6f77 6576  tion mode, howev
-0000a5a0: 6572 2c20 5365 6c66 206d 6f64 6520 7375  er, Self mode su
-0000a5b0: 7070 6f72 7473 206d 756c 7469 636f 6465  pports multicode
-0000a5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a5d0: 2020 2020 2020 7265 7375 6c74 7320 616e        results an
-0000a5e0: 6420 6120 6465 636f 6465 2061 7474 656d  d a decode attem
-0000a5f0: 7074 206f 6363 7572 7320 7769 7468 2065  pt occurs with e
-0000a600: 7665 7279 2069 6d61 6765 2e20 5468 6520  very image. The 
-0000a610: 6d61 696e 2064 6966 6665 7265 6e63 6520  main difference 
-0000a620: 6265 7477 6565 6e20 5365 6c66 2061 6e64  between Self and
-0000a630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a640: 2020 2020 2020 5072 6573 656e 7461 7469        Presentati
-0000a650: 6f6e 2069 7320 7468 6520 6669 7865 6420  on is the fixed 
-0000a660: 616e 6420 6578 6163 7420 696e 7465 7276  and exact interv
-0000a670: 616c 2066 6f72 2069 6d61 6765 2061 6371  al for image acq
-0000a680: 7569 7369 7469 6f6e 7320 696e 2053 656c  uisitions in Sel
-0000a690: 662e 0a20 2020 2020 2020 2020 2020 2020  f..             
-0000a6a0: 2020 2020 2020 2020 2a20 436f 6e74 696e          * Contin
-0000a6b0: 756f 7573 3a20 4265 6769 6e73 2061 6371  uous: Begins acq
-0000a6c0: 7569 7269 6e67 2069 6d61 6765 7320 6261  uiring images ba
-0000a6d0: 7365 6420 6f6e 2061 2073 696e 676c 6520  sed on a single 
-0000a6e0: 6578 7465 726e 616c 2074 7269 6767 6572  external trigger
-0000a6f0: 2061 6e64 2063 6f6e 7469 6e75 6573 2074   and continues t
-0000a700: 6f20 6163 7175 6972 650a 2020 2020 2020  o acquire.      
-0000a710: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000a720: 6d61 6765 7320 756e 7469 6c20 6120 7379  mages until a sy
-0000a730: 6d62 6f6c 2069 7320 666f 756e 6420 616e  mbol is found an
-0000a740: 6420 6465 636f 6465 642c 206f 7220 756e  d decoded, or un
-0000a750: 7469 6c20 6d75 6c74 6970 6c65 2069 6d61  til multiple ima
-0000a760: 6765 7320 636f 6e74 6169 6e69 6e67 2061  ges containing a
-0000a770: 7320 6d61 6e79 2063 6f64 6573 2061 730a  s many codes as.
-0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a790: 2020 2020 2073 7065 6369 6669 6564 2069       specified i
-0000a7a0: 6e20 6d75 6c74 6963 6f64 6520 6d6f 6465  n multicode mode
-0000a7b0: 2061 7265 206c 6f63 6174 6564 2c20 6f72   are located, or
-0000a7c0: 2075 6e74 696c 2074 6865 2074 7269 6767   until the trigg
-0000a7d0: 6572 2069 7320 7265 6c65 6173 6564 2e0a  er is released..
-0000a7e0: 2020 2020 2020 2020 4074 7970 6520 7472          @type tr
-0000a7f0: 6967 6765 725f 7479 7065 3a20 696e 740a  igger_type: int.
-0000a800: 2020 2020 2020 2020 4072 6574 7572 6e3a          @return:
-0000a810: 0a20 2020 2020 2020 2040 7274 7970 653a  .        @rtype:
-0000a820: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000a830: 2020 2020 2069 6620 636f 6e74 696e 756f       if continuo
-0000a840: 7573 6c79 3a0a 2020 2020 2020 2020 2020  usly:.          
-0000a850: 2020 636f 6d6d 616e 6420 3d20 6627 7c7c    command = f'||
-0000a860: 303a 3132 333e 5345 5420 5452 4947 4745  0:123>SET TRIGGE
-0000a870: 522e 5459 5045 207b 7472 6967 6765 725f  R.TYPE {trigger_
-0000a880: 7479 7065 7d5c 725c 6e27 0a20 2020 2020  type}\r\n'.     
-0000a890: 2020 2020 2020 2073 656c 662e 746e 2e77         self.tn.w
-0000a8a0: 7269 7465 2863 6f6d 6d61 6e64 2e65 6e63  rite(command.enc
-0000a8b0: 6f64 6528 2929 0a0a 2020 2020 6465 6620  ode())..    def 
-0000a8c0: 7472 6967 6765 725f 6f66 6628 7365 6c66  trigger_off(self
-0000a8d0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0000a8e0: 746e 2e77 7269 7465 2862 277c 7c30 3a31  tn.write(b'||0:1
-0000a8f0: 3233 3e53 4554 2054 5249 4747 4552 2e54  23>SET TRIGGER.T
-0000a900: 5950 4520 305c 725c 6e27 290a 2020 2020  YPE 0\r\n').    
-0000a910: 2020 2020 736c 6565 7028 3129 0a20 2020      sleep(1).   
-0000a920: 2020 2020 2023 2054 4f44 4f20 6d61 7962       # TODO mayb
-0000a930: 6520 636c 6561 6e20 616c 6c20 6d73 6773  e clean all msgs
-0000a940: 0a0a 2020 2020 6465 6620 636c 6f73 655f  ..    def close_
-0000a950: 706f 7274 2873 656c 6629 3a0a 2020 2020  port(self):.    
-0000a960: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000a970: 2020 2020 2073 656c 662e 746e 2e63 6c6f       self.tn.clo
-0000a980: 7365 2829 0a20 2020 2020 2020 2065 7863  se().        exc
-0000a990: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-0000a9a0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-0000a9b0: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
-0000a9c0: 6622 4661 696c 6564 2074 6f20 636c 6f73  f"Failed to clos
-0000a9d0: 6520 5465 6e65 7420 636f 6d6d 756e 6963  e Tenet communic
-0000a9e0: 6174 696f 6e3a 207b 657d 2229 0a0a 0a63  ation: {e}")...c
-0000a9f0: 6c61 7373 2043 6f67 6e65 7844 6174 614d  lass CognexDataM
-0000aa00: 616e 3a0a 2020 2020 434f 4e54 494e 554f  an:.    CONTINUO
-0000aa10: 5553 5f54 5249 4747 4552 5f54 5950 4520  US_TRIGGER_TYPE 
-0000aa20: 3d20 340a 2020 2020 5347 5449 4e5f 5354  = 4.    SGTIN_ST
-0000aa30: 5249 505f 4c45 4e20 3d20 3237 0a20 2020  RIP_LEN = 27.   
-0000aa40: 2053 4754 494e 5f4c 454e 203d 2033 310a   SGTIN_LEN = 31.
-0000aa50: 2020 2020 5245 454c 5f49 445f 4c45 4e20      REEL_ID_LEN 
-0000aa60: 3d20 340a 2020 2020 4d49 4e5f 5449 4d45  = 4.    MIN_TIME
-0000aa70: 5f54 4f5f 5245 4144 203d 2030 2e32 3030  _TO_READ = 0.200
-0000aa80: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0000aa90: 5f5f 2873 656c 662c 2070 6f72 743d 4e6f  __(self, port=No
-0000aaa0: 6e65 2c20 6261 7564 5f72 6174 653d 3131  ne, baud_rate=11
-0000aab0: 3532 3030 2c20 7469 6d65 6f75 743d 3530  5200, timeout=50
-0000aac0: 302c 206c 6f67 5f6e 616d 653d 4e6f 6e65  0, log_name=None
-0000aad0: 2c20 7472 6967 6765 725f 7479 7065 3d30  , trigger_type=0
-0000aae0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000aaf0: 2020 2020 2020 2068 7474 7073 3a2f 2f73         https://s
-0000ab00: 7570 706f 7274 2e63 6f67 6e65 782e 636f  upport.cognex.co
-0000ab10: 6d2f 646f 6373 2f64 6d73 745f 3233 3232  m/docs/dmst_2322
-0000ab20: 2f77 6562 2f45 4e2f 444d 4343 2f43 6f6e  /web/EN/DMCC/Con
-0000ab30: 7465 6e74 2f54 6f70 6963 732f 646d 6363  tent/Topics/dmcc
-0000ab40: 2d6d 6169 6e2e 6874 6d6c 0a20 2020 2020  -main.html.     
-0000ab50: 2020 2074 6f20 646f 776e 6c6f 6164 2043     to download C
-0000ab60: 4f47 4e45 5820 4755 493a 2068 7474 7073  OGNEX GUI: https
-0000ab70: 3a2f 2f73 7570 706f 7274 2e63 6f67 6e65  ://support.cogne
-0000ab80: 782e 636f 6d2f 656e 2f64 6f77 6e6c 6f61  x.com/en/downloa
-0000ab90: 6473 2f64 6574 6169 6c2f 6461 7461 6d61  ds/detail/datama
-0000aba0: 6e2f 3435 3132 2f31 3033 330a 2020 2020  n/4512/1033.    
-0000abb0: 2020 2020 4070 6172 616d 2070 6f72 743a      @param port:
-0000abc0: 0a20 2020 2020 2020 2040 7479 7065 2070  .        @type p
-0000abd0: 6f72 743a 0a20 2020 2020 2020 2040 7061  ort:.        @pa
-0000abe0: 7261 6d20 6261 7564 5f72 6174 653a 0a20  ram baud_rate:. 
-0000abf0: 2020 2020 2020 2040 7479 7065 2062 6175         @type bau
-0000ac00: 645f 7261 7465 3a0a 2020 2020 2020 2020  d_rate:.        
-0000ac10: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-0000ac20: 2e64 6576 6963 655f 6e61 6d65 203d 2027  .device_name = '
-0000ac30: 270a 2020 2020 2020 2020 7365 6c66 2e63  '.        self.c
-0000ac40: 6f6d 5f70 6f72 7420 3d20 2727 0a20 2020  om_port = ''.   
-0000ac50: 2020 2020 2073 656c 662e 6261 7564 5f72       self.baud_r
-0000ac60: 6174 6520 3d20 300a 2020 2020 2020 2020  ate = 0.        
-0000ac70: 7365 6c66 2e74 7269 6767 6572 5f74 7970  self.trigger_typ
-0000ac80: 6520 3d20 7472 6967 6765 725f 7479 7065  e = trigger_type
-0000ac90: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000aca0: 7220 3d20 4e6f 6e65 0a20 2020 2020 2020  r = None.       
-0000acb0: 2073 656c 662e 636f 6e6e 6563 7465 6420   self.connected 
-0000acc0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-0000acd0: 6966 206c 6f67 5f6e 616d 6520 6973 204e  if log_name is N
-0000ace0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000acf0: 2073 656c 662e 6c6f 6767 6572 203d 206c   self.logger = l
-0000ad00: 6f67 6769 6e67 2e67 6574 4c6f 6767 6572  ogging.getLogger
-0000ad10: 2827 436f 676e 6578 5363 616e 6e65 724c  ('CognexScannerL
-0000ad20: 6f67 6765 7227 290a 2020 2020 2020 2020  ogger').        
-0000ad30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000ad40: 2020 7365 6c66 2e6c 6f67 6765 7220 3d20    self.logger = 
-0000ad50: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
-0000ad60: 7228 6c6f 675f 6e61 6d65 290a 0a20 2020  r(log_name)..   
-0000ad70: 2020 2020 2069 6620 706f 7274 2069 7320       if port is 
-0000ad80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000ad90: 2020 2020 2020 7365 6c66 2e63 6f6e 6e65        self.conne
-0000ada0: 6374 6564 203d 2073 656c 662e 6f70 656e  cted = self.open
-0000adb0: 5f70 6f72 7428 636f 6d5f 706f 7274 3d70  _port(com_port=p
-0000adc0: 6f72 742c 2062 6175 645f 7261 7465 3d62  ort, baud_rate=b
-0000add0: 6175 645f 7261 7465 2c20 7469 6d65 6f75  aud_rate, timeou
-0000ade0: 743d 7469 6d65 6f75 7429 0a20 2020 2020  t=timeout).     
-0000adf0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000ae00: 2020 2020 2061 6c6c 5f70 6f72 7473 203d       all_ports =
-0000ae10: 2073 6572 6961 6c5f 706f 7274 7328 290a   serial_ports().
-0000ae20: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000ae30: 706f 7274 2069 6e20 616c 6c5f 706f 7274  port in all_port
-0000ae40: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000ae50: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000ae60: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-0000ae70: 6563 7465 6420 3d20 7365 6c66 2e6f 7065  ected = self.ope
-0000ae80: 6e5f 706f 7274 2863 6f6d 5f70 6f72 743d  n_port(com_port=
-0000ae90: 706f 7274 2c20 6261 7564 5f72 6174 653d  port, baud_rate=
-0000aea0: 6261 7564 5f72 6174 652c 2074 696d 656f  baud_rate, timeo
-0000aeb0: 7574 3d74 696d 656f 7574 290a 2020 2020  ut=timeout).    
-0000aec0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0000aed0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000aee0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000aef0: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
-0000af00: 6572 2e77 6172 6e69 6e67 2866 2743 6f75  er.warning(f'Cou
-0000af10: 6c64 206e 6f74 2063 6f6e 6e65 6374 2074  ld not connect t
-0000af20: 6f20 706f 7274 207b 706f 7274 7d20 6475  o port {port} du
-0000af30: 6520 746f 207b 657d 2729 0a20 2020 2020  e to {e}').     
-0000af40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000af50: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-0000af60: 2020 2020 2020 2020 6966 2063 6f6e 6e65          if conne
-0000af70: 6374 6564 3a0a 2020 2020 2020 2020 2020  cted:.          
-0000af80: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000af90: 6f6e 6e65 6374 6564 203d 2054 7275 650a  onnected = True.
-0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afb0: 2020 2020 6272 6561 6b0a 0a20 2020 2020      break..     
-0000afc0: 2020 2069 6620 7365 6c66 2e63 6f6e 6e65     if self.conne
-0000afd0: 6374 6564 3a0a 2020 2020 2020 2020 2020  cted:.          
-0000afe0: 2020 7365 6c66 2e69 6e69 745f 636f 6e66    self.init_conf
-0000aff0: 6967 7572 6174 696f 6e73 2829 0a20 2020  igurations().   
-0000b000: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000b010: 6d5f 706f 7274 203d 2070 6f72 740a 2020  m_port = port.  
-0000b020: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0000b030: 6175 645f 7261 7465 203d 2062 6175 645f  aud_rate = baud_
-0000b040: 7261 7465 0a0a 2020 2020 6465 6620 6f70  rate..    def op
-0000b050: 656e 5f70 6f72 7428 7365 6c66 2c20 636f  en_port(self, co
-0000b060: 6d5f 706f 7274 2c20 6261 7564 5f72 6174  m_port, baud_rat
-0000b070: 653d 3131 3532 3030 2c20 7469 6d65 6f75  e=115200, timeou
-0000b080: 743d 3530 302c 2063 6f6e 6669 673d 4661  t=500, config=Fa
-0000b090: 6c73 6529 3a0a 2020 2020 2020 2020 2222  lse):.        ""
-0000b0a0: 220a 0a20 2020 2020 2020 2040 7061 7261  "..        @para
-0000b0b0: 6d20 636f 6d5f 706f 7274 3a0a 2020 2020  m com_port:.    
-0000b0c0: 2020 2020 4074 7970 6520 636f 6d5f 706f      @type com_po
-0000b0d0: 7274 3a0a 2020 2020 2020 2020 4070 6172  rt:.        @par
-0000b0e0: 616d 2062 6175 645f 7261 7465 3a0a 2020  am baud_rate:.  
-0000b0f0: 2020 2020 2020 4074 7970 6520 6261 7564        @type baud
-0000b100: 5f72 6174 653a 0a20 2020 2020 2020 2040  _rate:.        @
-0000b110: 7061 7261 6d20 7469 6d65 6f75 743a 2074  param timeout: t
-0000b120: 696d 656f 7574 2069 6e20 6d73 6563 0a20  imeout in msec. 
-0000b130: 2020 2020 2020 2040 7479 7065 2074 696d         @type tim
-0000b140: 656f 7574 3a20 696e 7420 6f72 2073 7472  eout: int or str
-0000b150: 0a20 2020 2020 2020 2040 7061 7261 6d20  .        @param 
-0000b160: 636f 6e66 6967 3a20 7469 6d65 6f75 7420  config: timeout 
-0000b170: 696e 206d 7365 630a 2020 2020 2020 2020  in msec.        
-0000b180: 4074 7970 6520 636f 6e66 6967 3a20 696e  @type config: in
-0000b190: 7420 6f72 2073 7472 0a20 2020 2020 2020  t or str.       
-0000b1a0: 2040 7265 7475 726e 3a0a 2020 2020 2020   @return:.      
-0000b1b0: 2020 4072 7479 7065 3a0a 2020 2020 2020    @rtype:.      
-0000b1c0: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-0000b1d0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0000b1e0: 656c 662e 7365 7220 3d20 7365 7269 616c  elf.ser = serial
-0000b1f0: 2e53 6572 6961 6c28 636f 6d5f 706f 7274  .Serial(com_port
-0000b200: 2c20 6261 7564 5f72 6174 652c 2074 696d  , baud_rate, tim
-0000b210: 656f 7574 3d69 6e74 2874 696d 656f 7574  eout=int(timeout
-0000b220: 292f 3130 3030 290a 2020 2020 2020 2020  )/1000).        
-0000b230: 2020 2020 736c 6565 7028 3129 0a20 2020      sleep(1).   
-0000b240: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
-0000b250: 6564 203d 2073 656c 662e 6973 5f6f 7065  ed = self.is_ope
-0000b260: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-0000b270: 6966 2063 6f6e 6e65 6374 6564 2061 6e64  if connected and
-0000b280: 2063 6f6e 6669 673a 0a20 2020 2020 2020   config:.       
-0000b290: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
-0000b2a0: 6974 5f63 6f6e 6669 6775 7261 7469 6f6e  it_configuration
-0000b2b0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000b2c0: 7265 7475 726e 2063 6f6e 6e65 6374 6564  return connected
-0000b2d0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-0000b2e0: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
-0000b2f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000b300: 6520 4578 6365 7074 696f 6e28 6622 4661  e Exception(f"Fa
-0000b310: 696c 6564 2074 6f20 6f70 656e 2073 6572  iled to open ser
-0000b320: 6961 6c20 706f 7274 3a20 7b65 7d22 290a  ial port: {e}").
-0000b330: 0a20 2020 2064 6566 2069 735f 6f70 656e  .    def is_open
-0000b340: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000b350: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000b360: 2064 6576 5f6e 616d 6520 3d20 7365 6c66   dev_name = self
-0000b370: 2e67 6574 5f64 6576 6963 655f 7072 6f70  .get_device_prop
-0000b380: 6572 7479 2827 4445 5649 4345 2e4e 414d  erty('DEVICE.NAM
-0000b390: 4527 290a 2020 2020 2020 2020 2020 2020  E').            
-0000b3a0: 6966 2064 6576 5f6e 616d 652e 7374 6172  if dev_name.star
-0000b3b0: 7473 7769 7468 2827 444d 3727 293a 0a20  tswith('DM7'):. 
-0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b3d0: 656c 662e 6465 7669 6365 5f6e 616d 6520  elf.device_name 
-0000b3e0: 3d20 6465 765f 6e61 6d65 0a20 2020 2020  = dev_name.     
-0000b3f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b400: 6c6f 6767 6572 2e69 6e66 6f28 6627 636f  logger.info(f'co
-0000b410: 6e6e 6563 7465 6420 746f 207b 6465 765f  nnected to {dev_
-0000b420: 6e61 6d65 7d27 290a 2020 2020 2020 2020  name}').        
-0000b430: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000b440: 7275 650a 2020 2020 2020 2020 6578 6365  rue.        exce
-0000b450: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000b460: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000b470: 656c 662e 6c6f 6767 6572 2e69 6e66 6f28  elf.logger.info(
-0000b480: 6627 6465 7669 6365 2069 7320 6e6f 7420  f'device is not 
-0000b490: 636f 6d6d 756e 6963 6174 6520 6475 6520  communicate due 
-0000b4a0: 746f 207b 657d 2729 0a20 2020 2020 2020  to {e}').       
-0000b4b0: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-0000b4c0: 2020 2064 6566 2072 6563 6f6e 6e65 6374     def reconnect
-0000b4d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000b4e0: 7365 6c66 2e6c 6f67 6765 722e 696e 666f  self.logger.info
-0000b4f0: 2866 2754 7279 2020 746f 2072 6563 6f6e  (f'Try  to recon
-0000b500: 6e65 6374 2e2e 2e27 290a 2020 2020 2020  nect...').      
-0000b510: 2020 7365 6c66 2e63 6c6f 7365 5f70 6f72    self.close_por
-0000b520: 7428 290a 2020 2020 2020 2020 7472 793a  t().        try:
-0000b530: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b540: 662e 636f 6e6e 6563 7465 6420 3d20 7365  f.connected = se
-0000b550: 6c66 2e6f 7065 6e5f 706f 7274 2873 656c  lf.open_port(sel
-0000b560: 662e 636f 6d5f 706f 7274 2c20 7365 6c66  f.com_port, self
-0000b570: 2e62 6175 645f 7261 7465 290a 2020 2020  .baud_rate).    
-0000b580: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0000b590: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-0000b5a0: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
-0000b5b0: 6572 2e77 6172 6e69 6e67 2866 2763 6f75  er.warning(f'cou
-0000b5c0: 6c64 206e 6f74 2072 6563 6f6e 6e65 6374  ld not reconnect
-0000b5d0: 2074 6f20 6465 7669 6365 3a20 7b65 7d27   to device: {e}'
-0000b5e0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000b5f0: 2073 656c 662e 636f 6e6e 6563 7465 643a   self.connected:
-0000b600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b610: 2073 656c 662e 696e 6974 5f63 6f6e 6669   self.init_confi
-0000b620: 6775 7261 7469 6f6e 7328 290a 0a20 2020  gurations()..   
-0000b630: 2064 6566 2063 6f6e 6669 6775 7265 2873   def configure(s
-0000b640: 656c 662c 2063 6f6d 6d61 6e64 2c20 7661  elf, command, va
-0000b650: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
-0000b660: 6c66 2e73 6574 5f64 6576 6963 655f 7072  lf.set_device_pr
-0000b670: 6f70 6572 7479 2863 6f6d 6d61 6e64 2c20  operty(command, 
-0000b680: 7661 6c75 6529 0a20 2020 2020 2020 2073  value).        s
-0000b690: 6c65 6570 2830 2e31 290a 2020 2020 2020  leep(0.1).      
-0000b6a0: 2020 7273 7020 3d20 7365 6c66 2e67 6574    rsp = self.get
-0000b6b0: 5f64 6576 6963 655f 7072 6f70 6572 7479  _device_property
-0000b6c0: 2863 6f6d 6d61 6e64 290a 2020 2020 2020  (command).      
-0000b6d0: 2020 6966 2073 7472 2876 616c 7565 2920    if str(value) 
-0000b6e0: 6e6f 7420 696e 2072 7370 3a0a 2020 2020  not in rsp:.    
-0000b6f0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
-0000b700: 6365 7074 696f 6e28 6627 436f 756c 6420  ception(f'Could 
-0000b710: 6e6f 7420 636f 6e66 6967 7572 6520 7b63  not configure {c
-0000b720: 6f6d 6d61 6e64 7d20 746f 207b 7661 6c75  ommand} to {valu
-0000b730: 657d 2e20 7468 6520 7b63 6f6d 6d61 6e64  e}. the {command
-0000b740: 7d20 6973 2063 7572 7265 6e74 6c79 2073  } is currently s
-0000b750: 6574 2074 6f20 7b72 7370 7d27 290a 0a20  et to {rsp}').. 
-0000b760: 2020 2064 6566 2069 6e69 745f 636f 6e66     def init_conf
-0000b770: 6967 7572 6174 696f 6e73 2873 656c 6629  igurations(self)
-0000b780: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
-0000b790: 6f6e 6669 6775 7265 2827 5359 4d42 4f4c  onfigure('SYMBOL
-0000b7a0: 2e51 5227 2c20 274f 4e27 290a 2020 2020  .QR', 'ON').    
-0000b7b0: 2020 2020 7365 6c66 2e63 6f6e 6669 6775      self.configu
-0000b7c0: 7265 2827 5452 4947 4745 522e 5459 5045  re('TRIGGER.TYPE
-0000b7d0: 272c 2073 656c 662e 7472 6967 6765 725f  ', self.trigger_
-0000b7e0: 7479 7065 290a 0a20 2020 2064 6566 2073  type)..    def s
-0000b7f0: 656e 645f 636f 6d6d 616e 6428 7365 6c66  end_command(self
-0000b800: 2c20 636f 6d6d 616e 642c 2063 6f6d 6d61  , command, comma
-0000b810: 6e64 5f69 643d 3132 332c 2063 6865 636b  nd_id=123, check
-0000b820: 7375 6d3d 3029 3a0a 2020 2020 2020 2020  sum=0):.        
-0000b830: 636f 6d6d 616e 645f 6865 6164 6572 203d  command_header =
-0000b840: 2066 277c 7c7b 6368 6563 6b73 756d 7d3a   f'||{checksum}:
-0000b850: 7b63 6f6d 6d61 6e64 5f69 647d 3e27 0a20  {command_id}>'. 
-0000b860: 2020 2020 2020 2066 6f6f 7465 7220 3d20         footer = 
-0000b870: 275c 725c 6e27 0a20 2020 2020 2020 2066  '\r\n'.        f
-0000b880: 756c 6c5f 636f 6d6d 616e 6420 3d20 6627  ull_command = f'
-0000b890: 7b63 6f6d 6d61 6e64 5f68 6561 6465 727d  {command_header}
-0000b8a0: 7b63 6f6d 6d61 6e64 7d7b 666f 6f74 6572  {command}{footer
-0000b8b0: 7d27 0a20 2020 2020 2020 2074 7279 3a0a  }'.        try:.
-0000b8c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b8d0: 2e6c 6f67 6765 722e 696e 666f 2827 4d65  .logger.info('Me
-0000b8e0: 7373 6167 6520 7365 6e74 207b 7d27 2e66  ssage sent {}'.f
-0000b8f0: 6f72 6d61 7428 6675 6c6c 5f63 6f6d 6d61  ormat(full_comma
-0000b900: 6e64 2e65 6e63 6f64 6528 2929 290a 2020  nd.encode())).  
-0000b910: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000b920: 6572 2e77 7269 7465 2866 756c 6c5f 636f  er.write(full_co
-0000b930: 6d6d 616e 642e 656e 636f 6465 2829 290a  mmand.encode()).
-0000b940: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-0000b950: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
-0000b960: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000b970: 2045 7863 6570 7469 6f6e 2866 2246 6169   Exception(f"Fai
-0000b980: 6c65 6420 746f 2073 656e 6420 636f 6d6d  led to send comm
-0000b990: 616e 6420 6475 6520 746f 3a20 7b65 7d22  and due to: {e}"
-0000b9a0: 290a 0a20 2020 2064 6566 2072 6561 645f  )..    def read_
-0000b9b0: 7265 7370 6f6e 7365 2873 656c 6629 3a0a  response(self):.
-0000b9c0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000b9d0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-0000b9e0: 6520 3d20 7365 6c66 2e73 6572 2e72 6561  e = self.ser.rea
-0000b9f0: 646c 696e 6528 292e 6465 636f 6465 2829  dline().decode()
-0000ba00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000ba10: 706f 6e73 6520 3d20 7265 7370 6f6e 7365  ponse = response
-0000ba20: 2e73 7472 6970 2827 5c72 5c6e 2729 0a20  .strip('\r\n'). 
-0000ba30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000ba40: 6e20 7265 7370 6f6e 7365 0a20 2020 2020  n response.     
-0000ba50: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0000ba60: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
-0000ba70: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
-0000ba80: 7074 696f 6e28 6622 4661 696c 6564 2074  ption(f"Failed t
-0000ba90: 6f20 7265 6164 2072 6573 706f 6e73 653a  o read response:
-0000baa0: 207b 657d 2229 0a0a 2020 2020 6465 6620   {e}")..    def 
-0000bab0: 7265 6164 5f62 6174 6368 2873 656c 662c  read_batch(self,
-0000bac0: 206e 5f6d 7367 3d31 3030 302c 2077 6169   n_msg=1000, wai
-0000bad0: 745f 7469 6d65 3d30 2e30 293a 0a20 2020  t_time=0.0):.   
-0000bae0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000baf0: 2077 6169 745f 7469 6d65 2069 6e20 7365   wait_time in se
-0000bb00: 636f 6e64 730a 2020 2020 2020 2020 4070  conds.        @p
-0000bb10: 6172 616d 206e 5f6d 7367 206d 6178 206e  aram n_msg max n
-0000bb20: 756d 6265 7220 6f66 206d 7367 2074 6f20  umber of msg to 
-0000bb30: 7374 6f70 2074 6865 2072 6561 6469 6e67  stop the reading
-0000bb40: 2062 6174 6368 0a20 2020 2020 2020 2040   batch.        @
-0000bb50: 7479 7065 206e 5f6d 7367 2069 6e74 0a20  type n_msg int. 
-0000bb60: 2020 2020 2020 2040 7061 7261 6d20 7761         @param wa
-0000bb70: 6974 5f74 696d 6520 7468 6520 6d61 7820  it_time the max 
-0000bb80: 7469 6d65 2069 6e20 7365 636f 6e64 2074  time in second t
-0000bb90: 696c 6c20 6e65 6564 2074 6f20 7374 6f70  ill need to stop
-0000bba0: 2074 6865 2072 6561 6469 6e67 2062 6174   the reading bat
-0000bbb0: 6368 0a20 2020 2020 2020 2040 7479 7065  ch.        @type
-0000bbc0: 2077 6169 745f 7469 6d65 2066 6c6f 6174   wait_time float
-0000bbd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000bbe0: 2020 2020 2072 7370 5f6f 7574 203d 205b       rsp_out = [
-0000bbf0: 5d0a 2020 2020 2020 2020 745f 7374 6172  ].        t_star
-0000bc00: 7420 3d20 7469 6d65 2829 0a20 2020 2020  t = time().     
-0000bc10: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000bc20: 6528 6e5f 6d73 6729 3a0a 2020 2020 2020  e(n_msg):.      
-0000bc30: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
-0000bc40: 722e 696e 5f77 6169 7469 6e67 203d 3d20  r.in_waiting == 
-0000bc50: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-0000bc60: 2020 2069 6620 7469 6d65 2829 202d 2074     if time() - t
-0000bc70: 5f73 7461 7274 203c 2077 6169 745f 7469  _start < wait_ti
-0000bc80: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
-0000bc90: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
-0000bca0: 3035 3029 0a20 2020 2020 2020 2020 2020  050).           
-0000bcb0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000bcd0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-0000bce0: 2072 7370 203d 2073 656c 662e 7265 6164   rsp = self.read
-0000bcf0: 5f72 6573 706f 6e73 6528 290a 2020 2020  _response().    
-0000bd00: 2020 2020 2020 2020 6966 2072 7370 203d          if rsp =
-0000bd10: 3d20 2727 3a0a 2020 2020 2020 2020 2020  = '':.          
-0000bd20: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-0000bd30: 2020 2020 2020 2020 7273 705f 6f75 742e          rsp_out.
-0000bd40: 6170 7065 6e64 2872 7370 290a 2020 2020  append(rsp).    
-0000bd50: 2020 2020 7265 7475 726e 206c 6973 7428      return list(
-0000bd60: 7365 7428 7273 705f 6f75 7429 290a 0a20  set(rsp_out)).. 
-0000bd70: 2020 2064 6566 2064 6973 636f 7665 725f     def discover_
-0000bd80: 6465 7669 6365 2873 656c 6629 3a0a 2020  device(self):.  
-0000bd90: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
-0000bda0: 636f 6d6d 616e 6428 2747 4554 2044 4556  command('GET DEV
-0000bdb0: 4943 452e 5459 5045 2729 0a20 2020 2020  ICE.TYPE').     
-0000bdc0: 2020 2072 6574 7572 6e20 7365 6c66 2e72     return self.r
-0000bdd0: 6561 645f 7265 7370 6f6e 7365 2829 0a0a  ead_response()..
-0000bde0: 2020 2020 6465 6620 7365 745f 6465 7669      def set_devi
-0000bdf0: 6365 5f70 726f 7065 7274 7928 7365 6c66  ce_property(self
-0000be00: 2c20 7072 6f70 6572 7479 5f6e 616d 652c  , property_name,
-0000be10: 2076 616c 7565 293a 0a20 2020 2020 2020   value):.       
-0000be20: 2073 656c 662e 7365 6e64 5f63 6f6d 6d61   self.send_comma
-0000be30: 6e64 2866 2753 4554 207b 7072 6f70 6572  nd(f'SET {proper
-0000be40: 7479 5f6e 616d 657d 207b 7661 6c75 657d  ty_name} {value}
-0000be50: 2729 0a20 2020 2020 2020 2073 6c65 6570  ').        sleep
-0000be60: 2830 2e31 290a 2020 2020 2020 2020 7265  (0.1).        re
-0000be70: 7475 726e 2073 656c 662e 7265 6164 5f72  turn self.read_r
-0000be80: 6573 706f 6e73 6528 290a 0a20 2020 2064  esponse()..    d
-0000be90: 6566 2067 6574 5f64 6576 6963 655f 7072  ef get_device_pr
-0000bea0: 6f70 6572 7479 2873 656c 662c 2070 726f  operty(self, pro
-0000beb0: 7065 7274 795f 6e61 6d65 293a 0a20 2020  perty_name):.   
-0000bec0: 2020 2020 2073 656c 662e 7365 6e64 5f63       self.send_c
-0000bed0: 6f6d 6d61 6e64 2866 2747 4554 207b 7072  ommand(f'GET {pr
-0000bee0: 6f70 6572 7479 5f6e 616d 657d 2729 0a20  operty_name}'). 
-0000bef0: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
-0000bf00: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000bf10: 2073 656c 662e 7265 6164 5f72 6573 706f   self.read_respo
-0000bf20: 6e73 6528 290a 0a20 2020 2064 6566 2074  nse()..    def t
-0000bf30: 7269 6767 6572 5f6f 6e28 7365 6c66 2c20  rigger_on(self, 
-0000bf40: 636f 6e74 696e 756f 7573 6c79 3d46 616c  continuously=Fal
-0000bf50: 7365 2c20 7472 6967 6765 725f 7479 7065  se, trigger_type
-0000bf60: 3d30 2c20 6e65 6564 5f74 6f5f 636f 6e66  =0, need_to_conf
-0000bf70: 6967 3d54 7275 6529 3a0a 2020 2020 2020  ig=True):.      
-0000bf80: 2020 2222 220a 0a20 2020 2020 2020 2040    """..        @
-0000bf90: 7061 7261 6d20 7472 6967 6765 725f 7479  param trigger_ty
-0000bfa0: 7065 3a20 303a 2053 696e 676c 6520 2865  pe: 0: Single (e
-0000bfb0: 7874 6572 6e61 6c29 2c20 313a 2050 7265  xternal), 1: Pre
-0000bfc0: 7365 6e74 6174 696f 6e20 2869 6e74 6572  sentation (inter
-0000bfd0: 6e61 6c29 2c20 323a 204d 616e 7561 6c20  nal), 2: Manual 
-0000bfe0: 2862 7574 746f 6e29 2c20 333a 2042 7572  (button), 3: Bur
-0000bff0: 7374 2028 6578 7465 726e 616c 292c 0a20  st (external),. 
-0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c010: 2020 2020 343a 2053 656c 6620 2869 6e74      4: Self (int
-0000c020: 6572 6e61 6c29 2c20 353a 2043 6f6e 7469  ernal), 5: Conti
-0000c030: 6e75 6f75 7320 2865 7874 6572 6e61 6c29  nuous (external)
-0000c040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c050: 2020 2020 2020 2a20 5369 6e67 6c65 3a20        * Single: 
-0000c060: 4163 7175 6972 6573 2061 2073 696e 676c  Acquires a singl
-0000c070: 6520 696d 6167 6520 616e 6420 6174 7465  e image and atte
-0000c080: 6d70 7473 2074 6f20 6465 636f 6465 2061  mpts to decode a
-0000c090: 6e79 2073 796d 626f 6c20 6974 2063 6f6e  ny symbol it con
-0000c0a0: 7461 696e 7320 6f72 206d 6f72 6520 7468  tains or more th
-0000c0b0: 616e 206f 6e65 0a20 2020 2020 2020 2020  an one.         
-0000c0c0: 2020 2020 2020 2020 2020 2020 7379 6d62              symb
-0000c0d0: 6f6c 2069 6e20 6361 7365 7320 7768 6572  ol in cases wher
-0000c0e0: 6520 6d75 6c74 6963 6f64 6520 6973 2065  e multicode is e
-0000c0f0: 6e61 626c 6564 2e20 5468 6520 7265 6164  nabled. The read
-0000c100: 6572 2072 656c 6965 7320 6f6e 2061 6e20  er relies on an 
-0000c110: 6578 7465 726e 616c 2074 7269 6767 6572  external trigger
-0000c120: 2073 6f75 7263 652e 0a20 2020 2020 2020   source..       
-0000c130: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
-0000c140: 5072 6573 656e 7461 7469 6f6e 3a20 5265  Presentation: Re
-0000c150: 7065 6174 6564 6c79 2073 6361 6e73 2066  peatedly scans f
-0000c160: 6f72 2061 2073 796d 626f 6c20 616e 6420  or a symbol and 
-0000c170: 6465 636f 6465 7320 6974 2077 6865 6e65  decodes it whene
-0000c180: 7665 7220 6f6e 6520 6973 2064 6574 6563  ver one is detec
-0000c190: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
-0000c1a0: 2020 2020 2020 2020 2020 5468 6520 7265            The re
-0000c1b0: 6164 6572 2072 656c 6965 7320 6f6e 2061  ader relies on a
-0000c1c0: 6e20 696e 7465 726e 616c 2074 696d 696e  n internal timin
-0000c1d0: 6720 6d65 6368 616e 6973 6d20 746f 2061  g mechanism to a
-0000c1e0: 6371 7569 7265 2069 6d61 6765 732e 0a20  cquire images.. 
-0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c200: 2020 2020 2a20 4275 7273 743a 2050 6572      * Burst: Per
-0000c210: 666f 726d 7320 6d75 6c74 6970 6c65 2069  forms multiple i
-0000c220: 6d61 6765 2061 6371 7569 7369 7469 6f6e  mage acquisition
-0000c230: 7320 6261 7365 6420 6f6e 2061 6e20 6578  s based on an ex
-0000c240: 7465 726e 616c 2074 7269 6767 6572 2061  ternal trigger a
-0000c250: 6e64 2064 6563 6f64 6573 206f 6e65 206f  nd decodes one o
-0000c260: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0000c270: 2020 2020 2020 206d 756c 7469 706c 6520         multiple 
-0000c280: 7379 6d62 6f6c 7320 6170 7065 6172 696e  symbols appearin
-0000c290: 6720 696e 2074 6865 2073 6571 7565 6e63  g in the sequenc
-0000c2a0: 6520 6f66 2069 6d61 6765 732e 0a20 2020  e of images..   
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2c0: 2020 2a20 5365 6c66 3a20 5369 6d69 6c61    * Self: Simila
-0000c2d0: 7220 746f 2050 7265 7365 6e74 6174 696f  r to Presentatio
-0000c2e0: 6e20 6d6f 6465 2069 6e20 7468 6174 2074  n mode in that t
-0000c2f0: 6865 2072 6561 6465 7220 7065 7270 6574  he reader perpet
-0000c300: 7561 6c6c 7920 7363 616e 7320 666f 7220  ually scans for 
-0000c310: 7379 6d62 6f6c 7320 616e 6420 6465 636f  symbols and deco
-0000c320: 6465 730a 2020 2020 2020 2020 2020 2020  des.            
-0000c330: 2020 2020 2020 2020 2074 6865 6d20 6561           them ea
-0000c340: 6368 2074 696d 6520 6f6e 6520 6973 2064  ch time one is d
-0000c350: 6574 6563 7465 642e 2055 6e6c 696b 6520  etected. Unlike 
-0000c360: 5072 6573 656e 7461 7469 6f6e 206d 6f64  Presentation mod
-0000c370: 652c 2068 6f77 6576 6572 2c20 5365 6c66  e, however, Self
-0000c380: 206d 6f64 6520 7375 7070 6f72 7473 206d   mode supports m
-0000c390: 756c 7469 636f 6465 0a20 2020 2020 2020  ulticode.       
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000c3b0: 7375 6c74 7320 616e 6420 6120 6465 636f  sults and a deco
-0000c3c0: 6465 2061 7474 656d 7074 206f 6363 7572  de attempt occur
-0000c3d0: 7320 7769 7468 2065 7665 7279 2069 6d61  s with every ima
-0000c3e0: 6765 2e20 5468 6520 6d61 696e 2064 6966  ge. The main dif
-0000c3f0: 6665 7265 6e63 6520 6265 7477 6565 6e20  ference between 
-0000c400: 5365 6c66 2061 6e64 0a20 2020 2020 2020  Self and.       
-0000c410: 2020 2020 2020 2020 2020 2020 2020 5072                Pr
-0000c420: 6573 656e 7461 7469 6f6e 2069 7320 7468  esentation is th
-0000c430: 6520 6669 7865 6420 616e 6420 6578 6163  e fixed and exac
-0000c440: 7420 696e 7465 7276 616c 2066 6f72 2069  t interval for i
-0000c450: 6d61 6765 2061 6371 7569 7369 7469 6f6e  mage acquisition
-0000c460: 7320 696e 2053 656c 662e 0a20 2020 2020  s in Self..     
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c480: 2a20 436f 6e74 696e 756f 7573 3a20 4265  * Continuous: Be
-0000c490: 6769 6e73 2061 6371 7569 7269 6e67 2069  gins acquiring i
-0000c4a0: 6d61 6765 7320 6261 7365 6420 6f6e 2061  mages based on a
-0000c4b0: 2073 696e 676c 6520 6578 7465 726e 616c   single external
-0000c4c0: 2074 7269 6767 6572 2061 6e64 2063 6f6e   trigger and con
-0000c4d0: 7469 6e75 6573 2074 6f20 6163 7175 6972  tinues to acquir
-0000c4e0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000c4f0: 2020 2020 2020 2069 6d61 6765 7320 756e         images un
-0000c500: 7469 6c20 6120 7379 6d62 6f6c 2069 7320  til a symbol is 
-0000c510: 666f 756e 6420 616e 6420 6465 636f 6465  found and decode
-0000c520: 642c 206f 7220 756e 7469 6c20 6d75 6c74  d, or until mult
-0000c530: 6970 6c65 2069 6d61 6765 7320 636f 6e74  iple images cont
-0000c540: 6169 6e69 6e67 2061 7320 6d61 6e79 2063  aining as many c
-0000c550: 6f64 6573 2061 730a 2020 2020 2020 2020  odes as.        
-0000c560: 2020 2020 2020 2020 2020 2020 2073 7065               spe
-0000c570: 6369 6669 6564 2069 6e20 6d75 6c74 6963  cified in multic
-0000c580: 6f64 6520 6d6f 6465 2061 7265 206c 6f63  ode mode are loc
-0000c590: 6174 6564 2c20 6f72 2075 6e74 696c 2074  ated, or until t
-0000c5a0: 6865 2074 7269 6767 6572 2069 7320 7265  he trigger is re
-0000c5b0: 6c65 6173 6564 2e0a 2020 2020 2020 2020  leased..        
-0000c5c0: 4074 7970 6520 7472 6967 6765 725f 7479  @type trigger_ty
-0000c5d0: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
-0000c5e0: 4070 6172 616d 2063 6f6e 7469 6e75 6f75  @param continuou
-0000c5f0: 736c 793a 2069 6620 5472 7565 2c20 7468  sly: if True, th
-0000c600: 6520 7363 616e 6e65 7220 7769 6c6c 2072  e scanner will r
-0000c610: 6561 6420 696e 2063 6f6e 7469 6e75 6f75  ead in continuou
-0000c620: 7320 6d6f 6465 0a20 2020 2020 2020 2040  s mode.        @
-0000c630: 7479 7065 2063 6f6e 7469 6e75 6f75 736c  type continuousl
-0000c640: 793a 2062 6f6f 6c0a 2020 2020 2020 2020  y: bool.        
-0000c650: 4070 6172 616d 206e 6565 645f 746f 5f63  @param need_to_c
-0000c660: 6f6e 6669 673a 2069 6620 5472 7565 2c20  onfig: if True, 
-0000c670: 6669 7273 7420 7468 6520 7363 616e 6e65  first the scanne
-0000c680: 7220 6973 2063 6f6e 6669 6775 7265 6420  r is configured 
-0000c690: 7769 7468 2074 6865 2072 656c 6576 616e  with the relevan
-0000c6a0: 7420 7472 6967 6765 7220 7479 7065 0a20  t trigger type. 
-0000c6b0: 2020 2020 2020 2040 7479 7065 206e 6565         @type nee
-0000c6c0: 645f 746f 5f63 6f6e 6669 673a 2062 6f6f  d_to_config: boo
-0000c6d0: 6c0a 2020 2020 2020 2020 4072 6574 7572  l.        @retur
-0000c6e0: 6e3a 0a20 2020 2020 2020 2040 7274 7970  n:.        @rtyp
-0000c6f0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-0000c700: 2020 2020 2020 2069 6620 6e65 6564 5f74         if need_t
-0000c710: 6f5f 636f 6e66 6967 3a0a 2020 2020 2020  o_config:.      
-0000c720: 2020 2020 2020 6966 2063 6f6e 7469 6e75        if continu
-0000c730: 6f75 736c 7920 616e 6420 7472 6967 6765  ously and trigge
-0000c740: 725f 7479 7065 203d 3d20 303a 0a20 2020  r_type == 0:.   
-0000c750: 2020 2020 2020 2020 2020 2020 2074 7269               tri
-0000c760: 6767 6572 5f74 7970 6520 3d20 7365 6c66  gger_type = self
-0000c770: 2e43 4f4e 5449 4e55 4f55 535f 5452 4947  .CONTINUOUS_TRIG
-0000c780: 4745 525f 5459 5045 0a20 2020 2020 2020  GER_TYPE.       
-0000c790: 2020 2020 2073 656c 662e 7365 745f 6465       self.set_de
-0000c7a0: 7669 6365 5f70 726f 7065 7274 7928 2754  vice_property('T
-0000c7b0: 5249 4747 4552 2e54 5950 4527 2c20 7472  RIGGER.TYPE', tr
-0000c7c0: 6967 6765 725f 7479 7065 290a 2020 2020  igger_type).    
-0000c7d0: 2020 2020 7365 6c66 2e73 656e 645f 636f      self.send_co
-0000c7e0: 6d6d 616e 6428 2754 5249 4747 4552 204f  mmand('TRIGGER O
-0000c7f0: 4e27 290a 0a20 2020 2064 6566 2074 7269  N')..    def tri
-0000c800: 6767 6572 5f6f 6666 2873 656c 6629 3a0a  gger_off(self):.
-0000c810: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-0000c820: 645f 636f 6d6d 616e 6428 2754 5249 4747  d_command('TRIGG
-0000c830: 4552 204f 4646 2729 0a0a 2020 2020 6465  ER OFF')..    de
-0000c840: 6620 7265 7365 7428 7365 6c66 293a 0a20  f reset(self):. 
-0000c850: 2020 2020 2020 2077 6169 7469 6e67 5f62         waiting_b
-0000c860: 7974 6573 203d 2073 656c 662e 7365 722e  ytes = self.ser.
-0000c870: 696e 5f77 6169 7469 6e67 0a20 2020 2020  in_waiting.     
-0000c880: 2020 2069 6620 7761 6974 696e 675f 6279     if waiting_by
-0000c890: 7465 7320 213d 2030 3a0a 2020 2020 2020  tes != 0:.      
-0000c8a0: 2020 2020 2020 7365 6c66 2e73 6572 2e72        self.ser.r
-0000c8b0: 6573 6574 5f69 6e70 7574 5f62 7566 6665  eset_input_buffe
-0000c8c0: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
-0000c8d0: 7365 6c66 2e6c 6f67 6765 722e 696e 666f  self.logger.info
-0000c8e0: 2866 2763 6c65 616e 2062 7566 6665 7220  (f'clean buffer 
-0000c8f0: 6672 6f6d 207b 7761 6974 696e 675f 6279  from {waiting_by
-0000c900: 7465 737d 2062 7974 6573 2729 0a0a 2020  tes} bytes')..  
-0000c910: 2020 6465 6620 7363 616e 5f65 7874 5f69    def scan_ext_i
-0000c920: 6428 7365 6c66 2c20 6e65 6564 5f74 6f5f  d(self, need_to_
-0000c930: 7472 6967 6765 723d 5472 7565 293a 0a20  trigger=True):. 
-0000c940: 2020 2020 2020 2069 6620 6e65 6564 5f74         if need_t
-0000c950: 6f5f 7472 6967 6765 723a 0a20 2020 2020  o_trigger:.     
-0000c960: 2020 2020 2020 2073 656c 662e 7472 6967         self.trig
-0000c970: 6765 725f 6f6e 286e 6565 645f 746f 5f63  ger_on(need_to_c
-0000c980: 6f6e 6669 673d 4661 6c73 6529 0a0a 2020  onfig=False)..  
-0000c990: 2020 2020 2020 7273 7020 3d20 7365 6c66        rsp = self
-0000c9a0: 2e72 6561 645f 7265 7370 6f6e 7365 2829  .read_response()
-0000c9b0: 0a20 2020 2020 2020 2069 6620 7273 7020  .        if rsp 
-0000c9c0: 3d3d 2027 273a 0a20 2020 2020 2020 2020  == '':.         
-0000c9d0: 2020 2072 6574 7572 6e20 4e6f 6e65 2c20     return None, 
-0000c9e0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
-0000c9f0: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-0000ca00: 2872 7370 2920 3d3d 2073 656c 662e 5347  (rsp) == self.SG
-0000ca10: 5449 4e5f 5354 5249 505f 4c45 4e20 6f72  TIN_STRIP_LEN or
-0000ca20: 206c 656e 2872 7370 2920 3d3d 2073 656c   len(rsp) == sel
-0000ca30: 662e 5347 5449 4e5f 4c45 4e3a 0a20 2020  f.SGTIN_LEN:.   
-0000ca40: 2020 2020 2020 2020 2063 7572 5f69 6420           cur_id 
-0000ca50: 3d20 7273 702e 7370 6c69 7428 2754 2729  = rsp.split('T')
-0000ca60: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
-0000ca70: 6774 696e 5f61 6e64 5f72 6565 6c5f 6964  gtin_and_reel_id
-0000ca80: 203d 2072 7370 2e73 706c 6974 2827 5427   = rsp.split('T'
-0000ca90: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
-0000caa0: 2072 6565 6c5f 6964 203d 2067 7469 6e5f   reel_id = gtin_
-0000cab0: 616e 645f 7265 656c 5f69 645b 2d73 656c  and_reel_id[-sel
-0000cac0: 662e 5245 454c 5f49 445f 4c45 4e3a 5d0a  f.REEL_ID_LEN:].
-0000cad0: 2020 2020 2020 2020 2020 2020 6774 696e              gtin
-0000cae0: 203d 2067 7469 6e5f 616e 645f 7265 656c   = gtin_and_reel
-0000caf0: 5f69 645b 3a2d 7365 6c66 2e52 4545 4c5f  _id[:-self.REEL_
-0000cb00: 4944 5f4c 454e 5d0a 2020 2020 2020 2020  ID_LEN].        
-0000cb10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000cb20: 2020 6375 725f 6964 203d 2072 7370 2e73    cur_id = rsp.s
-0000cb30: 706c 6974 2827 5427 295b 315d 0a20 2020  plit('T')[1].   
-0000cb40: 2020 2020 2020 2020 2072 6565 6c5f 6964           reel_id
-0000cb50: 203d 2072 7370 2e73 706c 6974 2827 5427   = rsp.split('T'
-0000cb60: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
-0000cb70: 2067 7469 6e20 3d20 2727 0a20 2020 2020   gtin = ''.     
-0000cb80: 2020 2072 6574 7572 6e20 7273 702c 2063     return rsp, c
-0000cb90: 7572 5f69 642c 2072 6565 6c5f 6964 2c20  ur_id, reel_id, 
-0000cba0: 6774 696e 0a0a 2020 2020 6465 6620 6265  gtin..    def be
-0000cbb0: 6570 2873 656c 662c 2064 7572 6174 696f  ep(self, duratio
-0000cbc0: 6e29 3a0a 2020 2020 2020 2020 7365 6c66  n):.        self
-0000cbd0: 2e73 656e 645f 636f 6d6d 616e 6428 6627  .send_command(f'
-0000cbe0: 4245 4550 207b 6475 7261 7469 6f6e 7d27  BEEP {duration}'
-0000cbf0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000cc00: 2073 656c 662e 7265 6164 5f72 6573 706f   self.read_respo
-0000cc10: 6e73 6528 290a 0a20 2020 2064 6566 2073  nse()..    def s
-0000cc20: 6574 5f64 6563 6f64 6572 5f72 6f69 2873  et_decoder_roi(s
-0000cc30: 656c 662c 2078 312c 2078 322c 2079 312c  elf, x1, x2, y1,
-0000cc40: 2079 3229 3a0a 2020 2020 2020 2020 7365   y2):.        se
-0000cc50: 6c66 2e73 656e 645f 636f 6d6d 616e 6428  lf.send_command(
-0000cc60: 6627 5345 5420 4445 434f 4445 522e 524f  f'SET DECODER.RO
-0000cc70: 4920 7b78 317d 2c20 7b78 327d 2c20 7b79  I {x1}, {x2}, {y
-0000cc80: 317d 2c20 7b79 327d 2729 0a20 2020 2020  1}, {y2}').     
-0000cc90: 2020 2072 6574 7572 6e20 7365 6c66 2e72     return self.r
-0000cca0: 6561 645f 7265 7370 6f6e 7365 2829 0a0a  ead_response()..
-0000ccb0: 2020 2020 6465 6620 7365 745f 6674 705f      def set_ftp_
-0000ccc0: 696d 6167 655f 6970 5f61 6464 7265 7373  image_ip_address
-0000ccd0: 2873 656c 662c 2069 705f 6164 6472 6573  (self, ip_addres
-0000cce0: 7329 3a0a 2020 2020 2020 2020 7365 6c66  s):.        self
-0000ccf0: 2e73 656e 645f 636f 6d6d 616e 6428 6627  .send_command(f'
-0000cd00: 5345 5420 4654 502d 494d 4147 452e 4950  SET FTP-IMAGE.IP
-0000cd10: 2d41 4444 5245 5353 207b 6970 5f61 6464  -ADDRESS {ip_add
-0000cd20: 7265 7373 7d27 290a 2020 2020 2020 2020  ress}').        
-0000cd30: 7265 7475 726e 2073 656c 662e 7265 6164  return self.read
-0000cd40: 5f72 6573 706f 6e73 6528 290a 0a20 2020  _response()..   
-0000cd50: 2064 6566 2067 6574 5f6d 6163 5f61 6464   def get_mac_add
-0000cd60: 7265 7373 2873 656c 6629 3a0a 2020 2020  ress(self):.    
-0000cd70: 2020 2020 7365 6c66 2e73 656e 645f 636f      self.send_co
-0000cd80: 6d6d 616e 6428 2747 4554 2044 4556 4943  mmand('GET DEVIC
-0000cd90: 452e 4d41 432d 4144 4452 4553 5327 290a  E.MAC-ADDRESS').
-0000cda0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000cdb0: 656c 662e 7265 6164 5f72 6573 706f 6e73  elf.read_respons
-0000cdc0: 6528 290a 0a20 2020 2064 6566 2063 6c6f  e()..    def clo
-0000cdd0: 7365 5f70 6f72 7428 7365 6c66 293a 0a20  se_port(self):. 
-0000cde0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0000cdf0: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
-0000ce00: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-0000ce10: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0000ce20: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
-0000ce30: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
-0000ce40: 696f 6e28 6622 4661 696c 6564 2074 6f20  ion(f"Failed to 
-0000ce50: 636c 6f73 6520 7365 7269 616c 2070 6f72  close serial por
-0000ce60: 743a 207b 657d 2229 0a0a 0a63 6c61 7373  t: {e}")...class
-0000ce70: 2059 6f63 746f 5465 6d70 6572 6174 7572   YoctoTemperatur
-0000ce80: 6553 656e 736f 7228 6f62 6a65 6374 293a  eSensor(object):
-0000ce90: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000cea0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-0000ceb0: 2073 656c 662e 7365 6e73 6f72 203d 204e   self.sensor = N
-0000cec0: 6f6e 650a 2020 2020 2020 2020 6572 726d  one.        errm
-0000ced0: 7367 203d 2059 5265 6650 6172 616d 2829  sg = YRefParam()
-0000cee0: 0a20 2020 2020 2020 2023 2053 6574 7570  .        # Setup
-0000cef0: 2074 6865 2041 5049 2074 6f20 7573 6520   the API to use 
-0000cf00: 6c6f 6361 6c20 5553 4220 6465 7669 6365  local USB device
-0000cf10: 730a 2020 2020 2020 2020 6966 2059 4150  s.        if YAP
-0000cf20: 492e 5265 6769 7374 6572 4875 6228 2275  I.RegisterHub("u
-0000cf30: 7362 222c 2065 7272 6d73 6729 2021 3d20  sb", errmsg) != 
-0000cf40: 5941 5049 2e53 5543 4345 5353 3a0a 2020  YAPI.SUCCESS:.  
-0000cf50: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000cf60: 4571 7569 706d 656e 7445 7272 6f72 2827  EquipmentError('
-0000cf70: 796f 6374 6f20 7465 6d70 6572 6174 7572  yocto temperatur
-0000cf80: 6520 7365 6e73 6f72 2067 6f74 2069 6e69  e sensor got ini
-0000cf90: 7420 6572 726f 723a 207b 7d27 2e66 6f72  t error: {}'.for
-0000cfa0: 6d61 7428 6572 726d 7367 2e76 616c 7565  mat(errmsg.value
-0000cfb0: 2929 0a0a 2020 2020 6465 6620 636f 6e6e  ))..    def conn
-0000cfc0: 6563 7428 7365 6c66 2c20 7461 7267 6574  ect(self, target
-0000cfd0: 3d27 616e 7927 293a 0a20 2020 2020 2020  ='any'):.       
-0000cfe0: 2069 6620 7461 7267 6574 203d 3d20 2761   if target == 'a
-0000cff0: 6e79 273a 0a20 2020 2020 2020 2020 2020  ny':.           
-0000d000: 2023 2072 6574 7269 6576 6520 616e 7920   # retrieve any 
-0000d010: 7465 6d70 6572 6174 7572 6520 7365 6e73  temperature sens
-0000d020: 6f72 0a20 2020 2020 2020 2020 2020 2073  or.            s
-0000d030: 656c 662e 7365 6e73 6f72 203d 2059 5465  elf.sensor = YTe
-0000d040: 6d70 6572 6174 7572 652e 4669 7273 7454  mperature.FirstT
-0000d050: 656d 7065 7261 7475 7265 2829 0a20 2020  emperature().   
-0000d060: 2020 2020 2065 6c69 6620 7461 7267 6574       elif target
-0000d070: 203d 3d20 2727 3a0a 2020 2020 2020 2020   == '':.        
-0000d080: 2020 2020 7072 696e 7428 2773 7065 6369      print('speci
-0000d090: 6669 6564 2069 6e76 616c 6964 2074 6172  fied invalid tar
-0000d0a0: 6765 7427 290a 2020 2020 2020 2020 2020  get').          
-0000d0b0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-0000d0c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000d0d0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000d0e0: 6e73 6f72 203d 2059 5465 6d70 6572 6174  nsor = YTemperat
-0000d0f0: 7572 652e 4669 6e64 5465 6d70 6572 6174  ure.FindTemperat
-0000d100: 7572 6528 7461 7267 6574 202b 2027 2e74  ure(target + '.t
-0000d110: 656d 7065 7261 7475 7265 2729 0a20 2020  emperature').   
-0000d120: 2020 2020 2069 6620 7365 6c66 2e73 656e       if self.sen
-0000d130: 736f 7220 6973 204e 6f6e 6520 6f72 2073  sor is None or s
-0000d140: 656c 662e 6765 745f 7365 6e73 6f72 5f6e  elf.get_sensor_n
-0000d150: 616d 6528 2920 3d3d 2027 756e 7265 736f  ame() == 'unreso
-0000d160: 6c76 6564 273a 0a20 2020 2020 2020 2020  lved':.         
-0000d170: 2020 2070 7269 6e74 2827 4e6f 206d 6f64     print('No mod
-0000d180: 756c 6520 636f 6e6e 6563 7465 6427 290a  ule connected').
-0000d190: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d1a0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0000d1b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000d1c0: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-0000d1d0: 2020 2020 6465 6620 6765 745f 7365 6e73      def get_sens
-0000d1e0: 6f72 5f6e 616d 6528 7365 6c66 293a 0a20  or_name(self):. 
-0000d1f0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0000d200: 656e 736f 7220 6973 204e 6f6e 653a 0a20  ensor is None:. 
-0000d210: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000d220: 2827 6e6f 2073 656e 736f 7220 6973 2063  ('no sensor is c
-0000d230: 6f6e 6e65 6374 6564 2e20 7472 7920 746f  onnected. try to
-0000d240: 2063 616c 6c20 636f 6e6e 6563 7428 2920   call connect() 
-0000d250: 6669 7273 7427 290a 2020 2020 2020 2020  first').        
-0000d260: 2020 2020 7265 7475 726e 2027 270a 0a20      return ''.. 
-0000d270: 2020 2020 2020 2073 656e 736f 725f 7374         sensor_st
-0000d280: 7220 3d20 7365 6c66 2e73 656e 736f 722e  r = self.sensor.
-0000d290: 6465 7363 7269 6265 2829 0a20 2020 2020  describe().     
-0000d2a0: 2020 206e 616d 655f 7374 7220 3d20 7365     name_str = se
-0000d2b0: 6e73 6f72 5f73 7472 2e73 706c 6974 2827  nsor_str.split('
-0000d2c0: 3d27 295b 315d 2e73 706c 6974 2827 2e27  =')[1].split('.'
-0000d2d0: 295b 305d 0a20 2020 2020 2020 2072 6574  )[0].        ret
-0000d2e0: 7572 6e20 6e61 6d65 5f73 7472 0a0a 2020  urn name_str..  
-0000d2f0: 2020 6465 6620 6765 745f 7465 6d70 6572    def get_temper
-0000d300: 6174 7572 6528 7365 6c66 293a 0a20 2020  ature(self):.   
-0000d310: 2020 2020 2069 6620 7365 6c66 2e73 656e       if self.sen
-0000d320: 736f 7220 6973 204e 6f6e 653a 0a20 2020  sor is None:.   
-0000d330: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-0000d340: 7365 6e73 6f72 2069 7320 6e6f 7420 636f  sensor is not co
-0000d350: 6e6e 6563 7465 642e 2074 7279 2074 6f20  nnected. try to 
-0000d360: 6361 6c6c 2063 6f6e 6e65 6374 2829 2066  call connect() f
-0000d370: 6972 7374 2729 0a20 2020 2020 2020 2020  irst').         
-0000d380: 2020 2072 6574 7572 6e20 666c 6f61 7428     return float(
-0000d390: 276e 616e 2729 0a20 2020 2020 2020 2069  'nan').        i
-0000d3a0: 6620 6e6f 7420 2873 656c 662e 7365 6e73  f not (self.sens
-0000d3b0: 6f72 2e69 734f 6e6c 696e 6528 2929 3a0a  or.isOnline()):.
-0000d3c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000d3d0: 7428 2773 656e 736f 7220 6973 206e 6f74  t('sensor is not
-0000d3e0: 2063 6f6e 6e65 6374 6564 206f 7220 6469   connected or di
-0000d3f0: 7363 6f6e 6e65 6374 6564 2064 7572 696e  sconnected durin
-0000d400: 6720 7275 6e27 290a 2020 2020 2020 2020  g run').        
-0000d410: 2020 2020 7265 7475 726e 2066 6c6f 6174      return float
-0000d420: 2827 6e61 6e27 290a 0a20 2020 2020 2020  ('nan')..       
-0000d430: 2072 6574 7572 6e20 7365 6c66 2e73 656e   return self.sen
-0000d440: 736f 722e 6765 745f 6375 7272 656e 7456  sor.get_currentV
-0000d450: 616c 7565 2829 0a0a 2020 2020 4073 7461  alue()..    @sta
-0000d460: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-0000d470: 6620 6578 6974 5f61 7070 2829 3a0a 2020  f exit_app():.  
-0000d480: 2020 2020 2020 5941 5049 2e46 7265 6541        YAPI.FreeA
-0000d490: 5049 2829 0a0a 0a63 6c61 7373 2059 6f63  PI()...class Yoc
-0000d4a0: 746f 5365 6e73 6f72 286f 626a 6563 7429  toSensor(object)
-0000d4b0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0000d4c0: 5f5f 2873 656c 662c 206c 6f67 6765 7229  __(self, logger)
-0000d4d0: 3a0a 2020 2020 2020 2020 7365 6c66 2e74  :.        self.t
-0000d4e0: 656d 7065 7261 7475 7265 5f73 656e 736f  emperature_senso
-0000d4f0: 7220 3d20 4e6f 6e65 0a20 2020 2020 2020  r = None.       
-0000d500: 2073 656c 662e 6875 6d69 6469 7479 5f73   self.humidity_s
-0000d510: 656e 736f 7220 3d20 4e6f 6e65 0a20 2020  ensor = None.   
-0000d520: 2020 2020 2073 656c 662e 6c69 6768 745f       self.light_
-0000d530: 7365 6e73 6f72 203d 204e 6f6e 650a 2020  sensor = None.  
-0000d540: 2020 2020 2020 7365 6c66 2e6c 6f67 6765        self.logge
-0000d550: 7220 3d20 6c6f 6767 6572 0a20 2020 2020  r = logger.     
-0000d560: 2020 2065 7272 6d73 6720 3d20 5952 6566     errmsg = YRef
-0000d570: 5061 7261 6d28 290a 2020 2020 2020 2020  Param().        
-0000d580: 6966 2059 4150 492e 5265 6769 7374 6572  if YAPI.Register
-0000d590: 4875 6228 2275 7362 222c 2065 7272 6d73  Hub("usb", errms
-0000d5a0: 6729 2021 3d20 5941 5049 2e53 5543 4345  g) != YAPI.SUCCE
-0000d5b0: 5353 3a0a 2020 2020 2020 2020 2020 2020  SS:.            
-0000d5c0: 7261 6973 6520 4571 7569 706d 656e 7445  raise EquipmentE
-0000d5d0: 7272 6f72 2866 2759 6f63 746f 2073 656e  rror(f'Yocto sen
-0000d5e0: 736f 7220 696e 6974 6961 6c69 7a61 7469  sor initializati
-0000d5f0: 6f6e 2065 7272 6f72 3a20 7b65 7272 6d73  on error: {errms
-0000d600: 672e 7661 6c75 657d 2729 0a20 2020 2020  g.value}').     
-0000d610: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000d620: 2020 2020 7365 6c66 2e63 6f6e 6e65 6374      self.connect
-0000d630: 2829 0a20 2020 2020 2020 2065 7863 6570  ().        excep
-0000d640: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-0000d650: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000d660: 656c 662e 6c6f 6767 6572 2e69 6e66 6f28  elf.logger.info(
-0000d670: 2753 656e 736f 7220 6973 206e 6f74 2063  'Sensor is not c
-0000d680: 6f6e 6e65 6374 6564 2729 0a0a 2020 2020  onnected')..    
-0000d690: 6465 6620 636f 6e6e 6563 7428 7365 6c66  def connect(self
-0000d6a0: 2c20 7461 7267 6574 3d27 616e 7927 293a  , target='any'):
-0000d6b0: 0a20 2020 2020 2020 2073 656e 736f 725f  .        sensor_
-0000d6c0: 6d61 7070 696e 6720 3d20 7b0a 2020 2020  mapping = {.    
-0000d6d0: 2020 2020 2020 2020 2774 656d 7065 7261          'tempera
-0000d6e0: 7475 7265 273a 2028 5954 656d 7065 7261  ture': (YTempera
-0000d6f0: 7475 7265 2e46 6972 7374 5465 6d70 6572  ture.FirstTemper
-0000d700: 6174 7572 652c 2059 5465 6d70 6572 6174  ature, YTemperat
-0000d710: 7572 652e 4669 6e64 5465 6d70 6572 6174  ure.FindTemperat
-0000d720: 7572 6529 2c0a 2020 2020 2020 2020 2020  ure),.          
-0000d730: 2020 2768 756d 6964 6974 7927 3a20 2859    'humidity': (Y
-0000d740: 4875 6d69 6469 7479 2e46 6972 7374 4875  Humidity.FirstHu
-0000d750: 6d69 6469 7479 2c20 5948 756d 6964 6974  midity, YHumidit
-0000d760: 792e 4669 6e64 4875 6d69 6469 7479 292c  y.FindHumidity),
-0000d770: 0a20 2020 2020 2020 2020 2020 2027 6c69  .            'li
-0000d780: 6768 7427 3a20 2859 4c69 6768 7453 656e  ght': (YLightSen
-0000d790: 736f 722e 4669 7273 744c 6967 6874 5365  sor.FirstLightSe
-0000d7a0: 6e73 6f72 2c20 594c 6967 6874 5365 6e73  nsor, YLightSens
-0000d7b0: 6f72 2e46 696e 644c 6967 6874 5365 6e73  or.FindLightSens
-0000d7c0: 6f72 290a 2020 2020 2020 2020 7d0a 0a20  or).        }.. 
-0000d7d0: 2020 2020 2020 2069 6620 6e6f 7420 7461         if not ta
-0000d7e0: 7267 6574 3a0a 2020 2020 2020 2020 2020  rget:.          
-0000d7f0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000d800: 6f72 2827 496e 7661 6c69 6420 7461 7267  or('Invalid targ
-0000d810: 6574 2073 7065 6369 6669 6564 2729 0a0a  et specified')..
-0000d820: 2020 2020 2020 2020 7461 7267 6574 7320          targets 
-0000d830: 3d20 7461 7267 6574 2e73 706c 6974 2827  = target.split('
-0000d840: 2c27 2920 6966 2074 6172 6765 7420 213d  ,') if target !=
-0000d850: 2027 616e 7927 2065 6c73 6520 7365 6e73   'any' else sens
-0000d860: 6f72 5f6d 6170 7069 6e67 2e6b 6579 7328  or_mapping.keys(
-0000d870: 290a 0a20 2020 2020 2020 2066 6f72 2073  )..        for s
-0000d880: 656e 736f 725f 7479 7065 2069 6e20 7461  ensor_type in ta
-0000d890: 7267 6574 733a 0a20 2020 2020 2020 2020  rgets:.         
-0000d8a0: 2020 2069 6620 7365 6e73 6f72 5f74 7970     if sensor_typ
-0000d8b0: 6520 6e6f 7420 696e 2073 656e 736f 725f  e not in sensor_
-0000d8c0: 6d61 7070 696e 673a 0a20 2020 2020 2020  mapping:.       
-0000d8d0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-0000d8e0: 6767 6572 2e77 6172 6e69 6e67 2866 2757  gger.warning(f'W
-0000d8f0: 6172 6e69 6e67 3a20 556e 6b6e 6f77 6e20  arning: Unknown 
-0000d900: 7365 6e73 6f72 2074 7970 6520 227b 7365  sensor type "{se
-0000d910: 6e73 6f72 5f74 7970 657d 222e 2053 6b69  nsor_type}". Ski
-0000d920: 7070 696e 672e 2e2e 2729 0a20 2020 2020  pping...').     
-0000d930: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000d940: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
-0000d950: 2073 656e 736f 7220 3d20 7365 6e73 6f72   sensor = sensor
-0000d960: 5f6d 6170 7069 6e67 5b73 656e 736f 725f  _mapping[sensor_
-0000d970: 7479 7065 5d5b 305d 2829 2069 6620 7461  type][0]() if ta
-0000d980: 7267 6574 203d 3d20 2761 6e79 2720 656c  rget == 'any' el
-0000d990: 7365 2073 656e 736f 725f 6d61 7070 696e  se sensor_mappin
-0000d9a0: 675b 7365 6e73 6f72 5f74 7970 655d 5b31  g[sensor_type][1
-0000d9b0: 5d28 0a20 2020 2020 2020 2020 2020 2020  ](.             
-0000d9c0: 2020 2066 277b 7365 6e73 6f72 5f74 7970     f'{sensor_typ
-0000d9d0: 657d 2e7b 7365 6e73 6f72 5f74 7970 657d  e}.{sensor_type}
-0000d9e0: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
-0000d9f0: 6574 6174 7472 2873 656c 662c 2066 277b  etattr(self, f'{
-0000da00: 7365 6e73 6f72 5f74 7970 657d 5f73 656e  sensor_type}_sen
-0000da10: 736f 7227 2c20 7365 6e73 6f72 290a 0a20  sor', sensor).. 
-0000da20: 2020 2020 2020 2069 6620 6e6f 7420 616e         if not an
-0000da30: 7928 6765 7461 7474 7228 7365 6c66 2c20  y(getattr(self, 
-0000da40: 6627 7b73 656e 736f 725f 7479 7065 7d5f  f'{sensor_type}_
-0000da50: 7365 6e73 6f72 2729 2066 6f72 2073 656e  sensor') for sen
-0000da60: 736f 725f 7479 7065 2069 6e20 7461 7267  sor_type in targ
-0000da70: 6574 7329 3a0a 2020 2020 2020 2020 2020  ets):.          
-0000da80: 2020 7261 6973 6520 4571 7569 706d 656e    raise Equipmen
-0000da90: 7445 7272 6f72 2827 4e6f 206d 6f64 756c  tError('No modul
-0000daa0: 6520 636f 6e6e 6563 7465 6427 290a 0a20  e connected').. 
-0000dab0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000dac0: 7565 0a0a 2020 2020 6465 6620 6765 745f  ue..    def get_
-0000dad0: 7365 6e73 6f72 5f6e 616d 6573 2873 656c  sensor_names(sel
-0000dae0: 6629 3a0a 2020 2020 2020 2020 6e61 6d65  f):.        name
-0000daf0: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
-0000db00: 6f72 2073 656e 736f 7220 696e 205b 7365  or sensor in [se
-0000db10: 6c66 2e74 656d 7065 7261 7475 7265 5f73  lf.temperature_s
-0000db20: 656e 736f 722c 2073 656c 662e 6875 6d69  ensor, self.humi
-0000db30: 6469 7479 5f73 656e 736f 722c 2073 656c  dity_sensor, sel
-0000db40: 662e 6c69 6768 745f 7365 6e73 6f72 5d3a  f.light_sensor]:
-0000db50: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000db60: 7365 6e73 6f72 3a0a 2020 2020 2020 2020  sensor:.        
-0000db70: 2020 2020 2020 2020 6e61 6d65 5f73 7472          name_str
-0000db80: 203d 2073 656e 736f 722e 6465 7363 7269   = sensor.descri
-0000db90: 6265 2829 2e73 706c 6974 2827 3d27 295b  be().split('=')[
-0000dba0: 315d 2e73 706c 6974 2827 2e27 295b 305d  1].split('.')[0]
-0000dbb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dbc0: 206e 616d 6573 2e61 7070 656e 6428 6e61   names.append(na
-0000dbd0: 6d65 5f73 7472 290a 0a20 2020 2020 2020  me_str)..       
-0000dbe0: 2069 6620 6e6f 7420 6e61 6d65 733a 0a20   if not names:. 
-0000dbf0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000dc00: 2045 7175 6970 6d65 6e74 4572 726f 7228   EquipmentError(
-0000dc10: 274e 6f20 7365 6e73 6f72 2069 7320 636f  'No sensor is co
-0000dc20: 6e6e 6563 7465 642e 2054 7279 2074 6f20  nnected. Try to 
-0000dc30: 6361 6c6c 2063 6f6e 6e65 6374 2829 2066  call connect() f
-0000dc40: 6972 7374 2729 0a0a 2020 2020 2020 2020  irst')..        
-0000dc50: 7265 7475 726e 206e 616d 6573 0a0a 2020  return names..  
-0000dc60: 2020 6465 6620 6765 745f 7465 6d70 6572    def get_temper
-0000dc70: 6174 7572 6528 7365 6c66 293a 0a20 2020  ature(self):.   
-0000dc80: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000dc90: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000dca0: 662e 5f67 6574 5f73 656e 736f 725f 7661  f._get_sensor_va
-0000dcb0: 6c75 6528 7365 6c66 2e74 656d 7065 7261  lue(self.tempera
-0000dcc0: 7475 7265 5f73 656e 736f 722c 2027 7465  ture_sensor, 'te
-0000dcd0: 6d70 6572 6174 7572 6527 290a 2020 2020  mperature').    
-0000dce0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0000dcf0: 7469 6f6e 2061 7320 6565 3a0a 2020 2020  tion as ee:.    
-0000dd00: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
-0000dd10: 0a0a 2020 2020 6465 6620 6765 745f 6875  ..    def get_hu
-0000dd20: 6d69 6469 7479 2873 656c 6629 3a0a 2020  midity(self):.  
-0000dd30: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000dd40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000dd50: 6c66 2e5f 6765 745f 7365 6e73 6f72 5f76  lf._get_sensor_v
-0000dd60: 616c 7565 2873 656c 662e 6875 6d69 6469  alue(self.humidi
-0000dd70: 7479 5f73 656e 736f 722c 2027 6875 6d69  ty_sensor, 'humi
-0000dd80: 6469 7479 2729 0a20 2020 2020 2020 2065  dity').        e
-0000dd90: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0000dda0: 6173 2065 653a 0a20 2020 2020 2020 2020  as ee:.         
-0000ddb0: 2020 2072 6574 7572 6e20 300a 0a20 2020     return 0..   
-0000ddc0: 2064 6566 2067 6574 5f6c 6967 6874 2873   def get_light(s
-0000ddd0: 656c 6629 3a0a 2020 2020 2020 2020 7472  elf):.        tr
-0000dde0: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
-0000ddf0: 6574 7572 6e20 7365 6c66 2e5f 6765 745f  eturn self._get_
-0000de00: 7365 6e73 6f72 5f76 616c 7565 2873 656c  sensor_value(sel
-0000de10: 662e 6c69 6768 745f 7365 6e73 6f72 2c20  f.light_sensor, 
-0000de20: 276c 6967 6874 2729 0a20 2020 2020 2020  'light').       
-0000de30: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0000de40: 6e20 6173 2065 653a 0a20 2020 2020 2020  n as ee:.       
-0000de50: 2020 2020 2072 6574 7572 6e20 300a 0a20       return 0.. 
-0000de60: 2020 2064 6566 205f 6765 745f 7365 6e73     def _get_sens
-0000de70: 6f72 5f76 616c 7565 2873 656c 662c 2073  or_value(self, s
-0000de80: 656e 736f 722c 2073 656e 736f 725f 7479  ensor, sensor_ty
-0000de90: 7065 293a 0a20 2020 2020 2020 2069 6620  pe):.        if 
-0000dea0: 6e6f 7420 7365 6e73 6f72 206f 7220 6e6f  not sensor or no
-0000deb0: 7420 7365 6e73 6f72 2e69 734f 6e6c 696e  t sensor.isOnlin
-0000dec0: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
-0000ded0: 2072 6169 7365 2045 7175 6970 6d65 6e74   raise Equipment
-0000dee0: 4572 726f 7228 6627 7b73 656e 736f 725f  Error(f'{sensor_
-0000def0: 7479 7065 2e63 6170 6974 616c 697a 6528  type.capitalize(
-0000df00: 297d 2073 656e 736f 7220 6973 206e 6f74  )} sensor is not
-0000df10: 2063 6f6e 6e65 6374 6564 2e20 5472 7920   connected. Try 
-0000df20: 746f 2063 616c 6c20 636f 6e6e 6563 7428  to call connect(
-0000df30: 2920 6669 7273 7427 290a 0a20 2020 2020  ) first')..     
-0000df40: 2020 2072 6574 7572 6e20 7365 6e73 6f72     return sensor
-0000df50: 2e67 6574 5f63 7572 7265 6e74 5661 6c75  .get_currentValu
-0000df60: 6528 290a 0a20 2020 2064 6566 2063 616c  e()..    def cal
-0000df70: 6962 7261 7469 6f6e 2873 656c 662c 2072  ibration(self, r
-0000df80: 6561 6c5f 7661 6c75 652c 2063 616c 6962  eal_value, calib
-0000df90: 5f62 6f6f 6c3d 5472 7565 293a 0a20 2020  _bool=True):.   
-0000dfa0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000dfb0: 2063 616c 6962 7261 7469 6f6e 2061 6e64   calibration and
-0000dfc0: 2063 616e 6365 6c20 6361 6c69 6272 6174   cancel calibrat
-0000dfd0: 696f 6e20 6675 6e63 7469 6f6e 2e0a 2020  ion function..  
-0000dfe0: 2020 2020 2020 4070 6172 616d 2063 616c        @param cal
-0000dff0: 6962 5f62 6f6f 6c3a 2069 6620 5472 7565  ib_bool: if True
-0000e000: 2043 616c 6962 7261 7469 6f6e 206f 7468   Calibration oth
-0000e010: 6572 7769 7365 2043 616e 6365 6c20 4361  erwise Cancel Ca
-0000e020: 6c69 6272 6174 696f 6e0a 2020 2020 2020  libration.      
-0000e030: 2020 4074 7970 6520 6361 6c69 625f 626f    @type calib_bo
-0000e040: 6f6c 3a20 626f 6f6c 0a20 2020 2020 2020  ol: bool.       
-0000e050: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-0000e060: 6361 6c69 625f 626f 6f6c 3a0a 2020 2020  calib_bool:.    
-0000e070: 2020 2020 2020 2020 7661 6c75 655f 6265          value_be
-0000e080: 666f 7265 203d 205b 7365 6c66 2e67 6574  fore = [self.get
-0000e090: 5f6c 6967 6874 2829 5d0a 2020 2020 2020  _light()].      
-0000e0a0: 2020 2020 2020 7661 6c75 655f 6166 7465        value_afte
-0000e0b0: 7220 3d20 5b72 6561 6c5f 7661 6c75 655d  r = [real_value]
-0000e0c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000e0d0: 2020 2020 2020 2020 2020 2076 616c 7565             value
-0000e0e0: 5f62 6566 6f72 6520 3d20 5b5d 0a20 2020  _before = [].   
-0000e0f0: 2020 2020 2020 2020 2076 616c 7565 5f61           value_a
-0000e100: 6674 6572 203d 205b 5d0a 2020 2020 2020  fter = [].      
-0000e110: 2020 6620 3d20 594c 6967 6874 5365 6e73    f = YLightSens
-0000e120: 6f72 2e46 6972 7374 4c69 6768 7453 656e  or.FirstLightSen
-0000e130: 736f 7228 290a 2020 2020 2020 2020 662e  sor().        f.
-0000e140: 6361 6c69 6272 6174 6546 726f 6d50 6f69  calibrateFromPoi
-0000e150: 6e74 7328 7661 6c75 655f 6265 666f 7265  nts(value_before
-0000e160: 2c20 7661 6c75 655f 6166 7465 7229 0a20  , value_after). 
-0000e170: 2020 2020 2020 2066 2e67 6574 5f6d 6f64         f.get_mod
-0000e180: 756c 6528 292e 7361 7665 546f 466c 6173  ule().saveToFlas
-0000e190: 6828 290a 0a20 2020 2040 7374 6174 6963  h()..    @static
-0000e1a0: 6d65 7468 6f64 0a20 2020 2064 6566 2065  method.    def e
-0000e1b0: 7869 745f 6170 7028 293a 0a20 2020 2020  xit_app():.     
-0000e1c0: 2020 2059 4150 492e 4672 6565 4150 4928     YAPI.FreeAPI(
-0000e1d0: 290a 0a0a 6966 205f 5f6e 616d 655f 5f20  )...if __name__ 
-0000e1e0: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0a20  == '__main__':. 
-0000e1f0: 2020 2070 7269 6e74 2827 636f 676e 6578     print('cognex
-0000e200: 2073 6572 6961 6c27 290a 2020 2020 6320   serial').    c 
-0000e210: 3d20 436f 676e 6578 4461 7461 4d61 6e28  = CognexDataMan(
-0000e220: 706f 7274 3d27 434f 4d34 272c 2062 6175  port='COM4', bau
-0000e230: 645f 7261 7465 3d31 3135 3230 3029 0a20  d_rate=115200). 
-0000e240: 2020 2073 6361 6e5f 7265 7375 6c74 7320     scan_results 
-0000e250: 3d20 632e 7363 616e 5f65 7874 5f69 6428  = c.scan_ext_id(
-0000e260: 290a 2020 2020 7072 696e 7428 6627 7369  ).    print(f'si
-0000e270: 6e67 6c65 2073 6361 6e3a 207b 7363 616e  ngle scan: {scan
-0000e280: 5f72 6573 756c 7473 7d27 290a 2020 2020  _results}').    
-0000e290: 632e 7472 6967 6765 725f 6f6e 2863 6f6e  c.trigger_on(con
-0000e2a0: 7469 6e75 6f75 736c 793d 5472 7565 290a  tinuously=True).
-0000e2b0: 2020 2020 736c 6565 7028 3529 0a20 2020      sleep(5).   
-0000e2c0: 2065 785f 6964 203d 2063 2e72 6561 645f   ex_id = c.read_
-0000e2d0: 6261 7463 6828 290a 2020 2020 7072 696e  batch().    prin
-0000e2e0: 7428 6627 636f 6e74 696e 6f75 7320 7363  t(f'continous sc
-0000e2f0: 616e 3a20 7b65 785f 6964 7d27 290a 2020  an: {ex_id}').  
-0000e300: 2020 632e 7472 6967 6765 725f 6f66 6628    c.trigger_off(
-0000e310: 290a 2020 2020 632e 636c 6f73 655f 706f  ).    c.close_po
-0000e320: 7274 2829 0a0a 2020 2020 7072 696e 7428  rt()..    print(
-0000e330: 2763 6f67 6e65 7820 6e65 7477 6f72 6b27  'cognex network'
-0000e340: 290a 2020 2020 6320 3d20 436f 676e 6578  ).    c = Cognex
-0000e350: 4e65 7477 6f72 6b28 6970 5f61 6464 7265  Network(ip_addre
-0000e360: 7373 3d27 3137 322e 3236 2e34 312e 3230  ss='172.26.41.20
-0000e370: 3327 290a 2020 2020 632e 7472 6967 6765  3').    c.trigge
-0000e380: 725f 6f6e 2863 6f6e 7469 6e75 6f75 736c  r_on(continuousl
-0000e390: 793d 5472 7565 290a 2020 2020 7072 696e  y=True).    prin
-0000e3a0: 7428 2777 6169 7420 3520 7365 636f 6e64  t('wait 5 second
-0000e3b0: 7320 746f 2072 6563 6569 7665 2064 6174  s to receive dat
-0000e3c0: 6127 290a 2020 2020 736c 6565 7028 3529  a').    sleep(5)
-0000e3d0: 0a20 2020 2065 785f 6964 203d 2063 2e72  .    ex_id = c.r
-0000e3e0: 6561 645f 6261 7463 6828 6e5f 6d73 673d  ead_batch(n_msg=
-0000e3f0: 3130 290a 2020 2020 7072 696e 7428 6578  10).    print(ex
-0000e400: 5f69 6429 0a20 2020 2063 2e74 7269 6767  _id).    c.trigg
-0000e410: 6572 5f6f 6666 2829 0a20 2020 2063 2e63  er_off().    c.c
-0000e420: 6c6f 7365 5f70 6f72 7428 290a 2020 2020  lose_port().    
-0000e430: 7072 696e 7428 2764 6f6e 6527 290a       print('done').
+00009630: 2020 2020 2020 2073 656c 662e 7172 5f6c         self.qr_l
+00009640: 6f67 6765 722e 696e 666f 2827 4e6f 2062  ogger.info('No b
+00009650: 6172 636f 6465 2064 6574 6563 7465 6420  arcode detected 
+00009660: 2d20 4465 636f 6469 6e67 2074 696d 656f  - Decoding timeo
+00009670: 7574 2072 6561 6368 6564 2729 0a20 2020  ut reached').   
+00009680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009690: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000096a0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
+000096b0: 2c20 4e6f 6e65 0a20 2020 2020 2020 2020  , None.         
+000096c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000096d0: 6c69 6620 6675 6c6c 5f64 6174 6120 3d3d  lif full_data ==
+000096e0: 2027 273a 0a20 2020 2020 2020 2020 2020   '':.           
+000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009700: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+00009710: 2827 5072 6f62 6c65 6d20 7769 7468 2062  ('Problem with b
+00009720: 6172 636f 6465 2073 6361 6e6e 6572 2729  arcode scanner')
+00009730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009740: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00009750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009760: 2020 2020 2020 2020 2020 2063 7572 5f69             cur_i
+00009770: 6420 3d20 6675 6c6c 5f64 6174 612e 7370  d = full_data.sp
+00009780: 6c69 7428 2754 2729 5b31 5d0a 2020 2020  lit('T')[1].    
+00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097a0: 2020 2020 2020 2020 7265 656c 5f69 6420          reel_id 
+000097b0: 3d20 6675 6c6c 5f64 6174 612e 7370 6c69  = full_data.spli
+000097c0: 7428 2754 2729 5b30 5d0a 2020 2020 2020  t('T')[0].      
+000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097e0: 2020 2020 2020 6774 696e 203d 2027 270a        gtin = ''.
+000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009800: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009810: 2e71 725f 6c6f 6767 6572 2e69 6e66 6f28  .qr_logger.info(
+00009820: 2757 696c 696f 7420 5152 2064 6574 6563  'Wiliot QR detec
+00009830: 7465 6420 5265 656c 3a20 7b7d 2c20 4944  ted Reel: {}, ID
+00009840: 3a7b 7d27 2e66 6f72 6d61 7428 6375 725f  :{}'.format(cur_
+00009850: 6964 2c20 7265 656c 5f69 6429 290a 0a20  id, reel_id)).. 
+00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009870: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00009880: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+00009890: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000098a0: 662e 7172 5f6c 6f67 6765 722e 696e 666f  f.qr_logger.info
+000098b0: 2827 4e6f 7420 5769 6c69 6f74 2062 6172  ('Not Wiliot bar
+000098c0: 636f 6465 2729 0a0a 2020 2020 2020 2020  code')..        
+000098d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000098e0: 726e 2066 756c 6c5f 6461 7461 2c20 6375  rn full_data, cu
+000098f0: 725f 6964 2c20 7265 656c 5f69 642c 2067  r_id, reel_id, g
+00009900: 7469 6e0a 0a20 2020 2020 2020 2065 7863  tin..        exc
+00009910: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00009920: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00009930: 7365 6c66 2e71 725f 6c6f 6767 6572 2e65  self.qr_logger.e
+00009940: 7272 6f72 2866 2245 7272 6f72 2064 7572  rror(f"Error dur
+00009950: 696e 6720 7265 6164 696e 6720 5769 6c69  ing reading Wili
+00009960: 6f74 2062 6172 636f 6465 3a20 7b65 7d22  ot barcode: {e}"
+00009970: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
+00009980: 6973 6520 4578 6365 7074 696f 6e0a 0a20  ise Exception.. 
+00009990: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+000099a0: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  ne, None, None, 
+000099b0: 4e6f 6e65 0a0a 2020 2020 6465 6620 6175  None..    def au
+000099c0: 746f 5f73 6361 6e28 7365 6c66 293a 0a20  to_scan(self):. 
+000099d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000099e0: 2020 2041 7574 6f6d 6174 6963 616c 6c79     Automatically
+000099f0: 2073 6361 6e20 7468 6520 5152 2063 6f64   scan the QR cod
+00009a00: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00009a10: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00009a20: 616c 5f63 6f6e 6e65 6374 696f 6e2e 7772  al_connection.wr
+00009a30: 6974 6528 6222 5c78 3162 5c78 3332 2229  ite(b"\x1b\x32")
+00009a40: 0a20 2020 2020 2020 2074 203d 2073 656c  .        t = sel
+00009a50: 662e 7365 7269 616c 5f63 6f6e 6e65 6374  f.serial_connect
+00009a60: 696f 6e2e 7265 6164 5f61 6c6c 2829 0a20  ion.read_all(). 
+00009a70: 2020 2020 2020 2073 656c 662e 7172 5f6c         self.qr_l
+00009a80: 6f67 6765 722e 696e 666f 2866 2761 7574  ogger.info(f'aut
+00009a90: 6f20 7363 616e 3a20 676f 7420 6d73 6720  o scan: got msg 
+00009aa0: 7b74 7d27 290a 2020 2020 2020 2020 7265  {t}').        re
+00009ab0: 7475 726e 2074 0a0a 2020 2020 6465 6620  turn t..    def 
+00009ac0: 7472 6967 6765 725f 7374 6f70 5f73 6574  trigger_stop_set
+00009ad0: 7469 6e67 7328 7365 6c66 293a 0a20 2020  tings(self):.   
+00009ae0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00009af0: 2054 7269 6767 6572 2073 746f 7020 7365   Trigger stop se
+00009b00: 7474 696e 6773 2e0a 2020 2020 2020 2020  ttings..        
+00009b10: 2222 220a 2020 2020 2020 2020 736c 6565  """.        slee
+00009b20: 7028 302e 3035 290a 2020 2020 2020 2020  p(0.05).        
+00009b30: 7420 3d20 7365 6c66 2e73 6572 6961 6c5f  t = self.serial_
+00009b40: 636f 6e6e 6563 7469 6f6e 2e72 6561 645f  connection.read_
+00009b50: 616c 6c28 290a 2020 2020 2020 2020 736c  all().        sl
+00009b60: 6565 7028 302e 3035 290a 2020 2020 2020  eep(0.05).      
+00009b70: 2020 6163 6b73 203d 2073 7472 2874 292e    acks = str(t).
+00009b80: 7370 6c69 7428 273b 2729 5b3a 2d31 5d0a  split(';')[:-1].
+00009b90: 2020 2020 2020 2020 6973 5375 6363 6573          isSucces
+00009ba0: 7320 3d20 616c 6c28 5b54 7275 6520 6966  s = all([True if
+00009bb0: 2061 636b 2e65 6e64 7377 6974 6828 275c   ack.endswith('\
+00009bc0: 5c78 3036 2729 2065 6c73 6520 4661 6c73  \x06') else Fals
+00009bd0: 6520 666f 7220 6163 6b20 696e 2061 636b  e for ack in ack
+00009be0: 735d 290a 2020 2020 2020 2020 7265 7475  s]).        retu
+00009bf0: 726e 2074 2c20 6973 5375 6363 6573 730a  rn t, isSuccess.
+00009c00: 0a20 2020 2064 6566 2074 7269 6767 6572  .    def trigger
+00009c10: 5f6f 6666 2873 656c 6629 3a0a 2020 2020  _off(self):.    
+00009c20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00009c30: 746f 206b 6565 7020 7361 6d65 2062 6568  to keep same beh
+00009c40: 6176 696f 7220 6173 2074 6865 2043 6f67  avior as the Cog
+00009c50: 6e65 780a 2020 2020 2020 2020 4072 6574  nex.        @ret
+00009c60: 7572 6e3a 0a20 2020 2020 2020 2040 7274  urn:.        @rt
+00009c70: 7970 653a 0a20 2020 2020 2020 2022 2222  ype:.        """
+00009c80: 0a20 2020 2020 2020 2070 6173 730a 0a0a  .        pass...
+00009c90: 636c 6173 7320 436f 676e 6578 4e65 7477  class CognexNetw
+00009ca0: 6f72 6b3a 0a20 2020 2042 4152 434f 4445  ork:.    BARCODE
+00009cb0: 5f4c 454e 203d 2031 380a 2020 2020 4445  _LEN = 18.    DE
+00009cc0: 5649 4345 5f4e 414d 4520 3d20 2742 6172  VICE_NAME = 'Bar
+00009cd0: 436f 6465 5265 6164 6572 270a 0a20 2020  CodeReader'..   
+00009ce0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00009cf0: 6c66 2c20 6970 5f61 6464 7265 7373 2c20  lf, ip_address, 
+00009d00: 706f 7274 3d32 3329 3a0a 0a20 2020 2020  port=23):..     
+00009d10: 2020 2073 656c 662e 636f 6e6e 6563 7465     self.connecte
+00009d20: 6420 3d20 4661 6c73 650a 2020 2020 2020  d = False.      
+00009d30: 2020 7365 6c66 2e74 6e20 3d20 4e6f 6e65    self.tn = None
+00009d40: 0a20 2020 2020 2020 2073 656c 662e 686f  .        self.ho
+00009d50: 7374 203d 2073 7472 2869 705f 6164 6472  st = str(ip_addr
+00009d60: 6573 7329 0a20 2020 2020 2020 2073 656c  ess).        sel
+00009d70: 662e 706f 7274 203d 2070 6f72 740a 2020  f.port = port.  
+00009d80: 2020 2020 2020 7365 6c66 2e64 6576 6963        self.devic
+00009d90: 655f 6e61 6d65 203d 2027 270a 0a20 2020  e_name = ''..   
+00009da0: 2020 2020 2073 656c 662e 6f70 656e 5f70       self.open_p
+00009db0: 6f72 7428 290a 0a20 2020 2064 6566 206f  ort()..    def o
+00009dc0: 7065 6e5f 706f 7274 2873 656c 662c 2063  pen_port(self, c
+00009dd0: 6f6d 5f70 6f72 743d 4e6f 6e65 2c20 6261  om_port=None, ba
+00009de0: 7564 5f72 6174 653d 3131 3532 3030 2c20  ud_rate=115200, 
+00009df0: 7469 6d65 6f75 743d 3530 302c 2063 6f6e  timeout=500, con
+00009e00: 6669 673d 4661 6c73 6529 3a0a 2020 2020  fig=False):.    
+00009e10: 2020 2020 7365 6c66 2e63 6f6e 6e65 6374      self.connect
+00009e20: 6564 203d 2046 616c 7365 0a20 2020 2020  ed = False.     
+00009e30: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00009e40: 2020 2020 7365 6c66 2e74 6e20 3d20 7465      self.tn = te
+00009e50: 6c6e 6574 6c69 622e 5465 6c6e 6574 2868  lnetlib.Telnet(h
+00009e60: 6f73 743d 7365 6c66 2e68 6f73 742c 2070  ost=self.host, p
+00009e70: 6f72 743d 7365 6c66 2e70 6f72 742c 2074  ort=self.port, t
+00009e80: 696d 656f 7574 3d31 290a 2020 2020 2020  imeout=1).      
+00009e90: 2020 2020 2020 736c 6565 7028 3129 0a20        sleep(1). 
+00009ea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009eb0: 746e 2e77 7269 7465 2862 277c 7c30 3a31  tn.write(b'||0:1
+00009ec0: 3233 3e47 4554 2044 4556 4943 452e 4e41  23>GET DEVICE.NA
+00009ed0: 4d45 5c72 5c6e 2729 0a20 2020 2020 2020  ME\r\n').       
+00009ee0: 2020 2020 2072 7370 203d 2073 656c 662e       rsp = self.
+00009ef0: 7265 6164 5f72 6573 706f 6e73 6528 290a  read_response().
+00009f00: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00009f10: 656c 662e 4445 5649 4345 5f4e 414d 4520  elf.DEVICE_NAME 
+00009f20: 696e 2072 7370 3a0a 2020 2020 2020 2020  in rsp:.        
+00009f30: 2020 2020 2020 2020 7365 6c66 2e64 6576          self.dev
+00009f40: 6963 655f 6e61 6d65 203d 2072 7370 0a20  ice_name = rsp. 
+00009f50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009f60: 636f 6e6e 6563 7465 6420 3d20 5472 7565  connected = True
+00009f70: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00009f80: 6e74 2866 2743 6f6e 6e65 6374 6564 2074  nt(f'Connected t
+00009f90: 6f20 7b73 656c 662e 6465 7669 6365 5f6e  o {self.device_n
+00009fa0: 616d 657d 2729 0a20 2020 2020 2020 2065  ame}').        e
+00009fb0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00009fc0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00009fd0: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+00009fe0: 6e28 6622 4661 696c 6564 2074 6f20 636f  n(f"Failed to co
+00009ff0: 6e6e 6563 7420 746f 2054 656e 6574 2073  nnect to Tenet s
+0000a000: 6f63 6b65 743a 207b 657d 2229 0a0a 2020  ocket: {e}")..  
+0000a010: 2020 6465 6620 7265 6164 5f72 6573 706f    def read_respo
+0000a020: 6e73 6528 7365 6c66 293a 0a20 2020 2020  nse(self):.     
+0000a030: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000a040: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+0000a050: 656c 662e 746e 2e72 6561 645f 756e 7469  elf.tn.read_unti
+0000a060: 6c28 6227 5c6e 272c 2074 696d 656f 7574  l(b'\n', timeout
+0000a070: 3d31 290a 2020 2020 2020 2020 2020 2020  =1).            
+0000a080: 6966 2072 6573 706f 6e73 653a 0a20 2020  if response:.   
+0000a090: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0000a0a0: 706f 6e73 6520 3d20 7265 7370 6f6e 7365  ponse = response
+0000a0b0: 2e64 6563 6f64 6528 290a 2020 2020 2020  .decode().      
+0000a0c0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+0000a0d0: 7365 203d 2072 6573 706f 6e73 652e 7374  se = response.st
+0000a0e0: 7269 7028 275c 725c 6e27 290a 2020 2020  rip('\r\n').    
+0000a0f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a100: 726e 2072 6573 706f 6e73 650a 2020 2020  rn response.    
+0000a110: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+0000a120: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+0000a130: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
+0000a140: 6570 7469 6f6e 2866 2246 6169 6c65 6420  eption(f"Failed 
+0000a150: 746f 2072 6561 6420 7265 7370 6f6e 7365  to read response
+0000a160: 3a20 7b65 7d22 290a 2020 2020 2020 2020  : {e}").        
+0000a170: 7265 7475 726e 2027 270a 0a20 2020 2064  return ''..    d
+0000a180: 6566 2072 6561 645f 6261 7463 6828 7365  ef read_batch(se
+0000a190: 6c66 2c20 6e5f 6d73 673d 3130 3030 293a  lf, n_msg=1000):
+0000a1a0: 0a20 2020 2020 2020 2072 7370 5f6f 7574  .        rsp_out
+0000a1b0: 203d 205b 5d0a 2020 2020 2020 2020 7273   = [].        rs
+0000a1c0: 7020 3d20 7365 6c66 2e72 6561 645f 7265  p = self.read_re
+0000a1d0: 7370 6f6e 7365 2829 0a20 2020 2020 2020  sponse().       
+0000a1e0: 206d 7367 5f63 6f75 6e74 6572 203d 2030   msg_counter = 0
+0000a1f0: 0a20 2020 2020 2020 2077 6869 6c65 206c  .        while l
+0000a200: 656e 2872 7370 5f6f 7574 2920 3c20 6e5f  en(rsp_out) < n_
+0000a210: 6d73 6720 616e 6420 7273 7020 213d 2027  msg and rsp != '
+0000a220: 2720 616e 6420 6d73 675f 636f 756e 7465  ' and msg_counte
+0000a230: 7220 3c20 6e5f 6d73 673a 0a20 2020 2020  r < n_msg:.     
+0000a240: 2020 2020 2020 2077 6869 6c65 206c 656e         while len
+0000a250: 2872 7370 2920 3e3d 2073 656c 662e 4241  (rsp) >= self.BA
+0000a260: 5243 4f44 455f 4c45 4e3a 0a20 2020 2020  RCODE_LEN:.     
+0000a270: 2020 2020 2020 2020 2020 2072 7370 5f6f             rsp_o
+0000a280: 7574 2e61 7070 656e 6428 7273 705b 3a73  ut.append(rsp[:s
+0000a290: 656c 662e 4241 5243 4f44 455f 4c45 4e5d  elf.BARCODE_LEN]
+0000a2a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a2b0: 2020 7273 7020 3d20 7273 705b 7365 6c66    rsp = rsp[self
+0000a2c0: 2e42 4152 434f 4445 5f4c 454e 3a5d 0a20  .BARCODE_LEN:]. 
+0000a2d0: 2020 2020 2020 2020 2020 2072 7370 203d             rsp =
+0000a2e0: 2073 656c 662e 7265 6164 5f72 6573 706f   self.read_respo
+0000a2f0: 6e73 6528 290a 2020 2020 2020 2020 2020  nse().          
+0000a300: 2020 6d73 675f 636f 756e 7465 7220 2b3d    msg_counter +=
+0000a310: 2031 0a0a 2020 2020 2020 2020 7265 7475   1..        retu
+0000a320: 726e 206c 6973 7428 7365 7428 7273 705f  rn list(set(rsp_
+0000a330: 6f75 7429 290a 0a20 2020 2064 6566 2074  out))..    def t
+0000a340: 7269 6767 6572 5f6f 6e28 7365 6c66 2c20  rigger_on(self, 
+0000a350: 636f 6e74 696e 756f 7573 6c79 3d54 7275  continuously=Tru
+0000a360: 652c 2074 7269 6767 6572 5f74 7970 653d  e, trigger_type=
+0000a370: 3429 3a0a 2020 2020 2020 2020 2222 220a  4):.        """.
+0000a380: 0a20 2020 2020 2020 2040 7061 7261 6d20  .        @param 
+0000a390: 7472 6967 6765 725f 7479 7065 3a20 303a  trigger_type: 0:
+0000a3a0: 2053 696e 676c 6520 2865 7874 6572 6e61   Single (externa
+0000a3b0: 6c29 2c20 313a 2050 7265 7365 6e74 6174  l), 1: Presentat
+0000a3c0: 696f 6e20 2869 6e74 6572 6e61 6c29 2c20  ion (internal), 
+0000a3d0: 323a 204d 616e 7561 6c20 2862 7574 746f  2: Manual (butto
+0000a3e0: 6e29 2c20 333a 2042 7572 7374 2028 6578  n), 3: Burst (ex
+0000a3f0: 7465 726e 616c 292c 0a20 2020 2020 2020  ternal),.       
+0000a400: 2020 2020 2020 2020 2020 2020 2020 343a                4:
+0000a410: 2053 656c 6620 2869 6e74 6572 6e61 6c29   Self (internal)
+0000a420: 2c20 353a 2043 6f6e 7469 6e75 6f75 7320  , 5: Continuous 
+0000a430: 2865 7874 6572 6e61 6c29 0a20 2020 2020  (external).     
+0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a450: 2a20 5369 6e67 6c65 3a20 4163 7175 6972  * Single: Acquir
+0000a460: 6573 2061 2073 696e 676c 6520 696d 6167  es a single imag
+0000a470: 6520 616e 6420 6174 7465 6d70 7473 2074  e and attempts t
+0000a480: 6f20 6465 636f 6465 2061 6e79 2073 796d  o decode any sym
+0000a490: 626f 6c20 6974 2063 6f6e 7461 696e 7320  bol it contains 
+0000a4a0: 6f72 206d 6f72 6520 7468 616e 206f 6e65  or more than one
+0000a4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a4c0: 2020 2020 2020 7379 6d62 6f6c 2069 6e20        symbol in 
+0000a4d0: 6361 7365 7320 7768 6572 6520 6d75 6c74  cases where mult
+0000a4e0: 6963 6f64 6520 6973 2065 6e61 626c 6564  icode is enabled
+0000a4f0: 2e20 5468 6520 7265 6164 6572 2072 656c  . The reader rel
+0000a500: 6965 7320 6f6e 2061 6e20 6578 7465 726e  ies on an extern
+0000a510: 616c 2074 7269 6767 6572 2073 6f75 7263  al trigger sourc
+0000a520: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000a530: 2020 2020 2020 2020 2a20 5072 6573 656e          * Presen
+0000a540: 7461 7469 6f6e 3a20 5265 7065 6174 6564  tation: Repeated
+0000a550: 6c79 2073 6361 6e73 2066 6f72 2061 2073  ly scans for a s
+0000a560: 796d 626f 6c20 616e 6420 6465 636f 6465  ymbol and decode
+0000a570: 7320 6974 2077 6865 6e65 7665 7220 6f6e  s it whenever on
+0000a580: 6520 6973 2064 6574 6563 7465 642e 0a20  e is detected.. 
+0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5a0: 2020 2020 5468 6520 7265 6164 6572 2072      The reader r
+0000a5b0: 656c 6965 7320 6f6e 2061 6e20 696e 7465  elies on an inte
+0000a5c0: 726e 616c 2074 696d 696e 6720 6d65 6368  rnal timing mech
+0000a5d0: 616e 6973 6d20 746f 2061 6371 7569 7265  anism to acquire
+0000a5e0: 2069 6d61 6765 732e 0a20 2020 2020 2020   images..       
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+0000a600: 4275 7273 743a 2050 6572 666f 726d 7320  Burst: Performs 
+0000a610: 6d75 6c74 6970 6c65 2069 6d61 6765 2061  multiple image a
+0000a620: 6371 7569 7369 7469 6f6e 7320 6261 7365  cquisitions base
+0000a630: 6420 6f6e 2061 6e20 6578 7465 726e 616c  d on an external
+0000a640: 2074 7269 6767 6572 2061 6e64 2064 6563   trigger and dec
+0000a650: 6f64 6573 206f 6e65 206f 720a 2020 2020  odes one or.    
+0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a670: 206d 756c 7469 706c 6520 7379 6d62 6f6c   multiple symbol
+0000a680: 7320 6170 7065 6172 696e 6720 696e 2074  s appearing in t
+0000a690: 6865 2073 6571 7565 6e63 6520 6f66 2069  he sequence of i
+0000a6a0: 6d61 6765 732e 0a20 2020 2020 2020 2020  mages..         
+0000a6b0: 2020 2020 2020 2020 2020 2020 2a20 5365              * Se
+0000a6c0: 6c66 3a20 5369 6d69 6c61 7220 746f 2050  lf: Similar to P
+0000a6d0: 7265 7365 6e74 6174 696f 6e20 6d6f 6465  resentation mode
+0000a6e0: 2069 6e20 7468 6174 2074 6865 2072 6561   in that the rea
+0000a6f0: 6465 7220 7065 7270 6574 7561 6c6c 7920  der perpetually 
+0000a700: 7363 616e 7320 666f 7220 7379 6d62 6f6c  scans for symbol
+0000a710: 7320 616e 6420 6465 636f 6465 730a 2020  s and decodes.  
+0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a730: 2020 2074 6865 6d20 6561 6368 2074 696d     them each tim
+0000a740: 6520 6f6e 6520 6973 2064 6574 6563 7465  e one is detecte
+0000a750: 642e 2055 6e6c 696b 6520 5072 6573 656e  d. Unlike Presen
+0000a760: 7461 7469 6f6e 206d 6f64 652c 2068 6f77  tation mode, how
+0000a770: 6576 6572 2c20 5365 6c66 206d 6f64 6520  ever, Self mode 
+0000a780: 7375 7070 6f72 7473 206d 756c 7469 636f  supports multico
+0000a790: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
+0000a7a0: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
+0000a7b0: 616e 6420 6120 6465 636f 6465 2061 7474  and a decode att
+0000a7c0: 656d 7074 206f 6363 7572 7320 7769 7468  empt occurs with
+0000a7d0: 2065 7665 7279 2069 6d61 6765 2e20 5468   every image. Th
+0000a7e0: 6520 6d61 696e 2064 6966 6665 7265 6e63  e main differenc
+0000a7f0: 6520 6265 7477 6565 6e20 5365 6c66 2061  e between Self a
+0000a800: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+0000a810: 2020 2020 2020 2020 5072 6573 656e 7461          Presenta
+0000a820: 7469 6f6e 2069 7320 7468 6520 6669 7865  tion is the fixe
+0000a830: 6420 616e 6420 6578 6163 7420 696e 7465  d and exact inte
+0000a840: 7276 616c 2066 6f72 2069 6d61 6765 2061  rval for image a
+0000a850: 6371 7569 7369 7469 6f6e 7320 696e 2053  cquisitions in S
+0000a860: 656c 662e 0a20 2020 2020 2020 2020 2020  elf..           
+0000a870: 2020 2020 2020 2020 2020 2a20 436f 6e74            * Cont
+0000a880: 696e 756f 7573 3a20 4265 6769 6e73 2061  inuous: Begins a
+0000a890: 6371 7569 7269 6e67 2069 6d61 6765 7320  cquiring images 
+0000a8a0: 6261 7365 6420 6f6e 2061 2073 696e 676c  based on a singl
+0000a8b0: 6520 6578 7465 726e 616c 2074 7269 6767  e external trigg
+0000a8c0: 6572 2061 6e64 2063 6f6e 7469 6e75 6573  er and continues
+0000a8d0: 2074 6f20 6163 7175 6972 650a 2020 2020   to acquire.    
+0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8f0: 2069 6d61 6765 7320 756e 7469 6c20 6120   images until a 
+0000a900: 7379 6d62 6f6c 2069 7320 666f 756e 6420  symbol is found 
+0000a910: 616e 6420 6465 636f 6465 642c 206f 7220  and decoded, or 
+0000a920: 756e 7469 6c20 6d75 6c74 6970 6c65 2069  until multiple i
+0000a930: 6d61 6765 7320 636f 6e74 6169 6e69 6e67  mages containing
+0000a940: 2061 7320 6d61 6e79 2063 6f64 6573 2061   as many codes a
+0000a950: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000a960: 2020 2020 2020 2073 7065 6369 6669 6564         specified
+0000a970: 2069 6e20 6d75 6c74 6963 6f64 6520 6d6f   in multicode mo
+0000a980: 6465 2061 7265 206c 6f63 6174 6564 2c20  de are located, 
+0000a990: 6f72 2075 6e74 696c 2074 6865 2074 7269  or until the tri
+0000a9a0: 6767 6572 2069 7320 7265 6c65 6173 6564  gger is released
+0000a9b0: 2e0a 2020 2020 2020 2020 4074 7970 6520  ..        @type 
+0000a9c0: 7472 6967 6765 725f 7479 7065 3a20 696e  trigger_type: in
+0000a9d0: 740a 2020 2020 2020 2020 4072 6574 7572  t.        @retur
+0000a9e0: 6e3a 0a20 2020 2020 2020 2040 7274 7970  n:.        @rtyp
+0000a9f0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+0000aa00: 2020 2020 2020 2069 6620 636f 6e74 696e         if contin
+0000aa10: 756f 7573 6c79 3a0a 2020 2020 2020 2020  uously:.        
+0000aa20: 2020 2020 636f 6d6d 616e 6420 3d20 6627      command = f'
+0000aa30: 7c7c 303a 3132 333e 5345 5420 5452 4947  ||0:123>SET TRIG
+0000aa40: 4745 522e 5459 5045 207b 7472 6967 6765  GER.TYPE {trigge
+0000aa50: 725f 7479 7065 7d5c 725c 6e27 0a20 2020  r_type}\r\n'.   
+0000aa60: 2020 2020 2020 2020 2073 656c 662e 746e           self.tn
+0000aa70: 2e77 7269 7465 2863 6f6d 6d61 6e64 2e65  .write(command.e
+0000aa80: 6e63 6f64 6528 2929 0a0a 2020 2020 6465  ncode())..    de
+0000aa90: 6620 7472 6967 6765 725f 6f66 6628 7365  f trigger_off(se
+0000aaa0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+0000aab0: 662e 746e 2e77 7269 7465 2862 277c 7c30  f.tn.write(b'||0
+0000aac0: 3a31 3233 3e53 4554 2054 5249 4747 4552  :123>SET TRIGGER
+0000aad0: 2e54 5950 4520 305c 725c 6e27 290a 2020  .TYPE 0\r\n').  
+0000aae0: 2020 2020 2020 736c 6565 7028 3129 0a20        sleep(1). 
+0000aaf0: 2020 2020 2020 2023 2054 4f44 4f20 6d61         # TODO ma
+0000ab00: 7962 6520 636c 6561 6e20 616c 6c20 6d73  ybe clean all ms
+0000ab10: 6773 0a0a 2020 2020 6465 6620 636c 6f73  gs..    def clos
+0000ab20: 655f 706f 7274 2873 656c 6629 3a0a 2020  e_port(self):.  
+0000ab30: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000ab40: 2020 2020 2020 2073 656c 662e 746e 2e63         self.tn.c
+0000ab50: 6c6f 7365 2829 0a20 2020 2020 2020 2065  lose().        e
+0000ab60: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0000ab70: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+0000ab80: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+0000ab90: 6e28 6622 4661 696c 6564 2074 6f20 636c  n(f"Failed to cl
+0000aba0: 6f73 6520 5465 6e65 7420 636f 6d6d 756e  ose Tenet commun
+0000abb0: 6963 6174 696f 6e3a 207b 657d 2229 0a0a  ication: {e}")..
+0000abc0: 0a63 6c61 7373 2043 6f67 6e65 7844 6174  .class CognexDat
+0000abd0: 614d 616e 3a0a 2020 2020 434f 4e54 494e  aMan:.    CONTIN
+0000abe0: 554f 5553 5f54 5249 4747 4552 5f54 5950  UOUS_TRIGGER_TYP
+0000abf0: 4520 3d20 340a 2020 2020 5347 5449 4e5f  E = 4.    SGTIN_
+0000ac00: 5354 5249 505f 4c45 4e20 3d20 3237 0a20  STRIP_LEN = 27. 
+0000ac10: 2020 2053 4754 494e 5f4c 454e 203d 2033     SGTIN_LEN = 3
+0000ac20: 310a 2020 2020 5245 454c 5f49 445f 4c45  1.    REEL_ID_LE
+0000ac30: 4e20 3d20 340a 2020 2020 4d49 4e5f 5449  N = 4.    MIN_TI
+0000ac40: 4d45 5f54 4f5f 5245 4144 203d 2030 2e32  ME_TO_READ = 0.2
+0000ac50: 3030 0a0a 2020 2020 6465 6620 5f5f 696e  00..    def __in
+0000ac60: 6974 5f5f 2873 656c 662c 2070 6f72 743d  it__(self, port=
+0000ac70: 4e6f 6e65 2c20 6261 7564 5f72 6174 653d  None, baud_rate=
+0000ac80: 3131 3532 3030 2c20 7469 6d65 6f75 743d  115200, timeout=
+0000ac90: 3530 302c 206c 6f67 5f6e 616d 653d 4e6f  500, log_name=No
+0000aca0: 6e65 2c20 6465 6661 756c 745f 636f 6e66  ne, default_conf
+0000acb0: 6967 3d4e 6f6e 6529 3a0a 2020 2020 2020  ig=None):.      
+0000acc0: 2020 2222 220a 2020 2020 2020 2020 6874    """.        ht
+0000acd0: 7470 733a 2f2f 7375 7070 6f72 742e 636f  tps://support.co
+0000ace0: 676e 6578 2e63 6f6d 2f64 6f63 732f 646d  gnex.com/docs/dm
+0000acf0: 7374 5f32 3332 322f 7765 622f 454e 2f44  st_2322/web/EN/D
+0000ad00: 4d43 432f 436f 6e74 656e 742f 546f 7069  MCC/Content/Topi
+0000ad10: 6373 2f64 6d63 632d 6d61 696e 2e68 746d  cs/dmcc-main.htm
+0000ad20: 6c0a 2020 2020 2020 2020 746f 2064 6f77  l.        to dow
+0000ad30: 6e6c 6f61 6420 434f 474e 4558 2047 5549  nload COGNEX GUI
+0000ad40: 3a20 6874 7470 733a 2f2f 7375 7070 6f72  : https://suppor
+0000ad50: 742e 636f 676e 6578 2e63 6f6d 2f65 6e2f  t.cognex.com/en/
+0000ad60: 646f 776e 6c6f 6164 732f 6465 7461 696c  downloads/detail
+0000ad70: 2f64 6174 616d 616e 2f34 3531 322f 3130  /dataman/4512/10
+0000ad80: 3333 0a20 2020 2020 2020 2040 7061 7261  33.        @para
+0000ad90: 6d20 706f 7274 3a0a 2020 2020 2020 2020  m port:.        
+0000ada0: 4074 7970 6520 706f 7274 3a0a 2020 2020  @type port:.    
+0000adb0: 2020 2020 4070 6172 616d 2062 6175 645f      @param baud_
+0000adc0: 7261 7465 3a0a 2020 2020 2020 2020 4074  rate:.        @t
+0000add0: 7970 6520 6261 7564 5f72 6174 653a 0a20  ype baud_rate:. 
+0000ade0: 2020 2020 2020 2040 7061 7261 6d20 6465         @param de
+0000adf0: 6661 756c 745f 636f 6e66 6967 3a20 6469  fault_config: di
+0000ae00: 6374 696f 6e61 7279 2077 6865 7265 2074  ctionary where t
+0000ae10: 6865 2063 6f6d 6d61 6e64 2069 7320 7468  he command is th
+0000ae20: 6520 6b65 7420 616e 6420 7468 6520 636f  e ket and the co
+0000ae30: 6d6d 616e 6420 7661 6c75 6520 6973 2074  mmand value is t
+0000ae40: 6865 2076 616c 7565 2c0a 2020 2020 2020  he value,.      
+0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae60: 2020 2020 2020 2020 2065 2e67 2e20 7b27           e.g. {'
+0000ae70: 5452 4947 4745 522e 5459 5045 273a 2027  TRIGGER.TYPE': '
+0000ae80: 3027 2c20 2753 594d 424f 4c2e 5152 273a  0', 'SYMBOL.QR':
+0000ae90: 2027 4f4e 277d 0a20 2020 2020 2020 2040   'ON'}.        @
+0000aea0: 7479 7065 2064 6566 6175 6c74 5f63 6f6e  type default_con
+0000aeb0: 6669 673a 2064 6963 740a 2020 2020 2020  fig: dict.      
+0000aec0: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+0000aed0: 6c66 2e64 6576 6963 655f 6e61 6d65 203d  lf.device_name =
+0000aee0: 2027 270a 2020 2020 2020 2020 7365 6c66   ''.        self
+0000aef0: 2e63 6f6d 5f70 6f72 7420 3d20 2727 0a20  .com_port = ''. 
+0000af00: 2020 2020 2020 2073 656c 662e 6261 7564         self.baud
+0000af10: 5f72 6174 6520 3d20 300a 2020 2020 2020  _rate = 0.      
+0000af20: 2020 7365 6c66 2e64 6566 6175 6c74 5f63    self.default_c
+0000af30: 6f6e 6669 6720 3d20 6465 6661 756c 745f  onfig = default_
+0000af40: 636f 6e66 6967 0a20 2020 2020 2020 2073  config.        s
+0000af50: 656c 662e 7365 7220 3d20 4e6f 6e65 0a20  elf.ser = None. 
+0000af60: 2020 2020 2020 2073 656c 662e 636f 6e6e         self.conn
+0000af70: 6563 7465 6420 3d20 4661 6c73 650a 2020  ected = False.  
+0000af80: 2020 2020 2020 6966 206c 6f67 5f6e 616d        if log_nam
+0000af90: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+0000afa0: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
+0000afb0: 6572 203d 206c 6f67 6769 6e67 2e67 6574  er = logging.get
+0000afc0: 4c6f 6767 6572 2827 436f 676e 6578 5363  Logger('CognexSc
+0000afd0: 616e 6e65 724c 6f67 6765 7227 290a 2020  annerLogger').  
+0000afe0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000aff0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+0000b000: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
+0000b010: 744c 6f67 6765 7228 6c6f 675f 6e61 6d65  tLogger(log_name
+0000b020: 290a 0a20 2020 2020 2020 2069 6620 706f  )..        if po
+0000b030: 7274 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rt is not None:.
+0000b040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b050: 2e63 6f6e 6e65 6374 6564 203d 2073 656c  .connected = sel
+0000b060: 662e 6f70 656e 5f70 6f72 7428 636f 6d5f  f.open_port(com_
+0000b070: 706f 7274 3d70 6f72 742c 2062 6175 645f  port=port, baud_
+0000b080: 7261 7465 3d62 6175 645f 7261 7465 2c20  rate=baud_rate, 
+0000b090: 7469 6d65 6f75 743d 7469 6d65 6f75 7429  timeout=timeout)
+0000b0a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000b0b0: 2020 2020 2020 2020 2020 2061 6c6c 5f70             all_p
+0000b0c0: 6f72 7473 203d 2073 6572 6961 6c5f 706f  orts = serial_po
+0000b0d0: 7274 7328 290a 2020 2020 2020 2020 2020  rts().          
+0000b0e0: 2020 666f 7220 706f 7274 2069 6e20 616c    for port in al
+0000b0f0: 6c5f 706f 7274 733a 0a20 2020 2020 2020  l_ports:.       
+0000b100: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b120: 2020 636f 6e6e 6563 7465 6420 3d20 7365    connected = se
+0000b130: 6c66 2e6f 7065 6e5f 706f 7274 2863 6f6d  lf.open_port(com
+0000b140: 5f70 6f72 743d 706f 7274 2c20 6261 7564  _port=port, baud
+0000b150: 5f72 6174 653d 6261 7564 5f72 6174 652c  _rate=baud_rate,
+0000b160: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+0000b170: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000b180: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+0000b190: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+0000b1a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b1b0: 662e 6c6f 6767 6572 2e77 6172 6e69 6e67  f.logger.warning
+0000b1c0: 2866 2743 6f75 6c64 206e 6f74 2063 6f6e  (f'Could not con
+0000b1d0: 6e65 6374 2074 6f20 706f 7274 207b 706f  nect to port {po
+0000b1e0: 7274 7d20 6475 6520 746f 207b 657d 2729  rt} due to {e}')
+0000b1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b200: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+0000b210: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000b220: 2063 6f6e 6e65 6374 6564 3a0a 2020 2020   connected:.    
+0000b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b240: 7365 6c66 2e63 6f6e 6e65 6374 6564 203d  self.connected =
+0000b250: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+0000b260: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+0000b270: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000b280: 2e63 6f6e 6e65 6374 6564 3a0a 2020 2020  .connected:.    
+0000b290: 2020 2020 2020 2020 7365 6c66 2e69 6e69          self.ini
+0000b2a0: 745f 636f 6e66 6967 7572 6174 696f 6e73  t_configurations
+0000b2b0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+0000b2c0: 656c 662e 636f 6d5f 706f 7274 203d 2070  elf.com_port = p
+0000b2d0: 6f72 740a 2020 2020 2020 2020 2020 2020  ort.            
+0000b2e0: 7365 6c66 2e62 6175 645f 7261 7465 203d  self.baud_rate =
+0000b2f0: 2062 6175 645f 7261 7465 0a0a 2020 2020   baud_rate..    
+0000b300: 6465 6620 6f70 656e 5f70 6f72 7428 7365  def open_port(se
+0000b310: 6c66 2c20 636f 6d5f 706f 7274 2c20 6261  lf, com_port, ba
+0000b320: 7564 5f72 6174 653d 3131 3532 3030 2c20  ud_rate=115200, 
+0000b330: 7469 6d65 6f75 743d 3530 302c 2063 6f6e  timeout=500, con
+0000b340: 6669 673d 4661 6c73 6529 3a0a 2020 2020  fig=False):.    
+0000b350: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000b360: 2040 7061 7261 6d20 636f 6d5f 706f 7274   @param com_port
+0000b370: 3a0a 2020 2020 2020 2020 4074 7970 6520  :.        @type 
+0000b380: 636f 6d5f 706f 7274 3a0a 2020 2020 2020  com_port:.      
+0000b390: 2020 4070 6172 616d 2062 6175 645f 7261    @param baud_ra
+0000b3a0: 7465 3a0a 2020 2020 2020 2020 4074 7970  te:.        @typ
+0000b3b0: 6520 6261 7564 5f72 6174 653a 0a20 2020  e baud_rate:.   
+0000b3c0: 2020 2020 2040 7061 7261 6d20 7469 6d65       @param time
+0000b3d0: 6f75 743a 2074 696d 656f 7574 2069 6e20  out: timeout in 
+0000b3e0: 6d73 6563 0a20 2020 2020 2020 2040 7479  msec.        @ty
+0000b3f0: 7065 2074 696d 656f 7574 3a20 696e 7420  pe timeout: int 
+0000b400: 6f72 2073 7472 0a20 2020 2020 2020 2040  or str.        @
+0000b410: 7061 7261 6d20 636f 6e66 6967 3a20 7469  param config: ti
+0000b420: 6d65 6f75 7420 696e 206d 7365 630a 2020  meout in msec.  
+0000b430: 2020 2020 2020 4074 7970 6520 636f 6e66        @type conf
+0000b440: 6967 3a20 696e 7420 6f72 2073 7472 0a20  ig: int or str. 
+0000b450: 2020 2020 2020 2040 7265 7475 726e 3a0a         @return:.
+0000b460: 2020 2020 2020 2020 4072 7479 7065 3a0a          @rtype:.
+0000b470: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b480: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000b490: 2020 2020 2073 656c 662e 7365 7220 3d20       self.ser = 
+0000b4a0: 7365 7269 616c 2e53 6572 6961 6c28 636f  serial.Serial(co
+0000b4b0: 6d5f 706f 7274 2c20 6261 7564 5f72 6174  m_port, baud_rat
+0000b4c0: 652c 2074 696d 656f 7574 3d69 6e74 2874  e, timeout=int(t
+0000b4d0: 696d 656f 7574 292f 3130 3030 290a 2020  imeout)/1000).  
+0000b4e0: 2020 2020 2020 2020 2020 736c 6565 7028            sleep(
+0000b4f0: 3129 0a20 2020 2020 2020 2020 2020 2063  1).            c
+0000b500: 6f6e 6e65 6374 6564 203d 2073 656c 662e  onnected = self.
+0000b510: 6973 5f6f 7065 6e28 290a 2020 2020 2020  is_open().      
+0000b520: 2020 2020 2020 6966 2063 6f6e 6e65 6374        if connect
+0000b530: 6564 2061 6e64 2063 6f6e 6669 673a 0a20  ed and config:. 
+0000b540: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b550: 656c 662e 696e 6974 5f63 6f6e 6669 6775  elf.init_configu
+0000b560: 7261 7469 6f6e 7328 290a 2020 2020 2020  rations().      
+0000b570: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
+0000b580: 6e65 6374 6564 0a20 2020 2020 2020 2065  nected.        e
+0000b590: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0000b5a0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+0000b5b0: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+0000b5c0: 6e28 6622 4661 696c 6564 2074 6f20 6f70  n(f"Failed to op
+0000b5d0: 656e 2073 6572 6961 6c20 706f 7274 3a20  en serial port: 
+0000b5e0: 7b65 7d22 290a 0a20 2020 2064 6566 2069  {e}")..    def i
+0000b5f0: 735f 6f70 656e 2873 656c 6629 3a0a 2020  s_open(self):.  
+0000b600: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000b610: 2020 2020 2020 2064 6576 5f6e 616d 6520         dev_name 
+0000b620: 3d20 7365 6c66 2e67 6574 5f64 6576 6963  = self.get_devic
+0000b630: 655f 7072 6f70 6572 7479 2827 4445 5649  e_property('DEVI
+0000b640: 4345 2e4e 414d 4527 290a 2020 2020 2020  CE.NAME').      
+0000b650: 2020 2020 2020 6966 2064 6576 5f6e 616d        if dev_nam
+0000b660: 652e 7374 6172 7473 7769 7468 2827 444d  e.startswith('DM
+0000b670: 3727 293a 0a20 2020 2020 2020 2020 2020  7'):.           
+0000b680: 2020 2020 2073 656c 662e 6465 7669 6365       self.device
+0000b690: 5f6e 616d 6520 3d20 6465 765f 6e61 6d65  _name = dev_name
+0000b6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b6b0: 2073 656c 662e 6c6f 6767 6572 2e69 6e66   self.logger.inf
+0000b6c0: 6f28 6627 636f 6e6e 6563 7465 6420 746f  o(f'connected to
+0000b6d0: 207b 6465 765f 6e61 6d65 7d27 290a 2020   {dev_name}').  
+0000b6e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000b6f0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+0000b700: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+0000b710: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+0000b720: 2020 2020 2073 656c 662e 6c6f 6767 6572       self.logger
+0000b730: 2e69 6e66 6f28 6627 6465 7669 6365 2069  .info(f'device i
+0000b740: 7320 6e6f 7420 636f 6d6d 756e 6963 6174  s not communicat
+0000b750: 6520 6475 6520 746f 207b 657d 2729 0a20  e due to {e}'). 
+0000b760: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0000b770: 6c73 650a 0a20 2020 2064 6566 2072 6563  lse..    def rec
+0000b780: 6f6e 6e65 6374 2873 656c 6629 3a0a 2020  onnect(self):.  
+0000b790: 2020 2020 2020 7365 6c66 2e6c 6f67 6765        self.logge
+0000b7a0: 722e 696e 666f 2866 2754 7279 2020 746f  r.info(f'Try  to
+0000b7b0: 2072 6563 6f6e 6e65 6374 2e2e 2e27 290a   reconnect...').
+0000b7c0: 2020 2020 2020 2020 7365 6c66 2e63 6c6f          self.clo
+0000b7d0: 7365 5f70 6f72 7428 290a 2020 2020 2020  se_port().      
+0000b7e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000b7f0: 2020 2073 656c 662e 636f 6e6e 6563 7465     self.connecte
+0000b800: 6420 3d20 7365 6c66 2e6f 7065 6e5f 706f  d = self.open_po
+0000b810: 7274 2873 656c 662e 636f 6d5f 706f 7274  rt(self.com_port
+0000b820: 2c20 7365 6c66 2e62 6175 645f 7261 7465  , self.baud_rate
+0000b830: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+0000b840: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+0000b850: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000b860: 662e 6c6f 6767 6572 2e77 6172 6e69 6e67  f.logger.warning
+0000b870: 2866 2763 6f75 6c64 206e 6f74 2072 6563  (f'could not rec
+0000b880: 6f6e 6e65 6374 2074 6f20 6465 7669 6365  onnect to device
+0000b890: 3a20 7b65 7d27 290a 2020 2020 2020 2020  : {e}').        
+0000b8a0: 2020 2020 6966 2073 656c 662e 636f 6e6e      if self.conn
+0000b8b0: 6563 7465 643a 0a20 2020 2020 2020 2020  ected:.         
+0000b8c0: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
+0000b8d0: 5f63 6f6e 6669 6775 7261 7469 6f6e 7328  _configurations(
+0000b8e0: 290a 0a20 2020 2064 6566 2063 6f6e 6669  )..    def confi
+0000b8f0: 6775 7265 2873 656c 662c 2063 6f6d 6d61  gure(self, comma
+0000b900: 6e64 2c20 7661 6c75 6529 3a0a 2020 2020  nd, value):.    
+0000b910: 2020 2020 7365 6c66 2e73 6574 5f64 6576      self.set_dev
+0000b920: 6963 655f 7072 6f70 6572 7479 2863 6f6d  ice_property(com
+0000b930: 6d61 6e64 2c20 7661 6c75 6529 0a20 2020  mand, value).   
+0000b940: 2020 2020 2073 6c65 6570 2830 2e31 290a       sleep(0.1).
+0000b950: 2020 2020 2020 2020 7273 7020 3d20 7365          rsp = se
+0000b960: 6c66 2e67 6574 5f64 6576 6963 655f 7072  lf.get_device_pr
+0000b970: 6f70 6572 7479 2863 6f6d 6d61 6e64 290a  operty(command).
+0000b980: 2020 2020 2020 2020 6966 2073 7472 2876          if str(v
+0000b990: 616c 7565 2920 6e6f 7420 696e 2072 7370  alue) not in rsp
+0000b9a0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000b9b0: 6973 6520 4578 6365 7074 696f 6e28 6627  ise Exception(f'
+0000b9c0: 436f 756c 6420 6e6f 7420 636f 6e66 6967  Could not config
+0000b9d0: 7572 6520 7b63 6f6d 6d61 6e64 7d20 746f  ure {command} to
+0000b9e0: 207b 7661 6c75 657d 2e20 7468 6520 7b63   {value}. the {c
+0000b9f0: 6f6d 6d61 6e64 7d20 6973 2063 7572 7265  ommand} is curre
+0000ba00: 6e74 6c79 2073 6574 2074 6f20 7b72 7370  ntly set to {rsp
+0000ba10: 7d27 290a 0a20 2020 2064 6566 2069 6e69  }')..    def ini
+0000ba20: 745f 636f 6e66 6967 7572 6174 696f 6e73  t_configurations
+0000ba30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000ba40: 6966 2073 656c 662e 6465 6661 756c 745f  if self.default_
+0000ba50: 636f 6e66 6967 2069 7320 6e6f 7420 4e6f  config is not No
+0000ba60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000ba70: 666f 7220 636d 642c 2076 616c 2069 6e20  for cmd, val in 
+0000ba80: 7365 6c66 2e64 6566 6175 6c74 5f63 6f6e  self.default_con
+0000ba90: 6669 672e 6974 656d 7328 293a 0a20 2020  fig.items():.   
+0000baa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000bab0: 662e 636f 6e66 6967 7572 6528 636f 6d6d  f.configure(comm
+0000bac0: 616e 643d 636d 642c 2076 616c 7565 3d76  and=cmd, value=v
+0000bad0: 616c 290a 0a20 2020 2064 6566 2073 656e  al)..    def sen
+0000bae0: 645f 636f 6d6d 616e 6428 7365 6c66 2c20  d_command(self, 
+0000baf0: 636f 6d6d 616e 642c 2063 6f6d 6d61 6e64  command, command
+0000bb00: 5f69 643d 3132 332c 2063 6865 636b 7375  _id=123, checksu
+0000bb10: 6d3d 3029 3a0a 2020 2020 2020 2020 636f  m=0):.        co
+0000bb20: 6d6d 616e 645f 6865 6164 6572 203d 2066  mmand_header = f
+0000bb30: 277c 7c7b 6368 6563 6b73 756d 7d3a 7b63  '||{checksum}:{c
+0000bb40: 6f6d 6d61 6e64 5f69 647d 3e27 0a20 2020  ommand_id}>'.   
+0000bb50: 2020 2020 2066 6f6f 7465 7220 3d20 275c       footer = '\
+0000bb60: 725c 6e27 0a20 2020 2020 2020 2066 756c  r\n'.        ful
+0000bb70: 6c5f 636f 6d6d 616e 6420 3d20 6627 7b63  l_command = f'{c
+0000bb80: 6f6d 6d61 6e64 5f68 6561 6465 727d 7b63  ommand_header}{c
+0000bb90: 6f6d 6d61 6e64 7d7b 666f 6f74 6572 7d27  ommand}{footer}'
+0000bba0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+0000bbb0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0000bbc0: 6f67 6765 722e 696e 666f 2827 4d65 7373  ogger.info('Mess
+0000bbd0: 6167 6520 7365 6e74 207b 7d27 2e66 6f72  age sent {}'.for
+0000bbe0: 6d61 7428 6675 6c6c 5f63 6f6d 6d61 6e64  mat(full_command
+0000bbf0: 2e65 6e63 6f64 6528 2929 290a 2020 2020  .encode())).    
+0000bc00: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
+0000bc10: 2e77 7269 7465 2866 756c 6c5f 636f 6d6d  .write(full_comm
+0000bc20: 616e 642e 656e 636f 6465 2829 290a 2020  and.encode()).  
+0000bc30: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+0000bc40: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
+0000bc50: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+0000bc60: 7863 6570 7469 6f6e 2866 2246 6169 6c65  xception(f"Faile
+0000bc70: 6420 746f 2073 656e 6420 636f 6d6d 616e  d to send comman
+0000bc80: 6420 6475 6520 746f 3a20 7b65 7d22 290a  d due to: {e}").
+0000bc90: 0a20 2020 2064 6566 2072 6561 645f 7265  .    def read_re
+0000bca0: 7370 6f6e 7365 2873 656c 6629 3a0a 2020  sponse(self):.  
+0000bcb0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000bcc0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0000bcd0: 3d20 7365 6c66 2e73 6572 2e72 6561 646c  = self.ser.readl
+0000bce0: 696e 6528 292e 6465 636f 6465 2829 0a20  ine().decode(). 
+0000bcf0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+0000bd00: 6e73 6520 3d20 7265 7370 6f6e 7365 2e73  nse = response.s
+0000bd10: 7472 6970 2827 5c72 5c6e 2729 0a20 2020  trip('\r\n').   
+0000bd20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000bd30: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+0000bd40: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0000bd50: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+0000bd60: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+0000bd70: 696f 6e28 6622 4661 696c 6564 2074 6f20  ion(f"Failed to 
+0000bd80: 7265 6164 2072 6573 706f 6e73 653a 207b  read response: {
+0000bd90: 657d 2229 0a0a 2020 2020 6465 6620 7265  e}")..    def re
+0000bda0: 6164 5f62 6174 6368 2873 656c 662c 206e  ad_batch(self, n
+0000bdb0: 5f6d 7367 3d31 3030 302c 2077 6169 745f  _msg=1000, wait_
+0000bdc0: 7469 6d65 3d30 2e30 293a 0a20 2020 2020  time=0.0):.     
+0000bdd0: 2020 2022 2222 0a20 2020 2020 2020 2077     """.        w
+0000bde0: 6169 745f 7469 6d65 2069 6e20 7365 636f  ait_time in seco
+0000bdf0: 6e64 730a 2020 2020 2020 2020 4070 6172  nds.        @par
+0000be00: 616d 206e 5f6d 7367 206d 6178 206e 756d  am n_msg max num
+0000be10: 6265 7220 6f66 206d 7367 2074 6f20 7374  ber of msg to st
+0000be20: 6f70 2074 6865 2072 6561 6469 6e67 2062  op the reading b
+0000be30: 6174 6368 0a20 2020 2020 2020 2040 7479  atch.        @ty
+0000be40: 7065 206e 5f6d 7367 2069 6e74 0a20 2020  pe n_msg int.   
+0000be50: 2020 2020 2040 7061 7261 6d20 7761 6974       @param wait
+0000be60: 5f74 696d 6520 7468 6520 6d61 7820 7469  _time the max ti
+0000be70: 6d65 2069 6e20 7365 636f 6e64 2074 696c  me in second til
+0000be80: 6c20 6e65 6564 2074 6f20 7374 6f70 2074  l need to stop t
+0000be90: 6865 2072 6561 6469 6e67 2062 6174 6368  he reading batch
+0000bea0: 0a20 2020 2020 2020 2040 7479 7065 2077  .        @type w
+0000beb0: 6169 745f 7469 6d65 2066 6c6f 6174 0a20  ait_time float. 
+0000bec0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000bed0: 2020 2072 7370 5f6f 7574 203d 205b 5d0a     rsp_out = [].
+0000bee0: 2020 2020 2020 2020 745f 7374 6172 7420          t_start 
+0000bef0: 3d20 7469 6d65 2829 0a20 2020 2020 2020  = time().       
+0000bf00: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0000bf10: 6e5f 6d73 6729 3a0a 2020 2020 2020 2020  n_msg):.        
+0000bf20: 2020 2020 6966 2073 656c 662e 7365 722e      if self.ser.
+0000bf30: 696e 5f77 6169 7469 6e67 203d 3d20 303a  in_waiting == 0:
+0000bf40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bf50: 2069 6620 7469 6d65 2829 202d 2074 5f73   if time() - t_s
+0000bf60: 7461 7274 203c 2077 6169 745f 7469 6d65  tart < wait_time
+0000bf70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bf80: 2020 2020 2020 736c 6565 7028 302e 3035        sleep(0.05
+0000bf90: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+0000bfa0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000bfb0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+0000bfc0: 616b 0a20 2020 2020 2020 2020 2020 2072  ak.            r
+0000bfd0: 7370 203d 2073 656c 662e 7265 6164 5f72  sp = self.read_r
+0000bfe0: 6573 706f 6e73 6528 290a 2020 2020 2020  esponse().      
+0000bff0: 2020 2020 2020 6966 2072 7370 203d 3d20        if rsp == 
+0000c000: 2727 3a0a 2020 2020 2020 2020 2020 2020  '':.            
+0000c010: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+0000c020: 2020 2020 2020 7273 705f 6f75 742e 6170        rsp_out.ap
+0000c030: 7065 6e64 2872 7370 290a 2020 2020 2020  pend(rsp).      
+0000c040: 2020 7265 7475 726e 206c 6973 7428 7365    return list(se
+0000c050: 7428 7273 705f 6f75 7429 290a 0a20 2020  t(rsp_out))..   
+0000c060: 2064 6566 2064 6973 636f 7665 725f 6465   def discover_de
+0000c070: 7669 6365 2873 656c 6629 3a0a 2020 2020  vice(self):.    
+0000c080: 2020 2020 7365 6c66 2e73 656e 645f 636f      self.send_co
+0000c090: 6d6d 616e 6428 2747 4554 2044 4556 4943  mmand('GET DEVIC
+0000c0a0: 452e 5459 5045 2729 0a20 2020 2020 2020  E.TYPE').       
+0000c0b0: 2072 6574 7572 6e20 7365 6c66 2e72 6561   return self.rea
+0000c0c0: 645f 7265 7370 6f6e 7365 2829 0a0a 2020  d_response()..  
+0000c0d0: 2020 6465 6620 7365 745f 6465 7669 6365    def set_device
+0000c0e0: 5f70 726f 7065 7274 7928 7365 6c66 2c20  _property(self, 
+0000c0f0: 7072 6f70 6572 7479 5f6e 616d 652c 2076  property_name, v
+0000c100: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
+0000c110: 656c 662e 7365 6e64 5f63 6f6d 6d61 6e64  elf.send_command
+0000c120: 2866 2753 4554 207b 7072 6f70 6572 7479  (f'SET {property
+0000c130: 5f6e 616d 657d 207b 7661 6c75 657d 2729  _name} {value}')
+0000c140: 0a20 2020 2020 2020 2073 6c65 6570 2830  .        sleep(0
+0000c150: 2e31 290a 2020 2020 2020 2020 7265 7475  .1).        retu
+0000c160: 726e 2073 656c 662e 7265 6164 5f72 6573  rn self.read_res
+0000c170: 706f 6e73 6528 290a 0a20 2020 2064 6566  ponse()..    def
+0000c180: 2067 6574 5f64 6576 6963 655f 7072 6f70   get_device_prop
+0000c190: 6572 7479 2873 656c 662c 2070 726f 7065  erty(self, prope
+0000c1a0: 7274 795f 6e61 6d65 293a 0a20 2020 2020  rty_name):.     
+0000c1b0: 2020 2073 656c 662e 7365 6e64 5f63 6f6d     self.send_com
+0000c1c0: 6d61 6e64 2866 2747 4554 207b 7072 6f70  mand(f'GET {prop
+0000c1d0: 6572 7479 5f6e 616d 657d 2729 0a20 2020  erty_name}').   
+0000c1e0: 2020 2020 2073 6c65 6570 2830 2e31 290a       sleep(0.1).
+0000c1f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000c200: 656c 662e 7265 6164 5f72 6573 706f 6e73  elf.read_respons
+0000c210: 6528 290a 0a20 2020 2064 6566 2074 7269  e()..    def tri
+0000c220: 6767 6572 5f6f 6e28 7365 6c66 2c20 636f  gger_on(self, co
+0000c230: 6e74 696e 756f 7573 6c79 3d46 616c 7365  ntinuously=False
+0000c240: 2c20 7472 6967 6765 725f 7479 7065 3d30  , trigger_type=0
+0000c250: 2c20 6e65 6564 5f74 6f5f 636f 6e66 6967  , need_to_config
+0000c260: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
+0000c270: 2022 2222 0a0a 2020 2020 2020 2020 4070   """..        @p
+0000c280: 6172 616d 2074 7269 6767 6572 5f74 7970  aram trigger_typ
+0000c290: 653a 2030 3a20 5369 6e67 6c65 2028 6578  e: 0: Single (ex
+0000c2a0: 7465 726e 616c 292c 2031 3a20 5072 6573  ternal), 1: Pres
+0000c2b0: 656e 7461 7469 6f6e 2028 696e 7465 726e  entation (intern
+0000c2c0: 616c 292c 2032 3a20 4d61 6e75 616c 2028  al), 2: Manual (
+0000c2d0: 6275 7474 6f6e 292c 2033 3a20 4275 7273  button), 3: Burs
+0000c2e0: 7420 2865 7874 6572 6e61 6c29 2c0a 2020  t (external),.  
+0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c300: 2020 2034 3a20 5365 6c66 2028 696e 7465     4: Self (inte
+0000c310: 726e 616c 292c 2035 3a20 436f 6e74 696e  rnal), 5: Contin
+0000c320: 756f 7573 2028 6578 7465 726e 616c 290a  uous (external).
+0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c340: 2020 2020 202a 2053 696e 676c 653a 2041       * Single: A
+0000c350: 6371 7569 7265 7320 6120 7369 6e67 6c65  cquires a single
+0000c360: 2069 6d61 6765 2061 6e64 2061 7474 656d   image and attem
+0000c370: 7074 7320 746f 2064 6563 6f64 6520 616e  pts to decode an
+0000c380: 7920 7379 6d62 6f6c 2069 7420 636f 6e74  y symbol it cont
+0000c390: 6169 6e73 206f 7220 6d6f 7265 2074 6861  ains or more tha
+0000c3a0: 6e20 6f6e 650a 2020 2020 2020 2020 2020  n one.          
+0000c3b0: 2020 2020 2020 2020 2020 2073 796d 626f             symbo
+0000c3c0: 6c20 696e 2063 6173 6573 2077 6865 7265  l in cases where
+0000c3d0: 206d 756c 7469 636f 6465 2069 7320 656e   multicode is en
+0000c3e0: 6162 6c65 642e 2054 6865 2072 6561 6465  abled. The reade
+0000c3f0: 7220 7265 6c69 6573 206f 6e20 616e 2065  r relies on an e
+0000c400: 7874 6572 6e61 6c20 7472 6967 6765 7220  xternal trigger 
+0000c410: 736f 7572 6365 2e0a 2020 2020 2020 2020  source..        
+0000c420: 2020 2020 2020 2020 2020 2020 202a 2050               * P
+0000c430: 7265 7365 6e74 6174 696f 6e3a 2052 6570  resentation: Rep
+0000c440: 6561 7465 646c 7920 7363 616e 7320 666f  eatedly scans fo
+0000c450: 7220 6120 7379 6d62 6f6c 2061 6e64 2064  r a symbol and d
+0000c460: 6563 6f64 6573 2069 7420 7768 656e 6576  ecodes it whenev
+0000c470: 6572 206f 6e65 2069 7320 6465 7465 6374  er one is detect
+0000c480: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+0000c490: 2020 2020 2020 2020 2054 6865 2072 6561           The rea
+0000c4a0: 6465 7220 7265 6c69 6573 206f 6e20 616e  der relies on an
+0000c4b0: 2069 6e74 6572 6e61 6c20 7469 6d69 6e67   internal timing
+0000c4c0: 206d 6563 6861 6e69 736d 2074 6f20 6163   mechanism to ac
+0000c4d0: 7175 6972 6520 696d 6167 6573 2e0a 2020  quire images..  
+0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4f0: 2020 202a 2042 7572 7374 3a20 5065 7266     * Burst: Perf
+0000c500: 6f72 6d73 206d 756c 7469 706c 6520 696d  orms multiple im
+0000c510: 6167 6520 6163 7175 6973 6974 696f 6e73  age acquisitions
+0000c520: 2062 6173 6564 206f 6e20 616e 2065 7874   based on an ext
+0000c530: 6572 6e61 6c20 7472 6967 6765 7220 616e  ernal trigger an
+0000c540: 6420 6465 636f 6465 7320 6f6e 6520 6f72  d decodes one or
+0000c550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c560: 2020 2020 2020 6d75 6c74 6970 6c65 2073        multiple s
+0000c570: 796d 626f 6c73 2061 7070 6561 7269 6e67  ymbols appearing
+0000c580: 2069 6e20 7468 6520 7365 7175 656e 6365   in the sequence
+0000c590: 206f 6620 696d 6167 6573 2e0a 2020 2020   of images..    
+0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5b0: 202a 2053 656c 663a 2053 696d 696c 6172   * Self: Similar
+0000c5c0: 2074 6f20 5072 6573 656e 7461 7469 6f6e   to Presentation
+0000c5d0: 206d 6f64 6520 696e 2074 6861 7420 7468   mode in that th
+0000c5e0: 6520 7265 6164 6572 2070 6572 7065 7475  e reader perpetu
+0000c5f0: 616c 6c79 2073 6361 6e73 2066 6f72 2073  ally scans for s
+0000c600: 796d 626f 6c73 2061 6e64 2064 6563 6f64  ymbols and decod
+0000c610: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+0000c620: 2020 2020 2020 2020 7468 656d 2065 6163          them eac
+0000c630: 6820 7469 6d65 206f 6e65 2069 7320 6465  h time one is de
+0000c640: 7465 6374 6564 2e20 556e 6c69 6b65 2050  tected. Unlike P
+0000c650: 7265 7365 6e74 6174 696f 6e20 6d6f 6465  resentation mode
+0000c660: 2c20 686f 7765 7665 722c 2053 656c 6620  , however, Self 
+0000c670: 6d6f 6465 2073 7570 706f 7274 7320 6d75  mode supports mu
+0000c680: 6c74 6963 6f64 650a 2020 2020 2020 2020  lticode.        
+0000c690: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0000c6a0: 756c 7473 2061 6e64 2061 2064 6563 6f64  ults and a decod
+0000c6b0: 6520 6174 7465 6d70 7420 6f63 6375 7273  e attempt occurs
+0000c6c0: 2077 6974 6820 6576 6572 7920 696d 6167   with every imag
+0000c6d0: 652e 2054 6865 206d 6169 6e20 6469 6666  e. The main diff
+0000c6e0: 6572 656e 6365 2062 6574 7765 656e 2053  erence between S
+0000c6f0: 656c 6620 616e 640a 2020 2020 2020 2020  elf and.        
+0000c700: 2020 2020 2020 2020 2020 2020 2050 7265               Pre
+0000c710: 7365 6e74 6174 696f 6e20 6973 2074 6865  sentation is the
+0000c720: 2066 6978 6564 2061 6e64 2065 7861 6374   fixed and exact
+0000c730: 2069 6e74 6572 7661 6c20 666f 7220 696d   interval for im
+0000c740: 6167 6520 6163 7175 6973 6974 696f 6e73  age acquisitions
+0000c750: 2069 6e20 5365 6c66 2e0a 2020 2020 2020   in Self..      
+0000c760: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0000c770: 2043 6f6e 7469 6e75 6f75 733a 2042 6567   Continuous: Beg
+0000c780: 696e 7320 6163 7175 6972 696e 6720 696d  ins acquiring im
+0000c790: 6167 6573 2062 6173 6564 206f 6e20 6120  ages based on a 
+0000c7a0: 7369 6e67 6c65 2065 7874 6572 6e61 6c20  single external 
+0000c7b0: 7472 6967 6765 7220 616e 6420 636f 6e74  trigger and cont
+0000c7c0: 696e 7565 7320 746f 2061 6371 7569 7265  inues to acquire
+0000c7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c7e0: 2020 2020 2020 696d 6167 6573 2075 6e74        images unt
+0000c7f0: 696c 2061 2073 796d 626f 6c20 6973 2066  il a symbol is f
+0000c800: 6f75 6e64 2061 6e64 2064 6563 6f64 6564  ound and decoded
+0000c810: 2c20 6f72 2075 6e74 696c 206d 756c 7469  , or until multi
+0000c820: 706c 6520 696d 6167 6573 2063 6f6e 7461  ple images conta
+0000c830: 696e 696e 6720 6173 206d 616e 7920 636f  ining as many co
+0000c840: 6465 7320 6173 0a20 2020 2020 2020 2020  des as.         
+0000c850: 2020 2020 2020 2020 2020 2020 7370 6563              spec
+0000c860: 6966 6965 6420 696e 206d 756c 7469 636f  ified in multico
+0000c870: 6465 206d 6f64 6520 6172 6520 6c6f 6361  de mode are loca
+0000c880: 7465 642c 206f 7220 756e 7469 6c20 7468  ted, or until th
+0000c890: 6520 7472 6967 6765 7220 6973 2072 656c  e trigger is rel
+0000c8a0: 6561 7365 642e 0a20 2020 2020 2020 2040  eased..        @
+0000c8b0: 7479 7065 2074 7269 6767 6572 5f74 7970  type trigger_typ
+0000c8c0: 653a 2069 6e74 0a20 2020 2020 2020 2040  e: int.        @
+0000c8d0: 7061 7261 6d20 636f 6e74 696e 756f 7573  param continuous
+0000c8e0: 6c79 3a20 6966 2054 7275 652c 2074 6865  ly: if True, the
+0000c8f0: 2073 6361 6e6e 6572 2077 696c 6c20 7265   scanner will re
+0000c900: 6164 2069 6e20 636f 6e74 696e 756f 7573  ad in continuous
+0000c910: 206d 6f64 650a 2020 2020 2020 2020 4074   mode.        @t
+0000c920: 7970 6520 636f 6e74 696e 756f 7573 6c79  ype continuously
+0000c930: 3a20 626f 6f6c 0a20 2020 2020 2020 2040  : bool.        @
+0000c940: 7061 7261 6d20 6e65 6564 5f74 6f5f 636f  param need_to_co
+0000c950: 6e66 6967 3a20 6966 2054 7275 652c 2066  nfig: if True, f
+0000c960: 6972 7374 2074 6865 2073 6361 6e6e 6572  irst the scanner
+0000c970: 2069 7320 636f 6e66 6967 7572 6564 2077   is configured w
+0000c980: 6974 6820 7468 6520 7265 6c65 7661 6e74  ith the relevant
+0000c990: 2074 7269 6767 6572 2074 7970 650a 2020   trigger type.  
+0000c9a0: 2020 2020 2020 4074 7970 6520 6e65 6564        @type need
+0000c9b0: 5f74 6f5f 636f 6e66 6967 3a20 626f 6f6c  _to_config: bool
+0000c9c0: 0a20 2020 2020 2020 2040 7265 7475 726e  .        @return
+0000c9d0: 3a0a 2020 2020 2020 2020 4072 7479 7065  :.        @rtype
+0000c9e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000c9f0: 2020 2020 2020 6966 206e 6565 645f 746f        if need_to
+0000ca00: 5f63 6f6e 6669 673a 0a20 2020 2020 2020  _config:.       
+0000ca10: 2020 2020 2069 6620 636f 6e74 696e 756f       if continuo
+0000ca20: 7573 6c79 2061 6e64 2074 7269 6767 6572  usly and trigger
+0000ca30: 5f74 7970 6520 3d3d 2030 3a0a 2020 2020  _type == 0:.    
+0000ca40: 2020 2020 2020 2020 2020 2020 7472 6967              trig
+0000ca50: 6765 725f 7479 7065 203d 2073 656c 662e  ger_type = self.
+0000ca60: 434f 4e54 494e 554f 5553 5f54 5249 4747  CONTINUOUS_TRIGG
+0000ca70: 4552 5f54 5950 450a 2020 2020 2020 2020  ER_TYPE.        
+0000ca80: 2020 2020 7365 6c66 2e73 6574 5f64 6576      self.set_dev
+0000ca90: 6963 655f 7072 6f70 6572 7479 2827 5452  ice_property('TR
+0000caa0: 4947 4745 522e 5459 5045 272c 2074 7269  IGGER.TYPE', tri
+0000cab0: 6767 6572 5f74 7970 6529 0a20 2020 2020  gger_type).     
+0000cac0: 2020 2073 656c 662e 7365 6e64 5f63 6f6d     self.send_com
+0000cad0: 6d61 6e64 2827 5452 4947 4745 5220 4f4e  mand('TRIGGER ON
+0000cae0: 2729 0a0a 2020 2020 6465 6620 7472 6967  ')..    def trig
+0000caf0: 6765 725f 6f66 6628 7365 6c66 293a 0a20  ger_off(self):. 
+0000cb00: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+0000cb10: 5f63 6f6d 6d61 6e64 2827 5452 4947 4745  _command('TRIGGE
+0000cb20: 5220 4f46 4627 290a 0a20 2020 2064 6566  R OFF')..    def
+0000cb30: 2072 6573 6574 2873 656c 6629 3a0a 2020   reset(self):.  
+0000cb40: 2020 2020 2020 7761 6974 696e 675f 6279        waiting_by
+0000cb50: 7465 7320 3d20 7365 6c66 2e73 6572 2e69  tes = self.ser.i
+0000cb60: 6e5f 7761 6974 696e 670a 2020 2020 2020  n_waiting.      
+0000cb70: 2020 6966 2077 6169 7469 6e67 5f62 7974    if waiting_byt
+0000cb80: 6573 2021 3d20 303a 0a20 2020 2020 2020  es != 0:.       
+0000cb90: 2020 2020 2073 656c 662e 7365 722e 7265       self.ser.re
+0000cba0: 7365 745f 696e 7075 745f 6275 6666 6572  set_input_buffer
+0000cbb0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+0000cbc0: 656c 662e 6c6f 6767 6572 2e69 6e66 6f28  elf.logger.info(
+0000cbd0: 6627 636c 6561 6e20 6275 6666 6572 2066  f'clean buffer f
+0000cbe0: 726f 6d20 7b77 6169 7469 6e67 5f62 7974  rom {waiting_byt
+0000cbf0: 6573 7d20 6279 7465 7327 290a 0a20 2020  es} bytes')..   
+0000cc00: 2064 6566 2073 6361 6e5f 6578 745f 6964   def scan_ext_id
+0000cc10: 2873 656c 662c 206e 6565 645f 746f 5f74  (self, need_to_t
+0000cc20: 7269 6767 6572 3d54 7275 6529 3a0a 2020  rigger=True):.  
+0000cc30: 2020 2020 2020 6966 206e 6565 645f 746f        if need_to
+0000cc40: 5f74 7269 6767 6572 3a0a 2020 2020 2020  _trigger:.      
+0000cc50: 2020 2020 2020 7365 6c66 2e74 7269 6767        self.trigg
+0000cc60: 6572 5f6f 6e28 6e65 6564 5f74 6f5f 636f  er_on(need_to_co
+0000cc70: 6e66 6967 3d46 616c 7365 290a 0a20 2020  nfig=False)..   
+0000cc80: 2020 2020 2072 7370 203d 2073 656c 662e       rsp = self.
+0000cc90: 7265 6164 5f72 6573 706f 6e73 6528 290a  read_response().
+0000cca0: 2020 2020 2020 2020 6966 2072 7370 203d          if rsp =
+0000ccb0: 3d20 2727 3a0a 2020 2020 2020 2020 2020  = '':.          
+0000ccc0: 2020 7265 7475 726e 204e 6f6e 652c 204e    return None, N
+0000ccd0: 6f6e 652c 204e 6f6e 652c 204e 6f6e 650a  one, None, None.
+0000cce0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0000ccf0: 7273 7029 203d 3d20 7365 6c66 2e53 4754  rsp) == self.SGT
+0000cd00: 494e 5f53 5452 4950 5f4c 454e 206f 7220  IN_STRIP_LEN or 
+0000cd10: 6c65 6e28 7273 7029 203d 3d20 7365 6c66  len(rsp) == self
+0000cd20: 2e53 4754 494e 5f4c 454e 3a0a 2020 2020  .SGTIN_LEN:.    
+0000cd30: 2020 2020 2020 2020 6375 725f 6964 203d          cur_id =
+0000cd40: 2072 7370 2e73 706c 6974 2827 5427 295b   rsp.split('T')[
+0000cd50: 315d 0a20 2020 2020 2020 2020 2020 2067  1].            g
+0000cd60: 7469 6e5f 616e 645f 7265 656c 5f69 6420  tin_and_reel_id 
+0000cd70: 3d20 7273 702e 7370 6c69 7428 2754 2729  = rsp.split('T')
+0000cd80: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+0000cd90: 7265 656c 5f69 6420 3d20 6774 696e 5f61  reel_id = gtin_a
+0000cda0: 6e64 5f72 6565 6c5f 6964 5b2d 7365 6c66  nd_reel_id[-self
+0000cdb0: 2e52 4545 4c5f 4944 5f4c 454e 3a5d 0a20  .REEL_ID_LEN:]. 
+0000cdc0: 2020 2020 2020 2020 2020 2067 7469 6e20             gtin 
+0000cdd0: 3d20 6774 696e 5f61 6e64 5f72 6565 6c5f  = gtin_and_reel_
+0000cde0: 6964 5b3a 2d73 656c 662e 5245 454c 5f49  id[:-self.REEL_I
+0000cdf0: 445f 4c45 4e5d 0a20 2020 2020 2020 2065  D_LEN].        e
+0000ce00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000ce10: 2063 7572 5f69 6420 3d20 7273 702e 7370   cur_id = rsp.sp
+0000ce20: 6c69 7428 2754 2729 5b31 5d0a 2020 2020  lit('T')[1].    
+0000ce30: 2020 2020 2020 2020 7265 656c 5f69 6420          reel_id 
+0000ce40: 3d20 7273 702e 7370 6c69 7428 2754 2729  = rsp.split('T')
+0000ce50: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+0000ce60: 6774 696e 203d 2027 270a 2020 2020 2020  gtin = ''.      
+0000ce70: 2020 7265 7475 726e 2072 7370 2c20 6375    return rsp, cu
+0000ce80: 725f 6964 2c20 7265 656c 5f69 642c 2067  r_id, reel_id, g
+0000ce90: 7469 6e0a 0a20 2020 2064 6566 2062 6565  tin..    def bee
+0000cea0: 7028 7365 6c66 2c20 6475 7261 7469 6f6e  p(self, duration
+0000ceb0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000cec0: 7365 6e64 5f63 6f6d 6d61 6e64 2866 2742  send_command(f'B
+0000ced0: 4545 5020 7b64 7572 6174 696f 6e7d 2729  EEP {duration}')
+0000cee0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000cef0: 7365 6c66 2e72 6561 645f 7265 7370 6f6e  self.read_respon
+0000cf00: 7365 2829 0a0a 2020 2020 6465 6620 7365  se()..    def se
+0000cf10: 745f 6465 636f 6465 725f 726f 6928 7365  t_decoder_roi(se
+0000cf20: 6c66 2c20 7831 2c20 7832 2c20 7931 2c20  lf, x1, x2, y1, 
+0000cf30: 7932 293a 0a20 2020 2020 2020 2073 656c  y2):.        sel
+0000cf40: 662e 7365 6e64 5f63 6f6d 6d61 6e64 2866  f.send_command(f
+0000cf50: 2753 4554 2044 4543 4f44 4552 2e52 4f49  'SET DECODER.ROI
+0000cf60: 207b 7831 7d2c 207b 7832 7d2c 207b 7931   {x1}, {x2}, {y1
+0000cf70: 7d2c 207b 7932 7d27 290a 2020 2020 2020  }, {y2}').      
+0000cf80: 2020 7265 7475 726e 2073 656c 662e 7265    return self.re
+0000cf90: 6164 5f72 6573 706f 6e73 6528 290a 0a20  ad_response().. 
+0000cfa0: 2020 2064 6566 2073 6574 5f66 7470 5f69     def set_ftp_i
+0000cfb0: 6d61 6765 5f69 705f 6164 6472 6573 7328  mage_ip_address(
+0000cfc0: 7365 6c66 2c20 6970 5f61 6464 7265 7373  self, ip_address
+0000cfd0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000cfe0: 7365 6e64 5f63 6f6d 6d61 6e64 2866 2753  send_command(f'S
+0000cff0: 4554 2046 5450 2d49 4d41 4745 2e49 502d  ET FTP-IMAGE.IP-
+0000d000: 4144 4452 4553 5320 7b69 705f 6164 6472  ADDRESS {ip_addr
+0000d010: 6573 737d 2729 0a20 2020 2020 2020 2072  ess}').        r
+0000d020: 6574 7572 6e20 7365 6c66 2e72 6561 645f  eturn self.read_
+0000d030: 7265 7370 6f6e 7365 2829 0a0a 2020 2020  response()..    
+0000d040: 6465 6620 6765 745f 6d61 635f 6164 6472  def get_mac_addr
+0000d050: 6573 7328 7365 6c66 293a 0a20 2020 2020  ess(self):.     
+0000d060: 2020 2073 656c 662e 7365 6e64 5f63 6f6d     self.send_com
+0000d070: 6d61 6e64 2827 4745 5420 4445 5649 4345  mand('GET DEVICE
+0000d080: 2e4d 4143 2d41 4444 5245 5353 2729 0a20  .MAC-ADDRESS'). 
+0000d090: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000d0a0: 6c66 2e72 6561 645f 7265 7370 6f6e 7365  lf.read_response
+0000d0b0: 2829 0a0a 2020 2020 6465 6620 636c 6f73  ()..    def clos
+0000d0c0: 655f 706f 7274 2873 656c 6629 3a0a 2020  e_port(self):.  
+0000d0d0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000d0e0: 2020 2020 2020 2073 656c 662e 7365 722e         self.ser.
+0000d0f0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+0000d100: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+0000d110: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+0000d120: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+0000d130: 6f6e 2866 2246 6169 6c65 6420 746f 2063  on(f"Failed to c
+0000d140: 6c6f 7365 2073 6572 6961 6c20 706f 7274  lose serial port
+0000d150: 3a20 7b65 7d22 290a 0a0a 636c 6173 7320  : {e}")...class 
+0000d160: 596f 6374 6f54 656d 7065 7261 7475 7265  YoctoTemperature
+0000d170: 5365 6e73 6f72 286f 626a 6563 7429 3a0a  Sensor(object):.
+0000d180: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000d190: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000d1a0: 7365 6c66 2e73 656e 736f 7220 3d20 4e6f  self.sensor = No
+0000d1b0: 6e65 0a20 2020 2020 2020 2065 7272 6d73  ne.        errms
+0000d1c0: 6720 3d20 5952 6566 5061 7261 6d28 290a  g = YRefParam().
+0000d1d0: 2020 2020 2020 2020 2320 5365 7475 7020          # Setup 
+0000d1e0: 7468 6520 4150 4920 746f 2075 7365 206c  the API to use l
+0000d1f0: 6f63 616c 2055 5342 2064 6576 6963 6573  ocal USB devices
+0000d200: 0a20 2020 2020 2020 2069 6620 5941 5049  .        if YAPI
+0000d210: 2e52 6567 6973 7465 7248 7562 2822 7573  .RegisterHub("us
+0000d220: 6222 2c20 6572 726d 7367 2920 213d 2059  b", errmsg) != Y
+0000d230: 4150 492e 5355 4343 4553 533a 0a20 2020  API.SUCCESS:.   
+0000d240: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+0000d250: 7175 6970 6d65 6e74 4572 726f 7228 2779  quipmentError('y
+0000d260: 6f63 746f 2074 656d 7065 7261 7475 7265  octo temperature
+0000d270: 2073 656e 736f 7220 676f 7420 696e 6974   sensor got init
+0000d280: 2065 7272 6f72 3a20 7b7d 272e 666f 726d   error: {}'.form
+0000d290: 6174 2865 7272 6d73 672e 7661 6c75 6529  at(errmsg.value)
+0000d2a0: 290a 0a20 2020 2064 6566 2063 6f6e 6e65  )..    def conne
+0000d2b0: 6374 2873 656c 662c 2074 6172 6765 743d  ct(self, target=
+0000d2c0: 2761 6e79 2729 3a0a 2020 2020 2020 2020  'any'):.        
+0000d2d0: 6966 2074 6172 6765 7420 3d3d 2027 616e  if target == 'an
+0000d2e0: 7927 3a0a 2020 2020 2020 2020 2020 2020  y':.            
+0000d2f0: 2320 7265 7472 6965 7665 2061 6e79 2074  # retrieve any t
+0000d300: 656d 7065 7261 7475 7265 2073 656e 736f  emperature senso
+0000d310: 720a 2020 2020 2020 2020 2020 2020 7365  r.            se
+0000d320: 6c66 2e73 656e 736f 7220 3d20 5954 656d  lf.sensor = YTem
+0000d330: 7065 7261 7475 7265 2e46 6972 7374 5465  perature.FirstTe
+0000d340: 6d70 6572 6174 7572 6528 290a 2020 2020  mperature().    
+0000d350: 2020 2020 656c 6966 2074 6172 6765 7420      elif target 
+0000d360: 3d3d 2027 273a 0a20 2020 2020 2020 2020  == '':.         
+0000d370: 2020 2070 7269 6e74 2827 7370 6563 6966     print('specif
+0000d380: 6965 6420 696e 7661 6c69 6420 7461 7267  ied invalid targ
+0000d390: 6574 2729 0a20 2020 2020 2020 2020 2020  et').           
+0000d3a0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0000d3b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000d3c0: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+0000d3d0: 736f 7220 3d20 5954 656d 7065 7261 7475  sor = YTemperatu
+0000d3e0: 7265 2e46 696e 6454 656d 7065 7261 7475  re.FindTemperatu
+0000d3f0: 7265 2874 6172 6765 7420 2b20 272e 7465  re(target + '.te
+0000d400: 6d70 6572 6174 7572 6527 290a 2020 2020  mperature').    
+0000d410: 2020 2020 6966 2073 656c 662e 7365 6e73      if self.sens
+0000d420: 6f72 2069 7320 4e6f 6e65 206f 7220 7365  or is None or se
+0000d430: 6c66 2e67 6574 5f73 656e 736f 725f 6e61  lf.get_sensor_na
+0000d440: 6d65 2829 203d 3d20 2775 6e72 6573 6f6c  me() == 'unresol
+0000d450: 7665 6427 3a0a 2020 2020 2020 2020 2020  ved':.          
+0000d460: 2020 7072 696e 7428 274e 6f20 6d6f 6475    print('No modu
+0000d470: 6c65 2063 6f6e 6e65 6374 6564 2729 0a20  le connected'). 
+0000d480: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000d490: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+0000d4a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000d4b0: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+0000d4c0: 2020 2064 6566 2067 6574 5f73 656e 736f     def get_senso
+0000d4d0: 725f 6e61 6d65 2873 656c 6629 3a0a 2020  r_name(self):.  
+0000d4e0: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
+0000d4f0: 6e73 6f72 2069 7320 4e6f 6e65 3a0a 2020  nsor is None:.  
+0000d500: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000d510: 276e 6f20 7365 6e73 6f72 2069 7320 636f  'no sensor is co
+0000d520: 6e6e 6563 7465 642e 2074 7279 2074 6f20  nnected. try to 
+0000d530: 6361 6c6c 2063 6f6e 6e65 6374 2829 2066  call connect() f
+0000d540: 6972 7374 2729 0a20 2020 2020 2020 2020  irst').         
+0000d550: 2020 2072 6574 7572 6e20 2727 0a0a 2020     return ''..  
+0000d560: 2020 2020 2020 7365 6e73 6f72 5f73 7472        sensor_str
+0000d570: 203d 2073 656c 662e 7365 6e73 6f72 2e64   = self.sensor.d
+0000d580: 6573 6372 6962 6528 290a 2020 2020 2020  escribe().      
+0000d590: 2020 6e61 6d65 5f73 7472 203d 2073 656e    name_str = sen
+0000d5a0: 736f 725f 7374 722e 7370 6c69 7428 273d  sor_str.split('=
+0000d5b0: 2729 5b31 5d2e 7370 6c69 7428 272e 2729  ')[1].split('.')
+0000d5c0: 5b30 5d0a 2020 2020 2020 2020 7265 7475  [0].        retu
+0000d5d0: 726e 206e 616d 655f 7374 720a 0a20 2020  rn name_str..   
+0000d5e0: 2064 6566 2067 6574 5f74 656d 7065 7261   def get_tempera
+0000d5f0: 7475 7265 2873 656c 6629 3a0a 2020 2020  ture(self):.    
+0000d600: 2020 2020 6966 2073 656c 662e 7365 6e73      if self.sens
+0000d610: 6f72 2069 7320 4e6f 6e65 3a0a 2020 2020  or is None:.    
+0000d620: 2020 2020 2020 2020 7072 696e 7428 2773          print('s
+0000d630: 656e 736f 7220 6973 206e 6f74 2063 6f6e  ensor is not con
+0000d640: 6e65 6374 6564 2e20 7472 7920 746f 2063  nected. try to c
+0000d650: 616c 6c20 636f 6e6e 6563 7428 2920 6669  all connect() fi
+0000d660: 7273 7427 290a 2020 2020 2020 2020 2020  rst').          
+0000d670: 2020 7265 7475 726e 2066 6c6f 6174 2827    return float('
+0000d680: 6e61 6e27 290a 2020 2020 2020 2020 6966  nan').        if
+0000d690: 206e 6f74 2028 7365 6c66 2e73 656e 736f   not (self.senso
+0000d6a0: 722e 6973 4f6e 6c69 6e65 2829 293a 0a20  r.isOnline()):. 
+0000d6b0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000d6c0: 2827 7365 6e73 6f72 2069 7320 6e6f 7420  ('sensor is not 
+0000d6d0: 636f 6e6e 6563 7465 6420 6f72 2064 6973  connected or dis
+0000d6e0: 636f 6e6e 6563 7465 6420 6475 7269 6e67  connected during
+0000d6f0: 2072 756e 2729 0a20 2020 2020 2020 2020   run').         
+0000d700: 2020 2072 6574 7572 6e20 666c 6f61 7428     return float(
+0000d710: 276e 616e 2729 0a0a 2020 2020 2020 2020  'nan')..        
+0000d720: 7265 7475 726e 2073 656c 662e 7365 6e73  return self.sens
+0000d730: 6f72 2e67 6574 5f63 7572 7265 6e74 5661  or.get_currentVa
+0000d740: 6c75 6528 290a 0a20 2020 2040 7374 6174  lue()..    @stat
+0000d750: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+0000d760: 2065 7869 745f 6170 7028 293a 0a20 2020   exit_app():.   
+0000d770: 2020 2020 2059 4150 492e 4672 6565 4150       YAPI.FreeAP
+0000d780: 4928 290a 0a0a 636c 6173 7320 596f 6374  I()...class Yoct
+0000d790: 6f53 656e 736f 7228 6f62 6a65 6374 293a  oSensor(object):
+0000d7a0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000d7b0: 5f28 7365 6c66 2c20 6c6f 6767 6572 2c20  _(self, logger, 
+0000d7c0: 7461 7267 6574 3d4e 6f6e 6529 3a0a 2020  target=None):.  
+0000d7d0: 2020 2020 2020 7365 6c66 2e74 656d 7065        self.tempe
+0000d7e0: 7261 7475 7265 5f73 656e 736f 7220 3d20  rature_sensor = 
+0000d7f0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000d800: 662e 6875 6d69 6469 7479 5f73 656e 736f  f.humidity_senso
+0000d810: 7220 3d20 4e6f 6e65 0a20 2020 2020 2020  r = None.       
+0000d820: 2073 656c 662e 6c69 6768 745f 7365 6e73   self.light_sens
+0000d830: 6f72 203d 204e 6f6e 650a 2020 2020 2020  or = None.      
+0000d840: 2020 7365 6c66 2e6c 6f67 6765 7220 3d20    self.logger = 
+0000d850: 6c6f 6767 6572 0a20 2020 2020 2020 2065  logger.        e
+0000d860: 7272 6d73 6720 3d20 5952 6566 5061 7261  rrmsg = YRefPara
+0000d870: 6d28 290a 2020 2020 2020 2020 6966 2059  m().        if Y
+0000d880: 4150 492e 5265 6769 7374 6572 4875 6228  API.RegisterHub(
+0000d890: 2275 7362 222c 2065 7272 6d73 6729 2021  "usb", errmsg) !
+0000d8a0: 3d20 5941 5049 2e53 5543 4345 5353 3a0a  = YAPI.SUCCESS:.
+0000d8b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000d8c0: 6520 4571 7569 706d 656e 7445 7272 6f72  e EquipmentError
+0000d8d0: 2866 2759 6f63 746f 2073 656e 736f 7220  (f'Yocto sensor 
+0000d8e0: 696e 6974 6961 6c69 7a61 7469 6f6e 2065  initialization e
+0000d8f0: 7272 6f72 3a20 7b65 7272 6d73 672e 7661  rror: {errmsg.va
+0000d900: 6c75 657d 2729 0a20 2020 2020 2020 2074  lue}').        t
+0000d910: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000d920: 7365 6c66 2e63 6f6e 6e65 6374 2874 6172  self.connect(tar
+0000d930: 6765 743d 2761 6e79 2720 6966 2074 6172  get='any' if tar
+0000d940: 6765 7420 6973 204e 6f6e 6520 656c 7365  get is None else
+0000d950: 2074 6172 6765 7429 0a20 2020 2020 2020   target).       
+0000d960: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0000d970: 6e20 6173 2065 653a 0a20 2020 2020 2020  n as ee:.       
+0000d980: 2020 2020 2073 656c 662e 6c6f 6767 6572       self.logger
+0000d990: 2e69 6e66 6f28 2753 656e 736f 7220 6973  .info('Sensor is
+0000d9a0: 206e 6f74 2063 6f6e 6e65 6374 6564 2729   not connected')
+0000d9b0: 0a0a 2020 2020 6465 6620 636f 6e6e 6563  ..    def connec
+0000d9c0: 7428 7365 6c66 2c20 7461 7267 6574 3d27  t(self, target='
+0000d9d0: 616e 7927 293a 0a20 2020 2020 2020 2073  any'):.        s
+0000d9e0: 656e 736f 725f 6d61 7070 696e 6720 3d20  ensor_mapping = 
+0000d9f0: 7b0a 2020 2020 2020 2020 2020 2020 2774  {.            't
+0000da00: 656d 7065 7261 7475 7265 273a 2028 5954  emperature': (YT
+0000da10: 656d 7065 7261 7475 7265 2e46 6972 7374  emperature.First
+0000da20: 5465 6d70 6572 6174 7572 652c 2059 5465  Temperature, YTe
+0000da30: 6d70 6572 6174 7572 652e 4669 6e64 5465  mperature.FindTe
+0000da40: 6d70 6572 6174 7572 6529 2c0a 2020 2020  mperature),.    
+0000da50: 2020 2020 2020 2020 2768 756d 6964 6974          'humidit
+0000da60: 7927 3a20 2859 4875 6d69 6469 7479 2e46  y': (YHumidity.F
+0000da70: 6972 7374 4875 6d69 6469 7479 2c20 5948  irstHumidity, YH
+0000da80: 756d 6964 6974 792e 4669 6e64 4875 6d69  umidity.FindHumi
+0000da90: 6469 7479 292c 0a20 2020 2020 2020 2020  dity),.         
+0000daa0: 2020 2027 6c69 6768 7427 3a20 2859 4c69     'light': (YLi
+0000dab0: 6768 7453 656e 736f 722e 4669 7273 744c  ghtSensor.FirstL
+0000dac0: 6967 6874 5365 6e73 6f72 2c20 594c 6967  ightSensor, YLig
+0000dad0: 6874 5365 6e73 6f72 2e46 696e 644c 6967  htSensor.FindLig
+0000dae0: 6874 5365 6e73 6f72 290a 2020 2020 2020  htSensor).      
+0000daf0: 2020 7d0a 0a20 2020 2020 2020 2069 6620    }..        if 
+0000db00: 6e6f 7420 7461 7267 6574 3a0a 2020 2020  not target:.    
+0000db10: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0000db20: 6c75 6545 7272 6f72 2827 496e 7661 6c69  lueError('Invali
+0000db30: 6420 7461 7267 6574 2073 7065 6369 6669  d target specifi
+0000db40: 6564 2729 0a0a 2020 2020 2020 2020 7461  ed')..        ta
+0000db50: 7267 6574 7320 3d20 7461 7267 6574 2e73  rgets = target.s
+0000db60: 706c 6974 2827 2c27 2920 6966 2074 6172  plit(',') if tar
+0000db70: 6765 7420 213d 2027 616e 7927 2065 6c73  get != 'any' els
+0000db80: 6520 7365 6e73 6f72 5f6d 6170 7069 6e67  e sensor_mapping
+0000db90: 2e6b 6579 7328 290a 0a20 2020 2020 2020  .keys()..       
+0000dba0: 2066 6f72 2073 656e 736f 725f 7479 7065   for sensor_type
+0000dbb0: 2069 6e20 7461 7267 6574 733a 0a20 2020   in targets:.   
+0000dbc0: 2020 2020 2020 2020 2069 6620 7365 6e73           if sens
+0000dbd0: 6f72 5f74 7970 6520 6e6f 7420 696e 2073  or_type not in s
+0000dbe0: 656e 736f 725f 6d61 7070 696e 673a 0a20  ensor_mapping:. 
+0000dbf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000dc00: 656c 662e 6c6f 6767 6572 2e77 6172 6e69  elf.logger.warni
+0000dc10: 6e67 2866 2757 6172 6e69 6e67 3a20 556e  ng(f'Warning: Un
+0000dc20: 6b6e 6f77 6e20 7365 6e73 6f72 2074 7970  known sensor typ
+0000dc30: 6520 227b 7365 6e73 6f72 5f74 7970 657d  e "{sensor_type}
+0000dc40: 222e 2053 6b69 7070 696e 672e 2e2e 2729  ". Skipping...')
+0000dc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc60: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+0000dc70: 2020 2020 2020 2073 656e 736f 7220 3d20         sensor = 
+0000dc80: 7365 6e73 6f72 5f6d 6170 7069 6e67 5b73  sensor_mapping[s
+0000dc90: 656e 736f 725f 7479 7065 5d5b 305d 2829  ensor_type][0]()
+0000dca0: 2069 6620 7461 7267 6574 203d 3d20 2761   if target == 'a
+0000dcb0: 6e79 2720 656c 7365 2073 656e 736f 725f  ny' else sensor_
+0000dcc0: 6d61 7070 696e 675b 7365 6e73 6f72 5f74  mapping[sensor_t
+0000dcd0: 7970 655d 5b31 5d28 0a20 2020 2020 2020  ype][1](.       
+0000dce0: 2020 2020 2020 2020 2066 277b 7365 6e73           f'{sens
+0000dcf0: 6f72 5f74 7970 657d 2e7b 7365 6e73 6f72  or_type}.{sensor
+0000dd00: 5f74 7970 657d 2729 0a20 2020 2020 2020  _type}').       
+0000dd10: 2020 2020 2073 6574 6174 7472 2873 656c       setattr(sel
+0000dd20: 662c 2066 277b 7365 6e73 6f72 5f74 7970  f, f'{sensor_typ
+0000dd30: 657d 5f73 656e 736f 7227 2c20 7365 6e73  e}_sensor', sens
+0000dd40: 6f72 290a 0a20 2020 2020 2020 2069 6620  or)..        if 
+0000dd50: 6e6f 7420 616e 7928 6765 7461 7474 7228  not any(getattr(
+0000dd60: 7365 6c66 2c20 6627 7b73 656e 736f 725f  self, f'{sensor_
+0000dd70: 7479 7065 7d5f 7365 6e73 6f72 2729 2066  type}_sensor') f
+0000dd80: 6f72 2073 656e 736f 725f 7479 7065 2069  or sensor_type i
+0000dd90: 6e20 7461 7267 6574 7329 3a0a 2020 2020  n targets):.    
+0000dda0: 2020 2020 2020 2020 7261 6973 6520 4571          raise Eq
+0000ddb0: 7569 706d 656e 7445 7272 6f72 2827 4e6f  uipmentError('No
+0000ddc0: 206d 6f64 756c 6520 636f 6e6e 6563 7465   module connecte
+0000ddd0: 6427 290a 0a20 2020 2020 2020 2072 6574  d')..        ret
+0000dde0: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
+0000ddf0: 6620 6765 745f 7365 6e73 6f72 5f6e 616d  f get_sensor_nam
+0000de00: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
+0000de10: 2020 6e61 6d65 7320 3d20 5b5d 0a20 2020    names = [].   
+0000de20: 2020 2020 2066 6f72 2073 656e 736f 7220       for sensor 
+0000de30: 696e 205b 7365 6c66 2e74 656d 7065 7261  in [self.tempera
+0000de40: 7475 7265 5f73 656e 736f 722c 2073 656c  ture_sensor, sel
+0000de50: 662e 6875 6d69 6469 7479 5f73 656e 736f  f.humidity_senso
+0000de60: 722c 2073 656c 662e 6c69 6768 745f 7365  r, self.light_se
+0000de70: 6e73 6f72 5d3a 0a20 2020 2020 2020 2020  nsor]:.         
+0000de80: 2020 2069 6620 7365 6e73 6f72 3a0a 2020     if sensor:.  
+0000de90: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+0000dea0: 6d65 5f73 7472 203d 2073 656e 736f 722e  me_str = sensor.
+0000deb0: 6465 7363 7269 6265 2829 2e73 706c 6974  describe().split
+0000dec0: 2827 3d27 295b 315d 2e73 706c 6974 2827  ('=')[1].split('
+0000ded0: 2e27 295b 305d 0a20 2020 2020 2020 2020  .')[0].         
+0000dee0: 2020 2020 2020 206e 616d 6573 2e61 7070         names.app
+0000def0: 656e 6428 6e61 6d65 5f73 7472 290a 0a20  end(name_str).. 
+0000df00: 2020 2020 2020 2069 6620 6e6f 7420 6e61         if not na
+0000df10: 6d65 733a 0a20 2020 2020 2020 2020 2020  mes:.           
+0000df20: 2072 6169 7365 2045 7175 6970 6d65 6e74   raise Equipment
+0000df30: 4572 726f 7228 274e 6f20 7365 6e73 6f72  Error('No sensor
+0000df40: 2069 7320 636f 6e6e 6563 7465 642e 2054   is connected. T
+0000df50: 7279 2074 6f20 6361 6c6c 2063 6f6e 6e65  ry to call conne
+0000df60: 6374 2829 2066 6972 7374 2729 0a0a 2020  ct() first')..  
+0000df70: 2020 2020 2020 7265 7475 726e 206e 616d        return nam
+0000df80: 6573 0a0a 2020 2020 6465 6620 6765 745f  es..    def get_
+0000df90: 7465 6d70 6572 6174 7572 6528 7365 6c66  temperature(self
+0000dfa0: 293a 0a20 2020 2020 2020 2074 7279 3a0a  ):.        try:.
+0000dfb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000dfc0: 726e 2073 656c 662e 5f67 6574 5f73 656e  rn self._get_sen
+0000dfd0: 736f 725f 7661 6c75 6528 7365 6c66 2e74  sor_value(self.t
+0000dfe0: 656d 7065 7261 7475 7265 5f73 656e 736f  emperature_senso
+0000dff0: 722c 2027 7465 6d70 6572 6174 7572 6527  r, 'temperature'
+0000e000: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+0000e010: 2045 7863 6570 7469 6f6e 2061 7320 6565   Exception as ee
+0000e020: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000e030: 7475 726e 2030 0a0a 2020 2020 6465 6620  turn 0..    def 
+0000e040: 6765 745f 6875 6d69 6469 7479 2873 656c  get_humidity(sel
+0000e050: 6629 3a0a 2020 2020 2020 2020 7472 793a  f):.        try:
+0000e060: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e070: 7572 6e20 7365 6c66 2e5f 6765 745f 7365  urn self._get_se
+0000e080: 6e73 6f72 5f76 616c 7565 2873 656c 662e  nsor_value(self.
+0000e090: 6875 6d69 6469 7479 5f73 656e 736f 722c  humidity_sensor,
+0000e0a0: 2027 6875 6d69 6469 7479 2729 0a20 2020   'humidity').   
+0000e0b0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0000e0c0: 7074 696f 6e20 6173 2065 653a 0a20 2020  ption as ee:.   
+0000e0d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e0e0: 300a 0a20 2020 2064 6566 2067 6574 5f6c  0..    def get_l
+0000e0f0: 6967 6874 2873 656c 6629 3a0a 2020 2020  ight(self):.    
+0000e100: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000e110: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000e120: 2e5f 6765 745f 7365 6e73 6f72 5f76 616c  ._get_sensor_val
+0000e130: 7565 2873 656c 662e 6c69 6768 745f 7365  ue(self.light_se
+0000e140: 6e73 6f72 2c20 276c 6967 6874 2729 0a20  nsor, 'light'). 
+0000e150: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+0000e160: 6365 7074 696f 6e20 6173 2065 653a 0a20  ception as ee:. 
+0000e170: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e180: 6e20 300a 0a20 2020 2064 6566 205f 6765  n 0..    def _ge
+0000e190: 745f 7365 6e73 6f72 5f76 616c 7565 2873  t_sensor_value(s
+0000e1a0: 656c 662c 2073 656e 736f 722c 2073 656e  elf, sensor, sen
+0000e1b0: 736f 725f 7479 7065 293a 0a20 2020 2020  sor_type):.     
+0000e1c0: 2020 2069 6620 6e6f 7420 7365 6e73 6f72     if not sensor
+0000e1d0: 206f 7220 6e6f 7420 7365 6e73 6f72 2e69   or not sensor.i
+0000e1e0: 734f 6e6c 696e 6528 293a 0a20 2020 2020  sOnline():.     
+0000e1f0: 2020 2020 2020 2072 6169 7365 2045 7175         raise Equ
+0000e200: 6970 6d65 6e74 4572 726f 7228 6627 7b73  ipmentError(f'{s
+0000e210: 656e 736f 725f 7479 7065 2e63 6170 6974  ensor_type.capit
+0000e220: 616c 697a 6528 297d 2073 656e 736f 7220  alize()} sensor 
+0000e230: 6973 206e 6f74 2063 6f6e 6e65 6374 6564  is not connected
+0000e240: 2e20 5472 7920 746f 2063 616c 6c20 636f  . Try to call co
+0000e250: 6e6e 6563 7428 2920 6669 7273 7427 290a  nnect() first').
+0000e260: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000e270: 7365 6e73 6f72 2e67 6574 5f63 7572 7265  sensor.get_curre
+0000e280: 6e74 5661 6c75 6528 290a 0a20 2020 2064  ntValue()..    d
+0000e290: 6566 2063 616c 6962 7261 7469 6f6e 2873  ef calibration(s
+0000e2a0: 656c 662c 2072 6561 6c5f 7661 6c75 652c  elf, real_value,
+0000e2b0: 2063 616c 6962 5f62 6f6f 6c3d 5472 7565   calib_bool=True
+0000e2c0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000e2d0: 2020 2020 2020 2063 616c 6962 7261 7469         calibrati
+0000e2e0: 6f6e 2061 6e64 2063 616e 6365 6c20 6361  on and cancel ca
+0000e2f0: 6c69 6272 6174 696f 6e20 6675 6e63 7469  libration functi
+0000e300: 6f6e 2e0a 2020 2020 2020 2020 4070 6172  on..        @par
+0000e310: 616d 2063 616c 6962 5f62 6f6f 6c3a 2069  am calib_bool: i
+0000e320: 6620 5472 7565 2043 616c 6962 7261 7469  f True Calibrati
+0000e330: 6f6e 206f 7468 6572 7769 7365 2043 616e  on otherwise Can
+0000e340: 6365 6c20 4361 6c69 6272 6174 696f 6e0a  cel Calibration.
+0000e350: 2020 2020 2020 2020 4074 7970 6520 6361          @type ca
+0000e360: 6c69 625f 626f 6f6c 3a20 626f 6f6c 0a20  lib_bool: bool. 
+0000e370: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000e380: 2020 2069 6620 6361 6c69 625f 626f 6f6c     if calib_bool
+0000e390: 3a0a 2020 2020 2020 2020 2020 2020 7661  :.            va
+0000e3a0: 6c75 655f 6265 666f 7265 203d 205b 7365  lue_before = [se
+0000e3b0: 6c66 2e67 6574 5f6c 6967 6874 2829 5d0a  lf.get_light()].
+0000e3c0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+0000e3d0: 655f 6166 7465 7220 3d20 5b72 6561 6c5f  e_after = [real_
+0000e3e0: 7661 6c75 655d 0a20 2020 2020 2020 2065  value].        e
+0000e3f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000e400: 2076 616c 7565 5f62 6566 6f72 6520 3d20   value_before = 
+0000e410: 5b5d 0a20 2020 2020 2020 2020 2020 2076  [].            v
+0000e420: 616c 7565 5f61 6674 6572 203d 205b 5d0a  alue_after = [].
+0000e430: 2020 2020 2020 2020 6620 3d20 594c 6967          f = YLig
+0000e440: 6874 5365 6e73 6f72 2e46 6972 7374 4c69  htSensor.FirstLi
+0000e450: 6768 7453 656e 736f 7228 290a 2020 2020  ghtSensor().    
+0000e460: 2020 2020 662e 6361 6c69 6272 6174 6546      f.calibrateF
+0000e470: 726f 6d50 6f69 6e74 7328 7661 6c75 655f  romPoints(value_
+0000e480: 6265 666f 7265 2c20 7661 6c75 655f 6166  before, value_af
+0000e490: 7465 7229 0a20 2020 2020 2020 2066 2e67  ter).        f.g
+0000e4a0: 6574 5f6d 6f64 756c 6528 292e 7361 7665  et_module().save
+0000e4b0: 546f 466c 6173 6828 290a 0a20 2020 2064  ToFlash()..    d
+0000e4c0: 6566 2063 616c 6962 7261 7469 6f6e 5f70  ef calibration_p
+0000e4d0: 6f69 6e74 7328 7365 6c66 2c20 7265 616c  oints(self, real
+0000e4e0: 5f76 616c 7565 735f 6172 7261 792c 206d  _values_array, m
+0000e4f0: 6561 7375 7265 645f 7661 6c75 655f 6172  easured_value_ar
+0000e500: 7261 7929 3a0a 2020 2020 2020 2020 2222  ray):.        ""
+0000e510: 220a 2020 2020 2020 2020 5065 7266 6f72  ".        Perfor
+0000e520: 6d20 6361 6c69 6272 6174 696f 6e20 7573  m calibration us
+0000e530: 696e 6720 706f 696e 7473 3a20 6174 206c  ing points: at l
+0000e540: 6561 7374 2032 2e0a 2020 2020 2020 2020  east 2..        
+0000e550: 2222 220a 2020 2020 2020 2020 6966 206c  """.        if l
+0000e560: 656e 2872 6561 6c5f 7661 6c75 6573 5f61  en(real_values_a
+0000e570: 7272 6179 2920 213d 206c 656e 286d 6561  rray) != len(mea
+0000e580: 7375 7265 645f 7661 6c75 655f 6172 7261  sured_value_arra
+0000e590: 7929 2061 6e64 206c 656e 2872 6561 6c5f  y) and len(real_
+0000e5a0: 7661 6c75 6573 5f61 7272 6179 2920 3c20  values_array) < 
+0000e5b0: 323a 0a20 2020 2020 2020 2020 2020 2072  2:.            r
+0000e5c0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000e5d0: 2241 7272 6179 206d 7573 7420 6861 7665  "Array must have
+0000e5e0: 2061 6e20 6576 656e 206e 756d 6265 7220   an even number 
+0000e5f0: 6f66 2065 6c65 6d65 6e74 732e 2061 6e64  of elements. and
+0000e600: 206d 6f72 6520 7468 656e 2032 2073 616d   more then 2 sam
+0000e610: 706c 6573 2229 0a0a 2020 2020 2020 2020  ples")..        
+0000e620: 6620 3d20 594c 6967 6874 5365 6e73 6f72  f = YLightSensor
+0000e630: 2e46 6972 7374 4c69 6768 7453 656e 736f  .FirstLightSenso
+0000e640: 7228 290a 2020 2020 2020 2020 6966 206e  r().        if n
+0000e650: 6f74 2066 2e69 734f 6e6c 696e 6528 293a  ot f.isOnline():
+0000e660: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000e670: 7365 2045 7175 6970 6d65 6e74 4572 726f  se EquipmentErro
+0000e680: 7228 224c 6967 6874 2073 656e 736f 7220  r("Light sensor 
+0000e690: 6973 206e 6f74 2063 6f6e 6e65 6374 6564  is not connected
+0000e6a0: 2e22 290a 0a20 2020 2020 2020 2066 2e63  .")..        f.c
+0000e6b0: 616c 6962 7261 7465 4672 6f6d 506f 696e  alibrateFromPoin
+0000e6c0: 7473 286d 6561 7375 7265 645f 7661 6c75  ts(measured_valu
+0000e6d0: 655f 6172 7261 792c 2072 6561 6c5f 7661  e_array, real_va
+0000e6e0: 6c75 6573 5f61 7272 6179 290a 2020 2020  lues_array).    
+0000e6f0: 2020 2020 662e 6765 745f 6d6f 6475 6c65      f.get_module
+0000e700: 2829 2e73 6176 6554 6f46 6c61 7368 2829  ().saveToFlash()
+0000e710: 0a0a 2020 2020 6465 6620 6361 6c69 6272  ..    def calibr
+0000e720: 6174 696f 6e5f 6c69 6768 745f 706f 696e  ation_light_poin
+0000e730: 7428 7365 6c66 2c20 7661 6c29 3a0a 2020  t(self, val):.  
+0000e740: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000e750: 2020 4368 616e 6765 7320 7468 6520 7365    Changes the se
+0000e760: 6e73 6f72 2d73 7065 6369 6669 6320 6361  nsor-specific ca
+0000e770: 6c69 6272 6174 696f 6e20 7061 7261 6d65  libration parame
+0000e780: 7465 7220 736f 2074 6861 7420 7468 6520  ter so that the 
+0000e790: 6375 7272 656e 7420 7661 6c75 650a 2020  current value.  
+0000e7a0: 2020 2020 2020 6d61 7463 6865 7320 6120        matches a 
+0000e7b0: 6465 7369 7265 6420 7461 7267 6574 2028  desired target (
+0000e7c0: 6c69 6e65 6172 2073 6361 6c69 6e67 292e  linear scaling).
+0000e7d0: 0a0a 2020 2020 2020 2020 4070 6172 616d  ..        @param
+0000e7e0: 2063 616c 6962 7261 7465 6456 616c 203a   calibratedVal :
+0000e7f0: 2074 6865 2064 6573 6972 6564 2074 6172   the desired tar
+0000e800: 6765 7420 7661 6c75 652e 0a0a 2020 2020  get value...    
+0000e810: 2020 2020 5265 6d65 6d62 6572 2074 6f20      Remember to 
+0000e820: 6361 6c6c 2074 6865 2073 6176 6554 6f46  call the saveToF
+0000e830: 6c61 7368 2829 206d 6574 686f 6420 6f66  lash() method of
+0000e840: 2074 6865 206d 6f64 756c 6520 6966 2074   the module if t
+0000e850: 6865 0a20 2020 2020 2020 206d 6f64 6966  he.        modif
+0000e860: 6963 6174 696f 6e20 6d75 7374 2062 6520  ication must be 
+0000e870: 6b65 7074 2e0a 0a20 2020 2020 2020 2040  kept...        @
+0000e880: 7265 7475 726e 2059 4150 492e 5355 4343  return YAPI.SUCC
+0000e890: 4553 5320 6966 2074 6865 2063 616c 6c20  ESS if the call 
+0000e8a0: 7375 6363 6565 6473 2e0a 0a20 2020 2020  succeeds...     
+0000e8b0: 2020 204f 6e20 6661 696c 7572 652c 2074     On failure, t
+0000e8c0: 6872 6f77 7320 616e 2065 7863 6570 7469  hrows an excepti
+0000e8d0: 6f6e 206f 7220 7265 7475 726e 7320 6120  on or returns a 
+0000e8e0: 6e65 6761 7469 7665 2065 7272 6f72 2063  negative error c
+0000e8f0: 6f64 652e 0a20 2020 2020 2020 2022 2222  ode..        """
+0000e900: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000e910: 7365 6c66 2e6c 6967 6874 5f73 656e 736f  self.light_senso
+0000e920: 7220 6f72 206e 6f74 2073 656c 662e 6c69  r or not self.li
+0000e930: 6768 745f 7365 6e73 6f72 2e69 734f 6e6c  ght_sensor.isOnl
+0000e940: 696e 6528 293a 0a20 2020 2020 2020 2020  ine():.         
+0000e950: 2020 2072 6169 7365 2045 7175 6970 6d65     raise Equipme
+0000e960: 6e74 4572 726f 7228 224c 6967 6874 2073  ntError("Light s
+0000e970: 656e 736f 7220 6973 206e 6f74 2063 6f6e  ensor is not con
+0000e980: 6e65 6374 6564 2e22 290a 2020 2020 2020  nected.").      
+0000e990: 2020 7265 7475 726e 2073 656c 662e 6c69    return self.li
+0000e9a0: 6768 745f 7365 6e73 6f72 2e63 616c 6962  ght_sensor.calib
+0000e9b0: 7261 7465 2863 616c 6962 7261 7465 6456  rate(calibratedV
+0000e9c0: 616c 3d76 616c 290a 0a20 2020 2040 7374  al=val)..    @st
+0000e9d0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+0000e9e0: 6566 2065 7869 745f 6170 7028 293a 0a20  ef exit_app():. 
+0000e9f0: 2020 2020 2020 2059 4150 492e 4672 6565         YAPI.Free
+0000ea00: 4150 4928 290a 0a0a 6966 205f 5f6e 616d  API()...if __nam
+0000ea10: 655f 5f20 3d3d 2027 5f5f 6d61 696e 5f5f  e__ == '__main__
+0000ea20: 273a 0a20 2020 2070 7269 6e74 2827 636f  ':.    print('co
+0000ea30: 676e 6578 2073 6572 6961 6c27 290a 2020  gnex serial').  
+0000ea40: 2020 6320 3d20 436f 676e 6578 4461 7461    c = CognexData
+0000ea50: 4d61 6e28 290a 2020 2020 632e 7472 6967  Man().    c.trig
+0000ea60: 6765 725f 6f6e 2829 0a20 2020 2073 6361  ger_on().    sca
+0000ea70: 6e5f 7265 7375 6c74 7320 3d20 632e 7265  n_results = c.re
+0000ea80: 6164 5f62 6174 6368 2877 6169 745f 7469  ad_batch(wait_ti
+0000ea90: 6d65 3d30 2e35 290a 2020 2020 632e 7472  me=0.5).    c.tr
+0000eaa0: 6967 6765 725f 6f66 6628 290a 2020 2020  igger_off().    
+0000eab0: 7072 696e 7428 6627 7363 616e 5f72 6573  print(f'scan_res
+0000eac0: 756c 7473 3a20 7b73 6361 6e5f 7265 7375  ults: {scan_resu
+0000ead0: 6c74 737d 2729 0a20 2020 2063 2e74 7269  lts}').    c.tri
+0000eae0: 6767 6572 5f6f 6e28 636f 6e74 696e 756f  gger_on(continuo
+0000eaf0: 7573 6c79 3d54 7275 6529 0a20 2020 2073  usly=True).    s
+0000eb00: 6c65 6570 2835 290a 2020 2020 6578 5f69  leep(5).    ex_i
+0000eb10: 6420 3d20 632e 7265 6164 5f62 6174 6368  d = c.read_batch
+0000eb20: 2829 0a20 2020 2070 7269 6e74 2866 2763  ().    print(f'c
+0000eb30: 6f6e 7469 6e6f 7573 2073 6361 6e3a 207b  ontinous scan: {
+0000eb40: 6578 5f69 647d 2729 0a20 2020 2063 2e74  ex_id}').    c.t
+0000eb50: 7269 6767 6572 5f6f 6666 2829 0a20 2020  rigger_off().   
+0000eb60: 2063 2e63 6c6f 7365 5f70 6f72 7428 290a   c.close_port().
+0000eb70: 0a20 2020 2070 7269 6e74 2827 636f 676e  .    print('cogn
+0000eb80: 6578 206e 6574 776f 726b 2729 0a20 2020  ex network').   
+0000eb90: 2063 203d 2043 6f67 6e65 784e 6574 776f   c = CognexNetwo
+0000eba0: 726b 2869 705f 6164 6472 6573 733d 2731  rk(ip_address='1
+0000ebb0: 3732 2e32 362e 3431 2e32 3033 2729 0a20  72.26.41.203'). 
+0000ebc0: 2020 2063 2e74 7269 6767 6572 5f6f 6e28     c.trigger_on(
+0000ebd0: 636f 6e74 696e 756f 7573 6c79 3d54 7275  continuously=Tru
+0000ebe0: 6529 0a20 2020 2070 7269 6e74 2827 7761  e).    print('wa
+0000ebf0: 6974 2035 2073 6563 6f6e 6473 2074 6f20  it 5 seconds to 
+0000ec00: 7265 6365 6976 6520 6461 7461 2729 0a20  receive data'). 
+0000ec10: 2020 2073 6c65 6570 2835 290a 2020 2020     sleep(5).    
+0000ec20: 6578 5f69 6420 3d20 632e 7265 6164 5f62  ex_id = c.read_b
+0000ec30: 6174 6368 286e 5f6d 7367 3d31 3029 0a20  atch(n_msg=10). 
+0000ec40: 2020 2070 7269 6e74 2865 785f 6964 290a     print(ex_id).
+0000ec50: 2020 2020 632e 7472 6967 6765 725f 6f66      c.trigger_of
+0000ec60: 6628 290a 2020 2020 632e 636c 6f73 655f  f().    c.close_
+0000ec70: 706f 7274 2829 0a20 2020 2070 7269 6e74  port().    print
+0000ec80: 2827 646f 6e65 2729 0a                   ('done').
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/tester_utils.py` & `wiliot-testers-5.4.13/wiliot_testers/tester_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/upload_testers_data_to_cloud.py` & `wiliot-testers-5.4.13/wiliot_testers/upload_testers_data_to_cloud.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/utils/Install PPFP.bat` & `wiliot-testers-5.4.13/wiliot_testers/utils/Install PPFP.bat`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/utils/get_version.py` & `wiliot-testers-5.4.13/wiliot_testers/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/utils/ppfp_tool.py` & `wiliot-testers-5.4.13/wiliot_testers/utils/ppfp_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/utils/upload_to_cloud_api.py` & `wiliot-testers-5.4.13/wiliot_testers/utils/upload_to_cloud_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/utils/wiliot_external_ids.py` & `wiliot-testers-5.4.13/wiliot_testers/utils/wiliot_external_ids.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/wiliot_tester_log.py` & `wiliot-testers-5.4.13/wiliot_testers/wiliot_tester_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,14 @@
         self.run_header = []
         self.packets_header = []
         self.run_data_name = ''
         self.packets_data_name = ''
         self.run_data_path = ''
         self.packets_data_path = ''
         self.data_folder = ''
-        self.run_name = ''
         self.run_start_time = ''
         self.tester_station_name = ''
 
     def set_logger(self, log_path=None, tester_name='tester'):
         ''' Sets the logger if doesn't exist from main code - INFO level
         3 loggers declared
         self.logger - our main for packet
@@ -226,14 +225,15 @@
     @staticmethod
     def set_console_handler_level(logger, level):
         for handler in logger.handlers:
             original_formatter = handler.formatter  # Store the original formatter
             handler.setLevel(level)
             handler.setFormatter(original_formatter)  # Re-apply the original formatter
 
+
 def dict_to_csv(dict_in, path, append=False, only_titles=False):
     if append:
         method = 'a'
     else:
         method = 'w'
     with open(path, method, newline='') as f:
         dict_writer = DictWriter(f, fieldnames=dict_in.keys())
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/wiliot_tester_tag_result.py` & `wiliot-testers-5.4.13/wiliot_testers/wiliot_tester_tag_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         """
         check if all sub test passed (i.e. the whole test passed)
         :return:
         :rtype:
         """
         if self.is_results_empty():
             return None
-        return self.tests[-1].is_test_passed
+        return self.tests[-1].is_test_passed if self.status is None else self.status
 
     def get_total_test_duration(self):
         if self.is_results_empty():
             return None
         return (self.tests[-1].test_end - self.trigger_time).total_seconds()
     
     def get_total_fail_bin(self, as_name=False):
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/wiliot_tester_tag_test.py` & `wiliot-testers-5.4.13/wiliot_testers/wiliot_tester_tag_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 import pandas as pd
 import numpy as np
 
 from wiliot_core import WiliotDir
 from wiliot_core import WiliotGateway, ActionType, DataType, valid_output_power_vals
 from wiliot_core import PacketList
 from wiliot_testers.wiliot_tester_tag_result import WiliotTesterTagResultList, WiliotTesterTagResult, FailureCodes
+from wiliot_testers.wiliot_tester_log import WiliotTesterLog
 
 try:
     from wiliot_core import DecryptedPacketList, DecryptedPacket
     print('tag test: decryption mode is supported if needed')
 except Exception as e:
     pass
 
@@ -99,15 +100,15 @@
     """
     Wiliot Tags Tester according to configurations provided by user
     """
 
     def __init__(self, selected_test, test_suite=None, gw_obj=None, black_list=None,
                  stop_event_trig=None, tester_name=TesterName.OFFLINE,
                  logger_name=None, logger_result_name=None, logger_gw_name=None,
-                 lock_print=None, inlay=None, verbose=True):  # TODO add selected test dict
+                 lock_print=None, inlay=None, verbose=True):
         """
         :param logger_name: if specified the main logger is based on a predefine logger with the specified name.
                             otherwise the logger is set by the app
         :type logger_name: str
         :param logger_result_name: if specified the results logger is based on a predefine logger with the
                                    specified name. otherwise the logger is set by the app
         :type logger_result_name: str
@@ -463,16 +464,14 @@
         select which tag is under test even if more than one tag sends packets
         :param optional_tags: all tags that transmits during the tag-test
         :type optional_tags: list
         :return: the packet list of the selected tag under test
         :rtype: PacketList or DecryptedPacketList
         """
         selected_adva = None
-        self.tag_results.all_tags = self.tag_results.add_packets_to_multi_tags(packets_in=self.tag_results.all_packets,
-                                                                               multi_tag_out=self.tag_results.all_tags)
         self._printing_func('Starting to decide which tag is under test')
         optional_tags = list(set(optional_tags))
         if len(optional_tags) == 0:
             selected_adva = ''
         elif len(optional_tags) == 1:
             selected_adva = optional_tags[0]
             self.tag_results.selected_tag = self.tag_results.all_tags.tags[selected_adva]
@@ -526,32 +525,36 @@
             packets_received_list = self.GwObj.get_packets(action_type=ActionType.ALL_SAMPLE,
                                                            data_type=data_type,
                                                            tag_inlay=self.selected_test['inlay'])
         if packets_received_list:
             if packets_received_list.size() > 1:
                 self._printing_func('pulled more than one packet from the queue, check analysis performance')
 
-            self._printing_func('got {} packets'.format(
-                ['ADVA:' + p.get_adva() + ',    FLOW:' + p.get_flow() + ',    RSSI:' +
-                 p.get_rssi() + ',    ' + p.get_packet_string() for p in packets_received_list]),
-                log_level=logging.DEBUG)
+            self.print_packets(packets_received_list)
             filtered_packets = self.packet_filter(packets_received_list, filter_param=filter_param,
                                                   param_limits=[0, filter_value],
                                                   ignore_test_mode_packet=self.selected_test['ignore_test_mode'])
             self.tag_results.all_packets.__add__(packets_received_list)
             if filtered_packets.size():
                 self.tag_results.filtered_tags = \
                     self.tag_results.add_packets_to_multi_tags(filtered_packets, self.tag_results.filtered_tags)
-                self._printing_func('and {} pass the packet filter'.format(
-                    ['ADVA:' + p.get_adva() + ',    FLOW:' + p.get_flow() + ',    RSSI:' + p.get_rssi() + ',    ' +
-                     p.get_packet_string() for p in packets_received_list]), log_level=logging.DEBUG)
+                self.print_packets(packets_received_list, 'pass the packet filter')
             return True
         else:
             return False
 
+    def print_packets(self, packets_received_list, last_str = 'received packets'):
+        for p in packets_received_list:
+            packet_print = (f'ADVA:{p.get_adva()},    FLOW:{p.get_flow()},    RSSI:{p.get_rssi()},    '
+                            f'{p.get_packet_string()}')
+            self._printing_func(f'{packet_print} {last_str}', log_level=logging.DEBUG)
+
+    def is_stop_criteria_reached(self, tags_reached_criteria):
+        return len(tags_reached_criteria) > 0
+
     def check_stop_criteria(self, stop_criteria_dict=None, check_type='general'):
         """
         check if the received packet met the stop criteria and the test should be stopped
         :param stop_criteria_dict: dictionary according to the test suite definition, (e.g. {"num_packets": [1, 99]})
         :type stop_criteria_dict: dict
         :param check_type: specified the type of stop criteria to improve performance
         :type check_type: str
@@ -579,14 +582,15 @@
                 tags_stat_df = pd.concat([tags_stat_df, tag_id_df], axis=0)
         else:
             tags_stat_df = self.tag_results.filtered_tags.get_statistics()
         tags_reached_criteria = []
         if tags_stat_df.size > 0:
             for _, tag in tags_stat_df.iterrows():
                 try:
+                    self.logger.debug(f'check {[(k, tag.get(k, None)) for k in stop_criteria_dict.keys()]}')
                     criteria_status = [v[0] <= tag[k] <= v[-1] if k in tag.keys() and not pd.isnull(tag[k]) else False
                                        for k, v in stop_criteria_dict.items()]
                     if all(criteria_status):
                         tags_reached_criteria.append(tag['adv_address'] if 'adv_address' in tag.keys() else
                                                      tag['tag_id'])
                 except Exception as e:
                     raise e
@@ -665,29 +669,42 @@
             self.tag_results.set_quality_test_failure(test_param['quality_param'], targets_status)
 
         else:
             targets_status = [True]
 
         return all(targets_status)
 
-    def init_gw_test(self, sub_test, is_start_gw_app=True):
+    def init_gw_test(self, sub_test=None, is_start_gw_app=True):
         # Config GW according to Test Suite
         self.GwObj.reset_listener()
+        if sub_test is None:
+            sub_test = self.selected_test['tests'][0]
         is_gw_commands = 'gw_commands' in sub_test
-        self.GwObj.config_gw(energy_pattern_val=sub_test['energizingPattern'],
-                             received_channel=int(sub_test['rxChannel']),
-                             time_profile_val=sub_test['timeProfile'],
-                             output_power_val=sub_test['gw_power_dict']['gw_output_power'],
-                             bypass_pa_val=sub_test['gw_power_dict']['bypass_pa'],
-                             sub1g_output_power_val=sub_test['sub1g_power'],
-                             start_gw_app=is_start_gw_app and not is_gw_commands, with_ack=True, combined_msg=False)
+        _, gw_rsps = self.GwObj.config_gw(energy_pattern_val=sub_test['energizingPattern'],
+                                          received_channel=int(sub_test['rxChannel']),
+                                          time_profile_val=sub_test['timeProfile'],
+                                          output_power_val=sub_test['gw_power_dict']['gw_output_power'],
+                                          bypass_pa_val=sub_test['gw_power_dict']['bypass_pa'],
+                                          sub1g_output_power_val=sub_test['sub1g_power'],
+                                          start_gw_app=is_start_gw_app and not is_gw_commands,
+                                          with_ack=True, combined_msg=False)
+        gw_rsp_c = []
         if is_gw_commands:
             for cmd in sub_test['gw_commands']:
-                self.GwObj.write(cmd=cmd, with_ack=True)
-            self.GwObj.config_gw(start_gw_app=is_start_gw_app, with_ack=True)
+                gw_rsp = self.GwObj.write(cmd=cmd, with_ack=True)
+                gw_rsp['command'] = cmd
+                gw_rsps.append(gw_rsp)
+            _, gw_rsp_c = self.GwObj.config_gw(start_gw_app=is_start_gw_app, with_ack=True)
+
+        gw_rsps += gw_rsp_c
+        for gw_rsp in gw_rsps:
+            if not self.GwObj.is_command_acknowledged(cmd=gw_rsp['command'], rsp=gw_rsp['raw']):
+                err = f'WiliotTesterTagTest: Gateway did not response: cmd:{gw_rsp["command"]}, rsp:{gw_rsp["raw"]}'
+                self.logger.error(err)
+                raise Exception(err)
 
     def init_test(self, sub_test, is_start_gw_app=True, test_num=0):
         """
         initialize the test
         :param sub_test: the test parameter according to the test suite definition
         :type sub_test: dict
         :param is_start_gw_app: if True, the gw starts its application (transmit and receive)
@@ -843,14 +860,15 @@
 
         self.test_results.set_trigger_time()
 
         # Test begins
         self._printing_func('Trigger received')
 
         num_of_tests = len(self.selected_test['tests'])
+        all_selected_tags = []
         for test_num in range(num_of_tests):
             sub_test = self.selected_test['tests'][test_num]
 
             test_check_type = self.check_type_per_test(sub_test['stop_criteria'])
 
             # init sub-test
             self._printing_func('---------------------Started stage {} out of {} stages-----------------------'.
@@ -877,106 +895,66 @@
                                                       data_type=data_type)
                 if is_received_packet:
                     self.reset_timers(only_first_packet_timer=True)
                     # check if we reached stop criteria:
                     tags_reached_criteria = self.check_stop_criteria(stop_criteria_dict=sub_test['stop_criteria'],
                                                                      check_type=test_check_type)
 
-                    if len(tags_reached_criteria):
+                    if self.is_stop_criteria_reached(tags_reached_criteria):
                         self._printing_func('test reached stop criteria - starting to analyze the results')
                         self.test_end = True
                 else:
                     time.sleep(0)  # allow time for recovery
                     # check if GW ERROR occurred and fix it:
                     if self.is_gw_fetal_error():
                         self.logger_results.warning('gw fetal error was detected')
                         if not self.GwObj.is_connected():
                             raise Exception('Could not reconnect to the GW. please check connections')
                         self.gw_reset_and_config()
                         self.init_gw_test(sub_test=sub_test, is_start_gw_app=True)
                         self.tag_results.test_status = FailureCodes.GW_ERROR
 
+            # reset timers:
+            self.reset_timers()
             # stop gw from transmitting
             is_stopped = self.GwObj.stop_gw_app()
             if not is_stopped:
                 self.logger_results.warning('could not stop GW app')
-                self.gw_reset_and_config()
-                self.init_gw_test(sub_test=sub_test, is_start_gw_app=True)
+                raise Exception('could not stop GW app')
 
             # check again stop criteria:
             tags_reached_criteria = self.check_stop_criteria(stop_criteria_dict=sub_test['stop_criteria'],
                                                              check_type=test_check_type)
-            if len(tags_reached_criteria) and not self.test_end:
+            if self.is_stop_criteria_reached(tags_reached_criteria) and not self.test_end:
                 self._printing_func('test reached stop criteria just before time expired')
                 self.test_end = True
 
-            # check why the test is over
-            if self.is_stopped_by_user():  # Stop event was triggered
-                self._printing_func('Stop was triggered')
-                self._printing_func('Tag marked as Fail', logger_name=LoggerName.RESULTS)
-                self.reset_timers()
-                self.tag_results.test_status = FailureCodes.STOP_BY_USER
-                self.test_results.append(self.tag_results)
+            # update results:
+            self.tag_results.all_tags = self.tag_results.add_packets_to_multi_tags(
+                packets_in=self.tag_results.all_packets,
+                multi_tag_out=self.tag_results.all_tags)
 
-            elif self.test_end or sub_test['stop_criteria'] == {}:
-                if sub_test['stop_criteria'] != {}:
-                    selected_tag = self.select_tag_under_test(optional_tags=tags_reached_criteria)  # Get the best tag
-                else:
-                    all_optional_tags = list(self.tag_results.filtered_tags.tags.keys())
-                    selected_tag = self.select_tag_under_test(optional_tags=all_optional_tags)  # Get the best tag
-
-                all_selected_tags = self.test_results.get_test_unique_adva()
-                is_diff_tag_btwn_sub_tests = selected_tag not in all_selected_tags and len(all_selected_tags) > 0
-                if selected_tag and not is_diff_tag_btwn_sub_tests:
-                    self._printing_func('Tag {} was selected'.format(selected_tag))
-                    # selected tag performance:
-                    self.tag_results.is_test_passed = self.statistics_analyzer(test_param=sub_test, test_num=test_num)
-                    if self.tag_results.is_test_passed:
-                        self.tag_results.test_status = FailureCodes.PASS
-                        self._printing_func('Stage {} out of {} Passed'.format(test_num + 1, num_of_tests),
-                                            logger_name=LoggerName.RESULTS)
-                    else:
-                        self._printing_func('Tag failed quality test', logger_name=LoggerName.RESULTS,
-                                            log_level=logging.DEBUG)
-                        self._printing_func('Stage {} out of {} Failed'.format(test_num + 1, num_of_tests),
-                                            logger_name=LoggerName.RESULTS)
-                elif selected_tag == '':
-                    self.tag_results.test_status = FailureCodes.NO_RESPONSE
-                    self._printing_func("No Responds during run_all mode")
-                else:  # selected_tag is None:
-                    self.tag_results.test_status = FailureCodes.SEVERAL_TAGS_UNDER_TEST
-                    self._printing_func("Couldn't decide which tag transmitting, it will fail")
-
-                self.reset_timers()
-                self.test_results.append(self.tag_results)
+            # check why the test is over
+            if self.test_end or sub_test['stop_criteria'] == {}:
+                self.analyze_end_of_test(sub_test, tags_reached_criteria, all_selected_tags, test_num, num_of_tests)
 
             elif self.time_expired:  # time expired before reaching stop criteria
-                # check again stop criteria:
+                self.analyze_time_expired(test_num)
 
-                self._printing_func('Stage {} Failed - Timeout'.format(test_num + 1),
-                                    logger_name=LoggerName.RESULTS)
-                if self.tag_results.test_status == FailureCodes.GW_ERROR:
-                    pass
-                elif self.tag_results.all_packets.size() == 0:
-                    self.tag_results.test_status = FailureCodes.NO_RESPONSE
-                elif len(self.tag_results.filtered_tags) == 0:
-                    self.tag_results.test_status = FailureCodes.NO_PACKETS_UNDER_RSSI_THR
-                else:
-                    self.tag_results.all_tags = self.tag_results.add_packets_to_multi_tags(
-                        packets_in=self.tag_results.all_packets,
-                        multi_tag_out=self.tag_results.all_tags)
-                    self.tag_results.test_status = FailureCodes.NOT_ENOUGH_PACKETS
-                self.test_results.append(self.tag_results)
+            elif self.is_stopped_by_user():  # Stop event was triggered
+                self._printing_func('Stop was triggered')
+                self._printing_func('Tag marked as Fail', logger_name=LoggerName.RESULTS)
+                self.tag_results.test_status = FailureCodes.STOP_BY_USER
 
             else:
-                self.reset_timers()
                 msg = 'test was stopped due to unknown reason'
                 self._printing_func(msg, log_level=logging.WARNING)
                 raise Exception('test was stopped due to unknown reason')
 
+            self.test_results.append(self.tag_results)
             # check if delays between stages/sub-test
             if 'delayBeforeNextTest' in sub_test:
                 self._printing_func('Going to sleep for {} second '.format(sub_test['delayBeforeNextTest']))
                 t_i = datetime.datetime.now()
                 dt = datetime.datetime.now() - t_i
                 while dt.total_seconds() < float(sub_test['delayBeforeNextTest']):
                     dt = datetime.datetime.now() - t_i
@@ -984,17 +962,63 @@
             self.tag_results.test_end = datetime.datetime.now()
             if self.tag_results.test_status != FailureCodes.PASS and not self.run_all:
                 break  # stop the test if one of the stages was failed
 
         # prepare gw for the next run:
         if num_of_tests > 1:
             self.init_gw_test(sub_test=self.selected_test['tests'][0], is_start_gw_app=False)
-        self.reset_timers()
         return self.test_results
 
+    def analyze_end_of_test(self, sub_test, tags_reached_criteria, all_selected_tags, test_num, num_of_tests):
+        if sub_test['stop_criteria'] != {}:
+            selected_test_tag = self.select_tag_under_test(optional_tags=tags_reached_criteria)  # Get the best tag
+        else:
+            all_optional_tags = list(self.tag_results.filtered_tags.tags.keys())
+            selected_test_tag = self.select_tag_under_test(optional_tags=all_optional_tags)  # Get the best tag
+
+        # check selected tag on all previous tests
+        if selected_test_tag and selected_test_tag not in all_selected_tags:
+            is_diff_tag_btwn_sub_tests = len(all_selected_tags) > 0
+            all_selected_tags.append(selected_test_tag)
+        else:
+            is_diff_tag_btwn_sub_tests = False
+
+        if not is_diff_tag_btwn_sub_tests and len(all_selected_tags) > 0:
+            self._printing_func('Tag {} was selected'.format(selected_test_tag))
+            # selected tag performance:
+
+            self.tag_results.is_test_passed = self.statistics_analyzer(test_param=sub_test, test_num=test_num)
+            if self.tag_results.is_test_passed:
+                self.tag_results.test_status = FailureCodes.PASS
+                self._printing_func('Stage {} out of {} Passed'.format(test_num + 1, num_of_tests),
+                                    logger_name=LoggerName.RESULTS)
+            else:
+                self._printing_func('Tag failed quality test', logger_name=LoggerName.RESULTS,
+                                    log_level=logging.DEBUG)
+                self._printing_func('Stage {} out of {} Failed'.format(test_num + 1, num_of_tests),
+                                    logger_name=LoggerName.RESULTS)
+        elif selected_test_tag == '':
+            self.tag_results.test_status = FailureCodes.NO_RESPONSE
+            self._printing_func("No Responds during run_all mode")
+        else:  # selected_test_tag is None:
+            self.tag_results.test_status = FailureCodes.SEVERAL_TAGS_UNDER_TEST
+            self._printing_func("Couldn't decide which tag transmitting, it will fail")
+
+    def analyze_time_expired(self, test_num):
+        self._printing_func('Stage {} Failed - Timeout'.format(test_num + 1),
+                            logger_name=LoggerName.RESULTS)
+        if self.tag_results.test_status == FailureCodes.GW_ERROR:
+            pass
+        elif self.tag_results.all_packets.size() == 0:
+            self.tag_results.test_status = FailureCodes.NO_RESPONSE
+        elif len(self.tag_results.filtered_tags) == 0:
+            self.tag_results.test_status = FailureCodes.NO_PACKETS_UNDER_RSSI_THR
+        else:
+            self.tag_results.test_status = FailureCodes.NOT_ENOUGH_PACKETS
+
     def exit_tag_test(self, need_to_close_port=True):
         self.reset_timers()
         if need_to_close_port:
             self.GwObj.close_port(is_reset=True)
             self.GwObj.exit_gw_api()
         else:
             self.GwObj.reset_gw()
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers/yield_tester/arduino_counter/arduino_counter.ino` & `wiliot-testers-5.4.13/wiliot_testers/yield_tester/arduino_counter/arduino_counter.ino`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/yield_tester/configs/inlay_data.py` & `wiliot-testers-5.4.13/wiliot_testers/yield_tester/configs/inlay_data.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/yield_tester/from_listener_log_to_csv.py` & `wiliot-testers-5.4.13/wiliot_testers/yield_tester/from_listener_log_to_csv.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/yield_tester/simulation/gw_arduino_simulation/gw_arduino_simulation.ino` & `wiliot-testers-5.4.13/wiliot_testers/yield_tester/simulation/gw_arduino_simulation/gw_arduino_simulation.ino`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/yield_tester/simulation/yield_simulation_utils.py` & `wiliot-testers-5.4.13/wiliot_testers/yield_tester/simulation/yield_simulation_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/yield_tester/trigger_miss_catcher.py` & `wiliot-testers-5.4.13/wiliot_testers/yield_tester/trigger_miss_catcher.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/yield_tester/utils/get_arduino_ports.py` & `wiliot-testers-5.4.13/wiliot_testers/yield_tester/utils/get_arduino_ports.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-5.3.9/wiliot_testers/yield_tester/yield_tester.py` & `wiliot-testers-5.4.13/wiliot_testers/yield_tester/yield_tester.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,24 +53,15 @@
 #     FOR ANY LOSS OF USE OR DATA OR BUSINESS INTERRUPTION, AND/OR FOR ANY ECONOMIC LOSS
 #     (SUCH AS LOST PROFITS, REVENUE, ANTICIPATED SAVINGS). THE FOREGOING SHALL APPLY:
 #     (A) HOWEVER CAUSED AND REGARDLESS OF THE THEORY OR BASIS LIABILITY, WHETHER IN
 #     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
-"""
-Calculating Yield fraction by the following steps (with elaboration):
-1)Counting the unique advas in AdvaProcess class
-2)Counting number of tags in CountThread
-3)Creating two threads in MultiThreadingCalculation in order to run AdvaProcess instance and CountThread instance
-at the same time
-4)Calculating the Yield fraction according to the results we got from the instances
-5)Creating two threads in MainWindow class in order to calculate the fraction by MultiThreadingCalculation instance
-and to run the GUI function (open_session) at the same time.
-"""
+
 import sys
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from wiliot_core import *
 from wiliot_testers.test_equipment import YoctoSensor
 from configs.inlay_data import csv_dictionary
 
 import serial
@@ -84,57 +75,62 @@
 import json
 import matplotlib.pyplot as plt
 
 from wiliot_testers.utils.get_version import get_version
 from wiliot_testers.utils.upload_to_cloud_api import upload_to_cloud_api
 from wiliot_testers.yield_tester.simulation.yield_simulation_utils import get_simulated_gw_port, \
     AUTO_TRIGGERS, AUTO_PACKET, TIME_BETWEEN_AUTO_TRIGGERS
-from wiliot_testers.yield_tester.utils.get_arduino_ports import get_arduino_ports
 
 SECONDS_WITHOUT_PACKETS = 60
 SECONDS_FOR_GW_ERROR_AFTER_NO_PACKETS = 120
+TIME_BETWEEN_MATRICES = 3
 RED_COLOR = 'red'
 BLACK_COLOR = 'black'
 SET_VALUE_MORE_THAN_100 = 110
 VALUE_WHEN_NO_SENSOR = -10000
 MIN_Y_FOR_PLOTS = 0
 MAX_Y_FOR_PLOTS = 112
 FIRST_STEP_SIZE = 10
-BAUD_ARDUINO = 1000000
-MAND_FIELDS = ['wafer_lot', 'wafer_num', 'matrix_sec', 'matrix_num', 'thermodes_col',
+MAND_FIELDS = ['wafer_lot', 'wafer_num', 'matrix_num', 'thermodes_col',
                'rows_number']  # mandatory fields in GUI before the run
 PACKET_DATA_FEATURES_TITLE = [
     'raw_packet', 'adv_address', 'decrypted_packet_type', 'group_id',
     'flow_ver', 'test_mode', 'en', 'type', 'data_uid', 'nonce', 'enc_uid',
     'mic', 'enc_payload', 'gw_packet', 'rssi', 'stat_param', 'time_from_start',
     'counter_tag', 'is_valid_tag_packet', 'gw_process', 'is_valid_packet', 'inlay_type'
 ]
 
 script_dir = os.path.dirname(__file__)
 json_file_path = os.path.join(script_dir, 'configs', 'user_inputs.json')
+default_user_inputs = {
+    "min_cumulative": "60",
+    "min_cumulative_line": "yes",
+    "min_current": "20",
+    "min_current_line": "yes",
+    "max_temperature": "40",
+    "min_temperature": "10",
+    "temperature_type": "C",
+    "min_humidity": "20",
+    "max_humidity": "90",
+    "min_light_intensity": "0",
+    "max_light_intensity": "1500",
+    "red_line_cumulative": "85",
+    "red_line_current": "50",
+    "pin_number": "004"
+}
 try:
-
     with open(json_file_path) as f:
         user_inputs = json.load(f)
+    for key, value in default_user_inputs.items():
+        if key not in user_inputs:
+            user_inputs[key] = value
+    with open(json_file_path, 'w') as f:
+        json.dump(user_inputs, f, indent=4)
 except Exception as e:
-    user_inputs = {
-        "min_cumulative": "60",
-        "min_cumulative_line": "yes",
-        "min_current": "20",
-        "min_current_line": "yes",
-        "max_temperature": "40",
-        "min_temperature": "10",
-        "temperature_type": "C",
-        "min_humidity": "20",
-        "max_humidity": "90",
-        "min_light_intensity": "0",
-        "max_light_intensity": "1500",
-        "red_line_cumulative": "85",
-        "red_line_current": "50"
-    }
+    user_inputs = default_user_inputs
     os.makedirs(os.path.dirname(json_file_path), exist_ok=True)
     with open(json_file_path, 'w') as f:
         json.dump(user_inputs, f, indent=4)
 
 matplotlib.use('TkAgg')
 inlay_types_dict = {item.name: item.value for item in InlayTypes}
 today = datetime.date.today()
@@ -168,14 +164,16 @@
         self.all_tags = Queue()
         self.advas_before_tags = advas_before_tags
         self.stop = stop_event
         self.received_channel = received_channel
         self.gw_start_time = datetime.datetime.now()
         self.init_gw(listener_path)
         self.time_profile_val = ''
+        self.last_change_time = datetime.datetime.now()
+        self.number_of_sensor_triggers = 0
         try:
             self.time_profile_val = [int(time_pr) for time_pr in time_profile_val]
         except Exception as ee:
             raise Exception(f'could not retireive time profile from inlay_data value for {inlay_type}.\n'
                             f'time profile should be x,y but was {time_profile_val} [{ee}]')
         self.energy_pattern_val = energy_pattern_val
         self.inlay_type = inlay_type
@@ -209,17 +207,23 @@
 
         except Exception as ee:
             raise Exception(f"Couldn't connect to GW in main thread, error: {ee}")
 
     def get_gw_start_time(self):
         return self.gw_start_time
 
+    def get_last_change_time(self):
+        return self.last_change_time
+
     def get_gw_error_connection(self):
         return self.gw_error_connection
 
+    def get_sensors_triggers(self):
+        return self.number_of_sensor_triggers
+
     def gw_reset_config(self, start_gw_app=False):
         """
         Configs the gateway
         """
         if self.gw_instance.connected:
             self.gw_instance.reset_gw()
             self.gw_instance.reset_listener()
@@ -227,35 +231,56 @@
             if not self.gw_instance.is_gw_alive():
                 self.logger_file.warning('gw_reset_and_config: gw did not respond')
                 raise Exception('gw_reset_and_config: gw did not respond after rest')
             self.gw_instance.config_gw(received_channel=self.received_channel, time_profile_val=self.time_profile_val,
                                        energy_pattern_val=self.energy_pattern_val,
                                        start_gw_app=start_gw_app, with_ack=True,
                                        effective_output_power_val=22, sub1g_output_power_val=29, max_wait=400)
+            if not AUTO_TRIGGERS:
+                pin_num = user_inputs.get('pin_number')
+                cmd = '!cmd_gpio CONTROL_IN P%s 0' % pin_num.zfill(3)
+                self.gw_instance.write(cmd)
         else:
             raise Exception('Could NOT connect to GW')
 
+    def raising_trigger_number(self):
+        self.number_of_sensor_triggers += 1
+        self.last_change_time = datetime.datetime.now()
+
     def run(self):
         """
         Receives available data then counts and returns the number of unique advas.
         """
         self.gw_instance.config_gw(start_gw_app=True, max_wait=400)
         self.gw_instance.reset_start_time()
         self.gw_start_time = datetime.datetime.now()
         got_new_adva = False
         no_data_start_time = None  # Time when we first detect no data available
 
         while not self.stop.is_set():
+
+            if self.gw_instance.is_rsp_available():
+                # check if GW response is a new matrix
+                gw_rsp = self.gw_instance.get_gw_rsp()
+                current_time_of_data = datetime.datetime.now()
+                needed_time = TIME_BETWEEN_AUTO_TRIGGERS if AUTO_TRIGGERS else TIME_BETWEEN_MATRICES
+                if (current_time_of_data - self.last_change_time).total_seconds() >= needed_time:
+                    if AUTO_TRIGGERS:
+                        self.raising_trigger_number()
+                    elif gw_rsp is not None:
+                        if 'Detected High-to-Low peak' in gw_rsp['raw'] or \
+                                'Detected Low-to-High peak' in gw_rsp['raw']:
+                            self.raising_trigger_number()
+
             if self.gw_instance.is_data_available():
                 raw_packets_in = self.gw_instance.get_packets(action_type=ActionType.ALL_SAMPLE,
                                                               data_type=DataType.RAW, tag_inlay=self.inlay_type)
                 self.all_tags.put(raw_packets_in)
                 got_new_adva = True
                 no_data_start_time = None
-
             else:
                 if no_data_start_time is None:
                     no_data_start_time = time.time()
                 if time.time() - no_data_start_time >= SECONDS_WITHOUT_PACKETS:
                     got_new_adva = False
                     if not self.second_without_packets:
                         self.logger_file.warning("One minute without packets..")
@@ -283,118 +308,20 @@
     def get_raw_packets_queue(self):
         """
         Returns the packet queue that is created above
         """
         return self.all_tags
 
 
-class CountThread(object):
-    """
-    Counting the number of tags
-    """
-
-    def __init__(self, stop_event, logger_file, matrix_size=1, max_movement_time=3, ther_cols=1):
-        self.arduino_connection_error = False
-        self.max_movement_time = max_movement_time
-        self.logger_file = logger_file
-        self.last_arduino_trigger_time = datetime.datetime.now()
-        self.comPortObj = None
-        self.trigger_port = None
-        if not AUTO_TRIGGERS:
-            self.connect()
-        self.matrix_size = matrix_size
-        self.ther_cols = ther_cols
-        self.stop = stop_event
-        self.tested = 0
-
-    def connect(self):
-        optional_ports = get_arduino_ports()
-        if len(optional_ports) == 0:
-            raise Exception("NO ARDUINO")
-        for port in optional_ports:
-            try:
-                self.comPortObj = serial.Serial(port, BAUD_ARDUINO, timeout=0.1)
-                time.sleep(2)
-                initial_message = self.comPortObj.readline().decode().strip()
-                if "Wiliot Yield Counter" in initial_message:
-                    self.trigger_port = port
-            except Exception as e:
-                raise Exception(f'could not connect to port {port} due to {e}')
-
-    def raising_trigger(self):
-        self.last_arduino_trigger_time = datetime.datetime.now()
-        self.tested += self.matrix_size
-
-    def reconnect(self):
-        """
-        Attempts to reconnect to the Arduino.
-        """
-        connected = False
-        start_time = time.time()
-        while not connected and not self.stop.is_set() and time.time() - start_time < 60:
-            try:
-                self.comPortObj = serial.Serial(self.trigger_port, BAUD_ARDUINO, timeout=0.1)
-                connected = True
-                self.logger_file.info("Reconnected to Arduino")
-            except serial.SerialException:
-                self.logger_file.error("Reconnection failed. Trying again...")
-                time.sleep(5)
-        if not connected:
-            self.arduino_connection_error = True
-
-    def run(self):
-        """
-        Tries to read data and then counts the number of tags
-        """
-        while not self.stop.is_set():
-            time.sleep(0.100)
-            data = ''
-            if not AUTO_TRIGGERS:
-                try:
-                    data = self.comPortObj.readline()
-                    if data.__len__() > 0:
-                        try:
-                            tmp = data.decode().strip(' \t\n\r')
-                            if "pulses detected" in tmp:
-                                self.raising_trigger()
-                        except Exception as ee:
-                            self.logger_file.error(f'Warning: Could not decode counter data or Warning: {ee}')
-                except serial.SerialException as e:
-                    # Handle disconnection here
-                    self.logger_file.error("Arduino is disconnected   ", e)
-                    self.reconnect()
-                except Exception as ee:
-                    self.logger_file.error(f"NO READLINE: {ee}")
-            else:
-                self.raising_trigger()
-                time.sleep(TIME_BETWEEN_AUTO_TRIGGERS)
-
-        if not AUTO_TRIGGERS:
-            self.comPortObj.close()
-
-    def get_tested(self):
-        """
-        returns the number of tags
-        """
-        return self.tested
-
-    def get_last_arduino_trigger_time(self):
-        return self.last_arduino_trigger_time
-
-    def get_arduino_connection_error(self):
-        return self.arduino_connection_error
-
-
 class MainWindow:
     """
     The main class the runs the GUI and supervise the multi-threading process of fraction's calculation and GUI viewing
     """
 
     def __init__(self):
-        self.user_response_after_arduino_connection_error = False
         self.advanced_window = None
         self.user_response_after_gw_connection_error = False
         self.env_choice = 'prod'
         self.matrix_size = None
         self.latest_yield_value = None
         self.filling_missed_field = None
         self.latest_yield_formatted = 0
@@ -407,27 +334,23 @@
         self.logger = None
         self.ttfp = None
         self.cnt = None
         self.curr_adva_for_log = None
         self.matrix_tags = None
         self.conversion = None
         self.surface = None
-        self.matrix_sec = None
         self.adva_process = None
         self.adva_process_thread = None
-        self.count_process = None
-        self.count_process_thread = None
         self.folder_path = None
         self.py_wiliot_version = None
         self.final_path_run_data = None
         self.run_data_dict = None
         self.tags_num = 0
         self.last_printed = 0
         self.stop = threading.Event()
-        self.neg_col = 0
         self.thermodes_col = None
         self.print_neg_advas = True
         self.selected = ''
         self.wafer_lot = ''
         self.wafer_number = ''
         self.matrix_num = ''
         self.operator = ''
@@ -462,26 +385,26 @@
         self.logger.addHandler(file_handler)
 
     def get_result(self):
         """
         Calculates the yield fraction
         """
         result = 100
-        tags_num = self.count_process.get_tested()
+        tags_num = self.adva_process.get_sensors_triggers() * self.matrix_size
         if tags_num > 0:
             result = (self.not_neg_advas / tags_num) * 100
         return result
 
     def run(self):
         """
         Viewing the window and checking if the process stops
         """
         self.open_session()
         if self.start_run:
-            self.init_processes(self.rec_channel, self.time_pro, self.energy_pat, self.inlay_select, self.matrix_sec)
+            self.init_processes(self.rec_channel, self.time_pro, self.energy_pat, self.inlay_select)
             time.sleep(0.5)
             self.init_run_data()
             self.start_processes()
             self.overlay_window()
         else:
             self.logger.warning('Error Loading Program')
 
@@ -542,15 +465,15 @@
         """
         Updates the run_data CSV file while running the program
         """
 
         raw_packet_queue = self.adva_process.get_raw_packets_queue()
 
         self.number_of_unique_advas = len(self.seen_advas)
-        trigger_time = self.count_process.get_last_arduino_trigger_time()
+        trigger_time = self.adva_process.get_last_change_time()
         if not raw_packet_queue.empty():
             cur_df = pd.DataFrame()
             n_elements = raw_packet_queue.qsize()
             # Collecting Packets from the queue and putting them into a TagCollection
             for _ in range(n_elements):
                 for p in raw_packet_queue.get():
                     tag_matrix_ttfp = self.calc_tag_matrix_ttfp(p['time'], trigger_time)
@@ -587,49 +510,38 @@
         """
         Finishing the program and saves the last changes after pressing Stop in the second window
         """
         self.stop.set()
         window.close()
         self.fig_canvas_agg1.get_tk_widget().destroy()
         self.adva_process_thread.join()
-        self.count_process_thread.join()
 
         self.update_run_data_file(self.final_path_run_data, self.run_data_dict, formatted_date + ' ' + run_end_time,
                                   tags_num, advas, result, self.conversion, self.surface)
         self.update_packet_data()
 
-    def init_processes(self, rec_channel, time_pro, energy_pat, inlay_select, max_movement_time):
+    def init_processes(self, rec_channel, time_pro, energy_pat, inlay_select):
         """
         Initializing the two main instances and threads in order to start working
         """
         try:
             self.adva_process = AdvaProcess(self.stop, rec_channel, time_pro, energy_pat,
                                             inlay_select, self.logger,
                                             self.advas_before_tags, self.folder_path)
             self.adva_process_thread = threading.Thread(target=self.adva_process.run, args=())
         except Exception as e:
             self.logger.warning(f"{e}")
             sg.popup_error("GW is not connected. Please connect it.", keep_on_top=True)
             raise Exception('GW is not connected')
-        try:
-            self.count_process = CountThread(self.stop, self.logger, self.matrix_size, max_movement_time,
-                                             self.thermodes_col)
-            self.count_process_thread = threading.Thread(target=self.count_process.run, args=())
-
-        except Exception as e:
-            self.logger.warning(f"{e}")
-            sg.popup_error("Arduino is not connected. Please connect it.", keep_on_top=True)
-            raise Exception('Arduino is not connected')
 
     def start_processes(self):
         """
         Starting the work of the both threads
         """
         self.adva_process_thread.start()
-        self.count_process_thread.start()
 
     def draw_figure(self, canvas, figure):
         """
         Embeds a Matplotlib figure in a PySimpleGUI Canvas Element
         """
         figure_canvas_agg = FigureCanvasTkAgg(figure, canvas)
         figure_canvas_agg.draw()
@@ -697,44 +609,30 @@
                     time.sleep(1)
                     break
             except Exception as e:
                 self.logger.error('Error while waiting user response')
 
         window.close()
 
-    def overlay_window(self):
-        """
-        The small window open session
-        """
-
-        # taking values from user_input json file
-        temperature_type = user_inputs.get('temperature_type', 'F')
-        min_current = float(user_inputs.get('min_current', '0'))
-        min_cumulative = float(user_inputs.get('min_cumulative', '0'))
-        min_humidity = float(user_inputs.get('min_humidity', '0'))
-        max_humidity = float(user_inputs.get('max_humidity', '0'))
-        max_light_intensity = float(user_inputs.get('max_light_intensity', '2500'))
-        min_light_intensity = float(user_inputs.get('min_light_intensity', '2500'))
-        min_temperature = float(user_inputs.get('min_temperature', '0'))
-        max_temperature = float(user_inputs.get('max_temperature', '0'))
-        red_line_current = float(user_inputs.get('red_line_current', '0'))
-        red_line_cumulative = float(user_inputs.get('red_line_cumulative', '0'))
+    def overlay_layout(self, temperature_type):
         layout = [
             [
                 sg.Column([
                     [sg.Text('Number of tags:', font=('Helvetica', 20, 'bold')),
                      sg.Text(key='num_rows', font=('Helvetica', 20, 'bold'))],
                     [sg.Text('Number of advas:', font=('Helvetica', 20, 'bold')),
                      sg.Text(key='num_advas', font=('Helvetica', 20, 'bold'))],
                     [sg.Text('Light Intensity:', font=('Helvetica', 15)),
                      sg.Text(f'{self.light_intensity} lux', key='light_intensity_value',
                              font=('Helvetica', 15)),
                      sg.Text('', size=(31, 1)),
                      sg.Text('Temperature:', font=('Helvetica', 14)),
-                     sg.Text(f'{self.temperature} {temperature_type}', key='temperature_value', font=('Helvetica', 15)),
+                     sg.Text(
+                         f'{self.temperature if temperature_type == "C" else self.temperature * 9 / 5 + 32} {temperature_type}',
+                         key='temperature_value', font=('Helvetica', 15)),
                      sg.Text('', size=(31, 1)),
                      sg.Text('Humidity:', font=('Helvetica', 15)),
                      sg.Text(f'{self.humidity} %', key='humidity_value', font=('Helvetica', 15)),
                      sg.Text('', size=(31, 1)),
                      sg.Text(f'Matrix num: {self.matrix_num}', key='matrix_num_value', font=('Helvetica', 15))]
                 ]),
             ],
@@ -749,25 +647,17 @@
                 sg.Text('', size=(10, 1), key='-current_status_value-', font=('Helvetica', 18, 'bold')),
                 sg.Text('', size=(45, 1)),
                 sg.Text('', size=(23, 1), key='-cumulative_status-', font=('Helvetica', 14, 'bold')),
                 sg.Text('', size=(5, 1), key='-cumulative_status_value-', font=('Helvetica', 18, 'bold')),
                 sg.Text('', size=(21, 1)), sg.Button('Advanced Settings')
             ]
         ]
-        screen_width, screen_height = sg.Window.get_screen_size()
-        window = sg.Window('Wiliot Yield Tester', layout, modal=True, finalize=True, size=(screen_width - 100, screen_height - 100), resizable=True)
-
-        # initialize num_advas and num_rows
-        num_rows_text_elem = window['num_rows']
-        num_advas_text_elem = window['num_advas']
-        num_rows = (self.rows_number * self.neg_col)
-        num_advas = 0
-        num_rows_text_elem.update(f"{num_rows}", font=('Helvetica', 20, 'bold'))
-        num_advas_text_elem.update(f"{num_advas}", font=('Helvetica', 20, 'bold'))
+        return layout
 
+    def init_graphs(self, window, min_current, min_cumulative):
         # create the main figure and two subplots
         fig, (ax, axy) = plt.subplots(1, 2, figsize=(20, 6))
 
         # initialize the first graph
         prev_tests = 0
         prev_val = 100
         ax.set_xlabel('Number of tags', fontweight='bold')
@@ -795,14 +685,172 @@
                              fontweight='bold')
         if user_inputs.get('min_cumulative_line') == 'yes':
             axy.axhline(y=min_cumulative, color='black', linestyle='--')
         # embed the plots in the PySimpleGUI window
         canvas_elem1 = window['-CANVAS1-']
         self.fig_canvas_agg1 = self.draw_figure(canvas_elem1.TKCanvas, fig)
 
+        return ax, axy, prev_tests, prev_val, prev_tests1, prev_val1, text_box, text_box1
+
+    def update_current_graph(self, window, ax, new_num_rows, min_current, red_line_current, prev_tests,
+                             prev_val, current_tested):
+        curr_tests = new_num_rows
+        curr_val = 100 * ((len(self.seen_advas) - self.curr_adva_for_log) / self.matrix_size)
+        if curr_val > 100:
+            curr_val = SET_VALUE_MORE_THAN_100
+        self.curr_adva_for_log = len(self.seen_advas)
+
+        if curr_val < min_current:
+            font_color_current = RED_COLOR
+            status_message_current = f'Current yield is lower than'
+            status_value_current = f'{min_current}%'
+        else:
+            font_color_current = 'white'
+            status_message_current = ''
+            status_value_current = ''
+        figure_color_current = 'red' if curr_val < red_line_current else 'blue'
+
+        window['-current_status-'].update(status_message_current, text_color=font_color_current)
+        window['-current_status_value-'].update(status_value_current, text_color=font_color_current)
+        ax.plot([prev_tests, curr_tests], [prev_val, curr_val], color=figure_color_current)
+        prev_tests = curr_tests
+        prev_val = curr_val
+        prev_tested = current_tested
+        self.last_printed = current_tested
+        self.cnt += 1
+
+        return prev_tests, prev_val, prev_tested
+
+    def update_cumulative_graph(self, window, axy, new_num_rows, min_cumulative, red_line_cumulative, prev_tests1,
+                                prev_val1, text_box1):
+        curr_tests1 = new_num_rows
+        curr_val1 = self.get_result()
+
+        if curr_val1 > 100:
+            curr_val1 = SET_VALUE_MORE_THAN_100
+        elif 0 < curr_val1 < 101:
+            self.first_time_between_0_and_100 = True
+        if curr_val1 < min_cumulative:
+            font_color_cumulative = RED_COLOR
+            status_message_cumulative = f'Cumulative yield is lower than'
+            status_value_cumulative = f'{min_cumulative} % '
+        else:
+            font_color_cumulative = 'white'
+            status_message_cumulative = ''
+            status_value_cumulative = ''
+        figure_color_cumulative = 'red' if curr_val1 < red_line_cumulative else 'blue'
+
+        window['-cumulative_status-'].update(status_message_cumulative, text_color=font_color_cumulative)
+        window['-cumulative_status_value-'].update(status_value_cumulative, text_color=font_color_cumulative)
+
+        if new_num_rows != 0 and self.first_time_between_0_and_100:
+            axy.plot([prev_tests1, curr_tests1], [prev_val1, curr_val1], color=figure_color_cumulative)
+        prev_tests1 = curr_tests1
+        prev_val1 = curr_val1
+        text_box1.set_text(f"Cumulative Yield : {curr_val1:.2f} %")
+        self.fig_canvas_agg1.draw()
+
+        return prev_tests1, prev_val1
+
+    def handling_advanced_settings_window(self, adv_event, adv_values, window, ax, current_min_y_value,
+                                          current_max_y_value, current_size_value, axy, cumulative_min_y_value,
+                                          cumulative_max_y_value, cumulative_size_value):
+        if adv_event == 'OK':
+            if adv_values['matrix_num']:
+                self.matrix_num = int(adv_values['matrix_num'])
+                window['matrix_num_value'].update(f'Matrix num: {self.matrix_num}')
+            if adv_values['current_min_y_value']:
+                current_min_y_value = float(adv_values['current_min_y_value'])
+            if adv_values['current_max_y_value']:
+                current_max_y_value = float(adv_values['current_max_y_value'])
+            if adv_values['current_size_value']:
+                current_size_value = float(adv_values['current_size_value'])
+
+            if adv_values['cumulative_min_y_value']:
+                cumulative_min_y_value = float(adv_values['cumulative_min_y_value'])
+            if adv_values['cumulative_max_y_value']:
+                cumulative_max_y_value = float(adv_values['cumulative_max_y_value'])
+            if adv_values['cumulative_size_value']:
+                cumulative_size_value = float(adv_values['cumulative_size_value'])
+
+            ax.set_ylim([current_min_y_value, current_max_y_value])
+            ax.set_yticks(np.arange(current_min_y_value, current_max_y_value + current_size_value,
+                                    current_size_value))
+
+            axy.set_ylim([cumulative_min_y_value, cumulative_max_y_value])
+            axy.set_yticks(np.arange(cumulative_min_y_value, cumulative_max_y_value + cumulative_size_value,
+                                     cumulative_size_value))
+
+            self.fig_canvas_agg1.draw()
+
+            self.advanced_window.close()
+            self.advanced_window = None
+        elif adv_event in (None, sg.WINDOW_CLOSED):
+            self.advanced_window.close()
+            self.advanced_window = None
+        elif adv_event == 'Reset':
+            default_values = {
+                'current_min_y_value': 0,
+                'current_max_y_value': 120,
+                'current_size_value': 10,
+                'cumulative_min_y_value': 0,
+                'cumulative_max_y_value': 120,
+                'cumulative_size_value': 10
+            }
+            # Reset the values and update the input fields
+            for key in default_values:
+                self.advanced_window[key].update(default_values[key])
+                globals()[key] = default_values[key]
+
+            # Update the graph with reset values
+            ax.set_ylim([current_min_y_value, current_max_y_value])
+            ax.set_yticks(np.arange(current_min_y_value, current_max_y_value + current_size_value,
+                                    current_size_value))
+
+            axy.set_ylim([cumulative_min_y_value, cumulative_max_y_value])
+            axy.set_yticks(np.arange(cumulative_min_y_value, cumulative_max_y_value + cumulative_size_value,
+                                     cumulative_size_value))
+
+            self.fig_canvas_agg1.draw()
+
+    def overlay_window(self):
+        """
+        The small window open session
+        """
+        # taking values from user_input json file
+        temperature_type = user_inputs.get('temperature_type', 'F')
+        min_current = float(user_inputs.get('min_current', '0'))
+        min_cumulative = float(user_inputs.get('min_cumulative', '0'))
+        min_humidity = float(user_inputs.get('min_humidity', '0'))
+        max_humidity = float(user_inputs.get('max_humidity', '0'))
+        max_light_intensity = float(user_inputs.get('max_light_intensity', '2500'))
+        min_light_intensity = float(user_inputs.get('min_light_intensity', '2500'))
+        min_temperature = float(user_inputs.get('min_temperature', '0'))
+        max_temperature = float(user_inputs.get('max_temperature', '0'))
+        red_line_current = float(user_inputs.get('red_line_current', '0'))
+        red_line_cumulative = float(user_inputs.get('red_line_cumulative', '0'))
+
+        # creating the main window
+        layout = self.overlay_layout(temperature_type)
+        screen_width, screen_height = sg.Window.get_screen_size()
+        window = sg.Window('Wiliot Yield Tester', layout, modal=True, finalize=True,
+                           size=(screen_width - 100, screen_height - 100), resizable=True)
+
+        # initialize num_advas and num_rows
+        num_rows_text_elem = window['num_rows']
+        num_advas_text_elem = window['num_advas']
+        num_rows = 0
+        num_advas = 0
+        num_rows_text_elem.update(f"{num_rows}", font=('Helvetica', 20, 'bold'))
+        num_advas_text_elem.update(f"{num_advas}", font=('Helvetica', 20, 'bold'))
+
+        # initializing graphs
+        ax, axy, prev_tests, prev_val, prev_tests1, prev_val1, text_box, text_box1 = \
+            self.init_graphs(window, min_current, min_cumulative)
+
         # values before running
         self.neg_advas = len(self.seen_advas)
         self.curr_adva_for_log = len(self.seen_advas)
         self.cnt = 1
         stop_window = None
         sub = False
         current_min_y_value = MIN_Y_FOR_PLOTS
@@ -813,15 +861,15 @@
         cumulative_size_value = FIRST_STEP_SIZE
         prev_tested = 0
         result = float('inf')
 
         while True:
 
             event, values = window.read(timeout=100)
-            new_num_rows = self.count_process.get_tested() + (self.rows_number * self.neg_col)
+            new_num_rows = self.adva_process.get_sensors_triggers() * self.matrix_size
             new_num_advas = len(self.seen_advas) - self.neg_advas
             self.not_neg_advas = new_num_advas
             # update packet data
             self.update_packet_data()
             if event == 'Advanced Settings':
                 advanced_layout = [
                     [
@@ -837,116 +885,57 @@
                         ])
                     ],
                     [sg.Text('Matrix num:'), sg.Input(key='matrix_num', size=(10, 1))],
                     [sg.Button('Reset'), sg.Button('OK')]]
 
                 self.advanced_window = sg.Window('Advanced Settings', advanced_layout, modal=True)
 
-            elif event == 'Stop' or self.adva_process.get_gw_error_connection() or \
-                    self.count_process.get_arduino_connection_error():
+            elif event == 'Stop' or self.adva_process.get_gw_error_connection():
                 try:
                     self.logger.info('Final Yield: %s, Final Tags: %05d, Final Advas: %05d,',
-                                     result, self.count_process.get_tested(), len(self.seen_advas), )
+                                     result, self.adva_process.get_sensors_triggers() * self.matrix_size, len(self.seen_advas), )
                 except Exception as e:
                     result = 0
                     self.logger.info('Final Yield: %s, Final Tags: %05d, Final Advas: %05d,',
-                                     result, self.count_process.get_tested(), len(self.seen_advas), )
+                                     result, self.adva_process.get_sensors_triggers() * self.matrix_size, len(self.seen_advas), )
                 window.close()
-                if not self.adva_process.get_gw_error_connection() and \
-                        not self.count_process.get_arduino_connection_error():  # uploading after connection error
+                if not self.adva_process.get_gw_error_connection():  # uploading after connection error
                     # pressing 'OK'
                     self.upload_to_cloud()
                 else:
-                    if self.count_process.get_arduino_connection_error():
-                        self.user_response_after_arduino_connection_error = True
-                    else:
-                        self.user_response_after_gw_connection_error = True
+                    self.user_response_after_gw_connection_error = True
                 end_time = datetime.datetime.now()
                 run_end_time = end_time.strftime("%I:%M:%S")
                 advas = len(self.seen_advas)
-                tags_num = self.count_process.get_tested()
+                tags_num = self.adva_process.get_sensors_triggers() * self.matrix_size
                 result = float(100 * (advas / tags_num)) if tags_num != 0 else float('inf')
                 self.stop_button(window, run_end_time, tags_num, advas, result)
                 sub = True
             elif event in (None, sg.WINDOW_CLOSED):
                 window.close()
                 break
-            # ignoring all advas before receiving the first arduino trigger
-            elif new_num_rows < self.matrix_size + (self.rows_number * self.neg_col):
+            # ignoring all advas before receiving the first trigger
+            elif new_num_rows < self.matrix_size:
                 if self.adva_process.gw_instance.is_data_available():
                     packet_list_in = self.adva_process.gw_instance.get_packets(action_type=ActionType.ALL_SAMPLE,
                                                                                tag_inlay=self.adva_process.inlay_type)
                     for packet in packet_list_in:
                         adva = packet.get_adva()
                         self.adva_process.advas_before_tags.add(adva)
                 self.not_neg_advas = 0
-                new_num_rows = self.count_process.get_tested() + (self.rows_number * self.neg_col)
+                new_num_rows = self.adva_process.get_sensors_triggers() * self.matrix_size
                 continue
             else:
                 if self.advanced_window:
-
                     adv_event, adv_values = self.advanced_window.read(timeout=10)
 
-                    if adv_event == 'OK':
-                        if adv_values['matrix_num']:
-                            self.matrix_num = int(adv_values['matrix_num'])
-                            window['matrix_num_value'].update(f'Matrix num: {self.matrix_num}')
-                        if adv_values['current_min_y_value']:
-                            current_min_y_value = float(adv_values['current_min_y_value'])
-                        if adv_values['current_max_y_value']:
-                            current_max_y_value = float(adv_values['current_max_y_value'])
-                        if adv_values['current_size_value']:
-                            current_size_value = float(adv_values['current_size_value'])
-
-                        if adv_values['cumulative_min_y_value']:
-                            cumulative_min_y_value = float(adv_values['cumulative_min_y_value'])
-                        if adv_values['cumulative_max_y_value']:
-                            cumulative_max_y_value = float(adv_values['cumulative_max_y_value'])
-                        if adv_values['cumulative_size_value']:
-                            cumulative_size_value = float(adv_values['cumulative_size_value'])
-
-                        ax.set_ylim([current_min_y_value, current_max_y_value])
-                        ax.set_yticks(np.arange(current_min_y_value, current_max_y_value + current_size_value,
-                                                current_size_value))
-
-                        axy.set_ylim([cumulative_min_y_value, cumulative_max_y_value])
-                        axy.set_yticks(np.arange(cumulative_min_y_value, cumulative_max_y_value + cumulative_size_value,
-                                                 cumulative_size_value))
-
-                        self.fig_canvas_agg1.draw()
-
-                        self.advanced_window.close()
-                        self.advanced_window = None
-                    elif adv_event in (None, sg.WINDOW_CLOSED):
-                        self.advanced_window.close()
-                        self.advanced_window = None
-                    elif adv_event == 'Reset':
-                        default_values = {
-                            'current_min_y_value': 0,
-                            'current_max_y_value': 120,
-                            'current_size_value': 10,
-                            'cumulative_min_y_value': 0,
-                            'cumulative_max_y_value': 120,
-                            'cumulative_size_value': 10
-                        }
-                        # Reset the values and update the input fields
-                        for key in default_values:
-                            self.advanced_window[key].update(default_values[key])
-                            globals()[key] = default_values[key]
-
-                        # Update the graph with reset values
-                        ax.set_ylim([current_min_y_value, current_max_y_value])
-                        ax.set_yticks(np.arange(current_min_y_value, current_max_y_value + current_size_value,
-                                                current_size_value))
-
-                        axy.set_ylim([cumulative_min_y_value, cumulative_max_y_value])
-                        axy.set_yticks(np.arange(cumulative_min_y_value, cumulative_max_y_value + cumulative_size_value,
-                                                 cumulative_size_value))
-
-                        self.fig_canvas_agg1.draw()
+                    self.handling_advanced_settings_window(adv_event, adv_values, window, ax, current_min_y_value,
+                                                           current_max_y_value, current_size_value, axy,
+                                                           cumulative_min_y_value,
+                                                           cumulative_max_y_value, cumulative_size_value)
 
                 # updating number of rows in GUI
                 if new_num_rows != num_rows:
                     num_rows = new_num_rows
                     num_rows_text_elem.update(f"{num_rows}")
 
                 # updating number of advas in GUI
@@ -954,15 +943,15 @@
                     num_advas = new_num_advas
                     num_advas_text_elem.update(f"{num_advas - self.neg_advas}")
                 # writing the number of neglected advas in LOG
                 if self.print_neg_advas:
                     self.logger.info('neglected advas:  %05d', len(self.advas_before_tags))
                     self.print_neg_advas = False
                 # all processes when getting a new matrix
-                current_tested = self.count_process.get_tested()
+                current_tested = self.adva_process.get_sensors_triggers() * self.matrix_size
                 if (current_tested - prev_tested) % (self.matrix_size * int(self.matrix_num)) \
                         == 0 and current_tested != self.last_printed:
                     temperature_display = f"{self.temperature:.2f} °C"
                     if self.main_sensor:
                         self.light_intensity = self.main_sensor.get_light()
                         self.humidity = self.main_sensor.get_humidity()
                         self.temperature = self.main_sensor.get_temperature()
@@ -990,130 +979,56 @@
                         yield_result = "0" + yield_result
                     latest_adva = len(self.seen_advas) - self.curr_adva_for_log
                     self.latest_yield_formatted = "{:.5f}".format(float(latest_adva / self.matrix_size) * 100).zfill(9)
                     self.logger.info(
                         'Matrix Number: %05d, Cumulative Yield: %s, Cumulative Tags: %05d, Cumulative Advas: %05d,'
                         'Latest Yield: %s, Latest Tags: %05d, Latest Advas: %05d, Light Intensity: '
                         '%05.1f, Humidity: %05.1f, Temperature: %05.1f',
-                        (self.count_process.get_tested() / self.matrix_size),
-                        yield_result, self.count_process.get_tested(), len(self.seen_advas),
+                        (self.adva_process.get_sensors_triggers()),
+                        yield_result, self.adva_process.get_sensors_triggers() * self.matrix_size, len(self.seen_advas),
                         self.latest_yield_formatted,
                         self.matrix_size, latest_adva, self.light_intensity, self.humidity, self.temperature)
 
                     # updating the first graph
-                    curr_tests = new_num_rows
-                    curr_val = 100 * ((len(self.seen_advas) - self.curr_adva_for_log) / self.matrix_size)
-                    if curr_val > 100:
-                        curr_val = SET_VALUE_MORE_THAN_100
-                    self.curr_adva_for_log = len(self.seen_advas)
-
-                    if curr_val < min_current:
-                        font_color_current = RED_COLOR
-                        status_message_current = f'Current yield is lower than'
-                        status_value_current = f'{min_current}%'
-                    else:
-                        font_color_current = 'white'
-                        status_message_current = ''
-                        status_value_current = ''
-                    figure_color_current = 'red' if curr_val < red_line_current else 'blue'
-
-                    window['-current_status-'].update(status_message_current, text_color=font_color_current)
-                    window['-current_status_value-'].update(status_value_current, text_color=font_color_current)
-                    ax.plot([prev_tests, curr_tests], [prev_val, curr_val], color=figure_color_current)
-                    prev_tests = curr_tests
-                    prev_val = curr_val
-                    prev_tested = current_tested
-                    self.last_printed = current_tested
-                    self.cnt += 1
+                    prev_tests, prev_val, prev_tested = self.update_current_graph(window, ax, new_num_rows, min_current,
+                                                                                  red_line_current, prev_tests,
+                                                                                  prev_val, current_tested)
 
                 # updating the second graph
-                curr_tests1 = new_num_rows
-                curr_val1 = self.get_result()
-
-                if curr_val1 > 100:
-                    curr_val1 = SET_VALUE_MORE_THAN_100
-                elif 0 < curr_val1 < 101:
-                    self.first_time_between_0_and_100 = True
-                if curr_val1 < min_cumulative:
-                    font_color_cumulative = RED_COLOR
-                    status_message_cumulative = f'Cumulative yield is lower than'
-                    status_value_cumulative = f'{min_cumulative} % '
-                else:
-                    font_color_cumulative = 'white'
-                    status_message_cumulative = ''
-                    status_value_cumulative = ''
-                figure_color_cumulative = 'red' if curr_val1 < red_line_cumulative else 'blue'
-
-                window['-cumulative_status-'].update(status_message_cumulative, text_color=font_color_cumulative)
-                window['-cumulative_status_value-'].update(status_value_cumulative, text_color=font_color_cumulative)
-
-                if new_num_rows != 0 and self.first_time_between_0_and_100:
-                    axy.plot([prev_tests1, curr_tests1], [prev_val1, curr_val1], color=figure_color_cumulative)
-                prev_tests1 = curr_tests1
-                prev_val1 = curr_val1
-                text_box1.set_text(f"Cumulative Yield : {curr_val1:.2f} %")
-                self.fig_canvas_agg1.draw()
+                prev_tests1, prev_val1 = self.update_cumulative_graph(window, axy, new_num_rows, min_cumulative,
+                                                                      red_line_cumulative, prev_tests1, prev_val1,
+                                                                      text_box1)
 
                 # updating run_data_file
                 end_time = datetime.datetime.now()
                 run_end_time = end_time.strftime("%I:%M:%S")
                 advas = len(self.seen_advas)
-                tags_num = self.count_process.get_tested()
+                tags_num = self.adva_process.get_sensors_triggers() * self.matrix_size
                 result = float(100 * (advas / tags_num)) if tags_num != 0 else float('inf')
                 self.update_run_data_file(self.final_path_run_data, self.run_data_dict,
                                           formatted_date + ' ' + run_end_time,
                                           tags_num, advas, result, self.conversion, self.surface)
-            if self.user_response_after_gw_connection_error or self.user_response_after_arduino_connection_error:
-                connection_error = ''
-                if self.user_response_after_gw_connection_error:
-                    connection_error = 'GW'
-                else:
-                    connection_error = 'Arduino'
+            if self.user_response_after_gw_connection_error:
+                connection_error = 'GW'
                 self.error_popup(connection_error)
                 self.upload_to_cloud()
             if sub:
                 break
 
         return sub
 
-    def open_session(self):
-        """
-        opening a session for the process
-        """
-        # save data to configs file
-        if os.path.exists("configs/gui_input_do_not_delete.json"):
-            with open("configs/gui_input_do_not_delete.json", "r") as f:
-                previous_input = json.load(f)
-
-        else:
-            previous_input = {'inlay': '', 'number': '', 'received_channel': '',
-                              'energy_pattern_val': '', 'tester_station_name': '',
-                              'comments': '', 'operator': '', 'wafer_lot': '', 'wafer_num': '', 'conversion_type': '',
-                              'surface': '', 'matrix_tags': '', 'thermodes_col': '0', 'gw_energy_pattern': '',
-                              'gw_time_profile': '', 'rows_number': '0', 'matrix_sec': '', 'matrix_num': ''}
-
-        # update fields from configs
-        self.start_run = False
-        selected_inlay = csv_dictionary[previous_input['inlay']]
-        energy_pat = selected_inlay['energy_pattern_val']
-        time_pro = selected_inlay['time_profile_val']
-        rec_channel = selected_inlay['received_channel']
-        lst_inlay_options = list(inlay_types_dict.keys())
-        conv_opts = ['Not converted', 'Standard', 'Durable']
-        surfaces = ['Air', 'Cardboard', 'RPC', 'General Er3', 'General Er3.5']
-        default_matrix_tags = int(previous_input['thermodes_col']) * int(previous_input['rows_number'])
+    def open_session_layout(self, previous_input, lst_inlay_options, energy_pat, time_pro, rec_channel, conv_opts,
+                            surfaces, default_matrix_tags):
         layout = [
             [sg.Text('Wafer Lot:', size=(13, 1), font=4),
              sg.InputText(previous_input['wafer_lot'], key='wafer_lot', font=4),
              sg.Text('Wafer Number:', size=(13, 1), font=4),
              sg.InputText(previous_input['wafer_num'], key='wafer_num', font=4)],
 
             [
-                sg.Text('Time of matrix:', size=(13, 1), font=4),
-                sg.InputText(previous_input['matrix_sec'], key='matrix_sec', font=4),
                 sg.Text('Num of matrices:', size=(13, 1), font=4),
                 sg.InputText(previous_input['matrix_num'], key='matrix_num', font=4)],
 
             [sg.Text('Thermode Col:', size=(13, 1), font=4),
              sg.InputText(previous_input['thermodes_col'], key='thermodes_col', font=4, enable_events=True),
              sg.Text('Rows Number :', size=(13, 1), font=4),
              sg.InputText(previous_input['rows_number'], key='rows_number', font=4, enable_events=True)],
@@ -1140,14 +1055,45 @@
                       enable_events=True), sg.Text('Surface:', font=4),
              sg.Combo(values=surfaces, default_value=previous_input['surface'], key='surface', font=4,
                       enable_events=True)],
 
             [sg.Submit()]
         ]
 
+        return layout
+
+    def open_session(self):
+        """
+        opening a session for the process
+        """
+        # save data to configs file
+        if os.path.exists("configs/gui_input_do_not_delete.json"):
+            with open("configs/gui_input_do_not_delete.json", "r") as f:
+                previous_input = json.load(f)
+
+        else:
+            previous_input = {'inlay': '', 'number': '', 'received_channel': '',
+                              'energy_pattern_val': '', 'tester_station_name': '',
+                              'comments': '', 'operator': '', 'wafer_lot': '', 'wafer_num': '', 'conversion_type': '',
+                              'surface': '', 'matrix_tags': '', 'thermodes_col': '0', 'gw_energy_pattern': '',
+                              'gw_time_profile': '', 'rows_number': '0', 'matrix_num': ''}
+
+        # update fields from configs
+        self.start_run = False
+        selected_inlay = csv_dictionary[previous_input['inlay']]
+        energy_pat = selected_inlay['energy_pattern_val']
+        time_pro = selected_inlay['time_profile_val']
+        rec_channel = selected_inlay['received_channel']
+        lst_inlay_options = list(inlay_types_dict.keys())
+        conv_opts = ['Not converted', 'Standard', 'Durable']
+        surfaces = ['Air', 'Cardboard', 'RPC', 'General Er3', 'General Er3.5']
+        default_matrix_tags = int(previous_input['thermodes_col']) * int(previous_input['rows_number'])
+
+        layout = self.open_session_layout(previous_input, lst_inlay_options, energy_pat, time_pro, rec_channel,
+                                          conv_opts, surfaces, default_matrix_tags)
         window = sg.Window('WILIOT Yield Tester', layout, finalize=True)
 
         while True:
             event, values = window.read(timeout=100)
             inlay_select = values['inlay']
             self.selected = values['inlay']
             if event == 'inlay':
@@ -1164,15 +1110,14 @@
                     rec_channel = 'Invalid Selection'
 
                 window.find_element('rows_number').Update(value=self.rows_number)
                 window.find_element('energy_pattern_val').Update(value=energy_pat)
                 window.find_element('time_profile_val').Update(value=time_pro)
                 window.find_element('received_channel').Update(value=rec_channel)
             if event == 'Submit':
-                self.matrix_sec = (values['matrix_sec'])
                 self.wafer_lot = values['wafer_lot']
                 self.wafer_number = values['wafer_num']
                 self.matrix_num = values['matrix_num']
                 self.comments = values['comments']
                 self.rows_number = int(values['rows_number'])
                 self.gw_energy_pattern = energy_pat
                 self.gw_time_profile = time_pro
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers.egg-info/PKG-INFO` & `wiliot-testers-5.4.13/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: wiliot-testers
-Version: 5.3.9
-Summary: A library for interacting with Wiliot's Testers app
-Home-page: UNKNOWN
-Author: Wiliot
-Author-email: support@wiliot.com
-License: MIT
-Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyWiliot: wiliot-testers #
 
 wiliot-testers is a python library for accessing Wiliot's Testers scripts
 
 ## Public Library
 
 ### MAC Installation
@@ -57,14 +40,48 @@
 * [Yield Tester](wiliot_testers/yield_tester/yield_tester.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 5.4.13:
+-----------------
+    
+* tester SDK:
+    * raise exception if bad gateway configuration occurs
+    * even if test stopped by the user, first update and analyze results and then exit the test
+    * if fail bin was set outside the test, all functions should be updated accordingly
+    
+* sensors and hardware:
+    * improve light sensor calibration
+    * added a script to configure attenuator
+    * added beacons power calibration for chambers
+    
+* test equipment:
+    * improve chamber handling
+    * add more options to work with Cognex scanner
+    
+* offline tester
+    * added support for GW gpio new functionalities and control PLC using GW only
+    * added support to more external sensors
+    * added support to handle duplication if tag was not printed yet
+    * added support to label missing label case
+    
+* sample test
+    * new architecture for sample test including adding sample test sdk class based on the tester sdk.
+    * added a resolver class to get external id from packet based on api key
+    
+    
+* yield-tester:
+    * add support to clout wafer matrix using the GW and not Arduino.
+    * update graph and labels
+    * fix bug in temperature calculation
+
+
 Version 5.3.9:
 -----------------
 * offline tester: HOTFIX for running without printing
 
 Version 5.3.8:
 -----------------
 * offline tester: HOTFIX for printer communication
@@ -247,9 +264,7 @@
 Version 4.0.0:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
 for more information please read 'wiliot' package's release notes
-
-
```

### Comparing `wiliot-testers-5.3.9/wiliot_testers.egg-info/SOURCES.txt` & `wiliot-testers-5.4.13/wiliot_testers.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 wiliot_testers/wiliot_tester_tag_test.py
 wiliot_testers.egg-info/PKG-INFO
 wiliot_testers.egg-info/SOURCES.txt
 wiliot_testers.egg-info/dependency_links.txt
 wiliot_testers.egg-info/not-zip-safe
 wiliot_testers.egg-info/requires.txt
 wiliot_testers.egg-info/top_level.txt
+wiliot_testers/association_tester/__init__.py
+wiliot_testers/association_tester/association_and_verification_tester.py
+wiliot_testers/association_tester/association_module.py
+wiliot_testers/association_tester/performance_module.py
+wiliot_testers/association_tester/r2r_component.py
+wiliot_testers/association_tester/scanner_component.py
 wiliot_testers/calibration_test/__init__.py
 wiliot_testers/calibration_test/calibration_test.py
 wiliot_testers/calibration_test/calibration_test_by_tbp.py
 wiliot_testers/config/__init__.py
 wiliot_testers/config/equipment_config.json
 wiliot_testers/config/unusable_inlays.py
 wiliot_testers/docs/__init__.py
@@ -41,63 +47,71 @@
 wiliot_testers/offline/configs/__init__.py
 wiliot_testers/offline/configs/global_vars_and_enums.py
 wiliot_testers/offline/configs/moh_instruction.py
 wiliot_testers/offline/configs/tests_suites.json
 wiliot_testers/offline/modules/__init__.py
 wiliot_testers/offline/modules/offline_log.py
 wiliot_testers/offline/modules/offline_printing_and_validation.py
+wiliot_testers/offline/modules/offline_r2r_controller.py
 wiliot_testers/offline/modules/offline_tag_testing.py
 wiliot_testers/offline/modules/offline_utils.py
 wiliot_testers/offline/utils/__init__.py
 wiliot_testers/offline/utils/barcode_test.py
 wiliot_testers/offline/utils/env_install.bat
 wiliot_testers/offline/utils/env_install.py
 wiliot_testers/offline/utils/offline_log_editing.py
 wiliot_testers/offline/utils/tadbik_r2r_controller.py
 wiliot_testers/partners/__init__.py
-wiliot_testers/partners/avery_dennison/__init__.py
-wiliot_testers/partners/avery_dennison/simple_test.py
-wiliot_testers/partners/avery_dennison/test_upload_get_AD.py
-wiliot_testers/partners/avery_dennison/configs/test_suite_example.json
+wiliot_testers/partners/simple_test/__init__.py
+wiliot_testers/partners/simple_test/simple_test.py
+wiliot_testers/partners/simple_test/test_upload_get_results.py
+wiliot_testers/partners/simple_test/configs/__init__.py
+wiliot_testers/partners/simple_test/configs/test_suite_example.json
 wiliot_testers/sample/__init__.py
 wiliot_testers/sample/com_connect.py
 wiliot_testers/sample/configs_gui.py
-wiliot_testers/sample/get_temperature_sensor_name.py
 wiliot_testers/sample/sample_chamber.py
+wiliot_testers/sample/sample_slim.py
 wiliot_testers/sample/sample_test.bat
 wiliot_testers/sample/sample_test.py
 wiliot_testers/sample/configs/.default_surfaces.json
 wiliot_testers/sample/configs/.default_test_configs.json
 wiliot_testers/sample/configs/__init__.py
+wiliot_testers/sample/modules/__init__.py
+wiliot_testers/sample/modules/resolve_packets.py
+wiliot_testers/sample/modules/wiliot_sample_tag_test.py
 wiliot_testers/sample/utils/__init__.py
 wiliot_testers/sample/utils/com_connect.ui
 wiliot_testers/sample/utils/comm.gif
 wiliot_testers/sample/utils/configs.gif
 wiliot_testers/sample/utils/configs.ui
 wiliot_testers/sample/utils/edit.gif
 wiliot_testers/sample/utils/refresh.gif
 wiliot_testers/sample/utils/reset.png
 wiliot_testers/sample/utils/sample_test.ui
 wiliot_testers/sample/utils/save.png
 wiliot_testers/sample/utils/wiliot3.gif
-wiliot_testers/sensors/__init__.py
-wiliot_testers/sensors/get_light.py
-wiliot_testers/sensors/get_temperature.py
-wiliot_testers/sensors/light_sensor_calibration.py
+wiliot_testers/sensors_and_hardware/__init__.py
+wiliot_testers/sensors_and_hardware/config_attenuators.bat
+wiliot_testers/sensors_and_hardware/config_attenuators.py
+wiliot_testers/sensors_and_hardware/get_light.py
+wiliot_testers/sensors_and_hardware/get_temperature.py
+wiliot_testers/sensors_and_hardware/get_temperature_sensor_name.py
+wiliot_testers/sensors_and_hardware/light_sensor_calibration.py
 wiliot_testers/system_test/__init__.py
+wiliot_testers/system_test/beacon_power_calibration.py
 wiliot_testers/system_test/harvester_test.py
 wiliot_testers/system_test/system_test_example.py
 wiliot_testers/utils/Install PPFP.bat
 wiliot_testers/utils/__init__.py
 wiliot_testers/utils/get_version.py
 wiliot_testers/utils/ppfp_tool.py
 wiliot_testers/utils/upload_to_cloud_api.py
 wiliot_testers/utils/wiliot_external_ids.py
 wiliot_testers/yield_tester/__init__.py
-wiliot_testers/yield_tester/count_thread.py
 wiliot_testers/yield_tester/from_listener_log_to_csv.py
 wiliot_testers/yield_tester/run_yield_tester.bat
 wiliot_testers/yield_tester/trigger_miss_catcher.py
 wiliot_testers/yield_tester/yield_tester.py
 wiliot_testers/yield_tester/arduino_counter/__init__.py
 wiliot_testers/yield_tester/arduino_counter/arduino_counter.ino
 wiliot_testers/yield_tester/configs/.default_configs.json
```

