# Comparing `tmp/pyodide_mkdocs_theme-1.0.1.tar.gz` & `tmp/pyodide_mkdocs_theme-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-1.0.1.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-1.0.2.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-1.0.1.tar` & `pyodide_mkdocs_theme-1.0.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-1.0.1/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-1.0.1/README.md
--rw-r--r--   0        0        0     1347 2024-05-16 18:53:21.067527 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2591 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-05-16 18:53:21.103528 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0     1322 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
--rw-r--r--   0        0        0     1063 2024-05-15 21:11:56.293098 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-05-12 18:52:50.335028 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     5919 2024-05-15 21:11:56.321099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     2992 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py
--rw-r--r--   0        0        0        0 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0    11922 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py
--rw-r--r--   0        0        0    16534 2024-05-15 21:11:56.337099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py
--rw-r--r--   0        0        0    21130 2024-05-15 21:11:56.369100 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py
--rw-r--r--   0        0        0     4850 2024-05-15 21:11:56.377100 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py
--rw-r--r--   0        0        0     3470 2024-05-15 21:11:56.377100 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py
--rw-r--r--   0        0        0     2435 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11591 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    13668 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     7141 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0    14460 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4776 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0        0 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    15211 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11391 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0     9693 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
--rw-r--r--   0        0        0     1603 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     6652 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
--rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9042 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1163 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     9480 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0     4229 2024-05-16 18:53:21.063527 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     5487 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/mkdocs.yml
--rw-r--r--   0        0        0     3593 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/model.py
--rw-r--r--   0        0        0      823 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/README.md
--rw-r--r--   0        0        0        0 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     2857 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg
--rw-r--r--   0        0        0     1645 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png
--rw-r--r--   0        0        0     6093 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0    10609 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1770 2024-05-16 18:53:18.103440 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0    10814 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js
--rw-r--r--   0        0        0    14528 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js
--rw-r--r--   0        0        0     1183 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js
--rw-r--r--   0        0        0     8220 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js
--rw-r--r--   0        0        0    18519 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js
--rw-r--r--   0        0        0    12716 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js
--rw-r--r--   0        0        0     7231 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js
--rw-r--r--   0        0        0    11253 2024-05-15 21:11:56.481103 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js
--rw-r--r--   0        0        0     4455 2024-05-15 21:11:56.489103 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0     5341 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     2635 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     3831 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css
--rw-r--r--   0        0        0     1078 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css
--rw-r--r--   0        0        0     1947 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css
--rw-r--r--   0        0        0     3744 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css
--rw-r--r--   0        0        0     3904 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css
--rw-r--r--   0        0        0     1918 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css
--rw-r--r--   0        0        0     1766 2024-05-16 18:53:18.139441 pyodide_mkdocs_theme-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-1.0.2/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-1.0.2/README.md
+-rw-r--r--   0        0        0     1347 2024-05-16 18:55:51.771965 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2591 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-16 18:55:51.803966 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1322 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0     1063 2024-05-15 21:11:56.293098 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-05-12 18:52:50.335028 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     5919 2024-05-15 21:11:56.321099 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     2992 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0    11922 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py
+-rw-r--r--   0        0        0    16534 2024-05-15 21:11:56.337099 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py
+-rw-r--r--   0        0        0    21130 2024-05-15 21:11:56.369100 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py
+-rw-r--r--   0        0        0     4850 2024-05-15 21:11:56.377100 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py
+-rw-r--r--   0        0        0     3470 2024-05-15 21:11:56.377100 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py
+-rw-r--r--   0        0        0     2435 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11591 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13668 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     7262 2024-05-16 18:54:43.525957 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0    16287 2024-05-16 18:54:43.529958 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4776 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    15211 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11391 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0     9693 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
+-rw-r--r--   0        0        0     1603 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     6652 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
+-rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9042 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1163 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     9655 2024-05-16 18:54:43.529958 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0     4229 2024-05-16 18:55:51.771965 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     5487 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/scripts/mkdocs.yml
+-rw-r--r--   0        0        0     3593 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/scripts/model.py
+-rw-r--r--   0        0        0      823 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg
+-rw-r--r--   0        0        0     1645 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     6093 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0    10631 2024-05-16 18:54:43.529958 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1770 2024-05-16 18:55:49.163888 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0    10814 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js
+-rw-r--r--   0        0        0    14528 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js
+-rw-r--r--   0        0        0     1183 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js
+-rw-r--r--   0        0        0     8220 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js
+-rw-r--r--   0        0        0    18519 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js
+-rw-r--r--   0        0        0    12716 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js
+-rw-r--r--   0        0        0     7231 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js
+-rw-r--r--   0        0        0    11253 2024-05-15 21:11:56.481103 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0     4455 2024-05-15 21:11:56.489103 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0     5341 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     2635 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     3831 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css
+-rw-r--r--   0        0        0     1078 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css
+-rw-r--r--   0        0        0     1947 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css
+-rw-r--r--   0        0        0     3764 2024-05-16 18:54:43.529958 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css
+-rw-r--r--   0        0        0     3904 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css
+-rw-r--r--   0        0        0     1918 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css
+-rw-r--r--   0        0        0     1766 2024-05-16 18:55:49.195889 pyodide_mkdocs_theme-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-1.0.2/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-1.0.1/LICENSE` & `pyodide_mkdocs_theme-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/README.md` & `pyodide_mkdocs_theme-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,14 +140,16 @@
         """
 
         # Yield the global variable first, because the JS scripts will use it at runtime:
 
         global_var = '{' + ', '.join(
             f'"{ editor_name }": { conf.dump_to_js_code() }' for editor_name,conf in self.items()
         )+'}'
+        # print(json.loads(global_var))     # To check the validity of the dumped data
+        # print(repr(global_var))
         encoded = compress_LZW(global_var)
         chunks.append(Html.script(f"let PAGE_IDES_CONFIG = { encoded !r}"))
 
         # Spot invalid kinds:
         missed = {kind for kind in self.needs if kind not in kind_to_scripts}
         if missed:
             logger.error(
```

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
+from pathlib import Path
 import re
 from typing import Callable, List, Optional
 from string import printable
 from random import shuffle
 
 from mkdocs.exceptions import BuildError
 
 from .exceptions import PyodideMacrosParsingError
-from .tools_and_constants import LZW
+from .tools_and_constants import LZW, DebugConfig
 
 
 
 
 
 def replace_chunk(source:str, start:str, end:str, repl:str, *, at=0, keep_limiters=False):
     """ Given a @source and two delimiters/tokens, @start and @end, find those two tokens in
