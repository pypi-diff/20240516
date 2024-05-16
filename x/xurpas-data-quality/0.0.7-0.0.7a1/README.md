# Comparing `tmp/xurpas_data_quality-0.0.7.tar.gz` & `tmp/xurpas_data_quality-0.0.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xurpas_data_quality-0.0.7.tar", last modified: Wed May 15 01:42:06 2024, max compression
+gzip compressed data, was "xurpas_data_quality-0.0.7a1.tar", last modified: Thu May 16 07:00:02 2024, max compression
```

## Comparing `xurpas_data_quality-0.0.7.tar` & `xurpas_data_quality-0.0.7a1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.868093 xurpas_data_quality-0.0.7/
--rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2067 2024-05-15 01:42:06.865712 xurpas_data_quality-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2024-05-15 01:40:55.000000 xurpas_data_quality-0.0.7/README.md
--rw-rw-rw-   0        0        0      841 2024-05-15 01:11:13.000000 xurpas_data_quality-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 01:42:06.868145 xurpas_data_quality-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1147 2024-05-15 01:11:13.000000 xurpas_data_quality-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.770929 xurpas_data_quality-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.781263 xurpas_data_quality-0.0.7/src/xurpas_data_quality/
--rw-rw-rw-   0        0        0       59 2024-05-15 01:41:15.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.807759 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/
--rw-rw-rw-   0        0        0        0 2024-05-15 01:11:13.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.809914 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/alerts/
--rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/alerts/__init__.py
--rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/alerts/alerts.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.811100 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/algorithms/
--rw-rw-rw-   0        0        0       54 2024-05-15 01:11:13.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/algorithms/__init__.py
--rw-rw-rw-   0        0        0      495 2024-05-03 03:47:01.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/algorithms/algorithms.py
--rw-rw-rw-   0        0        0     1409 2024-05-15 01:21:11.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/dataframe.py
--rw-rw-rw-   0        0        0     6756 2024-05-15 01:11:13.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/describe.py
--rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/descriptions.py
--rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/pandas_dataframe.py
--rw-rw-rw-   0        0        0     2380 2024-05-15 01:30:43.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/data_report.py
--rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.815107 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/
--rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/__init__.py
--rw-rw-rw-   0        0        0      221 2024-05-15 01:11:13.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/render.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.819114 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/render_types/
--rw-rw-rw-   0        0        0        0 2024-05-15 01:11:13.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/render_types/render_numerical.py
--rw-rw-rw-   0        0        0      474 2024-05-15 01:11:13.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/render_variable.py
--rw-rw-rw-   0        0        0     4417 2024-05-14 05:05:46.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/renderer.py
--rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/template_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.833077 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.836339 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/assets/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/assets/__init__.py
--rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/assets/script.js
--rw-rw-rw-   0        0        0      600 2024-05-06 05:56:54.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/assets/style.css
--rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/base.html
--rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/collapse.html
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.854649 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/containers/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/containers/__init__.py
--rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/containers/box.html
--rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/containers/column.html
--rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/containers/default.html
--rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/containers/sections.html
--rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/containers/tabs.html
--rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/containers/test.html
--rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/dropdown.html
--rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/navigation.html
--rw-rw-rw-   0        0        0      279 2024-05-02 01:11:31.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/plot.html
--rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/script.html
--rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/style.html
--rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/table.html
--rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/toggle.html
--rw-rw-rw-   0        0        0      454 2024-05-06 05:58:21.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/variable.html
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.859760 xurpas_data_quality-0.0.7/src/xurpas_data_quality/report/
--rw-rw-rw-   0        0        0       30 2024-04-30 02:52:09.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/report/__init__.py
--rw-rw-rw-   0        0        0     7914 2024-05-14 07:29:58.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/report/report.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.863687 xurpas_data_quality-0.0.7/src/xurpas_data_quality/visuals/
--rw-rw-rw-   0        0        0      141 2024-05-06 02:32:12.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/visuals/__init__.py
--rw-rw-rw-   0        0        0     2279 2024-05-15 01:11:13.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality/visuals/plots.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:42:06.865712 xurpas_data_quality-0.0.7/src/xurpas_data_quality.egg-info/
--rw-rw-rw-   0        0        0     2067 2024-05-15 01:42:06.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2472 2024-05-15 01:42:06.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 01:42:06.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-15 01:42:06.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-15 01:42:06.000000 xurpas_data_quality-0.0.7/src/xurpas_data_quality.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.214032 xurpas_data_quality-0.0.7a1/
+-rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-0.0.7a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2081 2024-05-16 07:00:02.213034 xurpas_data_quality-0.0.7a1/PKG-INFO
+-rw-rw-rw-   0        0        0     1493 2024-05-15 01:55:13.000000 xurpas_data_quality-0.0.7a1/README.md
+-rw-rw-rw-   0        0        0      841 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.7a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:00:02.214032 xurpas_data_quality-0.0.7a1/setup.cfg
+-rw-rw-rw-   0        0        0     1147 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.7a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.139743 xurpas_data_quality-0.0.7a1/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.151465 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/
+-rw-rw-rw-   0        0        0       61 2024-05-16 06:51:44.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.165258 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/
+-rw-rw-rw-   0        0        0        0 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.167384 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/alerts/
+-rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/alerts/__init__.py
+-rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/alerts/alerts.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.169386 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/algorithms/
+-rw-rw-rw-   0        0        0       54 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/algorithms/__init__.py
+-rw-rw-rw-   0        0        0      598 2024-05-16 06:58:18.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/algorithms/algorithms.py
+-rw-rw-rw-   0        0        0     1282 2024-05-15 01:55:13.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/dataframe.py
+-rw-rw-rw-   0        0        0     6756 2024-05-16 06:35:50.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/describe.py
+-rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/descriptions.py
+-rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/pandas_dataframe.py
+-rw-rw-rw-   0        0        0     2380 2024-05-15 01:55:13.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data_report.py
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.174291 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/
+-rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/__init__.py
+-rw-rw-rw-   0        0        0      221 2024-05-15 01:55:13.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/render.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.175866 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/render_types/
+-rw-rw-rw-   0        0        0        0 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/render_types/render_numerical.py
+-rw-rw-rw-   0        0        0      474 2024-05-15 01:55:13.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/render_variable.py
+-rw-rw-rw-   0        0        0     4417 2024-05-14 05:05:46.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/renderer.py
+-rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/template_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.187110 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.190887 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/assets/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/assets/__init__.py
+-rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/assets/script.js
+-rw-rw-rw-   0        0        0      600 2024-05-06 05:56:54.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/assets/style.css
+-rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/base.html
+-rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/collapse.html
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.202264 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/containers/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/containers/__init__.py
+-rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/containers/box.html
+-rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/containers/column.html
+-rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/containers/default.html
+-rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/containers/sections.html
+-rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/containers/tabs.html
+-rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/containers/test.html
+-rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/dropdown.html
+-rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/navigation.html
+-rw-rw-rw-   0        0        0      279 2024-05-02 01:11:31.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/plot.html
+-rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/script.html
+-rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/style.html
+-rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/table.html
+-rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/toggle.html
+-rw-rw-rw-   0        0        0      454 2024-05-06 05:58:21.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/variable.html
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.208021 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/report/
+-rw-rw-rw-   0        0        0       30 2024-04-30 02:52:09.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/report/__init__.py
+-rw-rw-rw-   0        0        0     7914 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/report/report.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.211033 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/visuals/
+-rw-rw-rw-   0        0        0      141 2024-05-06 02:32:12.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/visuals/__init__.py
+-rw-rw-rw-   0        0        0     2279 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/visuals/plots.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:00:02.212032 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality.egg-info/
+-rw-rw-rw-   0        0        0     2081 2024-05-16 07:00:02.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2472 2024-05-16 07:00:02.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:00:02.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-16 07:00:02.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-16 07:00:02.000000 xurpas_data_quality-0.0.7a1/src/xurpas_data_quality.egg-info/top_level.txt
```

### Comparing `xurpas_data_quality-0.0.7/PKG-INFO` & `xurpas_data_quality-0.0.7a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 0.0.7
+Version: 0.0.7a1
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -25,19 +25,19 @@
 - Import the DataReport class
 - Save the report to html File
 
 ## DataReport
 Creates and saves to file the data report.
 
 **Args**
