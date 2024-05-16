# Comparing `tmp/libreflow_launcher-1.0.6.tar.gz` & `tmp/libreflow_launcher-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_launcher-1.0.6.tar", last modified: Tue May  7 05:52:33 2024, max compression
+gzip compressed data, was "libreflow_launcher-1.0.7.tar", last modified: Wed May 15 17:46:33 2024, max compression
```

## Comparing `libreflow_launcher-1.0.6.tar` & `libreflow_launcher-1.0.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.347470 libreflow_launcher-1.0.6/
--rw-rw-rw-   0 root         (0) root         (0)     1495 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2284 2024-05-07 05:52:33.347470 libreflow_launcher-1.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-07 05:52:33.347470 libreflow_launcher-1.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1691 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.333470 libreflow_launcher-1.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.337470 libreflow_launcher-1.0.6/src/libreflow_launcher/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-07 05:52:33.348470 libreflow_launcher-1.0.6/src/libreflow_launcher/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    18949 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.338470 libreflow_launcher-1.0.6/src/libreflow_launcher/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.338470 libreflow_launcher-1.0.6/src/libreflow_launcher/data/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/data/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/gui.py
--rw-rw-rw-   0 root         (0) root         (0)     6139 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/model.py
--rw-rw-rw-   0 root         (0) root         (0)     7983 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.339470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.341470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   503824 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   445528 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   579296 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
--rw-rw-rw-   0 root         (0) root         (0)   528976 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/OpenSans.ttf
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.341470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.346470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5628 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/arrow-down.png
--rw-rw-rw-   0 root         (0) root         (0)     5667 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     9732 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/close.png
--rw-rw-rw-   0 root         (0) root         (0)     9850 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/gitlab.svg
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/kitsu.svg
--rw-rw-rw-   0 root         (0) root         (0)     8760 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
--rw-rw-rw-   0 root         (0) root         (0)     7267 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/open.png
--rw-rw-rw-   0 root         (0) root         (0)    10491 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/pypi.svg
--rw-rw-rw-   0 root         (0) root         (0)    17905 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/server.png
--rw-rw-rw-   0 root         (0) root         (0)    13119 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/settings.png
--rw-rw-rw-   0 root         (0) root         (0)    19182 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/settings_outline.png
--rw-rw-rw-   0 root         (0) root         (0)     5851 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/start.png
--rw-rw-rw-   0 root         (0) root         (0)     7946 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash.png
--rw-rw-rw-   0 root         (0) root         (0)     8358 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     7996 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash_normal.png
--rw-rw-rw-   0 root         (0) root         (0)    11968 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/user.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.346470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.346470 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/default/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/default/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/default/default_style.css
--rw-rw-rw-   0 root         (0) root         (0)    56780 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/src/libreflow_launcher/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:52:33.347470 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2284 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2191 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-07 05:52:33.000000 libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-07 05:52:24.000000 libreflow_launcher-1.0.6/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.043801 libreflow_launcher-1.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-05-15 17:46:33.043801 libreflow_launcher-1.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-15 17:46:33.043801 libreflow_launcher-1.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.028802 libreflow_launcher-1.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.032801 libreflow_launcher-1.0.7/src/libreflow_launcher/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-15 17:46:33.044802 libreflow_launcher-1.0.7/src/libreflow_launcher/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    20859 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.033801 libreflow_launcher-1.0.7/src/libreflow_launcher/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.033801 libreflow_launcher-1.0.7/src/libreflow_launcher/data/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/data/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7983 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.033801 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.037801 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   503824 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   445528 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   579296 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   528976 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/OpenSans.ttf
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.037801 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.042801 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5628 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/arrow-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/arrow-right.png
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     9732 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/close.png
+-rw-rw-rw-   0 root         (0) root         (0)     9850 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/gitlab.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/kitsu.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8760 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/log-out.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/open.png
+-rw-rw-rw-   0 root         (0) root         (0)    10491 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/pypi.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17905 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/server.png
+-rw-rw-rw-   0 root         (0) root         (0)    13119 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/settings.png
+-rw-rw-rw-   0 root         (0) root         (0)    19182 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/settings_outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/start.png
+-rw-rw-rw-   0 root         (0) root         (0)     7946 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/trash.png
+-rw-rw-rw-   0 root         (0) root         (0)     8358 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/trash_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     7996 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/trash_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)    11968 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/user.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.042801 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.042801 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/styles/default/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/styles/default/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/ui/styles/default/default_style.css
+-rw-rw-rw-   0 root         (0) root         (0)    57039 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/src/libreflow_launcher/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:46:33.043801 libreflow_launcher-1.0.7/src/libreflow_launcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-05-15 17:46:32.000000 libreflow_launcher-1.0.7/src/libreflow_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2191 2024-05-15 17:46:32.000000 libreflow_launcher-1.0.7/src/libreflow_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 17:46:32.000000 libreflow_launcher-1.0.7/src/libreflow_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-15 17:46:32.000000 libreflow_launcher-1.0.7/src/libreflow_launcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-15 17:46:32.000000 libreflow_launcher-1.0.7/src/libreflow_launcher.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-15 17:46:23.000000 libreflow_launcher-1.0.7/versioneer.py
```

### Comparing `libreflow_launcher-1.0.6/PKG-INFO` & `libreflow_launcher-1.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.6
+Version: 1.0.7
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,29 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.7] - 2024-05-15
+
+### Fixed
+
+* Issue #11
+  * Added a exception for `HTTPError` and `RequestException` to avoid crashes when connection or authentification error has occured.
+  * Handle recent changes of Overseer API error codes for user token.
+  * Current user cache is now cleared when user token is invalid or expired.
+* Issue #7
+  * Current user is now properly setted when user settings folder do not exist.
+* Issue #14
+  * Append libreflow extensions with the correct pattern in the environment variable.
+
+* Connection status to a server is updated when hovering a server.
+
 ## [1.0.6] - 2024-05-07
 
 ### Added
 
 * Shell script to start a Libreflow instance on Linux.
 
 ## [1.0.5] - 2024-04-29
