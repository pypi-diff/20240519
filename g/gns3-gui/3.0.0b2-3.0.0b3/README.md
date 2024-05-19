# Comparing `tmp/gns3-gui-3.0.0b2.tar.gz` & `tmp/gns3_gui-3.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gns3-gui-3.0.0b2.tar", last modified: Sun Apr  7 12:41:31 2024, max compression
+gzip compressed data, was "gns3_gui-3.0.0b3.tar", last modified: Sun May 19 10:32:57 2024, max compression
```

## Comparing `gns3-gui-3.0.0b2.tar` & `gns3_gui-3.0.0b3.tar`

### file list

```diff
@@ -1,887 +1,888 @@
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.608210 gns3-gui-3.0.0b2/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   119702 2024-04-07 11:51:59.000000 gns3-gui-3.0.0b2/CHANGELOG
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35147 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/LICENSE
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      138 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/MANIFEST.in
--rw-r--r--   0 grossmj   (1000) grossmj   (1000)    43930 2024-04-07 12:41:31.608210 gns3-gui-3.0.0b2/PKG-INFO
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1714 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/README.md
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       94 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/dev-requirements.txt
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.056205 gns3-gui-3.0.0b2/gns3/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       33 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      736 2024-02-12 05:00:39.000000 gns3-gui-3.0.0b2/gns3/__main__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3456 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/appliance_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3017 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/application.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8604 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/base_node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5711 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/compute.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9953 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/compute_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7972 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/compute_summary_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9666 2024-03-04 16:17:41.000000 gns3-gui-3.0.0b2/gns3/console_cmd.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9947 2023-07-31 08:35:08.000000 gns3-gui-3.0.0b2/gns3/console_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17467 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/controller.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6351 2024-04-07 11:41:17.000000 gns3-gui-3.0.0b2/gns3/crash_report.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.080205 gns3-gui-3.0.0b2/gns3/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1197 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/about_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32085 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/appliance_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/capture_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2339 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/configuration_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5661 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/console_command_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8429 2022-11-02 16:17:56.000000 gns3-gui-3.0.0b2/gns3/dialogs/custom_adapters_configuration_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7834 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/doctor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3310 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/edit_compute_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6711 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/edit_project_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1993 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/exec_command_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4830 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/export_debug_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/file_editor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7036 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/filter_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3579 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/idlepc_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6486 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/image_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/login_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11851 2023-07-03 09:11:41.000000 gns3-gui-3.0.0b2/gns3/dialogs/new_template_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1879 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/node_info_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11399 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/node_properties_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/notif_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9036 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/preferences_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3788 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/profile_select.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14147 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/project_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9689 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/project_export_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3411 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/project_welcome_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11056 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/setup_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2457 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/show_readme_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5704 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/snapshots_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7860 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/style_editor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4838 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/dialogs/style_editor_dialog_link.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7859 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/symbol_selection_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4714 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/dialogs/text_editor_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7243 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/vm_with_images_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6675 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/dialogs/vm_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    70504 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/graphics_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32258 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/http_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1690 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/http_client_error.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8433 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/image_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2347 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/image_upload_manager.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.088205 gns3-gui-3.0.0b2/gns3/items/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10076 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/items/drawing_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/ellipse_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10344 2023-05-14 07:10:13.000000 gns3-gui-3.0.0b2/gns3/items/ethernet_link_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2428 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/image_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8318 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/label_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7141 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/line_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21450 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/items/link_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4404 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/logo_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19182 2024-03-04 16:17:41.000000 gns3-gui-3.0.0b2/gns3/items/node_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3125 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/items/rectangle_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7942 2023-05-14 07:10:13.000000 gns3-gui-3.0.0b2/gns3/items/serial_link_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7539 2023-11-03 04:55:32.000000 gns3-gui-3.0.0b2/gns3/items/shape_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6164 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/text_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1058 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/items/utils.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18698 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/link.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/applications/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      282 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/applications/gns3.desktop
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1152 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/gns3-gui.xml
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/16x16/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/16x16/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      832 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/16x16/apps/gns3.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/32x32/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/32x32/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1905 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/32x32/apps/gns3.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/apps/gns3.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6075 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4500 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.032205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/apps/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/apps/gns3.svg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.092205 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22534 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11492 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19682 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/local_config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21632 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/local_server.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/logger.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12548 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/main.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    56561 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/main_window.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.096205 gns3-gui-3.0.0b2/gns3/modules/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1095 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.096205 gns3-gui-3.0.0b2/gns3/modules/builtin/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4854 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5614 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/atm_switch.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5123 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/cloud.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.100206 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/cloud_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1930 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2891 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ethernet_hub.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4557 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ethernet_switch.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4085 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/frame_relay_switch.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2437 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/nat.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.104205 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7683 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/atm_switch_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2595 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/builtin_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22227 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/cloud_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9871 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/cloud_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5598 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9707 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10385 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6627 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1750 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.116206 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9107 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/atm_switch_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13163 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2666 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/builtin_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3269 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/builtin_preferences_page_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    19129 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24391 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4401 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5315 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3433 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5232 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3876 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5670 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4431 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5536 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4186 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6247 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9148 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13299 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4397 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5674 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4222 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6343 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7303 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11148 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.120206 gns3-gui-3.0.0b2/gns3/modules/builtin/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/utils/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1212 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/builtin/utils/tree_widget_item.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.120206 gns3-gui-3.0.0b2/gns3/modules/docker/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4407 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.120206 gns3-gui-3.0.0b2/gns3/modules/docker/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5356 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/dialogs/docker_vm_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5188 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/docker_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.120206 gns3-gui-3.0.0b2/gns3/modules/docker/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1968 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9394 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12700 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1385 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.128206 gns3-gui-3.0.0b2/gns3/modules/docker/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2400 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2852 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12930 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17480 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4709 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11020 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16543 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_wizard_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.132206 gns3-gui-3.0.0b2/gns3/modules/dynamips/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7828 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2360 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/adapters.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.132206 gns3-gui-3.0.0b2/gns3/modules/dynamips/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17596 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/dialogs/ios_router_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.136206 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1759 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c1700.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2320 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c2600.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c2691.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2022-12-24 09:42:12.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3600.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3725.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3745.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1885 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c7200.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2218 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/etherswitch_router.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12170 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/router.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.136206 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/dynamips_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27874 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/ios_router_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22638 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/ios_router_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7767 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.152206 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     6439 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/dynamips_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8491 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    35772 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    45950 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4850 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5957 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15247 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23315 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_wizard_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.160206 gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3261 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/decompress_ios.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2179 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/decompress_ios_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      905 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/dynamips/wics.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.160206 gns3-gui-3.0.0b2/gns3/modules/iou/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3974 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.160206 gns3-gui-3.0.0b2/gns3/modules/iou/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5044 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/dialogs/iou_device_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4930 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/iou_device.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.160206 gns3-gui-3.0.0b2/gns3/modules/iou/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13549 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_device_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15262 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_device_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5027 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1305 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/iou/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.168206 gns3-gui-3.0.0b2/gns3/modules/iou/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    13890 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17361 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4638 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5659 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6717 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9276 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2927 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3557 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4403 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/module.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1066 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/module_error.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.168206 gns3-gui-3.0.0b2/gns3/modules/qemu/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5394 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.168206 gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8102 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/qemu_image_wizard.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4777 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/qemu_vm_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.172206 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2896 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30797 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15366 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7651 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/qemu_vm.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2075 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.176206 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23636 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_image_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29391 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_image_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2888 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3655 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_preferences_page_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    33160 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    44174 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4602 2021-10-08 05:49:21.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5444 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12608 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18678 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.176206 gns3-gui-3.0.0b2/gns3/modules/virtualbox/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5807 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.176206 gns3-gui-3.0.0b2/gns3/modules/virtualbox/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.180206 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4001 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11547 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10054 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1438 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.184206 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3684 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4480 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    10804 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4373 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3801 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5833 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4953 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/virtualbox/virtualbox_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.188206 gns3-gui-3.0.0b2/gns3/modules/vmware/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10348 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.188206 gns3-gui-3.0.0b2/gns3/modules/vmware/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3586 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/dialogs/vmware_vm_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.192206 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5647 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11191 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_vm_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10397 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1731 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.200206 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7503 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8865 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9806 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13005 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4329 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5270 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3802 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5702 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6181 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vmware/vmware_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.200206 gns3-gui-3.0.0b2/gns3/modules/vpcs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4669 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/__init__.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.200206 gns3-gui-3.0.0b2/gns3/modules/vpcs/dialogs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/dialogs/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.204207 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7092 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9365 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3671 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1064 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/settings.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.208207 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4135 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6719 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4278 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4868 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3424 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5202 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3653 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4263 2022-07-11 22:23:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3367 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/modules/vpcs/vpcs_node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1630 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/network_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29284 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1513 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/nodes_dock_widget.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9340 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/nodes_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11255 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/packet_capture.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.208207 gns3-gui-3.0.0b2/gns3/pages/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/pages/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15586 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/pages/controller_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21008 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/pages/general_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8468 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/pages/gns3_vm_preferences_page.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/pages/packet_capture_preferences_page.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.212206 gns3-gui-3.0.0b2/gns3/ports/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      857 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/ethernet_port.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8108 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/port.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2335 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/port_name_factory.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      887 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ports/serial_port.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10489 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/progress.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25349 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/project.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12152 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/pycutext.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.212206 gns3-gui-3.0.0b2/gns3/qt/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6678 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/qt/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5143 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/qt/qimage_svg_renderer.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.216207 gns3-gui-3.0.0b2/gns3/registry/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/registry/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9946 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/appliance.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12895 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/appliance_to_template.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2646 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4251 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/image.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4698 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/registry/registry.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.216207 gns3-gui-3.0.0b2/gns3/schemas/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15780 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/schemas/appliance.json
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23629 2024-01-27 06:07:27.000000 gns3-gui-3.0.0b2/gns3/schemas/appliance_v8.json
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19651 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/settings.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2766 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/spice_console.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.220207 gns3-gui-3.0.0b2/gns3/static/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/static/.keep
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2732 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/status_bar.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/style.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1234 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/symbol.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6213 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/telnet_console.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/template.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8535 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/template_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20587 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/topology.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15220 2023-07-31 08:35:08.000000 gns3-gui-3.0.0b2/gns3/topology_summary_view.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.276207 gns3-gui-3.0.0b2/gns3/ui/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/__init__.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    96556 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/about_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   112145 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/about_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10358 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/appliance_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12795 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/appliance_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3516 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/capture_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4471 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/capture_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3197 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/configuration_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/configuration_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5108 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/ui/console_command_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/ui/console_command_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    20055 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/controller_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24755 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/controller_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2012 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/custom_adapters_configuration_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2258 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/custom_adapters_configuration_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3252 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/doctor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3521 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/doctor_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5487 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/edit_compute_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6478 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/edit_compute_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9096 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/edit_project_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11089 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/edit_project_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     1694 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/exec_command_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1648 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/exec_command_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3559 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/export_debug_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3716 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/export_debug_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5607 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/export_project_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8170 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/export_project_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3422 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/file_editor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/file_editor_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3881 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/filter_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3708 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/filter_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    43663 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/general_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54735 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/general_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7845 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/gns3_vm_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10781 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/gns3_vm_preferences_page_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1824 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/idlepc_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1919 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/idlepc_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3693 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/image_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3823 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/image_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2758 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/login_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2734 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/login_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    41762 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/main_window.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    50875 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/main_window_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3059 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/new_template_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4766 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/new_template_wizard_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2636 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/node_info_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/node_info_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/node_properties_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5071 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/node_properties_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     4492 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/ui/packet_capture_preferences_page.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7011 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/ui/packet_capture_preferences_page_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4704 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/preferences_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4996 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/preferences_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4950 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/profile_select_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5375 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/profile_select_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/project_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11436 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/project_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2754 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/project_welcome_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3385 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/project_welcome_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)  9439247 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/resources_rc.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7770 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/setup_wizard.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11373 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/setup_wizard_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     2778 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/show_readme_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2882 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/ui/show_readme_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2357 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/snapshots_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2588 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/snapshots_dialog_ui.py
--rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     6586 2023-11-03 04:55:32.000000 gns3-gui-3.0.0b2/gns3/ui/style_editor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8330 2023-11-03 04:55:32.000000 gns3-gui-3.0.0b2/gns3/ui/style_editor_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/symbol_selection_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5838 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/symbol_selection_dialog_ui.py
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4884 2020-11-07 04:27:16.000000 gns3-gui-3.0.0b2/gns3/ui/text_editor_dialog.ui
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/ui/text_editor_dialog_ui.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11356 2024-01-11 02:03:24.000000 gns3-gui-3.0.0b2/gns3/update_manager.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.284207 gns3-gui-3.0.0b2/gns3/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3691 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/utils/__init__.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1294 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/utils/authorize_ubridge.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2799 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/bring_to_front.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/file_copy_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1326 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/get_icon.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1528 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/utils/get_resource.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/utils/import_project_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3816 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/gns3/utils/install_mime_types.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/interfaces.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2295 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/utils/macos_ubridge_setuid.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1256 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/normalize_filename.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5435 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/process_files_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6405 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/progress_dialog.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1975 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/run_in_terminal.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2524 2023-06-21 10:04:51.000000 gns3-gui-3.0.0b2/gns3/utils/server_select.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4424 2023-08-14 02:01:18.000000 gns3-gui-3.0.0b2/gns3/utils/sudo.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2420 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/wait_for_command_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2713 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/wait_for_connection_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2288 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/wait_for_lambda_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2850 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/gns3/utils/wait_for_runas_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1490 2024-04-07 11:42:46.000000 gns3-gui-3.0.0b2/gns3/version.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2771 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/gns3/vnc_console.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.604210 gns3-gui-3.0.0b2/gns3_gui.egg-info/
--rw-r--r--   0 grossmj   (1000) grossmj   (1000)    43930 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/PKG-INFO
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    30105 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/SOURCES.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        1 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/dependency_links.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)       36 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/entry_points.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)      235 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/requires.txt
--rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        5 2024-04-07 12:41:31.000000 gns3-gui-3.0.0b2/gns3_gui.egg-info/top_level.txt
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1683 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/pyproject.toml
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      217 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/requirements.txt
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.288207 gns3-gui-3.0.0b2/resources/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.328208 gns3-gui-3.0.0b2/resources/charcoal_icons/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6231 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1-cancel.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-note-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/add-note.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2879 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/aux-console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/aux-console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/browse-all-icons-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/browse-all-icons.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13891 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/calculate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/calculate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2220 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/camera-photo-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2127 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/camera-photo.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/capture-start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/capture-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3369 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/capture-stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3362 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/capture-stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/command_line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6261 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/command_line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/configuration-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8406 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/configuration.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/console_edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/console_edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4172 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/delete-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4156 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/delete.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2881 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/duplicate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/duplicate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3852 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3846 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/ellipse-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/ellipse.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/export-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2822 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/export.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24996 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/filter-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/filter-reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25640 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/filter-reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24989 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/filter.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/firewall-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/firewall.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2141 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/front-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/front.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12619 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/help-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12581 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/help.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/image-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/image.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/import-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/import.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/import_export_configs-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/import_export_configs.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2409 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/inspect-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2403 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/inspect.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3738 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/lock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3730 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/lock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3546 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/lower_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/lower_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/minus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/minus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/new-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4223 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/new-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/node_conception-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/node_conception.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/open-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/open.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/pause-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/pc-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/pc.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2680 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/plus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2673 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/plus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6090 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/preferences-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6084 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/preferences.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5543 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/quit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5870 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/quit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/raise_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3542 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/raise_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/rectangle-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/rectangle.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/reload-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/reload.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2181 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2175 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/router-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/router.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5279 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/save-as-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5281 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/save-as-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/save-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/save-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/show-hostname-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/show-hostname.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/show-interface-names-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/show-interface-names.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/snapshot-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/snapshot.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2684 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/switch-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2648 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/unlock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/unlock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-in-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-in.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2808 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-out-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1746 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-out.svg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.364208 gns3-gui-3.0.0b2/resources/classic_icons/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5935 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-link-cancel.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2971 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-link-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3086 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-link.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4148 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-note-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4315 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/add-note.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2593 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/aux-console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2589 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/aux-console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/browse-all-icons-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5646 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/browse-all-icons.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13890 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/calculate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/calculate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2992 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/camera-photo-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2914 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/camera-photo.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/capture-start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/capture-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3368 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/capture-stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3363 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/capture-stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/command_line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6254 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/command_line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/configuration-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8405 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/configuration.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2046 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/console-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2070 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/console_edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/console_edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4162 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/delete-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4143 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/delete.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2885 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/duplicate-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/duplicate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3856 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/edit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3857 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4312 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/ellipse-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4321 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/ellipse.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/export-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/export.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24995 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/filter-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/filter-reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25639 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/filter-reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24990 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/filter.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2047 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/firewall-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2056 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/firewall.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/front-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/front.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9629 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/help-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9625 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/help.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2011 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/image-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2020 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/image.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/import-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/import.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2351 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/import_export_configs-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2375 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/import_export_configs.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2373 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/inspect-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2382 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/inspect.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/line-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/lock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3731 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/lock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3545 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/lower_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/lower_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/minus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/minus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4249 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/new-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4245 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/new-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/node_conception-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/node_conception.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2243 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/open-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2261 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/open.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/pause-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2166 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3496 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/pc-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3493 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/pc.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2679 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/plus-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2674 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/plus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5725 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/preferences-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5719 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/preferences.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5032 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/quit-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5026 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/quit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/raise_z_value-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3541 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/raise_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2530 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/rectangle-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2539 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/rectangle.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2266 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/reload-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2275 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/reload.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2180 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/reset-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2174 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2313 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/router-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2322 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/router.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4710 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/save-as-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4748 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/save-as-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3383 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/save-project-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3417 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/save-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/show-hostname-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/show-hostname.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3636 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/show-interface-names-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3686 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/show-interface-names.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2876 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/snapshot-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2901 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/snapshot.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1742 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2495 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/switch-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/unlock-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/unlock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2761 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/zoom-in-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2785 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/zoom-in.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2719 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/zoom-out-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2727 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/classic_icons/zoom-out.svg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.472209 gns3-gui-3.0.0b2/resources/icons/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    63187 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/PC-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    60045 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/PC.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    28134 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/add-note.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16099 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/applications.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21937 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/aux-console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   291074 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/browse-all-icons-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   297712 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/browse-all-icons.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32570 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/calculate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39042 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/camera-photo-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    37642 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/camera-photo.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25560 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/cancel-connection.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12039 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/cancel.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18737 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/capture-start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31090 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/capture-stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26448 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/command_line.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19139 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/configuration.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23701 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/connection-new-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23702 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/connection-new.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21216 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/console.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30385 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/console_edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13772 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/delete.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/dialog-warning.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26729 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/drawing.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23490 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/duplicate.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16831 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/edit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24733 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/ellipse-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21372 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/ellipse.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10572 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/export.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21681 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/filter-capture.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27285 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/filter-reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23917 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/filter.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    57273 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/firewall-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    53702 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/firewall.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8975 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/front.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13259 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/help.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7175 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/horizontally.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19675 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/image.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10549 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/import.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39319 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/import_export_configs.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15756 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/inspect.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10184 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/led_gray.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10135 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/led_green.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6952 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/led_red.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9965 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/led_yellow.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32132 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/lock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6518 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/lower_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4612 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/minus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24126 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/new-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16626 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/new.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27187 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/node_conception.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30745 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/open.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23462 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/icons/pause-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21534 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/icons/pause.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4975 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/plus.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19130 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/quit.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7903 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/raise_z_value.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35282 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/rectangle-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31055 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/rectangle.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16810 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/reload.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8571 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/reset.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    58719 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/router-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54133 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/router.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3184 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/rtv.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    40599 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/save-as-project.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31854 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/save-as.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29835 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/save.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15166 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/show-hostname.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26306 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/show-interface-names.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/snapshot.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18013 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/start-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17454 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/start.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/stop-hover.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/stop.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    67991 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/switch-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    64865 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/switch.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    34969 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/unlock.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5816 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/vertically.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/virtualbox.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/warning.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1906 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/wireshark.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5939 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/zoom-in-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6276 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/zoom-in.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5975 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/zoom-out-hover.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6157 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/icons/zoom-out.png
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.476209 gns3-gui-3.0.0b2/resources/images/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   370070 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/images/gns3.ico
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7892 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/images/gns3_icon_128x128.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16745 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/images/gns3_icon_256x256.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7921 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/images/gns3_logo.png
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16025 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/resources.qrc
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.476209 gns3-gui-3.0.0b2/resources/styles/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1231 2023-08-10 12:50:05.000000 gns3-gui-3.0.0b2/resources/styles/charcoal.css
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.476209 gns3-gui-3.0.0b2/resources/symbols/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16298 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/atm_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    78565 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/cloud.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/computer.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19782 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/docker_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18650 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/ethernet_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18401 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/firewall.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18343 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/frame_relay_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18128 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/hub.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19150 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/multilayer_switch.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18421 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/qemu_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18494 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/router.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16401 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/vbox_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16843 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/vmware_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/resources/symbols/vpcs_guest.svg
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       38 2024-04-07 12:41:31.608210 gns3-gui-3.0.0b2/setup.cfg
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.492209 gns3-gui-3.0.0b2/tests/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6326 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/conftest.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.492209 gns3-gui-3.0.0b2/tests/items/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1997 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/items/test_ellipse_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1509 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/items/test_image_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2106 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/items/test_label_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4449 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/items/test_line_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3046 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/items/test_rectangle_item.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2039 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/items/test_text_item.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.036205 gns3-gui-3.0.0b2/tests/modules/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.492209 gns3-gui-3.0.0b2/tests/modules/docker/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1478 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/docker/test_docker_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.496209 gns3-gui-3.0.0b2/tests/modules/dynamips/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1486 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/dynamips/test_dynamips_init.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.496209 gns3-gui-3.0.0b2/tests/modules/iou/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1841 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/iou/test_iou_device.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.496209 gns3-gui-3.0.0b2/tests/modules/qemu/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1526 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/qemu/test_qemu_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.500209 gns3-gui-3.0.0b2/tests/modules/virtualbox/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1574 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/virtualbox/test_virtualbox_vm.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.500209 gns3-gui-3.0.0b2/tests/modules/vpcs/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1637 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/modules/vpcs/test_vpcs_device.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.500209 gns3-gui-3.0.0b2/tests/qt/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1285 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/qt/test_qimage_svg_renderer.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.504209 gns3-gui-3.0.0b2/tests/registry/
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.532210 gns3-gui-3.0.0b2/tests/registry/appliances/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2607 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/arista-veos-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2451 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/arista-veos.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1353 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/broken-microcore-linux.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/cisco-3745-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1356 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/cisco-3745.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1171 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/cisco-iou-l3-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1019 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/cisco-iou-l3.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4047 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/empty-vm-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1612 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/juniper-vsrx.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2022 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/microcore-linux.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1216 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/openvswitch-v8.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1096 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/registry/appliances/openvswitch.gns3a
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9480 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/registry/test_appliance.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13248 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/registry/test_appliance_to_template.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2895 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/registry/test_config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2304 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/registry/test_image.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2185 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/registry/test_registry.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1376 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_compute.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5810 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_compute_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1717 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_controller.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1354 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_graphics_view.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8696 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_http_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3087 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_image_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1596 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_image_upload_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4739 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_link.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13656 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_local_config.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2980 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_local_server.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1760 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_main_window.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1184 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_network_client.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5698 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_node.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1496 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_progress.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5498 2024-04-07 05:43:49.000000 gns3-gui-3.0.0b2/tests/test_project.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2574 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/tests/test_spice_console.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_topology.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3575 2023-09-19 14:06:34.000000 gns3-gui-3.0.0b2/tests/test_update_manager.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1592 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/test_utils.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-11-06 07:06:12.000000 gns3-gui-3.0.0b2/tests/test_vnc_console.py
-drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-04-07 12:41:31.588210 gns3-gui-3.0.0b2/tests/utils/
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1394 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/utils/test_file_copy_worker.py
--rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3705 2022-07-11 22:23:48.000000 gns3-gui-3.0.0b2/tests/utils/test_server_select.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.505358 gns3_gui-3.0.0b3/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   120106 2024-05-19 10:23:05.000000 gns3_gui-3.0.0b3/CHANGELOG
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35147 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/LICENSE
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      138 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/MANIFEST.in
+-rw-r--r--   0 grossmj   (1000) grossmj   (1000)    43886 2024-05-19 10:32:57.505358 gns3_gui-3.0.0b3/PKG-INFO
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1714 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/README.md
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       94 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/dev-requirements.txt
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:56.981360 gns3_gui-3.0.0b3/gns3/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       33 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      736 2024-02-12 05:00:39.000000 gns3_gui-3.0.0b3/gns3/__main__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3456 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/appliance_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3017 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/application.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8604 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/base_node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5711 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/compute.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9953 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/compute_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7972 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/compute_summary_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9666 2024-03-04 16:17:41.000000 gns3_gui-3.0.0b3/gns3/console_cmd.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9947 2023-07-31 08:35:08.000000 gns3_gui-3.0.0b3/gns3/console_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17584 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/controller.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6351 2024-05-19 10:20:09.000000 gns3_gui-3.0.0b3/gns3/crash_report.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.013360 gns3_gui-3.0.0b3/gns3/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1197 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/about_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32085 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/appliance_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2661 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/capture_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2339 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/configuration_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5661 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/console_command_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8429 2022-11-02 16:17:56.000000 gns3_gui-3.0.0b3/gns3/dialogs/custom_adapters_configuration_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7834 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/doctor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3310 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/edit_compute_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6711 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/edit_project_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1993 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/exec_command_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4830 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/export_debug_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/file_editor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7036 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/filter_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3579 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/idlepc_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6486 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/image_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/login_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11851 2023-07-03 09:11:41.000000 gns3_gui-3.0.0b3/gns3/dialogs/new_template_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1879 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/node_info_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11399 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/node_properties_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5905 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/notif_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9036 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/preferences_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3788 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/profile_select.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14147 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/project_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9689 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/project_export_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3411 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/project_welcome_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11056 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/setup_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2457 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/show_readme_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5704 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/snapshots_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7860 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/style_editor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4838 2023-08-14 02:01:18.000000 gns3_gui-3.0.0b3/gns3/dialogs/style_editor_dialog_link.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7859 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/symbol_selection_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4714 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/dialogs/text_editor_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7243 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/vm_with_images_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6675 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/dialogs/vm_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    70504 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/graphics_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32258 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/http_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1690 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/http_client_error.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8433 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/image_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2347 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/image_upload_manager.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.025360 gns3_gui-3.0.0b3/gns3/items/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/items/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10076 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/items/drawing_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2145 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/items/ellipse_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10344 2023-05-14 07:10:13.000000 gns3_gui-3.0.0b3/gns3/items/ethernet_link_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2428 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/items/image_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8318 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/items/label_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7141 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/items/line_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21450 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/items/link_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4404 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/items/logo_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19182 2024-03-04 16:17:41.000000 gns3_gui-3.0.0b3/gns3/items/node_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3125 2023-08-14 02:01:18.000000 gns3_gui-3.0.0b3/gns3/items/rectangle_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7942 2023-05-14 07:10:13.000000 gns3_gui-3.0.0b3/gns3/items/serial_link_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7539 2023-11-03 04:55:32.000000 gns3_gui-3.0.0b3/gns3/items/shape_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6164 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/items/text_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1058 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/items/utils.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18698 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/link.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.025360 gns3_gui-3.0.0b3/gns3/linux/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.025360 gns3_gui-3.0.0b3/gns3/linux/applications/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      282 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/applications/gns3.desktop
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1152 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/gns3-gui.xml
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:56.953360 gns3_gui-3.0.0b3/gns3/linux/icons/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:56.953360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:56.953360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/16x16/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.029360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/16x16/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      832 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/16x16/apps/gns3.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:56.953360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/32x32/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.029360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/32x32/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1905 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/32x32/apps/gns3.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:56.953360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.029360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/apps/gns3.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.029360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/mimetypes/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6075 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4500 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:56.953360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.029360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/apps/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/apps/gns3.svg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.029360 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/mimetypes/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8950 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22534 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11492 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19682 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/local_config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21632 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/local_server.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4354 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/logger.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12548 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/main.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    56561 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/main_window.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.033360 gns3_gui-3.0.0b3/gns3/modules/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1095 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.033360 gns3_gui-3.0.0b3/gns3/modules/builtin/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4854 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5614 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/atm_switch.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5123 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/cloud.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.033360 gns3_gui-3.0.0b3/gns3/modules/builtin/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/dialogs/cloud_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1930 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2891 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ethernet_hub.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4557 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ethernet_switch.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4085 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/frame_relay_switch.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2435 2024-05-16 10:32:52.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/nat.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.041360 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7683 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/atm_switch_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2595 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/builtin_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22227 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/cloud_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9871 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/cloud_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5598 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9707 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10385 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6627 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1750 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.061360 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9107 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/atm_switch_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13163 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2666 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/builtin_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3269 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/builtin_preferences_page_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    19129 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24391 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4401 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5315 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3433 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5232 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3876 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5670 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4431 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5536 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4186 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6247 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9148 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13299 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4397 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5674 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4222 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6343 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7303 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11148 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.061360 gns3_gui-3.0.0b3/gns3/modules/builtin/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/utils/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1212 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/builtin/utils/tree_widget_item.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.065359 gns3_gui-3.0.0b3/gns3/modules/docker/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4407 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.065359 gns3_gui-3.0.0b3/gns3/modules/docker/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5356 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/docker/dialogs/docker_vm_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5188 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/docker/docker_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.065359 gns3_gui-3.0.0b3/gns3/modules/docker/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1968 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/pages/docker_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9394 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/docker/pages/docker_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12700 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/docker/pages/docker_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1385 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/docker/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.077359 gns3_gui-3.0.0b3/gns3/modules/docker/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/ui/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2400 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2852 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12930 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17480 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4709 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5671 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11020 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16543 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_wizard_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.077359 gns3_gui-3.0.0b3/gns3/modules/dynamips/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7828 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2360 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/adapters.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.077359 gns3_gui-3.0.0b3/gns3/modules/dynamips/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17596 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/dialogs/ios_router_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.085359 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1759 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c1700.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2320 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c2600.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c2691.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2022-12-24 09:42:12.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c3600.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c3725.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1538 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c3745.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1885 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c7200.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2218 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/etherswitch_router.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12128 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/router.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.089359 gns3_gui-3.0.0b3/gns3/modules/dynamips/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5637 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/pages/dynamips_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27874 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/pages/ios_router_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    22638 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/pages/ios_router_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7767 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.101359 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     6439 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/dynamips_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8491 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    35772 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    45950 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4850 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5957 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15247 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23315 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_wizard_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.109359 gns3_gui-3.0.0b3/gns3/modules/dynamips/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/utils/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3261 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/utils/decompress_ios.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2179 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/utils/decompress_ios_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      905 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/dynamips/wics.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.109359 gns3_gui-3.0.0b3/gns3/modules/iou/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3974 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.109359 gns3_gui-3.0.0b3/gns3/modules/iou/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5044 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/iou/dialogs/iou_device_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4930 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/iou/iou_device.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.109359 gns3_gui-3.0.0b3/gns3/modules/iou/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13549 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/iou/pages/iou_device_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15262 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/iou/pages/iou_device_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5027 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/pages/iou_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1305 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/iou/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.125359 gns3_gui-3.0.0b3/gns3/modules/iou/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    13890 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17361 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4638 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5659 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6717 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9276 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2927 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3557 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4403 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/module.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1066 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/module_error.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.125359 gns3_gui-3.0.0b3/gns3/modules/qemu/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5394 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.125359 gns3_gui-3.0.0b3/gns3/modules/qemu/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8102 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/dialogs/qemu_image_wizard.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4777 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/dialogs/qemu_vm_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.129359 gns3_gui-3.0.0b3/gns3/modules/qemu/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2896 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/pages/qemu_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30797 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/pages/qemu_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15366 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/pages/qemu_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7651 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/qemu_vm.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2075 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.137359 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23636 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_image_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29391 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_image_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2888 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3655 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_preferences_page_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    33160 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    44174 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4602 2021-10-08 05:49:21.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5444 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12608 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18678 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.137359 gns3_gui-3.0.0b3/gns3/modules/virtualbox/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5807 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.137359 gns3_gui-3.0.0b3/gns3/modules/virtualbox/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.137359 gns3_gui-3.0.0b3/gns3/modules/virtualbox/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4001 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11547 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10054 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1438 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.141359 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3684 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4480 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    10804 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    14637 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4373 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3801 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5833 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4953 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/virtualbox/virtualbox_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.141359 gns3_gui-3.0.0b3/gns3/modules/vmware/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10348 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.141359 gns3_gui-3.0.0b3/gns3/modules/vmware/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3586 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/dialogs/vmware_vm_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.141359 gns3_gui-3.0.0b3/gns3/modules/vmware/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5647 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/pages/vmware_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11191 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/pages/vmware_vm_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10397 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/pages/vmware_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1731 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.149359 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7503 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8865 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     9806 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13005 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4329 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5270 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3802 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5702 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6181 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vmware/vmware_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.149359 gns3_gui-3.0.0b3/gns3/modules/vpcs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4669 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/__init__.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.149359 gns3_gui-3.0.0b3/gns3/modules/vpcs/dialogs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/dialogs/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1678 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.149359 gns3_gui-3.0.0b3/gns3/modules/vpcs/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7092 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9365 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3671 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/pages/vpcs_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1064 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/settings.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.153359 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4135 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6719 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4278 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4868 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3424 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5202 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3653 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4263 2022-07-11 22:23:49.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3367 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/modules/vpcs/vpcs_node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1630 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/network_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29284 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1513 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/nodes_dock_widget.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9340 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/nodes_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11255 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/gns3/packet_capture.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.157359 gns3_gui-3.0.0b3/gns3/pages/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/pages/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15586 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/pages/controller_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21008 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/pages/general_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8468 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/pages/gns3_vm_preferences_page.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/pages/packet_capture_preferences_page.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.161359 gns3_gui-3.0.0b3/gns3/ports/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ports/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      857 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ports/ethernet_port.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8108 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ports/port.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2335 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ports/port_name_factory.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      887 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ports/serial_port.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10489 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/progress.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25466 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/project.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12152 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/pycutext.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.161359 gns3_gui-3.0.0b3/gns3/qt/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6678 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/qt/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5143 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/qt/qimage_svg_renderer.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.161359 gns3_gui-3.0.0b3/gns3/registry/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/registry/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9946 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/registry/appliance.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12895 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/registry/appliance_to_template.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2646 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/registry/config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4251 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/registry/image.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4698 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/registry/registry.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.165359 gns3_gui-3.0.0b3/gns3/schemas/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15780 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/gns3/schemas/appliance.json
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23629 2024-01-27 06:07:27.000000 gns3_gui-3.0.0b3/gns3/schemas/appliance_v8.json
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19651 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/settings.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2766 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/gns3/spice_console.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.165359 gns3_gui-3.0.0b3/gns3/static/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/static/.keep
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2732 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/status_bar.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/style.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1234 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/symbol.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6213 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/gns3/telnet_console.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3592 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/template.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8535 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/template_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20587 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/topology.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15220 2023-07-31 08:35:08.000000 gns3_gui-3.0.0b3/gns3/topology_summary_view.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.193359 gns3_gui-3.0.0b3/gns3/ui/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)        0 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/__init__.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    96556 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/about_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   112145 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/about_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10358 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/appliance_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12795 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/appliance_wizard_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     3401 2024-05-16 10:33:07.000000 gns3_gui-3.0.0b3/gns3/ui/capture_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4472 2024-05-16 10:33:07.000000 gns3_gui-3.0.0b3/gns3/ui/capture_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3197 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/configuration_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3662 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/configuration_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5108 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/gns3/ui/console_command_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/gns3/ui/console_command_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    20055 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/controller_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24755 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/controller_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2012 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/custom_adapters_configuration_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2258 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/custom_adapters_configuration_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3252 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/doctor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3521 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/doctor_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5487 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/edit_compute_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6478 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/edit_compute_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9096 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/edit_project_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11089 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/edit_project_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     1694 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/exec_command_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1648 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/exec_command_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3559 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/export_debug_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3716 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/export_debug_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5607 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/export_project_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8170 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/export_project_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3422 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/file_editor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3350 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/file_editor_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     3881 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/filter_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3708 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/filter_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)    43663 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/general_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54735 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/general_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     7845 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/gns3_vm_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10781 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/gns3_vm_preferences_page_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1824 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/idlepc_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1919 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/idlepc_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3693 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/image_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3823 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/image_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2758 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/login_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2734 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/login_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    41762 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/main_window.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    50875 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/main_window_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3059 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/new_template_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4766 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/new_template_wizard_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2636 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/node_info_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/node_info_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/node_properties_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5071 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/node_properties_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     4492 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/gns3/ui/packet_capture_preferences_page.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7011 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/gns3/ui/packet_capture_preferences_page_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4704 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/preferences_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4996 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/preferences_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4950 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/profile_select_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5375 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/profile_select_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10431 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/project_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11436 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/project_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2754 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/project_welcome_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3385 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/project_welcome_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)  9439247 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/resources_rc.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7770 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/setup_wizard.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11373 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/setup_wizard_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     2778 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/show_readme_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2882 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/ui/show_readme_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     2357 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/snapshots_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2588 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/snapshots_dialog_ui.py
+-rwxrwxr-x   0 grossmj   (1000) grossmj   (1000)     6586 2023-11-03 04:55:32.000000 gns3_gui-3.0.0b3/gns3/ui/style_editor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8330 2023-11-03 04:55:32.000000 gns3_gui-3.0.0b3/gns3/ui/style_editor_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     5053 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/symbol_selection_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5838 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/symbol_selection_dialog_ui.py
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)     4884 2020-11-07 04:27:16.000000 gns3_gui-3.0.0b3/gns3/ui/text_editor_dialog.ui
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5836 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/ui/text_editor_dialog_ui.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    11356 2024-01-11 02:03:24.000000 gns3_gui-3.0.0b3/gns3/update_manager.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.201359 gns3_gui-3.0.0b3/gns3/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3691 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/utils/__init__.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1294 2023-08-14 02:01:18.000000 gns3_gui-3.0.0b3/gns3/utils/authorize_ubridge.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2799 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/bring_to_front.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/file_copy_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1326 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/get_icon.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1528 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/utils/get_resource.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2111 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/utils/import_project_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3816 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/gns3/utils/install_mime_types.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6592 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/interfaces.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2295 2023-08-14 02:01:18.000000 gns3_gui-3.0.0b3/gns3/utils/macos_ubridge_setuid.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1256 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/normalize_filename.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5435 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/process_files_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6405 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/progress_dialog.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1975 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/run_in_terminal.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2524 2023-06-21 10:04:51.000000 gns3_gui-3.0.0b3/gns3/utils/server_select.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4424 2023-08-14 02:01:18.000000 gns3_gui-3.0.0b3/gns3/utils/sudo.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2420 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/wait_for_command_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2713 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/wait_for_connection_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2288 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/wait_for_lambda_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2850 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/gns3/utils/wait_for_runas_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1490 2024-05-19 10:23:05.000000 gns3_gui-3.0.0b3/gns3/version.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2771 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/gns3/vnc_console.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.501357 gns3_gui-3.0.0b3/gns3_gui.egg-info/
+-rw-r--r--   0 grossmj   (1000) grossmj   (1000)    43886 2024-05-19 10:32:56.000000 gns3_gui-3.0.0b3/gns3_gui.egg-info/PKG-INFO
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)    30131 2024-05-19 10:32:56.000000 gns3_gui-3.0.0b3/gns3_gui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        1 2024-05-19 10:32:56.000000 gns3_gui-3.0.0b3/gns3_gui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)       36 2024-05-19 10:32:56.000000 gns3_gui-3.0.0b3/gns3_gui.egg-info/entry_points.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)      233 2024-05-19 10:32:56.000000 gns3_gui-3.0.0b3/gns3_gui.egg-info/requires.txt
+-rwxrwxrwx   0 grossmj   (1000) grossmj   (1000)        5 2024-05-19 10:32:56.000000 gns3_gui-3.0.0b3/gns3_gui.egg-info/top_level.txt
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1642 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/pyproject.toml
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)      170 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/requirements.txt
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.201359 gns3_gui-3.0.0b3/resources/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.269358 gns3_gui-3.0.0b3/resources/charcoal_icons/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6231 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/add-link-1-cancel.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/add-link-1-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2182 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/add-link-1.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/add-note-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/add-note.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2879 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/aux-console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/aux-console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/browse-all-icons-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3497 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/browse-all-icons.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13891 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/calculate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/calculate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2220 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/camera-photo-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2127 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/camera-photo.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/capture-start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/capture-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3369 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/capture-stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3362 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/capture-stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/command_line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6261 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/command_line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/configuration-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8406 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/configuration.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1277 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/console_edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/console_edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4172 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/delete-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4156 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/delete.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2881 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/duplicate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/duplicate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3852 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3846 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/ellipse-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3430 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/ellipse.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/export-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2822 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/export.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24996 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/filter-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/filter-reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25640 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/filter-reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24989 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/filter.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/firewall-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1371 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/firewall.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2141 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/front-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/front.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12619 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/help-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12581 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/help.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/image-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1296 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/image.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/import-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2823 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/import.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/import_export_configs-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1559 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/import_export_configs.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2409 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/inspect-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2403 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/inspect.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3738 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/lock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3730 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/lock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3546 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/lower_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/lower_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/minus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/minus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4234 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/new-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4223 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/new-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/node_conception-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/node_conception.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/open-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1468 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/open.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/pause-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/pc-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1966 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/pc.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2680 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/plus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2673 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/plus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6090 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/preferences-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6084 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/preferences.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5543 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/quit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5870 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/quit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/raise_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3542 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/raise_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/rectangle-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1737 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/rectangle.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/reload-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1575 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/reload.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2181 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2175 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/router-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1582 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/router.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5279 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/save-as-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5281 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/save-as-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/save-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2222 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/save-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/show-hostname-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/show-hostname.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/show-interface-names-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2668 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/show-interface-names.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/snapshot-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2080 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/snapshot.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2684 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/switch-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2648 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/unlock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/unlock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/zoom-in-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1910 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/zoom-in.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2808 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/zoom-out-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1746 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/charcoal_icons/zoom-out.svg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.309358 gns3_gui-3.0.0b3/resources/classic_icons/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5935 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/add-link-cancel.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2971 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/add-link-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3086 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/add-link.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4148 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/add-note-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4315 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/add-note.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2593 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/aux-console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2589 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/aux-console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5534 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/browse-all-icons-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5646 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/browse-all-icons.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13890 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/calculate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13884 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/calculate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2992 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/camera-photo-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2914 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/camera-photo.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3102 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/capture-start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3096 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/capture-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3368 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/capture-stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3363 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/capture-stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6267 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/command_line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6254 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/command_line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/configuration-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8405 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/configuration.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2046 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/console-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2070 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6271 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/console_edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6265 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/console_edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4162 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/delete-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4143 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/delete.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2885 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/duplicate-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2880 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/duplicate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3856 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/edit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3857 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4312 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/ellipse-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4321 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/ellipse.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/export-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/export.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24995 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/filter-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25646 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/filter-reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25639 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/filter-reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24990 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/filter.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2047 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/firewall-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2056 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/firewall.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/front-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2135 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/front.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9629 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/help-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9625 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/help.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2011 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/image-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2020 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/image.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2843 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/import-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2837 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/import.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2351 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/import_export_configs-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2375 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/import_export_configs.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2373 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/inspect-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2382 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/inspect.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2786 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/line-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2780 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3737 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/lock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3731 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/lock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3545 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/lower_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3539 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/lower_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2227 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/minus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/minus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4249 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/new-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4245 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/new-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18976 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/node_conception-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18967 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/node_conception.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2243 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/open-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2261 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/open.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1430 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/pause-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2166 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3496 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/pc-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3493 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/pc.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2679 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/plus-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2674 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/plus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5725 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/preferences-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5719 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/preferences.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5032 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/quit-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5026 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/quit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3548 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/raise_z_value-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3541 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/raise_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2530 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/rectangle-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2539 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/rectangle.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2266 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/reload-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2275 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/reload.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2180 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/reset-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2174 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2313 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/router-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2322 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/router.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4710 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/save-as-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4748 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/save-as-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3383 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/save-project-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3417 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/save-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10613 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/show-hostname-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10607 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/show-hostname.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3636 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/show-interface-names-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3686 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/show-interface-names.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2876 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/snapshot-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2901 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/snapshot.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1000 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1742 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1034 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2495 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/switch-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2489 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4383 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/unlock-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4377 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/unlock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2761 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/zoom-in-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2785 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/zoom-in.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2719 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/zoom-out-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2727 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/classic_icons/zoom-out.svg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.397358 gns3_gui-3.0.0b3/resources/icons/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    63187 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/PC-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    60045 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/PC.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    28134 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/add-note.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16099 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/applications.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21937 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/aux-console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   291074 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/browse-all-icons-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   297712 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/browse-all-icons.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32570 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/calculate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39042 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/camera-photo-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    37642 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/camera-photo.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    25560 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/cancel-connection.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    12039 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/cancel.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18737 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/capture-start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31090 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/capture-stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26448 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/command_line.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19139 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/configuration.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23701 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/connection-new-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23702 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/connection-new.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21216 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/console.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30385 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/console_edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13772 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/delete.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/dialog-warning.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26729 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/drawing.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23490 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/duplicate.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16831 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/edit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24733 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/ellipse-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21372 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/ellipse.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10572 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/export.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21681 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/filter-capture.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27285 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/filter-reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23917 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/filter.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    57273 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/firewall-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    53702 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/firewall.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8975 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/front.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13259 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/help.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7175 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/horizontally.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19675 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/image.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10549 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/import.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    39319 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/import_export_configs.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15756 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/inspect.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10184 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/led_gray.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    10135 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/led_green.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6952 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/led_red.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9965 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/led_yellow.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    32132 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/lock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6518 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/lower_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4612 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/minus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    24126 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/new-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16626 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/new.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    27187 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/node_conception.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30745 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/open.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    23462 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/icons/pause-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    21534 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/icons/pause.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4975 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/plus.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19130 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/quit.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7903 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/raise_z_value.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    35282 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/rectangle-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31055 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/rectangle.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16810 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/reload.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8571 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/reset.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    58719 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/router-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    54133 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/router.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3184 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/rtv.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    40599 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/save-as-project.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    31854 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/save-as.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    29835 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/save.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    15166 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/show-hostname.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    26306 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/show-interface-names.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17574 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/snapshot.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18013 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/start-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    17454 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/start.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/stop-hover.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    20029 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/stop.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    67991 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/switch-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    64865 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/switch.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    34969 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/unlock.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5816 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/vertically.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8412 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/virtualbox.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1462 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/warning.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1906 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/wireshark.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5939 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/zoom-in-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6276 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/zoom-in.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5975 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/zoom-out-hover.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6157 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/icons/zoom-out.png
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.405358 gns3_gui-3.0.0b3/resources/images/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)   370070 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/images/gns3.ico
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7892 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/images/gns3_icon_128x128.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16745 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/images/gns3_icon_256x256.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     7921 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/images/gns3_logo.png
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16025 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/resources.qrc
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.405358 gns3_gui-3.0.0b3/resources/styles/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1231 2023-08-10 12:50:05.000000 gns3_gui-3.0.0b3/resources/styles/charcoal.css
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.405358 gns3_gui-3.0.0b3/resources/symbols/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16298 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/atm_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    78565 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/cloud.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/computer.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19782 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/docker_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18650 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/ethernet_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18401 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/firewall.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18343 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/frame_relay_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18128 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/hub.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    19150 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/multilayer_switch.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    30812 2024-05-16 10:32:52.000000 gns3_gui-3.0.0b3/resources/symbols/nat.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18421 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/qemu_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18494 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/router.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16401 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/vbox_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    16843 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/vmware_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    18297 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/resources/symbols/vpcs_guest.svg
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)       38 2024-05-19 10:32:57.505358 gns3_gui-3.0.0b3/setup.cfg
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.417358 gns3_gui-3.0.0b3/tests/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     6326 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/conftest.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.417358 gns3_gui-3.0.0b3/tests/items/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1997 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/items/test_ellipse_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1509 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/items/test_image_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2106 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/items/test_label_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4449 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/items/test_line_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3046 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/items/test_rectangle_item.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2039 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/items/test_text_item.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:56.957360 gns3_gui-3.0.0b3/tests/modules/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.417358 gns3_gui-3.0.0b3/tests/modules/docker/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1478 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/modules/docker/test_docker_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.417358 gns3_gui-3.0.0b3/tests/modules/dynamips/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1486 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/modules/dynamips/test_dynamips_init.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.417358 gns3_gui-3.0.0b3/tests/modules/iou/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1841 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/modules/iou/test_iou_device.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.417358 gns3_gui-3.0.0b3/tests/modules/qemu/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1526 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/modules/qemu/test_qemu_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.417358 gns3_gui-3.0.0b3/tests/modules/virtualbox/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1574 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/modules/virtualbox/test_virtualbox_vm.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.421358 gns3_gui-3.0.0b3/tests/modules/vpcs/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1637 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/modules/vpcs/test_vpcs_device.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.421358 gns3_gui-3.0.0b3/tests/qt/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1285 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/qt/test_qimage_svg_renderer.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.421358 gns3_gui-3.0.0b3/tests/registry/
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.425358 gns3_gui-3.0.0b3/tests/registry/appliances/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2607 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/arista-veos-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2451 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/arista-veos.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1353 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/broken-microcore-linux.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1576 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/cisco-3745-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1356 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/cisco-3745.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1171 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/cisco-iou-l3-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1019 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/cisco-iou-l3.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4047 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/empty-vm-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1612 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/juniper-vsrx.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2022 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/microcore-linux.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1216 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/openvswitch-v8.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1096 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/registry/appliances/openvswitch.gns3a
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     9480 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/registry/test_appliance.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13248 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/registry/test_appliance_to_template.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2895 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/registry/test_config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2304 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/registry/test_image.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2185 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/registry/test_registry.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1376 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/test_compute.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5810 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_compute_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1717 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_controller.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1354 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/test_graphics_view.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     8696 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_http_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3087 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_image_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1596 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_image_upload_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     4739 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_link.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)    13656 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_local_config.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2980 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_local_server.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1760 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_main_window.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1184 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/test_network_client.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5698 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/test_node.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1496 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/test_progress.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     5498 2024-05-19 08:59:01.000000 gns3_gui-3.0.0b3/tests/test_project.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2574 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/tests/test_spice_console.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3515 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/test_topology.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3575 2023-09-19 14:06:34.000000 gns3_gui-3.0.0b3/tests/test_update_manager.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1592 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/test_utils.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     2221 2023-11-06 07:06:12.000000 gns3_gui-3.0.0b3/tests/test_vnc_console.py
+drwxrwxr-x   0 grossmj   (1000) grossmj   (1000)        0 2024-05-19 10:32:57.493358 gns3_gui-3.0.0b3/tests/utils/
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     1394 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/utils/test_file_copy_worker.py
+-rw-rw-r--   0 grossmj   (1000) grossmj   (1000)     3705 2022-07-11 22:23:48.000000 gns3_gui-3.0.0b3/tests/utils/test_server_select.py
```

### Comparing `gns3-gui-3.0.0b2/CHANGELOG` & `gns3_gui-3.0.0b3/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Change Log
 