->**file**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;The path of the file you want to analyze. If empty, df parameter must exist. 
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Only supports .csv, .xlsx, .parquet, and .orc file formats
->**df**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Pandas DataFrame object of data to be analyzed, If using df, file must be empty.
->**report_name**: &emsp;Name of the report. Defaults to 'Data Report'
->**file_path**:&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved
+>**file**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;The path of the file you want to analyze. If empty, df parameter must exist.  
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Only supports .csv, .xlsx, .parquet, and .orc file formats.  
+>**df**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Pandas DataFrame object of data to be analyzed, If using df, file must be empty.  
+>**report_name**: &emsp;Name of the report. Defaults to 'Data Report'.  
+>**file_path**:&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved.  
 
 **Returns**
 >HTML File of data quality Report
 
 #### Sample Usage using pandas DataFrame
 ```python
 import pandas as pd
```

### Comparing `xurpas_data_quality-0.0.7/README.md` & `xurpas_data_quality-0.0.7a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 - Import the DataReport class
 - Save the report to html File
 
 ## DataReport
 Creates and saves to file the data report.
 
 **Args**
->**file**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;The path of the file you want to analyze. If empty, df parameter must exist. 
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Only supports .csv, .xlsx, .parquet, and .orc file formats
->**df**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Pandas DataFrame object of data to be analyzed, If using df, file must be empty.
->**report_name**: &emsp;Name of the report. Defaults to 'Data Report'
->**file_path**:&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved
+>**file**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;The path of the file you want to analyze. If empty, df parameter must exist.  
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Only supports .csv, .xlsx, .parquet, and .orc file formats.  
+>**df**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Pandas DataFrame object of data to be analyzed, If using df, file must be empty.  
+>**report_name**: &emsp;Name of the report. Defaults to 'Data Report'.  
+>**file_path**:&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved.  
 
 **Returns**
 >HTML File of data quality Report
 
 #### Sample Usage using pandas DataFrame
 ```python
 import pandas as pd
```