@@ -112,53 +113,60 @@
 
 
 TOME_BASE = re.sub(r'[<>"\[\]\\]', '', printable)[:-5]
 """ Removed:
         - "<>" because could generate tags
         - "[]" because could be seen as md links syntaxe by mkdocs-addresses
 """
-LAST_BASE = TOME_BASE[-1]
-BASE      = len(TOME_BASE)
+BASE = len(TOME_BASE)
+
 
 def i_to_base(n,size):
-    return ''.join(
+    out = ''.join(
         TOME_BASE[ n // BASE**p % BASE ]
         for p in reversed(range(size))
     )
+    if n != un_i_to_base(out):
+        raise
+    return out
 
 def compress_LZW(txt:str):
+    return txt
+    # print(txt)
 
     tome  = set(txt) - set('<>')                    # remove tags tokens
     big   = list(filter(chr(255).__lt__, tome))     # might be problematic for python->JS transfer
     small = list(filter(chr(255).__ge__, tome))     # easy ones (python->JS)
-    shuffle(small)                                # 'cause, why not... :p
+    if DebugConfig.shuffle:
+        shuffle(small)                              # 'cause, why not... :p
     alpha = list('><')+big+small                    # Will always be added afterward
 
     def grab(j):
         i,j = j,j+1
         while j<len(txt) and txt[i:j] in dct: j+=1
         token = txt[i:j]
 
         if token not in dct:
             # tokens.append(token)
             dct[token] = i_to_base(len(dct), size)
             return j-1, dct[token[:-1]]
 
         return len(txt), dct[token]
 
-    out,i,size = [],0,2
+    out,i,size,limit = [], 0, 2, BASE**2
     dct = {c: i_to_base(i, size) for i,c in enumerate(alpha)}
     # tokens = [*alpha]
 
-    while i<len(txt):
+    while i < len(txt):
         i,idx_base = grab(i)
         out.append(idx_base)
-        if not idx_base.strip(LAST_BASE):     # Reached x**base-1 => increase the chunk size
-            size += 1
+        if len(dct)==limit:     # Reached x**base-1 => increase the chunk size
             out.append(LZW)
+            size += 1
+            limit = BASE**size
 
     # Each \n char in the encoded tag means "increase the token byte length by one"
     # print(table)
     # print('dict size:',len(dct), 'size:', size)
     # print(len(src_txt),'->',len(output))
     # rev_table = {s:i for i,s in enumerate(table)}
     # counts = [tokens[rev_table[s]] for s in out]
@@ -166,19 +174,81 @@
 
     # version to put in the encoded tag, WITHOUT any "<" or ">" character:
     encoded_bigs      = '.'.join( str(ord(c)) for c in big )
     encoded_smalls    = ''.join(small)
     output_with_table = f".{ encoded_bigs }{ LZW }{ encoded_smalls }{ LZW }{ ''.join(out) }"
     # Extra leading dot to allow unconditional trim in JS, later...
 
+    if DebugConfig.check_decode:
+        decoded = decode_LZW(output_with_table)
+        if decoded != txt:
+            alpha = ''.join(sorted(set(txt)))
+            i = next(
+                (i for i,(a,b) in enumerate(zip(txt,decoded)) if a!=b),
+                min(len(txt), len(decoded))
+            )
+            (Path.cwd() / "encoded").write_text(output_with_table.replace('\x1e', '\n'), encoding='utf-8')
+            raise BuildError(f'''Failed to decode...
+Alpha: ]]{ alpha }[[ (len={len(alpha)})
+        { [*map(ord,alpha)] }
+
+table: len={len(dct)}
+{size=} | BASE**size = {BASE**size}
+
+source: len={len(txt)}
+back:   len={len(decoded)}
+Differ: {i=}
+
+source[i-50:i]:
+{ txt[i-50:i] }
+
+source[i:i+200]:
+{ txt[i:i+200]}
+
+source[i:i+200]:
+{decoded[i:i+200]}
+
+''')
+
+
     # MEAN.append((len(txt),len(out)))
     return output_with_table
 
 
 
+BASE_TOME = {c:i for i,c in enumerate(TOME_BASE)}
+def un_i_to_base(s:str):
+    v = 0
+    for c in s: v = BASE*v + BASE_TOME[c]
+    return v
+
+
+def decode_LZW(compressed:str):
+
+    big,small,*chunks = compressed.strip().split(LZW)
+    big = big[1:]
+    tome = [*'><'] + [chr(int(s)) for s in big and big.split('.')] + [*small]
+
+    txt,size = [],1
+    for chunk in chunks:
+        size += 1
+        assert not len(chunk)%size, (len(chunk), size, len(chunk)%size)
+        txt.extend( un_i_to_base(chunk[i:i+size]) for i in range(0, len(chunk), size) )
+
+    out = []
+    for i,idx in enumerate(txt):
+        w = tome[idx]
+        fresh = '' if i+1==len(txt) else w + ( w if txt[i+1]==len(tome) else tome[txt[i+1]] )[0]
+        # https://mooc-forums.inria.fr/moocnsi/t/question-lzw-cas-particulier-decompression/11491/2
+        out.append(w)
+        tome.append(fresh)
+
+    return ''.join(out)
+
+
 
 
 
 
 def build_code_fence(
     content:str,
     indent:str="",
```

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,7 +331,14 @@
 }
 
 
 BLOCKS_KINDS = set('content libs scripts extrahead'.split())
 INSERTIONS_KINDS = {s for s in dir(ScriptKind) if not s.startswith('_')
                                                and not callable(getattr(ScriptKind, s)) }
 PAGES_KINDS = INSERTIONS_KINDS - BLOCKS_KINDS
+
+
+class DebugConfig(Namespace):
+    check_decoding = False
+    """ If True, decode any LZW encoded string to check consistency """
+    shuffle = False
+    check_decode = True
```

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/mkdocs.yml` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/scripts/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/model.py` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/scripts/model.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/README.md` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -272,14 +272,15 @@
  *      1. dot separated unicode char codes
  *      2. regular alpha
  *      3. compressed data, size 2
  *      4. ..., size 3,
  *      5. ...
  */
 const decompressLZW = (compressed) => {
+    return compressed
 
     const [bigs, smalls, ...chunks] = compressed.trim().split(CONFIG.LZW)
     const tome = [
         [...'><'],
         bigs == '.' ? [] : bigs.slice(1) // no initial dot
         .split('.')
         .map(n => String.fromCodePoint(+n)),
```

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css`

 * *Files 2% similar despite different names*

```diff
@@ -130,28 +130,30 @@
 ------------------------
 */
 
 .ide_buttons_div_wrapper {
   display: grid;
   grid-template-columns: max-content auto;
 }
+.ide_buttons_div {
+  z-index: 2;
+}
 
 .compteur_wrapper {
   justify-self: end;
   width: 100%;
   display: grid;
 }
 
 .py_mk_ide .compteur {
   justify-self: end;
   position: absolute;
   float: right;
   color: var(--main-theme);
   font-size: 1.2em;
-  z-index: -1;
   width: max-content;
 }
 
 .py_mk_ide .compteur_txt {
   font-size: 0.8em
 }
```

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css` & `pyodide_mkdocs_theme-1.0.2/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.1/pyproject.toml` & `pyodide_mkdocs_theme-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "1.0.1"
+version = "1.0.2"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-1.0.1/PKG-INFO` & `pyodide_mkdocs_theme-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