+## 3.0.0b3 19/05/2024
+
+* Fix updating IOS router
+* Ensure Python >= 3.8 is used in pyproject.toml
+
+## 2.2.47 15/05/2024
+
+* Remove maximum size for capture dialog. Ref #3576
+* Change sentry-sdk version
+* Upgrade aiohttp, sentry-sdk and truststore
+* Upgrade jsonschema and aiohttp
+* Drop Python 3.7
+* Remove dev requirements for Python 3.6
+* Add NAT symbols
+* Only show log message if event has "message"
+
 ## 3.0.0b2 07/04/2024
 
 * Enable local controller support on Linux
 * Support for custom Qemu path in templates and nodes
 * Round CPUs value in Docker templates and VMs. Ref https://github.com/GNS3/gns3-gui/issues/3572
 
 ## 2.2.46 26/02/2024
```

### Comparing `gns3-gui-3.0.0b2/LICENSE` & `gns3_gui-3.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/PKG-INFO` & `gns3_gui-3.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gns3-gui
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: GNS3 graphical interface for the GNS3 server.
 Author-email: Jeremy Grossmann <developers@gns3.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,29 +686,28 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jsonschema<4.18,>=4.17.3
-Requires-Dist: sentry-sdk<1.41,==1.40.6
+Requires-Dist: jsonschema<4.23,>=4.22.0
+Requires-Dist: sentry-sdk<2.2,==2.1.1
 Requires-Dist: psutil==5.9.8
 Requires-Dist: distro>=1.9.0
