# Comparing `tmp/pyodide_mkdocs_theme-0.7.1.tar.gz` & `tmp/pyodide_mkdocs_theme-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.7.1.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-1.0.0.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.7.1.tar` & `pyodide_mkdocs_theme-1.0.0.tar`

### file list

```diff
@@ -1,76 +1,74 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.7.1/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.7.1/README.md
--rw-r--r--   0        0        0     1347 2024-05-01 21:31:49.354861 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-05-01 21:31:49.386862 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4979 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    24750 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    15749 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     3861 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11723 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    13163 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     7120 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4483 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4485 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    13652 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11739 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0     6663 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
--rw-r--r--   0        0        0     1603 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0    10204 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
--rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     8198 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0      374 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6933 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/scripts/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     3979 2024-05-01 21:31:49.354861 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py
--rw-r--r--   0        0        0     5565 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     5496 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7420 2024-05-01 08:58:57.928287 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1702 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4435 2024-05-01 19:58:44.788456 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     6642 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0    10326 2024-05-01 21:03:11.643963 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     7724 2024-05-01 21:03:11.647963 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16637 2024-05-01 21:21:46.481196 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0    11261 2024-05-01 20:52:28.704573 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9195 2024-04-29 14:09:33.377858 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3740 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5379 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4213 2024-05-01 21:21:46.493197 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1761 2024-05-01 21:31:46.854788 pyodide_mkdocs_theme-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-1.0.0/README.md
+-rw-r--r--   0        0        0     1347 2024-05-15 21:11:40.512726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2591 2024-05-10 09:58:57.896751 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-15 21:11:40.564727 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1322 2024-05-10 09:58:57.908752 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0     1063 2024-05-10 09:58:57.944753 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-05-12 18:52:50.335028 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     5919 2024-05-14 21:00:36.843691 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     2992 2024-05-14 21:00:36.843691 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py
+-rw-r--r--   0        0        0        0 2024-05-10 09:58:57.968754 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0    11922 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py
+-rw-r--r--   0        0        0    16534 2024-05-10 09:58:58.012755 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py
+-rw-r--r--   0        0        0    21130 2024-05-14 21:00:36.899692 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py
+-rw-r--r--   0        0        0     4850 2024-05-14 21:00:36.899692 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py
+-rw-r--r--   0        0        0     3470 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py
+-rw-r--r--   0        0        0     2435 2024-05-10 09:58:58.072757 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11591 2024-05-10 09:58:58.072757 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13668 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     7141 2024-05-11 20:11:49.116411 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0    14460 2024-05-14 21:00:36.971694 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4776 2024-05-14 21:00:37.003695 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0        0 2024-05-10 09:58:58.128759 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    15211 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11391 2024-05-14 21:00:37.003695 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0     9693 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
+-rw-r--r--   0        0        0     1603 2024-05-10 09:58:58.168760 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     6652 2024-05-10 09:58:58.188760 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
+-rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9042 2024-05-14 21:00:37.039696 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1163 2024-05-14 21:00:37.075698 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     9480 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0     4229 2024-05-15 21:11:40.512726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     5487 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/mkdocs.yml
+-rw-r--r--   0        0        0     3593 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/model.py
+-rw-r--r--   0        0        0      823 2024-05-10 09:58:58.304764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 09:58:58.304764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-10 09:58:58.304764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg
+-rw-r--r--   0        0        0     1645 2024-05-10 09:58:58.304764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     6093 2024-05-15 20:46:22.160139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0    10609 2024-05-14 21:00:37.167700 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1770 2024-05-15 21:11:37.872664 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0    10814 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js
+-rw-r--r--   0        0        0    14528 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js
+-rw-r--r--   0        0        0     1183 2024-05-15 21:11:40.508726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js
+-rw-r--r--   0        0        0     8220 2024-05-15 21:11:40.508726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js
+-rw-r--r--   0        0        0    18519 2024-05-15 21:11:40.508726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js
+-rw-r--r--   0        0        0    12716 2024-05-10 09:58:58.344765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js
+-rw-r--r--   0        0        0     7231 2024-05-14 21:00:37.171700 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js
+-rw-r--r--   0        0        0    11253 2024-05-10 09:58:58.344765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0     4455 2024-05-14 21:00:37.195701 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0     5341 2024-05-10 09:58:58.344765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     2635 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     3831 2024-05-10 09:58:58.356765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css
+-rw-r--r--   0        0        0     1078 2024-05-10 09:58:58.356765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css
+-rw-r--r--   0        0        0     1947 2024-05-10 09:58:58.356765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css
+-rw-r--r--   0        0        0     3744 2024-05-15 20:46:22.160139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css
+-rw-r--r--   0        0        0     3904 2024-05-10 09:58:58.364766 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css
+-rw-r--r--   0        0        0     1918 2024-05-14 21:00:37.255703 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css
+-rw-r--r--   0        0        0     1766 2024-05-15 21:11:37.908665 pyodide_mkdocs_theme-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-1.0.0/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.7.1/LICENSE` & `pyodide_mkdocs_theme-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/README.md` & `pyodide_mkdocs_theme-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 
 import sys
 from pathlib import Path
 from argparse import ArgumentParser
 from contextlib import redirect_stdout
 
 from .__version__ import __version__
-from .scripts.custom_lang import display_lang
-from .scripts.mkdocs_yaml import display_yml
 
 
 
 parser = ArgumentParser(
     'pyodide_mkdocs_theme',
     description = "Scripts for pyodide-mkdocs-theme",
     epilog = "Copyleft GNU GPLv3 🄯 2024 Frédéric Zinelli. "
@@ -37,14 +35,17 @@
 parser.add_argument(
     '-V', '--version', action='version', version=f'pyodide-mkdocs-theme {__version__}'
 )
 parser.add_argument(
     '--lang', action='store_true', help='Print the base python code to customize some messages.'
 )
 parser.add_argument(
+    '--py', action='store_true', help='Print an example of python file, for {{IDE(...)}} or {{terminal(...)}} macros.'
+)
+parser.add_argument(
     '--yml', action='store_true', help='Print a base configuration for the mkdocs.yml file.'
 )
 parser.add_argument(
     '-F', '--file', default="",
     help='Use this argument to write the information into a file instead of the stdout '
          '(existing content will be overridden. Use an absolute path or relative to cwd).'
 )
@@ -55,17 +56,27 @@
     # pylint: disable=multiple-statements
 
     if len(sys.argv) < 2:
         sys.argv.append('-h')
 
     args = parser.parse_args()
 
+    def display(filename:str):
+        """ Display the base code for GUI messages customizations """
+
+        src = Path(__file__).parent / 'scripts_files' / filename
+        txt = src.read_text(encoding='utf-8')
+        print(txt)
+
+
+
     def inner():
-        if args.yml:     display_yml()
-        elif args.lang:  display_lang()
+        if args.lang:   display('custom_lang.py')
+        elif args.yml:  display('mkdocs.yml')
+        elif args.py:   display('model.py')
 
 
     if not args.file:
         inner()
 
     else:
         path = Path(args.file)
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 from mkdocs.config import config_options as C
 
 
 from .pyodide_logger import logger
 
 
 
-def typ_deprecated_with_custom_msg(prop:str, typ:Any):
-    return C.Deprecated(
-        message=f"Macros using {prop} may not work anymore and will be removed in the future. "
-                "Please contact the author of the theme if you need this macro/tool.",
-        option_type = C.Optional(C.Type(typ)),
+def typ_deprecated_with_custom_msg(prop:str, typ:Any, is_old=True):
+    message=(
+        f"Macros using {prop} may not work anymore and will be removed in the future. "
+        "Please contact the author of the theme if you need this macro/tool."
+    ) if is_old else (
+        f"The {prop} option is deprecated: it has no use anymore abd will be removed in the future."
     )
+    return C.Deprecated( message=message, option_type = C.Optional(C.Type(typ)) )
 
 
 def deprecation_warning(that:str):
     logger.warning(that)
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,13 +13,20 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
-from mkdocs.exceptions import ConfigurationError
+from mkdocs.exceptions import ConfigurationError, BuildError
+
 
 
 class PyodideConfigurationError(ConfigurationError):
     """ Something went wrong in the Pyodide theme itself """
 
+
+class PyodideMacrosParsingError(BuildError):
+    """
+    Invalid syntax found while parsing a markdown file, when gathering
+    information about macros calls indentations in the page.
+    """
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -108,25 +108,39 @@
 def terminal(term_id:str, kls:str, n_lines_h:int, env:'PyodideMacrosPlugin', **kw):
     """
     Build a terminal div with its button. If n_lines_h is falsy, the height of the div isn't
     handled. Otherwise, it's the mac of n_lines_h and 5.
     """
 
     tip = tooltip(env.lang.feedback, width_em=env.lang.feedback.em, shift=90)
-    btn_div = div(
+    feed_div = div(
         _BTN_STDOUT_SVG + tip,
-        kls = f"{ HtmlClass.stdout_ctrl } { HtmlClass.tooltip }"
+        kls = f"twemoji { HtmlClass.stdout_ctrl } { HtmlClass.tooltip }"
     )
+
+    tip_wrap = tooltip(env.lang.wrap_term, width_em=env.lang.wrap_term.em, shift=90)
+    wrap_div = div(
+        _BTN_MATERIAL_OVERFLOW + tip_wrap,
+        kls=f"{ HtmlClass.stdout_wrap_btn } {HtmlClass.tooltip }",
+        style="--wrap-opacity: 30%",
+    )
+
+    btns_div = div(
+        feed_div + wrap_div,
+        kls=f"{ HtmlClass.term_btns_wrapper }",
+    )
+
     if n_lines_h:
         n_lines_h = max(n_lines_h, 5)
         kw['style'] = f"--n-lines:{ n_lines_h };" + kw.get('style','')
     kw['style'] = 'line-height:24px;' + kw.get('style','')
 
-    term_div = div(btn_div, id=term_id, kls=kls, **kw)
-    return term_div
+    term_div = div(id=term_id, kls=kls, **kw)
+    global_div = div(term_div+btns_div, kls=HtmlClass.term_wrapper)
+    return global_div
 
 
 _BTN_STDOUT_SVG = '''
 <svg viewBox="0 0 24 24" fill="none"
     stroke="var(--md-default-fg-color)" stroke-width="1" stroke-linecap="round" stroke-linejoin="round"
     xmlns="http://www.w3.org/2000/svg" xmlns:svg="http://www.w3.org/2000/svg">
 <g>
@@ -140,7 +154,16 @@
   <path d="M 7.9,17.25 H 11.9" />
   <path d="m 8,5.25 h 4" />
   <path d="m 8,7.25 h 4" />
 </g>
 <g><path class="stdout-x-ray-svg" d="M 3,11.4 v 6 L 21,13.8 V 7.7 Z" style="fill:var(--md-default-bg-color);stroke-width:0;" /></g>
 </svg>
 '''.replace('\n',' ')       # needed otherwise insertion in admonitions fails... XD
+
+
+# Cannot use the `:material-overflow:` syntax, because not rendered when the terminal is not
+# inside an admonition or tab... DX (markdown attributes missing, but putting them in IDE makes a whole mess of them...)
+_BTN_MATERIAL_OVERFLOW = '''
+<span class="twemoji">
+<svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
+<path d="M7 21H5V3h2v18m7-18h-2v6h2V3m0 12h-2v6h2v-6m5-3-3-3v2H9v2h7v2l3-3Z">
+</path></svg></span>'''.replace('\n',' ')       # needed otherwise insertion in admonitions fails... XD
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,70 +18,69 @@
 """
 
 # pylint: disable=unused-argument
 
 
 import re
 import hashlib
-from typing import Any, ClassVar, List, Literal, Optional, Tuple, Union
+from typing import Any, ClassVar, Dict, List, Literal, Optional, Tuple, Union
 from dataclasses import dataclass
 from pathlib import Path
 from math import inf
 
 from mkdocs.exceptions import BuildError
 
 from pyodide_mkdocs_theme.pyodide_macros.messages import Tip
+from pyodide_mkdocs_theme.pyodide_macros.paths_utils import get_ide_button_png_path
 
-from ... import html_builder as Html
-from ...pyodide_logger import logger
-from ...tools_and_constants import HtmlClass, Prefix, ScriptKind
-from ...pages_and_ides_configs import IdeConfigKey
-from ...parsing import build_code_fence, items_comma_joiner
-from ...paths_utils import convert_url_to_utf8, to_uri
-from ...plugin.maestro_IDE import MaestroIDE
+from .. import html_builder as Html
+from ..pyodide_logger import logger
+from ..tools_and_constants import HtmlClass, IdeConstants, ScriptKind
+from ..parsing import items_comma_joiner
+from ..plugin.maestro_IDE import MaestroIDE
 
 from .ide_files_data import IdeFilesExtractor
 
 
 
 
 #---------------------------------------------------------------------------------
 
 
 
 
 
 @dataclass
-class Ide:
+class IdeManager:
     """
-    Builds an editor + a terminal + the buttons and extra logistic needed for them.
+    Base class managing the information for the underlying environment.
+    To be extended by a concrete implementation, providing the actual logistic to
+    build the html hierarchy (see self.make_element).
+
+    This base class holds all the possible arguments fo any concrete class.
     """
 
+
     # Defined on instantiation:
     #--------------------------
 
-    my_env: MaestroIDE
+    env: MaestroIDE
     """ The MaestroEnv singleton """
 
     py_name: str
     """ Base name for the files to use (first argument passed to the macros)
         Partial path from the directory holding the sujet.md file, to the one holding all the
         other required files, ending with the common prefix for the exercice.
         Ex:   "exo" to extract:   "exo.py", "exo_corr.py", "exo_test.py", ...
                 "sub_exA/exo" for:  "sub_exA/exo.py", "sub_exA/exo_corr.py", ...
     """
 
-    mode: Union[Literal[""],Literal["_v"]]
-    """ The terminal will be below (mode="") or on the right (mode="_v") of the editor.
-        (what an awful interface, yeah... x) )
-    """
-
-    max_attempts: Optional[Union[int, Literal["+"]]]
-    """ Maximum number of attempts before the solution admonition will become available.
-        If None, use the global default value.
+    id: Optional[int]
+    """ Used to disambiguate the ids of two IDEs, if the same file is used several times
+        in the document.
     """
 
     excluded: str
     """ String of spaces or coma separated python functions or modules/packages that are forbidden
         at runtime. By default, nothing is forbidden.
             - Every string section that matches a builtin callable forbid that function by
               replacing it with another function which will raise an error if called.
@@ -93,42 +92,63 @@
 
         Note that the restrictions are rather strict, and may have unexpected side effects, such
         as, forbidding `exec` will also forbid to import numpy, because the package relies on exec
         for some operations at import time.
         To circumvent such a kind of problems, use the white_list argument.
     """
 
-    max_size: int
-    """ Max height of the editor (in number of lines) """
-
     white_list: str
     """ String of spaces or coma separated python modules/packages names the have to be
         preloaded before the code restrictions are enforced on the user's side.
     """
 
-    id: Optional[int]
-    """ Used to disambiguate the ids of two IDEs, if the same file is used several times
-        in the document.
+    rec_limit: int
+    """ If used, the recursion limit of the pyodide runtime will be updated before the user's
+        code or the tests are run.
+        Note that this also forbids the use of the `sys.setrecurionlimit` at runtime.
+    """
+
+    mode: Union[Literal[""],Literal["_v"]] = ""
+    """ The terminal will be below (mode="") or on the right (mode="_v") of the editor.
+        (what an awful interface, yeah... x) )
     """
 
-    auto_log_assert: Optional[bool]
+    max_attempts: Optional[Union[int, Literal["+"]]] = None
+    """ Maximum number of attempts before the solution admonition will become available.
+        If None, use the global default value.
+    """
+
+    max_size: Optional[int] = None
+    """
+    Max height of the editor (in number of lines)
+    """
+
+    auto_log_assert: Optional[bool] = None
     """ If True, failing assertions without feedback during the private tests will be
         augmented automatically with the code of the assertion itself. If None, use
         the global `show_assertion_code_on_failed_test` plugin value and defined in
         `CONFIG.showAssertionCodeOnFailedTest` in the JS runtime.
     """
 
-    rec_limit: int
-    """ If used, the recursion limit of the pyodide runtime will be updated before the user's
-        code or the tests are run.
-        Note that this also forbids the use of the `sys.setrecurionlimit` at runtime.
+    term_height: Optional[int] = None
+    """
+    Number of lines to define the height of the terminal (unless it's vertical)
+    """
+
+    prefill_term: Optional[str] = None
+    """
+    Command to prefill the terminal on startup.
     """
 
-    term_height: int
-    """ Number of lines to define the height of the terminal (unless it's vertical) """
+    extra_kw: Optional[Dict[str,Any]] = None
+    """
+    Any kw left in the original call.
+    Should be always be None when reaching IdeManager.__post_init__. This allows subclasses
+    to handle the extra (legacy) keywords on their side.
+    """
 
 
     # defined during post_init
     #-------------------------
 
 
     files_data: IdeFilesExtractor = None
@@ -142,22 +162,65 @@
     indentation: str = ''
     """ Indentation on the left of the macro call, as str """
 
 
     #-------------------------
 
 
-    MIN_IDE_ID_DIGITS: ClassVar[str] = 8
+    ID_PREFIX: ClassVar[str] = None
+    """ Must be overridden in the child class """
+
+    NEED_INDENTS: ClassVar[bool] = False
+    """
+    Specify the macro had adding multiline content (so it _will_ consume one indentation data).
+    """
+
+    KW_TO_TRANSFER: ClassVar[Tuple[ Union[str, Tuple[str,str]]] ]  = ()
+    """
+    Configuration of the keywords that should be extracted if given in the constructor.
+    This is an Iterable of  (argument, property) pairs.
+    If an element is a string, it will be used as (value, value.lower())
+    """
+
+    DEFAULTS_EXTRACTION: ClassVar[Tuple[Tuple[str,str]]] = ()
+    """
+    Configuration of the properties that should extract a global default value, if it's still
+    set to None after the extra arguments have been handled.
+    This is an Iterable of  (argument, property) pairs.
+    """
+
+    JS_EXPORTED_GENERICS: ClassVar[set] = set('''
+        py_name
+        env_content
+        user_content
+        public_tests
+        secret_tests
+        post_content
+        excluded
+        excluded_methods
+        rec_limit
+        white_list
+    '''.split())
+    """
+    Values that are always exported to JS, whatever the tool.
+    """
 
-    INFINITY_SYMBOL: ClassVar[str] = "∞"
+    JS_EXPORTED_VALUES: ClassVar[set] = None
+    """
+    If defined, gives the names of all the properties that should be exported to JS.
+    HAS TO BE OVERRIDDEN by the subclasses.
+    """
 
+    NEEDED_KINDS: ClassVar[Tuple[ScriptKind]] = ScriptKind.pyodide,
+    """
+    Register the kind of js scripts that must be added to the page, for the current object.
+    """
 
-    ICON_TEMPLATE: ClassVar[str] = (
-        "{lvl_up}/pyodide-mkdocs/IDE-and-buttons/images/icons8-{button_name}-64.png"
-    )
+
+    #-------------------------
 
 
     @property               # pylint: disable-next=all
     def has_corr(self):     return self.files_data.has_corr
     @property               # pylint: disable-next=all
     def has_secrets(self):  return self.files_data.has_secrets
     @property               # pylint: disable-next=all
@@ -169,92 +232,143 @@
     def has_any_corr_rem(self):
         return self.has_corr or self.has_rem or self.has_vis_rem
 
 
 
     def __post_init__(self):
 
-        to_globals_if_none = (
-            ('max_attempts', 'max_attempts_before_corr_available'),
-            ('max_size',     'default_ide_height_lines'),
-        )
-        for prop,conf_prop in to_globals_if_none:
-            if getattr(self, prop) is None:
-                def_val = getattr(self.my_env, conf_prop)
-                setattr(self, prop, def_val)
+        self.handle_extra_args()
 
-        self.files_data = IdeFilesExtractor(self.my_env, self.py_name, self.id)
+        self.env.set_current_page_insertion_needs(*self.NEEDED_KINDS)
+
+        self.files_data = IdeFilesExtractor(self.env, self.py_name)
 
         # Extract max number of attempts from file or macro argument, clean up the file if needed,
         # then pick the correct number of attempts and set it in the global structure.
         # Also defines self.ide_content.
         max_attempts = self._define_max_attempts_symbols_and_value()
 
-        self._validate_config(max_attempts)
+        self._validate_files_config(max_attempts)
+
+        self.has_check_btn   = self.has_secrets # or self.has_any_corr_rem and cnt_n_span != inf
 
+        if self.rec_limit < -1:         # standardization
+            self.rec_limit = -1
 
-        if 0 <= self.rec_limit < self.my_env.MIN_RECURSION_LIMIT:
+        if -1 < self.rec_limit < IdeConstants.min_recursion_limit:
             raise BuildError(
                 f"The recursion limit for {self} is set too low and may causes runtime troubles. "
-                f"Please set it to at least { self.my_env.MIN_RECURSION_LIMIT }."
+                f"Please set it to at least { IdeConstants.min_recursion_limit }."
             )
 
-        if self.id is not None and not isinstance(self.id, int):
-            raise BuildError(f'The ID argument should be an integer, for {self}')
+        # Extract python content and compute editor name:
+        if self.ID_PREFIX is None:
+            raise NotImplementedError("Subclasses should override the ID_PREFIX class property.")
 
 
-        # Extract python content and compute editor name:
-        exo_py: Optional[Path] = self.files_data.exo_py
-        id_ide: str = self._generate_id_ide(exo_py)
-        self.editor_name = f"{ Prefix.editor_ }{ id_ide }"
+        self.editor_name = self.generate_id()
 
 
         # Compute all code exclusions and white list of imports:
         white_list = self._compute_exclusions_and_white_list("white_list")
         excluded = self._compute_exclusions_and_white_list("excluded")
         excluded_methods = [ meth for meth in excluded if     meth.startswith('.') ]
         excluded =         [ meth for meth in excluded if not meth.startswith('.') ]
 
 
         # Search the indentation level for the current IDE:
-        is_v = self.mode.strip('_')
-        quotes = """['"]"""
-        script_pattern = "" if not self.py_name else f"{quotes}{ self.py_name }{quotes}"
-        id_pattern = r'(?!.*?ID\s*=)' if self.id is None else rf".*?ID\s*=\s*{ self.id }\b"
-
-        ide_jinja_reg = re.compile( rf"IDE{ is_v }\(\s*{ script_pattern }{ id_pattern }" )
-        self.indentation = self.my_env.get_indent_in_current_page(ide_jinja_reg)
-
+        if self.NEED_INDENTS:
+            self.indentation = self.env.get_macro_indent()
 
-
-        to_register: List[Tuple[IdeConfigKey,Any]] = [
+        # Guess an explicative enough py_name (when downloading the IDE content):
+        root_name = Path(self.env.page.url).stem
+        py_path = Path(self.py_name).stem
+        py_name = f"{root_name}-{py_path}".strip('-') or 'unknown'
+
+        # Prepare the dump of configuration to JS:
+        to_register: List[Tuple[str,Any]] = [
+            #-----------------------------------------------------
+            # Generic properties (always exported, but may be useless depending on the actual class)
+            ('py_name',             py_name+'.py'),
             ('env_content',         self.files_data.env_content),
             ('user_content',        self.files_data.user_content),
             ('public_tests',        self.files_data.public_tests),
             ('secret_tests',        self.files_data.secret_tests),
             ('post_content',        self.files_data.post_content),
-            ('corr_rem_config',     self.files_data.corr_rem_bit_mask),
-            ('attempts_left',       max_attempts),
+
             ("excluded",            excluded),
             ("excluded_methods",    excluded_methods),
+            ("rec_limit",           self.rec_limit),
             ("white_list",          white_list),
+
+            #-----------------------------------------------------
+            # Specific to some concrete class
+
+            # IDEs:
+            ('attempts_left',       max_attempts),
             ("auto_log_assert",     self.auto_log_assert),
-            ("rec_limit",           self.rec_limit),
+            ('corr_rems_mask',      self.files_data.corr_rems_bit_mask),
+            ("has_check_btn",       self.has_check_btn),
+
+            # Terminals:
+            ("prefill_term",        self.prefill_term),
+        ]
+
+        actually_registered = [
+            rule for rule in to_register
+                 if rule[0] in self.JS_EXPORTED_GENERICS
+                 or rule[0] in self.JS_EXPORTED_VALUES
         ]
-        for field,value in to_register:
-            self.my_env.set_current_page_js_data(self.editor_name, field, value)
+        for field,value in actually_registered:
+            self.env.set_current_page_js_data(self.editor_name, field, value)
 
 
 
     #-----------------------------------------------------------------------------
 
 
     def __str__(self):
-        with_id = '' if self.id is None else f', ID={self.id}'
-        return f"IDE('{self.py_name}'{with_id}), in file {self.my_env.page.file.src_uri}"
+        return f"{self.__class__.__name__}('{self.py_name}', ...), in file {self.env.location()}"
+
+
+
+    def handle_extra_args(self):
+        """
+        Fill the extra arguments provided through other keyword arguments, handling only those
+        actually required for the child class. If some are remaining, after this in self.extra_kw,
+        an error will be raised.
+        Also extract default values for properties that are still set to None after handling the
+        keyword arguments.
+        """
+        to_transfer = [
+            data if isinstance(data,tuple) else (data,data.lower()) for data in self.KW_TO_TRANSFER
+        ]
+        for kw, prop in to_transfer:
+            if kw in self.extra_kw:
+                value = self.extra_kw.pop(kw)
+                setattr(self, prop, value)
+
+        if self.extra_kw:
+            raise BuildError(
+                f"Fund forbidden arguments for {self}:\n" + "".join(
+                    f"    {k} = {v!r}\n" for k,v in self.extra_kw.items()
+                )
+            )
+
+        self.get_default_if_none(self.DEFAULTS_EXTRACTION)
+
+
+
+    def get_default_if_none(self, props_to_options: Tuple[str,str]):
+        """ Extract the default values if the current property is set to None. """
+        for prop, option_prop in props_to_options:
+            if getattr(self, prop) is None:
+                default_value = getattr(self.env, option_prop)
+                setattr(self, prop, default_value)
+
 
 
     def _define_max_attempts_symbols_and_value(self):
         """
         Any MAX value defined in the file takes precedence, because it's not possible to know
         if the value coming from the macro is the default one or not.
         """
@@ -266,25 +380,25 @@
             max_ide = max_from_file
 
         is_inf = max_ide in ("+", "1000")     # 1000: legacy...
 
         # If ever there are neither correction nor remark, or if no tests, use also inf:
         is_inf = is_inf or not self.has_any_corr_rem or not self.has_secrets
 
-        self.max_attempts_symbol = self.INFINITY_SYMBOL if is_inf else str(max_ide)
+        self.max_attempts_symbol = IdeConstants.infinity_symbol if is_inf else str(max_ide)
 
         max_attempts = inf if is_inf else int(max_ide)
         return max_attempts
 
 
 
-    def _validate_config(self, max_attempts: Union[int,float]):
-        msg: Optional[Tuple[str,str]] = None
+    def _validate_files_config(self, max_attempts: Union[int,float] ):
+        msg = None,None
 
-        if (self.my_env.forbid_secrets_without_corr_or_REMs
+        if (not msg and self.env.forbid_secrets_without_corr_or_REMs
             and self.has_secrets and not self.has_any_corr_rem
         ):
             msg = (
                 "A `secrets` section exist but there are no `corr` section, REM or VIS_REM file.",
                 "forbid_secrets_without_corr_or_REMs"
             )
 
@@ -293,357 +407,167 @@
             "a REM file"     * (not self.has_rem),
             "a VIS_REM file" * (not self.has_vis_rem),
         ))]
         elt_msg = items_comma_joiner(elements, 'and')
         single  = len(elements)==1
         elt_msg = f"{ elt_msg } exist{ 's' * (single)}".capitalize()
 
-        if (self.my_env.forbid_hidden_corr_and_REMs_without_secrets
+        if (not msg and self.env.forbid_hidden_corr_and_REMs_without_secrets
             and self.has_any_corr_rem and not self.has_secrets
         ):
             msg = (
                 f"{ elt_msg }, but there is no `secrets` section.",
                 'forbid_hidden_corr_and_REMs_without_secrets'
             )
 
-        if (self.my_env.forbid_corr_and_REMs_with_infinite_attempts
+        if (not msg and self.env.forbid_corr_and_REMs_with_infinite_attempts
             and max_attempts==inf and self.has_any_corr_rem
         ):
             subject = "it" if single else "they"
             msg = (
                 f"{ elt_msg }, but {subject} will never be visible because the number of "
                 "attempts is set to infinity.",
                 'forbid_corr_and_REMs_with_infinite_attempts'
             )
 
-        if msg:
-            msg, opt = msg
-            msg = (
-                f"Invalid configuration\n    {self}:\n    {msg}\n    You can deactivate this "
-                f"check by setting plugins.pyodide_macros.build.{opt} to false in `mkdocs.yml`."
+        self._validation_outcome(*msg)
+
+
+
+    def _validation_outcome(self, msg:Optional[str], config_opt:Optional[str]=None):
+        if not msg:
+            return
+
+        msg = f"Invalid configuration with: {self}\n    {msg}"
+        if config_opt:
+            msg += (
+                "\n    You can deactivate this check by setting plugins.pyodide_macros."
+                f"build.{config_opt} to false in `mkdocs.yml`."
             )
-            if self.my_env._dev_mode:       # pylint: disable=protected-access
-                logger.error("DEV_MODE (expected x2) - " + msg)
-            else:
-                raise BuildError(msg)
+
+        if self.env._dev_mode:       # pylint: disable=protected-access
+            logger.error("DEV_MODE (expected x3) - " + msg)
+        else:
+            raise BuildError(msg)
 
 
 
     def _compute_exclusions_and_white_list(self, prop:str):
         """
         Convert a string argument (exclusions or white list) tot he equivalent list of data.
         """
         rule = (getattr(self, prop) or "").strip(' ;,')       # (never allow None)
         lst = re.split(r'[ ;,]+', rule) if rule else []
         return lst
 
 
 
-    def _generate_id_ide(self, py_path:Optional[Path]):
+    def generate_id(self):
         """
-        Generate an id number for the current IDE (editor+terminal), as a "prefix_hash(32bits)".
+        Generate an id number for the current element, in the form:
+
+            PREFIX_{32 bits hash value}
 
         This id must be:
             - Unique to every IDE used throughout the whole website.
             - Stable, so that it can be used to identify what IDE goes with what file or what
-              localeStorage data.
+              localStorage data.
 
         Current strategy:
             - If the file exists, hash its path.
             - If there is no file, use the current global IDE_counter and hash its value as string.
             - The "mode" of the IDE is appended to the string before hashing.
             - Any ID value (macro argument) is also appended to the string before hashing.
 
         Uniqueness of the resulting hash is verified and a BuildError is raised if two identical
         hashes are encountered.
+
+        NOTE: uniqueness most be guaranteed for IDEs (LocalStorage). It's less critical for other
+        elements, but they still need to stay unique across a page, at least (especially when
+        feedback is involved, like with terminals. Note: maybe not anymore... :thinking: )
         """
-        if py_path:
-            path = str(py_path)
-        else:
-            path = str(self.my_env.ide_count)
+        path = str(self.env.generic_count)
+        if self.id is not None:
+            path += str(self.id)            # kept in case unlucky collision... (yeah, proba... XD )
+        return self.id_to_hash(path)
 
-        if self.mode:
-            path += self.mode
 
-        if self.id is not None:
-            path += str(self.id)
 
-        id_ide = hashlib.sha1(path.encode("utf-8")).hexdigest()
+    def id_to_hash(self, clear:str):
+        """ Hash the hash to add as html id tail, prefix it, and check the uniqueness of the hash
+            across the whole website.
+        """
+
+        hashed  = hashlib.sha1(clear.encode("utf-8")).hexdigest()
+        html_id = f"{ self.ID_PREFIX }{ hashed }"
 
-        if not self.my_env.register_if_unique(id_ide):
+        if not self.env.register_if_unique(html_id):
             raise BuildError(
-                "The same editor ID got generated twice. If you are trying to use the same set"
-                "of files for different IDEs, use the ID argument to disambiguate their id.\n"
+                "The same html id got generated twice.\nIf you are trying to use the same set "
+                "of python files for different IDE-related elements, use their ID argument to "
+                "disambiguate their id.\n"
                f"  Problematic call:  { self }\n"
-               f"  Possible solution: add the ID:int keyword argument or change its value"
+               f"  Possible solution: add the ID:int keyword argument or change its current value"
             )
-        return id_ide
-
+        return html_id
 
 
 
     #-----------------------------------------------------------------------------
 
 
 
-
-    def make_ide(self) -> str:
+    def make_element(self) -> str:
         """
-        Create an IDE (Editor+Terminal) within an Mkdocs document. {py_name}.py is loaded on
-        the editor if present.
+        Create an IDE (Editor+Terminal) within an Mkdocs document. {py_name}.py is loaded
+        on the editor if present.
         NOTES:
             - Two modes are available : vertical or horizontal. Buttons are added through
                 functional calls.
             - The last span hides the code content of the IDE when loaded.
         """
-        # Mark the page as needing this kind of scripts in the body section:
-        self.my_env.set_current_page_insertion_needs(ScriptKind.pyodide)
-
-        ide_layout = self.generate_empty_ide()
-        buttons = self.generate_buttons_row()
-        global_layout = Html.div(
-            ide_layout+buttons,
-            id = f"{ Prefix.global_ }{ self.editor_name }",
-            kls = HtmlClass.py_mk_ide,
-        )
-        solution_div = self._build_corr_and_rem()
-
-        return global_layout + solution_div
-
-
-
-    def generate_empty_ide(self) -> str:
-        """
-        Generate the global layout that will receive later the ace elements.
-        """
-        is_v = self.mode == '_v'
-        toggle_txt = '###'
-        tip: Tip = self.my_env.lang.comments
-        msg = str(tip)
-
-        shortcut_comment_asserts = Html.span(
-            toggle_txt + Html.tooltip(msg, tip.em, shift=95),
-            id = Prefix.comment_ + self.editor_name,
-            kls = f'{HtmlClass.comment} {HtmlClass.tooltip}',
-        )
-        editor_div = Html.div(
-            id = self.editor_name,
-            is_v = str(is_v).lower(),
-            mode = self.mode,
-            max_size = self.max_size,
-            py_name = self.py_name,
-        )
-        editor_wrapper = Html.div(
-            editor_div + shortcut_comment_asserts,
-            kls = Prefix.comment_ + HtmlClass.py_mk_wrapper
-        )
-
-        separator = Html.div(
-            kls= HtmlClass.ide_separator + self.mode
-        )
-        terminal_div = Html.terminal(
-            Prefix.term_ + self.editor_name ,
-            kls = f"{ HtmlClass.term_editor }{ self.mode } { HtmlClass.py_mk_terminal }",
-            n_lines_h = self.term_height * (not is_v),
-            is_v = is_v,
-            env=self.my_env,
-        )
-
-        return Html.div(
-            f"{ editor_wrapper }{ separator }{ terminal_div }",
-            kls = f"{ HtmlClass.py_mk_wrapper }{ self.mode }",
-        )
-
-
-
-
-
-    def _build_corr_and_rem(self):
-        """
-        Build the correction and REM holders. The rendered template is something like the
-        following, with the indentation level of the most outer div equal to the indentation
-        level of the IDE macro text in the markdown file.
-        Depending on the presence/absence of corr, REM and VIS_REM files, some elements may
-        be missing. In this method:
-
-        | var | meaning |
-        |-|-|
-        | `at_least_one` | corr or REM (=> inside admonition) |
-        | `anything` | corr or REM or VIS_REM |
-
-        Overall structure of the generated markdown (mixed with html):
-
-                <div markdown="1" id="solution_editor_id"       <<< ALWAYS
-                     class="py_mk_hidden" >
-
-                ENCRYPTION_TOKEN                                <<< at least one and encryption ON
-
-                ??? tip "Solution"                              <<< at least one
-
-                    <div markdown="1" style="padding:1em">      <<< at least one
-
-                    ```python linenums="1"'                     <<< solution
-                    --8<-- "{ corr_uri }"                       <<< solution
-                    ```                                         <<< solution
-
-                    ___Remarques :___                           <<< remark & solution
-
-                    --8<-- "{ rem_uri }"                        <<< remark
-
-                    </div>                                      <<< at least one
-
-                --8<-- "{ vis_rem_uri }"                        <<< vis_rem
-
-                ENCRYPTION_TOKEN                                <<< at least one and encryption ON
-
-                </div>                                          <<< ALWAYS
-
-        Don't forget that empty lines are mandatory to render the "md in html" as expected.
-        """
-
-        # Prepare data first (to ease reading of the below sections)
-        sol_title = ' & '.join(filter(bool, [
-            str(self.my_env.lang.title_corr) * self.has_corr,
-            str(self.my_env.lang.title_rem) * self.has_rem
-        ]))
-        corr_content = self.files_data.corr_content
-        at_least_one = self.has_corr or self.has_rem
-        anything     = at_least_one or self.has_vis_rem
-        with_encrypt = self.my_env.encrypt_corrections_and_rems and anything
-        extra_tokens = ( self.my_env.ENCRYPTION_TOKEN, ) * with_encrypt
-
-
-        # Build the whole div content:
-        md_div = [         '',   # Extra empty line to enforce proper rendering of the md around
-                           f'<div markdown="1" id="{ Prefix.solution_ }{ self.editor_name }" '
-                           f'     class="{ HtmlClass.py_mk_hidden }" data-search-exclude >',
-                            *extra_tokens ]
-        if at_least_one:
-            md_div.append( f'??? tip "{ sol_title }"' )
-            md_div.append(  '    <div markdown="1" style="margin:1.7em 1em" >' )
-
-        if self.has_corr:
-            # first indentation must be removed, EXCEPT one level, because handled lower
-            # for the whole block
-            one_level = '    '
-            fence = build_code_fence(
-                corr_content,
-                one_level + self.indentation,
-                title=str(self.my_env.lang.corr)
-            )
-            md_div.append(  one_level+fence.strip())
-
-        if self.has_corr and self.has_rem:
-            rem = self.my_env.lang.rem
-            md_div.append( f'    <span class="{ HtmlClass.rem_fake_h3 }">{ rem } :</span>')
-
-        if self.has_rem:
-            rem = self._rem_inclusion('rem_rel_path')
-            md_div.append( f'    { rem }' )
-
-        if at_least_one:
-            md_div.append(  '    </div>')
-
-        if self.has_vis_rem:
-            vis_rem = self._rem_inclusion('vis_rem_rel_path')
-            md_div.append(  vis_rem )
-
-        md_div.extend((     *extra_tokens,
-                            '</div>\n',    ))
-                # The extra linefeed is there to enforce md rendering of the following sections
-
-        # Add extra indentation according to IDE's insertion:
-        if self.indentation:
-            md_div = [ s and self.indentation + s for s in md_div ]
-
-        # Join every item with extra gaps, to following md rendering requirements
-        out = '\n\n'.join(md_div)
-        return out
-
-
-    def _rem_inclusion(self, rem_path_kind:str):
-        path_str = str(getattr(self.files_data, rem_path_kind))
-        rem_uri  = to_uri( convert_url_to_utf8(path_str) )
-        return f'--8<-- "{ rem_uri }"'
-
-
-
-    def generate_buttons_row(self) -> str:
-        """
-        Build all buttons below an "ide" (editor+terminal).
-        """
-        cnt_txt, cnt_or_inf = self.my_env.lang.attempts_left.msg, self.max_attempts_symbol
-        cnt_txt_span = Html.span(cnt_txt + " : ", kls=HtmlClass.compteur_txt)
-        cnt_n_span = Html.span(cnt_or_inf, id=f'{ Prefix.compteur_ }{ self.editor_name }')
-
-        buttons = [
-            self.create_button("play"),
-            self.create_button("check", btn_kind="validate") if self.has_secrets else "",
-            self.create_button("download", margin_left=1 ),
-            self.create_upload_button(margin_right=1),
-            self.create_button("restart"),
-            self.create_button("save"),
-            Html.span(f"{ cnt_txt_span }{ cnt_n_span }/{ cnt_or_inf }", kls=HtmlClass.compteur),
-        ]
-        buttons_div = Html.div( ''.join(buttons), kls=HtmlClass.ide_buttons_div )
-        return buttons_div
+        raise NotImplementedError("Subclasses should implement the make_element method.")
 
 
 
     def create_button(
-        self, button_name: str,
+        self,
+        button_name:    str,
         *,
-        btn_kind:str=None,
-        margin_left:float=0.2, margin_right:float=0.2,
-        extra_content:str = "",
+        btn_kind:       str   = None,
+        margin_left:    float = 0.2,
+        margin_right:   float = 0.2,
+        extra_content:  str   = "",
         **kwargs
     ) -> str:
         """
         Build one button, given its name.
 
-        @btn_kind:      The name of the JS function to bind the button click event to. If not
-                        given, use the lowercase version of button_name.
-        @margin_...:    CSS formatting as floats (em units). By default, 0.2 on each side.
+        @btn_kind:      The name of the JS function to bind the button click event to.
+                        If none given, use the lowercase version of @button_name.
+        @margin_...:    CSS formatting as floats (default: 0.2em on each side).
         @extra_content: Allow to inject some additional html inside the button tag.
         @**kwargs:      All the remaining kwargs are attributes added to the button tag.
         """
         if btn_kind is None:
             btn_kind = button_name.lower()
 
-        tip: Tip     = getattr(self.my_env.lang, button_name)
-        span_tooltip = Html.tooltip(tip, tip.em)
-        lvl_up       = self.my_env.level_up_from_current_page()
-        img_link     = self.ICON_TEMPLATE.format(lvl_up=lvl_up, button_name=button_name)
-        img          = Html.img(src=img_link, kls=HtmlClass.skip_light_box)
-        button_html  = Html.button(
-            f'{ img }{ span_tooltip }{ extra_content }',
-            kls = HtmlClass.tooltip,
+        style = f"margin-left:{margin_left}em; margin-right:{margin_right}em;"
+        if 'style' in kwargs:
+            style += kwargs.pop('style')
+
+        tip: Tip = getattr(self.env.lang, button_name)
+        tip_span = Html.tooltip(tip, tip.em)
+        lvl_up   = self.env.level_up_from_current_page()
+        img_link = get_ide_button_png_path(lvl_up,button_name)
+        img      = Html.img(src=img_link, kls=HtmlClass.skip_light_box)
+
+        button_html = Html.button(
+            f'{ img }{ tip_span }{ extra_content }',
             btn_kind = btn_kind,
-            style = f"margin-left:{margin_left}em; margin-right:{margin_right}em;",
-            **kwargs,
-            type='button',
+            kls = HtmlClass.tooltip,
+            style = style,
+            type = 'button',
                 # https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button#notes
+            **kwargs,
         )
         return button_html
-
-
-
-    def create_upload_button(self, margin_right:float = 1) -> str:
-        """
-        @brief : Create upload button for an IDE number {id_ide}.
-        @details : Use an HTML input to upload a file from user. The user clicks on the button to
-        fire a JS event that triggers the hidden input.
-        """
-
-        input_button_controller = Html.input(
-            id = f"{ Prefix.input_ }{ self.editor_name }",
-            kls = HtmlClass.py_mk_hidden,
-            type = 'file',
-            name = 'file',
-            enctype = "multipart/form-data",
-        )
-        button = self.create_button(
-            "upload",
-            margin_right = margin_right,
-            extra_content = input_button_controller,
-        )
-        return button
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 from pathlib import Path
 from dataclasses import dataclass
 import subprocess
 from typing import ClassVar, Dict, Optional, Union
 
 from mkdocs.exceptions import BuildError
 
-from ...plugin.maestro_IDE import MaestroIDE
-from ...paths_utils import (
+from ..plugin.maestro_IDE import MaestroIDE
+from ..paths_utils import (
     get_sibling_of_current_page,
     read_file,
 )
-from ...pyodide_logger import logger
-from ...tools_and_constants import ScriptSection, SiblingFile
+from ..pyodide_logger import logger
+from ..tools_and_constants import ScriptSection, SiblingFile
 
 
 
 
 CWD = Path.cwd()
 
 
@@ -54,38 +54,38 @@
 
         1.  {X}.py
             {X}_REM.md
             {X}_VIS_REM.md
             Where the py file contains all the needed python code/sections, separated by the
             pyodide python tokens: `# --- PYODIDE:{kind} --- #`
 