```

### Comparing `libreflow_launcher-1.0.6/README.md` & `libreflow_launcher-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/setup.py` & `libreflow_launcher-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/controller.py` & `libreflow_launcher-1.0.7/src/libreflow_launcher/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,41 +32,71 @@
 
     def __init__(self, servers, projects, settings):
         self._servers = servers
         self._projects = projects
         self._settings = settings
 
     def api_get(self, route, json):
-        resp = requests.get(
-            self.BASE_URL + route, json=json,
-            headers=self.CONFIG['headers']
-        )
-        resp.raise_for_status()
-        return resp.json()
+        try:
+            resp = requests.get(
+                self.BASE_URL + route, json=json,
+                headers=self.CONFIG['headers']
+            )
+            resp.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            return resp.json()
+        except requests.exceptions.RequestException as err:
+            print(f'ERROR: {err}')
+            return None
+        else:
+            return resp.json()
 
     def api_post(self, route, json):
-        resp = requests.post(
-            self.BASE_URL + route, json=json,
-            headers=self.CONFIG['headers']
-        )
-        resp.raise_for_status()
-        return resp.json()
+        try:
+            resp = requests.post(
+                self.BASE_URL + route, json=json,
+                headers=self.CONFIG['headers']
+            )
+            resp.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            return resp.json()
+        except requests.exceptions.RequestException as err:
+            print(f'ERROR: {err}')
+            return None
+        else:
+            return resp.json()
 
     def api_patch(self, route, json):
-        resp = requests.patch(
-            self.BASE_URL + route, json=json,
-            headers=self.CONFIG['headers']
-        )
-        resp.raise_for_status()
-        return resp.json()
+        try:
+            resp = requests.patch(
+                self.BASE_URL + route, json=json,
+                headers=self.CONFIG['headers']
+            )
+            resp.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            return resp.json()
+        except requests.exceptions.RequestException as err:
+            print(f'ERROR: {err}')
+            return None
+        else:
+            return resp.json()
 
     def get_token(self, data: dict) -> str:
-        resp = requests.post(self.BASE_URL + '/token', data=data)
-        resp.raise_for_status()
-        return resp.json()
+        try:
+            resp = requests.post(
+                self.BASE_URL + '/token', data=data
+            )
+            resp.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            return resp.json()
+        except requests.exceptions.RequestException as err:
+            print(f'ERROR: {err}')
+            return None
+        else:
+            return resp.json()
 
 
     def set_current_host(self, uid=None):
         user_settings_folder = self.user_settings_folder()
         if not os.path.exists(user_settings_folder):
             os.makedirs(user_settings_folder)
 