-Requires-Dist: truststore>=0.8.0; python_version >= "3.10"
+Requires-Dist: truststore>=0.9.1; python_version >= "3.10"
 Requires-Dist: importlib-resources>=1.3; python_version <= "3.9"
 Provides-Extra: dev
 Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: flake8==5.0.4; extra == "dev"
 Requires-Dist: pytest-timeout==2.3.1; extra == "dev"
 
 GNS3-gui
```

### Comparing `gns3-gui-3.0.0b2/README.md` & `gns3_gui-3.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/__main__.py` & `gns3_gui-3.0.0b3/gns3/__main__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/appliance_manager.py` & `gns3_gui-3.0.0b3/gns3/appliance_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/application.py` & `gns3_gui-3.0.0b3/gns3/application.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/base_node.py` & `gns3_gui-3.0.0b3/gns3/base_node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/compute.py` & `gns3_gui-3.0.0b3/gns3/compute.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/compute_manager.py` & `gns3_gui-3.0.0b3/gns3/compute_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/compute_summary_view.py` & `gns3_gui-3.0.0b3/gns3/compute_summary_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/console_cmd.py` & `gns3_gui-3.0.0b3/gns3/console_cmd.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/console_view.py` & `gns3_gui-3.0.0b3/gns3/console_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/controller.py` & `gns3_gui-3.0.0b3/gns3/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,15 +509,15 @@
             if project and project.id() == result["event"]["project_id"]:
                 Topology.instance().setProject(None)
         elif result["action"] == "project.updated":
             from .topology import Topology
             project = Topology.instance().project()
             if project and project.id() == result["event"]["project_id"]:
                 project.projectUpdatedCallback(result["event"])
