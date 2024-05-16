# Comparing `tmp/pyodide_mkdocs_theme-1.0.0.tar.gz` & `tmp/pyodide_mkdocs_theme-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-1.0.0.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-1.0.1.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-1.0.0.tar` & `pyodide_mkdocs_theme-1.0.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-1.0.0/README.md
--rw-r--r--   0        0        0     1347 2024-05-15 21:11:40.512726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2591 2024-05-10 09:58:57.896751 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-05-15 21:11:40.564727 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0     1322 2024-05-10 09:58:57.908752 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
--rw-r--r--   0        0        0     1063 2024-05-10 09:58:57.944753 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-05-12 18:52:50.335028 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     5919 2024-05-14 21:00:36.843691 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     2992 2024-05-14 21:00:36.843691 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py
--rw-r--r--   0        0        0        0 2024-05-10 09:58:57.968754 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0    11922 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py
--rw-r--r--   0        0        0    16534 2024-05-10 09:58:58.012755 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py
--rw-r--r--   0        0        0    21130 2024-05-14 21:00:36.899692 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py
--rw-r--r--   0        0        0     4850 2024-05-14 21:00:36.899692 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py
--rw-r--r--   0        0        0     3470 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py
--rw-r--r--   0        0        0     2435 2024-05-10 09:58:58.072757 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11591 2024-05-10 09:58:58.072757 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    13668 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     7141 2024-05-11 20:11:49.116411 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0    14460 2024-05-14 21:00:36.971694 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4776 2024-05-14 21:00:37.003695 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0        0 2024-05-10 09:58:58.128759 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    15211 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11391 2024-05-14 21:00:37.003695 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0     9693 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
--rw-r--r--   0        0        0     1603 2024-05-10 09:58:58.168760 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     6652 2024-05-10 09:58:58.188760 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
--rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9042 2024-05-14 21:00:37.039696 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1163 2024-05-14 21:00:37.075698 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     9480 2024-05-15 20:46:22.156139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0     4229 2024-05-15 21:11:40.512726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     5487 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/mkdocs.yml
--rw-r--r--   0        0        0     3593 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/model.py
--rw-r--r--   0        0        0      823 2024-05-10 09:58:58.304764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/README.md
--rw-r--r--   0        0        0        0 2024-05-10 09:58:58.304764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     2857 2024-05-10 09:58:58.304764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg
--rw-r--r--   0        0        0     1645 2024-05-10 09:58:58.304764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-05-10 09:58:58.308764 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png
--rw-r--r--   0        0        0     6093 2024-05-15 20:46:22.160139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0    10609 2024-05-14 21:00:37.167700 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1770 2024-05-15 21:11:37.872664 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0    10814 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js
--rw-r--r--   0        0        0    14528 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js
--rw-r--r--   0        0        0     1183 2024-05-15 21:11:40.508726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js
--rw-r--r--   0        0        0     8220 2024-05-15 21:11:40.508726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js
--rw-r--r--   0        0        0    18519 2024-05-15 21:11:40.508726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js
--rw-r--r--   0        0        0    12716 2024-05-10 09:58:58.344765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js
--rw-r--r--   0        0        0     7231 2024-05-14 21:00:37.171700 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js
--rw-r--r--   0        0        0    11253 2024-05-10 09:58:58.344765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js
--rw-r--r--   0        0        0     4455 2024-05-14 21:00:37.195701 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0     5341 2024-05-10 09:58:58.344765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     2635 2024-05-15 21:11:40.504726 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     3831 2024-05-10 09:58:58.356765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css
--rw-r--r--   0        0        0     1078 2024-05-10 09:58:58.356765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css
--rw-r--r--   0        0        0     1947 2024-05-10 09:58:58.356765 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css
--rw-r--r--   0        0        0     3744 2024-05-15 20:46:22.160139 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css
--rw-r--r--   0        0        0     3904 2024-05-10 09:58:58.364766 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css
--rw-r--r--   0        0        0     1918 2024-05-14 21:00:37.255703 pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css
--rw-r--r--   0        0        0     1766 2024-05-15 21:11:37.908665 pyodide_mkdocs_theme-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-1.0.1/README.md
+-rw-r--r--   0        0        0     1347 2024-05-16 18:53:21.067527 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2591 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-16 18:53:21.103528 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1322 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0     1063 2024-05-15 21:11:56.293098 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-05-12 18:52:50.335028 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     5919 2024-05-15 21:11:56.321099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     2992 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0    11922 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py
+-rw-r--r--   0        0        0    16534 2024-05-15 21:11:56.337099 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py
+-rw-r--r--   0        0        0    21130 2024-05-15 21:11:56.369100 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py
+-rw-r--r--   0        0        0     4850 2024-05-15 21:11:56.377100 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py
+-rw-r--r--   0        0        0     3470 2024-05-15 21:11:56.377100 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py
+-rw-r--r--   0        0        0     2435 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11591 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13668 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     7141 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0    14460 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4776 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    15211 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11391 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0     9693 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
+-rw-r--r--   0        0        0     1603 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     6652 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
+-rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9042 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1163 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     9480 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0     4229 2024-05-16 18:53:21.063527 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     5487 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/mkdocs.yml
+-rw-r--r--   0        0        0     3593 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/model.py
+-rw-r--r--   0        0        0      823 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg
+-rw-r--r--   0        0        0     1645 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     6093 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0    10609 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1770 2024-05-16 18:53:18.103440 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0    10814 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js
+-rw-r--r--   0        0        0    14528 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js
+-rw-r--r--   0        0        0     1183 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js
+-rw-r--r--   0        0        0     8220 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js
+-rw-r--r--   0        0        0    18519 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js
+-rw-r--r--   0        0        0    12716 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js
+-rw-r--r--   0        0        0     7231 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js
+-rw-r--r--   0        0        0    11253 2024-05-15 21:11:56.481103 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0     4455 2024-05-15 21:11:56.489103 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0     5341 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     2635 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     3831 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css
+-rw-r--r--   0        0        0     1078 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css
+-rw-r--r--   0        0        0     1947 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css
+-rw-r--r--   0        0        0     3744 2024-05-16 18:51:04.803499 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css
+-rw-r--r--   0        0        0     3904 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css
+-rw-r--r--   0        0        0     1918 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css
+-rw-r--r--   0        0        0     1766 2024-05-16 18:53:18.139441 pyodide_mkdocs_theme-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-1.0.1/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-1.0.0/LICENSE` & `pyodide_mkdocs_theme-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/README.md` & `pyodide_mkdocs_theme-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/mkdocs.yml` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/scripts/model.py` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/scripts/model.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/README.md` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css` & `pyodide_mkdocs_theme-1.0.1/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.0/pyproject.toml` & `pyodide_mkdocs_theme-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "1.0.0"
+version = "1.0.1"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-1.0.0/PKG-INFO` & `pyodide_mkdocs_theme-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