@@ -76,14 +106,15 @@
                 f = open(f"{user_settings_folder}/current_host.json", "r")
             except IOError:
                 return
             else:
                 data = json.load(f)
                 uid = data['uid']
                 restore = True
+                f.close()
 
         server = self._servers.fetch_server(uid)
 
         self.BASE_URL = f'http://{server["api_host"]}:{server["api_port"]}'
         self.server_name = server["display_name"]
         self.server_uid = uid
 
@@ -92,20 +123,25 @@
                 json.dump(dict(
                     uid=self.server_uid
                 ), f)
 
     def log_in(self, login, password):
         token = self.get_token({'username': login, 'password': password})
 
-        if 'detail' in token and token['detail'] == "invalid-auth":
+        if token is None:
+            print(f'ERROR: Connection failed to {self.server_name} server, {self.BASE_URL}')
+            return False
+        elif 'detail' in token and token['detail'] == "invalid-auth":
             print(f'ERROR: Authentification invalid to {self.server_name} server, {self.BASE_URL}')
             return False
 
         self.CONFIG['headers'] = {
-            'Authorization': 'Bearer {}'.format(token['access_token'])}
+            'Authorization': 'Bearer {}'.format(token['access_token'])
+        }
+        self.current_user = login
 
         user_settings_folder = self.user_settings_folder()
         if not os.path.exists(user_settings_folder):
             os.makedirs(user_settings_folder)
 
         server_folder = f"{user_settings_folder}/servers/{self.server_uid}"
         if not os.path.exists(server_folder):
@@ -132,43 +168,55 @@
         if os.path.exists(user_path):
             os.remove(user_path)
         
         print('INFO: Logged out')
 
     def check_log_in(self):
         logged_in = True
+        user_path = f"{self.user_settings_folder()}/servers/{self.server_uid}/current_user.json"
+        
         try:
-            f = open(f"{self.user_settings_folder()}/servers/{self.server_uid}/current_user.json", "r")
+            f = open(user_path, "r")
         except IOError:
             logged_in = False
         else:
             config = json.load(f)
             self.CONFIG['headers'] = {
                 'Authorization': 'Bearer {}'.format(config['access_token'])
             }
+            f.close()
 
             test_command = self.api_get('/versions', json={})
-            if test_command[0] == 'Not authenticated':
+            
+            if test_command is None:
+                logged_in = False
+                print(f'ERROR: Connection failed to {self.server_name} server, {self.BASE_URL}')
+            elif 'detail' in test_command and (test_command['detail'] == "invalid-token" or test_command['detail'] == "expired-token"):
                 logged_in = False
-                print(f'INFO: Token expired for {self.server_name} server, {self.BASE_URL}')
+                print(f'ERROR: Token expired for {self.server_name} server, {self.BASE_URL}')
             else:
                 self.current_user = config['name']
+            
+            if not logged_in:
+                self.CONFIG = {'headers': None}
+                os.remove(user_path)
 
         if logged_in:
             print(f'INFO: Connected to {self.server_name} server, {self.BASE_URL}')
 
         return logged_in
 
     def fetch_user_name(self, uid):
         try:
             f = open(f"{self.user_settings_folder()}/servers/{uid}/current_user.json", "r")
         except IOError:
             return None
         else:
             config = json.load(f)
+            f.close()
             return config['name']
 
 
     def fetch_servers(self):
         return self._servers.fetch_servers()
     
     def update_server(self, data, uid=None):
@@ -385,15 +433,18 @@
         if data_resolve:
             update = True
 
             # Format Kabaret Flow Extensions argument
             extensions = []
             for extension in data_resolve['extensions']:
                 if 'extension' in extension['categories']:
-                    extensions.append(f'libreflow.extensions.{extension["name"]}:install_extensions')
+                    if "libreflow.extensions" not in extension["name"]:
+                        extensions.append(f'libreflow.extensions.{extension["name"]}:install_extensions')
+                    else:
+                        extensions.append(f'{extension["name"]}:install_extensions')
 
             # Format launch command with arguments
             cmd = [
                 self.poetry_path,
                 "run",
                 "python",
                 "-m",
```

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/gui.py` & `libreflow_launcher-1.0.7/src/libreflow_launcher/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/model.py` & `libreflow_launcher-1.0.7/src/libreflow_launcher/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         try:
             f = open(f"{user_settings_folder()}/user_servers_order.json", "r")
         except IOError:
             pass
         else:
             user_data = json.load(f)['uid_list']
             self._servers = sorted(self._servers, key=lambda s: user_data.index(s['uid']))
+            f.close()
 
         print(f'INFO: Fetch {len(self._servers)} servers')
         return self._servers
 
     def fetch_server(self, uid):
         item = [s for s in self._servers if s['uid'] == uid]
         return item[0]
```

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/resources.py` & `libreflow_launcher-1.0.7/src/libreflow_launcher/resources.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/fonts/OpenSans.ttf` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/fonts/OpenSans.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/arrow-down.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/arrow-down.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/arrow-right.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/arrow-right.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/close.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/close.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/gitlab.svg` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/gitlab.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/kitsu.svg` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/kitsu.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/log-out.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out_hover.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/log-out_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/log-out_normal.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/log-out_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/open.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/open.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/pypi.svg` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/pypi.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/server.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/server.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/settings.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/settings.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/settings_outline.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/settings_outline.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/start.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/start.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/trash.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash_hover.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/trash_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/trash_normal.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/trash_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/icons/gui/user.png` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/icons/gui/user.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/ui/styles/default/default_style.css` & `libreflow_launcher-1.0.7/src/libreflow_launcher/ui/styles/default/default_style.css`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher/view.py` & `libreflow_launcher-1.0.7/src/libreflow_launcher/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,16 @@
                 self.projects.show()
                 if init:
                     self.notification_header.pop('Connected', 'valid', True)
             else:
                 self.login.build()
                 self.login.show()
                 self.projects.hide()
+                if self.menu_bar.servers.current_item:
+                    self.menu_bar.servers.current_item.refresh()
             
             return
         
         if redirect == 'settings':
             self.settings_bar.list.refresh(True)
             if self.settings_bar.list.current_item.text() != 'Global':
                 self.settings_bar.list.setSelected(self.settings_bar.list.layout.itemAt(0).widget())
@@ -1063,14 +1065,15 @@
         super(ServerItem, self).__init__()
         self.setFixedHeight(45)
 
         self.servers_list = servers_list
         self._data = data
         self._current_user = current_user
         self._mw = servers_list._mw
+        self._ctrl = servers_list._ctrl
 
         self.setWindowFlags(QtCore.Qt.FramelessWindowHint)
         self.setAttribute(QtCore.Qt.WA_TranslucentBackground)
             
         # shadow = QtWidgets.QGraphicsDropShadowEffect(self)
         # shadow.setBlurRadius(40)
         # shadow.setXOffset(0)
@@ -1104,14 +1107,17 @@
         self.arrow.setAlignment(QtCore.Qt.AlignCenter)
         self.arrow.setFixedSize(15,15)
         self.arrow.setStyleSheet('border-radius: 7px; background-color: #5553ac;')
         self.arrow.installEventFilter(self)
         container.addWidget(self.arrow, 0, 0, alignment=QtCore.Qt.AlignRight)
         self.arrow.hide()
 
+    def refresh(self):
+        self._current_user = self._ctrl.fetch_user_name(self._data['uid'])
+
     def setSelected(self):
         if not self.circle.property('selected'):
             self.circle.setProperty('selected', True)
             self.text.setProperty('selected', True)
             self.arrow.show()
         else:
             self.circle.setProperty('selected', False)
```

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/PKG-INFO` & `libreflow_launcher-1.0.7/src/libreflow_launcher.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.6
+Version: 1.0.7
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,29 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.7] - 2024-05-15
+
+### Fixed
+
+* Issue #11
+  * Added a exception for `HTTPError` and `RequestException` to avoid crashes when connection or authentification error has occured.
+  * Handle recent changes of Overseer API error codes for user token.
+  * Current user cache is now cleared when user token is invalid or expired.
+* Issue #7
+  * Current user is now properly setted when user settings folder do not exist.
+* Issue #14
+  * Append libreflow extensions with the correct pattern in the environment variable.
+
+* Connection status to a server is updated when hovering a server.
+
 ## [1.0.6] - 2024-05-07
 
 ### Added
 
 * Shell script to start a Libreflow instance on Linux.
 
 ## [1.0.5] - 2024-04-29
```

### Comparing `libreflow_launcher-1.0.6/src/libreflow_launcher.egg-info/SOURCES.txt` & `libreflow_launcher-1.0.7/src/libreflow_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.6/versioneer.py` & `libreflow_launcher-1.0.7/versioneer.py`

 * *Files identical despite different names*