-        elif result["action"] == "log.error":
-            log.error(result["event"]["message"])
-        elif result["action"] == "log.warning":
-            log.warning(result["event"]["message"])
-        elif result["action"] == "log.info":
-            log.info(result["event"]["message"], extra={"show": True})
+        elif result["action"] == "log.error" and result["event"].get("message"):
+            log.error(result["event"].get("message"))
+        elif result["action"] == "log.warning" and result["event"].get("message"):
+            log.warning(result["event"].get("message"))
+        elif result["action"] == "log.info" and result["event"].get("message"):
+            log.info(result["event"].get("message"), extra={"show": True})
         elif result["action"] == "ping":
             pass
```

### Comparing `gns3-gui-3.0.0b2/gns3/crash_report.py` & `gns3_gui-3.0.0b3/gns3/crash_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 class CrashReport:
 
     """
     Report crash to a third party service
     """
 
-    DSN = "https://5450a634dcf74dacf3f24800e31c4cf8@o19455.ingest.us.sentry.io/38506"
+    DSN = "https://4c7f622318895db756d831ed45f65940@o19455.ingest.us.sentry.io/38506"
     _instance = None
 
     def __init__(self):
         # We don't want sentry making noise if an error is caught when we don't have internet
         sentry_errors = logging.getLogger('sentry.errors')
         sentry_errors.disabled = True
