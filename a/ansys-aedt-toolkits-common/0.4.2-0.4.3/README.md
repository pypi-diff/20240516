# Comparing `tmp/ansys_aedt_toolkits_common-0.4.2.tar.gz` & `tmp/ansys_aedt_toolkits_common-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_aedt_toolkits_common-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_aedt_toolkits_common-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_aedt_toolkits_common-0.4.2.tar` & `ansys_aedt_toolkits_common-0.4.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0     1089 2024-05-09 12:15:52.269873 ansys_aedt_toolkits_common-0.4.2/LICENSE
--rw-r--r--   0        0        0     3531 2024-05-09 12:15:52.269873 ansys_aedt_toolkits_common-0.4.2/README.rst
--rw-r--r--   0        0        0     2684 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1230 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/__init__.py
--rw-r--r--   0        0        0    37347 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/api.py
--rw-r--r--   0        0        0      265 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/common_properties.toml
--rw-r--r--   0        0        0     1976 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/constants.py
--rw-r--r--   0        0        0     2517 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/logger_handler.py
--rw-r--r--   0        0        0     2541 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/models.py
--rw-r--r--   0        0        0     3706 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/multithreading_server.py
--rw-r--r--   0        0        0     7884 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/rest_api.py
--rw-r--r--   0        0        0     3339 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/thread_manager.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/__init__.py
--rw-r--r--   0        0        0    21177 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/actions_generic.py
--rw-r--r--   0        0        0     1051 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_properties.toml
--rw-r--r--   0        0        0        0 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/__init__.py
--rw-r--r--   0        0        0     4997 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py
--rw-r--r--   0        0        0     8951 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py
--rw-r--r--   0        0        0     2381 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/logger_handler.py
--rw-r--r--   0        0        0        0 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/main_window/__init__.py
--rw-r--r--   0        0        0    19844 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py
--rw-r--r--   0        0        0     2997 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/models.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py
--rw-r--r--   0        0        0     2406 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg
--rw-r--r--   0        0        0     2487 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg
--rw-r--r--   0        0        0    57746 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico
--rw-r--r--   0        0        0    35360 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png
--rw-r--r--   0        0        0     2379 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg
--rw-r--r--   0        0        0      982 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg
--rw-r--r--   0        0        0     1007 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg
--rw-r--r--   0        0        0     5074 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg
--rw-r--r--   0        0        0      819 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg
--rw-r--r--   0        0        0     6058 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg
--rw-r--r--   0        0        0     1124 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg
--rw-r--r--   0        0        0     2436 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg
--rw-r--r--   0        0        0     8449 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg
--rw-r--r--   0        0        0     1615 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg
--rw-r--r--   0        0        0     6064 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg
--rw-r--r--   0        0        0    24133 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg
--rw-r--r--   0        0        0     2300 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg
--rw-r--r--   0        0        0     4241 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg
--rw-r--r--   0        0        0     5091 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg
--rw-r--r--   0        0        0     1969 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg
--rw-r--r--   0        0        0      797 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg
--rw-r--r--   0        0        0     1058 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg
--rw-r--r--   0        0        0     2037 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg
--rw-r--r--   0        0        0     3207 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg
--rw-r--r--   0        0        0     1857 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg
--rw-r--r--   0        0        0      344 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu.svg
--rw-r--r--   0        0        0     1877 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg
--rw-r--r--   0        0        0     1749 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg
--rw-r--r--   0        0        0     7977 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg
--rw-r--r--   0        0        0      959 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg
--rw-r--r--   0        0        0     1263 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg
--rw-r--r--   0        0        0     3615 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg
--rw-r--r--   0        0        0      448 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_solve.svg
--rw-r--r--   0        0        0     2255 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg
--rw-r--r--   0        0        0      423 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/motor.svg
--rw-r--r--   0        0        0     3184 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg
--rw-r--r--   0        0        0     8477 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg
--rw-r--r--   0        0        0     2024 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg
--rw-r--r--   0        0        0     3641 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py
--rw-r--r--   0        0        0      897 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json
--rw-r--r--   0        0        0      899 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json
--rw-r--r--   0        0        0      868 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json
--rw-r--r--   0        0        0      894 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json
--rw-r--r--   0        0        0     1986 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py
--rw-r--r--   0        0        0     1947 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui
--rw-r--r--   0        0        0     1963 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui
--rw-r--r--   0        0        0     2421 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py
--rw-r--r--   0        0        0     2503 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py
--rw-r--r--   0        0        0     5116 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui
--rw-r--r--   0        0        0     4927 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py
--rw-r--r--   0        0        0     2780 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py
--rw-r--r--   0        0        0     2005 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py
--rw-r--r--   0        0        0      603 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py
--rw-r--r--   0        0        0     3871 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py
--rw-r--r--   0        0        0     1821 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py
--rw-r--r--   0        0        0     2587 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py
--rw-r--r--   0        0        0     9910 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py
--rw-r--r--   0        0        0      172 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/styles.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py
--rw-r--r--   0        0        0     7191 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py
--rw-r--r--   0        0        0     6578 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py
--rw-r--r--   0        0        0    10249 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py
--rw-r--r--   0        0        0    10452 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py
--rw-r--r--   0        0        0     2879 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py
--rw-r--r--   0        0        0      471 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/styles.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py
--rw-r--r--   0        0        0     1467 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py
--rw-r--r--   0        0        0     4120 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py
--rw-r--r--   0        0        0     1512 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py
--rw-r--r--   0        0        0      405 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/styles.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py
--rw-r--r--   0        0        0     4896 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py
--rw-r--r--   0        0        0     2165 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py
--rw-r--r--   0        0        0     1463 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py
--rw-r--r--   0        0        0    12519 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py
--rw-r--r--   0        0        0    11434 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py
--rw-r--r--   0        0        0     4599 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py
--rw-r--r--   0        0        0     4408 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py
--rw-r--r--   0        0        0      290 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/styles.py
--rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py
--rw-r--r--   0        0        0    21788 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py
--rw-r--r--   0        0        0     7009 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/utils.py
--rw-r--r--   0        0        0     6019 1970-01-01 00:00:00.000000 ansys_aedt_toolkits_common-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-16 08:38:25.553665 ansys_aedt_toolkits_common-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3531 2024-05-16 08:38:25.553665 ansys_aedt_toolkits_common-0.4.3/README.rst
+-rw-r--r--   0        0        0     2684 2024-05-16 08:38:25.557664 ansys_aedt_toolkits_common-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1230 2024-05-16 08:38:25.557664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.557664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/__init__.py
+-rw-r--r--   0        0        0    37391 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/api.py
+-rw-r--r--   0        0        0      265 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/common_properties.toml
+-rw-r--r--   0        0        0     1976 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/constants.py
+-rw-r--r--   0        0        0     2517 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/logger_handler.py
+-rw-r--r--   0        0        0     2541 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/models.py
+-rw-r--r--   0        0        0     3706 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/multithreading_server.py
+-rw-r--r--   0        0        0     7884 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/rest_api.py
+-rw-r--r--   0        0        0     3339 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/thread_manager.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/__init__.py
+-rw-r--r--   0        0        0    21182 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/actions_generic.py
+-rw-r--r--   0        0        0     1051 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/common_properties.toml
+-rw-r--r--   0        0        0        0 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/common_windows/__init__.py
+-rw-r--r--   0        0        0     5169 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py
+-rw-r--r--   0        0        0     8951 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py
+-rw-r--r--   0        0        0     2381 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/logger_handler.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/main_window/__init__.py
+-rw-r--r--   0        0        0    19844 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py
+-rw-r--r--   0        0        0     2997 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/models.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py
+-rw-r--r--   0        0        0     2406 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg
+-rw-r--r--   0        0        0     2487 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg
+-rw-r--r--   0        0        0    57746 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico
+-rw-r--r--   0        0        0    35360 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png
+-rw-r--r--   0        0        0     2379 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg
+-rw-r--r--   0        0        0      982 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg
+-rw-r--r--   0        0        0     1007 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg
+-rw-r--r--   0        0        0     5074 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg
+-rw-r--r--   0        0        0      819 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg
+-rw-r--r--   0        0        0     6058 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg
+-rw-r--r--   0        0        0     1124 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg
+-rw-r--r--   0        0        0     2436 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg
+-rw-r--r--   0        0        0     8449 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg
+-rw-r--r--   0        0        0     1615 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg
+-rw-r--r--   0        0        0     6064 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg
+-rw-r--r--   0        0        0    24133 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg
+-rw-r--r--   0        0        0     2300 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg
+-rw-r--r--   0        0        0     4241 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg
+-rw-r--r--   0        0        0     5091 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg
+-rw-r--r--   0        0        0     1969 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg
+-rw-r--r--   0        0        0      797 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg
+-rw-r--r--   0        0        0     1058 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg
+-rw-r--r--   0        0        0     2037 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg
+-rw-r--r--   0        0        0     3207 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg
+-rw-r--r--   0        0        0     1857 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg
+-rw-r--r--   0        0        0      344 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu.svg
+-rw-r--r--   0        0        0     1877 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg
+-rw-r--r--   0        0        0     1749 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg
+-rw-r--r--   0        0        0     7977 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg
+-rw-r--r--   0        0        0      959 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg
+-rw-r--r--   0        0        0     1263 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg
+-rw-r--r--   0        0        0     3615 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg
+-rw-r--r--   0        0        0      448 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_solve.svg
+-rw-r--r--   0        0        0     2255 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg
+-rw-r--r--   0        0        0      423 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/motor.svg
+-rw-r--r--   0        0        0     3184 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg
+-rw-r--r--   0        0        0     8477 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg
+-rw-r--r--   0        0        0     2024 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg
+-rw-r--r--   0        0        0     3641 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json
+-rw-r--r--   0        0        0      899 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json
+-rw-r--r--   0        0        0      868 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json
+-rw-r--r--   0        0        0      894 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json
+-rw-r--r--   0        0        0     1986 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py
+-rw-r--r--   0        0        0     1947 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui
+-rw-r--r--   0        0        0     1963 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui
+-rw-r--r--   0        0        0     2421 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py
+-rw-r--r--   0        0        0     2503 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py
+-rw-r--r--   0        0        0     5116 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui
+-rw-r--r--   0        0        0     4927 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py
+-rw-r--r--   0        0        0     2780 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py
+-rw-r--r--   0        0        0     2005 2024-05-16 08:38:25.561664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py
+-rw-r--r--   0        0        0      603 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py
+-rw-r--r--   0        0        0     3871 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py
+-rw-r--r--   0        0        0     1821 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py
+-rw-r--r--   0        0        0     2587 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py
+-rw-r--r--   0        0        0     9910 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py
+-rw-r--r--   0        0        0      172 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py
+-rw-r--r--   0        0        0     7191 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py
+-rw-r--r--   0        0        0     6578 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py
+-rw-r--r--   0        0        0    10249 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py
+-rw-r--r--   0        0        0    10452 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py
+-rw-r--r--   0        0        0     2879 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py
+-rw-r--r--   0        0        0      471 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py
+-rw-r--r--   0        0        0     4120 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py
+-rw-r--r--   0        0        0     1512 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py
+-rw-r--r--   0        0        0      405 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py
+-rw-r--r--   0        0        0     4896 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py
+-rw-r--r--   0        0        0     2165 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py
+-rw-r--r--   0        0        0     1463 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py
+-rw-r--r--   0        0        0    12519 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py
+-rw-r--r--   0        0        0    11434 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py
+-rw-r--r--   0        0        0     4599 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py
+-rw-r--r--   0        0        0     4408 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py
+-rw-r--r--   0        0        0      290 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py
+-rw-r--r--   0        0        0    21788 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py
+-rw-r--r--   0        0        0     7229 2024-05-16 08:38:25.565664 ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/utils.py
+-rw-r--r--   0        0        0     6019 1970-01-01 00:00:00.000000 ansys_aedt_toolkits_common-0.4.3/PKG-INFO
```

### Comparing `ansys_aedt_toolkits_common-0.4.2/LICENSE` & `ansys_aedt_toolkits_common-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/README.rst` & `ansys_aedt_toolkits_common-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/pyproject.toml` & `ansys_aedt_toolkits_common-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 """
 pyaedt-toolkits.
 
 ansys.aedt.toolkits.common
 """
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
```

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/api.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -675,15 +675,17 @@
         >>> toolkit_api.release_aedt()
 
         """
         if self.aedtapp:
             self.release_aedt()
         if not self.connect_aedt():  # pragma: no cover
             return False
-        if not project_name and self.properties.active_project and os.path.exists(self.properties.active_project):
+        if (
+            not project_name and self.properties.active_project and os.path.exists(self.properties.active_project)
+        ):  # pragma: no cover
             project_name = os.path.abspath(self.properties.active_project)
         if not os.path.exists(project_name + ".lock") and self.desktop and project_name:
             self.desktop.odesktop.OpenProject(project_name)
             logger.debug("Project {} is opened".format(project_name))
             self.__save_project_info()
             self.release_aedt(False, False)
             return True
```

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/constants.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/logger_handler.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/logger_handler.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/models.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/models.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/multithreading_server.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/multithreading_server.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/rest_api.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/rest_api.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/thread_manager.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/backend/thread_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/actions_generic.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/actions_generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,15 +448,16 @@
         else:
             be_properties["active_project"] = active_project
 
         design_list = be_properties["design_list"].get(active_project)
         if not design_list:
             design_list = ["No Design"]
             be_properties["active_design"] = "No Design"