-        2. {X}.py
-           {X}_text.py
-           {X}_corr.py
-           {X}_REM.md
+        2.  {X}.py
+            {X}_text.py
+            {X}_corr.py
+            {X}_REM.md
             {X}_VIS_REM.md
 
-        3. scripts/{F}/{X}.py
-           scripts/{F}/{X}_REM.md
-           scripts/{F}/{X}_VIS_REM.md
-           Where the py file contains all the needed python code/sections, separated by the
-           pyodide python tokens: `# --- PYODIDE:{kind} --- #`
-
-        4. scripts/{F}/{X}.py
-           scripts/{F}/{X}_test.py
-           scripts/{F}/{X}_corr.py
-           scripts/{F}/{X}_REM.md
-           scripts/{F}/{X}_VIS_REM.md
+        3.  scripts/{F}/{X}.py
+            scripts/{F}/{X}_REM.md
+            scripts/{F}/{X}_VIS_REM.md
+            Where the py file contains all the needed python code/sections, separated by the
+            pyodide python tokens: `# --- PYODIDE:{kind} --- #`
+
+        4.  scripts/{F}/{X}.py
+            scripts/{F}/{X}_test.py
+            scripts/{F}/{X}_corr.py
+            scripts/{F}/{X}_REM.md
+            scripts/{F}/{X}_VIS_REM.md
 
     The order gives the precedence. Way "1" is excluding the 2 others (except for the REM file)
     """
 
     env: MaestroIDE
     py_name: str
-    id: Optional[int] = None
+    # id: Optional[int] = None
 
     #-----------------------------
 
     exo_py: Optional[Path] = None
     """ Path to the master python file (if any) """
 
     file_max_attempts: Union[int, str] = ""
@@ -100,15 +100,15 @@
     rem_rel_path: Optional[Path] = None
     """ Relative path to the ...REM.md file (or None if no file) """
 
     vis_rem_rel_path: Optional[Path] = None
     """ Relative path to the ..._VIS_REM.md file (or None if no file) """
 
 
-    corr_rem_bit_mask: int = 0
+    corr_rems_bit_mask: int = 0
     """ Bit mask giving the configuration for correction and/or remark data
         mask&1 represent the presence of correction, mask&2 is for REM.
     """
 
     env_content: str = ""
     """ Python header code content (run async) """
 
@@ -152,20 +152,32 @@
         ScriptSection.tests:   "public_tests",
         ScriptSection.secrets: "secret_tests",
         ScriptSection.post:    "post_content",
     }
 
 
     @property
+    def has_env(self):
+        return bool(self.env_content)
+    @property
+    def has_code(self):
+        return bool(self.user_content)
+    @property
     def has_corr(self):
         return bool(self.corr_content)
     @property
+    def has_tests(self):
+        return bool(self.public_tests)
+    @property
     def has_secrets(self):
         return bool(self.secret_tests)
     @property
+    def has_post(self):
+        return bool(self.post_content)
+    @property
     def has_rem(self):
         return bool(self.rem_rel_path)
     @property
     def has_vis_rem(self):
         return bool(self.vis_rem_rel_path)
 
 
@@ -173,26 +185,27 @@
 
 
     def __post_init__(self):
 
         self.exo_py: Optional[Path] = get_sibling_of_current_page(self.env, self.py_name, tail='.py')
         if not self.exo_py and self.py_name:
             raise BuildError(
-                f"No python script for { self.py_name }, in { self.env.page.file.src_uri }"
+                f"No python file could be found for py_name='{ self.py_name }', "
+                f"in { self.env.location() }"
             )
 
         script_content = read_file(self.exo_py) if self.exo_py  else ""
 
         # Extract everything:
         if self.SECTION_TOKEN.search(script_content):
             self.extract_multi_sections(script_content)
         else:
             self.extract_multi_files(script_content)
 
-        self.corr_rem_bit_mask = self.has_corr + self.has_rem * 2
+        self.corr_rems_bit_mask = self.has_corr + (self.has_rem or self.has_vis_rem) * 2
 
         # if not self.skip_check and self.env.check_python_files:
         #     self.check_python()
 
         # self._fuuuuuusion()
         # self._cleanup_tests()
 
@@ -244,28 +257,36 @@
 
         chunks = self.SECTION_TOKEN.split(script_content)
         chunks = [*filter(bool, map(str.strip, chunks))]
         pairs  = [*zip(*[iter(chunks)]*2)]
 
 
         # File structure validations:
-        headers = [ self._extract_section_name(section) for section in chunks
-                                                     if self.SECTION_TOKEN.match(section) ]
+        headers = [ self._extract_section_name(section)
+                        for section in chunks if self.SECTION_TOKEN.match(section) ]
         odds_sections = len(chunks) & 1
-        duplicates    = len(headers) != len(set(headers))
         wrong_tic_toc = len(headers) != sum(
             bool(self.SECTION_TOKEN.match(header)) for header,_ in pairs
         )
-        if odds_sections or duplicates or wrong_tic_toc:
-            raise BuildError(f"Invalid file structure for { self.exo_py }")
-
+        if odds_sections or wrong_tic_toc:
+            raise BuildError(
+                f"Invalid file structure for { self.exo_py }: no empty sections allowed."
+            )
+        no_ignores_headers = [ h for h in headers if h != ScriptSection.ignore ]
+        if len(no_ignores_headers) != len(set(no_ignores_headers)):
+            raise BuildError(
+                f"Invalid file structure for { self.exo_py }: Duplicate sections are not "
+                "allowed (except for the `ignore` section)."
+            )
 
         # Codes registrations:
         for section,content in pairs:
             section_name = self._extract_section_name(section)
+            if section_name == ScriptSection.ignore:
+                continue
             prop = self._get_section_property(section_name)
             setattr(self, prop, content)
 
         self.rem_rel_path, _     = self.get_path_and_existence(SiblingFile.rem)
         self.vis_rem_rel_path, _ = self.get_path_and_existence(SiblingFile.vis_rem)
 
 
@@ -280,15 +301,16 @@
         prop = self._get_section_property(section)
         return  getattr(self, prop)
 
 
     def _get_section_property(self, section:ScriptSection):
         if section not in self.SECTION_TO_PROP:
             raise BuildError(f'Unknown section name {section!r} in { self.exo_py }')
-        return self.SECTION_TO_PROP[section]
+        else:
+            return self.SECTION_TO_PROP[section]
 
 
 
 
     #--------------------------------------------------------------------------
     #                            OLD FASHION WAY
     #--------------------------------------------------------------------------
@@ -338,15 +360,15 @@
 
     def check_python(self):
         """
         * hdr + corr + public + secret => pass
         * hdr + user + public => doesn't pass
         * hdr + user + secret => doesn't pass
         """
-        raise ValueError("The build.check_python_files option has been disabled.")
+        raise ValueError("The plugin option `build.check_python_files` has been disabled.")
         if not self.py_name: # or self.id is not None:
             # skip: nothing to check
             return
 
         src    = get_sibling_of_current_page(self.env, self.py_name, tail='.py')
         target = Path('___XXX_check_python.py')
         target.touch(exist_ok=True)
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,59 +16,50 @@
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 # pylint: disable=unused-argument
 
 
 import re
-from pathlib import Path
 from functools import wraps
 
 
-from .. import html_builder as Html
 from ..plugin.maestro_IDE import MaestroIDE
 from ..parsing import build_code_fence
 from ..paths_utils import get_sibling_of_current_page
-from ..tools_and_constants import HtmlClass, Prefix, ScriptKind
 
 
 
 
 
 def script(
     env: MaestroIDE,
-    macro: str,
     nom: str,
     *,
     lang: str='python',
     stop= None,
-    ID: int=None
 ) -> str:
     """
     Renvoie le script dans une balise bloc avec langage spécifié
 