```

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/about_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/about_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/appliance_wizard.py` & `gns3_gui-3.0.0b3/gns3/dialogs/appliance_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/capture_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/capture_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/configuration_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/configuration_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/console_command_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/console_command_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/custom_adapters_configuration_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/custom_adapters_configuration_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/doctor_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/doctor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/edit_compute_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/edit_compute_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/edit_project_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/edit_project_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/exec_command_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/exec_command_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/export_debug_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/export_debug_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/file_editor_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/file_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/filter_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/filter_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/idlepc_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/idlepc_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/image_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/image_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/login_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/login_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/new_template_wizard.py` & `gns3_gui-3.0.0b3/gns3/dialogs/new_template_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/node_info_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/node_info_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/node_properties_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/node_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/notif_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/notif_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/preferences_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/preferences_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/profile_select.py` & `gns3_gui-3.0.0b3/gns3/dialogs/profile_select.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/project_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/project_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/project_export_wizard.py` & `gns3_gui-3.0.0b3/gns3/dialogs/project_export_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/project_welcome_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/project_welcome_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/setup_wizard.py` & `gns3_gui-3.0.0b3/gns3/dialogs/setup_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/show_readme_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/show_readme_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/snapshots_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/snapshots_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/style_editor_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/style_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/style_editor_dialog_link.py` & `gns3_gui-3.0.0b3/gns3/dialogs/style_editor_dialog_link.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/symbol_selection_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/symbol_selection_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/text_editor_dialog.py` & `gns3_gui-3.0.0b3/gns3/dialogs/text_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/vm_with_images_wizard.py` & `gns3_gui-3.0.0b3/gns3/dialogs/vm_with_images_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/dialogs/vm_wizard.py` & `gns3_gui-3.0.0b3/gns3/dialogs/vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/graphics_view.py` & `gns3_gui-3.0.0b3/gns3/graphics_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/http_client.py` & `gns3_gui-3.0.0b3/gns3/http_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/http_client_error.py` & `gns3_gui-3.0.0b3/gns3/http_client_error.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/image_manager.py` & `gns3_gui-3.0.0b3/gns3/image_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/image_upload_manager.py` & `gns3_gui-3.0.0b3/gns3/image_upload_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/drawing_item.py` & `gns3_gui-3.0.0b3/gns3/items/drawing_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/ellipse_item.py` & `gns3_gui-3.0.0b3/gns3/items/ellipse_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/ethernet_link_item.py` & `gns3_gui-3.0.0b3/gns3/items/ethernet_link_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/image_item.py` & `gns3_gui-3.0.0b3/gns3/items/image_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/label_item.py` & `gns3_gui-3.0.0b3/gns3/items/label_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/line_item.py` & `gns3_gui-3.0.0b3/gns3/items/line_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/link_item.py` & `gns3_gui-3.0.0b3/gns3/items/link_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/logo_item.py` & `gns3_gui-3.0.0b3/gns3/items/logo_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/node_item.py` & `gns3_gui-3.0.0b3/gns3/items/node_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/rectangle_item.py` & `gns3_gui-3.0.0b3/gns3/items/rectangle_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/serial_link_item.py` & `gns3_gui-3.0.0b3/gns3/items/serial_link_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/shape_item.py` & `gns3_gui-3.0.0b3/gns3/items/shape_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/text_item.py` & `gns3_gui-3.0.0b3/gns3/items/text_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/items/utils.py` & `gns3_gui-3.0.0b3/gns3/items/utils.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/link.py` & `gns3_gui-3.0.0b3/gns3/link.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/gns3-gui.xml` & `gns3_gui-3.0.0b3/gns3/linux/gns3-gui.xml`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/16x16/apps/gns3.png` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/16x16/apps/gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/32x32/apps/gns3.png` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/32x32/apps/gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/apps/gns3.png` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/apps/gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3appliance.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/48x48/mimetypes/application-x-gns3project.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/apps/gns3.svg` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/apps/gns3.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3appliance.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg` & `gns3_gui-3.0.0b3/gns3/linux/icons/hicolor/scalable/mimetypes/application-x-gns3project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/local_config.py` & `gns3_gui-3.0.0b3/gns3/local_config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/local_server.py` & `gns3_gui-3.0.0b3/gns3/local_server.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/logger.py` & `gns3_gui-3.0.0b3/gns3/logger.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/main.py` & `gns3_gui-3.0.0b3/gns3/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,17 +185,17 @@
             print("YOUR SYSTEM IS OUT OF MEMORY!")
         else:
             CrashReport.instance().captureException(exception, value, tb)
 
     # catch exceptions to write them in a file
     sys.excepthook = exceptionHook
 
-    # we only support Python 3 version >= 3.7
-    if sys.version_info < (3, 7):
-        raise SystemExit("Python 3.7 or higher is required")
+    # we only support Python 3 version >= 3.8
+    if sys.version_info < (3, 8):
+        raise SystemExit("Python 3.8 or higher is required")
 
     if parse_version(QtCore.QT_VERSION_STR) < parse_version("5.5.0"):
         raise SystemExit("Requirement is PyQt5 version 5.5.0 or higher, got version {}".format(QtCore.QT_VERSION_STR))
 
     if parse_version(psutil.__version__) < parse_version("2.2.1"):
         raise SystemExit("Requirement is psutil version 2.2.1 or higher, got version {}".format(psutil.__version__))
```

### Comparing `gns3-gui-3.0.0b2/gns3/main_window.py` & `gns3_gui-3.0.0b3/gns3/main_window.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/__init__.py` & `gns3_gui-3.0.0b3/gns3/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/__init__.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/atm_switch.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/atm_switch.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/cloud.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/cloud.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/cloud_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/dialogs/cloud_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/dialogs/ethernet_hub_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/dialogs/ethernet_switch_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ethernet_hub.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ethernet_hub.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ethernet_switch.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ethernet_switch.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/frame_relay_switch.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/frame_relay_switch.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/nat.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/nat.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def defaultSymbol():
         """
         Returns the default symbol path for this nat.
 
         :returns: symbol path (or resource).
         """
 