### Comparing `xurpas_data_quality-0.0.7/pyproject.toml` & `xurpas_data_quality-0.0.7a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/setup.py` & `xurpas_data_quality-0.0.7a1/setup.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/alerts/alerts.py` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/dataframe.py` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/dataframe.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,12 +43,9 @@
     
     # If the loading method exists, call it, else raise an error
     if load_method:
         return load_method(file_path)
     else:
         raise ValueError(f'Unsupported file format: {file_extension}')
 
-def check_file_path(file_path:str):
-    def has_extension(file_path):
-        return os.path.splitext(file_path)[1] != ''
+
     
-
```

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/data/describe.py` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data/describe.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/data_report.py` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/data_report.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/renderer.py` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/renderer.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/template_loader.py` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/template_loader.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/assets/script.js` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/assets/script.js`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/assets/style.css` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/assets/style.css`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/render/templates/containers/tabs.html` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/render/templates/containers/tabs.html`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/report/report.py` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/report/report.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality/visuals/plots.py` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality/visuals/plots.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality.egg-info/PKG-INFO` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 0.0.7
+Version: 0.0.7a1
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -25,19 +25,19 @@
 - Import the DataReport class
 - Save the report to html File
 
 ## DataReport
 Creates and saves to file the data report.
 
 **Args**
->**file**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;The path of the file you want to analyze. If empty, df parameter must exist. 
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Only supports .csv, .xlsx, .parquet, and .orc file formats
->**df**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Pandas DataFrame object of data to be analyzed, If using df, file must be empty.
->**report_name**: &emsp;Name of the report. Defaults to 'Data Report'
->**file_path**:&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved
+>**file**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;The path of the file you want to analyze. If empty, df parameter must exist.  
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Only supports .csv, .xlsx, .parquet, and .orc file formats.  
+>**df**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Pandas DataFrame object of data to be analyzed, If using df, file must be empty.  
+>**report_name**: &emsp;Name of the report. Defaults to 'Data Report'.  
+>**file_path**:&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved.  
 
 **Returns**
 >HTML File of data quality Report
 
 #### Sample Usage using pandas DataFrame
 ```python
 import pandas as pd
```

### Comparing `xurpas_data_quality-0.0.7/src/xurpas_data_quality.egg-info/SOURCES.txt` & `xurpas_data_quality-0.0.7a1/src/xurpas_data_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

