# Comparing `tmp/libreflow_flows-2.3.0.tar.gz` & `tmp/libreflow_flows-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_flows-2.3.0.tar", last modified: Fri Apr 26 14:43:21 2024, max compression
+gzip compressed data, was "libreflow_flows-2.3.1.tar", last modified: Thu May 16 12:26:25 2024, max compression
```

## Comparing `libreflow_flows-2.3.0.tar` & `libreflow_flows-2.3.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.455455 libreflow_flows-2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)     4940 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5866 2024-04-26 14:43:21.455455 libreflow_flows-2.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-04-26 14:43:21.455455 libreflow_flows-2.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2116 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.440456 libreflow_flows-2.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.444455 libreflow_flows-2.3.0/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.455455 libreflow_flows-2.3.0/src/libreflow/flows/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-04-26 14:43:21.455455 libreflow_flows-2.3.0/src/libreflow/flows/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.446456 libreflow_flows-2.3.0/src/libreflow/flows/custom_home/
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/custom_home/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7386 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/custom_home/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.447456 libreflow_flows-2.3.0/src/libreflow/flows/default/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.448455 libreflow_flows-2.3.0/src/libreflow/flows/default/flow/
--rw-rw-rw-   0 root         (0) root         (0)     7380 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/default/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5768 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/default/flow/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/default/flow/entity_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    16548 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/default/flow/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/default/flow/film.py
--rw-rw-rw-   0 root         (0) root         (0)     2757 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/default/flow/shot.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/default/flow/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7961 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/default/flow/user.py
--rw-rw-rw-   0 root         (0) root         (0)     5739 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.448455 libreflow_flows-2.3.0/src/libreflow/flows/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.449456 libreflow_flows-2.3.0/src/libreflow/flows/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   149688 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/file_templates/template.blend
--rw-rw-rw-   0 root         (0) root         (0)    88244 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/file_templates/template.wav
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.450456 libreflow_flows-2.3.0/src/libreflow/flows/resources/gifs/
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/gifs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   744158 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/gifs/magic_word.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.451455 libreflow_flows-2.3.0/src/libreflow/flows/resources/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.451455 libreflow_flows-2.3.0/src/libreflow/flows/resources/gui/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/gui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.451455 libreflow_flows-2.3.0/src/libreflow/flows/resources/gui/styles/default_style/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/gui/styles/default_style/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/resources/gui/styles/default_style/default_style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.451455 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.453456 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/
--rw-rw-rw-   0 root         (0) root         (0)     5702 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13809 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/file.py
--rw-rw-rw-   0 root         (0) root         (0)    45139 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/film.py
--rw-rw-rw-   0 root         (0) root         (0)    22662 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3125 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.453456 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.453456 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    94110 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/file_templates/template.blend
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.454455 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.454455 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/icons/flow/
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/icons/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:43:21.454455 libreflow_flows-2.3.0/src/libreflow.flows.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5866 2024-04-26 14:43:21.000000 libreflow_flows-2.3.0/src/libreflow.flows.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2072 2024-04-26 14:43:21.000000 libreflow_flows-2.3.0/src/libreflow.flows.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 14:43:21.000000 libreflow_flows-2.3.0/src/libreflow.flows.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-26 14:43:21.000000 libreflow_flows-2.3.0/src/libreflow.flows.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 14:43:21.000000 libreflow_flows-2.3.0/src/libreflow.flows.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    80044 2024-04-26 14:43:12.000000 libreflow_flows-2.3.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.837632 libreflow_flows-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)     5167 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6093 2024-05-16 12:26:25.837632 libreflow_flows-2.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-05-16 12:26:25.837632 libreflow_flows-2.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.821632 libreflow_flows-2.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.825632 libreflow_flows-2.3.1/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.837632 libreflow_flows-2.3.1/src/libreflow/flows/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-05-16 12:26:25.837632 libreflow_flows-2.3.1/src/libreflow/flows/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.828632 libreflow_flows-2.3.1/src/libreflow/flows/custom_home/
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/custom_home/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7386 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/custom_home/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.828632 libreflow_flows-2.3.1/src/libreflow/flows/default/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.830632 libreflow_flows-2.3.1/src/libreflow/flows/default/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     7380 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/default/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5768 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/default/flow/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/default/flow/entity_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    16548 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/default/flow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/default/flow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)     2757 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/default/flow/shot.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/default/flow/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7961 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/default/flow/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     6711 2024-05-16 12:26:15.000000 libreflow_flows-2.3.1/src/libreflow/flows/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.830632 libreflow_flows-2.3.1/src/libreflow/flows/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.831632 libreflow_flows-2.3.1/src/libreflow/flows/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   149688 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/file_templates/template.blend
+-rw-rw-rw-   0 root         (0) root         (0)    88244 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/file_templates/template.wav
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.831632 libreflow_flows-2.3.1/src/libreflow/flows/resources/gifs/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/gifs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   744158 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/gifs/magic_word.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.832632 libreflow_flows-2.3.1/src/libreflow/flows/resources/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.833632 libreflow_flows-2.3.1/src/libreflow/flows/resources/gui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/gui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.833632 libreflow_flows-2.3.1/src/libreflow/flows/resources/gui/styles/default_style/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8358 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.833632 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.834632 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     5702 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13809 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)    45139 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)    22662 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.835632 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.835632 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    94110 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.835632 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.836632 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/icons/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/icons/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 12:26:25.836632 libreflow_flows-2.3.1/src/libreflow.flows.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6093 2024-05-16 12:26:25.000000 libreflow_flows-2.3.1/src/libreflow.flows.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-16 12:26:25.000000 libreflow_flows-2.3.1/src/libreflow.flows.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 12:26:25.000000 libreflow_flows-2.3.1/src/libreflow.flows.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-16 12:26:25.000000 libreflow_flows-2.3.1/src/libreflow.flows.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-16 12:26:25.000000 libreflow_flows-2.3.1/src/libreflow.flows.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2024-05-16 12:26:16.000000 libreflow_flows-2.3.1/versioneer.py
```

### Comparing `libreflow_flows-2.3.0/CHANGELOG.md` & `libreflow_flows-2.3.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.3.1] - 2024-05-16
+
+### Added
+
+* New session option to redefine its home oid. This oid can be provided either using the command line argument `--home-oid` or through the environment using the variable `KABARET_HOME_OID`.
+
 ## [2.3.0] - 2024-04-26
 
 ### Added
 
 The session now uses the new Kabaret's layout manager which is enabled by default with the session autosave feature.
 
 ## [2.2.0] - 2024-04-26