-        return ":/symbols/cloud.svg"
+        return ":/symbols/nat.svg"
 
     @staticmethod
     def categories():
         """
         Returns the node categories the node is part of (used by the device panel).
 
         :returns: list of node categories
```

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/atm_switch_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/pages/atm_switch_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/builtin_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/pages/builtin_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/cloud_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/pages/cloud_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/cloud_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/pages/cloud_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/pages/ethernet_hub_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/pages/ethernet_hub_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/pages/ethernet_switch_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/pages/ethernet_switch_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/pages/frame_relay_switch_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/settings.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/atm_switch_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/atm_switch_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/atm_switch_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/builtin_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/builtin_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/builtin_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/builtin_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/cloud_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/cloud_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_hub_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/ethernet_switch_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/frame_relay_switch_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/ui/frame_relay_switch_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/builtin/utils/tree_widget_item.py` & `gns3_gui-3.0.0b3/gns3/modules/builtin/utils/tree_widget_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/__init__.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/dialogs/docker_vm_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/dialogs/docker_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/docker_vm.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/docker_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/pages/docker_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_vm_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/pages/docker_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/pages/docker_vm_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/pages/docker_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/settings.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/docker/ui/docker_vm_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/docker/ui/docker_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/__init__.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/adapters.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/adapters.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/dialogs/ios_router_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/dialogs/ios_router_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c1700.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c1700.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c2600.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c2600.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c2691.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c2691.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3600.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c3600.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3725.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c3725.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c3745.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c3745.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/c7200.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/c7200.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/etherswitch_router.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/etherswitch_router.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/nodes/router.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/nodes/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     def __init__(self, module, server, project, platform="c7200"):
 
         super().__init__(module, server, project)
         self._dynamips_id = None
 
         router_settings = {"platform": platform,
                            "usage": "",
-                           "chassis": "",
                            "image": "",
                            "image_md5sum": "",
                            "startup_config": "",
                            "private_config": "",
                            "ram": 128,
                            "nvram": 128,
                            "mmap": True,
```

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/dynamips_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/pages/dynamips_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/ios_router_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/pages/ios_router_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/pages/ios_router_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/pages/ios_router_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/settings.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/dynamips_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/dynamips_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/dynamips_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/ui/ios_router_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/ui/ios_router_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/decompress_ios.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/utils/decompress_ios.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/utils/decompress_ios_worker.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/utils/decompress_ios_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/dynamips/wics.py` & `gns3_gui-3.0.0b3/gns3/modules/dynamips/wics.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/__init__.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/dialogs/iou_device_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/dialogs/iou_device_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/iou_device.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/iou_device.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_device_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/pages/iou_device_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_device_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/pages/iou_device_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/pages/iou_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/pages/iou_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/settings.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_device_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_device_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/iou/ui/iou_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/iou/ui/iou_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/module.py` & `gns3_gui-3.0.0b3/gns3/modules/module.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/module_error.py` & `gns3_gui-3.0.0b3/gns3/modules/module_error.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/__init__.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/qemu_image_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/dialogs/qemu_image_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/dialogs/qemu_vm_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/dialogs/qemu_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/pages/qemu_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_vm_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/pages/qemu_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/pages/qemu_vm_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/pages/qemu_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/qemu_vm.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/qemu_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/settings.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_image_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_image_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_image_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_image_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/qemu/ui/qemu_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/__init__.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/dialogs/virtualbox_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/pages/virtualbox_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/pages/virtualbox_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/pages/virtualbox_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/settings.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/ui/virtualbox_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/virtualbox/virtualbox_vm.py` & `gns3_gui-3.0.0b3/gns3/modules/virtualbox/virtualbox_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/__init__.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/dialogs/vmware_vm_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/dialogs/vmware_vm_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/pages/vmware_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_vm_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/pages/vmware_vm_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/pages/vmware_vm_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/pages/vmware_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/settings.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/ui/vmware_vm_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vmware/vmware_vm.py` & `gns3_gui-3.0.0b3/gns3/modules/vmware/vmware_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/__init__.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/dialogs/vpcs_node_wizard.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/pages/vpcs_node_configuration_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/pages/vpcs_node_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/pages/vpcs_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/pages/vpcs_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/settings.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_wizard.ui` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_node_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/ui/vpcs_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/modules/vpcs/vpcs_node.py` & `gns3_gui-3.0.0b3/gns3/modules/vpcs/vpcs_node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/network_client.py` & `gns3_gui-3.0.0b3/gns3/network_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/node.py` & `gns3_gui-3.0.0b3/gns3/node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/nodes_dock_widget.py` & `gns3_gui-3.0.0b3/gns3/nodes_dock_widget.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/nodes_view.py` & `gns3_gui-3.0.0b3/gns3/nodes_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/packet_capture.py` & `gns3_gui-3.0.0b3/gns3/packet_capture.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/pages/controller_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/pages/controller_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/pages/general_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/pages/general_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/pages/gns3_vm_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/pages/gns3_vm_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/pages/packet_capture_preferences_page.py` & `gns3_gui-3.0.0b3/gns3/pages/packet_capture_preferences_page.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ports/ethernet_port.py` & `gns3_gui-3.0.0b3/gns3/ports/ethernet_port.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ports/port.py` & `gns3_gui-3.0.0b3/gns3/ports/port.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ports/port_name_factory.py` & `gns3_gui-3.0.0b3/gns3/ports/port_name_factory.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ports/serial_port.py` & `gns3_gui-3.0.0b3/gns3/ports/serial_port.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/progress.py` & `gns3_gui-3.0.0b3/gns3/progress.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/project.py` & `gns3_gui-3.0.0b3/gns3/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -732,15 +732,15 @@
         # when connected to an older controller version
         elif result["action"] == "project.closed":
             Topology.instance().setProject(None)
         elif result["action"] == "project.updated":
             self.projectUpdatedCallback(result["event"])
         elif result["action"] == "snapshot.restored":
             Topology.instance().restoreSnapshot(result["event"]["project_id"])
-        elif result["action"] == "log.error":
-            log.error(result["event"]["message"])
-        elif result["action"] == "log.warning":
-            log.warning(result["event"]["message"])
-        elif result["action"] == "log.info":
-            log.info(result["event"]["message"], extra={"show": True})
+        elif result["action"] == "log.error" and result["event"].get("message"):
+            log.error(result["event"].get("message"))
+        elif result["action"] == "log.warning" and result["event"].get("message"):
+            log.warning(result["event"].get("message"))
+        elif result["action"] == "log.info" and result["event"].get("message"):
+            log.info(result["event"].get("message"), extra={"show": True})
         elif result["action"] == "ping":
             pass
```

### Comparing `gns3-gui-3.0.0b2/gns3/pycutext.py` & `gns3_gui-3.0.0b3/gns3/pycutext.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/qt/__init__.py` & `gns3_gui-3.0.0b3/gns3/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/qt/qimage_svg_renderer.py` & `gns3_gui-3.0.0b3/gns3/qt/qimage_svg_renderer.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/registry/appliance.py` & `gns3_gui-3.0.0b3/gns3/registry/appliance.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/registry/appliance_to_template.py` & `gns3_gui-3.0.0b3/gns3/registry/appliance_to_template.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/registry/config.py` & `gns3_gui-3.0.0b3/gns3/registry/config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/registry/image.py` & `gns3_gui-3.0.0b3/gns3/registry/image.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/registry/registry.py` & `gns3_gui-3.0.0b3/gns3/registry/registry.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/schemas/appliance.json` & `gns3_gui-3.0.0b3/gns3/schemas/appliance.json`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/schemas/appliance_v8.json` & `gns3_gui-3.0.0b3/gns3/schemas/appliance_v8.json`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/settings.py` & `gns3_gui-3.0.0b3/gns3/settings.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/spice_console.py` & `gns3_gui-3.0.0b3/gns3/spice_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/status_bar.py` & `gns3_gui-3.0.0b3/gns3/status_bar.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/style.py` & `gns3_gui-3.0.0b3/gns3/style.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/symbol.py` & `gns3_gui-3.0.0b3/gns3/symbol.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/telnet_console.py` & `gns3_gui-3.0.0b3/gns3/telnet_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/template.py` & `gns3_gui-3.0.0b3/gns3/template.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/template_manager.py` & `gns3_gui-3.0.0b3/gns3/template_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/topology.py` & `gns3_gui-3.0.0b3/gns3/topology.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/topology_summary_view.py` & `gns3_gui-3.0.0b3/gns3/topology_summary_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/about_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/about_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/about_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/appliance_wizard.ui` & `gns3_gui-3.0.0b3/gns3/ui/appliance_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/appliance_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/appliance_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/capture_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/capture_dialog.ui`

 * *Files 8% similar despite different names*

#### Comparing `gns3-gui-3.0.0b2/gns3/ui/capture_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/capture_dialog.ui`

```diff
@@ -5,24 +5,18 @@
     <property name="windowModality">
       <enum>Qt::WindowModal</enum>
     </property>
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>500</width>
-        <height>147</height>
+        <width>460</width>
+        <height>142</height>
       </rect>
     </property>
-    <property name="maximumSize">
-      <size>
-        <width>500</width>
-        <height>147</height>
-      </size>
-    </property>
     <property name="windowTitle">
       <string>Packet capture</string>
     </property>
     <property name="modal">
       <bool>false</bool>
     </property>
     <layout class="QGridLayout" name="gridLayout">
```

### Comparing `gns3-gui-3.0.0b2/gns3/ui/capture_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/capture_dialog_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file '/home/grossmj/PycharmProjects/gns3-gui/gns3/ui/capture_dialog.ui'
 #
-# Created: Mon May 30 21:49:29 2016
-#      by: PyQt5 UI code generator 5.2.1
+# Created by: PyQt5 UI code generator 5.15.6
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic5 is
+# run again.  Do not edit this file unless you know what you are doing.
+
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
+
 class Ui_CaptureDialog(object):
     def setupUi(self, CaptureDialog):
         CaptureDialog.setObjectName("CaptureDialog")
         CaptureDialog.setWindowModality(QtCore.Qt.WindowModal)
-        CaptureDialog.resize(500, 147)
-        CaptureDialog.setMaximumSize(QtCore.QSize(500, 147))
+        CaptureDialog.resize(460, 142)
         CaptureDialog.setModal(False)
         self.gridLayout = QtWidgets.QGridLayout(CaptureDialog)
         self.gridLayout.setObjectName("gridLayout")
         self.uiLinkTypeLabel = QtWidgets.QLabel(CaptureDialog)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
@@ -69,9 +70,8 @@
 
     def retranslateUi(self, CaptureDialog):
         _translate = QtCore.QCoreApplication.translate
         CaptureDialog.setWindowTitle(_translate("CaptureDialog", "Packet capture"))
         self.uiLinkTypeLabel.setText(_translate("CaptureDialog", "Link type:"))
         self.uiFileNameLabel.setText(_translate("CaptureDialog", "File name:"))
         self.uiStartCommandCheckBox.setText(_translate("CaptureDialog", "Start the capture visualization program"))
-
 from . import resources_rc
```

### Comparing `gns3-gui-3.0.0b2/gns3/ui/configuration_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/configuration_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/configuration_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/console_command_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/console_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/console_command_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/console_command_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/controller_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/ui/controller_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/controller_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/controller_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/custom_adapters_configuration_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/custom_adapters_configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/custom_adapters_configuration_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/custom_adapters_configuration_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/doctor_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/doctor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/doctor_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/doctor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/edit_compute_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/edit_compute_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/edit_compute_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/edit_compute_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/edit_project_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/edit_project_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/edit_project_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/edit_project_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/exec_command_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/exec_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/exec_command_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/exec_command_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/export_debug_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/export_debug_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/export_debug_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/export_debug_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/export_project_wizard.ui` & `gns3_gui-3.0.0b3/gns3/ui/export_project_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/export_project_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/export_project_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/file_editor_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/file_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/file_editor_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/file_editor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/filter_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/filter_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/filter_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/filter_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/general_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/ui/general_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/general_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/general_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/gns3_vm_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/ui/gns3_vm_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/gns3_vm_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/gns3_vm_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/idlepc_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/idlepc_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/idlepc_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/idlepc_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/image_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/image_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/image_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/image_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/login_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/login_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/login_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/login_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/main_window.ui` & `gns3_gui-3.0.0b3/gns3/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/main_window_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/new_template_wizard.ui` & `gns3_gui-3.0.0b3/gns3/ui/new_template_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/new_template_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/new_template_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/node_info_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/node_info_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/node_info_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/node_info_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/node_properties_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/node_properties_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/node_properties_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/node_properties_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/packet_capture_preferences_page.ui` & `gns3_gui-3.0.0b3/gns3/ui/packet_capture_preferences_page.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/packet_capture_preferences_page_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/packet_capture_preferences_page_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/preferences_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/preferences_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/preferences_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/preferences_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/profile_select_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/profile_select_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/profile_select_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/profile_select_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/project_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/project_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/project_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/project_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/project_welcome_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/project_welcome_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/project_welcome_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/project_welcome_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/resources_rc.py` & `gns3_gui-3.0.0b3/gns3/ui/resources_rc.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/setup_wizard.ui` & `gns3_gui-3.0.0b3/gns3/ui/setup_wizard.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/setup_wizard_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/setup_wizard_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/show_readme_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/show_readme_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/show_readme_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/show_readme_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/snapshots_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/snapshots_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/snapshots_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/snapshots_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/style_editor_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/style_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/style_editor_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/style_editor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/symbol_selection_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/symbol_selection_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/symbol_selection_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/symbol_selection_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/text_editor_dialog.ui` & `gns3_gui-3.0.0b3/gns3/ui/text_editor_dialog.ui`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/ui/text_editor_dialog_ui.py` & `gns3_gui-3.0.0b3/gns3/ui/text_editor_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/update_manager.py` & `gns3_gui-3.0.0b3/gns3/update_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/__init__.py` & `gns3_gui-3.0.0b3/gns3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/authorize_ubridge.py` & `gns3_gui-3.0.0b3/gns3/utils/authorize_ubridge.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/bring_to_front.py` & `gns3_gui-3.0.0b3/gns3/utils/bring_to_front.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/file_copy_worker.py` & `gns3_gui-3.0.0b3/gns3/utils/file_copy_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/get_icon.py` & `gns3_gui-3.0.0b3/gns3/utils/get_icon.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/get_resource.py` & `gns3_gui-3.0.0b3/gns3/utils/get_resource.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/import_project_worker.py` & `gns3_gui-3.0.0b3/gns3/utils/import_project_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/install_mime_types.py` & `gns3_gui-3.0.0b3/gns3/utils/install_mime_types.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/interfaces.py` & `gns3_gui-3.0.0b3/gns3/utils/interfaces.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/macos_ubridge_setuid.py` & `gns3_gui-3.0.0b3/gns3/utils/macos_ubridge_setuid.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/normalize_filename.py` & `gns3_gui-3.0.0b3/gns3/utils/normalize_filename.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/process_files_worker.py` & `gns3_gui-3.0.0b3/gns3/utils/process_files_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/progress_dialog.py` & `gns3_gui-3.0.0b3/gns3/utils/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/run_in_terminal.py` & `gns3_gui-3.0.0b3/gns3/utils/run_in_terminal.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/server_select.py` & `gns3_gui-3.0.0b3/gns3/utils/server_select.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/sudo.py` & `gns3_gui-3.0.0b3/gns3/utils/sudo.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/wait_for_command_worker.py` & `gns3_gui-3.0.0b3/gns3/utils/wait_for_command_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/wait_for_connection_worker.py` & `gns3_gui-3.0.0b3/gns3/utils/wait_for_connection_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/wait_for_lambda_worker.py` & `gns3_gui-3.0.0b3/gns3/utils/wait_for_lambda_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/utils/wait_for_runas_worker.py` & `gns3_gui-3.0.0b3/gns3/utils/wait_for_runas_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3/version.py` & `gns3_gui-3.0.0b3/gns3/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # __version_info__ is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
 
-__version__ = "3.0.0b2"
+__version__ = "3.0.0b3"
 __version_info__ = (3, 0, 0, -99)
 
 if "dev" in __version__:
     try:
         import os
         import subprocess
         if os.path.exists(os.path.join(os.path.dirname(os.path.abspath(__file__)), "..", ".git")):
```

### Comparing `gns3-gui-3.0.0b2/gns3/vnc_console.py` & `gns3_gui-3.0.0b3/gns3/vnc_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/gns3_gui.egg-info/PKG-INFO` & `gns3_gui-3.0.0b3/gns3_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gns3-gui
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: GNS3 graphical interface for the GNS3 server.
 Author-email: Jeremy Grossmann <developers@gns3.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,29 +686,28 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jsonschema<4.18,>=4.17.3
-Requires-Dist: sentry-sdk<1.41,==1.40.6
+Requires-Dist: jsonschema<4.23,>=4.22.0
+Requires-Dist: sentry-sdk<2.2,==2.1.1
 Requires-Dist: psutil==5.9.8
 Requires-Dist: distro>=1.9.0
-Requires-Dist: truststore>=0.8.0; python_version >= "3.10"
+Requires-Dist: truststore>=0.9.1; python_version >= "3.10"
 Requires-Dist: importlib-resources>=1.3; python_version <= "3.9"
 Provides-Extra: dev
 Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: flake8==5.0.4; extra == "dev"
 Requires-Dist: pytest-timeout==2.3.1; extra == "dev"
 
 GNS3-gui
```

### Comparing `gns3-gui-3.0.0b2/gns3_gui.egg-info/SOURCES.txt` & `gns3_gui-3.0.0b3/gns3_gui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -738,14 +738,15 @@
 resources/symbols/computer.svg
 resources/symbols/docker_guest.svg
 resources/symbols/ethernet_switch.svg
 resources/symbols/firewall.svg
 resources/symbols/frame_relay_switch.svg
 resources/symbols/hub.svg
 resources/symbols/multilayer_switch.svg
+resources/symbols/nat.svg
 resources/symbols/qemu_guest.svg
 resources/symbols/router.svg
 resources/symbols/vbox_guest.svg
 resources/symbols/vmware_guest.svg
 resources/symbols/vpcs_guest.svg
 tests/conftest.py
 tests/test_compute.py
```

### Comparing `gns3-gui-3.0.0b2/pyproject.toml` & `gns3_gui-3.0.0b3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 name = "gns3-gui"
 description = "GNS3 graphical interface for the GNS3 server."
 license = {file = "LICENSE"}
 authors = [
   { name = "Jeremy Grossmann", email = "developers@gns3.com" }
 ]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Environment :: X11 Applications :: Qt",
         "Intended Audience :: Information Technology",
         "Topic :: System :: Networking",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Operating System :: POSIX",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
 ]
```

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1-cancel.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/add-link-1-cancel.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/add-link-1-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/add-link-1.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/add-link-1.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/add-note-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/add-note-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/add-note.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/add-note.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/aux-console-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/aux-console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/aux-console.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/aux-console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/browse-all-icons-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/browse-all-icons-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/browse-all-icons.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/browse-all-icons.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/calculate-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/calculate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/calculate.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/camera-photo-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/camera-photo-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/camera-photo.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/capture-start-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/capture-start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/capture-start.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/capture-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/capture-stop-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/capture-stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/capture-stop.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/capture-stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/command_line-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/command_line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/command_line.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/command_line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/configuration-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/configuration-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/configuration.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/configuration.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/console-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/console.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/console_edit-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/console_edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/console_edit.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/console_edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/delete-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/delete-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/delete.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/delete.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/duplicate-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/duplicate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/duplicate.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/edit-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/edit.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/ellipse-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/ellipse-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/ellipse.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/export-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/export-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/export.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/export.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/filter-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/filter-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/filter-reset-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/filter-reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/filter-reset.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/filter-reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/filter.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/filter.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/firewall-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/firewall-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/firewall.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/firewall.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/front-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/front-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/front.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/front.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/help-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/help-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/help.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/help.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/image-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/image-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/image.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/image.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/import-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/import-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/import.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/import.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/import_export_configs-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/import_export_configs-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/import_export_configs.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/import_export_configs.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/inspect-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/inspect-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/inspect.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/inspect.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/line-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/line.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/lock-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/lock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/lock.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/lock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/lower_z_value-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/lower_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/lower_z_value.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/lower_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/minus-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/minus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/minus.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/minus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/new-project-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/new-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/new-project.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/new-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/node_conception-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/node_conception-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/node_conception.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/node_conception.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/open-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/open-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/open.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/open.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/pause-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/pause-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/pause.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/pc-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/pc-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/pc.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/pc.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/plus-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/plus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/plus.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/plus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/preferences-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/preferences-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/preferences.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/preferences.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/quit-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/quit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/quit.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/quit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/raise_z_value-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/raise_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/raise_z_value.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/raise_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/rectangle-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/rectangle-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/rectangle.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/reload-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/reload-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/reload.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/reload.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/reset-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/reset.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/router-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/router-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/router.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/router.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/save-as-project-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/save-as-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/save-as-project.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/save-as-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/save-project-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/save-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/save-project.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/save-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/show-hostname-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/show-hostname-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/show-hostname.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/show-hostname.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/show-interface-names-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/show-interface-names-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/show-interface-names.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/show-interface-names.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/snapshot-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/snapshot-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/snapshot.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/snapshot.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/start-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/start.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/stop-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/stop.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/switch-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/switch-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/switch.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/unlock-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/unlock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/unlock.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-in-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/zoom-in-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-in.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-out-hover.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/zoom-out-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/charcoal_icons/zoom-out.svg` & `gns3_gui-3.0.0b3/resources/charcoal_icons/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/add-link-cancel.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/add-link-cancel.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/add-link-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/add-link-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/add-link.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/add-link.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/add-note-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/add-note-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/add-note.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/add-note.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/aux-console-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/aux-console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/aux-console.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/aux-console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/browse-all-icons-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/browse-all-icons-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/browse-all-icons.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/browse-all-icons.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/calculate-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/calculate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/calculate.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/camera-photo-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/camera-photo-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/camera-photo.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/capture-start-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/capture-start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/capture-start.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/capture-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/capture-stop-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/capture-stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/capture-stop.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/capture-stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/command_line-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/command_line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/command_line.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/command_line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/configuration-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/configuration-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/configuration.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/configuration.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/console-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/console-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/console.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/console_edit-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/console_edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/console_edit.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/console_edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/delete-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/delete-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/delete.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/delete.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/duplicate-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/duplicate-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/duplicate.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/edit-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/edit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/edit.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/ellipse-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/ellipse-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/ellipse.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/export-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/export-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/export.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/export.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/filter-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/filter-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/filter-reset-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/filter-reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/filter-reset.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/filter-reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/filter.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/filter.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/firewall-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/firewall-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/firewall.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/firewall.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/front-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/front-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/front.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/front.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/help-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/help-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/help.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/help.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/image-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/image-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/image.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/image.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/import-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/import-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/import.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/import.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/import_export_configs-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/import_export_configs-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/import_export_configs.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/import_export_configs.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/inspect-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/inspect-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/inspect.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/inspect.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/line-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/line-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/line.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/lock-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/lock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/lock.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/lock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/lower_z_value-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/lower_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/lower_z_value.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/lower_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/minus-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/minus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/minus.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/minus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/new-project-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/new-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/new-project.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/new-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/node_conception-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/node_conception-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/node_conception.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/node_conception.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/open-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/open-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/open.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/open.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/pause-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/pause-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/pause.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/pc-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/pc-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/pc.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/pc.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/plus-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/plus-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/plus.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/plus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/preferences-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/preferences-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/preferences.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/preferences.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/quit-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/quit-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/quit.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/quit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/raise_z_value-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/raise_z_value-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/raise_z_value.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/raise_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/rectangle-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/rectangle-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/rectangle.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/reload-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/reload-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/reload.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/reload.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/reset-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/reset-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/reset.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/router-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/router-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/router.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/router.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/save-as-project-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/save-as-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/save-as-project.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/save-as-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/save-project-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/save-project-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/save-project.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/save-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/show-hostname-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/show-hostname-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/show-hostname.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/show-hostname.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/show-interface-names-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/show-interface-names-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/show-interface-names.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/show-interface-names.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/snapshot-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/snapshot-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/snapshot.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/snapshot.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/start-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/start.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/stop-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/stop.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/switch-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/switch-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/switch.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/unlock-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/unlock-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/unlock.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/zoom-in-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/zoom-in-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/zoom-in.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/zoom-out-hover.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/zoom-out-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/classic_icons/zoom-out.svg` & `gns3_gui-3.0.0b3/resources/classic_icons/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/PC-hover.png` & `gns3_gui-3.0.0b3/resources/icons/PC-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/PC.png` & `gns3_gui-3.0.0b3/resources/icons/PC.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/add-note.svg` & `gns3_gui-3.0.0b3/resources/icons/add-note.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/applications.svg` & `gns3_gui-3.0.0b3/resources/icons/applications.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/aux-console.svg` & `gns3_gui-3.0.0b3/resources/icons/aux-console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/browse-all-icons-hover.png` & `gns3_gui-3.0.0b3/resources/icons/browse-all-icons-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/browse-all-icons.png` & `gns3_gui-3.0.0b3/resources/icons/browse-all-icons.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/calculate.svg` & `gns3_gui-3.0.0b3/resources/icons/calculate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/camera-photo-hover.svg` & `gns3_gui-3.0.0b3/resources/icons/camera-photo-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/camera-photo.svg` & `gns3_gui-3.0.0b3/resources/icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/cancel-connection.svg` & `gns3_gui-3.0.0b3/resources/icons/cancel-connection.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/cancel.svg` & `gns3_gui-3.0.0b3/resources/icons/cancel.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/capture-start.svg` & `gns3_gui-3.0.0b3/resources/icons/capture-start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/capture-stop.svg` & `gns3_gui-3.0.0b3/resources/icons/capture-stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/command_line.svg` & `gns3_gui-3.0.0b3/resources/icons/command_line.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/configuration.svg` & `gns3_gui-3.0.0b3/resources/icons/configuration.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/connection-new-hover.svg` & `gns3_gui-3.0.0b3/resources/icons/connection-new-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/connection-new.svg` & `gns3_gui-3.0.0b3/resources/icons/connection-new.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/console.svg` & `gns3_gui-3.0.0b3/resources/icons/console.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/console_edit.svg` & `gns3_gui-3.0.0b3/resources/icons/console_edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/delete.svg` & `gns3_gui-3.0.0b3/resources/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/dialog-warning.svg` & `gns3_gui-3.0.0b3/resources/icons/dialog-warning.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/drawing.svg` & `gns3_gui-3.0.0b3/resources/icons/drawing.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/duplicate.svg` & `gns3_gui-3.0.0b3/resources/icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/edit.svg` & `gns3_gui-3.0.0b3/resources/icons/edit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/ellipse-hover.svg` & `gns3_gui-3.0.0b3/resources/icons/ellipse-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/ellipse.svg` & `gns3_gui-3.0.0b3/resources/icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/export.svg` & `gns3_gui-3.0.0b3/resources/icons/export.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/filter-capture.svg` & `gns3_gui-3.0.0b3/resources/icons/filter-capture.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/filter-reset.svg` & `gns3_gui-3.0.0b3/resources/icons/filter-reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/filter.svg` & `gns3_gui-3.0.0b3/resources/icons/filter.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/firewall-hover.png` & `gns3_gui-3.0.0b3/resources/icons/firewall-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/firewall.png` & `gns3_gui-3.0.0b3/resources/icons/firewall.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/front.svg` & `gns3_gui-3.0.0b3/resources/icons/front.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/help.svg` & `gns3_gui-3.0.0b3/resources/icons/help.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/horizontally.svg` & `gns3_gui-3.0.0b3/resources/icons/horizontally.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/image.svg` & `gns3_gui-3.0.0b3/resources/icons/image.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/import.svg` & `gns3_gui-3.0.0b3/resources/icons/import.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/import_export_configs.svg` & `gns3_gui-3.0.0b3/resources/icons/import_export_configs.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/inspect.svg` & `gns3_gui-3.0.0b3/resources/icons/inspect.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/led_gray.svg` & `gns3_gui-3.0.0b3/resources/icons/led_gray.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/led_green.svg` & `gns3_gui-3.0.0b3/resources/icons/led_green.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/led_red.svg` & `gns3_gui-3.0.0b3/resources/icons/led_red.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/led_yellow.svg` & `gns3_gui-3.0.0b3/resources/icons/led_yellow.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/lock.svg` & `gns3_gui-3.0.0b3/resources/icons/lock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/lower_z_value.svg` & `gns3_gui-3.0.0b3/resources/icons/lower_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/minus.svg` & `gns3_gui-3.0.0b3/resources/icons/minus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/new-project.svg` & `gns3_gui-3.0.0b3/resources/icons/new-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/new.svg` & `gns3_gui-3.0.0b3/resources/icons/new.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/node_conception.svg` & `gns3_gui-3.0.0b3/resources/icons/node_conception.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/open.svg` & `gns3_gui-3.0.0b3/resources/icons/open.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/pause-hover.svg` & `gns3_gui-3.0.0b3/resources/icons/pause-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/pause.svg` & `gns3_gui-3.0.0b3/resources/icons/pause.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/plus.svg` & `gns3_gui-3.0.0b3/resources/icons/plus.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/quit.svg` & `gns3_gui-3.0.0b3/resources/icons/quit.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/raise_z_value.svg` & `gns3_gui-3.0.0b3/resources/icons/raise_z_value.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/rectangle-hover.svg` & `gns3_gui-3.0.0b3/resources/icons/rectangle-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/rectangle.svg` & `gns3_gui-3.0.0b3/resources/icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/reload.svg` & `gns3_gui-3.0.0b3/resources/icons/reload.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/reset.svg` & `gns3_gui-3.0.0b3/resources/icons/reset.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/router-hover.png` & `gns3_gui-3.0.0b3/resources/icons/router-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/router.png` & `gns3_gui-3.0.0b3/resources/icons/router.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/rtv.png` & `gns3_gui-3.0.0b3/resources/icons/rtv.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/save-as-project.svg` & `gns3_gui-3.0.0b3/resources/icons/save-as-project.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/save-as.svg` & `gns3_gui-3.0.0b3/resources/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/save.svg` & `gns3_gui-3.0.0b3/resources/icons/save.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/show-hostname.svg` & `gns3_gui-3.0.0b3/resources/icons/show-hostname.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/show-interface-names.svg` & `gns3_gui-3.0.0b3/resources/icons/show-interface-names.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/snapshot.svg` & `gns3_gui-3.0.0b3/resources/icons/snapshot.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/start-hover.svg` & `gns3_gui-3.0.0b3/resources/icons/start-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/start.svg` & `gns3_gui-3.0.0b3/resources/icons/start.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/stop-hover.svg` & `gns3_gui-3.0.0b3/resources/icons/stop-hover.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/stop.svg` & `gns3_gui-3.0.0b3/resources/icons/stop.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/switch-hover.png` & `gns3_gui-3.0.0b3/resources/icons/switch-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/switch.png` & `gns3_gui-3.0.0b3/resources/icons/switch.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/unlock.svg` & `gns3_gui-3.0.0b3/resources/icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/vertically.svg` & `gns3_gui-3.0.0b3/resources/icons/vertically.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/virtualbox.png` & `gns3_gui-3.0.0b3/resources/icons/virtualbox.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/warning.svg` & `gns3_gui-3.0.0b3/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/wireshark.png` & `gns3_gui-3.0.0b3/resources/icons/wireshark.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/zoom-in-hover.png` & `gns3_gui-3.0.0b3/resources/icons/zoom-in-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/zoom-in.png` & `gns3_gui-3.0.0b3/resources/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/zoom-out-hover.png` & `gns3_gui-3.0.0b3/resources/icons/zoom-out-hover.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/icons/zoom-out.png` & `gns3_gui-3.0.0b3/resources/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/images/gns3.ico` & `gns3_gui-3.0.0b3/resources/images/gns3.ico`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/images/gns3_icon_128x128.png` & `gns3_gui-3.0.0b3/resources/images/gns3_icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/images/gns3_icon_256x256.png` & `gns3_gui-3.0.0b3/resources/images/gns3_icon_256x256.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/images/gns3_logo.png` & `gns3_gui-3.0.0b3/resources/images/gns3_logo.png`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/resources.qrc` & `gns3_gui-3.0.0b3/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/styles/charcoal.css` & `gns3_gui-3.0.0b3/resources/styles/charcoal.css`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/atm_switch.svg` & `gns3_gui-3.0.0b3/resources/symbols/atm_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/cloud.svg` & `gns3_gui-3.0.0b3/resources/symbols/cloud.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/computer.svg` & `gns3_gui-3.0.0b3/resources/symbols/computer.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/docker_guest.svg` & `gns3_gui-3.0.0b3/resources/symbols/docker_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/ethernet_switch.svg` & `gns3_gui-3.0.0b3/resources/symbols/ethernet_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/firewall.svg` & `gns3_gui-3.0.0b3/resources/symbols/firewall.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/frame_relay_switch.svg` & `gns3_gui-3.0.0b3/resources/symbols/frame_relay_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/hub.svg` & `gns3_gui-3.0.0b3/resources/symbols/hub.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/multilayer_switch.svg` & `gns3_gui-3.0.0b3/resources/symbols/multilayer_switch.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/qemu_guest.svg` & `gns3_gui-3.0.0b3/resources/symbols/qemu_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/router.svg` & `gns3_gui-3.0.0b3/resources/symbols/router.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/vbox_guest.svg` & `gns3_gui-3.0.0b3/resources/symbols/vbox_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/vmware_guest.svg` & `gns3_gui-3.0.0b3/resources/symbols/vmware_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/resources/symbols/vpcs_guest.svg` & `gns3_gui-3.0.0b3/resources/symbols/vpcs_guest.svg`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/conftest.py` & `gns3_gui-3.0.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/items/test_ellipse_item.py` & `gns3_gui-3.0.0b3/tests/items/test_ellipse_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/items/test_image_item.py` & `gns3_gui-3.0.0b3/tests/items/test_image_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/items/test_label_item.py` & `gns3_gui-3.0.0b3/tests/items/test_label_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/items/test_line_item.py` & `gns3_gui-3.0.0b3/tests/items/test_line_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/items/test_rectangle_item.py` & `gns3_gui-3.0.0b3/tests/items/test_rectangle_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/items/test_text_item.py` & `gns3_gui-3.0.0b3/tests/items/test_text_item.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/modules/docker/test_docker_vm.py` & `gns3_gui-3.0.0b3/tests/modules/docker/test_docker_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/modules/dynamips/test_dynamips_init.py` & `gns3_gui-3.0.0b3/tests/modules/dynamips/test_dynamips_init.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/modules/iou/test_iou_device.py` & `gns3_gui-3.0.0b3/tests/modules/iou/test_iou_device.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/modules/qemu/test_qemu_vm.py` & `gns3_gui-3.0.0b3/tests/modules/qemu/test_qemu_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/modules/virtualbox/test_virtualbox_vm.py` & `gns3_gui-3.0.0b3/tests/modules/virtualbox/test_virtualbox_vm.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/modules/vpcs/test_vpcs_device.py` & `gns3_gui-3.0.0b3/tests/modules/vpcs/test_vpcs_device.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/qt/test_qimage_svg_renderer.py` & `gns3_gui-3.0.0b3/tests/qt/test_qimage_svg_renderer.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/arista-veos-v8.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/arista-veos-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/arista-veos.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/arista-veos.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/broken-microcore-linux.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/broken-microcore-linux.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/cisco-3745-v8.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/cisco-3745-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/cisco-3745.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/cisco-3745.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/cisco-iou-l3-v8.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/cisco-iou-l3-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/cisco-iou-l3.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/cisco-iou-l3.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/empty-vm-v8.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/empty-vm-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/juniper-vsrx.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/juniper-vsrx.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/microcore-linux.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/microcore-linux.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/openvswitch-v8.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/openvswitch-v8.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/appliances/openvswitch.gns3a` & `gns3_gui-3.0.0b3/tests/registry/appliances/openvswitch.gns3a`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/test_appliance.py` & `gns3_gui-3.0.0b3/tests/registry/test_appliance.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/test_appliance_to_template.py` & `gns3_gui-3.0.0b3/tests/registry/test_appliance_to_template.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/test_config.py` & `gns3_gui-3.0.0b3/tests/registry/test_config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/test_image.py` & `gns3_gui-3.0.0b3/tests/registry/test_image.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/registry/test_registry.py` & `gns3_gui-3.0.0b3/tests/registry/test_registry.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_compute.py` & `gns3_gui-3.0.0b3/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_compute_manager.py` & `gns3_gui-3.0.0b3/tests/test_compute_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_controller.py` & `gns3_gui-3.0.0b3/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_graphics_view.py` & `gns3_gui-3.0.0b3/tests/test_graphics_view.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_http_client.py` & `gns3_gui-3.0.0b3/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_image_manager.py` & `gns3_gui-3.0.0b3/tests/test_image_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_image_upload_manager.py` & `gns3_gui-3.0.0b3/tests/test_image_upload_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_link.py` & `gns3_gui-3.0.0b3/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_local_config.py` & `gns3_gui-3.0.0b3/tests/test_local_config.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_local_server.py` & `gns3_gui-3.0.0b3/tests/test_local_server.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_main_window.py` & `gns3_gui-3.0.0b3/tests/test_main_window.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_network_client.py` & `gns3_gui-3.0.0b3/tests/test_network_client.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_node.py` & `gns3_gui-3.0.0b3/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_progress.py` & `gns3_gui-3.0.0b3/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_project.py` & `gns3_gui-3.0.0b3/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_spice_console.py` & `gns3_gui-3.0.0b3/tests/test_spice_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_topology.py` & `gns3_gui-3.0.0b3/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_update_manager.py` & `gns3_gui-3.0.0b3/tests/test_update_manager.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_utils.py` & `gns3_gui-3.0.0b3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/test_vnc_console.py` & `gns3_gui-3.0.0b3/tests/test_vnc_console.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/utils/test_file_copy_worker.py` & `gns3_gui-3.0.0b3/tests/utils/test_file_copy_worker.py`

 * *Files identical despite different names*

### Comparing `gns3-gui-3.0.0b2/tests/utils/test_server_select.py` & `gns3_gui-3.0.0b3/tests/utils/test_server_select.py`

 * *Files identical despite different names*