-    - macro: permet de retrouver le niveau d'indentation de l'appel de macro
     - lang: le nom du lexer pour la coloration syntaxique
     - nom: le chemin du script relativement au .md d'appel
     - stop: si ce motif est rencontré, il n'est pas affichée, ni la suite.
     """
     target = get_sibling_of_current_page(env, nom, tail='.py')
     _,content,public_tests = env.get_hdr_and_public_contents_from(target)
 
     # Split again if another token is provided
     if stop is not None:
         # rebuild "original" if another token is provided
         if public_tests:
             content = f"{ content }{ env.lang.tests.msg }{ public_tests }"
         content = re.split(stop, content)[0]
 
-    id_pattern = "" if ID is None else rf".*?,\s*ID\s*=\s*{ ID }"
-    macro_pattern = f"""['"]{ nom }['"]"""
-    ide_jinja_reg = re.compile( rf"{ macro }\(\s*{ macro_pattern }{ id_pattern }" )
-    indent = env.get_indent_in_current_page(ide_jinja_reg)
+    indent = env.get_macro_indent()
     out = build_code_fence(content, indent, lang=lang)
     return out
 
 
 
 def py(env:MaestroIDE):
     """
@@ -76,45 +67,10 @@
     automatiquement supprimées, de même que les tests publics. Si un argument @stop est
     fourni, ce dot être une chaîne de caractère compatible avec re.split, SANS matching groups.
     Tout contenu après ce token sera ignoré (token compris) et "strippé".
 
     ATTENTION: Ne marche pas sur les exercices avec tous les codes python dans le même fichier.
     """
     @wraps(py)
-    def wrapped(nom: str, stop=None, ID:int=None) -> str:
-        return script(env, 'py', nom, stop=stop, ID=ID)
-    return wrapped
-
-
-# def py_sujet(env:MaestroIDE):
-#     """
-#     Macro python rapide, pour un sujet sans les tests => code formaté seulement, non modifiable.
-
-#     ATTENTION: Ne marche pas sur les exercices avec tous les codes python dans le même fichier.
-#     """
-#     @wraps(py_sujet)
-#     def wrapped(nom: str, stop=None, ID:int=None) -> str:
-#         return script(env, 'py_sujet', nom, stop=stop, ID=ID)
-#     return wrapped
-
-
-
-
-
-
-def terminal(env:MaestroIDE):
-    """
-    Create a Python Terminal.
-    @SIZE(=6): number of lines (height) of the terminal
-    """
-
-    @wraps(terminal)
-    def wrapped(SIZE:int=6) -> str:
-
-        env.set_current_page_insertion_needs(ScriptKind.pyodide)
-
-        term_id = f'{ Prefix.term_only_ }{ env.terminal_count }'
-        classes = " ".join((HtmlClass.py_mk_terminal_solo, HtmlClass.py_mk_terminal))
-        div     = Html.terminal(term_id, kls=classes, n_lines_h=SIZE, env=env)
-        return div
-
+    def wrapped(nom: str, stop=None, **_) -> str:
+        return script(env, nom, stop=stop)
     return wrapped
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 import re
 from functools import wraps
 from textwrap import dedent
 from typing import Any, List, Optional
 
 from mkdocs.exceptions import BuildError
 
+
 from ..plugin.maestro_extras import MaestroExtras
 from ..paths_utils import get_sibling_of_current_page
-from ..tools_and_constants import HtmlClass
+from ..tools_and_constants import HtmlClass, ScriptKind
 
 
 
 
 
 
 
@@ -62,29 +63,28 @@
     @shuffle=False:   Questions and their items are shuffled on each refresh/retry
     @hide=False:      Correct answers will stay hidden if True after checking the user's answers
     @multi=None:      Set the default behavior for unique correct answers, at qcm level.
     @admo_kind="!!!": Control the kind of admonition used for the QCM
     @admo_type='tip': Category of admonition to use
     @qcm_title=None:  Title for the admonition. If not given "Question" (possibly plural) is used.
 
-    @ID:int=None:     To disambiguate GCMs macro calls if needed
     @DEBUG=False:     If True, md output will be printed to the console
     """
 
     @wraps(multi_qcm)
     def wrapped(
         *inputs,
         shuffle:    Optional[bool]=None,
         hide:       Optional[bool]=None,
         multi:      Optional[bool]=None,
         admo_kind:  str="!!!",
         admo_class: str="tip",
         qcm_title:  Optional[str]=None,
-        ID:         Optional[int]=None,
         DEBUG:      bool=False,
+        ID=None,                        # sink (deprecated)
     ):
         """
         WARNING:    extra closing </p> tags needed here and there to guarantee the
                     final html structure!
 
         Reasons:
         1. THE MD RENDERER GENERATES INVALID HTML, WHEN MIXING html+md PERIOD!
@@ -96,14 +96,17 @@
             depending on the html parser used, Beautif(o)ulSoup _WILL_ generate the missing
             closing tags, and this will entirely mess up the rendered page.
 
         So, to avoid this, the extra closing `</p>` are added. They _LOOK_ like they are hanging,
         but they _will_ actually produce valid html!
         """
 
+        env.set_current_page_insertion_needs(ScriptKind.qcm)
+
+
         def qcm_start():
             qcm_id = env.get_qcm_id()
 
             admo_classes = ' '.join(kls for kls in [
                 HtmlClass.py_mk_admonition_qcm,
                 HtmlClass.qcm_shuffle * shuffle,
                 HtmlClass.qcm_hidden * hide,
@@ -190,17 +193,15 @@
                 [*map(qcm_format,items)],
                 ans,
                 dct[0] if dct else {}
             ]
             for q,items,ans,*dct in inputs
         ]
 
-        id_pattern = "" if ID is None else rf".*?,\s*ID\s*=\s*{ ID }\b\s*"
-        call_pattern = re.compile(rf"multi_qcm[(]{ id_pattern }")
-        indent = env.get_indent_in_current_page(call_pattern)
+        indent = env.get_macro_indent()
         auto_indent = auto_indenter_factory(indent)
 
         if hide is None:    hide    = env.hide
         if multi is None:   multi   = env.multi
         if shuffle is None: shuffle = env.shuffle
 
         admonition_lst = qcm_start()
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
 @dataclass
 class Tip(JsDumper):
     """
     Data for tooltips.
 
     Parameters:
-        em:     Width of the tooltip element, in em units.
+        em:     Width of the tooltip element, in em units (if 0, use automatic width).
         msg:    Tooltip message.
         kbd:    Keyboard shortcut (as "Ctrl+I", for example). Informational only (no
                 impact on the behaviors)
 
     If a `kbd` combination is present, it will be automatically added in a new line
     after the tooltip `msg`.
     """
@@ -201,83 +201,89 @@
 
 
 class Lang(Namespace):
     # pylint: disable=no-member
 
     # LANG_TOKEN
     # Editors:
-    comments:   Tr = Tip(15, "(Dés-)Active le code après la ligne <code>{tests}</code> "
-                             "(insensible à la casse)", "Ctrl+I")    ###
-    """
-    Info-bulle pour le bouton permettant d'activer ou désactiver les tests publics.
-    La chaîne utilisée doit contenir `{tests}` car le contenu de TestsToken.msg y sera inséré.
-    """###
     tests:      Tr = TestsToken("\n# Tests\n")  ###
     """
     Séparateur placé entre le code utilisateur et les tests publics.
 
     * Les sauts de lignes situés au début ou à la fin indiquent le nombre de lignes vides avant
     ou après le texte lui-même.
     * Le séparateur lui-même doit commencer par `#` et avoir au moins 6 caractères (hors espaces).
     """###
+    comments:   Tr = Tip(15, "(Dés-)Active le code après la ligne <code>{tests}</code> "
+                             "(insensible à la casse)", "Ctrl+I")    ###
+    """
+    Info-bulle pour le bouton permettant d'activer ou désactiver les tests publics.
+    La chaîne utilisée doit contenir `{tests}` car le contenu de TestsToken.msg y sera inséré.
+    """###
 
 
     # Terminals
-    run_script:    Tr = Msg("Script lancé...")    ###
+    feedback:      Tr = Tip(15, "Tronquer ou non le feedback dans les terminaux (sortie standard"
+                                " & stacktrace / relancer le code pour appliquer)")    ###
     """
-    Message annonçant le début des executions (pyodide).
+    Info-bulle du bouton contrôlant le "niveau de feedback" affiché dans le terminal
     """###
-    success_msg:   Tr = Msg("Terminé sans erreur !")    ###
+    wrap_term:     Tr = Tip(15, "Si activé, le texte copié dans le terminal est joint sur une "
+                                "seule ligne avant d'être copié dans le presse-papier")    ###
     """
-    Message affiché à la fin des tests publics, si aucune erreur n'a été rencontrée.
+    Info-bulle du bouton Indiquant si le texte copié depuis le terminal est join anat d'être copié ou non.
+    """###
+    run_script:    Tr = Msg("Script lancé...")    ###
+    """
+    Message annonçant le début des executions (pyodide).
     """###
     install_start: Tr = Msg("Installation de paquets python. Ceci peut prendre un certain temps...")    ###
     """
     Message affiché dans la console avant le chargement de micropip, en vue d'installer des modules manquants.
     """###
     install_done:  Tr = Msg("Installations terminées!")    ###
     """
     Message affiché lorsque les installation de paquets par micropip sont finies.
     """###
-    feedback:      Tr = Tip(15, "Tronquer ou non le feedback dans les terminaux (sortie standard"
-                                " & stacktrace / relancer le code pour appliquer)")    ###
+    success_msg:   Tr = Msg("Terminé sans erreur !")    ###
     """
-    Info-bulle du bouton contrôlant le "niveau de feedback" affiché dans le terminal
+    Message affiché à la fin des tests publics, si aucune erreur n'a été rencontrée.
     """###
 
+
     # Terminals: validation success/failure messages
     success_head:  Tr = Msg("Bravo !")    ###
     """
     Entête du message de succès (gras, italique, en vert)
     """###
-    success_head_extra:  Tr = Msg("Vous avez réussi tous les tests !")    ###
+    success_tail:  Tr = Msg("Pensez à lire")    ###
     """
-    Fin du message annonçant un succès.
+    Fin du message de succès.
     """###
     fail_head:     Tr = Msg("Dommage !")    ###
     """
     Entête du message d'échec (gras, italique, en orange)
     """###
-    success_tail:  Tr = Msg("Pensez à lire")    ###
-    """
-    Fin du message de succès.
-    """###
     reveal_corr:   Tr = Msg("le corrigé")    ###
     """
     Bout de phrase annonçant l'existence d'une correction.
     """###
     reveal_join:   Tr = Msg("et")    ###
     """
     Conjonction de coordination joignant reveal_corr et reveal_rem, quand correction et
     remarques sont présentes.
     """###
     reveal_rem:    Tr = Msg("les commentaires")    ###
     """
     Bout de phrase annonçant l'existence de remarques.
     """###
+    success_head_extra:  Tr = Msg("Vous avez réussi tous les tests !")    ###
+    """
+    Fin du message annonçant un succès.
+    """###
     fail_tail:     Tr = MsgPlural("est maintenant disponible", "sont maintenant disponibles") ###
     """
     Fin du message annonçant un échec.
     """###
 
 
     # Corr  rems admonition:
@@ -299,15 +305,19 @@
     rem:        Tr = Msg('Remarques')    ###
     """
     Titre (équivalent &lt;h3&gt;) annonçant le début des remarques, dans l'admonition "correction &
     remarques"
     """###
 
 
-    # IDEs buttons & counter:
+    # Buttons, IDEs buttons & counter:
+    py_btn: Tr = Tip(9, "Exécuter le code")    ###
+    """
+    Info-bulle d'un bouton isolé, permettant de lancer un code python.
+    """###
     play:       Tr = Tip(9,  "Exécuter le code", "Ctrl+S")    ###
     """
     Info-bulle du bouton pour lancer les tests publics.
     """###
     check:      Tr = Tip(9,  "Valider", "Ctrl+Enter")    ###
     """
     Info-bulle du bouton pour lancer les tests privés.
@@ -322,23 +332,24 @@
     """###
     restart:    Tr = Tip(0,  "Réinitialiser l'éditeur")    ###
     """
     Info-bulle du bouton réinitialisant le contenu d'un éditeur.
     """###
     save:       Tr = Tip(0,  "Sauvegarder dans le navigateur")    ###
     """
-    Info-bulle du bouton pour enregistrer le contenu d'un éditeur dans le LocaleStorage du
+    Info-bulle du bouton pour enregistrer le contenu d'un éditeur dans le localStorage du
     navigateur.
     """###
     attempts_left: Tr = Msg("Évaluations restantes")    ###
     """
-    Info-bulle du bouton pour enregistrer le contenu d'un éditeur dans le LocaleStorage du
+    Info-bulle du bouton pour enregistrer le contenu d'un éditeur dans le localStorage du
     navigateur.
     """###
 
+
     # QCMS
     qcm_title:     Tr = MsgPlural("Question")    ###
     """
     Titre utilisé par défaut pour les admonitions contenant les qcms (si pas d'argument renseigné
     dans l'appel de la macro `multi_qcm`).
     """###
     qcm_mask_tip:  Tr = Tip(15, "Les réponses resteront cachées...")    ###
@@ -350,14 +361,15 @@
     Info-bulle du bouton de validation des réponses des qcms.
     """###
     qcm_redo_tip:  Tr = Tip(9,  "Recommencer")    ###
     """
     Info-bulle du bouton de réinitialisation des qcms.
     """###
 
+
     # Others
     tip_trash: Tr = Tip(15, "Supprimer du navigateur les codes enregistrés pour {site_name}") ###
     """
     Info-bulle du bouton de pour supprimer les données stockées dans le navigateur
     (la poubelle en haut à côté de la barre de recherche).
     Le nom du site (`site_name` dans `mkdocs.yml`) est automatiquement intégré dans la phrase
     avec "{site_name}".
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,104 +16,94 @@
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 # pylint: disable=multiple-statements
 
 
 import json
-from typing import Any, Dict, List, Literal, Set, Tuple, Type, TYPE_CHECKING
+from typing import Any, Dict, List, Set, Tuple, Type, TYPE_CHECKING
+from itertools import starmap
 from dataclasses import dataclass
 from math import inf
 
 
-from .tools_and_constants import EditorName, ScriptKind
+
+from .tools_and_constants import KIND_ORDER, EditorName, ScriptKind
 from .pyodide_logger import logger
+from .parsing import compress_LZW
 from . import html_builder as Html
 
 if TYPE_CHECKING:
     from .plugin.pyodide_macros_plugin import PyodideMacrosPlugin
 
 
 
 
-
-
-# Automatically updated from IdeConfig code, through build_tools:
-IdeConfigKey = Literal[
-    'attempts_left',
-    'auto_log_assert',
-    'corr_content',
-    'corr_rem_config',
-    'encrypted',
-    'env_content',
-    'excluded',
-    'excluded_methods',
-    'post_content',
-    'public_tests',
-    'rec_limit',
-    'secret_tests',
-    'user_content',
-    'white_list',
-]
-
 MAYBE_LISTS: Tuple[str,...] = ('excluded', 'excluded_methods', 'white_list')
 
 
 @dataclass
 class IdeConfig:
     """
     Configuration of one IDE in one page of the documentation. Convertible to JS, to define the
     global variable specific to each page.
+
+    Always instantiated without arguments, and items are updated when needed.
     """
 
-    # BUILD_TOOL_TOKEN
-    attempts_left: int = 0      # Not overwriting this means there is no counter displayed
-    auto_log_assert: bool=None  # If None, use the global setting, CONFIG.showAssertionCodeOnFailedTest
-    env_content: str = ""       # HDR part of "exo.py"
-    user_content: str = ""      # Non-HDR part of "exo.py" (initial code)
-    corr_content: str = ""      # content of "exo_corr.py"
-    public_tests: str = ""      # test part of "exo.py" (initial code)
-    secret_tests: str = ""      # Content of "exo_test.py" (private tests)
-    post_content: str = ""      # Content to run after executions are done
-    corr_rem_config: int = 0    # Bit mask:   has_corr=corr_rem_config&1 ; has_rem=corr_rem_config&2
-    encrypted: bool = True      # Tells if the html content is still encrypted or not
-    rec_limit: int = -1         # recursion depth to use at runtime, if defined (-1 otherwise).
-    excluded: List[str]=None    # List of forbidden instructions (functions or packages)
-    excluded_methods: List[str]=None # List of forbidden methods accesses
-    white_list: List[str]=None  # White list of packages to preload at runtime
-    # BUILD_TOOL_TOKEN
+    py_name:      str = ""          # name to use for downloaded file
+    env_content:  str = ""          # HDR part of "exo.py"
+    user_content: str = ""          # Non-HDR part of "exo.py" (initial code)
+    #corr_content: str = ""         # not exported to JS!
+    public_tests: str = ""          # test part of "exo.py" (initial code)
+    secret_tests: str = ""          # Content of "exo_test.py" (private tests)
+    post_content: str = ""          # Content to run after executions are done
+
+    excluded: List[str] = None      # List of forbidden instructions (functions or packages)
+    excluded_methods: List[str] = None # List of forbidden methods accesses
+    rec_limit: int = None           # recursion depth to use at runtime, if defined (-1 otherwise).
+    white_list: List[str] = None    # White list of packages to preload at runtime
+
+    attempts_left: int = None       # Not overwriting this means there is no counter displayed
+    auto_log_assert: bool = None    # If None, use the global setting, CONFIG.showAssertionCodeOnFailedTest
+    corr_rems_mask: int = None      # Bit mask:   has_corr=corr_rems_mask&1 ; has_rem=corr_rems_mask&2
+    has_check_btn: bool = None      # Store the info about the Ide having its check button visible or not
+
+    prefill_term: str = None        # Command to insert in the terminal after it's startup.
 
 
 
     def dump_to_js_code(self):
         """
         Convert the current config to a valid string representation of a JS object.
         """
         content = ', '.join(
-            f'"{k}": { self._convert(k, typ) }'
-            for k,typ in self.__class__.__annotations__.items()     # pylint: disable=no-member
-            if k!='corr_content'        # corr_content is not exported to JS env!
+            f'"{k}": { typ }'                  # pylint: disable-next=no-member
+            for k,typ in starmap(self._convert, self.__class__.__annotations__.items())
+            if typ is not None      # This filtering operation
         )
         return f"{ '{' }{ content }{ '}' }"
 
 
     def _convert(self, prop:str, typ:Type):
         """
         Convert the current python value to the equivalent "code representation" for a JS file.
         @prop: property name to convert
         @typ: type (annotation) of the property
         @returns: str
         """
         val = getattr(self, prop)
-        is_lst = prop in MAYBE_LISTS
+        if val is None:
+            return prop, None
 
-        if is_lst:           return json.dumps(val or [])
-        if val == inf:       return "Infinity"
-        if typ is bool:      return str(val).lower() if val is not None else "null"
-        if typ in (int,str): return repr(val)
+        is_lst = prop in MAYBE_LISTS
+        if is_lst:           return prop, json.dumps(val or [])
+        if val == inf:       return prop, '"Infinity"'
+        if typ is bool:      return prop, str(val).lower() if val is not None else "null"
+        if typ in (int,str): return prop, json.dumps(val)
 
         raise NotImplementedError(
             f"Conversion for {prop}:{typ} in {self.__class__.__name__} is not implemented"
         )
 
 
 
@@ -146,39 +136,37 @@
 
         @going_up:          Relative path string allowing to retrieve the root level of the docs.
         @kind_to_scripts:   Relations between kinds and the scripts the involve.
         @chunks:            List of slices of the current page. The insertions must be added to it.
         """
 
         # Yield the global variable first, because the JS scripts will use it at runtime:
-        global_var = 'var PAGE_IDES_CONFIG = {' + ', '.join(
+
+        global_var = '{' + ', '.join(
             f'"{ editor_name }": { conf.dump_to_js_code() }' for editor_name,conf in self.items()
         )+'}'
-        chunks.append(Html.script(global_var))
-
-        # store kinds that are desired by a page, but for which there is nothing to insert
-        missed = set()
-
-        # Then yield all the scripts and/or css the current page is needing:
-        for kind in self.needs:
-            if kind in kind_to_scripts:
-                insertion = kind_to_scripts[kind].format(to_base=going_up)
-                chunks.append(insertion)
-            else:
-                missed.add(kind)
+        encoded = compress_LZW(global_var)
+        chunks.append(Html.script(f"let PAGE_IDES_CONFIG = { encoded !r}"))
 
+        # Spot invalid kinds:
+        missed = {kind for kind in self.needs if kind not in kind_to_scripts}
         if missed:
             logger.error(
                 "Some macros are registering the need for these kinds while there are no files "
               + "registered for them:"
               + ''.join(f"\n    { ScriptKind.__name__ }.{ k }" for k in missed)
             )
 
+        # Then register all the scripts and/or css the current page is needing:
+        for kind in sorted(self.needs, key=KIND_ORDER.__getitem__):
+            insertion = kind_to_scripts[kind].format(to_base=going_up)
+            chunks.append(insertion)
+
 
-    def set(self, editor_name:str, prop:IdeConfigKey, value:Any):
+    def set(self, editor_name:str, prop:str, value:Any):
         """ Register an IDE configuration property, creating the IdeConfig on the fly,
             if it doesn't exist yet.
         """
         if self.env._dev_mode and prop not in IdeConfig.__annotations__:    # pylint: disable=no-member, protected-access
             msg = f'{prop!r} is not a valide attribut of { IdeConfig.__name__ } class'
             raise AttributeError(msg)
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,23 @@
 """
 
 
 from urllib.parse import unquote
 from pathlib import Path
 from typing import Optional, Union
 
+from pyodide_mkdocs_theme.pyodide_macros.tools_and_constants import IdeConstants
+
+
 from .plugin.maestro_base import BaseMaestro
 
 
 
 
+
 PathOrStr = Union[str,Path]
 
 
 
 
 def to_uri(path:Union[Path,str], *segments:str):
     """ Take a path string, potentially os dependent, and rebuild a slash separated
@@ -92,24 +96,26 @@
         If @tail is given, it is added to the name of the built path.
         Return None if:
             - @src has no explicit parent (using '.' on the cwd will cause troubles)
             - @rel is an empty string or is a Path without name property (empty IDE)
     """
     if not src.name or not rel or isinstance(rel,Path) and not rel.name:
         return None
-    path: Path = src.parent / rel
-    if tail:
-        path = path.with_name( path.stem + tail )
 
-    if not path.is_file():
-        path = src.parent / 'scripts' / src.stem / rel
+    possible_paths = [
+        src.parent / rel,
+        src.parent / 'scripts' / src.stem / rel
+    ]
+    for path in possible_paths:
         if tail:
             path = path.with_name( path.stem + tail )
+        if path.is_file():
+            return path
 
-    return path
+    return None
 
 
 
 
 def read_file(target:Path) -> str:
     """
     Read the content of the given target filepath (absolute or relative to the cwd),
@@ -125,7 +131,16 @@
     return content
 
 
 
 
 def convert_url_to_utf8(nom: str) -> str:
     return unquote(nom, encoding="utf-8")
+
+
+
+def get_ide_button_png_path(lvl_up:str, button_name:str):
+    path = IdeConstants.ide_buttons_path_template.format(
+        lvl_up = lvl_up,
+        button_name = button_name
+    )
+    return path
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 """
 
 
 from mkdocs.config.base import Config
 from mkdocs.config import config_options as C
 from mkdocs_macros.plugin import MacrosPlugin
 
+
 from ..deprecation import typ_deprecated_with_custom_msg
 
 
 
 
 
 
 
+
 # Verify if something changed on the MacrosPlugin side... (moved to on_startup)
 # Current setup for MacrosPlugin v1.0.5
 
 _EXPECTED_MACRO_CONF = set("""
 module_name
 modules
 render_by_default
@@ -119,15 +121,15 @@
     When this option is set to True, any error raised within the code of the editor will stop
     the validation process without modifying the number of attempts left.
     """
 
     default_ide_height_lines = C.Type(int, default=30)
     """
     Max height of the editor (in number of lines). For the macro IDEv, this takes precedence on
-    the TERM_H argument.
+    the TERM_H argument of the terminal.
     """
 
     deactivate_stdout_for_secrets = C.Type(bool, default=True)
     """
     Define if the stdout will be shown to the user or not, for the secret tests.
     """
 
@@ -137,14 +139,43 @@
     will be left unchanged, when an error is raised during the secret tests.
     """
 
 
 
 
 
+class TermConfig(Config):
+    """ Terminals configuration options """
+
+    default_height_ide_term = C.Type(int, default=10)
+    """
+    Default height value (number of lines) for terminals in IDEs.
+    """
+
+
+    default_height_isolated_term = C.Type(int, default=10)
+    """
+    Default height value (number of lines) for isolated terminals.
+    """
+
+
+    stdout_cut_off = C.Type(int, default=200)
+    """
+    Maximum number of lines displayed at once in a terminal. If more lines are printed, the
+    lines at the top are removed.
+
+    NOTE: jQuery.terminals become AWFULLY SLOW when the number of characters they display
+    become somewhat massive. This option allows to limit these performances troubles, when
+    the stdout is not truncated (see terminals upper right corner button). Also note that
+    this option _does not_ limit the number of characters per line, so a frozen page can
+    still occur, while the truncation feature will take care of that.
+    """
+
+
+
 
 
 class BuildConfig(Config):
     """ Build configuration options """
 
 
     ignore_macros_plugin_diffs = C.Type(bool, default=False)
@@ -176,14 +207,24 @@
     This ensures that the macros related to IDEs will work properly.
 
     If unwanted characters are found, a BuildError is raised, but this verification can be turned
     off by setting this flag to True. Use it at your own risks.
     """
 
 
+    python_libs = C.ListOfItems(C.Type(str), default=['py_libs'])
+    """
+    Personal python packages directories to use on the built site.
+
+    * Invalid names are ignored during the build.
+    * A warning will be emitted, unless it's the default directory that is missing.
+    * The libraries have to be ___directories___ in the project directory (_not_ the docs_dir).
+    """
+
+
 
     load_yaml_encoding = C.Type(str, default='utf-8')
     """
     Encoding to use when loading yaml data with the original MacrosPlugin functionalities :
 
     The original method doesn't use any encoding argument, which can lead to different behaviors
     between Windows and Linux (typically: during a pipeline!).
@@ -197,16 +238,18 @@
     indented multiline contents in the page.
 
     This is relying on `PyodideMacrosPlugin.get_indent` logistic.
     """
 
 
 
-    bypass_indent_errors = C.Type(bool, default=False)
+    bypass_indent_errors = typ_deprecated_with_custom_msg('bypass_indent_errors', bool, False)
     """
+    _DEPRECATED: This option shouldn't be needed anymore._
+
     If True, all errors raised when trying to find what is the indentation level of a macro call
     are bypassed and a message is instead printed to the console.
 
     The purpose of this option is _not_ to deactivate the securities, but to allow gathering info
     about all the indentation problems at once: the resulting markdown content will most likely be
     incorrect and be rendered with unexpected results.
     """
@@ -303,31 +346,30 @@
 
 # This only defines the values exposed to the user in mkdocs.yml.
 # When a property is declared here, don't forgot to add the related extractor on the
 # BaseMaestro class.
 class PyodideMacrosConfig(Config):
     """ Configuration for the main pyodide-mkdocs-theme plugin. """
 
+    _dev_mode = C.Type(bool, default=False)
+    """ Run the plugin in development mode (...don't use that). """
+
 
     build = C.SubConfig(BuildConfig)
     """ Build related options """
 
-
     ides = C.SubConfig(IdeConfig)
     """ Configuration related to the validation tests in IDEs """
 
+    terms = C.SubConfig(TermConfig)
+    """ Configuration related to the terminals """
 
     qcms = C.SubConfig(QcmsConfig)
     """ QCMs related options """
 
-
-    _dev_mode = C.Type(bool, default=False)
-    """ Run the plugin in development mode (...don't use that). """
-
-
     _others = C.SubConfig(OtherConfig)
     """ Old configuration options (unmaintained, so far) """
 
 
     # ---------------------------------------------------------------------------------------
     # Replication of MacrosPlugin options (merging the config_scheme properties programmatically
     # is not enough, unfortunately...)
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,83 +15,60 @@
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 # pylint: disable=multiple-statements, attribute-defined-outside-init, unused-argument
 
 
-import re
 from collections import defaultdict
-from typing import ClassVar, Dict, List, Optional, Set, Tuple, Union
+from typing import Dict, List, Optional, Set, Tuple, Union
 from pathlib import Path
 
 from mkdocs.exceptions import BuildError
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.structure.pages import Page
 from mkdocs.structure.nav import Navigation
 from mkdocs.plugins import event_priority
 
 
 
-from ..tools_and_constants import INSERTIONS_KINDS, PageUrl
-from ..pages_and_ides_configs import (
-    IdeConfigKey,
-    PageConfiguration,
-    ScriptKind
-)
+from ..tools_and_constants import INSERTIONS_KINDS, IdeConstants, PageUrl
+from ..pages_and_ides_configs import PageConfiguration, ScriptKind
 from ..pyodide_logger import logger
-from ..parsing import eat, encrypt_string
+from ..parsing import eat, compress_LZW
 from ..scripts_templates import SCRIPTS_TEMPLATES
 
 from .maestro_tools import AutoCounter
-from .maestro_base import BaseMaestro
 from .maestro_indent import MaestroIndent
 
 
 
 
 
 
 
 
 
 
-class MaestroIDE(MaestroIndent,BaseMaestro):
+class MaestroIDE(MaestroIndent):
     """ Holds the global logic related to the IDE macros """
 
 
-
-    ENCRYPTION_TOKEN: ClassVar[str] = "ENCRYPTION_TOKEN"
-    """
-    Denote the start and end point of the content of the div tag holding correction and/or remark.
-    (only used in the python layer: it is either removed in the on_page_context hook, or it's just
-    not inserted at all if the encrypt_corrections_and_rems is False)
-    """
-
-    MIN_RECURSION_LIMIT: ClassVar[int] = 20
-    """
-    Minimum recursion depth allowed.
-    """
-
-    HDR_PATTERN: ClassVar[re.Pattern] = re.compile(
-        r"#\s*-+\s*(?:HDR|ENV)\s*-+\s*#", flags=re.IGNORECASE
-    )
-    """
-    Old fashion way of defining the `env` code in the python source file (still supported).
-    """
-
-
-    terminal_count: int = AutoCounter()
+    generic_count: int = AutoCounter()
     """
     Number of empty terminals (per site count. Related to the terminal() macro).
+    Since there are no data associated to these in the locale storage (at least, no _important_
+    data), this counter is used for everything.
     """
 
     ide_count: int = AutoCounter()
     """
     Number of empty IDEs (per site count. Used for IDE without python files).
+    Dedicated counter, for legacy reasons. Might break users' storage sometimes, but this will
+    provide more consistency with the evolution of the redactor's documentation.
     """
 
     _editors_ids:  Set[str]
     """
     Store the ids of all the created IDEs, to enforce their uniqueness.
     """
 
@@ -109,15 +86,15 @@
     Represent the configurations of every IDE in every Page of the documentation.
     """
 
 
 
     def on_config(self, config:MkDocsConfig):
 
-        self.terminal_count = 0
+        self.generic_count = 0
         self.ide_count = 0
         self._editors_ids = set()
         self._pages_configs = defaultdict(lambda: PageConfiguration(self))
         self._scripts_or_link_tags_to_insert = {}
 
         self.register_js_and_css_tags(SCRIPTS_TEMPLATES)
 
@@ -133,15 +110,15 @@
         This hook uses high priority because the html content must be modified before the search
         plugin starts indexing stuff in it (which precisely happens in the on_page_context hook).
         """
         # pylint: disable=pointless-string-statement
 
         if self.is_page_with_something_to_insert(page):
 
-            logger.debug(f"Add scripts + encrypt solutions and remarks in { page.file.src_uri }")
+            logger.debug(f"Add scripts + encrypt solutions and remarks in { self.location() }")
             """
             self._omg_they_killed_keanu("exercices/tests_feedback/", page)
             chunks = [page.content]
             """
             chunks = []
             self.chunk_and_encrypt_solutions_and_rems(page.content, chunks)
             #"""
@@ -182,15 +159,15 @@
         if isinstance(opt_path_or_content,str):
             content = opt_path_or_content
         else:
             if opt_path_or_content is None or not opt_path_or_content.is_file():
                 return '','',''
             content = opt_path_or_content.read_text(encoding="utf-8")
 
-        lst = self.HDR_PATTERN.split(content)
+        lst = IdeConstants.hdr_pattern.split(content)
         # NOTE: If HDR tokens are present, split will return an empty string as first element, so:
         #   - len == 1 : [content]
         #   - len == 3 : ['', hdr, content]
 
         if len(lst) not in (1,3):
             raise BuildError(
                 f"Wrong number of HDR/ENV tokens (found { len(lst)-1 }) in:\n"
@@ -241,16 +218,18 @@
             for kind,s in self._scripts_or_link_tags_to_insert.items()
         ))
 
 
     #---------------------------------------------------------------------------------------
 
 
-    def set_current_page_js_data(self, editor_name:str, prop:IdeConfigKey, data:Union[str,int]):
-        """ Store data for an IDE in the current Page """
+    def set_current_page_js_data(self, editor_name:str, prop:str, data:Union[str,int]):
+        """
+        Store data for an IDE in the current Page. @prop must be a property of the IdeConfig class.
+        """
         self._pages_configs[self.page.url].set(editor_name, prop, data)
 
 
     def set_current_page_insertion_needs(self, *kind:ScriptKind):
         """ Mark a page url as needing some specific kinds of scripts (depending on the macro
             triggering the call). """
         self._pages_configs[self.page.url].update_kinds(kind)
@@ -304,28 +283,28 @@
         """
         if not self.encrypt_corrections_and_rems:
             chunks.append(html)
             return
 
         entering = 0
         while entering < len(html):
-            i,j = eat(html, self.ENCRYPTION_TOKEN, start=entering, skip_error=True)
+            i,j = eat(html, IdeConstants.encryption_token, start=entering, skip_error=True)
             i,j = self._cleanup_p_tags_around_encryption_tokens(html, i, j)
 
             chunks.append( html[entering:i] )
 
             if i==len(html):
                 break
 
-            ii,entering = eat(html, self.ENCRYPTION_TOKEN, start=j)     # raise if not found
+            ii,entering = eat(html, IdeConstants.encryption_token, start=j)     # raise if not found
             ii,entering = self._cleanup_p_tags_around_encryption_tokens(html, ii, entering)
 
             solution_and_rem = html[j:ii].strip()
-            encrypted = encrypt_string(solution_and_rem)
-            chunks.append(encrypted)
+            encrypted_content = compress_LZW(solution_and_rem)
+            chunks.append(encrypted_content)
 
 
 
     def _cleanup_p_tags_around_encryption_tokens(self, html:str, i:int, j:int):
         """
         mkdocs automatically surrounds the encryption token with <p> tag, so they must be removed.
         Note: Including the tags in the ENCRYPTION_TOKEN doesn't change the problem: you'd just
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,30 +21,38 @@
 
 import re
 import json
 from typing import List, Optional
 from pathlib import Path
 
 from mkdocs.config.defaults import MkDocsConfig
+from mkdocs.exceptions import BuildError
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.pages import Page
 
+
 from ...__version__ import __version__
+from ..tools_and_constants import ICONS_IN_TEMPLATES_DIR
+from ..deprecation import deprecation_warning
 from ..messages import Lang
 from ..pyodide_logger import logger
 from .maestro_tools import ConfigExtractor, dump_and_dumper
 from .config import PyodideMacrosConfig
 
 
 
 
 
-ICONS_FROM_TEMPLATES = Path("pyodide-mkdocs/IDE-and-buttons/images/")
 
-NO_DUMP = tuple('docs_dir_path docs_dir_cwd_rel lang page'.split())
+NO_DUMP = tuple('''
+    docs_dir_path
+    docs_dir_cwd_rel
+    lang
+    page
+'''.split())
 
 
 
 
 
 class BaseMaestro( BasePlugin[PyodideMacrosConfig] ):
     """
@@ -57,44 +65,55 @@
     extend MacrosPlugin at some point.
     """
 
     ignore_macros_plugin_diffs:              bool = ConfigExtractor('build')
     skip_py_md_paths_names_validation:       bool = ConfigExtractor('build')
     load_yaml_encoding:                      str  = ConfigExtractor('build')
     macros_with_indents:                List[str] = ConfigExtractor('build')
-    bypass_indent_errors:                    bool = ConfigExtractor('build')
     encrypt_corrections_and_rems:            bool = ConfigExtractor('build')
     forbid_secrets_without_corr_or_REMs:     bool = ConfigExtractor('build')
     forbid_hidden_corr_and_REMs_without_secrets: bool = ConfigExtractor('build')
     forbid_corr_and_REMs_with_infinite_attempts: bool = ConfigExtractor('build')
-    # check_python_files:                      bool = ConfigExtractor('build')
-    # soft_check:                              bool = ConfigExtractor('build')
+    python_libs:                        List[str] = ConfigExtractor('build')
+    # bypass_indent_errors:                  bool = ConfigExtractor('build')
+    # check_python_files:                    bool = ConfigExtractor('build')
+    # soft_check:                            bool = ConfigExtractor('build')
 
     show_assertion_code_on_failed_test:      bool = ConfigExtractor("ides")
     max_attempts_before_corr_available:      bool = ConfigExtractor("ides")
     decrease_attempts_on_user_code_failure:  bool = ConfigExtractor("ides")
-    default_ide_height_lines:       Optional[int] = ConfigExtractor("ides")
+    default_ide_height_lines:                 int = ConfigExtractor("ides")
     deactivate_stdout_for_secrets: Optional[bool] = ConfigExtractor("ides")
     show_only_assertion_errors_for_secrets: Optional[bool] = ConfigExtractor("ides")
 
+    default_height_ide_term:              int = ConfigExtractor("terms")
+    default_height_isolated_term:             int = ConfigExtractor("terms")
+    stdout_cut_off:                           int = ConfigExtractor("terms")
+
+
     hide:    Optional[bool] = ConfigExtractor("qcms")
     multi:   Optional[bool] = ConfigExtractor("qcms")
     shuffle: Optional[bool] = ConfigExtractor("qcms")
 
-    _dev_mode:  bool = ConfigExtractor()
+    _dev_mode:               bool = ConfigExtractor()
+    j2_block_start_string:    str = ConfigExtractor()
+    j2_block_end_string:      str = ConfigExtractor()
+    j2_variable_start_string: str = ConfigExtractor()
+    j2_variable_end_string:   str = ConfigExtractor()
 
     scripts_url: str = ConfigExtractor("_others")
     site_root:   str = ConfigExtractor("_others")
 
 
     # global mkdocs config data:
     docs_dir:    str = ConfigExtractor(root='_conf')
     repo_url:    str = ConfigExtractor(root='_conf')
     site_name:   str = ConfigExtractor(root='_conf')
     site_url:    str = ConfigExtractor(root='_conf')
+    site_dir:    str = ConfigExtractor(root='_conf')
 
 
     #----------------------------------------------------------------------------
     # WARNING: the following properties are assigned from "other places":
     #   - pages from the original MacrosPlugin
     #   - others from PyodideMacrosPlugin
 
@@ -119,63 +138,119 @@
     base_url:str = ""
     pmt_url:str = 'https://gitlab.com/frederic-zinelli/pyodide-mkdocs-theme'
     version:str = __version__
 
     lang: Lang = None
 
 
-
-    def on_config(self, config:MkDocsConfig):
-        # pylint: disable=unused-argument, no-member, missing-function-docstring
+    def on_config(self, config:MkDocsConfig):       # pylint: disable=missing-function-docstring
 
         self.lang = Lang()
         self.lang.register_env(self)
 
-        if self.bypass_indent_errors:
-            logger.warning("bypass_indent_errors option is activated.")
         if self.skip_py_md_paths_names_validation:
             logger.warning("skip_py_md_paths_names_validation option is activated.")
 
-        super().on_config(config)     # MacrosPlugin is actually "next in line" and has the method
+        super().on_config(config)   # pylint: disable-next=no-member
+                                    # MacrosPlugin is actually "next in line" and has the method
+
+
+    #----------------------------------------------------------------------------
+
+    def location(self, page:Optional[Page]=None):
+        """ Path to the current file, relative to the cwd. """
+        page = page or getattr(self, 'page', None)
+        if not page:
+            raise BuildError("No page defined yet")
+        return f"{ self.docs_dir_cwd_rel }/{ page.file.src_uri }"
 
 
+    def level_up_from_current_page(self, url:str=None) -> str:
+        """
+        Return the appropriate number of ".." steps needed to build a relative url to go from the
+        current page url back to the root directory.
+
+        Note there are no trailing backslash.
+
+        @url: relative to the docs_dir (ex: "exercices/ ..."). If None, use self.page.url instead.
+        """
+        url = self.page.url if url is None else url
+        page_loc:Path = self.docs_dir_path / url
+        segments = page_loc.relative_to(self.docs_dir_path).parts
+        out = len(segments) * ['..']
+        return '/'.join(out) or '.'
+
+
+    #----------------------------------------------------------------------------
+
 
     def rebase(self, base_url:str):
         """
         Necessary for development only (to replace the wrong base_url value during a serve in the
         theme project)
-        NOTE: Keep in mind the bas_url SOMETIMES ends with a slash...
+        NOTE: Keep in mind the base_url SOMETIMES ends with a slash...
         """
         return base_url if base_url!='/' else '.'
 
 
     def dump_to_js_config(self, base_url):
         """
-        Create the <script> tag that will add all the CONFIG properties needed in the JS global.
+        Create the <script> tag that will add all the CONFIG properties needed in the JS
+        global config file, and also applies the post conversion where needed.
         """
-        to_dump = [ p for p in BaseMaestro.__annotations__ if p[0]!='_' and p not in NO_DUMP ]
+
+        to_dump = [
+            p for p in sorted(BaseMaestro.__annotations__)
+              if not p.startswith('_') and p not in NO_DUMP
+                 or p=='_dev_mode' and self and self._dev_mode
+        ]
 
         if self:                                # HACK!
             # pylint: disable=w0201
             base_url = self.rebase(base_url).rstrip('/')
-            self.button_icons_directory = f"{base_url}/{ICONS_FROM_TEMPLATES}"
+            self.button_icons_directory = f"{base_url}/{ICONS_IN_TEMPLATES_DIR}"
             self.base_url = base_url
 
-
         dct = dump_and_dumper(to_dump, self, json.dumps)
         dct['lang'] = Lang.dump_as_str(self and self.lang)
 
-
         if self is None:                        # HACK!
             # Dump to config.js (helper):
             dumping = [ f"\n    { prop }: { val }," for prop,val in dct.items() ]
             return ''.join(dumping)
 
-        # Dump to main.html:
+        # Dump to main.html...
         dumping = [ f"\n  CONFIG.{ prop } = { val }" for prop,val in dct.items() ]
 
+        # ... adding post conversions operations.
         out = f'''\
 <script type="application/javascript">
 { "".join(dumping) }
 CONFIG.lang.tests.as_pattern = new RegExp(CONFIG.lang.tests.as_pattern, 'i')
+CONFIG.pythonLibs = new Set(CONFIG.pythonLibs)
 </script>'''
         return out
+
+
+    #----------------------------------------------------------------------------
+
+
+    def _omg_they_killed_keanu(self,page_name:str, page_on_context:Page=None):
+        """ Debugging purpose only. Use as breakpoint utility.
+            @page_on_context argument used when called "outside" of the macro logic (fro example,
+            in external hooks)
+        """
+        page = page_on_context or self.page
+        if page_name == page.url:
+            logger.error("Breakpoint! (the CALL to this method should be removed)")
+
+
+    def warn_unmaintained(self, that:str):
+        """
+        Generic warning message for people trying to used untested/unmaintained macros.
+        """
+        deprecation_warning(
+            f"{ that.capitalize() } has not been maintained since the original pyodide-mkdocs "
+            "project, may not currently work, and will be removed in the future.\n"
+            "Please open an issue on the pyodide-mkdocs-theme repository, if you need it.\n\n"
+            f"\t{ self.pmt_url }"
+        )
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,41 +17,44 @@
 If not, see <https://www.gnu.org/licenses/>.
 """
 # pylint: disable=multiple-statements
 
 
 from mkdocs.config.defaults import MkDocsConfig
 
+
+
 from ..tools_and_constants import Prefix
-from .maestro_base import BaseMaestro
 from .maestro_tools import AutoCounter
+from .maestro_IDE import MaestroIDE
 
 
 
 
 
 
 
 
-class MaestroExtras(BaseMaestro):
+class MaestroExtras(MaestroIDE):
     """ Class holding the "one of"/remaining/unused functionalities """
 
 
     compteur_exo: int = AutoCounter(warn=True)
     """ Number of exercices (per page count. Related to exercice() macro)
         Can be reinitialized manually through arguments of the exercice macro.
     """
 
     compteur_qcms: int = AutoCounter()
     """ Number of qcm or qcs in the docs """
 
-    def get_qcm_id(self):
-        return f"{ Prefix.py_mk_qcm_id_ }{ self.compteur_qcms :0>5}"
-
-
 
     def on_config(self, config:MkDocsConfig):
         # pylint: disable=attribute-defined-outside-init
         self.compteur_exo = 0
         self.compteur_qcms = 0
 
         super().on_config(config)
+
+
+
+    def get_qcm_id(self):
+        return f"{ Prefix.py_mk_qcm_id_ }{ self.compteur_qcms :0>5}"
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,262 +14,265 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
+import os
 import re
-from typing import Dict, Optional, Union
+import shutil
+from collections import defaultdict
+from functools import wraps
 from pathlib import Path
 
+from mkdocs.structure.files import Files, File
 from mkdocs.config.defaults import MkDocsConfig
-from mkdocs.structure.pages import Page
 from mkdocs.exceptions import BuildError
-
-
-from ..deprecation import deprecation_warning
-from ..messages import  Msg, Tip
-
-from ..tools_and_constants import PageUrl
-from ..pyodide_logger import logger
-from ..parsing import eat
-
-from .maestro_base import BaseMaestro
-
+from mkdocs_macros.plugin import MacrosPlugin
 
 
 
 
 
+from ...__version__ import __version__
+from ..exceptions import PyodideConfigurationError
+from ..tools_and_constants import PY_LIBS
+from ..pyodide_logger import logger
+from ..macros import (
+    autres,
+    IDEs,
+    isolated_components,
+    qcm,
+)
+from .config import MISSING_MACROS_PROPS, EXTRAS_MACROS_PROPS
+from .maestro_base import BaseMaestro
+from .maestro_indent import MaestroIndent
+from .maestro_IDE import MaestroIDE
+from .maestro_extras import MaestroExtras
 
 
 
 
 
-class MaestroIndent(BaseMaestro):
-    """ Manage Indentation logistic """
 
 
-    _pages_indents: 'PageIndents'
-    """
-    Cache storing the indentations for each jinja/macro template in a Page.
-    A page is entirely studied the first time it's seen and the result of the indentation levels
-    are stored.
-    The data stays correct throughout the md->html conversion because the indentation levels
-    "horizontal") are not affected by the content growing ("vertical").
+class PyodideMacrosPlugin(
+    MaestroExtras,
+    MaestroIDE,
+    MaestroIndent,
+    BaseMaestro,
+    MacrosPlugin,    # Always last, so that other classes may trigger super methods appropriately.
+):
     """
+    Class centralizing all the behaviors of the different parent classes.
 
-    _running_macro: Optional[str] = None
-    """
-    Name of the macro currently running (or the last one called. None if no macro called yet).
-    """
+    This is kinda the "controller", linking all the behaviors to mkdocs machinery, while the
+    parent classes hold the "somewhat self contained" behaviors.
 
+    For reference, here are the hooks defined in the original MacrosPlugin:
+        - on_config
+        - on_nav
+        - on_page_markdown  (+ on_pre_page_macros + on_post_page_macros)
+        - on_post_build     (on_post_build macros)
+        - on_serve
+    """
 
 
+    # Override
     def on_config(self, config:MkDocsConfig):
-        # pylint: disable=unused-argument, no-member, missing-function-docstring
-        self._pages_indents = PageIndents()
-        super().on_config(config)     # MacrosPlugin is actually "next in line" and has the method
+        # pylint: disable=attribute-defined-outside-init
+        # --------------------------------------------------------------
+        # Section to always apply first:
 
+        self._conf = config # done in MacrosPlugin, but also done here because needed here or there
 
-    def override_messages(self, dct_lang: Dict[str, Union[Msg,Tip]]):
-        """ Replace some default messages or configurations with the given content """
-        self.lang.overload(dct_lang)
+        self.docs_dir_path    = Path(config.docs_dir)
+        self.docs_dir_cwd_rel = self.docs_dir_path.relative_to(Path.cwd())
 
+        # --------------------------------------------------------------
 
-    #----------------------------------------------------------------------------
+        self._check_macros_plugin_props()
+        self._check_docs_paths_validity()
 
+        super().on_config(config)
 
-    def get_indent_in_current_page(self, macro_predicate:re.Pattern):
-        """
-        Extract the indentation needed for the given macro template call.
-        @throws:    BuildError if the same macro call is found several times in the page.
-        """
-        return self._pages_indents.get_indent(self, macro_predicate)
 
 
-    def is_macro_with_indent(self, macro_call:str) -> bool:
+    def on_files(self, files: Files, /, *, config: MkDocsConfig):
         """
-        Return True if the given macro call requires to register indentation data.
-        This is using a white list, so that user defined macro cannot cause troubles.
+        If python libs directories are registered, create one archive for each of them.
+        It's on the responsibility of the user to work with them correctly...
         """
-        return bool(self._macro_with_indent_pattern.match(macro_call))
+        for py_str in self.python_libs:
+            py_path = Path(py_str)
 
+            if py_str.endswith('.py'):
+                raise BuildError(
+                    f"Python libraries must be packages but was: {py_str}.\n\n"
+                    "(package = a directory with at least an __init__.py file, "
+                    "and possibly other files or packages)"
+                )
+            elif not py_path.exists():
+                if py_str != PY_LIBS:
+                    logger.warning(f"Invalid python library: {py_str} not found")
+                continue
+            if len(py_path.parts) > 1:
+                raise BuildError(
+                    f"Python libraries have to be directly in the CWD, but was: {py_str}"
+                )
 
-    def level_up_from_current_page(self, url:str=None) -> str:
-        """
-        Return the appropriate number of ".." steps needed to build a relative url to go from the
-        current page url back to the root directory.
+            # Remove any cached files to make the archive lighter (the version won't match
+            # pyodide compiler anyway!):
+            for cached in py_path.rglob("*.pyc"):
+                cached.unlink()
+
+            shutil.make_archive(py_path, 'zip', py_path)
+            files.append(
+                File(py_str+'.zip', '.', Path(self.site_dir), False)
+            )
 
-        Note there are no trailing backslash.
 
-        @url: relative to the docs_dir (ex: "exercices/ ..."). If None, use self.page.url instead.
+    # Override
+    def on_post_build(self, config: MkDocsConfig) -> None:
         """
-        url = self.page.url if url is None else url
-        page_loc:Path = self.docs_dir_path / url
-        segments = page_loc.relative_to(self.docs_dir_path).parts
-        out = len(segments) * ['..']
-        return '/'.join(out) or '.'
+        Suppress the python archives from the CWD.
+        """
+        for py_str in self.python_libs:
+            file = Path(py_str+'.zip')
+            file.unlink(missing_ok=True)
 
+        super().on_post_build(config)
 
-    #----------------------------------------------------------------------------
 
+    #--------------------------------------------------------------------------
 
-    def _omg_they_killed_keanu(self,page_name:str, page_on_context:Page=None):
-        """ Debugging purpose only. Use as breakpoint utility.
-            @page_on_context argument used when called "outside" of the macro logic (fro example,
-            in external hooks)
-        """
-        page = page_on_context or self.page
-        if page_name == page.url:
-            logger.error("Breakpoint! (the CALL to this method should be removed)")
 
 
-    def warn_unmaintained(self, that:str):
-        """
-        Generic warning message for people trying to used untested/unmaintained macros.
-        """
-        deprecation_warning(
-            f"{ that.capitalize() } has not been maintained since the original pyodide-mkdocs "
-            "project, may not currently work, and will be removed in the future.\n"
-            "Please open an issue on the pyodide-mkdocs-theme repository, if you need it.\n\n"
-            f"\t{ self.pmt_url }"
-        )
+    # Override
+    def _load_modules(self):
+        """ Override the super method to register the Pyodide macros at appropriate time """
 
+        def macro_with_warning(func):
+            macro = func(self)
+            logged = False          # log once only only per macro...
 
+            @wraps(func)
+            def wrapper(*a,**kw):
+                nonlocal logged
+                if not logged:
+                    logged = True
+                    self.warn_unmaintained(f'The macro {func.__name__!r}')
+                return macro(*a,**kw)
+            return wrapper
 
 
+        macros = [
+            IDEs.IDE,
+            IDEs.IDEv,
+            IDEs.terminal,
+            IDEs.py_btn,
+            IDEs.section,
 
+            qcm.multi_qcm,
 
+            # isolated_components.py_sujet,     # just an alias for py, actually...
+            isolated_components.py,
+        ]
+        old_macros = [
+            autres.cours,
+            autres.exercice,
+            autres.ext,
+            autres.html_fig,
+            autres.numworks,
+            autres.python_carnet,
+            autres.python_ide,
+            autres.tit,
+            autres.mult_col,
+        ]
 
+        for func in macros:
+            self.macro(func(self))
 
-class PageIndents( Dict[PageUrl, Dict[str,str]] ):
-    """ Cache storing the indentations for each jinja/macro template in all Pages.
-        a page is entirely studied the first time it's seen and the result of the indentation
-        levels are stored.
-        The data stays correct throughout the md->html conversion because the indentation
-        levels "horizontal") are not affected by the content growing ("vertical").
-    """
+        for func in old_macros:
+            self.macro( macro_with_warning(func) )
 
-    def _explore_page_markdown(self, env:'BaseMaestro', txt:str):
-        """
-        Gather the indentations for all the macros insertions (aka `{{...}}`) in the page markdown.
-        Only insertions following spaces or right at the beginning of a line are extracted.
+        super()._load_modules()
 
-        During parsing, it is also checked that there is no  `{{` starting again inside a macro
-        call (this is subject to false positives, if the call contains `"{{"`!)
-        """
-        dct = {}
-        end = len(txt)
 
-        i,i_cmd = eat(txt, '{{', skip_error=True)
-        while i < end:
 
-            i_next_open = eat(txt, '{{', start=i+2, skip_error=True)
-            i_close, _  = eat(txt, '}}', start=i)
+    # Override
+    def _load_yaml(self):
+        """
+        Override the MacrosPlugin method, replacing on the fly `__builtins__.open` with a version
+        handling the encoding.
+        """
+        # pylint: disable=multiple-statements
+        src_open = open
+        def open_with_utf8(*a,**kw):
+            return src_open(*a,**kw, encoding=self.load_yaml_encoding)
 
-            # Check no nested macro calls:
-            if i_next_open[0] < i_close:
-                self._handle_error(
-                    env,
-                    f"""
-Couldn't figure out the structure of macros calls in the template of the page {env.page.file.src_uri!s} :
-    {"{{"!r} at index {i}
-    {"{{"!r} at index {i_next_open[0]}  << should be after the next one
-    {"}}"!r} at index {i_close}
-If you are trying to use {"{{"!r} or {"}}"!r}:
-  - in data structures: just add some extra spaces in between.
-  - inside a string: please raise an issue on { env.pmt_url }.
-                    """.strip()
-                )
+        # Depending on the python version/context, the __builtins__ can be of different types
+        as_dct = isinstance(__builtins__, dict)
 
-            indent = self._extract_indentation(txt, i)
-            cmd = re.sub(r'\s+', '', txt[i_cmd:i_close] )
+        if as_dct:  __builtins__['open'] = open_with_utf8
+        else:       __builtins__.open = open_with_utf8
+        try:
+            super()._load_yaml()
+        finally:
+            if as_dct:  __builtins__['open'] = src_open
+            else:       __builtins__.open = src_open
 
-            if env.is_macro_with_indent(cmd):
-                if cmd not in dct:
-                    dct[cmd] = indent
-                else:
-                    call_data = txt[i_cmd:i_close]
-                    self._handle_error(env,
-                        f"In the page { env.page.file.src_uri }: the same macro call has been "
-                        "found several times (ignoring spaces).",
-                        epilogue=f"\n\nCall found:\n{ call_data }"
-                    )
 
-            i,i_cmd = i_next_open      # step forward to next opening template
 
-        self[env.page.url] = dct
+    #--------------------------------------------------------------------------
 
 
 
-    def _extract_indentation(self, txt:str, i_macro:int) -> int :
+    def _check_docs_paths_validity(self) -> None :
         """
-        Step back in the markdown until a line feed or a non space char is found, then return
-        the index of the char where the line begins or the previous "non space sequence" ends
+        Travel through all paths in the docs_dir and raises an BuildError if "special characters"
+        are found in directory, py, or md file names (accepted characters are: r'[\\w.-]+' )
         """
-        if not i_macro:
-            return ''
+        if self.skip_py_md_paths_names_validation:
+            return
 
-        i = i_macro-1
-        while i>0 and txt[i].isspace() and txt[i]!='\n':
-            i -= 1
+        invalid_chars = re.compile(r'[^A-Za-z0-9_.-]+')
+        wrongs = defaultdict(list)
 
-        n_indent = i_macro-i-1 if txt[i]=='\n' else 0
-        return ' ' * n_indent
+        # Validation is done on the individual/current segments of the paths, so that an invalid
+        # directory name is not affecting the validation of its children.
+        for path,dirs,files in os.walk(self.docs_dir):
+            files_to_check = [ file for file in files if re.search(r'\.(py|md)$', file)]
+            for segment in dirs + files_to_check:
+                invalids = frozenset(invalid_chars.findall(segment))
+                if invalids:
+                    wrongs[invalids].append( os.path.join(path,segment) )
 
+        if wrongs:
+            msg = ''.join(
+                f"\nWrong characters { repr(''.join(sorted(invalids))) } in:"
+                + "".join(f"\n\t{ path }" for path in sorted(lst))
+                for invalids,lst in wrongs.items()
+            )
+            raise BuildError(f'Found path(s) with invalid characters:{ msg }')
 
 
-    def get_indent(self, env:'BaseMaestro', macro_predicate:re.Pattern) -> str :
-        """
-        Extract the indentation needed for the given macro template call.
-        @throws:    BuildError if the same macro call is found several times in the page.
-        """
-        page:Page = env.page
-        if page.url not in self:
-            self._explore_page_markdown(env, env.page.markdown)
-
-        all_indents_in_page = self[page.url]
-        indents_gen = ( indent for cmd,indent in all_indents_in_page.items()
-                               if macro_predicate.match(cmd) )
-        target = next( indents_gen, None)
-        second = next( indents_gen, None)
-
-        id_reason = err_msg = ""
-        if target is None:
-            id_reason, err_msg = "no match", (
-                f"In the page { page.file.src_uri }:\nCouldn't find indentation data for the "
-                f"macro call with this pattern {macro_predicate.pattern!r}."
-            )
-        elif second is not None:
-            id_reason, err_msg = "duplicate match", (
-                f"In the page { page.file.src_uri }:\nFound several macro calls matching "
-                f"{macro_predicate.pattern}. This is not allowed because it could lead to "
-                "very weird behaviors/bugs."
-            )
-        if err_msg:
-            data = "\n\t>>>".join(map(repr, all_indents_in_page))
-            self._handle_error(env, err_msg,
-                f"\n\nRegistered indentation keys for the current page are:\n\t>>>{ data }"
-                f"\n\nDebugging info:\nFirst match is: {target=!r}\nSecond match is: {second=!r}",
-                id_reason=id_reason,
-            )
-        return target
 
+    def _check_macros_plugin_props(self):
+        """ Verify that the config of the MacroPlugin class is still the expected one """
 
+        if not MISSING_MACROS_PROPS and not EXTRAS_MACROS_PROPS:
+            return
 
-    def _handle_error(self, env:'BaseMaestro', err_msg:str, epilogue:str='', id_reason:str=""):
-        if env.bypass_indent_errors:
-            id_reason = id_reason or "invalid call structure?"
-            logger.warning(                 # pylint: disable-next=protected-access
-                f"[INDENT] - Macro {env._running_macro}, in {env.page.file.src_uri} ({id_reason})"
+        if self.ignore_macros_plugin_diffs:
+            logger.error(
+                "Inconsistent MacrosPlugin properties / ignore_macros_plugin_diffs is set to true"
             )
+
         else:
-            if id_reason:
-                err_msg = (
-                    f"{ err_msg }\nTo disambiguate the calls, use the ID:int argument of the "
-                    "macro. Do not forget to add it to every macro call of this kind in the "
-                    "page!\nIf this is coming from one of your own macro, you will need to add "
-                    "the related logic and argument in your code."
-                )
-            raise BuildError( err_msg + epilogue )
+            raise PyodideConfigurationError(f"""
+Cannot configure PyodideMacrosPlugin: the basic configuration of MacrosPlugin changed:
+{MISSING_MACROS_PROPS}{EXTRAS_MACROS_PROPS}"""
+"\nIf you absolutely need to run mkdocs before any fix is done, you can try the option "
+"`ignore_macros_plugin_diffs: true` in the `plugin_macros` section of `mkdocs.yml`, "
+"but there are no guarantees the build will succeed, depending on what the changes were.\n\n")
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
+
 from pyodide_mkdocs_theme.pyodide_macros import (
     PyodideMacrosPlugin,
     Msg, MsgPlural, TestsToken, Tip,
 )
 
 
 def define_env(env:PyodideMacrosPlugin):
@@ -40,58 +41,64 @@
                         MsgPlural(msg, plural="")
                         Tip(width_in_em, msg, kbd=None)
                         TestsToken(token_str)
     """
 
     custom = {
     # Editors:
+        "tests":      TestsToken("\n# Tests\n"),
         "comments":   Tip(15, "(Dés-)Active le code après la ligne <code>{tests}</code> "
                              "(insensible à la casse)", "Ctrl+I"),
-        "tests":      TestsToken("\n# Tests\n"),
 
 
     # Terminals
+        "feedback":      Tip(15, "Tronquer ou non le feedback dans les terminaux (sortie standard"
+                                " & stacktrace / relancer le code pour appliquer)"),
+        "wrap_term":     Tip(15, "Si activé, le texte copié dans le terminal est joint sur une "
+                                "seule ligne avant d'être copié dans le presse-papier"),
         "run_script":    Msg("Script lancé..."),
-        "success_msg":   Msg("Terminé sans erreur !"),
         "install_start": Msg("Installation de paquets python. Ceci peut prendre un certain temps..."),
         "install_done":  Msg("Installations terminées!"),
-        "feedback":      Tip(15, "Tronquer ou non le feedback dans les terminaux (sortie standard"
-                                " & stacktrace / relancer le code pour appliquer)"),
+        "success_msg":   Msg("Terminé sans erreur !"),
+
 
     # Terminals: validation success/failure messages
         "success_head":  Msg("Bravo !"),
-        "success_head_extra":  Msg("Vous avez réussi tous les tests !"),
-        "fail_head":     Msg("Dommage !"),
         "success_tail":  Msg("Pensez à lire"),
+        "fail_head":     Msg("Dommage !"),
         "reveal_corr":   Msg("le corrigé"),
         "reveal_join":   Msg("et"),
         "reveal_rem":    Msg("les commentaires"),
+        "success_head_extra":  Msg("Vous avez réussi tous les tests !"),
         "fail_tail":     MsgPlural("est maintenant disponible", "sont maintenant disponibles"),
 
 
     # Corr  rems admonition:
         "title_corr": Msg('Solution'),
         "title_rem":  Msg('Remarques'),
         "corr":       Msg('🐍 Proposition de correction'),
         "rem":        Msg('Remarques'),
 
 
-    # IDEs buttons & counter:
+    # Buttons, IDEs buttons & counter:
+        "py_btn": Tip(9, "Exécuter le code"),
         "play":       Tip(9,  "Exécuter le code", "Ctrl+S"),
         "check":      Tip(9,  "Valider", "Ctrl+Enter"),
         "download":   Tip(0,  "Télécharger"),
         "upload":     Tip(0,  "Téléverser"),
         "restart":    Tip(0,  "Réinitialiser l'éditeur"),
         "save":       Tip(0,  "Sauvegarder dans le navigateur"),
         "attempts_left": Msg("Évaluations restantes"),
 
+
     # QCMS
         "qcm_title":     MsgPlural("Question"),
         "qcm_mask_tip":  Tip(15, "Les réponses resteront cachées..."),
         "qcm_check_tip": Tip(11, "Vérifier les réponses"),
         "qcm_redo_tip":  Tip(9,  "Recommencer"),
 
+
     # Others
         "tip_trash": Tip(15, "Supprimer du navigateur les codes enregistrés pour {site_name}")
     }
 
     env.lang.overload(custom)
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,348 +1,343 @@
-00000000: 2222 220a 7079 6f64 6964 652d 6d6b 646f  """.pyodide-mkdo
-00000010: 6373 2d74 6865 6d65 0a43 6f70 796c 6566  cs-theme.Copylef
+00000000: 2320 7079 6f64 6964 652d 6d6b 646f 6373  # pyodide-mkdocs
+00000010: 2d74 6865 6d65 0a23 2043 6f70 796c 6566  -theme.# Copylef
 00000020: 7420 474e 5520 4750 4c76 3320 f09f 84af  t GNU GPLv3 ....
 00000030: 2032 3032 3420 4672 c3a9 64c3 a972 6963   2024 Fr..d..ric
-00000040: 205a 696e 656c 6c69 0a0a 5468 6973 2070   Zinelli..This p
-00000050: 726f 6772 616d 2069 7320 6672 6565 2073  rogram is free s
-00000060: 6f66 7477 6172 653a 2079 6f75 2063 616e  oftware: you can
-00000070: 2072 6564 6973 7472 6962 7574 6520 6974   redistribute it
-00000080: 2061 6e64 2f6f 7220 6d6f 6469 6679 0a69   and/or modify.i
-00000090: 7420 756e 6465 7220 7468 6520 7465 726d  t under the term
-000000a0: 7320 6f66 2074 6865 2047 4e55 2047 656e  s of the GNU Gen
-000000b0: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-000000c0: 6e73 6520 6173 2070 7562 6c69 7368 6564  nse as published
-000000d0: 2062 790a 7468 6520 4672 6565 2053 6f66   by.the Free Sof
-000000e0: 7477 6172 6520 466f 756e 6461 7469 6f6e  tware Foundation
-000000f0: 2c20 6569 7468 6572 2076 6572 7369 6f6e  , either version
-00000100: 2033 206f 6620 7468 6520 4c69 6365 6e73   3 of the Licens
-00000110: 652c 206f 720a 2861 7420 796f 7572 206f  e, or.(at your o
-00000120: 7074 696f 6e29 2061 6e79 206c 6174 6572  ption) any later
-00000130: 2076 6572 7369 6f6e 2e0a 0a54 6869 7320   version...This 
-00000140: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
-00000150: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
-00000160: 7065 2074 6861 7420 6974 2077 696c 6c20  pe that it will 
-00000170: 6265 2075 7365 6675 6c2c 0a62 7574 2057  be useful,.but W
-00000180: 4954 484f 5554 2041 4e59 2057 4152 5241  ITHOUT ANY WARRA
-00000190: 4e54 593b 2077 6974 686f 7574 2065 7665  NTY; without eve
-000001a0: 6e20 7468 6520 696d 706c 6965 6420 7761  n the implied wa
-000001b0: 7272 616e 7479 206f 660a 4d45 5243 4841  rranty of.MERCHA
-000001c0: 4e54 4142 494c 4954 5920 6f72 2046 4954  NTABILITY or FIT
-000001d0: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
-000001e0: 4355 4c41 5220 5055 5250 4f53 452e 0a53  CULAR PURPOSE..S
-000001f0: 6565 2074 6865 2047 4e55 2047 656e 6572  ee the GNU Gener
-00000200: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-00000210: 6520 666f 7220 6d6f 7265 2064 6574 6169  e for more detai
-00000220: 6c73 2e0a 0a59 6f75 2073 686f 756c 6420  ls...You should 
-00000230: 6861 7665 2072 6563 6569 7665 6420 6120  have received a 
-00000240: 636f 7079 206f 6620 7468 6520 474e 5520  copy of the GNU 
-00000250: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-00000260: 6963 656e 7365 0a61 6c6f 6e67 2077 6974  icense.along wit
-00000270: 6820 7468 6973 2070 726f 6772 616d 2e0a  h this program..
-00000280: 4966 206e 6f74 2c20 7365 6520 3c68 7474  If not, see <htt
-00000290: 7073 3a2f 2f77 7777 2e67 6e75 2e6f 7267  ps://www.gnu.org
-000002a0: 2f6c 6963 656e 7365 732f 3e2e 0a22 2222  /licenses/>.."""
-000002b0: 0a0a 0a64 6566 2064 6973 706c 6179 5f79  ...def display_y
-000002c0: 6d6c 2829 3a0a 2020 2020 2222 220a 2020  ml():.    """.  
-000002d0: 2020 4d69 6e69 6d61 6c20 6d6b 646f 6373    Minimal mkdocs
-000002e0: 2e79 6d6c 2063 6f6e 6669 6775 7261 7469  .yml configurati
-000002f0: 6f6e 2066 696c 6520 666f 7220 5079 6f64  on file for Pyod
-00000300: 6964 652d 4d6b 646f 6373 2d54 6865 6d65  ide-Mkdocs-Theme
-00000310: 2e0a 2020 2020 2222 220a 0a20 2020 2070  ..    """..    p
-00000320: 7269 6e74 2827 2727 0a23 2056 6f69 6369  rint('''.# Voici
-00000330: 2075 6e20 6578 656d 706c 6520 7072 6573   un exemple pres
-00000340: 7175 6520 636f 6d70 6c65 7420 6465 2063  que complet de c
-00000350: 6f6e 6669 6775 7261 7469 6f6e 2070 6f75  onfiguration pou
-00000360: 7220 756e 2066 6963 6869 6572 0a23 206d  r un fichier.# m
-00000370: 6b64 6f63 732e 796d 6c20 7574 696c 6973  kdocs.yml utilis
-00000380: 616e 7420 7079 6f64 6964 652d 6d6b 646f  ant pyodide-mkdo
-00000390: 6373 2d74 6865 6d65 2e0a 0a73 6974 655f  cs-theme...site_
-000003a0: 7572 6c3a 2022 7b3e 3e20 4c27 6164 7265  url: "{>> L'adre
-000003b0: 7373 6520 6465 2076 6f74 7265 2073 6974  sse de votre sit
-000003c0: 6520 7765 6220 6963 6920 3c3c 7d22 0a73  e web ici <<}".s
-000003d0: 6974 655f 6e61 6d65 3a20 227b 3e3e 2054  ite_name: "{>> T
-000003e0: 6974 7265 2070 6f75 7220 766f 7472 6520  itre pour votre 
-000003f0: 7369 7465 203c 3c7d 220a 2320 7369 7465  site <<}".# site
-00000400: 5f64 6573 6372 6970 7469 6f6e 3a20 2228  _description: "(
-00000410: 6f70 7469 6f6e 6e65 6c29 220a 2320 7265  optionnel)".# re
-00000420: 706f 5f75 726c 3a20 2228 6f70 7469 6f6e  po_url: "(option
-00000430: 6e65 6c29 220a 2320 6564 6974 5f75 7269  nel)".# edit_uri
-00000440: 3a20 2228 6f70 7469 6f6e 6e65 6c29 220a  : "(optionnel)".
-00000450: 0a23 2043 6f70 7972 6967 6874 2022 4343  .# Copyright "CC
-00000460: 2042 592d 4e43 2d53 4122 0a63 6f70 7972   BY-NC-SA".copyr
-00000470: 6967 6874 3a20 7c0a 2020 3c70 2078 6d6c  ight: |.  <p xml
-00000480: 6e73 3a63 633d 2268 7474 703a 2f2f 6372  ns:cc="http://cr
-00000490: 6561 7469 7665 636f 6d6d 6f6e 732e 6f72  eativecommons.or
-000004a0: 672f 6e73 2322 0a20 2078 6d6c 6e73 3a64  g/ns#".  xmlns:d
-000004b0: 6374 3d22 6874 7470 3a2f 2f70 7572 6c2e  ct="http://purl.
-000004c0: 6f72 672f 6463 2f74 6572 6d73 2f22 3e50  org/dc/terms/">P
-000004d0: 6172 7461 6765 206f 7520 6164 6170 7461  artage ou adapta
-000004e0: 7469 6f6e 2070 6f73 7369 626c 6520 7365  tion possible se
-000004f0: 6c6f 6e20 6c65 7320 636f 6e64 6974 696f  lon les conditio
-00000500: 6e73 2064 6520 6c61 0a20 206c 6963 656e  ns de la.  licen
-00000510: 6365 203c 610a 2020 6872 6566 3d22 6874  ce <a.  href="ht
-00000520: 7470 3a2f 2f63 7265 6174 6976 6563 6f6d  tp://creativecom
-00000530: 6d6f 6e73 2e6f 7267 2f6c 6963 656e 7365  mons.org/license
-00000540: 732f 6279 2d6e 632d 7361 2f34 2e30 2f3f  s/by-nc-sa/4.0/?
-00000550: 7265 663d 6368 6f6f 7365 722d 7631 220a  ref=chooser-v1".
-00000560: 2020 7461 7267 6574 3d22 5f62 6c61 6e6b    target="_blank
-00000570: 2220 7265 6c3d 226c 6963 656e 7365 206e  " rel="license n
-00000580: 6f6f 7065 6e65 7220 6e6f 7265 6665 7272  oopener noreferr
-00000590: 6572 220a 2020 7374 796c 653d 2264 6973  er".  style="dis
-000005a0: 706c 6179 3a69 6e6c 696e 652d 626c 6f63  play:inline-bloc
-000005b0: 6b3b 223e 2043 4320 4259 2d4e 432d 5341  k;"> CC BY-NC-SA
-000005c0: 2034 2e30 203c 696d 670a 2020 7374 796c   4.0 <img.  styl
-000005d0: 653d 2268 6569 6768 743a 3232 7078 2169  e="height:22px!i
-000005e0: 6d70 6f72 7461 6e74 3b6d 6172 6769 6e2d  mportant;margin-
-000005f0: 6c65 6674 3a33 7078 3b76 6572 7469 6361  left:3px;vertica
-00000600: 6c2d 616c 6967 6e3a 7465 7874 2d62 6f74  l-align:text-bot
-00000610: 746f 6d3b 220a 2020 7372 633d 2268 7474  tom;".  src="htt
-00000620: 7073 3a2f 2f6d 6972 726f 7273 2e63 7265  ps://mirrors.cre
-00000630: 6174 6976 6563 6f6d 6d6f 6e73 2e6f 7267  ativecommons.org
-00000640: 2f70 7265 7373 6b69 742f 6963 6f6e 732f  /presskit/icons/
-00000650: 6363 2e73 7667 3f72 6566 3d63 686f 6f73  cc.svg?ref=choos
-00000660: 6572 2d76 3122 3e3c 696d 670a 2020 7374  er-v1"><img.  st
-00000670: 796c 653d 2268 6569 6768 743a 3232 7078  yle="height:22px
-00000680: 2169 6d70 6f72 7461 6e74 3b6d 6172 6769  !important;margi
-00000690: 6e2d 6c65 6674 3a33 7078 3b76 6572 7469  n-left:3px;verti
-000006a0: 6361 6c2d 616c 6967 6e3a 7465 7874 2d62  cal-align:text-b
-000006b0: 6f74 746f 6d3b 220a 2020 7372 633d 2268  ottom;".  src="h
-000006c0: 7474 7073 3a2f 2f6d 6972 726f 7273 2e63  ttps://mirrors.c
-000006d0: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-000006e0: 7267 2f70 7265 7373 6b69 742f 6963 6f6e  rg/presskit/icon
-000006f0: 732f 6279 2e73 7667 3f72 6566 3d63 686f  s/by.svg?ref=cho
-00000700: 6f73 6572 2d76 3122 3e3c 696d 670a 2020  oser-v1"><img.  
-00000710: 7374 796c 653d 2268 6569 6768 743a 3232  style="height:22
-00000720: 7078 2169 6d70 6f72 7461 6e74 3b6d 6172  px!important;mar
-00000730: 6769 6e2d 6c65 6674 3a33 7078 3b76 6572  gin-left:3px;ver
-00000740: 7469 6361 6c2d 616c 6967 6e3a 7465 7874  tical-align:text
-00000750: 2d62 6f74 746f 6d3b 220a 2020 7372 633d  -bottom;".  src=
-00000760: 2268 7474 7073 3a2f 2f6d 6972 726f 7273  "https://mirrors
-00000770: 2e63 7265 6174 6976 6563 6f6d 6d6f 6e73  .creativecommons
-00000780: 2e6f 7267 2f70 7265 7373 6b69 742f 6963  .org/presskit/ic
-00000790: 6f6e 732f 6e63 2e73 7667 3f72 6566 3d63  ons/nc.svg?ref=c
-000007a0: 686f 6f73 6572 2d76 3122 3e3c 696d 670a  hooser-v1"><img.
-000007b0: 2020 7374 796c 653d 2268 6569 6768 743a    style="height:
-000007c0: 3232 7078 2169 6d70 6f72 7461 6e74 3b6d  22px!important;m
-000007d0: 6172 6769 6e2d 6c65 6674 3a33 7078 3b76  argin-left:3px;v
-000007e0: 6572 7469 6361 6c2d 616c 6967 6e3a 7465  ertical-align:te
-000007f0: 7874 2d62 6f74 746f 6d3b 220a 2020 7372  xt-bottom;".  sr
-00000800: 633d 2268 7474 7073 3a2f 2f6d 6972 726f  c="https://mirro
-00000810: 7273 2e63 7265 6174 6976 6563 6f6d 6d6f  rs.creativecommo
-00000820: 6e73 2e6f 7267 2f70 7265 7373 6b69 742f  ns.org/presskit/
-00000830: 6963 6f6e 732f 7361 2e73 7667 3f72 6566  icons/sa.svg?ref
-00000840: 3d63 686f 6f73 6572 2d76 3122 3e3c 2f61  =chooser-v1"></a
-00000850: 3e3c 2f70 3e0a 0a0a 646f 6373 5f64 6972  ></p>...docs_dir
-00000860: 3a20 646f 6373 0a0a 6e61 763a 0a20 202d  : docs..nav:.  -
-00000870: 2022 4163 6375 6569 6c22 3a20 696e 6465   "Accueil": inde
-00000880: 782e 6d64 0a23 202d 202e 2e2e 0a0a 2320  x.md.# - .....# 
-00000890: 506f 7572 2073 7570 7072 696d 6572 2063  Pour supprimer c
-000008a0: 6572 7461 696e 7320 6669 6368 6965 7273  ertains fichiers
-000008b0: 206d 6172 6b64 6f77 6e20 6465 206c 6120   markdown de la 
-000008c0: 6e61 7669 6761 7469 6f6e 2028 7061 7474  navigation (patt
-000008d0: 6572 6e20 7368 656c 6c29 3a0a 2320 6e6f  ern shell):.# no
-000008e0: 745f 696e 5f6e 6176 3a20 7c0a 2320 2020  t_in_nav: |.#   
-000008f0: 2a2f 2a2a 2f2a 2e6d 640a 0a23 204e c3a9  */**/*.md..# N..
-00000900: 6365 7373 6974 6520 6d6b 646f 6373 2031  cessite mkdocs 1
-00000910: 2e36 2b20 706f 7572 2066 6f6e 6374 696f  .6+ pour fonctio
-00000920: 6e6e 6572 2063 6f72 7265 6374 656d 656e  nner correctemen
-00000930: 742e 2053 696e 6f6e 2c20 766f 7573 2070  t. Sinon, vous p
-00000940: 6f75 7665 7a20 7574 696c 6973 6572 0a23  ouvez utiliser.#
-00000950: 206c 6520 706c 7567 696e 206d 6b64 6f63   le plugin mkdoc
-00000960: 732d 6578 636c 7564 6520 c3a0 206c 6120  s-exclude .. la 
-00000970: 706c 6163 652e 0a23 204e 6520 7375 7274  place..# Ne surt
-00000980: 6f75 7420 7061 7320 6d65 7474 7265 2064  out pas mettre d
-00000990: 6520 636f 6d6d 656e 7461 6972 6573 2073  e commentaires s
-000009a0: 7572 206c 6120 6c69 676e 6520 6427 6578  ur la ligne d'ex
-000009b0: 636c 7573 696f 6e20 6465 7320 6669 6368  clusion des fich
-000009c0: 6965 7273 2070 7974 686f 6e2e 2e2e 2021  iers python... !
-000009d0: 0a23 2028 6c61 2064 6572 6e69 c3a8 7265  .# (la derni..re
-000009e0: 206c 6967 6e65 3a20 7072 6f6a 6574 7320   ligne: projets 
-000009f0: 706f 7572 2070 6c75 7320 7461 7264 2e2e  pour plus tard..
-00000a00: 2e29 0a65 7863 6c75 6465 5f64 6f63 733a  .).exclude_docs:
-00000a10: 207c 0a20 202a 2a2f 2a5f 5245 4d2e 6d64   |.  **/*_REM.md
-00000a20: 0a20 202a 2a2f 2a2e 7079 0a20 2021 2f70  .  **/*.py.  !/p
-00000a30: 795f 6c69 6273 2f2a 2e70 790a 0a74 6865  y_libs/*.py..the
-00000a40: 6d65 3a0a 2020 6e61 6d65 3a20 7079 6f64  me:.  name: pyod
-00000a50: 6964 652d 6d6b 646f 6373 2d74 6865 6d65  ide-mkdocs-theme
-00000a60: 0a0a 2320 6665 6174 7572 6573 3a0a 2320  ..# features:.# 
-00000a70: 2020 2d20 6e61 7669 6761 7469 6f6e 2e69    - navigation.i
-00000a80: 6e73 7461 6e74 2020 2020 2020 2320 4e65  nstant      # Ne
-00000a90: 2073 7572 746f 7574 2070 6173 2061 6374   surtout pas act
-00000aa0: 6976 6572 2063 6574 7465 206f 7074 696f  iver cette optio
-00000ab0: 6e20 210a 0a0a 2320 436f 6e66 6967 7572  n !...# Configur
-00000ac0: 6174 696f 6e20 6d69 6e69 6d61 6c65 2070  ation minimale p
-00000ad0: 6f75 7220 6c65 7320 706c 7567 696e 730a  our les plugins.
-00000ae0: 706c 7567 696e 733a 0a20 202d 2061 7765  plugins:.  - awe
-00000af0: 736f 6d65 2d70 6167 6573 3a20 2020 2020  some-pages:     
-00000b00: 2020 2020 2023 2050 6173 2069 6e64 6973       # Pas indis
-00000b10: 7065 6e73 6162 6c65 2c20 6d61 6973 2e2e  pensable, mais..
-00000b20: 2e20 2870 6970 2069 6e73 7461 6c6c 206d  . (pip install m
-00000b30: 6b64 6f63 732d 6177 6573 6f6d 652d 7061  kdocs-awesome-pa
-00000b40: 6765 732d 706c 7567 696e 290a 2020 2020  ges-plugin).    
-00000b50: 2020 636f 6c6c 6170 7365 5f73 696e 676c    collapse_singl
-00000b60: 655f 7061 6765 733a 2074 7275 650a 0a20  e_pages: true.. 
-00000b70: 202d 206d 6174 6572 6961 6c2f 7365 6172   - material/sear
-00000b80: 6368 2020 2020 2020 2020 2023 2021 2152  ch         # !!R
-00000b90: 4551 5549 5321 2120 2f20 4e6f 7461 3a20  EQUIS!! / Nota: 
-00000ba0: 4c65 7320 706c 7567 696e 7320 6465 206d  Les plugins de m
-00000bb0: 6174 6572 6961 6c2d 6d6b 646f 6373 2064  aterial-mkdocs d
-00000bc0: 6f69 7665 6e74 20c3 aa74 7265 2070 72c3  oivent ..tre pr.
-00000bd0: a966 6978 c3a9 7321 0a0a 2020 2d20 7079  .fix..s!..  - py
-00000be0: 6f64 6964 655f 6d61 6372 6f73 2020 2020  odide_macros    
-00000bf0: 2020 2020 2020 2320 2121 5245 5155 4953        # !!REQUIS
-00000c00: 2121 0a20 2020 2020 206f 6e5f 6572 726f  !!.      on_erro
-00000c10: 725f 6661 696c 3a20 7472 7565 2020 2020  r_fail: true    
-00000c20: 2023 2046 6f72 7465 6d65 6e74 2063 6f6e   # Fortement con
-00000c30: 7365 696c 6cc3 a92e 2e2e 0a0a 2320 2d20  seill.......# - 
-00000c40: 6578 636c 7564 652d 7365 6172 6368 3a20  exclude-search: 
-00000c50: 2020 2020 2020 2020 2320 4150 52c3 8853          # APR..S
-00000c60: 206c 6520 706c 7567 696e 2073 6561 7263   le plugin searc
-00000c70: 6820 2870 6970 2069 6e73 7461 6c6c 206d  h (pip install m
-00000c80: 6b64 6f63 732d 6578 636c 7564 652d 7365  kdocs-exclude-se
-00000c90: 6172 6368 290a 2320 2020 2020 6578 636c  arch).#     excl
-00000ca0: 7564 653a 2020 2020 2020 2020 2020 2020  ude:            
-00000cb0: 2020 2320 506f 7572 206c 6573 2066 6963    # Pour les fic
-00000cc0: 6869 6572 7320 696e 636c 7573 2064 616e  hiers inclus dan
-00000cd0: 7320 6c65 2062 7569 6c64 2c20 7175 6520  s le build, que 
-00000ce0: 6c61 2072 6563 6865 7263 6865 206e 6520  la recherche ne 
-00000cf0: 646f 6974 2070 6173 2069 6e64 6578 6572  doit pas indexer
-00000d00: 0a23 2020 2020 2020 202d 2062 6163 5f61  .#       - bac_a
-00000d10: 5f73 6162 6c65 2e6d 640a 0a0a 6d61 726b  _sable.md...mark
-00000d20: 646f 776e 5f65 7874 656e 7369 6f6e 733a  down_extensions:
-00000d30: 0a0a 2020 2320 4578 7465 6e73 696f 6e73  ..  # Extensions
-00000d40: 2069 6e64 6973 7065 6e73 6162 6c65 7320   indispensables 
-00000d50: 706f 7572 206c 6520 7468 c3a8 6d65 3a0a  pour le th..me:.
-00000d60: 2020 2d20 6d64 5f69 6e5f 6874 6d6c 2020    - md_in_html  
-00000d70: 2020 2020 2020 2020 2020 2020 2320 2121              # !!
-00000d80: 5245 5155 4953 2121 0a20 202d 2061 646d  REQUIS!!.  - adm
-00000d90: 6f6e 6974 696f 6e20 2020 2020 2020 2020  onition         
-00000da0: 2020 2020 2023 2021 2152 4551 5549 5321       # !!REQUIS!
-00000db0: 2120 426c 6f63 7320 636f 6c6f 72c3 a973  ! Blocs color..s
-00000dc0: 3a20 2021 2121 2069 6e66 6f20 226d 6120  :  !!! info "ma 
-00000dd0: 7265 6d61 7271 7565 220a 2020 2d20 6174  remarque".  - at
-00000de0: 7472 5f6c 6973 7420 2020 2020 2020 2020  tr_list         
-00000df0: 2020 2020 2020 2320 2121 5245 5155 4953        # !!REQUIS
-00000e00: 2121 2055 6e20 7065 7520 6465 2043 5353  !! Un peu de CSS
-00000e10: 2065 7420 6465 7320 6174 7472 6962 7574   et des attribut
-00000e20: 7320 4854 4d4c 2c20 6578 3a20 7b20 2369  s HTML, ex: { #i
-00000e30: 6420 2e63 6c61 7373 2073 7479 6c65 3d22  d .class style="
-00000e40: 6469 7370 6c61 793a 6e6f 6e65 2220 7d0a  display:none" }.
-00000e50: 2020 2d20 7079 6d64 6f77 6e78 2e64 6574    - pymdownx.det
-00000e60: 6169 6c73 2020 2020 2020 2020 2320 2121  ails        # !!
-00000e70: 5245 5155 4953 2121 2041 646d 6f6e 6974  REQUIS!! Admonit
-00000e80: 696f 6e3a 203f 3f3f 202d 3e20 7065 7576  ion: ??? -> peuv
-00000e90: 656e 7420 7365 2064 c3a9 706c 6965 7220  ent se d..plier 
-00000ea0: 3b20 3f3f 3f2b 202d 3e20 7065 7576 656e  ; ???+ -> peuven
-00000eb0: 7420 7365 2072 6570 6c69 6572 2e0a 2020  t se replier..  
-00000ec0: 2d20 7079 6d64 6f77 6e78 2e65 6d6f 6a69  - pymdownx.emoji
-00000ed0: 3a20 2020 2020 2020 2020 2320 2121 5245  :         # !!RE
-00000ee0: 5155 4953 2121 20c3 896d 6f6a 6973 3a20  QUIS!! ..mojis: 
-00000ef0: 203a 626f 6f6d 3a0a 2020 2020 2020 656d   :boom:.      em
-00000f00: 6f6a 695f 696e 6465 783a 2021 2170 7974  oji_index: !!pyt
-00000f10: 686f 6e2f 6e61 6d65 3a6d 6174 6572 6961  hon/name:materia
-00000f20: 6c2e 6578 7465 6e73 696f 6e73 2e65 6d6f  l.extensions.emo
-00000f30: 6a69 2e74 7765 6d6f 6a69 0a20 2020 2020  ji.twemoji.     
-00000f40: 2065 6d6f 6a69 5f67 656e 6572 6174 6f72   emoji_generator
-00000f50: 3a20 2121 7079 7468 6f6e 2f6e 616d 653a  : !!python/name:
-00000f60: 6d61 7465 7269 616c 2e65 7874 656e 7369  material.extensi
-00000f70: 6f6e 732e 656d 6f6a 692e 746f 5f73 7667  ons.emoji.to_svg
-00000f80: 0a20 202d 2070 796d 646f 776e 782e 6869  .  - pymdownx.hi
-00000f90: 6768 6c69 6768 7420 2020 2020 2023 2021  ghlight      # !
-00000fa0: 2152 4551 5549 5321 2120 436f 6c6f 7261  !REQUIS!! Colora
-00000fb0: 7469 6f6e 2073 796e 7461 7869 7175 6520  tion syntaxique 
-00000fc0: 6475 2063 6f64 650a 2020 2d20 7079 6d64  du code.  - pymd
-00000fd0: 6f77 6e78 2e69 6e6c 696e 6568 696c 6974  ownx.inlinehilit
-00000fe0: 6520 2020 2320 2121 5245 5155 4953 2121  e   # !!REQUIS!!
-00000ff0: 2043 6f6c 6f72 6174 696f 6e20 7379 6e74   Coloration synt
-00001000: 6178 6971 7565 2070 6f75 7220 6c65 7320  axique pour les 
-00001010: 2263 6f64 6520 7370 616e 7322 3a20 6023  "code spans": `#
-00001020: 2170 7974 686f 6e20 2063 6f64 655f 7079  !python  code_py
-00001030: 7468 6f6e 600a 2020 2d20 7079 6d64 6f77  thon`.  - pymdow
-00001040: 6e78 2e73 6e69 7070 6574 733a 2020 2020  nx.snippets:    
-00001050: 2020 2320 2121 5245 5155 4953 2121 2049    # !!REQUIS!! I
-00001060: 6e63 6c75 7369 6f6e 2064 6520 6669 6368  nclusion de fich
-00001070: 6965 7273 2065 7874 6572 6e65 2e0a 2020  iers externe..  
-00001080: 2020 2020 6368 6563 6b5f 7061 7468 733a      check_paths:
-00001090: 2074 7275 6520 2020 2020 2320 466f 7274   true     # Fort
-000010a0: 656d 656e 7420 636f 6e73 6569 6c6c c3a9  ement conseill..
-000010b0: 2e2e 2e0a 2020 2d20 7079 6d64 6f77 6e78  ....  - pymdownx
-000010c0: 2e73 7570 6572 6665 6e63 6573 2020 2020  .superfences    
-000010d0: 2320 2121 5245 5155 4953 2121 0a20 202d  # !!REQUIS!!.  -
-000010e0: 2070 796d 646f 776e 782e 6172 6974 686d   pymdownx.arithm
-000010f0: 6174 6578 3a20 2020 2023 2021 2152 4551  atex:    # !!REQ
-00001100: 5549 5321 2120 506f 7572 204c 6154 6578  UIS!! Pour LaTex
-00001110: 0a20 2020 2020 2067 656e 6572 6963 3a20  .      generic: 
-00001120: 7472 7565 0a20 202d 2070 796d 646f 776e  true.  - pymdown
-00001130: 782e 7374 7269 7068 746d 6c3a 0a20 2020  x.striphtml:.   
-00001140: 2020 2073 7472 6970 5f6a 735f 6f6e 5f61     strip_js_on_a
-00001150: 7474 7269 6275 7465 733a 2066 616c 7365  ttributes: false
-00001160: 2020 2020 2023 2021 2152 4551 5549 5321       # !!REQUIS!
-00001170: 210a 2020 2020 2020 7374 7269 705f 6174  !.      strip_at
-00001180: 7472 6962 7574 6573 3a20 2222 2020 2020  tributes: ""    
-00001190: 2020 2020 2020 2020 2020 2320 2121 5245            # !!RE
-000011a0: 5155 4953 2121 0a0a 0a20 2023 2045 7874  QUIS!!...  # Ext
-000011b0: 656e 7369 6f6e 7320 636f 6e73 6569 6c6c  ensions conseill
-000011c0: c3a9 6573 3a0a 2020 2d20 6d65 7461 0a20  ..es:.  - meta. 
-000011d0: 202d 2061 6262 720a 2020 2d20 6465 665f   - abbr.  - def_
-000011e0: 6c69 7374 2020 2020 2020 2020 2020 2020  list            
-000011f0: 2020 2020 2320 4c65 7320 6c69 7374 6573      # Les listes
-00001200: 2064 6520 64c3 a966 696e 6974 696f 6e2e   de d..finition.
-00001210: 0a20 202d 2066 6f6f 746e 6f74 6573 2020  .  - footnotes  
-00001220: 2020 2020 2020 2020 2020 2020 2023 204e               # N
-00001230: 6f74 6573 5b5e 315d 2064 6520 6261 7320  otes[^1] de bas 
-00001240: 6465 2070 6167 652e 2020 5b5e 315d 3a20  de page.  [^1]: 
-00001250: 6d61 206e 6f74 652e 0a20 202d 2070 796d  ma note..  - pym
-00001260: 646f 776e 782e 6361 7265 7420 2020 2020  downx.caret     
-00001270: 2020 2020 2023 2050 6173 7361 6765 205e       # Passage ^
-00001280: 5e73 6f75 6c69 676e c3a9 5e5e 206f 7520  ^soulign..^^ ou 
-00001290: 656e 205e 6578 706f 7361 6e74 5e2e 0a20  en ^exposant^.. 
-000012a0: 202d 2070 796d 646f 776e 782e 6d61 726b   - pymdownx.mark
-000012b0: 2020 2020 2020 2020 2020 2023 2050 6173             # Pas
-000012c0: 7361 6765 203d 3d73 7572 6c69 676e c3a9  sage ==surlign..
-000012d0: 3d3d 2e0a 2020 2d20 7079 6d64 6f77 6e78  ==..  - pymdownx
-000012e0: 2e74 696c 6465 2020 2020 2020 2020 2020  .tilde          
-000012f0: 2320 5061 7373 6167 6520 7e7e 6261 7272  # Passage ~~barr
-00001300: c3a9 7e7e 206f 7520 656e 207e 696e 6469  ..~~ ou en ~indi
-00001310: 6365 7e2e 0a20 202d 2070 796d 646f 776e  ce~..  - pymdown
-00001320: 782e 7461 736b 6c69 7374 3a20 2020 2020  x.tasklist:     
-00001330: 2023 2043 6173 6573 20c3 a020 636f 6368   # Cases .. coch
-00001340: 6572 2020 2d20 5b20 5d20 2065 7420 2d20  er  - [ ]  et - 
-00001350: 5b78 5d0a 2020 2020 2020 6375 7374 6f6d  [x].      custom
-00001360: 5f63 6865 636b 626f 783a 2066 616c 7365  _checkbox: false
-00001370: 0a20 2020 2020 2063 6c69 636b 6162 6c65  .      clickable
-00001380: 5f63 6865 636b 626f 783a 2074 7275 650a  _checkbox: true.
-00001390: 2020 2d20 7079 6d64 6f77 6e78 2e74 6162    - pymdownx.tab
-000013a0: 6265 643a 2020 2020 2020 2020 2320 566f  bed:        # Vo
-000013b0: 6c65 7473 2067 6c69 7373 616e 7473 3a20  lets glissants: 
-000013c0: 203d 3d3d 2022 4d6f 6e20 766f 6c65 7422   === "Mon volet"
-000013d0: 0a20 2020 2020 2061 6c74 6572 6e61 7465  .      alternate
-000013e0: 5f73 7479 6c65 3a20 7472 7565 2023 204d  _style: true # M
-000013f0: 6569 6c6c 6575 7265 2063 6f6d 7061 7469  eilleure compati
-00001400: 6269 6c69 74c3 a920 706f 7572 206d 6f62  bilit.. pour mob
-00001410: 696c 6573 0a20 2020 2020 2073 6c75 6769  iles.      slugi
-00001420: 6679 3a20 2121 7079 7468 6f6e 2f6f 626a  fy: !!python/obj
-00001430: 6563 742f 6170 706c 793a 7079 6d64 6f77  ect/apply:pymdow
-00001440: 6e78 2e73 6c75 6773 2e73 6c75 6769 6679  nx.slugs.slugify
-00001450: 0a20 2020 2020 2020 206b 7764 733a 0a20  .        kwds:. 
-00001460: 2020 2020 2020 2020 2063 6173 653a 206c           case: l
-00001470: 6f77 6572 0a20 202d 2070 796d 646f 776e  ower.  - pymdown
-00001480: 782e 6b65 7973 2020 2020 2020 2020 2020  x.keys          
-00001490: 2023 2054 6f75 6368 6573 2064 7520 636c   # Touches du cl
-000014a0: 6176 6965 723a 2020 2b2b 6374 726c 2b64  avier:  ++ctrl+d
-000014b0: 2b2b 0a20 202d 2074 6f63 3a0a 2020 2020  ++.  - toc:.    
-000014c0: 2020 746f 635f 6465 7074 683a 2030 2020    toc_depth: 0  
-000014d0: 2020 2020 2020 2020 2320 5369 2076 6f75          # Si vou
-000014e0: 7320 766f 756c 657a 2073 7570 7072 696d  s voulez supprim
-000014f0: 6572 206c 6120 546f 4320 2874 6162 6c65  er la ToC (table
-00001500: 206f 6620 636f 6e74 656e 7429 2064 6520   of content) de 
-00001510: 6c61 2070 6167 650a 0a0a 0a23 2053 6920  la page....# Si 
-00001520: 6d6b 646f 6373 2065 7374 206c 616e 63c3  mkdocs est lanc.
-00001530: a920 656e 206d 6f64 6520 7374 7269 6374  . en mode strict
-00001540: 2028 6d6b 646f 6373 202e 2e2e 202d 2d73   (mkdocs ... --s
-00001550: 7472 6963 7429 2c20 6c65 7320 7761 726e  trict), les warn
-00001560: 696e 6773 206c c3a8 7665 726f 6e74 2075  ings l..veront u
-00001570: 6e65 2065 7272 6575 720a 7661 6c69 6461  ne erreur.valida
-00001580: 7469 6f6e 3a0a 2020 6f6d 6974 7465 645f  tion:.  omitted_
-00001590: 6669 6c65 733a 2077 6172 6e0a 2020 756e  files: warn.  un
-000015a0: 7265 636f 676e 697a 6564 5f6c 696e 6b73  recognized_links
-000015b0: 3a20 7761 726e 0a0a 2727 2729 0a         : warn..''').
+00000040: 205a 696e 656c 6c69 0a23 0a23 2054 6869   Zinelli.#.# Thi
+00000050: 7320 7072 6f67 7261 6d20 6973 2066 7265  s program is fre
+00000060: 6520 736f 6674 7761 7265 3a20 796f 7520  e software: you 
+00000070: 6361 6e20 7265 6469 7374 7269 6275 7465  can redistribute
+00000080: 2069 7420 616e 642f 6f72 206d 6f64 6966   it and/or modif
+00000090: 790a 2320 6974 2075 6e64 6572 2074 6865  y.# it under the
+000000a0: 2074 6572 6d73 206f 6620 7468 6520 474e   terms of the GN
+000000b0: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+000000c0: 204c 6963 656e 7365 2061 7320 7075 626c   License as publ
+000000d0: 6973 6865 6420 6279 0a23 2074 6865 2046  ished by.# the F
+000000e0: 7265 6520 536f 6674 7761 7265 2046 6f75  ree Software Fou
+000000f0: 6e64 6174 696f 6e2c 2065 6974 6865 7220  ndation, either 
+00000100: 7665 7273 696f 6e20 3320 6f66 2074 6865  version 3 of the
+00000110: 204c 6963 656e 7365 2c20 6f72 0a23 2028   License, or.# (
+00000120: 6174 2079 6f75 7220 6f70 7469 6f6e 2920  at your option) 
+00000130: 616e 7920 6c61 7465 7220 7665 7273 696f  any later versio
+00000140: 6e2e 0a23 0a23 2054 6869 7320 7072 6f67  n..#.# This prog
+00000150: 7261 6d20 6973 2064 6973 7472 6962 7574  ram is distribut
+00000160: 6564 2069 6e20 7468 6520 686f 7065 2074  ed in the hope t
+00000170: 6861 7420 6974 2077 696c 6c20 6265 2075  hat it will be u
+00000180: 7365 6675 6c2c 0a23 2062 7574 2057 4954  seful,.# but WIT
+00000190: 484f 5554 2041 4e59 2057 4152 5241 4e54  HOUT ANY WARRANT
+000001a0: 593b 2077 6974 686f 7574 2065 7665 6e20  Y; without even 
+000001b0: 7468 6520 696d 706c 6965 6420 7761 7272  the implied warr
+000001c0: 616e 7479 206f 660a 2320 4d45 5243 4841  anty of.# MERCHA
+000001d0: 4e54 4142 494c 4954 5920 6f72 2046 4954  NTABILITY or FIT
+000001e0: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
+000001f0: 4355 4c41 5220 5055 5250 4f53 452e 0a23  CULAR PURPOSE..#
+00000200: 2053 6565 2074 6865 2047 4e55 2047 656e   See the GNU Gen
+00000210: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
+00000220: 6e73 6520 666f 7220 6d6f 7265 2064 6574  nse for more det
+00000230: 6169 6c73 2e0a 230a 2320 596f 7520 7368  ails..#.# You sh
+00000240: 6f75 6c64 2068 6176 6520 7265 6365 6976  ould have receiv
+00000250: 6564 2061 2063 6f70 7920 6f66 2074 6865  ed a copy of the
+00000260: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
+00000270: 6c69 6320 4c69 6365 6e73 650a 2320 616c  lic License.# al
+00000280: 6f6e 6720 7769 7468 2074 6869 7320 7072  ong with this pr
+00000290: 6f67 7261 6d2e 0a23 2049 6620 6e6f 742c  ogram..# If not,
+000002a0: 2073 6565 203c 6874 7470 733a 2f2f 7777   see <https://ww
+000002b0: 772e 676e 752e 6f72 672f 6c69 6365 6e73  w.gnu.org/licens
+000002c0: 6573 2f3e 2e0a 0a23 2056 6f69 6369 2075  es/>...# Voici u
+000002d0: 6e20 6578 656d 706c 6520 7072 6573 7175  n exemple presqu
+000002e0: 6520 636f 6d70 6c65 7420 6465 2063 6f6e  e complet de con
+000002f0: 6669 6775 7261 7469 6f6e 2070 6f75 7220  figuration pour 
+00000300: 756e 2066 6963 6869 6572 0a23 206d 6b64  un fichier.# mkd
+00000310: 6f63 732e 796d 6c20 7574 696c 6973 616e  ocs.yml utilisan
+00000320: 7420 7079 6f64 6964 652d 6d6b 646f 6373  t pyodide-mkdocs
+00000330: 2d74 6865 6d65 2e0a 0a73 6974 655f 7572  -theme...site_ur
+00000340: 6c3a 2022 7b3e 3e20 4c27 6164 7265 7373  l: "{>> L'adress
+00000350: 6520 6465 2076 6f74 7265 2073 6974 6520  e de votre site 
+00000360: 7765 6220 6963 6920 3c3c 7d22 0a73 6974  web ici <<}".sit
+00000370: 655f 6e61 6d65 3a20 227b 3e3e 2054 6974  e_name: "{>> Tit
+00000380: 7265 2070 6f75 7220 766f 7472 6520 7369  re pour votre si
+00000390: 7465 203c 3c7d 220a 2320 7369 7465 5f64  te <<}".# site_d
+000003a0: 6573 6372 6970 7469 6f6e 3a20 2228 6f70  escription: "(op
+000003b0: 7469 6f6e 6e65 6c29 220a 2320 7265 706f  tionnel)".# repo
+000003c0: 5f75 726c 3a20 2228 6f70 7469 6f6e 6e65  _url: "(optionne
+000003d0: 6c29 220a 2320 6564 6974 5f75 7269 3a20  l)".# edit_uri: 
+000003e0: 2228 6f70 7469 6f6e 6e65 6c29 220a 0a23  "(optionnel)"..#
+000003f0: 2043 6f70 7972 6967 6874 2022 4343 2042   Copyright "CC B
+00000400: 592d 4e43 2d53 4122 0a63 6f70 7972 6967  Y-NC-SA".copyrig
+00000410: 6874 3a20 7c0a 2020 3c70 2078 6d6c 6e73  ht: |.  <p xmlns
+00000420: 3a63 633d 2268 7474 703a 2f2f 6372 6561  :cc="http://crea
+00000430: 7469 7665 636f 6d6d 6f6e 732e 6f72 672f  tivecommons.org/
+00000440: 6e73 2322 0a20 2078 6d6c 6e73 3a64 6374  ns#".  xmlns:dct
+00000450: 3d22 6874 7470 3a2f 2f70 7572 6c2e 6f72  ="http://purl.or
+00000460: 672f 6463 2f74 6572 6d73 2f22 3e50 6172  g/dc/terms/">Par
+00000470: 7461 6765 206f 7520 6164 6170 7461 7469  tage ou adaptati
+00000480: 6f6e 2070 6f73 7369 626c 6520 7365 6c6f  on possible selo
+00000490: 6e20 6c65 7320 636f 6e64 6974 696f 6e73  n les conditions
+000004a0: 2064 6520 6c61 0a20 206c 6963 656e 6365   de la.  licence
+000004b0: 203c 610a 2020 6872 6566 3d22 6874 7470   <a.  href="http
+000004c0: 3a2f 2f63 7265 6174 6976 6563 6f6d 6d6f  ://creativecommo
+000004d0: 6e73 2e6f 7267 2f6c 6963 656e 7365 732f  ns.org/licenses/
+000004e0: 6279 2d6e 632d 7361 2f34 2e30 2f3f 7265  by-nc-sa/4.0/?re
+000004f0: 663d 6368 6f6f 7365 722d 7631 220a 2020  f=chooser-v1".  
+00000500: 7461 7267 6574 3d22 5f62 6c61 6e6b 2220  target="_blank" 
+00000510: 7265 6c3d 226c 6963 656e 7365 206e 6f6f  rel="license noo
+00000520: 7065 6e65 7220 6e6f 7265 6665 7272 6572  pener noreferrer
+00000530: 220a 2020 7374 796c 653d 2264 6973 706c  ".  style="displ
+00000540: 6179 3a69 6e6c 696e 652d 626c 6f63 6b3b  ay:inline-block;
+00000550: 223e 2043 4320 4259 2d4e 432d 5341 2034  "> CC BY-NC-SA 4
+00000560: 2e30 203c 696d 670a 2020 7374 796c 653d  .0 <img.  style=
+00000570: 2268 6569 6768 743a 3232 7078 2169 6d70  "height:22px!imp
+00000580: 6f72 7461 6e74 3b6d 6172 6769 6e2d 6c65  ortant;margin-le
+00000590: 6674 3a33 7078 3b76 6572 7469 6361 6c2d  ft:3px;vertical-
+000005a0: 616c 6967 6e3a 7465 7874 2d62 6f74 746f  align:text-botto
+000005b0: 6d3b 220a 2020 7372 633d 2268 7474 7073  m;".  src="https
+000005c0: 3a2f 2f6d 6972 726f 7273 2e63 7265 6174  ://mirrors.creat
+000005d0: 6976 6563 6f6d 6d6f 6e73 2e6f 7267 2f70  ivecommons.org/p
+000005e0: 7265 7373 6b69 742f 6963 6f6e 732f 6363  resskit/icons/cc
+000005f0: 2e73 7667 3f72 6566 3d63 686f 6f73 6572  .svg?ref=chooser
+00000600: 2d76 3122 3e3c 696d 670a 2020 7374 796c  -v1"><img.  styl
+00000610: 653d 2268 6569 6768 743a 3232 7078 2169  e="height:22px!i
+00000620: 6d70 6f72 7461 6e74 3b6d 6172 6769 6e2d  mportant;margin-
+00000630: 6c65 6674 3a33 7078 3b76 6572 7469 6361  left:3px;vertica
+00000640: 6c2d 616c 6967 6e3a 7465 7874 2d62 6f74  l-align:text-bot
+00000650: 746f 6d3b 220a 2020 7372 633d 2268 7474  tom;".  src="htt
+00000660: 7073 3a2f 2f6d 6972 726f 7273 2e63 7265  ps://mirrors.cre
+00000670: 6174 6976 6563 6f6d 6d6f 6e73 2e6f 7267  ativecommons.org
+00000680: 2f70 7265 7373 6b69 742f 6963 6f6e 732f  /presskit/icons/
+00000690: 6279 2e73 7667 3f72 6566 3d63 686f 6f73  by.svg?ref=choos
+000006a0: 6572 2d76 3122 3e3c 696d 670a 2020 7374  er-v1"><img.  st
+000006b0: 796c 653d 2268 6569 6768 743a 3232 7078  yle="height:22px
+000006c0: 2169 6d70 6f72 7461 6e74 3b6d 6172 6769  !important;margi
+000006d0: 6e2d 6c65 6674 3a33 7078 3b76 6572 7469  n-left:3px;verti
+000006e0: 6361 6c2d 616c 6967 6e3a 7465 7874 2d62  cal-align:text-b
+000006f0: 6f74 746f 6d3b 220a 2020 7372 633d 2268  ottom;".  src="h
+00000700: 7474 7073 3a2f 2f6d 6972 726f 7273 2e63  ttps://mirrors.c
+00000710: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
+00000720: 7267 2f70 7265 7373 6b69 742f 6963 6f6e  rg/presskit/icon
+00000730: 732f 6e63 2e73 7667 3f72 6566 3d63 686f  s/nc.svg?ref=cho
+00000740: 6f73 6572 2d76 3122 3e3c 696d 670a 2020  oser-v1"><img.  
+00000750: 7374 796c 653d 2268 6569 6768 743a 3232  style="height:22
+00000760: 7078 2169 6d70 6f72 7461 6e74 3b6d 6172  px!important;mar
+00000770: 6769 6e2d 6c65 6674 3a33 7078 3b76 6572  gin-left:3px;ver
+00000780: 7469 6361 6c2d 616c 6967 6e3a 7465 7874  tical-align:text
+00000790: 2d62 6f74 746f 6d3b 220a 2020 7372 633d  -bottom;".  src=
+000007a0: 2268 7474 7073 3a2f 2f6d 6972 726f 7273  "https://mirrors
+000007b0: 2e63 7265 6174 6976 6563 6f6d 6d6f 6e73  .creativecommons
+000007c0: 2e6f 7267 2f70 7265 7373 6b69 742f 6963  .org/presskit/ic
+000007d0: 6f6e 732f 7361 2e73 7667 3f72 6566 3d63  ons/sa.svg?ref=c
+000007e0: 686f 6f73 6572 2d76 3122 3e3c 2f61 3e3c  hooser-v1"></a><
+000007f0: 2f70 3e0a 0a0a 646f 6373 5f64 6972 3a20  /p>...docs_dir: 
+00000800: 646f 6373 0a0a 6e61 763a 0a20 202d 2022  docs..nav:.  - "
+00000810: 4163 6375 6569 6c22 3a20 696e 6465 782e  Accueil": index.
+00000820: 6d64 0a23 202d 202e 2e2e 0a0a 2320 506f  md.# - .....# Po
+00000830: 7572 2073 7570 7072 696d 6572 2063 6572  ur supprimer cer
+00000840: 7461 696e 7320 6669 6368 6965 7273 206d  tains fichiers m
+00000850: 6172 6b64 6f77 6e20 6465 206c 6120 6e61  arkdown de la na
+00000860: 7669 6761 7469 6f6e 2028 7061 7474 6572  vigation (patter
+00000870: 6e20 7368 656c 6c29 3a0a 2320 6e6f 745f  n shell):.# not_
+00000880: 696e 5f6e 6176 3a20 7c0a 2320 2020 2a2f  in_nav: |.#   */
+00000890: 2a2a 2f2a 2e6d 640a 0a23 204e c3a9 6365  **/*.md..# N..ce
+000008a0: 7373 6974 6520 6d6b 646f 6373 2031 2e36  ssite mkdocs 1.6
+000008b0: 2b20 706f 7572 2066 6f6e 6374 696f 6e6e  + pour fonctionn
+000008c0: 6572 2063 6f72 7265 6374 656d 656e 742e  er correctement.
+000008d0: 2053 696e 6f6e 2c20 766f 7573 2070 6f75   Sinon, vous pou
+000008e0: 7665 7a20 7574 696c 6973 6572 0a23 206c  vez utiliser.# l
+000008f0: 6520 706c 7567 696e 206d 6b64 6f63 732d  e plugin mkdocs-
+00000900: 6578 636c 7564 6520 c3a0 206c 6120 706c  exclude .. la pl
+00000910: 6163 652e 0a23 204e 6520 7375 7274 6f75  ace..# Ne surtou
+00000920: 7420 7061 7320 6d65 7474 7265 2064 6520  t pas mettre de 
+00000930: 636f 6d6d 656e 7461 6972 6573 2073 7572  commentaires sur
+00000940: 206c 6120 6c69 676e 6520 6427 6578 636c   la ligne d'excl
+00000950: 7573 696f 6e20 6465 7320 6669 6368 6965  usion des fichie
+00000960: 7273 2070 7974 686f 6e2e 2e2e 2021 0a23  rs python... !.#
+00000970: 2028 6578 636c 7572 6520 6c65 7320 6669   (exclure les fi
+00000980: 6368 6965 7273 2070 7974 686f 6e20 6e27  chiers python n'
+00000990: 6166 6665 6374 6520 7061 7320 6c65 7320  affecte pas les 
+000009a0: 2270 7974 686f 6e5f 6c69 6273 2229 0a65  "python_libs").e
+000009b0: 7863 6c75 6465 5f64 6f63 733a 207c 0a20  xclude_docs: |. 
+000009c0: 202a 2a2f 2a5f 5245 4d2e 6d64 0a20 202a   **/*_REM.md.  *
+000009d0: 2a2f 2a2e 7079 0a0a 7468 656d 653a 0a20  */*.py..theme:. 
+000009e0: 206e 616d 653a 2070 796f 6469 6465 2d6d   name: pyodide-m
+000009f0: 6b64 6f63 732d 7468 656d 650a 0a23 2066  kdocs-theme..# f
+00000a00: 6561 7475 7265 733a 0a23 2020 202d 206e  eatures:.#   - n
+00000a10: 6176 6967 6174 696f 6e2e 696e 7374 616e  avigation.instan
+00000a20: 7420 2020 2020 2023 204e 6520 7375 7274  t      # Ne surt
+00000a30: 6f75 7420 7061 7320 6163 7469 7665 7220  out pas activer 
+00000a40: 6365 7474 6520 6f70 7469 6f6e 2021 0a0a  cette option !..
+00000a50: 0a23 2043 6f6e 6669 6775 7261 7469 6f6e  .# Configuration
+00000a60: 206d 696e 696d 616c 6520 706f 7572 206c   minimale pour l
+00000a70: 6573 2070 6c75 6769 6e73 0a70 6c75 6769  es plugins.plugi
+00000a80: 6e73 3a0a 2020 2d20 6177 6573 6f6d 652d  ns:.  - awesome-
+00000a90: 7061 6765 733a 2020 2020 2020 2020 2020  pages:          
+00000aa0: 2320 5061 7320 696e 6469 7370 656e 7361  # Pas indispensa
+00000ab0: 626c 652c 206d 6169 732e 2e2e 2028 7069  ble, mais... (pi
+00000ac0: 7020 696e 7374 616c 6c20 6d6b 646f 6373  p install mkdocs
+00000ad0: 2d61 7765 736f 6d65 2d70 6167 6573 2d70  -awesome-pages-p
+00000ae0: 6c75 6769 6e29 0a20 2020 2020 2063 6f6c  lugin).      col
+00000af0: 6c61 7073 655f 7369 6e67 6c65 5f70 6167  lapse_single_pag
+00000b00: 6573 3a20 7472 7565 0a0a 2020 2d20 6d61  es: true..  - ma
+00000b10: 7465 7269 616c 2f73 6561 7263 6820 2020  terial/search   
+00000b20: 2020 2020 2020 2320 2121 5245 5155 4953        # !!REQUIS
+00000b30: 2121 202f 204e 6f74 613a 204c 6573 2070  !! / Nota: Les p
+00000b40: 6c75 6769 6e73 2064 6520 6d61 7465 7269  lugins de materi
+00000b50: 616c 2d6d 6b64 6f63 7320 646f 6976 656e  al-mkdocs doiven
+00000b60: 7420 c3aa 7472 6520 7072 c3a9 6669 78c3  t ..tre pr..fix.
+00000b70: a973 210a 0a20 202d 2070 796f 6469 6465  .s!..  - pyodide
+00000b80: 5f6d 6163 726f 733a 2020 2020 2020 2020  _macros:        
+00000b90: 2023 2021 2152 4551 5549 5321 210a 2020   # !!REQUIS!!.  
+00000ba0: 2020 2020 6f6e 5f65 7272 6f72 5f66 6169      on_error_fai
+00000bb0: 6c3a 2074 7275 6520 2020 2320 466f 7274  l: true   # Fort
+00000bc0: 656d 656e 7420 636f 6e73 6569 6c6c c3a9  ement conseill..
+00000bd0: 2e2e 2e0a 0a23 202d 2065 7863 6c75 6465  .....# - exclude
+00000be0: 2d73 6561 7263 683a 2020 2020 2020 2020  -search:        
+00000bf0: 2023 2041 5052 c388 5320 6c65 2070 6c75   # APR..S le plu
+00000c00: 6769 6e20 7365 6172 6368 2028 7069 7020  gin search (pip 
+00000c10: 696e 7374 616c 6c20 6d6b 646f 6373 2d65  install mkdocs-e
+00000c20: 7863 6c75 6465 2d73 6561 7263 6829 0a23  xclude-search).#
+00000c30: 2020 2020 2065 7863 6c75 6465 3a20 2020       exclude:   
+00000c40: 2020 2020 2020 2020 2020 2023 2050 6f75             # Pou
+00000c50: 7220 6c65 7320 6669 6368 6965 7273 2069  r les fichiers i
+00000c60: 6e63 6c75 7320 6461 6e73 206c 6520 6275  nclus dans le bu
+00000c70: 696c 642c 2071 7565 206c 6120 7265 6368  ild, que la rech
+00000c80: 6572 6368 6520 6e65 2064 6f69 7420 7061  erche ne doit pa
+00000c90: 7320 696e 6465 7865 720a 2320 2020 2020  s indexer.#     
+00000ca0: 2020 2d20 6261 635f 615f 7361 626c 652e    - bac_a_sable.
+00000cb0: 6d64 0a0a 0a6d 6172 6b64 6f77 6e5f 6578  md...markdown_ex
+00000cc0: 7465 6e73 696f 6e73 3a0a 0a20 2023 2045  tensions:..  # E
+00000cd0: 7874 656e 7369 6f6e 7320 696e 6469 7370  xtensions indisp
+00000ce0: 656e 7361 626c 6573 2070 6f75 7220 6c65  ensables pour le
+00000cf0: 2074 68c3 a86d 653a 0a20 202d 206d 645f   th..me:.  - md_
+00000d00: 696e 5f68 746d 6c20 2020 2020 2020 2020  in_html         
+00000d10: 2020 2020 2023 2021 2152 4551 5549 5321       # !!REQUIS!
+00000d20: 210a 2020 2d20 6164 6d6f 6e69 7469 6f6e  !.  - admonition
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00000d40: 2121 5245 5155 4953 2121 2042 6c6f 6373  !!REQUIS!! Blocs
+00000d50: 2063 6f6c 6f72 c3a9 733a 2020 2121 2120   color..s:  !!! 
+00000d60: 696e 666f 2022 6d61 2072 656d 6172 7175  info "ma remarqu
+00000d70: 6522 0a20 202d 2061 7474 725f 6c69 7374  e".  - attr_list
+00000d80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00000d90: 2021 2152 4551 5549 5321 2120 556e 2070   !!REQUIS!! Un p
+00000da0: 6575 2064 6520 4353 5320 6574 2064 6573  eu de CSS et des
+00000db0: 2061 7474 7269 6275 7473 2048 544d 4c2c   attributs HTML,
+00000dc0: 2065 783a 207b 2023 6964 202e 636c 6173   ex: { #id .clas
+00000dd0: 7320 7374 796c 653d 2264 6973 706c 6179  s style="display
+00000de0: 3a6e 6f6e 6522 207d 0a20 202d 2070 796d  :none" }.  - pym
+00000df0: 646f 776e 782e 6465 7461 696c 7320 2020  downx.details   
+00000e00: 2020 2020 2023 2021 2152 4551 5549 5321       # !!REQUIS!
+00000e10: 2120 4164 6d6f 6e69 7469 6f6e 3a20 3f3f  ! Admonition: ??
+00000e20: 3f20 2d3e 2070 6575 7665 6e74 2073 6520  ? -> peuvent se 
+00000e30: 64c3 a970 6c69 6572 203b 203f 3f3f 2b20  d..plier ; ???+ 
+00000e40: 2d3e 2070 6575 7665 6e74 2073 6520 7265  -> peuvent se re
+00000e50: 706c 6965 722e 0a20 202d 2070 796d 646f  plier..  - pymdo
+00000e60: 776e 782e 656d 6f6a 693a 2020 2020 2020  wnx.emoji:      
+00000e70: 2020 2023 2021 2152 4551 5549 5321 2120     # !!REQUIS!! 
+00000e80: c389 6d6f 6a69 733a 2020 3a62 6f6f 6d3a  ..mojis:  :boom:
+00000e90: 2028 7574 696c 6973 c3a9 2064 616e 7320   (utilis.. dans 
+00000ea0: 6c65 7320 7465 726d 696e 6175 7829 0a20  les terminaux). 
+00000eb0: 2020 2020 2065 6d6f 6a69 5f69 6e64 6578       emoji_index
+00000ec0: 3a20 2121 7079 7468 6f6e 2f6e 616d 653a  : !!python/name:
+00000ed0: 6d61 7465 7269 616c 2e65 7874 656e 7369  material.extensi
+00000ee0: 6f6e 732e 656d 6f6a 692e 7477 656d 6f6a  ons.emoji.twemoj
+00000ef0: 690a 2020 2020 2020 656d 6f6a 695f 6765  i.      emoji_ge
+00000f00: 6e65 7261 746f 723a 2021 2170 7974 686f  nerator: !!pytho
+00000f10: 6e2f 6e61 6d65 3a6d 6174 6572 6961 6c2e  n/name:material.
+00000f20: 6578 7465 6e73 696f 6e73 2e65 6d6f 6a69  extensions.emoji
+00000f30: 2e74 6f5f 7376 670a 2020 2d20 7079 6d64  .to_svg.  - pymd
+00000f40: 6f77 6e78 2e68 6967 686c 6967 6874 2020  ownx.highlight  
+00000f50: 2020 2020 2320 2121 5245 5155 4953 2121      # !!REQUIS!!
+00000f60: 2043 6f6c 6f72 6174 696f 6e20 7379 6e74   Coloration synt
+00000f70: 6178 6971 7565 2064 7520 636f 6465 0a20  axique du code. 
+00000f80: 202d 2070 796d 646f 776e 782e 696e 6c69   - pymdownx.inli
+00000f90: 6e65 6869 6c69 7465 2020 2023 2021 2152  nehilite   # !!R
+00000fa0: 4551 5549 5321 2120 436f 6c6f 7261 7469  EQUIS!! Colorati
+00000fb0: 6f6e 2073 796e 7461 7869 7175 6520 706f  on syntaxique po
+00000fc0: 7572 206c 6573 2022 636f 6465 2073 7061  ur les "code spa
+00000fd0: 6e73 223a 2060 2321 7079 7468 6f6e 2020  ns": `#!python  
+00000fe0: 636f 6465 5f70 7974 686f 6e60 0a20 202d  code_python`.  -
+00000ff0: 2070 796d 646f 776e 782e 736e 6970 7065   pymdownx.snippe
+00001000: 7473 3a20 2020 2020 2023 2021 2152 4551  ts:      # !!REQ
+00001010: 5549 5321 2120 496e 636c 7573 696f 6e20  UIS!! Inclusion 
+00001020: 6465 2066 6963 6869 6572 7320 6578 7465  de fichiers exte
+00001030: 726e 652e 0a20 2020 2020 2063 6865 636b  rne..      check
+00001040: 5f70 6174 6873 3a20 7472 7565 2020 2020  _paths: true    
+00001050: 2023 2046 6f72 7465 6d65 6e74 2063 6f6e   # Fortement con
+00001060: 7365 696c 6cc3 a920 210a 2020 2d20 7079  seill.. !.  - py
+00001070: 6d64 6f77 6e78 2e73 7570 6572 6665 6e63  mdownx.superfenc
+00001080: 6573 2020 2020 2320 2121 5245 5155 4953  es    # !!REQUIS
+00001090: 2121 0a20 202d 2070 796d 646f 776e 782e  !!.  - pymdownx.
+000010a0: 6172 6974 686d 6174 6578 3a20 2020 2023  arithmatex:    #
+000010b0: 2021 2152 4551 5549 5321 2120 506f 7572   !!REQUIS!! Pour
+000010c0: 204c 6154 6578 0a20 2020 2020 2067 656e   LaTex.      gen
+000010d0: 6572 6963 3a20 7472 7565 0a20 202d 2070  eric: true.  - p
+000010e0: 796d 646f 776e 782e 7374 7269 7068 746d  ymdownx.striphtm
+000010f0: 6c3a 0a20 2020 2020 2073 7472 6970 5f6a  l:.      strip_j
+00001100: 735f 6f6e 5f61 7474 7269 6275 7465 733a  s_on_attributes:
+00001110: 2066 616c 7365 2020 2020 2023 2021 2152   false     # !!R
+00001120: 4551 5549 5321 210a 2020 2020 2020 7374  EQUIS!!.      st
+00001130: 7269 705f 6174 7472 6962 7574 6573 3a20  rip_attributes: 
+00001140: 2222 2020 2020 2020 2020 2020 2020 2020  ""              
+00001150: 2320 2121 5245 5155 4953 2121 0a0a 0a20  # !!REQUIS!!... 
+00001160: 2023 2045 7874 656e 7369 6f6e 7320 636f   # Extensions co
+00001170: 6e73 6569 6c6c c3a9 6573 3a0a 2020 2d20  nseill..es:.  - 
+00001180: 6d65 7461 0a20 202d 2061 6262 720a 2020  meta.  - abbr.  
+00001190: 2d20 6465 665f 6c69 7374 2020 2020 2020  - def_list      
+000011a0: 2020 2020 2020 2020 2020 2320 4c65 7320            # Les 
+000011b0: 6c69 7374 6573 2064 6520 64c3 a966 696e  listes de d..fin
+000011c0: 6974 696f 6e2e 0a20 202d 2066 6f6f 746e  ition..  - footn
+000011d0: 6f74 6573 2020 2020 2020 2020 2020 2020  otes            
+000011e0: 2020 2023 204e 6f74 6573 5b5e 315d 2064     # Notes[^1] d
+000011f0: 6520 6261 7320 6465 2070 6167 652e 2020  e bas de page.  
+00001200: 5b5e 315d 3a20 6d61 206e 6f74 652e 0a20  [^1]: ma note.. 
+00001210: 202d 2070 796d 646f 776e 782e 6361 7265   - pymdownx.care
+00001220: 7420 2020 2020 2020 2020 2023 2050 6173  t          # Pas
+00001230: 7361 6765 205e 5e73 6f75 6c69 676e c3a9  sage ^^soulign..
+00001240: 5e5e 206f 7520 656e 205e 6578 706f 7361  ^^ ou en ^exposa
+00001250: 6e74 5e2e 0a20 202d 2070 796d 646f 776e  nt^..  - pymdown
+00001260: 782e 6d61 726b 2020 2020 2020 2020 2020  x.mark          
+00001270: 2023 2050 6173 7361 6765 203d 3d73 7572   # Passage ==sur
+00001280: 6c69 676e c3a9 3d3d 2e0a 2020 2d20 7079  lign..==..  - py
+00001290: 6d64 6f77 6e78 2e74 696c 6465 2020 2020  mdownx.tilde    
+000012a0: 2020 2020 2020 2320 5061 7373 6167 6520        # Passage 
+000012b0: 7e7e 6261 7272 c3a9 7e7e 206f 7520 656e  ~~barr..~~ ou en
+000012c0: 207e 696e 6469 6365 7e2e 0a20 202d 2070   ~indice~..  - p
+000012d0: 796d 646f 776e 782e 6b65 7973 2020 2020  ymdownx.keys    
+000012e0: 2020 2020 2020 2023 2054 6f75 6368 6573         # Touches
+000012f0: 2064 7520 636c 6176 6965 723a 2020 2b2b   du clavier:  ++
+00001300: 6374 726c 2b64 2b2b 0a20 202d 2070 796d  ctrl+d++.  - pym
+00001310: 646f 776e 782e 7461 736b 6c69 7374 3a20  downx.tasklist: 
+00001320: 2020 2020 2023 2043 6173 6573 20c3 a020       # Cases .. 
+00001330: 636f 6368 6572 2020 2d20 5b20 5d20 2065  cocher  - [ ]  e
+00001340: 7420 2d20 5b78 5d0a 2020 2020 2020 6375  t - [x].      cu
+00001350: 7374 6f6d 5f63 6865 636b 626f 783a 2066  stom_checkbox: f
+00001360: 616c 7365 0a20 2020 2020 2063 6c69 636b  alse.      click
+00001370: 6162 6c65 5f63 6865 636b 626f 783a 2074  able_checkbox: t
+00001380: 7275 650a 2020 2d20 7079 6d64 6f77 6e78  rue.  - pymdownx
+00001390: 2e74 6162 6265 643a 2020 2020 2020 2020  .tabbed:        
+000013a0: 2320 566f 6c65 7473 2067 6c69 7373 616e  # Volets glissan
+000013b0: 7473 3a20 203d 3d3d 2022 4d6f 6e20 766f  ts:  === "Mon vo
+000013c0: 6c65 7422 0a20 2020 2020 2061 6c74 6572  let".      alter
+000013d0: 6e61 7465 5f73 7479 6c65 3a20 7472 7565  nate_style: true
+000013e0: 2023 204d 6569 6c6c 6575 7265 2063 6f6d   # Meilleure com
+000013f0: 7061 7469 6269 6c69 74c3 a920 706f 7572  patibilit.. pour
+00001400: 206d 6f62 696c 6573 0a20 2020 2020 2073   mobiles.      s
+00001410: 6c75 6769 6679 3a20 2121 7079 7468 6f6e  lugify: !!python
+00001420: 2f6f 626a 6563 742f 6170 706c 793a 7079  /object/apply:py
+00001430: 6d64 6f77 6e78 2e73 6c75 6773 2e73 6c75  mdownx.slugs.slu
+00001440: 6769 6679 0a20 2020 2020 2020 206b 7764  gify.        kwd
+00001450: 733a 0a20 2020 2020 2020 2020 2063 6173  s:.          cas
+00001460: 653a 206c 6f77 6572 0a20 2023 202d 2074  e: lower.  # - t
+00001470: 6f63 3a0a 2020 2320 2020 2020 746f 635f  oc:.  #     toc_
+00001480: 6465 7074 683a 2030 2020 2020 2020 2020  depth: 0        
+00001490: 2320 5369 2076 6f75 7320 766f 756c 657a  # Si vous voulez
+000014a0: 2073 7570 7072 696d 6572 206c 6120 546f   supprimer la To
+000014b0: 4320 2874 6162 6c65 206f 6620 636f 6e74  C (table of cont
+000014c0: 656e 7429 2064 6520 6c61 2070 6167 650a  ent) de la page.
+000014d0: 0a0a 0a23 2053 6920 6d6b 646f 6373 2065  ...# Si mkdocs e
+000014e0: 7374 206c 616e 63c3 a920 656e 206d 6f64  st lanc.. en mod
+000014f0: 6520 7374 7269 6374 2028 6d6b 646f 6373  e strict (mkdocs
+00001500: 202e 2e2e 202d 2d73 7472 6963 7429 2c20   ... --strict), 
+00001510: 6c65 7320 7761 726e 696e 6773 206c c3a8  les warnings l..
+00001520: 7665 726f 6e74 2075 6e65 2065 7272 6575  veront une erreu
+00001530: 720a 7661 6c69 6461 7469 6f6e 3a0a 2020  r.validation:.  
+00001540: 6f6d 6974 7465 645f 6669 6c65 733a 2077  omitted_files: w
+00001550: 6172 6e0a 2020 756e 7265 636f 676e 697a  arn.  unrecogniz
+00001560: 6564 5f6c 696e 6b73 3a20 7761 726e 0a    ed_links: warn.
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -20,89 +20,114 @@
 
 /*
 NOTE: Globals defined somewhere else:
 
     * The "ace" variable is defined in the ace library. Everything using it must be called after
       the libs step insertions.
 */