```

### Comparing `libreflow_flows-2.3.0/LICENSE` & `libreflow_flows-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/PKG-INFO` & `libreflow_flows-2.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.flows
-Version: 2.3.0
+Version: 2.3.1
 Summary: A set of flows specific to projects handled by Libreflow at Les Fées Spéciales.
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow.flows
 Author: Baptiste Delos, Flavio Perez
 Author-email: baptiste@les-fees-speciales.coop, flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -37,14 +37,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.3.1] - 2024-05-16
+
+### Added
+
+* New session option to redefine its home oid. This oid can be provided either using the command line argument `--home-oid` or through the environment using the variable `KABARET_HOME_OID`.
+
 ## [2.3.0] - 2024-04-26
 
 ### Added
 
 The session now uses the new Kabaret's layout manager which is enabled by default with the session autosave feature.
 
 ## [2.2.0] - 2024-04-26
```

### Comparing `libreflow_flows-2.3.0/setup.py` & `libreflow_flows-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/custom_home/__init__.py` & `libreflow_flows-2.3.1/src/libreflow/flows/custom_home/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/custom_home/ui.py` & `libreflow_flows-2.3.1/src/libreflow/flows/custom_home/ui.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/default/flow/__init__.py` & `libreflow_flows-2.3.1/src/libreflow/flows/default/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/default/flow/asset.py` & `libreflow_flows-2.3.1/src/libreflow/flows/default/flow/asset.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/default/flow/entity_manager.py` & `libreflow_flows-2.3.1/src/libreflow/flows/default/flow/entity_manager.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/default/flow/file.py` & `libreflow_flows-2.3.1/src/libreflow/flows/default/flow/file.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/default/flow/film.py` & `libreflow_flows-2.3.1/src/libreflow/flows/default/flow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/default/flow/shot.py` & `libreflow_flows-2.3.1/src/libreflow/flows/default/flow/shot.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/default/flow/user.py` & `libreflow_flows-2.3.1/src/libreflow/flows/default/flow/user.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/gui.py` & `libreflow_flows-2.3.1/src/libreflow/flows/gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,14 +99,34 @@
             type_name = self.register_view_type(JobsView)
             self.add_view(
                 type_name,
                 hidden=not DEBUG,
                 area=QtCore.Qt.RightDockWidgetArea,
             )
 
+    def set_home_oid(self, home_oid):
+        if home_oid is None:
+            home_oid = os.environ.get('KABARET_HOME_OID')
+            if home_oid is None:
+                return
+            self.log_info(f"Home oid from environment: {home_oid}")
+
+        if not home_oid.startswith('/'):
+            # Project name provided: turn into oid
+            home_oid = '/'+home_oid
+        project_name = home_oid.split('/', 2)[1]
+        # Check project separately since undefined name raises an error
+        has_project = self.get_actor('Flow').has_project(project_name)
+        if not has_project or not self.cmds.Flow.exists(home_oid):
+            self.log_warning(f"Home oid {home_oid} not found: fall back to default")
+            return
+
+        self.log_info(f"Set home oid to {home_oid}")
+        self.cmds.Flow.set_home_oid(home_oid)
+
     def _create_actors(self):
         '''
         Instanciate the session actors.
         Subclasses can override this to install customs actors or
         replace default ones.
         '''
         if CUSTOM_HOME:
@@ -128,14 +148,17 @@
     parser.add_argument(
         '-u', '--user', dest='user'
     )
     parser.add_argument(
         '-s', '--site', default='LFS', dest='site'
     )
     parser.add_argument(
+        '--home-oid', dest='home_oid'
+    )
+    parser.add_argument(
         '-j', '--jobs_default_filter', dest='jobs_default_filter'
     )
     parser.add_argument(
         '--search-index-uri', dest='search_index_uri'
     )
     parser.add_argument(
         '--search-auto-indexing', dest='search_auto_indexing', nargs='?', const=True, type=bool
@@ -150,15 +173,15 @@
         os.environ['JOBS_DEFAULT_FILTER'] = values.jobs_default_filter
     else:
         os.environ['JOBS_DEFAULT_FILTER'] = values.site
     
     if values.search_auto_indexing is None:
         values.search_auto_indexing = 'SEARCH_AUTO_INDEXING' in os.environ
     
-    return values.search_index_uri, values.search_auto_indexing
+    return values.search_index_uri, values.search_auto_indexing, values.home_oid
 
 
 def main(argv):
     (
         session_name,
         host,
         port,
@@ -167,23 +190,23 @@
         password,
         debug,
         layout_mgr,
         layout_autosave,
         layout_savepath,
         remaining_args,
     ) = SessionGUI.parse_command_line_args(argv)
-
-    uri, auto_indexing = process_remaining_args(remaining_args)
+    uri, auto_indexing, home_oid = process_remaining_args(remaining_args)
 
     session = SessionGUI(
         session_name=session_name, debug=debug,
         layout_mgr=layout_mgr, layout_autosave=layout_autosave, layout_savepath=layout_savepath,
         search_index_uri=uri, search_auto_indexing=auto_indexing
     )
     session.cmds.Cluster.connect(host, port, cluster_name, db, password)
+    session.set_home_oid(home_oid)
 
     session.start()
     session.close()
 
 
 if __name__ == '__main__':
     main(sys.argv[1:])
```

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/resources/file_templates/template.blend` & `libreflow_flows-2.3.1/src/libreflow/flows/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/resources/file_templates/template.wav` & `libreflow_flows-2.3.1/src/libreflow/flows/resources/file_templates/template.wav`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/resources/gifs/magic_word.gif` & `libreflow_flows-2.3.1/src/libreflow/flows/resources/gifs/magic_word.gif`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/resources/gui/styles/default_style/__init__.py` & `libreflow_flows-2.3.1/src/libreflow/flows/resources/gui/styles/default_style/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/resources/gui/styles/default_style/default_style.css` & `libreflow_flows-2.3.1/src/libreflow/flows/resources/gui/styles/default_style/default_style.css`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/__init__.py` & `libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/file.py` & `libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/file.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/film.py` & `libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/lib.py` & `libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/tinykin/flow/users.py` & `libreflow_flows-2.3.1/src/libreflow/flows/tinykin/flow/users.py`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/file_templates/template.blend` & `libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png` & `libreflow_flows-2.3.1/src/libreflow/flows/tinykin/resources/icons/flow/publish-ok.png`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/src/libreflow.flows.egg-info/PKG-INFO` & `libreflow_flows-2.3.1/src/libreflow.flows.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.flows
-Version: 2.3.0
+Version: 2.3.1
 Summary: A set of flows specific to projects handled by Libreflow at Les Fées Spéciales.
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow.flows
 Author: Baptiste Delos, Flavio Perez
 Author-email: baptiste@les-fees-speciales.coop, flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -37,14 +37,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.3.1] - 2024-05-16
+
+### Added
+
+* New session option to redefine its home oid. This oid can be provided either using the command line argument `--home-oid` or through the environment using the variable `KABARET_HOME_OID`.
+
 ## [2.3.0] - 2024-04-26
 
 ### Added
 
 The session now uses the new Kabaret's layout manager which is enabled by default with the session autosave feature.
 
 ## [2.2.0] - 2024-04-26
```

### Comparing `libreflow_flows-2.3.0/src/libreflow.flows.egg-info/SOURCES.txt` & `libreflow_flows-2.3.1/src/libreflow.flows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_flows-2.3.0/versioneer.py` & `libreflow_flows-2.3.1/versioneer.py`

 * *Files identical despite different names*