-        be_properties["design_list"] = {active_project: design_list}
+        else:
+            be_properties["active_design"] = design_list[0]
         self.set_properties(be_properties)
         return design_list
 
     def save_project(self):
         """Save the current AEDT project.
 
         Opens a file dialog to select a location to save the AEDT project. The project is saved
```

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_properties.toml` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/common_properties.toml`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,26 +100,30 @@
 
         main_logo.setFixedSize(240, 120)
 
         # Check backend connection
         success = self.app.check_connection()
         if success:
             backend_properties = self.app.get_properties()
-            if backend_properties.get("active_project") and backend_properties.get("active_design"):
+            if (
+                backend_properties.get("active_project")
+                and backend_properties.get("active_design")
+                or backend_properties.get("selected_process") != 0
+            ):
                 self.update_project()
                 self.update_design()
 
     def update_project(self):
         self.project_combobox.blockSignals(True)
         project_list = self.app.get_aedt_data()
         self.main_window.home_menu.project_combobox.setEnabled(True)
         self.main_window.home_menu.project_combobox.clear()
         self.main_window.home_menu.project_combobox.addItems(project_list)
         self.project_combobox.blockSignals(False)
         return project_list
 
     def update_design(self):
         self.project_combobox.blockSignals(True)
-        design_list = self.app.update_design_names()
+        design_list = self.app.update_design_names(self.main_window.home_menu.project_combobox.currentText())
         self.main_window.home_menu.design_combobox.clear()
         self.main_window.home_menu.design_combobox.addItems(design_list)
         self.project_combobox.blockSignals(False)
```

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/logger_handler.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/logger_handler.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/models.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/models.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/utils.py` & `ansys_aedt_toolkits_common-0.4.3/src/ansys/aedt/toolkits/common/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,25 +31,25 @@
 import threading
 import time
 
 import psutil
 import requests
 
 
-def download_file(url, local_filename):
+def download_file(url, local_filename):  # pragma: no cover
     """Download a file from a URL into a local file."""
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
         with open(local_filename, "wb") as f:
             for chunk in r.iter_content(chunk_size=4096):
                 f.write(chunk)
     return local_filename
 
 
-def is_server_running(server="localhost", port=5001):
+def is_server_running(server="localhost", port=5001):  # pragma: no cover
     """Check if port is used."""
     result = None
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
         result = sock.connect_ex((server, port))
     except socket.error as e:
         print(f"Socket error occurred: {e}")
@@ -66,36 +66,36 @@
     for _ in range(max_attempts):
         try:
             print("Trying port {}.".format(str(port)))
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 s.bind((server, port))
                 print("Port {} is free.".format(str(port)))
                 return port
-        except OSError:
+        except OSError:  # pragma: no cover
             print("Port {} is used.".format(str(port)))
-        except Exception as e:
+        except Exception as e:  # pragma: no cover
             print("An error occurred:", e)
             return False
-        port = random.randint(start_port, start_port + 100)
-    return False
+        port = random.randint(start_port, start_port + 100)  # pragma: no cover
+    return False  # pragma: no cover
 
 
-def wait_for_server(server="localhost", port=5001, timeout=10.0):
+def wait_for_server(server="localhost", port=5001, timeout=10.0):  # pragma: no cover
     """Wait for server response."""
     start_time = time.time()
     first_time = True
     while time.time() - start_time < timeout:
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
             sock.settimeout(2)
             sock.connect((server, port))
             sock.close()
             print("\nServer is ready.")
             return True
-        except socket.error as e:
+        except socket.error as e:  # pragma: no cover
             print(f"Socket error occurred: {e}")
             if first_time:
                 print("Server not ready yet. Retrying...", end="")
                 first_time = False
             else:
                 print(".", end="")
             time.sleep(1)
@@ -122,39 +122,39 @@
     """Run command as a separate thread."""
     thread = threading.Thread(target=run_command, args=command, kwargs={"is_linux": is_linux}, name=name)
     thread.daemon = True
     thread.start()
     return thread
 
 
-def clean_python_processes(url, port):
+def clean_python_processes(url, port):  # pragma: no cover
     """Clean up Python processes."""
     for conn in psutil.net_connections():
         (ip_tmp, port_tmp) = conn.laddr
         pid = conn.pid
         if ip_tmp == url and port_tmp == port and pid and pid != 0:
             try:
                 process = psutil.Process(pid)
                 print(f"Killing process {process.pid} on {ip_tmp}:{port_tmp}")
                 process.terminate()
             except psutil.NoSuchProcess:
                 print(f"Process {process.pid} on {ip}:{port_tmp} was already killed")
 
 
-def check_backend_communication(url_call):
+def check_backend_communication(url_call):  # pragma: no cover
     """Check backend communication."""
     try:
         response = requests.get(url_call + "/health")
         return response.ok
     except requests.exceptions.RequestException:
         print("Failed to check backend communication.")
         return False
 
 
-def process_desktop_properties(is_linux, url_call):
+def process_desktop_properties(is_linux, url_call):  # pragma: no cover
     """Process desktop properties."""
     desktop_pid = None
     desktop_version = None
     grpc = True
     is_student = False
     if "PYAEDT_SCRIPT_VERSION" in os.environ and "PYAEDT_SCRIPT_PORT" in os.environ:
         desktop_version = os.environ["PYAEDT_SCRIPT_VERSION"]
```

### Comparing `ansys_aedt_toolkits_common-0.4.2/PKG-INFO` & `ansys_aedt_toolkits_common-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-aedt-toolkits-common
-Version: 0.4.2
+Version: 0.4.3
 Summary: User interface example repository to create your toolkit.
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