-
+const SqBs = {
+    '[': '&lsqb;',
+    ']': '&rsqb;',
+    '&lsqb;': '[',
+    '&rsqb;': ']',
+    L: '&lsqb;',
+    R: '&rsqb;',
+}
 
 const CONFIG = {
 
     /*
     The following values are passed from python to JS through the main.html,
     once this script got loaded */
-    //CONFIG_DUMP
+    //JS_CONFIG_DUMP
+    baseUrl: null,
+    buttonIconsDirectory: null,
+    deactivateStdoutForSecrets: null,
+    decreaseAttemptsOnUserCodeFailure: null,
+    defaultHeightIdeTerm: null,
+    defaultHeightIsolatedTerm: null,
+    defaultIdeHeightLines: null,
+    docsDir: null,
+    encryptCorrectionsAndRems: null,
+    forbidCorrAnd_REMsWithInfiniteAttempts: null,
+    forbidHiddenCorrAnd_REMsWithoutSecrets: null,
+    forbidSecretsWithoutCorrOr_REMs: null,
+    hide: null,
     ignoreMacrosPluginDiffs: null,
-    skipPyMdPathsNamesValidation: null,
+    j2BlockEndString: null,
+    j2BlockStartString: null,
+    j2VariableEndString: null,
+    j2VariableStartString: null,
     loadYamlEncoding: null,
     macrosWithIndents: null,
-    bypassIndentErrors: null,
-    encryptCorrectionsAndRems: null,
-    forbidSecretsWithoutCorrOr_REMs: null,
-    forbidHiddenCorrAnd_REMsWithoutSecrets: null,
-    forbidCorrAnd_REMsWithInfiniteAttempts: null,
-    showAssertionCodeOnFailedTest: null,
     maxAttemptsBeforeCorrAvailable: null,
-    decreaseAttemptsOnUserCodeFailure: null,
-    defaultIdeHeightLines: null,
-    deactivateStdoutForSecrets: null,
-    showOnlyAssertionErrorsForSecrets: null,
-    hide: null,
     multi: null,
-    shuffle: null,
-    scriptsUrl: null,
-    siteRoot: null,
-    docsDir: null,
+    pmtUrl: null,
+    pythonLibs: null,
     repoUrl: null,
+    scriptsUrl: null,
+    showAssertionCodeOnFailedTest: null,
+    showOnlyAssertionErrorsForSecrets: null,
+    shuffle: null,
+    siteDir: null,
     siteName: null,
+    siteRoot: null,
     siteUrl: null,
-    buttonIconsDirectory: null,
-    baseUrl: null,
-    pmtUrl: null,
+    skipPyMdPathsNamesValidation: null,
+    stdoutCutOff: null,
     version: null,
     lang: {
-        comments: null,
         tests: null,
+        comments: null,
+        feedback: null,
+        wrapTerm: null,
         runScript: null,
-        successMsg: null,
         installStart: null,
         installDone: null,
-        feedback: null,
+        successMsg: null,
         successHead: null,
-        successHeadExtra: null,
-        failHead: null,
         successTail: null,
+        failHead: null,
         revealCorr: null,
         revealJoin: null,
         revealRem: null,
+        successHeadExtra: null,
         failTail: null,
         titleCorr: null,
         titleRem: null,
         corr: null,
         rem: null,
+        pyBtn: null,
         play: null,
         check: null,
         download: null,
         upload: null,
         restart: null,
         save: null,
         attemptsLeft: null,
         qcmTitle: null,
         qcmMaskTip: null,
         qcmCheckTip: null,
         qcmRedoTip: null,
         tipTrash: null
     },
-    //CONFIG_DUMP
+    //JS_CONFIG_DUMP
 
 
-    ideProp: {}, // filled dynamically
+    /**Constant, to archive the terminals at runtime.
+     *   - Will be garbage collected on page change or reload.
+     *   - Warning if navigation.instant gets restored !!
+     * */
+    terms: {}, // debugging purpose
+    editors: {}, // debugging purpose
+    objs: {}, // debugging purpose
 
     onDoneEvent: 'unload', // unused, so far...
+    pyodideDelay: 500,
+    LZW: '\x1e',
 
     // Various UI elements identifiers
     element: {
         searchBlock: "div.md-search",
         searchBtnsLeft: "#search-btns-left",
         searchBtnsRight: "#search-btns-right",
         dayNight: "form.md-header__option",
@@ -118,37 +143,30 @@
     // Auto subscriber tracking:
     subscriptionReady: {},
     subscriptionsTries: {},
 
     loggerOptions: {}, // jsLogger debugging config/activations
 
 
-    /**Constant, to archive the terminals at runtime.
-     *   - Will be garbage collected on page change or reload.
-     *   - Warning if navigation.instant gets restored !!
-     * */
-    terms: {}, // All registered terminals
-
-
-    currentScroll: undefined, // [x,y]
-
 
     // (defined in the securedPagesData-libs.js file)
     // JS <-> python property names tracker
 
-
     cutFeedback: true,
+    joinTerminalLines: false,
 
-    COMMENTED_PATTERN: /(^\s*)(\S)(.?)/,
     // HDR_TOKEN_PATTERN:   /#\s*-[\s-]*HDR\s*-[\s-]*#/i,           // not used anymore
-
+    COMMENTED_PATTERN: /(^\s*)(\S)(.?)/,
     MODULE_REG: /File "<(env|post|exec|console)>", line (\d+)($|, in (?!await_fut))/,
     TRACE_REG: /  File "<(env|post|exec|console)>"/,
     TRACE_NUM_LINE: /File "<(?:env|post|exec|console)>", line (\d+)/,
 
+    ESCAPE_SQ_B: /\[|\]/g,
+    UNESCAPE_SQ_B: new RegExp(`[${ SqBs.L }${ SqBs.R }]`, 'g'),
+
     ACE_COLOR_THEME: {
         customTheme: undefined,
         customThemeDefaultKey: "",
         aceStyle: undefined,
     },
 
 
@@ -172,16 +190,16 @@
 
 
     MSG: {
         successEmojis: ['🔥', '✨', '🌠', '✅', '🥇', '🎖'],
 
         promptStart: ">>> ",
         promptWait: "... ",
-        leftSafeSqbr: "&lsqb;",
-        rightSafeSqbr: "&rsqb;",
+        leftSafeSqbr: SqBs.L,
+        rightSafeSqbr: SqBs.R,
         exclusionMarker: "FORBIDDEN",
         bigFail: "\nIf You see this, there is a bug either in the website code, or in the way " +
             "this exercice is configured.\nPlease contact the webmaster with information " +
             "about what You were doing when this happened!\n\nDon't forget to check the " +
             "content of the console (F12) and possibly make a screenshot of any message " +
             "there, to help debugging.",
     },
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -13,49 +13,76 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
+
+
 /**Decorator like factory function, managing the global pyodide lock.
  * If a call is done while pyodide is locked, it is delayed until the lock is available.
  * */
-var withPyodideAsyncLock = (function() {
+var withPyodideAsyncLock = (_ => {
 
-    /**Everything is run async but single threaded, so a global lock can be added, using a simple
-     * boolean flag...
-     * */
+    /* Everything is run async but single threaded, so a global lock can be added, using
+     * a simple simple boolean flag, declared inside a closure to avoid a user messing
+     * with the variable... */
     let pyodideLocked = false
 
-    return function(asyncCallback, name = "") {
+    return function(name, asyncCallback) {
         const logName = asyncCallback.name || name
 
         const wrapper = async function(...args) {
+            await waitForPyodideReady()
+
             jsLogger("[LOCK?] -", logName, pyodideLocked)
             while (pyodideLocked) {
                 await sleep(100)
             }
             jsLogger("[LOCK ACQUIRE] -", logName)
             pyodideLocked = true
             let ret;
             try {
                 ret = await asyncCallback.apply(this, args)
+            } catch (e) {
+                console.log(e) // Always keep that, otherwise errors in JS are just swallowed
+                // (impossible to rethrow them, not sure why... async probably)
             } finally {
                 pyodideLocked = false
                 jsLogger("[LOCK RELEASE] -", logName)
             }
             return ret
         }
         return wrapper
     }
+
 })()
 
 
 
+/**Allow to delay the executions of various functions, until the pyodide environment
+ * is done loading.
+ * */
+async function waitForPyodideReady() {
+
+    const maxWaitingTime = 20 // in seconds
+    const attempts = 80
+    const step_ms = Math.round(1000 * maxWaitingTime / attempts)
+
+    let counter = 0
+    while (!globalThis.pyodideIsReady) {
+        await sleep(step_ms);
+        if (++counter == attempts) {
+            throw new Error(`Couldn't access to pyodide environment in time (${maxWaitingTime}s)`)
+        }
+    }
+}
+
+
 
 
 /**Auto-subscription routine to document changes.
  * If the subscription is not possible yet (readyForSubscription[waitOn] is falsy), try again
  * @delay later until it works.
  *
  * @waitId :  Property to observe in readyForSubscription global object.Also used as subscription
@@ -81,15 +108,14 @@
         waitFor
     } = {
         delay: 50,
         now: false,
         waitFor: null,
         ...options
     }
-
     now = now && !waitFor // has to wait if waitFor is used
     CONFIG.subscriptionReady[waitId] = now
 
     const checkReady = !waitFor ? () => null :
         typeof(waitFor) == 'string' ? () => {
             CONFIG.subscriptionReady[waitId] = $(waitFor).length > 0
         } :
@@ -109,15 +135,22 @@
                 throw new Error(`Impossible to subscribe to ${ waitId } in time: too many tries.`)
             }
             CONFIG.subscriptionsTries[waitId] = nTries
             setTimeout(autoSubscribe, delay)
 
         } else {
             jsLogger('[Subscribing] -', waitId)
-            const subscript = document$.subscribe(callback)
+            const wrapper = function() {
+                try {
+                    callback()
+                } catch (e) {
+                    console.log(e)
+                }
+            }
+            const subscript = document$.subscribe(wrapper)
             document.addEventListener(CONFIG.onDoneEvent, function() {
                 jsLogger("[Unsubscribing] -", waitId)
                 subscript.unsubscribe()
             })
         }
     }
 
@@ -156,24 +189,24 @@
 let warning = (content) => richTextFormat(content, "", "orange");
 let stress = (content) => richTextFormat(content, "b");
 let info = (content) => richTextFormat(content, "i", "grey");
 let italic = (content) => richTextFormat(content, "i");
 let success = (content) => richTextFormat(content, "ib", "green");
 let failure = (content) => richTextFormat(content, "ib", "orange");
 
+
+// Update CONFIG strings on the fly:
 'successMsg runScript installStart installDone'
 .split(' ').forEach(
     prop => CONFIG.lang[prop].msg = info(CONFIG.lang[prop].msg)
 )
 
 
 
 
-
-
 /**Takes a string and cut the "middle chunk" of them if it is considered too long (length > 1750),
  * shortening it in the following way:
  *   - keep the 500 first and 300 last chars
  *   - replace the middle with a message
  * */
 function textShortener(text) {
     if (CONFIG.cutFeedback && text.length > CONFIG.feedbackShortener.limit) {
@@ -218,14 +251,86 @@
         throw new Error("Cannot pick from an empty array")
     }
     const i = Math.random() * arr.length | 0
     return arr[i]
 }
 
 
+/**Applique c ^ key à chaque nombre de text
+ * (Nota: 43960 = 0b1010101010101010)
+ * */
+const decrypt_string = (text, key = 43960) => {
+    if (!CONFIG.encryptCorrectionsAndRems) return text
+    return text.split('.').map(c => String.fromCodePoint(key ^ +c)).join('')
+}
+
+const ALPHA = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!#$%&'()*+,-./:;=?@^_`{|}~ "
+const TOME_B = [...ALPHA].reduce((o, c, i) => (o[c] = i, o), {})
+
+const unBase = s => [...s].reduce((v, c) => v * ALPHA.length + TOME_B[c], 0)
+
+/**@txt: CONFIG.LZW separated lines, with:
+ *      1. dot separated unicode char codes
+ *      2. regular alpha
+ *      3. compressed data, size 2
+ *      4. ..., size 3,
+ *      5. ...
+ */
+const decompressLZW = (compressed) => {
+
+    const [bigs, smalls, ...chunks] = compressed.trim().split(CONFIG.LZW)
+    const tome = [
+        [...'><'],
+        bigs == '.' ? [] : bigs.slice(1) // no initial dot
+        .split('.')
+        .map(n => String.fromCodePoint(+n)),
+        [...smalls],
+    ].flat()
+
+    let txt = [],
+        size = 1,
+        out = []
+    chunks.forEach(chunk => {
+        size++
+        if (chunk.length % size) {
+            throw new Error(`Wrong chunk: size=${size}, length=${chunk.length}`)
+        }
+        for (let i = 0; i < chunk.length; i += size) {
+            txt.push(unBase(chunk.slice(i, i + size)))
+        }
+    })
+    txt.forEach((iBase, i) => {
+        const s = tome[iBase]
+        const fresh = s + (tome[txt[i + 1]] || s)[0]
+        out.push(s)
+        tome.push(fresh)
+    })
+    return out.join('')
+}
+
+const escapeSqBrackets = msg => {
+    return msg.replace(CONFIG.ESCAPE_SQ_B, c => SqBs[c])
+}
 
+const unEscapeSqBrackets = msg => {
+    return msg.replace(CONFIG.UNESCAPE_SQ_B, c => SqBs[c])
+}
 
 /**Async sleep (time given in milliseconds / must be awaited by the caller)
  * */
 function sleep(ms = 0) {
     return new Promise((resolve) => setTimeout(resolve, ms));
+}
+
+
+
+// Code issued from https://stackoverflow.com/questions/5379120/get-the-highlighted-selected-text
+function getSelectionText() {
+    let text = "";
+    if (window.getSelection) {
+        text = window.getSelection().toString();
+
+    } else if (document.selection && document.selection.type != "Control") {
+        text = document.selection.createRange().text;
+    }
+    return text;
 }
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
 
     AroundSearch: false,
     Feature: false,
     HourGlass: false,
     LOCK: false,
     MathJax: false,
     Paint_ACEs: false,
-    QCM: true,
+    QCM: false,
     Scroll: false,
     SetupIDEs: false,
     SetupLoneTerms: false,
     StdoutController: false,
     Subscribing: false,
     Terminal: false,
     TrashCan: false,
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # pyodide-mkdocs-theme
 # Copyleft GNU GPLv3 🄯 2024 Frédéric Zinelli
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.
+# If not, see <https://www.gnu.org/licenses/>.
+
+# pyodide-mkdocs-theme
+# Copyleft GNU GPLv3 🄯 2024 Frédéric Zinelli
 # 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 # 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css`

 * *Files 10% similar despite different names*

```diff
@@ -91,16 +91,16 @@
 }
 
 /* Fix the active line color in dark mode */
 .ace-tomorrow-night-bright .ace_marker-layer .ace_active-line {
   background: #42424242;
 }
 
-/* overloading ace gutters to hide them behind the navbar */
-.ace_gutter {
+/* overloading ace gutters and sliders to hide them behind the navbar or header */
+.ace_gutter, .ace_scrollbar {
   z-index: 1;
 }
 
 .ace_gutter > .ace_layer {
   color: var(--main-theme);
   background-color: var(--gutter-theme);
   border-right: solid 1px var(--main-theme);
@@ -126,18 +126,33 @@
 
 /*
 ------------------------
   Le compteur d'essais
 ------------------------
 */
 
+.ide_buttons_div_wrapper {
+  display: grid;
+  grid-template-columns: max-content auto;
+}
+
+.compteur_wrapper {
+  justify-self: end;
+  width: 100%;
+  display: grid;
+}
+
 .py_mk_ide .compteur {
+  justify-self: end;
+  position: absolute;
   float: right;
   color: var(--main-theme);
-  font-size: 1.2em
+  font-size: 1.2em;
+  z-index: -1;
+  width: max-content;
 }
 
 .py_mk_ide .compteur_txt {
   font-size: 0.8em
 }
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -16,228 +16,231 @@
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
 
 
 
-/**Prepare the runtime python environment:
- *  - Save the current code in the editor to LocaleStorage
- *  - Refresh the basic functionalities
- *  - Refresh any HDR content in the environment
- *  - Refresh any exclusion logistic, by defining extra functions in the environment
- *  - Returns the modified code, with the active terminal
- */
-async function setupRuntimeAndTerminal(editorName) {
-
-    // Extract the user's full code (possibly with public tests):
-    let aceCode = await ace.edit(editorName).getSession().getValue();
-
-    // save before anything else, in case an error occur somewhere...
-    _save(editorName, aceCode)
-    storeUserCodeInPython(aceCode)
-
-
-    // Build the default configuration options to use to run the user's code:
-    const options = buildOptionsForPyodideRun(editorName)
-    const terminal = await setupOrGetTerminalAndPyEnv("term_" + editorName, true);
-
-    terminal.pause() // Pause is to avoid ">>>" showing up during executions
-    terminal.clear() // Erase previous content
-    terminal.echo(CONFIG.lang.runScript.msg) // tell the user it started to run
-    await sleep() // Make sure the change is noticeable
+class _TerminalHandler extends PyodideSectionsRunner {
 
-    const isOk = await runEnvironmentAsync(editorName, options, terminal, 'env')
+    constructor(id) {
+        super(id)
+        this.terminal = null
+        this.termEnabled = false
+    }
+
+    addResizer() {
+        // Add resize listener (throttled):
+        const topDiv = this.terminal.closest(".py_mk_wrapper")
+        window.addEventListener('resize', _.throttle(_ => {
+            const wWrapper = topDiv.width()
+            if (wWrapper != this.terminal.width()) {
+                this.terminal.width(wWrapper)
+            }
+        }, 50, {
+            leading: false,
+            trailing: true
+        }))
 
-    return [aceCode, terminal, options, isOk]
-}
-
-
-
-/**Actions performed once all the running code steps have been completed.
- *
- * This function MUST be always executed, whatever happened before, even for JS errors,
- * otherwise the terminal would stay locked. So its call must be in a try/finally clause.
- *
- * @terminal :   the currently "active" (paused) terminal.
- * @stdErr :     message that got already displayed in the terminal, or empty string id no error.
- * @successMsg : only used for validation tests. If they succeeded, this string won't be empty.
- * */
-async function tearDownRuntimeAndTerminal(editorName, options, terminal, stdErr, finalMsg = "") {
-    jsLogger("[Teardown] -", JSON.stringify(stdErr))
-
-    await runEnvironmentAsync(editorName, options, terminal, 'post')
-
-    if (!stdErr || finalMsg) {
-        terminal.echo(finalMsg || CONFIG.lang.successMsg.msg)
     }
-    globalTearDown(terminal)
-}
-
 
+    addEventToRunOnce(target, event, cbk, withLock = false) {
+        let clickHandler = async _ => {
+            target.off(event, clickHandler)
+            cbk()
+        }
+        if (withLock) {
+            clickHandler = withPyodideAsyncLock('term_' + event, clickHandler)
+        }
+        target.on('click', clickHandler)
+    }
 
-function storeUserCodeInPython(code) {
-    // The double quotes are all escaped to make sure no multiline string will cause troubles
-    const escapedCode = code.replace(/"/g, '\\"')
-    pyodide.runPython(`__builtins__.__USER_CODE__ = """${ escapedCode }"""`)
-}
 
+    /**Build a jQuery terminal and bind it to the underlying pyodide runtime.
+     *
+     * WARNING:  If this is an IdeEditorHandler, this.id is the id of the editor div, not
+     *           the id of the terminal div ! (hence the use of the termId argument)
+     * */
+    build(termId = null) {
+        if (!termId) termId = this.id
+        const jqTermId = '#' + termId
+
+        jsLogger("[Terminal] - build " + jqTermId)
+
+        const commandsCbk = this.getAsyncPythonExecutor()
+        const termOptions = {
+            greetings: "", // cancel terminal banner (welcome message),
+            completionEscape: false,
+            prompt: CONFIG.MSG.promptStart,
+            outputLimit: CONFIG.stdoutCutOff,
+            enabled: false, // GET RID OF THE DAMN AUTO-SCROLL!!!!!!
+            // wrap: getWrapTerms(),          // Also deactivate colors... FUCK THIS!
+            keymap: this.getTerminalBindings(),
+            completion: function(command, callback) {
+                callback(pyFuncs.pyconsole.complete(command).toJs()[0]); // autocompletion
+            },
+            onBlur: function() {}, // Allow to leave the textarea, focus-wise.
+            // DO NOT PUT ANY CODE INSIDE THIS !!
+        }
 
+        this.terminal = $(jqTermId).terminal(commandsCbk, termOptions)
+        if (CONFIG._devMode) CONFIG.terms[termId] = this.terminal
 
-/**Extract the content of the an environment code for the given editorName, and run its content
- * into pyodide environment.
- * */
-async function runEnvironmentAsync(editorName, options, terminal, name) {
-    const prop = `${name}Content`
-
-    let gotErr, stdErr = ''
-    setupStdIO()
-    try {
-        const content = securedExtraction(editorName, CONFIG.ideProp[prop])
-        if (content) {
-            // make sure packages are installed
-            await installAndImportMissingModules(content, options, terminal)
-
-            // run env/post content
-            await pyodide.runPythonAsync(content, {
-                filename: `<${name}>`
-            })
-        }
+        // Since terminal are created deactivated, add an EventListener for click to reactivate
+        // them (once only: unsubscribe the listener on click. Note: no original click event)
+        // Using the async lock so that the user cannot resume a terminal while it's running
+        // (could occur on first click/run).
+        this.addEventToRunOnce(this.terminal, 'click', _ => {
+            if (this.termEnabled) return;
+            this.terminal.focus(true).enable()
+            this.termEnabled = true
+        }, true)
+        this.prefillTermIfAllowed()
 
-        // If an error occurred, give feedback in the console, with stdout teardown on the way,
-        // then stop everything :
-    } catch (err) {
-        gotErr = err;
-        [stdErr, isAssertErr] = generateErrorLog(err, "", false, false)
-    } finally {
-        let someMsg = getFullStdIO() + stdErr
-        if (someMsg) terminal.echo(someMsg)
-    }
-    if (gotErr) {
-        globalTearDown(terminal) // May occur in env section!
-        if (isAssertErr) {
-            return false
-        }
-        throw gotErr // Reraise, stopping executions if error
+        super.build() // nothing done so far, but for consistency...
     }
-    return true
-}
 
 
-/**Generic teardown operations UNRELATED to pyodide (hence, JS or DOM related).
- * */
-function globalTearDown(terminal) {
-    terminal.resume()
-}
 
 
+    /**Hook returning the configuration for terminal keyboard shortcuts bindings.
+     * To override in child classes when needed.
+     *
+     * Handled here: transfer KeyInterrupt from DOM to python runtime (note: actually
+     * useless as long as no worker used!).
+     * */
+    getTerminalBindings() {
+        return ({
+            "CTRL+C": async (e) => {
+                const txt = getSelectionText()
 
+                // Skip if some text is selected (=copy!)
+                if (!txt) {
+                    let currentCmd = this.terminal.get_command();
+                    pyFuncs.clear_console(); // Looks like it does nothing...? :/
+                    this.terminal.echo(CONFIG.MSG.promptStart + currentCmd);
+                    this.terminal.echo(error("KeyboardInterrupt"));
+                    this.terminal.set_command("");
+                    this.terminal.set_prompt(CONFIG.MSG.promptStart);
 
+                } else if (CONFIG.joinTerminalLines) {
+                    // If not activated, rely on the original clipboard event, so that the user still can
+                    // copy content if the browser complains with this functionality.
+                    e.preventDefault()
+                    e.stopPropagation()
+                    await navigator.clipboard.writeText(txt.replace(/\n/g, ''))
+                }
+            }
+        })
+    }
 
-/**Applique c ^ key à chaque nombre de text
- * (Nota: 43960 = 0b1010101010101010)
- * */
-const decrypt_string = (text, key = 43960) => {
-    if (!CONFIG.encryptCorrectionsAndRems) return text
-    return text.split('.').map(c => String.fromCodePoint(key ^ +c)).join('')
+    getAsyncPythonExecutor() {
+        throw new Error('Should be overridden in the child class.')
+    }
 }
 
 
 
 
 
 
 
 
-function getAttemptsLeft(editorName) {
-    return securedExtraction(editorName, CONFIG.ideProp.attemptsLeft)
-}
-
-
 
+class TerminalRunner extends _TerminalHandler {
 
-function updateIdeCounter(editorName) {
-
-    let nAttempts = getAttemptsLeft(editorName) - 1
-    securedUpdate(editorName, "attempts_left", nAttempts)
-    const encrypted = securedExtraction(editorName, CONFIG.ideProp.encrypted)
-
-    // Update the GUI counter if needed
-    if (Number.isFinite(nAttempts) && nAttempts >= 0 && encrypted) {
-        const cntElement = document.getElementById("compteur_" + editorName)
-        cntElement.textContent = nAttempts
+    prefillTermIfAllowed() {
+        if (this.prefillTerm) this.terminal.set_command(this.prefillTerm)
     }
-    return nAttempts
-}
 
 
 
-/**Reveal the solution+rem if still encrypted and either success or no attempts left
- * */
-function unhideSolutionAndRem(editorName, nAttemptsLeft = Infinity, success = true) {
-
-    let encrypted = securedExtraction(editorName, CONFIG.ideProp.encrypted)
-    let something = securedExtraction(editorName, CONFIG.ideProp.corrRemMask)
-
-    if (something && encrypted && (success || nAttemptsLeft < 1)) {
-        const sol_div = document.getElementById("solution_" + editorName)
-        const corr_content = decrypt_string(sol_div.innerHTML)
-        sol_div.innerHTML = corr_content
-        sol_div.classList = []
-        mathJaxUpdate() // Enforce formatting, if ever...
-        securedUpdate(editorName, 'encrypted', false) // Forbid coming back here
-        return true
+    /**When a terminal is available, display stdout and errors if any
+     * */
+    giveFeedback(stdout, stdErr = "", _) {
+        if (stdErr) stdErr = error(stdErr)
+        const msg = (stdout + stdErr).trim()
+        if (msg) this.terminal.echo(msg)
+        return msg
     }
-    return false
-}
-
-
 
 
+    globalTearDown() {
+        this.terminal.resume()
+        super.globalTearDown()
+    }
 
-/**Build an additional final message to add after an error message (which has already been
- * displayed in the terminal.
- * */
-function enhanceFailureMsg(editorName, _stdErr) {
-    let out = getSolRemTxt(editorName, false)
-    return out
-}
 
+    /**Generate the async-locked callback used to run commands typed into the terminal.
+     *
+     * WARNING: USE `super.[...]` !
+     *
+     * Using super calls, because one only wants the setup specific to terminal here, while "this"
+     * could be an IdeRunner object. Ine that case, this.setupRuntime would run the setup for the
+     * code in the editor, and not the command typed in the terminal.
+     * This also way work with TerminalRunners, because the generic setupRuntime is _NOT_ on the
+     * TerminalRunner class, but actually on the PythonSectionRunner one.
+     *
+     * For the very same kind of reasons, the `options` used cannot be the ones returned as usual
+     * by this.runPythonCodeWithOptions, because the terminal commands are run async, so store
+     * locally the needed version.
+     */
+    getAsyncPythonExecutor() {
+        const commandsBuffer = []
 
+        return withPyodideAsyncLock('terminal', async (command) => {
 
-/**Build the full success message
- * */
-function buildSuccessMessage(editorName) {
-    const emo = choice(CONFIG.MSG.successEmojis)
-    let info = getSolRemTxt(editorName, true)
-    return `${ success(CONFIG.lang.successHead.msg) } ${ emo } ${ CONFIG.lang.successHeadExtra.msg }${ info }`
-}
+            commandsBuffer.push(command)
+            this.storeUserCodeInPython('__USER_CMD__', commandsBuffer.join('\n'))
+            this.terminal.pause()
 
+            let outcome
+            try {
+                outcome = await super.setupRuntime()
+                /* HAS to be done before the pyconsole.push, otherwise, because of async loop
+                   scheduling, the environment is setup AFTER the user command has been run...
+                   Because of this, need the commandBuffer to update the __USER_CMD__ variable, and
+                   _also_ because of this, the env section will also run on incomplete commands...
+                */
 
+                // multiline commands should be split (useful when pasting)
+                for (let c of command.split("\n")) {
 
-/**Build the message for the terminal, announcing that correction and remarks becoming available.
- * */
-function getSolRemTxt(editorName, isSuccess) {
-    const CorrRemMask = securedExtraction(editorName, CONFIG.ideProp.corrRemMask)
-    if (!CorrRemMask) return ""
+                    let future = pyFuncs.pyconsole.push(c);
 
-    const msg = []
-    if (isSuccess) msg.push("\n" + CONFIG.lang.successTail.msg)
-    else msg.push(failure(CONFIG.lang.failHead.msg))
+                    // set the beginning of the next line in the terminal:
+                    const isIncompleteExpr = future.syntax_check == "incomplete"
+                    const headLine = isIncompleteExpr ? CONFIG.MSG.promptWait : CONFIG.MSG.promptStart
+                    this.terminal.set_prompt(headLine);
 
-    const sentence = []
-    if (CorrRemMask & 1) sentence.push(CONFIG.lang.revealCorr.msg)
-    if (CorrRemMask == 3) sentence.push(CONFIG.lang.revealJoin.msg)
-    if (CorrRemMask & 2) sentence.push(CONFIG.lang.revealRem.msg)
+                    switch (future.syntax_check) {
+                        case "complete":
+                            try {
+                                outcome.options.runCodeAsync = async _ => {
+                                    await pyFuncs.await_fut(future)
+                                }
+                                if (!outcome.stdErr) await this.runPythonCodeWithOptions(command, outcome.options)
+                            } finally {
+                                commandsBuffer.length = 0
+                                future.destroy() // to destroy only if it got awaited first
+                                await sleep() // Enforce GUI update, going through the next tick
+                            }
+                        case "incomplete":
+                            continue // complete also goes there...
 
-    if (!isSuccess) {
-        if (sentence.length) sentence[0] = _.capitalize(sentence[0])
+                        case "syntax-error":
+                            commandsBuffer.length = 0
+                            this.terminal.error(future.formatted_error.trimEnd());
+                            continue
+                        default:
+                            commandsBuffer.length = 0
+                            throw new Error(`Unexpected state ${future.syntax_check}`);
+                    }
+                }
 
-        if (CorrRemMask & 2) sentence.push(CONFIG.lang.failTail.plural)
-        else if (CorrRemMask) sentence.push(CONFIG.lang.failTail.msg)
+            } finally {
+                super.teardownRuntime(outcome.options) // Will Release the terminal to the user
+                this.storeUserCodeInPython('__USER_CMD__', "")
+            }
+        })
     }
-
-    msg.push(...sentence)
-    msg[msg.length - 1] += "."
-
-    return msg.join(' ')
 }
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -14,456 +14,419 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
 
+class PyodideSectionsRunner {
 
-/**Given an editorName, automatically build the default options to pass as argument to the
- * runPythonCodeWithOptions function.
- *
- * The content of the config optional argument will override any basic option, except for
- * the packagesAliases object, where the config.packagesAliases entries will be added.
- *
- * @returns: an options object, described as follow:
- *     @options :
- *          .autoLogAssert:   (boolean) If true, will automatically add the code of a failing
- *                            assertion as its message if it doesn't have one already.
- *          .excluded:        (String[]) Instructions to exclude at runtime.
- *          .excludedMethods: (String[]) Methods calls to exclude at runtime (string containment).
- *          .packagesAliases: (Record<string,string>) mapping of imports that should be aliased
- *                            automatically for the user, if they try to import them.
- *          .recLimit:        (number) recursion depth (or -1 if not used)
- *          .runCodeAsync:    async python code runner.
- *          .withStdOut:      (boolean) Display the content of the stdOut or not.
- *          .whiteList:       (Array of strings) list of modules to import before the code
- *                            restrictions are put in place for the user's code.
- *
- * WARNING: If the editorName argument isn't given or is falsy, the fields excluded, whiteList
- *          and recLimit are not included.
- * */
-const buildOptionsForPyodideRun = (editorName = '', config = {}) => {
-    const options = {
-        autoLogAssert: true, // default for the PUBLIC tests...
-        excluded: [],
-        excludedMethods: [],
-        recLimit: -1,
-        runCodeAsync: async (code) => pyodide.runPython(code),
-        withStdOut: true, // default for the PUBLIC tests...
-        whiteList: [],
-    }
-    if (editorName) {
-        OPTIONS_TO_EXTRACT.forEach(js_prop => {
-            options[js_prop] = securedExtraction(editorName, CONFIG.ideProp[js_prop])
-        })
+    no_undefined = prop => v => {
+        if (v !== undefined) return v
+        throw new Error(`Undefined is not allow: ${this.constructor.name}.${prop}.`)
     }
-    return {
-        ...options,
-        ...config,
-        packagesAliases: {
-            // turtle: "pyo_js_turtle",         // this never got finished => unusable.
-            ...config.packagesAliases || {}
-        },
-    }
-}
-
-const OPTIONS_TO_EXTRACT = [
-    'excluded',
-    'excludedMethods',
-    'whiteList',
-    'recLimit',
-]
-
-
 
+    //JS_CONFIG_DUMP
+    get attemptsLeft() {
+        return this.no_undefined('attemptsLeft')(this.data.attempts_left)
+    }
+    get autoLogAssert() {
+        return this.no_undefined('autoLogAssert')(this.data.auto_log_assert)
+    }
+    get corrRemsMask() {
+        return this.no_undefined('corrRemsMask')(this.data.corr_rems_mask)
+    }
+    get envContent() {
+        return this.no_undefined('envContent')(this.data.env_content)
+    }
+    get excluded() {
+        return this.no_undefined('excluded')(this.data.excluded)
+    }
+    get excludedMethods() {
+        return this.no_undefined('excludedMethods')(this.data.excluded_methods)
+    }
+    get hasCheckBtn() {
+        return this.no_undefined('hasCheckBtn')(this.data.has_check_btn)
+    }
+    get postContent() {
+        return this.no_undefined('postContent')(this.data.post_content)
+    }
+    get prefillTerm() {
+        return this.no_undefined('prefillTerm')(this.data.prefill_term)
+    }
+    get publicTests() {
+        return this.no_undefined('publicTests')(this.data.public_tests)
+    }
+    get pyName() {
+        return this.no_undefined('pyName')(this.data.py_name)
+    }
+    get recLimit() {
+        return this.no_undefined('recLimit')(this.data.rec_limit)
+    }
+    get secretTests() {
+        return this.no_undefined('secretTests')(this.data.secret_tests)
+    }
+    get userContent() {
+        return this.no_undefined('userContent')(this.data.user_content)
+    }
+    get whiteList() {
+        return this.no_undefined('whiteList')(this.data.white_list)
+    }
+    //JS_CONFIG_DUMP
 
+    constructor(id) {
+        this.id = id
+        this.decompressPagesIfNeeded()
+        this.data = PAGE_IDES_CONFIG[id]
+        if (CONFIG._devMode)
+            CONFIG.objs[this.id] = this
+        else {
+            delete PAGE_IDES_CONFIG[id]
+        }
+    }
 
-/**Special JS Error: methods calls exclusions are tested from the JS runtime, instead of pyodide.
- * So, JS has to throw a special error that will mimic ("enough"...) the pattern of pyodide errors
- * and hance, will be considered legit errors.
- */
-class PythonError extends Error {
-    toString() {
-        return "Python" + super.toString()
-    }
-}
-
-
+    decompressPagesIfNeeded() {
+        if (typeof(PAGE_IDES_CONFIG) != 'string') return;
+        const decompressed = decompressLZW(PAGE_IDES_CONFIG)
+        PAGE_IDES_CONFIG = JSON.parse(
+            decompressed, (key, val) => key == 'attempts_left' && val == "Infinity" ? Infinity : val
+        )
+    }
 
 
+    build() {} // For inheritance consistency
 
-/**Takes a code as argument, and run it in the pyodide environment, using various options:
- *
- * @throws: Any JS runtime Error, if something went very wrong... (python errors are swallowed
- *          and just printed in the terminal)
- * @returns: The stdErr formatted string message that got printed in the terminal, or empty
- *           string if no error.
- *           Note that the message is displayed in the console already, so this is only a
- *           "marker" to propagate some logic in other parts of the application.
- *
- * NOTE:
- *    - Pyodide itself is using eval, so replacing globally the builtin will cause a lot of
- *      troubles and just won't work.
- *    - This function doesn't take in charge the pyodide environment setup, (preparation,
- *      rebuilding the setup, ...).
- *    - On the other hand it DOES take in charge installation of missing modules/packages.
- */
-async function runPythonCodeWithOptions(code, terminal, options, isPublicRun) {
-
-    try {
-        // Do first the methods exclusions check, to gain some time (avoids loading modules if
-        // the error would show up anyway after loading them)
-        const nope = options.excludedMethods.filter(methodCall => code.includes(methodCall))
-        if (nope.length) {
-            const plural = nope.length > 1 ? "s" : ""
-            const nopes = nope.map(s => s.slice(1)).join(', ')
-            const msg = `${ CONFIG.MSG.exclusionMarker } method${plural}: ${ nopes }`
-            throw new PythonError(msg)
-        }
 
-        // Detect possible user imports and install the packages to allow their imports:
-        await installAndImportMissingModules(code, options, terminal)
+    /**Actions to perform when the current code in the editor has been extracted,
+     * before anything is run.
+     * */
+    getCurrentEditorCode() {
+        return ""
+    }
 
-    } catch (err) {
-        const [strErr, _] = generateErrorLog(err, code, false, !isPublicRun)
-        terminal.echo(strErr)
-        return strErr
-    }
-
-    const withExclusions = options.excluded.length > 0 || options.recLimit > 0
-
-    // Setup stdout capture. WARNING: this must always be done even if it's not shown to the user.
-    // If not done, a previous execution might have close the StringIO and if ever the user prints
-    // something, it would result in an error without that:
-    setupStdIO()
-
-    // Setup code/imports exclusions if any (later id better)
-    if (withExclusions) setupExclusions(options.excluded, options.recLimit)
-
-    let stdErr = "",
-        stdOut = "",
-        delayedErr
-    try {
-        await options.runCodeAsync(code)
-    } catch (err) {
-        // Since generateErrorLog might run python code, the exclusions must be removed _before_
-        // the function is called, so store the error for later use.
-        delayedErr = err
-
-    } finally {
-        // Teardown steps must always occur, whatever happened (even for JS errors), hence in a
-        // finally close, and they also must be protected against failure, so in their own
-        // try/catch/finally construct:
-        try {
-            if (withExclusions) restoreOriginalFunctions(options.excluded)
 
-            // Now only, compute the error message if needed.
-            if (delayedErr) {
-                ;
-                [stdErr, _] = generateErrorLog(delayedErr, code, options.autoLogAssert, !isPublicRun)
-            }
+    /**Store code or command in the python runtime.
+     * */
+    storeUserCodeInPython(varName, code) {
+        // The double quotes are all escaped to make sure no multiline string will cause troubles
+        const escapedCode = code.replace(/"/g, '\\"')
+        pyodide.runPython(`__builtins__.${ varName } = """${ escapedCode }"""`)
+    }
 
-            // Always extract the stdout and close the buffer (avoid memory leaks)
-            let captured = getFullStdIO()
+    globalTearDown() {}
 
-            // Send stdout feedback to the user only if allowed:
-            if (options.withStdOut) {
-                stdOut = textShortener(captured)
-            }
 
-        } catch (err) {
-            // This second catch is there so that the user can see the JS error in the terminal.
-            // (Note: maybe I should actually throw them again...?)
-            ;
-            [stdErr, _] = generateErrorLog(err, code, true, false)
 
-        } finally {
-            const someMsg = stdOut + stdErr
-            if (someMsg) {
-                terminal.echo(someMsg);
-            }
-            return stdErr
+    /**Runners without any terminal won't ever give feedback, unless it's a critical error.
+     * In that case, a window alert will be used, so that it doesn't go unnoticed
+     *
+     * @returns: the concatenation of stdout and stdErr (useful in some places...).
+     * */
+    giveFeedback(stdout, stdErr = "", forEnv = false) {
+        if (forEnv && stdErr) {
+            // Format back any escaped square brackets, because window.alert is not in the DOM...
+            const msg = unEscapeSqBrackets(stdErr)
+            window.alert(msg)
         }
+        return stdout + stdErr
     }
-}
 
 
-/*
-------------------------------------------------------------------
-                       Imports logistic
-------------------------------------------------------------------
-*/
 
 
-/**Explore the user's code to find missing modules to install. If some are found, load micropip
- * (if not done yet), then install all the missing modules.
- * Also import all the packages present in options.whiteList.
- *
- * @code : the user's code
- * @options :Same as `runPythonCodeWithOptions`
- * */
-const installAndImportMissingModules = async function(code, options, terminal) {
-
-    const pkgReplacements = options.packagesAliases
-    const whiteList = options.whiteList
-
-    // Things to import whatever happens:
-    const preImport = whiteList.map(name => 'import ' + name)
-
-    const wantedModules = getUserImportedModules(code)
-    const installedModules = getAvailablePackages()
-    const missing = wantedModules.filter(
-        name => !installedModules.includes(name) && !options.excluded.includes(name)
-    )
-
-    if (missing.length) {
-        terminal.echo(CONFIG.lang.installStart.msg)
-
-        await pyodide.loadPackage("micropip");
-        let micropip = pyodide.pyimport("micropip");
-
-        for (let name of missing) {
-            if (name in pkgReplacements) {
-                preImport.push(`import ${ pkgReplacements[name] } as ${ name }`)
-                name = pkgReplacements[name]
-            }
-            jsLogger("[Micropip] - Install", name)
-            await micropip.install(name);
+
+    /**Given an editorName, automatically build the default options to pass as argument to the
+     * runPythonCodeWithOptions function.
+     *
+     * The content of the config optional argument will override any basic option, except for
+     * the packagesAliases object, where the config.packagesAliases entries will be added.
+     *
+     * @returns: an options object, described as follow:
+     *     @options :
+     *          .autoLogAssert:   (boolean) If true, will automatically add the code of a failing
+     *                            assertion as its message if it doesn't have one already.
+     *          .excluded:        (String[]) Instructions to exclude at runtime.
+     *          .excludedMethods: (String[]) Methods calls to exclude at runtime (string containment).
+     *          .isPublic:        (boolean) Define if the executions are for public or secret tests.
+     *          .packagesAliases: (Record<string,string>) mapping of imports that should be aliased
+     *                            automatically for the user, if they try to import them.
+     *          .recLimit:        (number) recursion depth (or -1 if not used)
+     *          .runCodeAsync:    async python code runner.
+     *          .withStdOut:      (boolean) Display the content of the stdOut or not.
+     *          .whiteList:       (Array of strings) list of modules to import before the code
+     *                            restrictions are put in place for the user's code.
+     *
+     * WARNING: If the editorName argument isn't given or is falsy, the fields excluded, whiteList
+     *          and recLimit are not included.
+     * */
+    buildOptionsForPyodideRun(config = {}) {
+        return {
+            autoLogAssert: true, // default for the PUBLIC tests...
+            excluded: this.excluded,
+            excludedMethods: this.excludedMethods,
+            isPublic: true,
+            recLimit: this.recLimit,
+            runCodeAsync: async (code) => pyodide.runPython(code),
+            whiteList: this.whiteList,
+            withStdOut: true, // default for the PUBLIC tests...
+            ...config,
+            packagesAliases: {
+                // turtle: "pyo_js_turtle",         // this never got finished => unusable.
+                ...config.packagesAliases || {}
+            },
         }
-        terminal.echo(CONFIG.lang.installDone.msg)
     }
 
-    // Import everything that is needed (either because module aliasing or because the code
-    // restrictions would forbid it later):
-    pyodide.runPython(preImport.join('\n'))
-}
 
 
 
-/**Rely on pyodide to analyze the code content and find the imports the user is trying to use.
- * */
-const getUserImportedModules = (code) => {
-    return pyodide.runPython(`
-    def _hack():
-        from pyodide.code import find_imports
-        __builtins__.imported_modules = find_imports(${JSON.stringify(code)})
-    _hack()
-    del _hack
-    __builtins__.imported_modules
-    `);
-}
-
-
-/**Extract all the packages names currently available in pyodide.
- * */
-const getAvailablePackages = () => {
-    return pyodide.runPython(`
-    def _hack():
-        import sys
-        __builtins__.loaded_modules = " ".join(sys.modules.keys())
-    _hack()
-    del _hack
-    __builtins__.loaded_modules
-    `).split(' ')
-}
 
+    /**Extract the content of an environment code, and run its content into pyodide environment.
+     *    - Stdout will be visible if an interface is available.
+     *    - StdErr will be visible if an interface is available, and if none, an alert will be
+     *      used (because environment code should never fail...)
+     * */
+    async runEnvironmentAsync(options, name) {
+        const prop = `${name}Content`
+        const content = this[prop].trim()
+
+        let stdErr = '',
+            isAssertErr = false
+        setupStdIO()
+        try {
+            if (content) {
+                // make sure packages are installed
+                await this.installAndImportMissingModules(content, options)
+
+                // run env/post content
+                await pyodide.runPythonAsync(content, {
+                    filename: `<${name}>`
+                })
+            }
+
+            // If an error occurred, give feedback in the console, with stdout teardown on the way,
+            // then stop everything :
+        } catch (err) {
+            ;
+            [stdErr, isAssertErr] = generateErrorLog(err, "", false)
+        } finally {
+            this.giveFeedback(getFullStdIO(), stdErr, true)
+        }
+        return [stdErr, isAssertErr]
+    }
 
 
 
-/*
-------------------------------------------------------------------
-        Manage python standard out redirection in terminal
-------------------------------------------------------------------
-*/
 
 
-/**Use a StringIO stdout, so that the full content can be extracted later
- * */
-const setupStdIO = _ => pyodide.runPython(`
-    def _hack():
-        import sys, io
-        sys.stdout = io.StringIO()
-    _hack()
-    del _hack
-`)
-
-const getFullStdIO = _ => escapeSquareBrackets(pyodide.runPython(`
-    def _hack():
-        import sys
-        __builtins__._stdout = sys.stdout.getvalue()
-        sys.stdout.close()
-
-    _hack()
-    del _hack
-    __builtins__._stdout
-`) || '')
+    /**Explore the user's code to find missing modules to install. If some are found, load micropip
+     * (if not done yet), then install all the missing modules.
+     * Also import all the packages present in options.whiteList.
+     *
+     * @code : the python code to run.
+     * @options :Same as `buildOptionsForPyodideRun`.
+     * */
+    async installAndImportMissingModules(code, options) {
 
 
+        const installedModules = getAvailablePackages()
+        const wantedModules = getUserImportedModules(code)
 
+        const needPyLibs = wantedModules.filter(
+            name => CONFIG.pythonLibs.has(name) && !installedModules.has(name)
+        )
+        const missing = wantedModules.filter(
+            name => !installedModules.has(name) && !CONFIG.pythonLibs.has(name) &&
+            !options.excluded.includes(name)
+        )
 
-/*
-------------------------------------------------------------------
-                      Manage code exclusions
-------------------------------------------------------------------
-*/
+        const pkgReplacements = options.packagesAliases
+        const whiteList = options.whiteList.filter(name => !installedModules.has(name))
+        missing.push(...whiteList)
+
+        // Things to import whatever happens:
+        const preImport = whiteList.map(name => 'import ' + name)
+
+        if (missing.length || needPyLibs.length) {
+            this.giveFeedback(CONFIG.lang.installStart.msg)
+
+            for (const lib of needPyLibs) {
+                try {
+                    const archive = `${ CONFIG.baseUrl }/${ lib }.zip`
+                    const zipResponse = await fetch(archive)
+                    const zipBinary = await zipResponse.arrayBuffer()
+                    pyodide.unpackArchive(zipBinary, "zip", {
+                        extractDir: lib
+                    })
+                } catch (_) {}
+            }
 
+            if (missing.length) {
+                await pyodide.loadPackage("micropip");
+                let micropip = pyodide.pyimport("micropip");
+
+                for (let name of missing) {
+                    if (name in pkgReplacements) {
+                        preImport.push(`import ${ pkgReplacements[name] } as ${ name }`)
+                        name = pkgReplacements[name]
+                    }
+                    jsLogger("[Micropip] - Install", name)
+                    await micropip.install(name);
+                }
+            }
 
+            this.giveFeedback(CONFIG.lang.installDone.msg)
+        }
 
-/**Put in place code exclusions. Are handled:
- *   - builtin function calls
- *   - imports
- *   - method calls (done through a simple string check in the code, in runPythonCodeWithOptions)
- *
- *
- * ## RATIONALS:
- *
- * To forbid the use of some functions or packages, replace them in the global scope by "functions"
- * that look "more or less the same", but will raise an error when called, or when used in the
- * wrong way (imports).
- *
- *
- * ## PROBLEMS:
- *
- * 1. Pyodide itself uses various functions to run python code:
- *      - eval is used in pyodide.runPython
- *      - reversed and/or min and/or max may be used when building a stacktrace when an error is
- *        thrown in python
- * 2. This forbids to replace the __builtins__ versions of those functions (see about imports)
- * 3. but the __main__ script is run separately of pyodide actual "python runtime".
- *
- *
- * ## SOLUTION FOR BUILTINS FUNCTIONS:
- *
- * - Redeclare forbidden things in the global scope, through `globals()`, using an object that will
- *   systematically throw an ExclusionError when it's called.
- * - Since those are in the global scope, they are visible through `dir()`, so add some make up on
- *   those, using a class that redefines its __qualname__ and __repr__, so that it's less obvious
- *   they are the anti-cheats (it will still remain obvious for those who know enough, but if they
- *   can find about that, they probably could solve the problem the right way anyway).
- * - The (hidden) function `__move_forward__('builtin_name')` can be used in the tests to get back the
- *   original builtin. If used, it must be done inside a closure, so that the original builtin
- *   doesn't override the "Raiser" in the global scope (see below).
- * - Pyodide runtime won't see those globals, so it is not affected in any way. Only the user's or
- *   tester's codes are.
- * - Since the hacked version are available to the user in the global runtime, they could just
- *   delete them to get back the access to the original  __builtins__ version. To limit this risk,
- *   an extra check is done after the user's code has been run, verifying that the hacked function
- *    is still defined in the global scope, and that it's still the original Raiser instance.
- *
- *
- * ## SOLUTION FOR IMPORTS
- *
- * The main problem about `import` is that it actually go directly through `__builtins__`, using
- * `__import__`. So in that case, there is no other choice than hacking directly the __builtins__,
- * and then put it back in place when not useful anymore.
- *
- *
- * ## RECURSION LIMIT
- *
- * The sys module function is directly hacked, then put back in place: meaning, the function
- * setrecursionlimit is replaced at user's runtime with a Raiser object.
- *
- * */
-const setupExclusions = (excluded, recLimit) => {
-    // Store None in the __builtins___ dict for things that aren't builtin functions, aka, names
-    // of forbidden module.
-
-    /** WARNING!
-     *  Keep in mind that the code of the Raiser instances will run "in context".
-     *  This means it will be subject to existing exclusions, so it must never use a function that
-     *  could be forbidden. Possibly...
-     *  Force this reason, copies of all the builtins used in the Raiser code are stored locally,
-     *  to be sure the Raiser won't use Raiser instances... XD
-     * */
-    const code = `
-    def _hack():
+        // Import everything that is needed (either because module aliasing or because the code
+        // restrictions would forbid it later):
+        if (preImport.length) {
+            pyodide.runPython(preImport.join('\n'))
+        }
+    }
 
-        class Raiser:
-            __name__ = __qualname__ = 'function'
 
-            def __init__(self, key):  self.key = key
 
-            def __repr__(self): return f"<built-in function {self.key}>"
 
-            def __call__(self, *a, **kw):
-                key = self.key
 
-                head = a and base_isinstance(a[0],base_str) and a[0].split(".")[0]
 
-                is_forbidden = (
-                    key != '__import__' or
-                    key == '__import__' and head in dct
-                )
-                if is_forbidden:
-                    that = key if key!='__import__' else head
-                    raise ExclusionError.throw(that)
+    /** 1. Refresh the features defined in pyodide environment, in case the user messed with them
+     *     (accidentally or not).
+     *  2. Then run the content of the `env` section.
+     *
+     * @returns: [options, isOk].
+     *     If isOk is false, an error has been raised: this is a CRITICAL ERROR and executions at
+     *     upper level must be stopped.
+     * */
+    async setupRuntime() {
 
-                # if reaching this point, the call is a valid import, so apply it:
-                return base_import(*a,**kw)
+        Object.entries({
+            exclusionsTools: true,
+            inputPrompt: true,
+            version: true,
+            refresher: true,
+        }).forEach(([opt, todo]) => {
+            jsLogger("[Feature (re-/load)] -", opt)
+            if (todo) pyodide.runPython(terminalFeatureCode(opt))
+        })
 
+        // Build the default configuration options to use to run the user's code:
+        const options = this.buildOptionsForPyodideRun()
+        const [stdErr, isAssertErr] = await this.runEnvironmentAsync(options, 'env')
+        return {
+            options,
+            stdErr,
+            isAssertErr
+        }
+    }
 
-        # Store the originals used here to avoid troubles with exclusions at runtime:
-        base_import = __import__
-        base_str = str
-        base_isinstance = isinstance
 
-        __builtins__.__builtins___ = dct = {}
-        raiser_import = Raiser('__import__')
-        dct['__import__'] = [base_import, raiser_import]
-        __builtins__.__import__ = raiser_import
 
+    /**Takes a code as argument, and run it in the pyodide environment, using various options:
+     *
+     * @throws: Any JS runtime Error, if something went very wrong... (python errors are swallowed
+     *          and just printed to the terminal)
+     * @returns: The stdErr formatted string message that got printed in the terminal, or empty
+     *           string if no error.
+     *           Note that the message is displayed in the console already, so this is only a
+     *           "marker" to propagate some logic in other parts of the application.
+     *
+     * NOTE:
+     *    - Pyodide itself is using eval, so replacing globally the builtin will cause a lot of
+     *      troubles and just won't work.
+     *    - This function doesn't take in charge the pyodide environment setup, (preparation,
+     *      rebuilding the setup, ...).
+     *    - On the other hand it DOES take in charge installation of missing modules/packages
+     *      in the user's/given code.
+     */
+    async runPythonCodeWithOptions(code, options) {
 
-        for key in ${ JSON.stringify(excluded) }:
-            stuff = getattr(__builtins__, key, None)
-            dct[key] = [stuff, None]
-            # => the dict will store [None,None] for module names
+        // Do nothing if nothing to do...!
+        if (!code.trim()) return ""
 
-        if ${ recLimit } != -1:
-            import sys
-            sys.setrecursionlimit(${ recLimit })
-            dct['setrecursionlimit'] = [sys.setrecursionlimit, None]
+        try {
+            // Do first the methods exclusions check, to gain some time (avoids loading modules if
+            // the error would show up anyway after loading them)
+            const nope = options.excludedMethods.filter(methodCall => code.includes(methodCall))
+            if (nope.length) {
+                const plural = nope.length > 1 ? "s" : ""
+                const nopes = nope.map(s => s.slice(1)).join(', ')
+                const msg = `${ CONFIG.MSG.exclusionMarker } method${plural}: ${ nopes }`
+                throw new PythonError(msg)
+            }
 
-        for key,lst in dct.items():
-            stuff = lst[0]
-            if callable(stuff) and key!='__import__':       # import already handled
-                globals()[key] = lst[1] = Raiser(key)
-                # store the reference to the raiser, to check against it later
+            // Detect possible user imports and install the packages to allow their imports:
+            await this.installAndImportMissingModules(code, options)
 
-    _hack()
-    del _hack `
+        } catch (err) {
+            const [strErr, _] = generateErrorLog(err, code, false, !options.isPublic)
+            return this.giveFeedback("", strErr)
+        }
 
-    // console.log(code)
+        const withExclusions = options.excluded.length > 0 || options.recLimit > 0
 
-    pyodide.runPython(code)
-}
+        // Setup stdout capture. WARNING: this must always be done even if it's not shown to the user.
+        // If not done, a previous execution might have close the StringIO and if ever the user prints
+        // something, it would result in an error without that:
+        setupStdIO()
+
+        // Setup code/imports exclusions if any (later id better)
+        if (withExclusions) setupExclusions(options.excluded, options.recLimit)
+
+        let stdErr = "",
+            stdOut = "",
+            delayedErr, _ // "_" to avoid loosing lodash...
+        try {
+            await options.runCodeAsync(code)
+        } catch (err) {
+            // Since generateErrorLog might run python code, the exclusions must be removed _before_
+            // the function is called, so store the error for later use.
+            delayedErr = err
 
+        } finally {
+            // Teardown steps must always occur, whatever happened (even for JS errors), hence in a
+            // finally close, and they also must be protected against failure, so in their own
+            // try/catch/finally construct:
+            try {
+                if (withExclusions) restoreOriginalFunctions(options.excluded)
+
+                // Now only, compute the error message if needed.
+                if (delayedErr) {
+                    ;
+                    [stdErr, _] = generateErrorLog(delayedErr, code, options.autoLogAssert, !options.isPublic)
+                }
+
+                // Always extract the stdout and close the buffer (avoid memory leaks)
+                let captured = getFullStdIO()
+
+                // Send stdout feedback to the user only if allowed:
+                if (options.withStdOut) {
+                    stdOut = textShortener(captured)
+                }
+
+            } catch (err) {
+                // This second catch is there so that the user can see the JS error in the terminal.
+                // (Note: maybe I should actually throw them again...?)
+                ;
+                [stdErr, _] = generateErrorLog(err, code, true)
 
+            } finally {
+                // Use a finally clause, in case something went wrong in generateErrorLog...
+                // (the message probably won't be accurate, but at least, something will be visible)
+                this.giveFeedback(stdOut, stdErr)
+            }
+            return stdErr
+        }
+    }
 
 
-/**Cancel the code exclusions (done as soon as possible, to restore pyodide's normal behaviors).
- * */
-const restoreOriginalFunctions = exclusions => {
-    pyodide.runPython(`
-    def _hack():
-        G = globals()
 
-        not_ok = any(
-            key for key,(func,raiser) in __builtins___.items()
-                if raiser is not None and key!='__import__' and raiser is not G.get(key)
-        )
-        if not_ok:
-            ExclusionError.throw("${ exclusions }")
 
-        for key,(func,raiser) in __builtins___.items():
+    async teardownRuntime(options, _gotError, _finalMsg = "") {
+        jsLogger("[Teardown] - PyodideRunner")
 
-            if key == '__import__':
-                __builtins__.__import__ = func
+        const out = await this.runEnvironmentAsync(options, 'post')
+        this.globalTearDown()
+        return out
+    }
 
-            elif func is not None:
-                G[key] = func
-                if key == 'setrecursionlimit':
-                    func(1000)
-    _hack()
-    del _hack
-    `)
 }
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -15,19 +15,19 @@
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
 
 /**Return the plain error message, unless it's an assertion error, where the message is formatted.
- * @err (Error) :           The Error object caught in JS context.
- * @code (string):          The python code that (possibly) generated the error.
- * @autoMsg (boolean=true): If the error is an AssertionError without message, automatically add
- *                          the assertion instruction if autoMsg is true.
- * @extraErrInfo (string=""): extra message the is added
+ * @err (Error):   The Error object caught in JS context.
+ * @code (string): The python code that (possibly) generated the error.
+ * @allowAssertCodeExtraction (boolean=true): If the error is an AssertionError without message, automatically add
+ *                 the assertion instruction if autoMsg is true.
+ * @purgeErr (boolean): if true, the complète stacktrace will be removed of error messages
  *
  * ---
  *
  * ## Rationals
  *
  * - The argument error can be of any kind (JS or python)
  * - "Legit" errors are those starting with "PythonError".
@@ -107,21 +107,22 @@
  *       File "<exec>", line 2, in <module>
  *       File "<env>", line 10, in essai
  *       File "<env>", line 10, in essai
  *       File "<env>", line 10, in essai
  *       [Previous line repeated 44 more times]
  *     RecursionError: maximum recursion depth exceeded
  * */
-function generateErrorLog(err, code, allowAssertionCodeExtraction, purgeErr) {
+function generateErrorLog(err, code, allowAssertCodeExtraction, purgeErr = false) {
 
     const msg = String(err).trimEnd() // Note: err has a trailing linefeed, so, trim it...
 
+
     // Return directly non python errors. => allows to also see JS errors.
     if (!msg.startsWith('PythonError')) {
-        return youAreInTroubles(err)
+        return [youAreInTroubles(err), false]
     }
 
     const errLines = msg.split("\n")
 
     /*
     Search for the first line after the pyodide-specific infos, avoiding false positives for
     terminals, where the second line is: ""  File "<exec>", line dd, in await_fut".
@@ -139,30 +140,31 @@
     */
     const isFromUserCode = iModule > 0
 
     const [iError, isAssertErr] = getErrorKindInfos(errLines)
 
     // If ExclusionError, just throw the last line without anything else:
     if (errLines[iError].includes(CONFIG.MSG.exclusionMarker)) {
-        let msg = errLines.slice(iError).join('\n')
+        const msg = errLines.slice(iError).join('\n')
         const i = msg.indexOf(CONFIG.MSG.exclusionMarker)
-        return error(msg.slice(i))
+        return [msg.slice(i), false]
     }
 
     const isMultiLineError = iError + 1 < errLines.length
     const cleaned = (errLines[iError] || "").replace("AssertionError", "").trim()
     const hasNoMsg = !isMultiLineError && !cleaned
 
     // WARNING: working by mutation, so successive splices are done 'from the end".
 
     // Rebuild the assertion message first, if needed:
-    if (isAssertErr && hasNoMsg && allowAssertionCodeExtraction) {
-        buildAssertionMsg(code, errLines, iError)
+    if (isAssertErr && hasNoMsg && allowAssertCodeExtraction) {
+        const bigFail = buildAssertionMsg(code, errLines, iError)
+        if (bigFail) return [bigFail, false]
 
-    } else if (!isAssertErr && purgeErr && CONFIG.showOnlyAssertionErrorsForSecrets) {
+    } else if (!isAssertErr && purgeErr) {
         // Reformat error message if needed
         const errKind = errLines[iError].split(':')[0]
         errLines.splice(iError, errLines.length)
         errLines.push(`${errKind} has been raised.`)
     }
 
     // Shorten the error code section (if multiline assertion message), and then the stacktrace.
@@ -172,32 +174,31 @@
     // it's the user's code that is run, otherwise, keep the full stack trace to ease debugging:
     if (isFromUserCode) {
         shortenArrSection('trace', errLines, iModule, iError - 1, iModule, purgeErr)
 
     } else {
         errLines.push(CONFIG.MSG.bigFail)
     }
-
-    return [error(errLines.join('\n')), isAssertErr]
+    return [errLines.join('\n'), isAssertErr]
 }
 
 
 
 /**Mutate the content of the given array, if the section identified by the original `from` and
  * `to` indices is considered too long.
  * Both indices arguments are inclusive.
  * */
 const shortenArrSection = (kind, errLines, from, to, iModule, purgeErr) => {
 
-    if (kind == 'trace' && CONFIG.showOnlyAssertionErrorsForSecrets && purgeErr) {
+    if (kind == 'trace' && purgeErr) {
         errLines.splice(0, to + 1)
         return
     }
 
-    if (!CONFIG.cutFeedback) {
+    if (CONFIG.cutFeedback) {
 
         const [limit, head, tail] = "Limit Head Tail".split(' ').map(prop => CONFIG.feedbackShortener[kind + prop])
         if (to - from > limit) {
             from += head
             to -= tail
             let middle = CONFIG.feedbackShortener.msg
             if (kind == 'trace') {
@@ -299,9 +300,9 @@
 }
 
 
 
 
 /**Extract full information when something gets VERY wrong... */
 function youAreInTroubles(err) {
-    return error(`${ err }\n\n${ err.stack || '[no stack]' }\n${ CONFIG.MSG.bigFail }`)
+    return `${ err }\n\n${ err.stack || '[no stack]' }\n${ CONFIG.MSG.bigFail }`
 }
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -14,206 +14,140 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
 
-/**Insertion of the hourglass svg (note: done in the libs section because it's a general tool,
- * but the header doesn't exist yet, so the subscription delay is used, and it's done from here
- * so that the hourglass cannot show up in pages tht do not need it.
+
+/**This is what's triggering the huge lag, when loading the page, so do it only when an ide or
+ * or terminal is needed, and do it on next tick, so that all the scripts are actually loaded first
  * */
-subscribeWhenReady(
-    "HourGlass",
-    function() {
-        jsLogger('[HourGlass]')
+setTimeout(async () => {
 
-        const hourGlassSvg = `
-<svg viewBox="0 0 512 512" id="${ CONFIG.element.hourGlass.slice(1) }"
-    height="24px" width="24px" version="1.1" xmlns="http://www.w3.org/2000/svg"
-    xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" fill="#ffffff">
-    <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
-    <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
-    <g id="SVGRepo_iconCarrier">
-        <g>
-            <path class="st0" d="M329.368,237.908l42.55-39.905c25.237-23.661,39.56-56.701,39.56-91.292V49.156 c0.009-13.514-5.538-25.918-14.402-34.754C388.24,5.529,375.828-0.009,362.314,0H149.677c-13.514-0.009-25.918,5.529-34.754,14.401 c-8.872,8.837-14.41,21.24-14.402,34.754v57.554c0,34.591,14.315,67.632,39.552,91.292l42.55,39.888 c2.352,2.205,3.678,5.272,3.678,8.493v19.234c0,3.221-1.326,6.279-3.67,8.475l-42.558,39.905 c-25.237,23.653-39.552,56.702-39.552,91.292v57.554c-0.009,13.514,5.529,25.918,14.402,34.755 c8.836,8.871,21.24,14.409,34.754,14.401h212.636c13.514,0.008,25.926-5.53,34.763-14.401c8.863-8.838,14.41-21.241,14.402-34.755 v-57.554c0-34.59-14.324-67.64-39.56-91.292l-42.55-39.896c-2.344-2.205-3.678-5.263-3.678-8.484v-19.234 C325.69,243.162,327.025,240.095,329.368,237.908z M373.942,462.844c-0.009,3.273-1.266,6.055-3.403,8.218 c-2.162,2.135-4.952,3.402-8.226,3.41H149.677c-3.273-0.009-6.055-1.275-8.225-3.41c-2.128-2.163-3.394-4.945-3.402-8.218v-57.554 c0-24.212,10.026-47.356,27.691-63.91l42.55-39.906c9.914-9.285,15.538-22.274,15.538-35.857v-19.234 c0-13.592-5.624-26.58-15.547-35.866l-42.541-39.896c-17.666-16.555-27.691-39.69-27.691-63.91V49.156 c0.008-3.273,1.274-6.055,3.402-8.226c2.17-2.127,4.952-3.394,8.225-3.402h212.636c3.273,0.009,6.064,1.275,8.226,3.402 c2.136,2.171,3.394,4.952,3.403,8.226v57.554c0,24.22-10.026,47.355-27.683,63.91l-42.55,39.896 c-9.922,9.286-15.547,22.274-15.547,35.866v19.234c0,13.583,5.625,26.572,15.547,35.874l42.55,39.88 c17.658,16.563,27.683,39.707,27.683,63.918V462.844z"></path>
-            <path class="st0" d="M256,248.674c10.017,0,18.131-8.122,18.131-18.139c3.032-12.051,9.397-23.161,18.578-31.757l42.542-39.888 c13.592-12.739,21.602-30.448,22.446-48.984H154.302c0.844,18.536,8.854,36.245,22.438,48.984l42.541,39.888 c9.19,8.596,15.547,19.706,18.579,31.757C237.861,240.552,245.983,248.674,256,248.674z"></path>
-            <path class="st0" d="M256,267.796c-10.017,0-18.139,8.122-18.139,18.139c0,10.009,8.122,18.131,18.139,18.131 c10.017,0,18.131-8.122,18.131-18.131C274.131,275.918,266.017,267.796,256,267.796z"></path>
-            <path class="st0" d="M256,332.137c-10.017,0-18.139,8.122-18.139,18.14c0,10.009,8.122,18.131,18.139,18.131 c10.017,0,18.131-8.122,18.131-18.131C274.131,340.259,266.017,332.137,256,332.137z"></path>
-            <path class="st0" d="M239.876,389.742l-66.538,66.538h165.315l-66.537-66.538C263.21,380.845,248.782,380.845,239.876,389.742z"></path>
-        </g>
-    </g>
-</svg>`
-        $(CONFIG.element.searchBtnsLeft).prepend($(hourGlassSvg))
-    }, {
-        waitFor: CONFIG.element.searchBtnsLeft
-    },
-)
+    ace.require("ace/ext/language_tools");
 
+    // Delay to let the elements in the page to load before the page starts to freeze...
+    await sleep(CONFIG.pyodideDelay)
 
+    // slow step...
+    globalThis.pyodide = await loadPyodide()
 
+    // Extract basic utilities for JS <-> python communication:
+    globalThis.pyFuncs = setupPyodideEnvironmentTools()
 
 
-/**Allow to delay the executions of various functions, until the pyodide environment
- * is done loading.
- * */
-async function waitForPyodideReady() {
+    // Check everything is as expected on pyodide side:
+    const keeper = ['__name__', '__doc__', '__package__', '__loader__', '__spec__', '__annotations__', '__builtins__', '_pyodide_core', 'version']
+    const unknown = pyodide.runPython('",".join(globals())').split(',').filter(k => !keeper.includes(k))
 
-    const maxWaitingTime = 20
-    const attempts = 80
-    const step_ms = Math.round(1000 * maxWaitingTime / attempts)
-
-    let counter = 0
-    while (!globalThis.pyodide) {
-        await sleep(step_ms);
-        if (++counter == attempts) {
-            throw new Error(`Couldn't access to pyodide environment in time (${maxWaitingTime}s)`)
-        }
-    }
-}
+    if (unknown.length) {
+        window.alert(`
+Something unexpected was found in pyodide environnement startup.
 
+The python environment might behave strangely because of this, or even raise unexpected errors.
+Please contact the author of the theme by opening a ticket with this complete message on:
 
-/**This is what's triggering the huge lag, when loading the page, so do it only when an ide or
- * or terminal is needed, and do it on next tick, so that all the scripts are actually loaded first
- * */
-setTimeout(async () => {
+  ${ CONFIG.pmtUrl }/-/issues
 
-    globalThis.pyodide = await loadPyodide()
+Unknown = ${ JSON.stringify(unknown) }
+`)
+    }
 
-    globalThis.pyFuncs = setupPyodideEnvironmentTools()
 
-    pyodide._module.on_fatal = withPyodideAsyncLock(async (e) => {
+    // Put in place a "critical error" message (never saw it, so far...)
+    pyodide._module.on_fatal = withPyodideAsyncLock('fatal', async (e) => {
         const term = $.terminal.active()
         term.error(
             "Pyodide has suffered a fatal error. Please report this to the Pyodide maintainers."
         )
         term.error("The cause of the fatal error was:")
         term.error(e)
-        term.error("The console will start again in 10s")
-        term.pause();
         await sleep(); // Enforce UI refresh
-        term.resume();
     })
-})
-
 
+    // All done!
+    globalThis.pyodideIsReady = true
+    $("#header-hourglass-svg").attr("class", "py_mk_vanish")
+})
 
 
 
 /**Creates the console: the variable pyconsole, which is the runtime tool behind the  "terminal
  * process" is created here.
  * Returns the PyodideConsoleManager which handles the python functions needed to control the
  * python console from the JS layer
  *
  * https://pyodide.org/en/stable/usage/api/python-api/console.html#pyodide.console.PyodideConsole
  * */
 function setupPyodideEnvironmentTools() {
 
+    const routines = "pyconsole, await_fut, clear_console"
+
     // Indentation does matter a bit: 1 extra indent is ok, but 2 fails (whatever... :rolleyes: )
     const pythonRoutinesExtractionCode = `
     def _hack():
         import js
         import __main__
         from pyodide.console import PyodideConsole, repr_shorten
 
         pyconsole = PyodideConsole(__main__.__dict__)
 
         async def await_fut(fut):
             res = await fut
+
             if res is None:
                 return
+            __builtins__['_'] = res
 
-            if js.getFeedbackConfig():
+            if js.getCutFeedbackConfig():
                 res = repr_shorten(res)
             print(res, end='')
 
-        def clear_console():
+        def clear_console():            # Useless...?
             pyconsole.buffer = []
 
-        return pyconsole, await_fut, clear_console
+        return ${ routines }
 
-    pyconsole, await_fut, clear_console = _hack()
+    ${ routines } = _hack()
     del _hack`
 
     const namespace = pyodide.globals.get("dict")();
     pyodide.runPython(pythonRoutinesExtractionCode, {
         globals: namespace
     });
 
-    const routines = "await_fut pyconsole clear_console".split(" ")
     const outRoutines = {}
-    for (let key of routines) {
+    for (let key of routines.split(/, */)) {
         outRoutines[key] = namespace.get(key)
     }
     namespace.destroy(); // avoid (some) memory leaks
     return outRoutines
 }
 
 
 
 
-
-/**Archive the current window scroll position
- * */
-var setCurrentScroll = _.debounce(function() {
-    CONFIG.currentScroll = [window.scrollX, window.scrollY]
-    jsLogger("[Scroll] - current =", CONFIG.currentScroll)
-}, 200, {
-    leading: true,
-    trailing: false
-})
-
-
-
-
-
-/**Search for the input#py_mk_pin_scroll element and activate focus on it if it exists.
- * */
-function restoreScrollPositionAndBlur() {
-    jsLogger('[Scroll] - Scroll handling attempt...')
-    if (CONFIG.currentScroll) window.scrollTo(...CONFIG.currentScroll)
-    debouncedTerminalBlur()
-}
-
-
-
-
-/**Debounced callback, to enforce blurring the text areas of terminals.
- * This is debounced, in case several terminals are put in place.
- * In case setting up terminals is too slow, the hidden input will be removed from the page
- * by previous terminals, so it should just be put back in place and the logic should still work.
+/**Insertion of the hourglass svg (note: done in the libs section because it's a general tool,
+ * but the header doesn't exist yet, so the subscription delay is used, and it's done from here
+ * so that the hourglass cannot show up in pages tht do not need it.
  * */
-var debouncedTerminalBlur = _.debounce(function() {
-    $("#header-hourglass-svg").attr("class", "py_mk_vanish")
+subscribeWhenReady(
+    "HourGlass",
+    function() {
+        jsLogger('[HourGlass]')
 
-    /*
-    Handling the focus/blur of jQuery terminal is an absolute nightmare... The only way I
-    found to enforce them to release focus without action from the user is:
-        1. Override onBlur on each terminal (otherwise they never lose focus)
-        2. Enforce scrolling back to the position before creation of the terminal
-        3. Use an hidden input button and its click event to make sure the last textarea
-            defined loses the focus... (note: it _doesn't_ work with a text input or autofocus)
-    */
-    const [x, y] = CONFIG.currentScroll
-    jsLogger('[Scroll]', x, y)
-    $('body').append(`
-        <input type="button" id="py_mk_pin_scroll_input"
-            style="
-                position:absolute; left:${x}px; top:${y}px;
-                width:50px; height:20px; color: red;background-color: red; z-index: 20;
-                visibility:hidden;
-        ">`.replace(/\s+/g, " "))
-
-    // This is mostly out of despair... x/
-    window.scrollTo(x, y)
-    setTimeout(() => {
-        let inp = $('#py_mk_pin_scroll_input')[0]
-        inp.click()
-        inp.remove()
-        jsLogger('[Scroll] - blur terminal!!', x, y)
-        window.scrollTo(x, y)
-    }, 40)
-    setTimeout(() => {
-        window.scrollTo(x, y)
-        // checkTerms()
-    }, 25)
-}, 40)
+        const hourGlassSvg = `
+<svg viewBox="0 0 512 512" id="${ CONFIG.element.hourGlass.slice(1) }"
+    height="24px" width="24px" version="1.1" xmlns="http://www.w3.org/2000/svg"
+    xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" fill="#ffffff"><g>
+    <path class="st0" d="M329.368,237.908l42.55-39.905c25.237-23.661,39.56-56.701,39.56-91.292V49.156 c0.009-13.514-5.538-25.918-14.402-34.754C388.24,5.529,375.828-0.009,362.314,0H149.677c-13.514-0.009-25.918,5.529-34.754,14.401 c-8.872,8.837-14.41,21.24-14.402,34.754v57.554c0,34.591,14.315,67.632,39.552,91.292l42.55,39.888 c2.352,2.205,3.678,5.272,3.678,8.493v19.234c0,3.221-1.326,6.279-3.67,8.475l-42.558,39.905 c-25.237,23.653-39.552,56.702-39.552,91.292v57.554c-0.009,13.514,5.529,25.918,14.402,34.755 c8.836,8.871,21.24,14.409,34.754,14.401h212.636c13.514,0.008,25.926-5.53,34.763-14.401c8.863-8.838,14.41-21.241,14.402-34.755 v-57.554c0-34.59-14.324-67.64-39.56-91.292l-42.55-39.896c-2.344-2.205-3.678-5.263-3.678-8.484v-19.234 C325.69,243.162,327.025,240.095,329.368,237.908z M373.942,462.844c-0.009,3.273-1.266,6.055-3.403,8.218 c-2.162,2.135-4.952,3.402-8.226,3.41H149.677c-3.273-0.009-6.055-1.275-8.225-3.41c-2.128-2.163-3.394-4.945-3.402-8.218v-57.554 c0-24.212,10.026-47.356,27.691-63.91l42.55-39.906c9.914-9.285,15.538-22.274,15.538-35.857v-19.234 c0-13.592-5.624-26.58-15.547-35.866l-42.541-39.896c-17.666-16.555-27.691-39.69-27.691-63.91V49.156 c0.008-3.273,1.274-6.055,3.402-8.226c2.17-2.127,4.952-3.394,8.225-3.402h212.636c3.273,0.009,6.064,1.275,8.226,3.402 c2.136,2.171,3.394,4.952,3.403,8.226v57.554c0,24.22-10.026,47.355-27.683,63.91l-42.55,39.896 c-9.922,9.286-15.547,22.274-15.547,35.866v19.234c0,13.583,5.625,26.572,15.547,35.874l42.55,39.88 c17.658,16.563,27.683,39.707,27.683,63.918V462.844z"></path>
+    <path class="st0" d="M256,248.674c10.017,0,18.131-8.122,18.131-18.139c3.032-12.051,9.397-23.161,18.578-31.757l42.542-39.888 c13.592-12.739,21.602-30.448,22.446-48.984H154.302c0.844,18.536,8.854,36.245,22.438,48.984l42.541,39.888 c9.19,8.596,15.547,19.706,18.579,31.757C237.861,240.552,245.983,248.674,256,248.674z"></path>
+    <path class="st0" d="M256,267.796c-10.017,0-18.139,8.122-18.139,18.139c0,10.009,8.122,18.131,18.139,18.131 c10.017,0,18.131-8.122,18.131-18.131C274.131,275.918,266.017,267.796,256,267.796z"></path>
+    <path class="st0" d="M256,332.137c-10.017,0-18.139,8.122-18.139,18.14c0,10.009,8.122,18.131,18.139,18.131 c10.017,0,18.131-8.122,18.131-18.131C274.131,340.259,266.017,332.137,256,332.137z"></path>
+    <path class="st0" d="M239.876,389.742l-66.538,66.538h165.315l-66.537-66.538C263.21,380.845,248.782,380.845,239.876,389.742z"></path>
+</g></svg>`
+        $(CONFIG.element.searchBtnsLeft).prepend($(hourGlassSvg))
+    }, {
+        waitFor: CONFIG.element.searchBtnsLeft
+    },
+)
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
 /* https://pustelto.com/blog/optimizing-css-for-faster-page-loads/ */
 
+/* NOTE: this file must be loaded BEFORE the one about header-btns (overloading order) */
+
 
 :root {
   --main-color: 87, 147, 240;
   --main-theme: rgb(var(--main-color));
   --gutter-theme: transparent;
   --background-theme: transparent;
   --code-outline-color: #959595;
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
+.term_wrapper {
+  position: relative;
+}
 
 /* Common to all terminales.
    --n-lines is defined on the parent, through the terminal macro */
 .py_mk_terminal {
   --color: var(--main-theme);
   --base-color: var(--main-theme);
   --background: var(--gutter-theme);
   --base-background: var(--md-default-bg-color);    /* FIX wrong colors on selection */
   --size: 1.3;
   width: 100%;
-  position: relative;
   overflow: auto;
 }
 
 .term_editor, .py_mk_terminal_solo {
   height: calc( 1em * var(--n-lines) * var(--size) * 0.95 );
   /* min-width: this is a bad idea, because if a terminal is inside an admonition, the terminal
      will go out of the admonition (which is ignoring its content...)
@@ -43,16 +45,31 @@
 .py_mk_terminal_solo {
   border: solid 1px;
   border-radius: 0 8px 0 8px;
   border-color: var(--main-theme);
 }
 
 
-.stdout-ctrl {
-  width: 24px;
-  height: 24px;
+.term_btns_wrapper {
   position: absolute;
-  right: 7px;
   top: 5px;
-  z-index: 101;   /* lol XD */
+  right: 5px;
+  display: grid;
+  font-size: 1.15em;
+  line-height: 1em;
+  gap: 3px;
   font-family: var(--md-text-font-family);    /* for the tooltips */
 }
+
+
+.md-typeset .stdout-ctrl svg {
+  fill: none !important;
+}
+
+.stdout-wraps-btn span.twemoji:hover {
+  --wrap-opacity: 55% !important;
+}
+
+.md-typeset .stdout-wraps-btn span.twemoji {
+  opacity:var(--wrap-opacity);
+  margin-left: 2px;
+}
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
+/*
+WARNING:  This file HAS to be loaded before the DOM is built, otherwise
+          the content won't be properly formatted.
+*/
+
 .md-typeset .py_mk_admonition_qcm-inner  {
   text-align: justify;
   width: calc( 100% - 4em);
   margin: 0;
   position: relative;
 }
```

### Comparing `pyodide_mkdocs_theme-0.7.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.7.1/pyproject.toml` & `pyodide_mkdocs_theme-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.7.1"
+version = "1.0.0"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
@@ -43,15 +43,16 @@
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.1"
 pytest = "^8.1"
 mkdocs-awesome-pages-plugin = "^2.9"
 mkdocs-exclude-search = "^0.6"
 mkdocs-enumerate-headings-plugin = "^0.6"
-mkdocs-addresses = "^0.3"
 mkdocstrings = {version = "^0.24", extras = ["python"]}
-mkdocs-glightbox = "^0.3"
+mkdocs-addresses = "^0.3.2"
+mkdocs-glightbox = "^0.4.0"
+
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyodide_mkdocs_theme-0.7.1/PKG-INFO` & `pyodide_mkdocs_theme-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.7.1
+Version: 1.0.0
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

