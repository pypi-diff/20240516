# Comparing `tmp/amiya-0.0.1.tar.gz` & `tmp/amiya-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amiya-0.0.1.tar", last modified: Wed May  1 06:24:04 2024, max compression
+gzip compressed data, was "amiya-0.0.3.tar", last modified: Wed May 15 23:15:05 2024, max compression
```

## Comparing `amiya-0.0.1.tar` & `amiya-0.0.3.tar`

### file list

```diff
@@ -1,98 +1,118 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.483245 amiya-0.0.1/
--rw-rw-rw-   0        0        0     1086 2024-04-03 01:29:58.000000 amiya-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      160 2024-05-01 04:29:03.000000 amiya-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2592 2024-05-01 06:24:04.483245 amiya-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1775 2024-05-01 06:23:26.000000 amiya-0.0.1/README.md
--rw-rw-rw-   0        0        0       95 2024-05-01 05:31:02.000000 amiya-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      120 2024-05-01 03:36:05.000000 amiya-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 06:24:04.483245 amiya-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2379 2024-05-01 06:22:01.000000 amiya-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.434714 amiya-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.442212 amiya-0.0.1/src/amiya/
--rw-rw-rw-   0        0        0     1122 2024-05-01 05:27:34.000000 amiya-0.0.1/src/amiya/__init__.py
--rw-rw-rw-   0        0        0     1948 2024-05-01 05:27:10.000000 amiya-0.0.1/src/amiya/amiya.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.454763 amiya-0.0.1/src/amiya/apps_manager/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:21:03.000000 amiya-0.0.1/src/amiya/apps_manager/__init__.py
--rw-rw-rw-   0        0        0     7736 2024-04-26 19:28:44.000000 amiya-0.0.1/src/amiya/apps_manager/app.py
--rw-rw-rw-   0        0        0    21981 2024-05-01 05:09:39.000000 amiya-0.0.1/src/amiya/apps_manager/apps_manager.py
--rw-rw-rw-   0        0        0     1805 2024-04-25 01:14:39.000000 amiya-0.0.1/src/amiya/apps_manager/apps_viewer.py
--rw-rw-rw-   0        0        0     3166 2024-05-01 03:00:03.000000 amiya-0.0.1/src/amiya/apps_manager/safety_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.456182 amiya-0.0.1/src/amiya/apps_manager/sync_controller/
--rw-rw-rw-   0        0        0        0 2024-04-22 19:14:02.000000 amiya-0.0.1/src/amiya/apps_manager/sync_controller/__init__.py
--rw-rw-rw-   0        0        0     2863 2024-04-26 02:54:50.000000 amiya-0.0.1/src/amiya/apps_manager/sync_controller/sync_controller.py
--rw-rw-rw-   0        0        0      539 2024-05-01 03:42:43.000000 amiya-0.0.1/src/amiya/apps_manager/sync_controller/sys_uuid_controller.py
--rw-rw-rw-   0        0        0       64 2024-04-07 04:55:43.000000 amiya-0.0.1/src/amiya/apps_manager/test.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.458188 amiya-0.0.1/src/amiya/automation_handler/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:45.000000 amiya-0.0.1/src/amiya/automation_handler/__init__.py
--rw-rw-rw-   0        0        0      723 2024-04-25 02:34:30.000000 amiya-0.0.1/src/amiya/automation_handler/automation_config_handler.py
--rw-rw-rw-   0        0        0     9319 2024-05-01 03:11:13.000000 amiya-0.0.1/src/amiya/automation_handler/automation_controller.py
--rw-rw-rw-   0        0        0     7161 2024-04-26 19:09:19.000000 amiya-0.0.1/src/amiya/automation_handler/automation_recorder.py
--rw-rw-rw-   0        0        0      977 2024-04-25 02:20:57.000000 amiya-0.0.1/src/amiya/automation_handler/automation_viewer.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.460189 amiya-0.0.1/src/amiya/automation_handler/units/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:54.000000 amiya-0.0.1/src/amiya/automation_handler/units/__init__.py
--rw-rw-rw-   0        0        0     4276 2024-04-27 22:23:01.000000 amiya-0.0.1/src/amiya/automation_handler/units/action.py
--rw-rw-rw-   0        0        0     1595 2024-04-25 03:15:44.000000 amiya-0.0.1/src/amiya/automation_handler/units/plate.py
--rw-rw-rw-   0        0        0     6285 2024-04-27 22:22:10.000000 amiya-0.0.1/src/amiya/automation_handler/units/sequence.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.461189 amiya-0.0.1/src/amiya/bin/
--rwxrwxrwx   0        0        0    42388 2024-04-26 03:59:33.000000 amiya-0.0.1/src/amiya/bin/focus_pid.exe
--rwxrwxrwx   0        0        0    42243 2024-04-26 03:59:33.000000 amiya-0.0.1/src/amiya/bin/get_active_pid.exe
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.462190 amiya-0.0.1/src/amiya/bin/scripts/
--rw-rw-rw-   0        0        0      788 2024-04-05 01:04:57.000000 amiya-0.0.1/src/amiya/bin/scripts/focus_pid.c
--rw-rw-rw-   0        0        0      469 2024-04-13 02:51:25.000000 amiya-0.0.1/src/amiya/bin/scripts/get_active_pid.c
--rw-rw-rw-   0        0        0     1841 2024-04-26 04:14:54.000000 amiya-0.0.1/src/amiya/bin/scripts/get_window_size.c
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.463195 amiya-0.0.1/src/amiya/entrypoints/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:03.000000 amiya-0.0.1/src/amiya/entrypoints/__init__.py
--rw-rw-rw-   0        0        0     8460 2024-05-01 05:00:06.000000 amiya-0.0.1/src/amiya/entrypoints/entrypoint_handler.py
--rw-rw-rw-   0        0        0     8974 2024-05-01 05:08:34.000000 amiya-0.0.1/src/amiya/entrypoints/entrypoints.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.464712 amiya-0.0.1/src/amiya/exceptions/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:17.000000 amiya-0.0.1/src/amiya/exceptions/__init__.py
--rw-rw-rw-   0        0        0     3819 2024-05-01 04:45:51.000000 amiya-0.0.1/src/amiya/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.466711 amiya-0.0.1/src/amiya/module_utilities/
--rw-rw-rw-   0        0        0        0 2024-04-18 07:52:26.000000 amiya-0.0.1/src/amiya/module_utilities/__init__.py
--rw-rw-rw-   0        0        0     2709 2024-05-01 05:07:37.000000 amiya-0.0.1/src/amiya/module_utilities/power_controller.py
--rw-rw-rw-   0        0        0     1062 2024-05-01 05:07:47.000000 amiya-0.0.1/src/amiya/module_utilities/search_controller.py
--rw-rw-rw-   0        0        0     3032 2024-05-01 03:32:42.000000 amiya-0.0.1/src/amiya/module_utilities/volume_controller.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.468211 amiya-0.0.1/src/amiya/pixel_calculator/
--rw-rw-rw-   0        0        0        0 2024-04-19 04:01:16.000000 amiya-0.0.1/src/amiya/pixel_calculator/__init__.py
--rw-rw-rw-   0        0        0     1792 2024-04-26 18:57:19.000000 amiya-0.0.1/src/amiya/pixel_calculator/pixel_calculator.py
--rw-rw-rw-   0        0        0     2505 2024-04-26 18:50:20.000000 amiya-0.0.1/src/amiya/pixel_calculator/resolution_detector.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.471212 amiya-0.0.1/src/amiya/resources/
--rw-rw-rw-   0        0        0    94080 2024-04-13 19:09:50.000000 amiya-0.0.1/src/amiya/resources/amiya-cli-2.png
--rw-rw-rw-   0        0        0   104680 2024-04-13 19:09:37.000000 amiya-0.0.1/src/amiya/resources/amiya-cli-3.png
--rw-rw-rw-   0        0        0   254392 2024-05-01 05:56:34.000000 amiya-0.0.1/src/amiya/resources/amiya-cli-4.png
--rw-rw-rw-   0        0        0    46585 2024-04-13 19:10:01.000000 amiya-0.0.1/src/amiya/resources/amiya-cli.png
--rw-rw-rw-   0        0        0   166735 2024-04-05 02:00:17.000000 amiya-0.0.1/src/amiya/resources/amiya.png
--rw-rw-rw-   0        0        0   197822 2024-04-05 17:56:21.000000 amiya-0.0.1/src/amiya/resources/amiya_with_border.png
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.472214 amiya-0.0.1/src/amiya/resources/code_snippets/
--rw-rw-rw-   0        0        0    60828 2024-04-13 19:08:35.000000 amiya-0.0.1/src/amiya/resources/code_snippets/add-app.png
--rw-rw-rw-   0        0        0    78155 2024-04-13 19:08:59.000000 amiya-0.0.1/src/amiya/resources/code_snippets/add-tag.png
--rw-rw-rw-   0        0        0    25735 2024-04-13 19:09:12.000000 amiya-0.0.1/src/amiya/resources/code_snippets/start.png
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.474552 amiya-0.0.1/src/amiya/scheduler/
--rw-rw-rw-   0        0        0        0 2024-04-23 03:48:30.000000 amiya-0.0.1/src/amiya/scheduler/__init__.py
--rw-rw-rw-   0        0        0     4458 2024-04-23 03:07:35.000000 amiya-0.0.1/src/amiya/scheduler/scheduler.py
--rw-rw-rw-   0        0        0      934 2024-04-22 21:49:58.000000 amiya-0.0.1/src/amiya/scheduler/scheduler_config_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.476735 amiya-0.0.1/src/amiya/utils/
--rw-rw-rw-   0        0        0        0 2024-04-10 04:03:44.000000 amiya-0.0.1/src/amiya/utils/__init__.py
--rw-rw-rw-   0        0        0     1334 2024-05-01 05:05:46.000000 amiya-0.0.1/src/amiya/utils/constants.py
--rw-rw-rw-   0        0        0     7484 2024-05-01 05:03:20.000000 amiya-0.0.1/src/amiya/utils/helper.py
--rw-rw-rw-   0        0        0     1039 2024-04-24 20:18:29.000000 amiya-0.0.1/src/amiya/utils/json_handler.py
--rw-rw-rw-   0        0        0     1415 2024-04-10 04:03:43.000000 amiya-0.0.1/src/amiya/utils/pynput_mapping.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.482237 amiya-0.0.1/src/amiya.egg-info/
--rw-rw-rw-   0        0        0     2592 2024-05-01 06:24:04.000000 amiya-0.0.1/src/amiya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2577 2024-05-01 06:24:04.000000 amiya-0.0.1/src/amiya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 06:24:04.000000 amiya-0.0.1/src/amiya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-01 06:24:04.000000 amiya-0.0.1/src/amiya.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-05-01 06:24:04.000000 amiya-0.0.1/src/amiya.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-01 06:24:04.000000 amiya-0.0.1/src/amiya.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 06:24:04.481737 amiya-0.0.1/test/
--rw-rw-rw-   0        0        0     6164 2024-05-01 04:27:56.000000 amiya-0.0.1/test/test1.py
--rw-rw-rw-   0        0        0      323 2024-04-26 03:55:02.000000 amiya-0.0.1/test/test10.py
--rw-rw-rw-   0        0        0     1496 2024-04-26 18:47:21.000000 amiya-0.0.1/test/test11.py
--rw-rw-rw-   0        0        0      308 2024-04-22 04:22:36.000000 amiya-0.0.1/test/test2.py
--rw-rw-rw-   0        0        0      926 2024-04-23 04:57:30.000000 amiya-0.0.1/test/test3.py
--rw-rw-rw-   0        0        0     3404 2024-04-13 22:28:40.000000 amiya-0.0.1/test/test4.py
--rw-rw-rw-   0        0        0      565 2024-04-14 20:12:50.000000 amiya-0.0.1/test/test5.py
--rw-rw-rw-   0        0        0     2589 2024-04-23 00:30:52.000000 amiya-0.0.1/test/test6.py
--rw-rw-rw-   0        0        0      757 2024-04-24 02:58:50.000000 amiya-0.0.1/test/test7.py
--rw-rw-rw-   0        0        0     3140 2024-04-26 04:28:13.000000 amiya-0.0.1/test/test8.py
--rw-rw-rw-   0        0        0      265 2024-04-26 03:32:33.000000 amiya-0.0.1/test/test9.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.732537 amiya-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2024-04-03 01:29:58.000000 amiya-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      213 2024-05-15 23:14:11.000000 amiya-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2678 2024-05-15 23:15:05.732037 amiya-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1839 2024-05-15 22:41:01.000000 amiya-0.0.3/README.md
+-rw-rw-rw-   0        0        0       95 2024-05-01 05:31:02.000000 amiya-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      128 2024-05-15 22:58:42.000000 amiya-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 23:15:05.733033 amiya-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2391 2024-05-15 23:08:36.000000 amiya-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.680917 amiya-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.692933 amiya-0.0.3/src/amiya/
+-rw-rw-rw-   0        0        0     1122 2024-05-01 05:27:34.000000 amiya-0.0.3/src/amiya/__init__.py
+-rw-rw-rw-   0        0        0     1880 2024-05-15 22:01:51.000000 amiya-0.0.3/src/amiya/amiya.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.685918 amiya-0.0.3/src/amiya/apps/
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.697438 amiya-0.0.3/src/amiya/apps/afk-journey/
+-rw-rw-rw-   0        0        0      248 2024-05-15 21:59:19.000000 amiya-0.0.3/src/amiya/apps/afk-journey/app-config.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.681916 amiya-0.0.3/src/amiya/apps/afk-journey/automation/
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.698458 amiya-0.0.3/src/amiya/apps/afk-journey/automation/sequence/
+-rw-rw-rw-   0        0        0    59570 2024-05-15 01:49:58.000000 amiya-0.0.3/src/amiya/apps/afk-journey/automation/sequence/daily.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.698963 amiya-0.0.3/src/amiya/apps/chrome/
+-rw-rw-rw-   0        0        0      256 2024-05-15 21:59:19.000000 amiya-0.0.3/src/amiya/apps/chrome/app-config.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.699463 amiya-0.0.3/src/amiya/apps/genshin-impact/
+-rw-rw-rw-   0        0        0      265 2024-05-15 21:59:19.000000 amiya-0.0.3/src/amiya/apps/genshin-impact/app-config.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.699968 amiya-0.0.3/src/amiya/apps/honkai-star-rail/
+-rw-rw-rw-   0        0        0      251 2024-05-15 21:59:19.000000 amiya-0.0.3/src/amiya/apps/honkai-star-rail/app-config.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.700465 amiya-0.0.3/src/amiya/apps/ld-player/
+-rw-rw-rw-   0        0        0      240 2024-05-15 21:59:20.000000 amiya-0.0.3/src/amiya/apps/ld-player/app-config.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.683418 amiya-0.0.3/src/amiya/apps/ld-player/automation/
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.701464 amiya-0.0.3/src/amiya/apps/ld-player/automation/sequence/
+-rw-rw-rw-   0        0        0    56052 2024-05-14 23:43:35.000000 amiya-0.0.3/src/amiya/apps/ld-player/automation/sequence/arknights-base.json
+-rw-rw-rw-   0        0        0     3048 2024-05-04 02:32:47.000000 amiya-0.0.3/src/amiya/apps/ld-player/automation/sequence/arknights-start.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.701963 amiya-0.0.3/src/amiya/apps/league-of-legends/
+-rw-rw-rw-   0        0        0      274 2024-05-15 21:59:20.000000 amiya-0.0.3/src/amiya/apps/league-of-legends/app-config.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.702464 amiya-0.0.3/src/amiya/apps/persona-5-x/
+-rw-rw-rw-   0        0        0      243 2024-05-15 21:59:20.000000 amiya-0.0.3/src/amiya/apps/persona-5-x/app-config.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.685918 amiya-0.0.3/src/amiya/apps/persona-5-x/automation/
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.703464 amiya-0.0.3/src/amiya/apps/persona-5-x/automation/sequence/
+-rw-rw-rw-   0        0        0   110959 2024-04-26 03:13:43.000000 amiya-0.0.3/src/amiya/apps/persona-5-x/automation/sequence/daily.json
+-rw-rw-rw-   0        0        0    96070 2024-05-05 04:33:03.000000 amiya-0.0.3/src/amiya/apps/persona-5-x/automation/sequence/test.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.703966 amiya-0.0.3/src/amiya/apps/steam/
+-rw-rw-rw-   0        0        0      216 2024-05-15 21:59:20.000000 amiya-0.0.3/src/amiya/apps/steam/app-config.json
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.706465 amiya-0.0.3/src/amiya/apps_manager/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:21:03.000000 amiya-0.0.3/src/amiya/apps_manager/__init__.py
+-rw-rw-rw-   0        0        0     8624 2024-05-13 19:47:34.000000 amiya-0.0.3/src/amiya/apps_manager/app.py
+-rw-rw-rw-   0        0        0    23221 2024-05-13 19:45:19.000000 amiya-0.0.3/src/amiya/apps_manager/apps_manager.py
+-rw-rw-rw-   0        0        0     1938 2024-05-07 23:50:31.000000 amiya-0.0.3/src/amiya/apps_manager/apps_viewer.py
+-rw-rw-rw-   0        0        0     3359 2024-05-13 18:16:23.000000 amiya-0.0.3/src/amiya/apps_manager/safety_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.707470 amiya-0.0.3/src/amiya/apps_manager/sync_controller/
+-rw-rw-rw-   0        0        0        0 2024-04-22 19:14:02.000000 amiya-0.0.3/src/amiya/apps_manager/sync_controller/__init__.py
+-rw-rw-rw-   0        0        0     2863 2024-04-26 02:54:50.000000 amiya-0.0.3/src/amiya/apps_manager/sync_controller/sync_controller.py
+-rw-rw-rw-   0        0        0      539 2024-05-01 03:42:43.000000 amiya-0.0.3/src/amiya/apps_manager/sync_controller/sys_uuid_controller.py
+-rw-rw-rw-   0        0        0       64 2024-04-07 04:55:43.000000 amiya-0.0.3/src/amiya/apps_manager/test.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.710489 amiya-0.0.3/src/amiya/automation_handler/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:45.000000 amiya-0.0.3/src/amiya/automation_handler/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-04-25 02:34:30.000000 amiya-0.0.3/src/amiya/automation_handler/automation_config_handler.py
+-rw-rw-rw-   0        0        0     9304 2024-05-07 23:35:45.000000 amiya-0.0.3/src/amiya/automation_handler/automation_controller.py
+-rw-rw-rw-   0        0        0     7043 2024-05-15 22:11:47.000000 amiya-0.0.3/src/amiya/automation_handler/automation_recorder.py
+-rw-rw-rw-   0        0        0      977 2024-04-25 02:20:57.000000 amiya-0.0.3/src/amiya/automation_handler/automation_viewer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.712490 amiya-0.0.3/src/amiya/automation_handler/units/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:54.000000 amiya-0.0.3/src/amiya/automation_handler/units/__init__.py
+-rw-rw-rw-   0        0        0     4595 2024-05-05 22:30:53.000000 amiya-0.0.3/src/amiya/automation_handler/units/action.py
+-rw-rw-rw-   0        0        0     1595 2024-04-25 03:15:44.000000 amiya-0.0.3/src/amiya/automation_handler/units/plate.py
+-rw-rw-rw-   0        0        0     7763 2024-05-10 13:26:52.000000 amiya-0.0.3/src/amiya/automation_handler/units/sequence.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.713988 amiya-0.0.3/src/amiya/bin/
+-rwxrwxrwx   0        0        0    42694 2024-05-13 19:09:05.000000 amiya-0.0.3/src/amiya/bin/focus_pid.exe
+-rwxrwxrwx   0        0        0    42243 2024-05-13 19:09:04.000000 amiya-0.0.3/src/amiya/bin/get_active_pid.exe
+-rwxrwxrwx   0        0        0    42845 2024-05-13 19:09:04.000000 amiya-0.0.3/src/amiya/bin/get_window_size.exe
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.714988 amiya-0.0.3/src/amiya/bin/scripts/
+-rw-rw-rw-   0        0        0     1831 2024-05-13 19:09:02.000000 amiya-0.0.3/src/amiya/bin/scripts/focus_pid.c
+-rw-rw-rw-   0        0        0      469 2024-04-13 02:51:25.000000 amiya-0.0.3/src/amiya/bin/scripts/get_active_pid.c
+-rw-rw-rw-   0        0        0     1841 2024-04-26 04:14:54.000000 amiya-0.0.3/src/amiya/bin/scripts/get_window_size.c
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.716489 amiya-0.0.3/src/amiya/entrypoints/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:03.000000 amiya-0.0.3/src/amiya/entrypoints/__init__.py
+-rw-rw-rw-   0        0        0    12117 2024-05-15 22:36:22.000000 amiya-0.0.3/src/amiya/entrypoints/entrypoint_handler.py
+-rw-rw-rw-   0        0        0    13338 2024-05-15 22:22:51.000000 amiya-0.0.3/src/amiya/entrypoints/entrypoints.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.717492 amiya-0.0.3/src/amiya/exceptions/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:17.000000 amiya-0.0.3/src/amiya/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     3819 2024-05-01 04:45:51.000000 amiya-0.0.3/src/amiya/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.720513 amiya-0.0.3/src/amiya/module_utilities/
+-rw-rw-rw-   0        0        0      214 2024-05-12 19:29:56.000000 amiya-0.0.3/src/amiya/module_utilities/__init__.py
+-rw-rw-rw-   0        0        0     2579 2024-05-15 22:13:01.000000 amiya-0.0.3/src/amiya/module_utilities/continuous_click_controller.py
+-rw-rw-rw-   0        0        0     3168 2024-05-12 22:48:48.000000 amiya-0.0.3/src/amiya/module_utilities/cursor_controller.py
+-rw-rw-rw-   0        0        0     1245 2024-05-13 18:35:25.000000 amiya-0.0.3/src/amiya/module_utilities/dev_features.py
+-rw-rw-rw-   0        0        0     2709 2024-05-07 23:22:25.000000 amiya-0.0.3/src/amiya/module_utilities/power_controller.py
+-rw-rw-rw-   0        0        0     1062 2024-05-01 05:07:47.000000 amiya-0.0.3/src/amiya/module_utilities/search_controller.py
+-rw-rw-rw-   0        0        0     8832 2024-05-12 16:53:49.000000 amiya-0.0.3/src/amiya/module_utilities/volume_controller.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.722016 amiya-0.0.3/src/amiya/pixel_calculator/
+-rw-rw-rw-   0        0        0        0 2024-04-19 04:01:16.000000 amiya-0.0.3/src/amiya/pixel_calculator/__init__.py
+-rw-rw-rw-   0        0        0     1693 2024-05-15 02:40:55.000000 amiya-0.0.3/src/amiya/pixel_calculator/pixel_calculator.py
+-rw-rw-rw-   0        0        0     2830 2024-05-14 06:07:14.000000 amiya-0.0.3/src/amiya/pixel_calculator/resolution_detector.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.725515 amiya-0.0.3/src/amiya/resources/
+-rw-rw-rw-   0        0        0    94080 2024-04-13 19:09:50.000000 amiya-0.0.3/src/amiya/resources/amiya-cli-2.png
+-rw-rw-rw-   0        0        0   104680 2024-04-13 19:09:37.000000 amiya-0.0.3/src/amiya/resources/amiya-cli-3.png
+-rw-rw-rw-   0        0        0   254392 2024-05-01 05:56:34.000000 amiya-0.0.3/src/amiya/resources/amiya-cli-4.png
+-rw-rw-rw-   0        0        0    46585 2024-04-13 19:10:01.000000 amiya-0.0.3/src/amiya/resources/amiya-cli.png
+-rw-rw-rw-   0        0        0   166735 2024-04-05 02:00:17.000000 amiya-0.0.3/src/amiya/resources/amiya.png
+-rw-rw-rw-   0        0        0   197822 2024-04-05 17:56:21.000000 amiya-0.0.3/src/amiya/resources/amiya_with_border.png
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.727518 amiya-0.0.3/src/amiya/resources/code_snippets/
+-rw-rw-rw-   0        0        0    60828 2024-04-13 19:08:35.000000 amiya-0.0.3/src/amiya/resources/code_snippets/add-app.png
+-rw-rw-rw-   0        0        0    78155 2024-04-13 19:08:59.000000 amiya-0.0.3/src/amiya/resources/code_snippets/add-tag.png
+-rw-rw-rw-   0        0        0    25735 2024-04-13 19:09:12.000000 amiya-0.0.3/src/amiya/resources/code_snippets/start.png
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.728826 amiya-0.0.3/src/amiya/scheduler/
+-rw-rw-rw-   0        0        0        0 2024-04-23 03:48:30.000000 amiya-0.0.3/src/amiya/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     4458 2024-04-23 03:07:35.000000 amiya-0.0.3/src/amiya/scheduler/scheduler.py
+-rw-rw-rw-   0        0        0      934 2024-04-22 21:49:58.000000 amiya-0.0.3/src/amiya/scheduler/scheduler_config_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.731036 amiya-0.0.3/src/amiya/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-10 04:03:44.000000 amiya-0.0.3/src/amiya/utils/__init__.py
+-rw-rw-rw-   0        0        0     1652 2024-05-15 22:44:44.000000 amiya-0.0.3/src/amiya/utils/constants.py
+-rw-rw-rw-   0        0        0    10960 2024-05-13 19:29:29.000000 amiya-0.0.3/src/amiya/utils/helper.py
+-rw-rw-rw-   0        0        0     1039 2024-04-24 20:18:29.000000 amiya-0.0.3/src/amiya/utils/json_handler.py
+-rw-rw-rw-   0        0        0     1415 2024-04-10 04:03:43.000000 amiya-0.0.3/src/amiya/utils/pynput_mapping.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.731534 amiya-0.0.3/src/amiya.egg-info/
+-rw-rw-rw-   0        0        0     2678 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3253 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/top_level.txt
```

### Comparing `amiya-0.0.1/LICENSE` & `amiya-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/PKG-INFO` & `amiya-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: amiya
-Version: 0.0.1
+Version: 0.0.3
 Summary: A lightweight cross-platform automation tool for games and daily tasks!
 Home-page: http://github.com/rezeroe/amiya
 Author: Kevin L.
 Author-email: kevinliu@vt.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pywin32
 Requires-Dist: psutil
 Requires-Dist: pynput
 Requires-Dist: pyautogui
@@ -20,29 +20,32 @@
 Requires-Dist: setuptools
 Requires-Dist: elevate
 Requires-Dist: termcolor
 Requires-Dist: schedule
 Requires-Dist: screeninfo
 Requires-Dist: customtkinter
 Requires-Dist: pycaw
+Requires-Dist: Pillow
+
+# Amiya
+Amiya - a lightweight cross-platform automation tool that allows scheduled start and automation of any application from the CLI.
 
-# Amiya (in development)
-Amiya - a lightweight cross-platform automation tool that allows scheduled start and automation of any application from the CLI. 
 
 <div align="center">
     <p style="padding-bottom: 0">
         <img src="https://i.imgur.com/l6VZmHq.png" alt="Amiya Icon" width="85%" height="auto"/>
     </p>
     <!-- <span style="color: #093163">A lightweight cross-platform automation tool for daily tasks!</span> -->
 </div>
 
 
 ## Overview
-Amiya is a easy-to-use and versatile cross-platform application and game automation tool designed for efficiency and ease of use directly from the CLI. This package offers automation capabilities for any applications (including games), enabling users to start and control any application with simple CLI commands.
+_This project is currently in development (`Development Status :: 4 - Beta`)._
 
+Amiya is a easy-to-use and versatile cross-platform application and game automation tool designed for efficiency and ease of use directly from the CLI. This package offers automation capabilities for any applications (including games), enabling users to start and control any application with simple CLI commands.
 
 
 The primary features supported by the `amiya` package are:
 1. **Application Launcher**: Start and terminate any applications from the CLI
 2. **Automation Controller**: Automate any applications with recorded mouse & keyboard sequences
 3. **Scheduling**: Schedule the start/automation of any application to run at any time
 4. **Other Utilities** Other lightweight quality-of-life utilities for applications:
```

### Comparing `amiya-0.0.1/README.md` & `amiya-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# Amiya (in development)
-Amiya - a lightweight cross-platform automation tool that allows scheduled start and automation of any application from the CLI. 
+# Amiya
+Amiya - a lightweight cross-platform automation tool that allows scheduled start and automation of any application from the CLI.
+
 
 <div align="center">
     <p style="padding-bottom: 0">
         <img src="https://i.imgur.com/l6VZmHq.png" alt="Amiya Icon" width="85%" height="auto"/>
     </p>
     <!-- <span style="color: #093163">A lightweight cross-platform automation tool for daily tasks!</span> -->
 </div>
 
 
 ## Overview
-Amiya is a easy-to-use and versatile cross-platform application and game automation tool designed for efficiency and ease of use directly from the CLI. This package offers automation capabilities for any applications (including games), enabling users to start and control any application with simple CLI commands.
+_This project is currently in development (`Development Status :: 4 - Beta`)._
 
+Amiya is a easy-to-use and versatile cross-platform application and game automation tool designed for efficiency and ease of use directly from the CLI. This package offers automation capabilities for any applications (including games), enabling users to start and control any application with simple CLI commands.
 
 
 The primary features supported by the `amiya` package are:
 1. **Application Launcher**: Start and terminate any applications from the CLI
 2. **Automation Controller**: Automate any applications with recorded mouse & keyboard sequences
 3. **Scheduling**: Schedule the start/automation of any application to run at any time
 4. **Other Utilities** Other lightweight quality-of-life utilities for applications:
```

### Comparing `amiya-0.0.1/setup.py` & `amiya-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 # SOFTWARE.
 
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='amiya',
-    version='0.0.1',
+    version='0.0.3',
     author='Kevin L.',
     author_email='kevinliu@vt.edu',
     description='A lightweight cross-platform automation tool for games and daily tasks!',
     long_description=open('README.md', encoding='utf-8').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url='http://github.com/rezeroe/amiya',
     package_dir={'': 'src'},                                                            # Tell setuptools that all packages are under src
     packages=find_packages(where='src'),                                                # Find packages in src directory
     install_requires=open('requirements.txt', encoding='utf-8').read().splitlines(),    # List of dependencies
     python_requires='>=3.6, <4',
     entry_points={
         'console_scripts': [
-            'amiya=amiya.entrypoints.entrypoints:start_amiya',
+            'amiya=amiya.entrypoints.entrypoints:start_amiya_cli_as_admin',
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Development Status :: 3 - Alpha'
+        'Development Status :: 4 - Beta'
     ],  
     include_package_data=True,
 )
```

### Comparing `amiya-0.0.1/src/amiya/__init__.py` & `amiya-0.0.3/src/amiya/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/amiya.py` & `amiya-0.0.3/src/amiya/amiya.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,17 +30,15 @@
 # TO INSTALL THE AMIYA CLI MODULE LOCALLY, RUN
 #   
 #     $ pip install amiya
 # OR
 #     $ git clone https://github.com/ReZeroE/Amiya.git
 #     $ cd Amiya/
 #     $ pip install .
-#
-#
-# RUN THIS SCRIPT TO START THE AMIYA CLI WITHOUT INSTALLATION.
+
 
 import sys
 from amiya.utils.helper import verify_platform
 from amiya.entrypoints.entrypoints import start_amiya
 from amiya.exceptions.exceptions import AmiyaOSNotSupported
 
 if verify_platform():
```

### Comparing `amiya-0.0.1/src/amiya/apps_manager/__init__.py` & `amiya-0.0.3/src/amiya/apps_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/apps_manager/app.py` & `amiya-0.0.3/src/amiya/apps_manager/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import time
 import psutil
 import subprocess
 from pathlib import Path
 from amiya.utils.constants import APPS_DIRECTORY, FOCUS_PID_EXE
 from amiya.exceptions.exceptions import *
+from amiya.utils.helper import WindowUtils, aprint
 from amiya.automation_handler.automation_controller import AutomationController
 from amiya.apps_manager.sync_controller.sys_uuid_controller import SysUUIDController
 
 APP_AUTOMATION_DIRNAME          = "automation"
 APP_CONFIG_FILENAME             = "app-config.json"
 
 class App:
@@ -33,15 +34,17 @@
         # It is not always (and most likely not) up-to-date as the program continues to run. 
         # This variable is only updated when is_running() is called and therefore this variable 
         # should NEVER be used to identify the current activity/status of the application.
         #
         # This variable should ONLY be used to identify the initial status of the application
         # as its started since any callback to is_running() (while a new instance of the application
         # is created) will overwrite the previous process.
-        self.process    = None
+        #
+        # Use get_app_process() instead.
+        self.process: psutil.Process = None
     
         self.app_config_dirpath     = os.path.join(APPS_DIRECTORY, self.get_reformatted_app_name())
         self.app_config_filepath    = os.path.join(self.app_config_dirpath, APP_CONFIG_FILENAME)
         self.app_automation_dirpath = os.path.join(self.app_config_dirpath, APP_AUTOMATION_DIRNAME)
         
         self.new = new
         self.automation_controller = None
@@ -90,49 +93,68 @@
             self.bring_to_foreground()
             return True
         
         # If the application is not running, then start the application
         if self.verified == True:   
             subprocess.Popen([self.exe_path], shell=True)
             
-            if self.started_successfully():
+            if self.wait_to_start():
                 self.bring_to_foreground()
                 return True
             return False
         else:
             raise Amiya_AppInvalidPathException(path=self.exe_path)
 
-    def started_successfully(self) -> bool:
+    def wait_to_start(self) -> bool:
         TIMEOUT = 30
         starting_time = time.time()
         while time.time() - starting_time < TIMEOUT:
             if self.is_running():
                 return True
             time.sleep(1)
         return False
 
-    def is_running(self) -> bool:
+    def is_running(self, timeout: int = 0) -> bool:
+        if timeout == 0:
+            return self.get_app_process() != None
+        
+        # Timeout will ensure the application is still running after timeout seconds.
+        if self.get_app_process() != None:
+            time.sleep(timeout)
+            return self.get_app_process() != None
+        return False
+    
+    def get_app_process(self) -> psutil.Process:
         APP_EXE_NAME = os.path.basename(self.exe_path)
         for p in psutil.process_iter():
             if APP_EXE_NAME.replace(".exe", "") in p.name():
                 try:
-                    self.process = psutil.Process(p.pid)
-                    if self.process.is_running():
-                        return True
-                    return False
+                    app_process = psutil.Process(p.pid)
+                    if app_process.is_running():
+                        self.process = app_process
+                        return app_process
+                    
                 except Exception as ex:
-                    raise AmiyaBaseException("Failed to identify the app's process due to an unknown error.")
-        return False
+                    raise AmiyaBaseException(f"Failed to identify the app's process due to an unknown error ({ex}).")
+        return None
+    
     
     def bring_to_foreground(self):
         try:
-            if self.is_running():
-                subprocess.run([FOCUS_PID_EXE, str(self.process.pid)], shell=True)
-        except:
-            raise AmiyaBaseException(f"The app '{self.name}' is currently not running, therefore can't be brought to foreground.")
+            TIMEOUT = 10
+            start_time = time.time()
+            while time.time() - start_time < TIMEOUT:
+                if self.is_running():
+                    success = WindowUtils.bring_to_foreground(self.process.pid)
+                    if success:
+                        return
+        except Exception as ex:
+            raise AmiyaBaseException(f"The app '{self.name}' is currently not running, therefore can't be brought to foreground ({ex}).")
+
+        raise AmiyaBaseException(f"The app '{self.name}' cannot be brought to foreground due to an unknown error.") 
 
     # ==========================================
     # ============| APP UTILITIES | ============
     # ==========================================
 
     def to_json(self):
         return {
```

### Comparing `amiya-0.0.1/src/amiya/apps_manager/apps_manager.py` & `amiya-0.0.3/src/amiya/apps_manager/apps_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,33 @@
         app.save_app_config()
     
     def __parse_tag(self, tag: str):
         return tag.strip()
     
         
     # HELPER FUNCTIONS ======================
+    def verbose_app_config(self, tag: str = None, show_all: bool = False):
+        app = None
+        if tag == None:                             # If no application tag is inputted by user
+            self.print_apps()
+            user_input = input(atext(f"Which app would you like to DELETE? (0-{len(self.apps)-1}) "))
+            app = self.apps[int(user_input)]
+        else:                                       # If user inputted an application tag tag
+            tag = self.__parse_tag(tag)
+            app = self.get_app_by_tag(tag)
+            
+        text = f"Application Configuration:"
+        text += f"\nApp Name: {app.name}"
+        text += f"\nApp ID: {app.id}"  
+        text += f"\nApp Tags: {app.tags}"
+        text += f"\nApp Config Directory: {app.app_config_dirpath}" 
+        text += f"\nApp Configuration System UUID: {app.sys_uuid}"  
+        aprint(text)
+        
+    
     def __initial_setup(self):
         if not os.path.isdir(APPS_DIRECTORY):
             os.mkdir(APPS_DIRECTORY)
             
     def __get_next_app_id(self) -> int:
         return max(self.apps.keys()) + 1
 
@@ -332,15 +351,15 @@
         )
         self.__print_sequence(new_sequence_recorded)
         
 
     # =================================================
     # ================| RUN SEQUENCES | ===============
     # =================================================
-    def run_sequence(self, tag: str = None, seq_name: str = None, add_global_delay: bool = False, terminate_on_finish: bool = False):
+    def run_sequence(self, tag: str = None, seq_name: str = None, global_delay: int = 0, terminate_on_finish: bool = False, no_confirmation: bool = False):
         self.__verify_non_empty_apps_dir()
         
         if tag != None:
             tag = self.__parse_tag(tag)
             app = self.get_app_by_tag(tag)
         else:
             self.print_apps()
@@ -353,45 +372,47 @@
         if seq_name == None:
             self.__print_sequences(sequence_list)                             # Verbose all sequences in the CLI and wait for user selection
             seq_name = input(atext(f"Which sequence would you like to run (i.e. start-game)? "))
         sequence: AutomationSequence = self.__safe_get_sequence(app, seq_name)
         
         # ============== GET GLOBAL DELAY ==============
         global_delay = 0
-        if add_global_delay:
+        if global_delay == -1:                                                # If global_delay == -1, then the argument -g is used but no time is specified (in entrypoints.py)
             aprint(f"Add global delay to all actions (seconds) [leave empty to default to 0]: ", end="")
             user_input = input().lower().strip()
             if user_input:
-                global_delay = self.__parse_int(user_input)                     # If user inputted global delay
+                global_delay = self.__parse_int(user_input)                   # If user inputted global delay
         sequence.set_global_delay(global_delay)
         
         # ============== RUN CONFIRMATION ==============
-        terminate_text = " Terminate on finish." if terminate_on_finish else ""
-        aprint(f"The sequence '{sequence.sequence_name}' will run for {sequence.get_runtime()} seconds.{terminate_text} Continue? [y/n] ", log_type=LogType.WARNING, end="")
-        if input().lower() != "y": return                                       # Verbose runtime and wait for user confirmation to run
+        if not no_confirmation:
+            terminate_text = " Terminate on finish." if terminate_on_finish else ""
+            aprint(f"The sequence '{sequence.sequence_name}' will run for {sequence.get_runtime()} seconds.{terminate_text} Continue? [y/n] ", log_type=LogType.WARNING, end="")
+            if input().lower() != "y": return                                  # Verbose runtime and wait for user confirmation to run
         
         # =============== START RUNNING ===============
         aprint(f"[Automation {sequence.sequence_name}] Running...")
-        self.__safe_start_app(app); time.sleep(5)                               # Starts the application for the sequence
-        safety_monitor = SafetyMonitor(app.process)                             # Creates a safety monitor object for sequence execution safety (must be created after the app is started)
-        self.__safe_execute_sequence(sequence, safety_monitor)                   # Runs the sequence (with the safety monitor)
+        self.__safe_start_app(app);                                            # Starts the application for the sequence
+        app_process = app.get_app_process()                                    # Get application's process
+        safety_monitor = SafetyMonitor(app_process)                            # Creates a safety monitor object for sequence execution safety (must be created after the app is started)
+        self.__safe_execute_sequence(sequence, safety_monitor)                 # Runs the sequence (with the safety monitor)
 
         print("")
         aprint(f"[Automation {sequence.sequence_name}] Run Completed!", log_type=LogType.SUCCESS)
         
         if terminate_on_finish:
             self.__safe_terminate_current_app()
         
         
     def __safe_execute_sequence(self, sequence: AutomationSequence, safety_monitor: SafetyMonitor):
         try:
             sequence.execute(safety_monitor)
         except Amiya_AppNotFocusedException:
             aprint("[Amiya Safety-Monitor] The application is unfocused during an automation sequence. Automation stopped.", log_type=LogType.ERROR)
-            exit(1)
+            raise AmiyaExit()
      
     def __safe_get_sequence(self, app: App, sequence_name: str) -> AutomationSequence:
         sequence = app.automation_controller.get_sequence(sequence_name)
         if sequence == None:
             aprint(f"No sequence with name '{sequence_name}' exists. Exiting.", log_type=LogType.ERROR); raise AmiyaExit()
         return sequence
```

### Comparing `amiya-0.0.1/src/amiya/apps_manager/apps_viewer.py` & `amiya-0.0.3/src/amiya/apps_manager/apps_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 
 from termcolor import colored
 from tabulate import tabulate
 from amiya.apps_manager.app import App
 from amiya.utils.constants import APPS_DIRECTORY
-from amiya.utils.helper import bool_to_str, Printer, shorten_display_path
+from amiya.utils.helper import bool_to_str, Printer, shorten_display_path, resize_terminal
 
 
 class AppsViewer:
     
     @staticmethod
     def tabulate_apps(apps_dict: dict[int, App], tablefmt) -> str:
         table = [[id, app.name, Printer.to_lightgrey(shorten_display_path(app.exe_path)), bool_to_str(app.verified), ", ".join(app.tags)] for id, app in apps_dict.items()]
         table = sorted(table, key=lambda x: x[0])
         headers = ["ID", "App Name", "Executable Path", "Path Verified", "Tags"]
         headers = [Printer.to_blue(title) for title in headers]
         tabulated_table =  tabulate(table, headers, tablefmt=tablefmt)
         # tabulated_table = '\n'.join('  ' + line for line in tabulated_table.split('\n'))
+        
+        table_len = len(tabulated_table.split('\n')[0])
+        resize_terminal(table_len, 5)
+        
         return tabulated_table
     
     @staticmethod
     def tabulate_apps_list(apps_list: list[App], tablefmt) -> str:
         table = [[app.name, app.exe_path, app.verified, ", ".join(app.tags)] for app in apps_list]
         table = sorted(table, key=lambda x: x[0])
         headers = ["App Name", "Executable Path", "Verified", "Tags"]
```

### Comparing `amiya-0.0.1/src/amiya/apps_manager/safety_monitor.py` & `amiya-0.0.3/src/amiya/apps_manager/safety_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,17 @@
         '''
         focused_pid = SafetyMonitor.get_focused_pid()
         
         # If PID == original APP's PID, return True
         if focused_pid == self.app_process.pid:
             return True
 
-
         # print(f"Focused {focused_pid}")
         # print(f"App: {self.app_process.pid}")
         # print(f"Cached: {self.cached_pids}")
-        
 
         if focused_pid not in self.cached_pids:
             self.__update_cached_pids()  # Update the cache if PID not found initially
             
             if focused_pid not in self.cached_pids:
                 aprint(f"Focused PID: [{focused_pid}], Original App PID: [{self.app_process.pid}], Cached PID: {self.cached_pids}", log_type=LogType.ERROR, new_line_no_prefix=False)
                 raise Amiya_AppNotFocusedException()
@@ -39,17 +37,25 @@
                 return True
         else:
             return True
         
 
     
     def __update_cached_pids(self):
-        children_pids = set(proc.pid for proc in self.app_process.children(recursive=True))                  # Get children PIDs
-        parents_pids = set(proc.pid for proc in self.app_process.parents() if proc.pid != os.getpid())       # Get parent PIDs
-        self.cached_pids = children_pids.union(parents_pids)
+        # If the inital process is still running
+        try:
+            children_pids = set(proc.pid for proc in self.app_process.children(recursive=True))                  # Get children PIDs
+            parents_pids = set(proc.pid for proc in self.app_process.parents() if proc.pid != os.getpid())       # Get parent PIDs
+            self.cached_pids = children_pids.union(parents_pids)
+        
+        # If the inital proecss is killed
+        except psutil.NoSuchProcess:
+            pass
+        
+        
     
     
     @staticmethod
     def get_focused_pid() -> int|None:
         result = subprocess.run([GET_FOCUSED_PID_EXE], capture_output=True, text=True)
     
         pid = None
```

### Comparing `amiya-0.0.1/src/amiya/apps_manager/sync_controller/sync_controller.py` & `amiya-0.0.3/src/amiya/apps_manager/sync_controller/sync_controller.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/apps_manager/sync_controller/sys_uuid_controller.py` & `amiya-0.0.3/src/amiya/apps_manager/sync_controller/sys_uuid_controller.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/automation_handler/__init__.py` & `amiya-0.0.3/src/amiya/automation_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/automation_handler/automation_config_handler.py` & `amiya-0.0.3/src/amiya/automation_handler/automation_config_handler.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/automation_handler/automation_controller.py` & `amiya-0.0.3/src/amiya/automation_handler/automation_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,18 +52,18 @@
         return None
      
     def sequence_exists(self, sequence_name):
         return self.get_sequence(sequence_name) != None
         
     def record_sequence(self, new_sequence_name, safety_monitor: SafetyMonitor) -> AutomationSequence:
         NEW_SEQUENCE_NAME = self.__reformat_sequence_name(new_sequence_name)
-        recording_sequence = AutomationSequence(NEW_SEQUENCE_NAME)                           # Create new empty actions sequence (later populated during recording)
+        recording_sequence = AutomationSequence(NEW_SEQUENCE_NAME)                        # Create new empty actions sequence (later populated during recording)
         recording_sequence.set_date_created_to_current()                                  # Set current time to creation time
 
-        action_recorder   = AutomationRecorder(recording_sequence, safety_monitor)           # Create the AutomationRecorder object by passing it the empty sequence object to populate and a safety monitor (to fetch app window size)
+        action_recorder   = AutomationRecorder(recording_sequence, safety_monitor)        # Create the AutomationRecorder object by passing it the empty sequence object to populate and a safety monitor (to fetch app window size)
         action_recorder.record(start_on_callback=True)                                    # Record mouse actions until "end-recording" is pressed
         
         aprint("Saving to configurations...")
         config_handler    = SequenceConfigHandler(self.__get_sequence_filepath(new_sequence_name))
         json_sequence     = recording_sequence.to_json()                                  # Convert the AutomationSequence object into a list of JSON objects
         success           = config_handler.save_config(json_sequence)                     # Write JSON actions to config
         assert(success == True)
@@ -153,16 +153,16 @@
         plate.set_date_created_to_current()
         
         config_handler = SequenceConfigHandler(self.__get_plate_filepath(plate_name))
         plate_json = plate.to_json()
         config_handler.save_config(plate_json)
         
         self.__plate_list.append(plate)
+ 
     
-
     def parse_plate_config(self, raw_json):
         metadata = raw_json["metadata"]
         
         plate_name = metadata["plate_name"]
         date_created = metadata["date_created"]
         other_data = metadata["other_data"]
         
@@ -179,13 +179,12 @@
             sequence_list
         )
         
         automation_plate.date_created = date_created
         automation_plate.other_data   = other_data
         
         
-        
     def __reformat_plate_name(self, sequence_name: str):
         return sequence_name.strip().replace(" ", "-").lower()
     
     def __get_plate_filepath(self, sequence_name: str):
         return os.path.join(self.auto_plate_config_dir, f"{self.__reformat_sequence_name(sequence_name)}.json")
```

### Comparing `amiya-0.0.1/src/amiya/automation_handler/automation_recorder.py` & `amiya-0.0.3/src/amiya/automation_handler/automation_recorder.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     def __init__(self, sequence: AutomationSequence, safety_monitor: SafetyMonitor):
         self.sequence = sequence
         self.safety_monitor = safety_monitor
         
         self.last_click_time = None
         self.is_recording = False
         
-        self.window_event: threading.Event = None
+        self.stop_event = threading.Event()
         self.label = None
         
         
     def stop_recording(self, root: tk.Tk):
-        self.window_event.set()
+        self.stop_event.set()
         self.is_recording = False
         self.sequence.actions = self.sequence.actions[:-1]    # Remove the last key click (user clicks on the Stop Recording button)
-        root.destroy()
+        root.quit()
     
     def create_indicator_window(self):
         LENGTH = 300
         WIDTH = 400
         
         root = tk.Tk()
         root.title("Recording...")
@@ -86,17 +86,14 @@
 
         self.label.config(text=f"Recording...")
 
         root.mainloop()
         
         
     def record(self, start_on_callback=False) -> AutomationSequence:
-        from elevate import elevate; elevate()
-        
-        self.window_event = threading.Event()
         threading.Thread(target=self.create_indicator_window, daemon=True).start()
         
         if start_on_callback:
             self.is_recording = True
             self.last_click_time = time.time()
             aprint("Recording in-progress (press the 'Stop Recording' button or the UP-ARROW key to stop)...")
         else:
@@ -111,15 +108,15 @@
             mouse_listener_thread     = threading.Thread(target=mouse_listener.join)
             keyboard_listener_thread  = threading.Thread(target=keyboard_listener.join)
             
             mouse_listener_thread.start()
             keyboard_listener_thread.start()
 
             # Wait until stop recording event is triggered
-            self.window_event.wait()
+            self.stop_event.wait()
 
             # Stop listeners
             mouse_listener.stop()
             keyboard_listener.stop()
 
             # Wait for listeners to finish
             mouse_listener_thread.join()
```

### Comparing `amiya-0.0.1/src/amiya/automation_handler/automation_viewer.py` & `amiya-0.0.3/src/amiya/automation_handler/automation_viewer.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/automation_handler/units/__init__.py` & `amiya-0.0.3/src/amiya/automation_handler/units/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/automation_handler/units/action.py` & `amiya-0.0.3/src/amiya/automation_handler/units/action.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,215 +54,235 @@
 00000350: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
 00000360: 636f 6f72 6469 6e61 7465 2020 2020 203d  coordinate     =
 00000370: 2063 6f6f 720d 0a20 2020 2020 2020 2073   coor..        s
 00000380: 656c 662e 6465 6c61 7920 2020 2020 2020  elf.delay       
 00000390: 2020 203d 2064 656c 6179 0d0a 2020 2020     = delay..    
 000003a0: 2020 2020 7365 6c66 2e63 6c69 636b 2020      self.click  
 000003b0: 2020 2020 2020 2020 3d20 636c 6963 6b0d          = click.
-000003c0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000003d0: 2020 2073 656c 662e 7769 6e64 6f77 5f69     self.window_i
-000003e0: 6e66 6f20 2020 203d 2077 696e 646f 775f  nfo    = window_
-000003f0: 696e 666f 0d0a 2020 2020 2020 2020 6173  info..        as
-00000400: 7365 7274 2822 7769 6474 6822 2069 6e20  sert("width" in 
-00000410: 7365 6c66 2e77 696e 646f 775f 696e 666f  self.window_info
-00000420: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00000430: 7428 2268 6569 6768 7422 2069 6e20 7365  t("height" in se
-00000440: 6c66 2e77 696e 646f 775f 696e 666f 290d  lf.window_info).
-00000450: 0a20 2020 2020 2020 2061 7373 6572 7428  .        assert(
-00000460: 2269 735f 6675 6c6c 7363 7265 656e 2220  "is_fullscreen" 
-00000470: 696e 2073 656c 662e 7769 6e64 6f77 5f69  in self.window_i
-00000480: 6e66 6f29 0d0a 200d 0a20 2020 2064 6566  nfo).. ..    def
-00000490: 2065 7865 6375 7465 2873 656c 6629 3a0d   execute(self):.
-000004a0: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
-000004b0: 2020 2020 2020 5468 6520 6465 6c61 7920        The delay 
-000004c0: 7265 7072 6573 656e 7420 7468 6520 7469  represent the ti
-000004d0: 6d65 206c 6167 2062 6574 7765 656e 2074  me lag between t
-000004e0: 6865 2063 7572 7265 6e74 2063 6c69 636b  he current click
-000004f0: 2061 6e64 2074 6865 2070 7265 7669 6f75   and the previou
-00000500: 7320 636c 6963 6b2c 0d0a 2020 2020 2020  s click,..      
-00000510: 2020 7468 6572 6566 6f72 6520 7469 6d65    therefore time
-00000520: 2e73 6c65 6570 2829 2069 7320 6578 6563  .sleep() is exec
-00000530: 7574 6564 2061 7420 7468 6520 7374 6172  uted at the star
-00000540: 7420 6f66 2061 206e 6577 2061 6374 696f  t of a new actio
-00000550: 6e2e 0d0a 2020 2020 2020 2020 2727 270d  n...        '''.
-00000560: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000570: 2020 2078 203d 2073 656c 662e 636f 6f72     x = self.coor
-00000580: 6469 6e61 7465 5b30 5d0d 0a20 2020 2020  dinate[0]..     
-00000590: 2020 2079 203d 2073 656c 662e 636f 6f72     y = self.coor
-000005a0: 6469 6e61 7465 5b31 5d0d 0a20 2020 2020  dinate[1]..     
-000005b0: 2020 2070 7961 7574 6f67 7569 2e6d 6f76     pyautogui.mov
-000005c0: 6554 6f28 782c 2079 2c20 6475 7261 7469  eTo(x, y, durati
-000005d0: 6f6e 3d30 2e31 290d 0a20 2020 2020 2020  on=0.1)..       
-000005e0: 200d 0a20 2020 2020 2020 2069 6620 7365   ..        if se
-000005f0: 6c66 2e63 6c69 636b 3a0d 0a20 2020 2020  lf.click:..     
-00000600: 2020 2020 2020 2023 2070 7961 7574 6f67         # pyautog
-00000610: 7569 2e63 6c69 636b 2869 6e74 6572 7661  ui.click(interva
-00000620: 6c3d 302e 3129 0d0a 2020 2020 2020 2020  l=0.1)..        
-00000630: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00000640: 2020 7079 6175 746f 6775 692e 6d6f 7573    pyautogui.mous
-00000650: 6544 6f77 6e28 290d 0a20 2020 2020 2020  eDown()..       
-00000660: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-00000670: 302e 3129 2020 0d0a 2020 2020 2020 2020  0.1)  ..        
-00000680: 2020 2020 7079 6175 746f 6775 692e 6d6f      pyautogui.mo
-00000690: 7573 6555 7028 290d 0a20 2020 200d 0a20  useUp()..    .. 
-000006a0: 2020 2064 6566 2074 6f5f 6a73 6f6e 2873     def to_json(s
-000006b0: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-000006c0: 6574 7572 6e20 7b0d 0a20 2020 2020 2020  eturn {..       
-000006d0: 2020 2020 2022 636f 6f72 6469 6e61 7465       "coordinate
-000006e0: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-000006f0: 2020 2020 2020 2278 223a 2073 656c 662e        "x": self.
-00000700: 636f 6f72 6469 6e61 7465 5b30 5d2c 0d0a  coordinate[0],..
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2279 223a 2073 656c 662e 636f 6f72 6469  "y": self.coordi
-00000730: 6e61 7465 5b31 5d0d 0a20 2020 2020 2020  nate[1]..       
-00000740: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00000750: 2020 2020 2022 6465 6c61 7922 3a20 7365       "delay": se
-00000760: 6c66 2e64 656c 6179 2c0d 0a20 2020 2020  lf.delay,..     
-00000770: 2020 2020 2020 2022 636c 6963 6b22 3a20         "click": 
-00000780: 7365 6c66 2e63 6c69 636b 2c0d 0a20 2020  self.click,..   
-00000790: 2020 2020 2020 2020 2022 7769 6e64 6f77           "window
-000007a0: 5f69 6e66 6f22 3a20 7365 6c66 2e77 696e  _info": self.win
-000007b0: 646f 775f 696e 666f 0d0a 2020 2020 2020  dow_info..      
-000007c0: 2020 7d0d 0a20 2020 2020 2020 200d 0a20    }..        .. 
-000007d0: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
-000007e0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000007f0: 7265 7475 726e 2066 224d 6f75 7365 4163  return f"MouseAc
-00000800: 7469 6f6e 2863 6f6f 723d 7b73 656c 662e  tion(coor={self.
-00000810: 636f 6f72 6469 6e61 7465 7d2c 2064 656c  coordinate}, del
-00000820: 6179 3d7b 726f 756e 6428 7365 6c66 2e64  ay={round(self.d
-00000830: 656c 6179 2c20 3229 7d2c 2063 6c69 636b  elay, 2)}, click
-00000840: 3d7b 7365 6c66 2e63 6c69 636b 7d29 220d  ={self.click})".
-00000850: 0a0d 0a0d 0a63 6c61 7373 204b 6579 626f  .....class Keybo
-00000860: 6172 6441 6374 696f 6e28 4163 7469 6f6e  ardAction(Action
-00000870: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-00000880: 6974 5f5f 2873 656c 662c 206b 6579 3a20  it__(self, key: 
-00000890: 7374 722c 2064 656c 6179 3a20 666c 6f61  str, delay: floa
-000008a0: 7429 3a0d 0a20 2020 2020 2020 2073 656c  t):..        sel
-000008b0: 662e 6b65 7920 3d20 7365 6c66 2e72 6566  f.key = self.ref
-000008c0: 6f72 6d61 745f 6b65 7928 6b65 7929 0d0a  ormat_key(key)..
-000008d0: 2020 2020 2020 2020 7365 6c66 2e64 656c          self.del
-000008e0: 6179 203d 2064 656c 6179 0d0a 2020 2020  ay = delay..    
-000008f0: 0d0a 2020 2020 6465 6620 6578 6563 7574  ..    def execut
-00000900: 6528 7365 6c66 2c20 6b65 7962 6f61 7264  e(self, keyboard
-00000910: 293a 0d0a 2020 2020 2020 2020 2727 270d  ):..        '''.
-00000920: 0a20 2020 2020 2020 2054 6865 2064 656c  .        The del
-00000930: 6179 2072 6570 7265 7365 6e74 2074 6865  ay represent the
-00000940: 2074 696d 6520 6c61 6720 6265 7477 6565   time lag betwee
-00000950: 6e20 7468 6520 6375 7272 656e 7420 636c  n the current cl
-00000960: 6963 6b20 616e 6420 7468 6520 7072 6576  ick and the prev
-00000970: 696f 7573 2063 6c69 636b 2c0d 0a20 2020  ious click,..   
-00000980: 2020 2020 2074 6865 7265 666f 7265 2074       therefore t
-00000990: 696d 652e 736c 6565 7028 2920 6973 2065  ime.sleep() is e
-000009a0: 7865 6375 7465 6420 6174 2074 6865 2073  xecuted at the s
-000009b0: 7461 7274 206f 6620 6120 6e65 7720 6163  tart of a new ac
-000009c0: 7469 6f6e 2e0d 0a20 2020 2020 2020 2027  tion...        '
-000009d0: 2727 0d0a 2020 2020 2020 2020 0d0a 2020  ''..        ..  
-000009e0: 2020 2020 2020 7365 6c66 2e70 7265 7373        self.press
-000009f0: 5f6b 6579 2873 656c 662e 6b65 792c 206b  _key(self.key, k
-00000a00: 6579 626f 6172 6429 0d0a 2020 2020 0d0a  eyboard)..    ..
-00000a10: 2020 2020 6465 6620 746f 5f6a 736f 6e28      def to_json(
-00000a20: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00000a30: 7265 7475 726e 207b 0d0a 2020 2020 2020  return {..      
-00000a40: 2020 2020 2020 226b 6579 223a 2073 656c        "key": sel
-00000a50: 662e 6b65 792c 0d0a 2020 2020 2020 2020  f.key,..        
-00000a60: 2020 2020 2264 656c 6179 223a 2073 656c      "delay": sel
-00000a70: 662e 6465 6c61 790d 0a20 2020 2020 2020  f.delay..       
-00000a80: 207d 0d0a 2020 2020 2020 2020 0d0a 2020   }..        ..  
-00000a90: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
-00000aa0: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00000ab0: 6574 7572 6e20 6622 4b65 7962 6f61 7264  eturn f"Keyboard
-00000ac0: 4163 7469 6f6e 286b 6579 3d7b 7365 6c66  Action(key={self
-00000ad0: 2e6b 6579 7d2c 2064 656c 6179 3d7b 726f  .key}, delay={ro
-00000ae0: 756e 6428 7365 6c66 2e64 656c 6179 2c20  und(self.delay, 
-00000af0: 3229 7d29 220d 0a0d 0a20 2020 2064 6566  2)})"....    def
-00000b00: 2070 7265 7373 5f6b 6579 2873 656c 662c   press_key(self,
-00000b10: 206b 6579 3a20 7374 722c 2070 796e 7075   key: str, pynpu
-00000b20: 745f 6b65 7962 6f61 7264 3a20 7079 6e70  t_keyboard: pynp
-00000b30: 7574 2e6b 6579 626f 6172 642e 436f 6e74  ut.keyboard.Cont
-00000b40: 726f 6c6c 6572 293a 0d0a 2020 2020 2020  roller):..      
-00000b50: 2020 2727 270d 0a20 2020 2020 2020 2054    '''..        T
-00000b60: 6869 7320 6973 2067 6f69 6e67 2074 6f20  his is going to 
-00000b70: 6265 2061 2064 6966 6669 6375 6c74 2074  be a difficult t
-00000b80: 6f20 6578 706c 6169 6e2c 2062 7574 2065  o explain, but e
-00000b90: 7373 656e 7469 616c 6c79 2074 6865 2073  ssentially the s
-00000ba0: 7472 696e 6720 666f 726d 6174 206b 6579  tring format key
-00000bb0: 730d 0a20 2020 2020 2020 2072 6563 6f72  s..        recor
-00000bc0: 6465 6420 6279 2070 796e 7075 7420 6361  ded by pynput ca
-00000bd0: 6e27 7420 6265 2072 652d 7265 636f 676e  n't be re-recogn
-00000be0: 697a 6564 2062 7920 7079 6e70 7574 2066  ized by pynput f
-00000bf0: 6f72 2065 7865 6375 7469 6f6e 2e20 5468  or execution. Th
-00000c00: 6572 6566 6f72 652c 2061 206d 6170 7069  erefore, a mappi
-00000c10: 6e67 0d0a 2020 2020 2020 2020 6265 7477  ng..        betw
-00000c20: 6565 6e20 7468 6520 7374 7269 6e67 2066  een the string f
-00000c30: 6f72 6d61 7465 6420 6b65 7973 2028 636f  ormated keys (co
-00000c40: 6c6c 6563 7465 6420 6279 2070 796e 7075  llected by pynpu
-00000c50: 7420 6974 7365 6c66 2920 616e 6420 7468  t itself) and th
-00000c60: 6520 6163 7475 616c 204b 6579 206f 626a  e actual Key obj
-00000c70: 6563 740d 0a20 2020 2020 2020 2069 7320  ect..        is 
-00000c80: 7573 6564 2074 6f20 636f 6e76 6572 7420  used to convert 
-00000c90: 7468 6520 6b65 7920 7768 656e 2074 7279  the key when try
-00000ca0: 696e 6720 746f 2065 7865 6375 7465 2074  ing to execute t
-00000cb0: 6865 206b 6579 626f 6172 6420 6163 7469  he keyboard acti
-00000cc0: 6f6e 2e0d 0a20 2020 2020 2020 200d 0a20  on...        .. 
-00000cd0: 2020 2020 2020 2054 6865 7265 2061 7265         There are
-00000ce0: 2067 6f69 6e67 2074 6f20 6265 2061 2077   going to be a w
-00000cf0: 6964 6520 7261 6e67 6520 6f66 206b 6579  ide range of key
-00000d00: 7320 7468 6174 2061 7265 6e27 7420 7375  s that aren't su
-00000d10: 7070 6f72 7465 6420 696e 636c 7564 696e  pported includin
-00000d20: 6720 2268 6f74 6b65 7973 2220 6f72 0d0a  g "hotkeys" or..
-00000d30: 2020 2020 2020 2020 6120 636f 6d62 696e          a combin
-00000d40: 6174 696f 6e20 6f66 2074 776f 2064 6966  ation of two dif
-00000d50: 6665 7265 6e74 206b 6579 732e 2054 6869  ferent keys. Thi
-00000d60: 7320 7769 6c6c 206e 6565 6420 746f 2062  s will need to b
-00000d70: 6520 7370 6563 6966 6965 6420 696e 2074  e specified in t
-00000d80: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
-00000d90: 2e0d 0a20 2020 2020 2020 2027 2727 0d0a  ...        '''..
-00000da0: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
-00000db0: 6669 6e64 2061 2062 6574 7465 7220 7761  find a better wa
-00000dc0: 7920 746f 2069 6d70 6c65 6d65 6e74 2074  y to implement t
-00000dd0: 6869 732c 2069 6620 706f 7373 6962 6c65  his, if possible
-00000de0: 0d0a 2020 2020 2020 2020 7079 6e70 7574  ..        pynput
-00000df0: 5f6b 6579 203d 2050 594e 5055 545f 4b45  _key = PYNPUT_KE
-00000e00: 595f 4d41 5050 494e 472e 6765 7428 6b65  Y_MAPPING.get(ke
-00000e10: 792c 206b 6579 290d 0a20 2020 2020 2020  y, key)..       
-00000e20: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00000e30: 2020 2070 796e 7075 745f 6b65 7962 6f61     pynput_keyboa
-00000e40: 7264 2e70 7265 7373 2870 796e 7075 745f  rd.press(pynput_
-00000e50: 6b65 7929 0d0a 2020 2020 2020 2020 2020  key)..          
-00000e60: 2020 7469 6d65 2e73 6c65 6570 2830 2e30    time.sleep(0.0
-00000e70: 3529 0d0a 2020 2020 2020 2020 2020 2020  5)..            
-00000e80: 7079 6e70 7574 5f6b 6579 626f 6172 642e  pynput_keyboard.
-00000e90: 7265 6c65 6173 6528 7079 6e70 7574 5f6b  release(pynput_k
-00000ea0: 6579 290d 0a20 2020 2020 2020 2065 7863  ey)..        exc
-00000eb0: 6570 7420 286b 6579 626f 6172 642e 436f  ept (keyboard.Co
-00000ec0: 6e74 726f 6c6c 6572 2e49 6e76 616c 6964  ntroller.Invalid
-00000ed0: 4b65 7945 7863 6570 7469 6f6e 2c20 5661  KeyException, Va
-00000ee0: 6c75 6545 7272 6f72 2920 6173 2065 783a  lueError) as ex:
-00000ef0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00000f00: 544f 444f 3a20 6c6f 6720 7468 6973 2075  TODO: log this u
-00000f10: 6e73 7570 706f 7274 6564 206b 6579 2061  nsupported key a
-00000f20: 7320 6f70 706f 7365 6420 746f 2070 7269  s opposed to pri
-00000f30: 6e74 2069 740d 0a20 2020 2020 2020 2020  nt it..         
-00000f40: 2020 2023 2070 7269 6e74 2866 2255 6e73     # print(f"Uns
-00000f50: 7570 706f 7274 6564 206b 6579 3a20 3c7b  upported key: <{
-00000f60: 6b65 797d 3e22 290d 0a20 2020 2020 2020  key}>")..       
-00000f70: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-00000f80: 2020 200d 0a20 2020 2064 6566 2072 6566     ..    def ref
-00000f90: 6f72 6d61 745f 6b65 7928 7365 6c66 2c20  ormat_key(self, 
-00000fa0: 6b65 793a 206b 6579 626f 6172 642e 4b65  key: keyboard.Ke
-00000fb0: 7929 202d 3e20 7374 723a 0d0a 2020 2020  y) -> str:..    
-00000fc0: 2020 2020 6b65 793a 2073 7472 203d 2073      key: str = s
-00000fd0: 7472 286b 6579 292e 7374 7269 7028 292e  tr(key).strip().
-00000fe0: 7265 706c 6163 6528 2227 222c 2022 2229  replace("'", "")
-00000ff0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00001000: 2020 2020 7265 6d6f 7669 6e67 203d 205b      removing = [
-00001010: 225f 7222 2c20 225f 6772 222c 2022 5f6c  "_r", "_gr", "_l
-00001020: 225d 0d0a 2020 2020 2020 2020 666f 7220  "]..        for 
-00001030: 7375 6666 6978 2069 6e20 7265 6d6f 7669  suffix in removi
-00001040: 6e67 3a0d 0a20 2020 2020 2020 2020 2020  ng:..           
-00001050: 2069 6620 6b65 792e 656e 6473 7769 7468   if key.endswith
-00001060: 2873 7566 6669 7829 3a0d 0a20 2020 2020  (suffix):..     
-00001070: 2020 2020 2020 2020 2020 206b 6579 203d             key =
-00001080: 206b 6579 2e72 6570 6c61 6365 2873 7566   key.replace(suf
-00001090: 6669 782c 2022 2229 0d0a 0d0a 2020 2020  fix, "")....    
-000010a0: 2020 2020 7265 7475 726e 206b 6579 0d0a      return key..
-000010b0: 2020 2020                                    
+000003c0: 0a20 2020 2020 2020 2073 656c 662e 7769  .        self.wi
+000003d0: 6e64 6f77 5f69 6e66 6f20 2020 203d 2077  ndow_info    = w
+000003e0: 696e 646f 775f 696e 666f 0d0a 2020 2020  indow_info..    
+000003f0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+00000400: 6c66 2e69 735f 7661 6c69 645f 666f 725f  lf.is_valid_for_
+00000410: 7069 7865 6c5f 6361 6c63 203d 2073 656c  pixel_calc = sel
+00000420: 662e 5f5f 6973 5f76 616c 6964 5f66 6f72  f.__is_valid_for
+00000430: 5f70 6978 656c 5f63 616c 6328 290d 0a20  _pixel_calc().. 
+00000440: 0d0a 2020 2020 6465 6620 6578 6563 7574  ..    def execut
+00000450: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
+00000460: 2020 2727 270d 0a20 2020 2020 2020 2054    '''..        T
+00000470: 6865 2064 656c 6179 2072 6570 7265 7365  he delay represe
+00000480: 6e74 2074 6865 2074 696d 6520 6c61 6720  nt the time lag 
+00000490: 6265 7477 6565 6e20 7468 6520 6375 7272  between the curr
+000004a0: 656e 7420 636c 6963 6b20 616e 6420 7468  ent click and th
+000004b0: 6520 7072 6576 696f 7573 2063 6c69 636b  e previous click
+000004c0: 2c0d 0a20 2020 2020 2020 2074 6865 7265  ,..        there
+000004d0: 666f 7265 2074 696d 652e 736c 6565 7028  fore time.sleep(
+000004e0: 2920 6973 2065 7865 6375 7465 6420 6174  ) is executed at
+000004f0: 2074 6865 2073 7461 7274 206f 6620 6120   the start of a 
+00000500: 6e65 7720 6163 7469 6f6e 2e0d 0a20 2020  new action...   
+00000510: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
+00000520: 2020 0d0a 2020 2020 2020 2020 7820 3d20    ..        x = 
+00000530: 7365 6c66 2e63 6f6f 7264 696e 6174 655b  self.coordinate[
+00000540: 305d 0d0a 2020 2020 2020 2020 7920 3d20  0]..        y = 
+00000550: 7365 6c66 2e63 6f6f 7264 696e 6174 655b  self.coordinate[
+00000560: 315d 0d0a 2020 2020 2020 2020 7079 6175  1]..        pyau
+00000570: 746f 6775 692e 6d6f 7665 546f 2878 2c20  togui.moveTo(x, 
+00000580: 792c 2064 7572 6174 696f 6e3d 302e 3129  y, duration=0.1)
+00000590: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000005a0: 2020 2020 6966 2073 656c 662e 636c 6963      if self.clic
+000005b0: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
+000005c0: 2320 7079 6175 746f 6775 692e 636c 6963  # pyautogui.clic
+000005d0: 6b28 696e 7465 7276 616c 3d30 2e31 290d  k(interval=0.1).
+000005e0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+000005f0: 2020 2020 2020 2020 2020 2070 7961 7574             pyaut
+00000600: 6f67 7569 2e6d 6f75 7365 446f 776e 2829  ogui.mouseDown()
+00000610: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
+00000620: 6d65 2e73 6c65 6570 2830 2e31 2920 200d  me.sleep(0.1)  .
+00000630: 0a20 2020 2020 2020 2020 2020 2070 7961  .            pya
+00000640: 7574 6f67 7569 2e6d 6f75 7365 5570 2829  utogui.mouseUp()
+00000650: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00000660: 746f 5f6a 736f 6e28 7365 6c66 293a 0d0a  to_json(self):..
+00000670: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+00000680: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
+00000690: 6f6f 7264 696e 6174 6522 3a20 7b0d 0a20  oordinate": {.. 
+000006a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000006b0: 7822 3a20 7365 6c66 2e63 6f6f 7264 696e  x": self.coordin
+000006c0: 6174 655b 305d 2c0d 0a20 2020 2020 2020  ate[0],..       
+000006d0: 2020 2020 2020 2020 2022 7922 3a20 7365           "y": se
+000006e0: 6c66 2e63 6f6f 7264 696e 6174 655b 315d  lf.coordinate[1]
+000006f0: 0d0a 2020 2020 2020 2020 2020 2020 7d2c  ..            },
+00000700: 0d0a 2020 2020 2020 2020 2020 2020 2264  ..            "d
+00000710: 656c 6179 223a 2073 656c 662e 6465 6c61  elay": self.dela
+00000720: 792c 0d0a 2020 2020 2020 2020 2020 2020  y,..            
+00000730: 2263 6c69 636b 223a 2073 656c 662e 636c  "click": self.cl
+00000740: 6963 6b2c 0d0a 2020 2020 2020 2020 2020  ick,..          
+00000750: 2020 2277 696e 646f 775f 696e 666f 223a    "window_info":
+00000760: 2073 656c 662e 7769 6e64 6f77 5f69 6e66   self.window_inf
+00000770: 6f0d 0a20 2020 2020 2020 207d 0d0a 2020  o..        }..  
+00000780: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
+00000790: 5f5f 7265 7072 5f5f 2873 656c 6629 3a0d  __repr__(self):.
+000007a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000007b0: 6622 4d6f 7573 6541 6374 696f 6e28 636f  f"MouseAction(co
+000007c0: 6f72 3d7b 7365 6c66 2e63 6f6f 7264 696e  or={self.coordin
+000007d0: 6174 657d 2c20 6465 6c61 793d 7b72 6f75  ate}, delay={rou
+000007e0: 6e64 2873 656c 662e 6465 6c61 792c 2032  nd(self.delay, 2
+000007f0: 297d 2c20 636c 6963 6b3d 7b73 656c 662e  )}, click={self.
+00000800: 636c 6963 6b7d 2922 0d0a 0d0a 2020 2020  click})"....    
+00000810: 6465 6620 5f5f 6973 5f76 616c 6964 5f66  def __is_valid_f
+00000820: 6f72 5f70 6978 656c 5f63 616c 6328 7365  or_pixel_calc(se
+00000830: 6c66 293a 0d0a 2020 2020 2020 2020 7472  lf):..        tr
+00000840: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00000850: 6173 7365 7274 2822 7769 6474 6822 2069  assert("width" i
+00000860: 6e20 7365 6c66 2e77 696e 646f 775f 696e  n self.window_in
+00000870: 666f 290d 0a20 2020 2020 2020 2020 2020  fo)..           
+00000880: 2061 7373 6572 7428 2268 6569 6768 7422   assert("height"
+00000890: 2069 6e20 7365 6c66 2e77 696e 646f 775f   in self.window_
+000008a0: 696e 666f 290d 0a20 2020 2020 2020 2020  info)..         
+000008b0: 2020 2061 7373 6572 7428 2274 6f70 2220     assert("top" 
+000008c0: 696e 2073 656c 662e 7769 6e64 6f77 5f69  in self.window_i
+000008d0: 6e66 6f29 0d0a 2020 2020 2020 2020 2020  nfo)..          
+000008e0: 2020 6173 7365 7274 2822 6c65 6674 2220    assert("left" 
+000008f0: 696e 2073 656c 662e 7769 6e64 6f77 5f69  in self.window_i
+00000900: 6e66 6f29 0d0a 2020 2020 2020 2020 2020  nfo)..          
+00000910: 2020 6173 7365 7274 2822 6973 5f66 756c    assert("is_ful
+00000920: 6c73 6372 6565 6e22 2069 6e20 7365 6c66  lscreen" in self
+00000930: 2e77 696e 646f 775f 696e 666f 290d 0a20  .window_info).. 
+00000940: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000950: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
+00000960: 6578 6365 7074 2041 7373 6572 7469 6f6e  except Assertion
+00000970: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
+00000980: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00000990: 0d0a 0d0a 636c 6173 7320 4b65 7962 6f61  ....class Keyboa
+000009a0: 7264 4163 7469 6f6e 2841 6374 696f 6e29  rdAction(Action)
+000009b0: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
+000009c0: 745f 5f28 7365 6c66 2c20 6b65 793a 2073  t__(self, key: s
+000009d0: 7472 2c20 6465 6c61 793a 2066 6c6f 6174  tr, delay: float
+000009e0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+000009f0: 2e6b 6579 203d 2073 656c 662e 7265 666f  .key = self.refo
+00000a00: 726d 6174 5f6b 6579 286b 6579 290d 0a20  rmat_key(key).. 
+00000a10: 2020 2020 2020 2073 656c 662e 6465 6c61         self.dela
+00000a20: 7920 3d20 6465 6c61 790d 0a20 2020 200d  y = delay..    .
+00000a30: 0a20 2020 2064 6566 2065 7865 6375 7465  .    def execute
+00000a40: 2873 656c 662c 206b 6579 626f 6172 6429  (self, keyboard)
+00000a50: 3a0d 0a20 2020 2020 2020 2027 2727 0d0a  :..        '''..
+00000a60: 2020 2020 2020 2020 5468 6520 6465 6c61          The dela
+00000a70: 7920 7265 7072 6573 656e 7420 7468 6520  y represent the 
+00000a80: 7469 6d65 206c 6167 2062 6574 7765 656e  time lag between
+00000a90: 2074 6865 2063 7572 7265 6e74 2063 6c69   the current cli
+00000aa0: 636b 2061 6e64 2074 6865 2070 7265 7669  ck and the previ
+00000ab0: 6f75 7320 636c 6963 6b2c 0d0a 2020 2020  ous click,..    
+00000ac0: 2020 2020 7468 6572 6566 6f72 6520 7469      therefore ti
+00000ad0: 6d65 2e73 6c65 6570 2829 2069 7320 6578  me.sleep() is ex
+00000ae0: 6563 7574 6564 2061 7420 7468 6520 7374  ecuted at the st
+00000af0: 6172 7420 6f66 2061 206e 6577 2061 6374  art of a new act
+00000b00: 696f 6e2e 0d0a 2020 2020 2020 2020 2727  ion...        ''
+00000b10: 270d 0a20 2020 2020 2020 200d 0a20 2020  '..        ..   
+00000b20: 2020 2020 2073 656c 662e 7072 6573 735f       self.press_
+00000b30: 6b65 7928 7365 6c66 2e6b 6579 2c20 6b65  key(self.key, ke
+00000b40: 7962 6f61 7264 290d 0a20 2020 200d 0a20  yboard)..    .. 
+00000b50: 2020 2064 6566 2074 6f5f 6a73 6f6e 2873     def to_json(s
+00000b60: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00000b70: 6574 7572 6e20 7b0d 0a20 2020 2020 2020  eturn {..       
+00000b80: 2020 2020 2022 6b65 7922 3a20 7365 6c66       "key": self
+00000b90: 2e6b 6579 2c0d 0a20 2020 2020 2020 2020  .key,..         
+00000ba0: 2020 2022 6465 6c61 7922 3a20 7365 6c66     "delay": self
+00000bb0: 2e64 656c 6179 0d0a 2020 2020 2020 2020  .delay..        
+00000bc0: 7d0d 0a20 2020 2020 2020 200d 0a20 2020  }..        ..   
+00000bd0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+00000be0: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+00000bf0: 7475 726e 2066 224b 6579 626f 6172 6441  turn f"KeyboardA
+00000c00: 6374 696f 6e28 6b65 793d 7b73 656c 662e  ction(key={self.
+00000c10: 6b65 797d 2c20 6465 6c61 793d 7b72 6f75  key}, delay={rou
+00000c20: 6e64 2873 656c 662e 6465 6c61 792c 2032  nd(self.delay, 2
+00000c30: 297d 2922 0d0a 0d0a 2020 2020 6465 6620  )})"....    def 
+00000c40: 7072 6573 735f 6b65 7928 7365 6c66 2c20  press_key(self, 
+00000c50: 6b65 793a 2073 7472 2c20 7079 6e70 7574  key: str, pynput
+00000c60: 5f6b 6579 626f 6172 643a 2070 796e 7075  _keyboard: pynpu
+00000c70: 742e 6b65 7962 6f61 7264 2e43 6f6e 7472  t.keyboard.Contr
+00000c80: 6f6c 6c65 7229 3a0d 0a20 2020 2020 2020  oller):..       
+00000c90: 2027 2727 0d0a 2020 2020 2020 2020 5468   '''..        Th
+00000ca0: 6973 2069 7320 676f 696e 6720 746f 2062  is is going to b
+00000cb0: 6520 6120 6469 6666 6963 756c 7420 746f  e a difficult to
+00000cc0: 2065 7870 6c61 696e 2c20 6275 7420 6573   explain, but es
+00000cd0: 7365 6e74 6961 6c6c 7920 7468 6520 7374  sentially the st
+00000ce0: 7269 6e67 2066 6f72 6d61 7420 6b65 7973  ring format keys
+00000cf0: 0d0a 2020 2020 2020 2020 7265 636f 7264  ..        record
+00000d00: 6564 2062 7920 7079 6e70 7574 2063 616e  ed by pynput can
+00000d10: 2774 2062 6520 7265 2d72 6563 6f67 6e69  't be re-recogni
+00000d20: 7a65 6420 6279 2070 796e 7075 7420 666f  zed by pynput fo
+00000d30: 7220 6578 6563 7574 696f 6e2e 2054 6865  r execution. The
+00000d40: 7265 666f 7265 2c20 6120 6d61 7070 696e  refore, a mappin
+00000d50: 670d 0a20 2020 2020 2020 2062 6574 7765  g..        betwe
+00000d60: 656e 2074 6865 2073 7472 696e 6720 666f  en the string fo
+00000d70: 726d 6174 6564 206b 6579 7320 2863 6f6c  rmated keys (col
+00000d80: 6c65 6374 6564 2062 7920 7079 6e70 7574  lected by pynput
+00000d90: 2069 7473 656c 6629 2061 6e64 2074 6865   itself) and the
+00000da0: 2061 6374 7561 6c20 4b65 7920 6f62 6a65   actual Key obje
+00000db0: 6374 0d0a 2020 2020 2020 2020 6973 2075  ct..        is u
+00000dc0: 7365 6420 746f 2063 6f6e 7665 7274 2074  sed to convert t
+00000dd0: 6865 206b 6579 2077 6865 6e20 7472 7969  he key when tryi
+00000de0: 6e67 2074 6f20 6578 6563 7574 6520 7468  ng to execute th
+00000df0: 6520 6b65 7962 6f61 7264 2061 6374 696f  e keyboard actio
+00000e00: 6e2e 0d0a 2020 2020 2020 2020 0d0a 2020  n...        ..  
+00000e10: 2020 2020 2020 5468 6572 6520 6172 6520        There are 
+00000e20: 676f 696e 6720 746f 2062 6520 6120 7769  going to be a wi
+00000e30: 6465 2072 616e 6765 206f 6620 6b65 7973  de range of keys
+00000e40: 2074 6861 7420 6172 656e 2774 2073 7570   that aren't sup
+00000e50: 706f 7274 6564 2069 6e63 6c75 6469 6e67  ported including
+00000e60: 2022 686f 746b 6579 7322 206f 720d 0a20   "hotkeys" or.. 
+00000e70: 2020 2020 2020 2061 2063 6f6d 6269 6e61         a combina
+00000e80: 7469 6f6e 206f 6620 7477 6f20 6469 6666  tion of two diff
+00000e90: 6572 656e 7420 6b65 7973 2e20 5468 6973  erent keys. This
+00000ea0: 2077 696c 6c20 6e65 6564 2074 6f20 6265   will need to be
+00000eb0: 2073 7065 6369 6669 6564 2069 6e20 7468   specified in th
+00000ec0: 6520 646f 6375 6d65 6e74 6174 696f 6e2e  e documentation.
+00000ed0: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
+00000ee0: 2020 2020 2020 2023 2054 4f44 4f3a 2066         # TODO: f
+00000ef0: 696e 6420 6120 6265 7474 6572 2077 6179  ind a better way
+00000f00: 2074 6f20 696d 706c 656d 656e 7420 7468   to implement th
+00000f10: 6973 2c20 6966 2070 6f73 7369 626c 650d  is, if possible.
+00000f20: 0a20 2020 2020 2020 2070 796e 7075 745f  .        pynput_
+00000f30: 6b65 7920 3d20 5059 4e50 5554 5f4b 4559  key = PYNPUT_KEY
+00000f40: 5f4d 4150 5049 4e47 2e67 6574 286b 6579  _MAPPING.get(key
+00000f50: 2c20 6b65 7929 0d0a 2020 2020 2020 2020  , key)..        
+00000f60: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00000f70: 2020 7079 6e70 7574 5f6b 6579 626f 6172    pynput_keyboar
+00000f80: 642e 7072 6573 7328 7079 6e70 7574 5f6b  d.press(pynput_k
+00000f90: 6579 290d 0a20 2020 2020 2020 2020 2020  ey)..           
+00000fa0: 2074 696d 652e 736c 6565 7028 302e 3035   time.sleep(0.05
+00000fb0: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00000fc0: 796e 7075 745f 6b65 7962 6f61 7264 2e72  ynput_keyboard.r
+00000fd0: 656c 6561 7365 2870 796e 7075 745f 6b65  elease(pynput_ke
+00000fe0: 7929 0d0a 2020 2020 2020 2020 6578 6365  y)..        exce
+00000ff0: 7074 2028 6b65 7962 6f61 7264 2e43 6f6e  pt (keyboard.Con
+00001000: 7472 6f6c 6c65 722e 496e 7661 6c69 644b  troller.InvalidK
+00001010: 6579 4578 6365 7074 696f 6e2c 2056 616c  eyException, Val
+00001020: 7565 4572 726f 7229 2061 7320 6578 3a0d  ueError) as ex:.
+00001030: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00001040: 4f44 4f3a 206c 6f67 2074 6869 7320 756e  ODO: log this un
+00001050: 7375 7070 6f72 7465 6420 6b65 7920 6173  supported key as
+00001060: 206f 7070 6f73 6564 2074 6f20 7072 696e   opposed to prin
+00001070: 7420 6974 0d0a 2020 2020 2020 2020 2020  t it..          
+00001080: 2020 2320 7072 696e 7428 6622 556e 7375    # print(f"Unsu
+00001090: 7070 6f72 7465 6420 6b65 793a 203c 7b6b  pported key: <{k
+000010a0: 6579 7d3e 2229 0d0a 2020 2020 2020 2020  ey}>")..        
+000010b0: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
+000010c0: 2020 0d0a 2020 2020 6465 6620 7265 666f    ..    def refo
+000010d0: 726d 6174 5f6b 6579 2873 656c 662c 206b  rmat_key(self, k
+000010e0: 6579 3a20 6b65 7962 6f61 7264 2e4b 6579  ey: keyboard.Key
+000010f0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+00001100: 2020 206b 6579 3a20 7374 7220 3d20 7374     key: str = st
+00001110: 7228 6b65 7929 2e73 7472 6970 2829 2e72  r(key).strip().r
+00001120: 6570 6c61 6365 2822 2722 2c20 2222 290d  eplace("'", "").
+00001130: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00001140: 2020 2072 656d 6f76 696e 6720 3d20 5b22     removing = ["
+00001150: 5f72 222c 2022 5f67 7222 2c20 225f 6c22  _r", "_gr", "_l"
+00001160: 5d0d 0a20 2020 2020 2020 2066 6f72 2073  ]..        for s
+00001170: 7566 6669 7820 696e 2072 656d 6f76 696e  uffix in removin
+00001180: 673a 0d0a 2020 2020 2020 2020 2020 2020  g:..            
+00001190: 6966 206b 6579 2e65 6e64 7377 6974 6828  if key.endswith(
+000011a0: 7375 6666 6978 293a 0d0a 2020 2020 2020  suffix):..      
+000011b0: 2020 2020 2020 2020 2020 6b65 7920 3d20            key = 
+000011c0: 6b65 792e 7265 706c 6163 6528 7375 6666  key.replace(suff
+000011d0: 6978 2c20 2222 290d 0a0d 0a20 2020 2020  ix, "")....     
+000011e0: 2020 2072 6574 7572 6e20 6b65 790d 0a20     return key.. 
+000011f0: 2020 20
```

### Comparing `amiya-0.0.1/src/amiya/automation_handler/units/plate.py` & `amiya-0.0.3/src/amiya/automation_handler/units/plate.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/automation_handler/units/sequence.py` & `amiya-0.0.3/src/amiya/automation_handler/units/sequence.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import time
+import copy
 from datetime import datetime
 from pynput import keyboard
 from amiya.automation_handler.automation_config_handler import SequenceConfigHandler
 from amiya.automation_handler.units.action import Action, MouseAction, KeyboardAction
 from amiya.exceptions.exceptions import AmiyaBaseException, Amiya_AppNotFocusedException
-from amiya.utils.constants import FORCE_ACTIONS_DELAY
+from amiya.utils.constants import FORCE_ACTIONS_DELAY, VERSION
 from amiya.utils.helper import *
 from amiya.apps_manager.safety_monitor import SafetyMonitor
 from amiya.pixel_calculator.resolution_detector import ResolutionDetector
 from amiya.pixel_calculator.pixel_calculator import PixelCalculator
 
 class AutomationSequence:
     def __init__(
@@ -20,34 +21,68 @@
         self.date_created: datetime         = None                          # Default to None (and set at to_json() and parse_json())
         self.primary_monitor_info: dict     = None                          # Fetch PRIMARY monitor's size (width x height)
         self.other_data                     = None
         self.actions: list[Action]          = []
         
         self.global_delay                   = 0
     
+    
+    def __progress_bar(self, actions: list[Action], prefix="", size=40, out=sys.stdout):
+        count = len(actions)
+        start = time.time() # time estimate start
+        total_time = self.get_runtime()
+        
+        
+        def show(j, delay, remaining_time_str):
+            x = int(size*j/count)   
+            aprint(f"{prefix}|{u'█'*x}{(' '*(size-x))}| {int(j)}/{count}  -  Remaining: {remaining_time_str}", end='\r', file=out, flush=True) 
+        
+        def secs_to_str(secs):
+            mins, sec = divmod(secs, 60)
+            time_str = f"{int(mins)} mins {round(sec, 2)} secs"
+            return time_str
+        
+        show(0.1, delay=actions[0].delay, remaining_time_str=secs_to_str(total_time)) # avoid div/0 
+        for i, action in enumerate(actions):
+            yield action
+            
+            total_time -= action.delay
+            show(i+1, action.delay, secs_to_str(total_time))
+            
+        print("", flush=True, file=out)
+    
+    
     def execute(self, safety_monitor: SafetyMonitor):
         
         def verbose_action(idx: int, action: Action):
             buffer_space = " "*5                                # Verbose current action
             aprint(f"(CMD {idx+1}/{len(self.actions)}) Executing: {action.__repr__()}{buffer_space}", end="\r")
         
-        pixel_calculator = PixelCalculator(self.primary_monitor_info)
+        def verbose_warning():
+            # Verbose warning if the current action isn't suited for the pixel calculator developed in ver0.0.2+
+            for action in self.actions:
+                if isinstance(action, MouseAction) and action.is_valid_for_pixel_calc == False:
+                    aprint(f"This automation sequence is not available for pixel calculator in version {VERSION}.")
+                    return
+        
+
+        # Becuase the pixel calculator will directory modify the MouseAction's coordinates, we need a way to reset the 
+        # sequence's coordinates after the sequence finishes running. Therefore, we first make a copy of the sequence
+        # before it is modified by the pixel calculator and then replace the modified sequence at the end.
+        actions_copy = copy.deepcopy(self.actions)
+        
+        verbose_warning()
         pynput_keyboard = keyboard.Controller()
         
-        for idx, action in enumerate(self.actions):
+        # for idx, action in enumerate(self.__progress_bar(self.actions, f"Running: ", 40)):
             
-            # I don't ever know where to start explaining this.
-            # But some applications may have extra processes that popup (where the pop-up process has a different PID)
-            # When the new pop-up process get's clicked on, the pixel calculator will try to fetch the size of this process.
-            # However, if the previous action closed this pop-up process, the active/focused process takes a split second
-            # to switch back to the original process, and therefore the pixel calculator will try to fetch the already closed
-            # pop-up process' PID, causing an error.
-            time.sleep(FORCE_ACTIONS_DELAY)     
+        for idx, action in enumerate(self.actions):
             verbose_action(idx, action)
             
+            time.sleep(FORCE_ACTIONS_DELAY)
             time.sleep(action.delay)                            # Execute current action after standard action delay
             time.sleep(self.global_delay)                       # Execute current action after global delay
             
             safety_monitor.app_is_focused()                     # If the application is no longer focused, stop the automation
             
             # ====================================
             # ===========| KEYBOARD | ============
@@ -56,20 +91,23 @@
                 action.execute(pynput_keyboard)
                 
 
             # ==================================
             # ============| MOUSE | ============
             # ==================================
             elif isinstance(action, MouseAction):
-                # new_coord = pixel_calculator.calculate_new_coordinate(action.coordinate, action.window_info)
-                # if new_coord != None:
-                #     action.coordinate = new_coord
+                
+                if action.is_valid_for_pixel_calc == True:
+                    new_coord = PixelCalculator.transform_coordinate(action.coordinate, action.window_info)
+                    action.coordinate = new_coord
                 
                 action.execute()
             
+        # Reset the modified version of the sequence (modified by the pixel calculator)
+        self.actions = actions_copy
 
             
     def add(self, action: Action):
         assert(isinstance(action, Action))
         self.actions.append(action)
 
     def to_json(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `amiya-0.0.1/src/amiya/bin/focus_pid.exe` & `amiya-0.0.3/src/amiya/bin/focus_pid.exe`

 * *Files 3% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 00000010: b800 0000 0000 0000 4000 0000 0000 0000  ........@.......
 00000020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000030: 0000 0000 0000 0000 0000 0000 8000 0000  ................
 00000040: 0e1f ba0e 00b4 09cd 21b8 014c cd21 5468  ........!..L.!Th
 00000050: 6973 2070 726f 6772 616d 2063 616e 6e6f  is program canno
 00000060: 7420 6265 2072 756e 2069 6e20 444f 5320  t be run in DOS 
 00000070: 6d6f 6465 2e0d 0d0a 2400 0000 0000 0000  mode....$.......
-00000080: 5045 0000 4c01 0d00 a526 2b66 0074 0000  PE..L....&+f.t..
-00000090: e801 0000 e000 0701 0b01 021c 002e 0000  ................
+00000080: 5045 0000 4c01 0d00 5165 4266 0074 0000  PE..L...QeBf.t..
+00000090: f401 0000 e000 0701 0b01 021c 002e 0000  ................
 000000a0: 004a 0000 0002 0000 e012 0000 0010 0000  .J..............
 000000b0: 0040 0000 0000 4000 0010 0000 0002 0000  .@....@.........
 000000c0: 0400 0000 0100 0000 0400 0000 0000 0000  ................
-000000d0: 0010 0100 0004 0000 dfab 0000 0300 0000  ................
+000000d0: 0010 0100 0004 0000 2528 0100 0300 0000  ........%(......
 000000e0: 0000 2000 0010 0000 0000 1000 0010 0000  .. .............
 000000f0: 0000 0000 1000 0000 0000 0000 0000 0000  ................
-00000100: 0080 0000 5c06 0000 0000 0000 0000 0000  ....\...........
+00000100: 0080 0000 a806 0000 0000 0000 0000 0000  ................
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000140: 04a0 0000 1800 0000 0000 0000 0000 0000  ................
-00000150: 0000 0000 0000 0000 5081 0000 ec00 0000  ........P.......
+00000150: 0000 0000 0000 0000 5c81 0000 f800 0000  ........\.......
 00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000170: 0000 0000 0000 0000 2e74 6578 7400 0000  .........text...
-00000180: 542c 0000 0010 0000 002e 0000 0004 0000  T,..............
+00000180: a42c 0000 0010 0000 002e 0000 0004 0000  .,..............
 00000190: 0000 0000 0000 0000 0000 0000 6000 5060  ............`.P`
 000001a0: 2e64 6174 6100 0000 1c00 0000 0040 0000  .data........@..
 000001b0: 0002 0000 0032 0000 0000 0000 0000 0000  .....2..........
 000001c0: 0000 0000 4000 30c0 2e72 6461 7461 0000  ....@.0..rdata..
-000001d0: e402 0000 0050 0000 0004 0000 0034 0000  .....P.......4..
+000001d0: 0803 0000 0050 0000 0004 0000 0034 0000  .....P.......4..
 000001e0: 0000 0000 0000 0000 0000 0000 4000 3040  ............@.0@
 000001f0: 2f34 0000 0000 0000 d809 0000 0060 0000  /4...........`..
 00000200: 000a 0000 0038 0000 0000 0000 0000 0000  .....8..........
 00000210: 0000 0000 4000 3040 2e62 7373 0000 0000  ....@.0@.bss....
 00000220: 7000 0000 0070 0000 0000 0000 0000 0000  p....p..........
 00000230: 0000 0000 0000 0000 0000 0000 8000 30c0  ..............0.
-00000240: 2e69 6461 7461 0000 5c06 0000 0080 0000  .idata..\.......
+00000240: 2e69 6461 7461 0000 a806 0000 0080 0000  .idata..........
 00000250: 0008 0000 0042 0000 0000 0000 0000 0000  .....B..........
 00000260: 0000 0000 4000 30c0 2e43 5254 0000 0000  ....@.0..CRT....
 00000270: 1800 0000 0090 0000 0002 0000 004a 0000  .............J..
 00000280: 0000 0000 0000 0000 0000 0000 4000 30c0  ............@.0.
 00000290: 2e74 6c73 0000 0000 2000 0000 00a0 0000  .tls.... .......
 000002a0: 0002 0000 004c 0000 0000 0000 0000 0000  .....L..........
 000002b0: 0000 0000 4000 30c0 2f31 3400 0000 0000  ....@.0./14.....
@@ -61,725 +61,725 @@
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 83ec 1c8b 4424 208b 008b 003d 9100 00c0  ....D$ ....=....
 00000410: 774e 3d8d 0000 c073 603d 0500 00c0 0f85  wN=....s`=......
 00000420: cc00 0000 c744 2404 0000 0000 c704 240b  .....D$.......$.
-00000430: 0000 00e8 a02a 0000 83f8 010f 8448 0100  .....*.......H..
+00000430: 0000 00e8 d02a 0000 83f8 010f 8448 0100  .....*.......H..
 00000440: 0085 c00f 85e7 0000 008d b426 0000 0000  ...........&....
 00000450: 31c0 83c4 1cc2 0400 908d b426 0000 0000  1..........&....
 00000460: 3d94 0000 c074 493d 9600 00c0 0f84 8900  =....tI=........
 00000470: 0000 3d93 0000 c075 d7c7 4424 0400 0000  ..=....u..D$....
-00000480: 00c7 0424 0800 0000 e84b 2a00 0083 f801  ...$.....K*.....
+00000480: 00c7 0424 0800 0000 e87b 2a00 0083 f801  ...$.....{*.....
 00000490: 0f84 ad00 0000 85c0 74b6 c704 2408 0000  ........t...$...
 000004a0: 00ff d0b8 ffff ffff eba8 8db6 0000 0000  ................
 000004b0: c744 2404 0000 0000 c704 2408 0000 00e8  .D$.......$.....
-000004c0: 142a 0000 83f8 0175 cdc7 4424 0401 0000  .*.....u..D$....
-000004d0: 00c7 0424 0800 0000 e8fb 2900 00b8 ffff  ...$......).....
+000004c0: 442a 0000 83f8 0175 cdc7 4424 0401 0000  D*.....u..D$....
+000004d0: 00c7 0424 0800 0000 e82b 2a00 00b8 ffff  ...$.....+*.....
 000004e0: ffff e96b ffff ff89 f68d bc27 0000 0000  ...k.......'....
 000004f0: 3d1d 0000 c00f 8555 ffff ffc7 4424 0400  =......U....D$..
-00000500: 0000 00c7 0424 0400 0000 e8c9 2900 0083  .....$......)...
+00000500: 0000 00c7 0424 0400 0000 e8f9 2900 0083  .....$......)...
 00000510: f801 7459 85c0 0f84 34ff ffff c704 2404  ..tY....4.....$.
 00000520: 0000 00ff d0b8 ffff ffff e923 ffff ff90  ...........#....
 00000530: c704 240b 0000 00ff d0b8 ffff ffff e90f  ..$.............
 00000540: ffff ffc7 4424 0401 0000 00c7 0424 0800  ....D$.......$..
-00000550: 0000 e881 2900 00c7 0424 0000 0000 e86d  ....)....$.....m
+00000550: 0000 e8b1 2900 00c7 0424 0000 0000 e89d  ....)....$......
 00000560: 0f00 00b8 ffff ffff e9e5 feff ffc7 4424  ..............D$
-00000570: 0401 0000 00c7 0424 0400 0000 e857 2900  .......$.....W).
+00000570: 0401 0000 00c7 0424 0400 0000 e887 2900  .......$......).
 00000580: 0083 c8ff e9c9 feff ffc7 4424 0401 0000  ..........D$....
-00000590: 00c7 0424 0b00 0000 e83b 2900 0083 c8ff  ...$.....;).....
+00000590: 00c7 0424 0b00 0000 e86b 2900 0083 c8ff  ...$.....k).....
 000005a0: e9ad feff ff8d 7426 008d bc27 0000 0000  ......t&...'....
-000005b0: 5589 e553 83ec 14a1 7850 4000 85c0 741c  U..S....xP@...t.
+000005b0: 5589 e553 83ec 14a1 9c50 4000 85c0 741c  U..S.....P@...t.
 000005c0: c744 2408 0000 0000 c744 2404 0200 0000  .D$......D$.....
 000005d0: c704 2400 0000 00ff d083 ec0c c704 2400  ..$...........$.
-000005e0: 1040 00e8 c029 0000 83ec 04e8 d006 0000  .@...)..........
-000005f0: a108 4040 0089 0424 e8d3 0e00 00e8 1e03  ..@@...$........
-00000600: 0000 a120 7040 0085 c074 428b 1dcc 8140  ... p@...tB....@
+000005e0: 1040 00e8 082a 0000 83ec 04e8 0007 0000  .@...*..........
+000005f0: a108 4040 0089 0424 e803 0f00 00e8 4e03  ..@@...$......N.
+00000600: 0000 a120 7040 0085 c074 428b 1dd8 8140  ... p@...tB....@
 00000610: 00a3 0c40 4000 8944 2404 8b43 1089 0424  ...@@..D$..C...$
-00000620: e813 2900 00a1 2070 4000 8944 2404 8b43  ..)... p@..D$..C
-00000630: 3089 0424 e8ff 2800 00a1 2070 4000 8944  0..$..(... p@..D
-00000640: 2404 8b43 5089 0424 e8eb 2800 00e8 0e29  $..CP..$..(....)
-00000650: 0000 8b15 0c40 4000 8910 e871 0c00 0083  .....@@....q....
-00000660: e4f0 e8e9 0700 00e8 fc28 0000 8b00 8944  .........(.....D
+00000620: e84b 2900 00a1 2070 4000 8944 2404 8b43  .K)... p@..D$..C
+00000630: 3089 0424 e837 2900 00a1 2070 4000 8944  0..$.7)... p@..D
+00000640: 2404 8b43 5089 0424 e823 2900 00e8 4629  $..CP..$.#)...F)
+00000650: 0000 8b15 0c40 4000 8910 e8a1 0c00 0083  .....@@.........
+00000660: e4f0 e819 0800 00e8 3429 0000 8b00 8944  ........4).....D
 00000670: 2408 a100 7040 0089 4424 04a1 0470 4000  $...p@..D$...p@.
-00000680: 8904 24e8 1e02 0000 89c3 e8c9 2800 0089  ..$.........(...
-00000690: 1c24 e871 2900 0089 f68d bc27 0000 0000  .$.q)......'....
+00000680: 8904 24e8 5302 0000 89c3 e801 2900 0089  ..$.S.......)...
+00000690: 1c24 e8b9 2900 0089 f68d bc27 0000 0000  .$..)......'....
 000006a0: 83ec 3c8d 4424 2cc7 4424 0400 7040 00c7  ..<.D$,.D$..p@..
 000006b0: 0424 0470 4000 c744 242c 0000 0000 8944  .$.p@..D$,.....D
 000006c0: 2410 a104 4040 0083 e001 8944 240c 8d44  $...@@.....D$..D
-000006d0: 2428 8944 2408 e895 2800 0083 c43c c390  $(.D$...(....<..
-000006e0: 83ec 1cc7 0424 0100 0000 ff15 b881 4000  .....$........@.
+000006d0: 2428 8944 2408 e8cd 2800 0083 c43c c390  $(.D$...(....<..
+000006e0: 83ec 1cc7 0424 0100 0000 ff15 c481 4000  .....$........@.
 000006f0: e8bb feff ff8d 7426 008d bc27 0000 0000  ......t&...'....
-00000700: 83ec 1cc7 0424 0200 0000 ff15 b881 4000  .....$........@.
+00000700: 83ec 1cc7 0424 0200 0000 ff15 c481 4000  .....$........@.
 00000710: e89b feff ff8d 7426 008d bc27 0000 0000  ......t&...'....
-00000720: ff25 e481 4000 8d76 008d bc27 0000 0000  .%..@..v...'....
-00000730: ff25 d481 4000 9090 9090 9090 9090 9090  .%..@...........
+00000720: ff25 f081 4000 8d76 008d bc27 0000 0000  .%..@..v...'....
+00000730: ff25 e081 4000 9090 9090 9090 9090 9090  .%..@...........
 00000740: 5589 e556 5383 ec10 c704 2400 5040 00e8  U..VS.....$.P@..
-00000750: 7c28 0000 83ec 0485 c00f 84b1 0000 00c7  |(..............
-00000760: 0424 0050 4000 89c3 e843 2800 0083 ec04  .$.P@....C(.....
+00000750: c428 0000 83ec 0485 c00f 84b1 0000 00c7  .(..............
+00000760: 0424 0050 4000 89c3 e88b 2800 0083 ec04  .$.P@.....(.....
 00000770: a36c 7040 00c7 4424 0413 5040 0089 1c24  .lp@..D$..P@...$
-00000780: e843 2800 0083 ec08 89c6 c744 2404 2950  .C(........D$.)P
-00000790: 4000 891c 24e8 2e28 0000 83ec 08a3 0040  @...$..(.......@
+00000780: e88b 2800 0083 ec08 89c6 c744 2404 2950  ..(........D$.)P
+00000790: 4000 891c 24e8 7628 0000 83ec 08a3 0040  @...$.v(.......@
 000007a0: 4000 85f6 7411 c744 2404 0870 4000 c704  @...t..D$..p@...
 000007b0: 24b8 6040 00ff d6a1 1840 4000 85c0 743a  $.`@.....@@...t:
-000007c0: c704 2441 5040 00e8 0428 0000 83ec 0485  ..$AP@...(......
+000007c0: c704 2441 5040 00e8 4c28 0000 83ec 0485  ..$AP@..L(......
 000007d0: c0ba 0000 0000 7415 c744 2404 4f50 4000  ......t..D$.OP@.
-000007e0: 8904 24e8 e027 0000 83ec 0889 c285 d274  ..$..'.........t
+000007e0: 8904 24e8 2828 0000 83ec 0889 c285 d274  ..$.((.........t
 000007f0: 09c7 0424 1840 4000 ffd2 c704 2430 1440  ...$.@@.....$0.@
 00000800: 00e8 1aff ffff 8d65 f85b 5e5d c38d 7600  .......e.[^]..v.
 00000810: c705 0040 4000 0000 0000 be00 0000 00eb  ...@@...........
 00000820: 81eb 0d90 9090 9090 9090 9090 9090 9090  ................
 00000830: 5589 e583 ec18 a100 4040 0085 c074 09c7  U.......@@...t..
 00000840: 0424 b860 4000 ffd0 a16c 7040 0085 c074  .$.`@....lp@...t
-00000850: 0b89 0424 e88f 2700 0083 ec04 c9c3 9090  ...$..'.........
-00000860: 5589 e583 ec28 8d45 f089 4424 048b 4508  U....(.E..D$..E.
-00000870: 8904 24e8 0827 0000 83ec 088b 55f0 8b45  ..$..'......U..E
-00000880: 0c39 c275 188b 4508 8904 24e8 e826 0000  .9.u..E...$..&..
-00000890: 83ec 0489 45f4 b800 0000 00eb 05b8 0100  ....E...........
-000008a0: 0000 c9c2 0800 8d4c 2404 83e4 f0ff 71fc  .......L$.....q.
-000008b0: 5589 e553 5183 ec20 89cb e891 0500 0083  U..SQ.. ........
-000008c0: 3b02 741c 8b43 048b 0089 4424 04c7 0424  ;.t..C....D$...$
-000008d0: 6450 4000 e817 2600 00b8 0100 0000 eb2e  dP@...&.........
-000008e0: 8b43 0483 c004 8b00 8904 24e8 3826 0000  .C........$.8&..
-000008f0: 8945 f48b 45f4 8944 2404 c704 2460 1440  .E..E..D$...$`.@
-00000900: 00e8 8226 0000 83ec 08b8 0000 0000 8d65  ...&...........e
-00000910: f859 5b5d 8d61 fcc3 6690 6690 6690 6690  .Y[].a..f.f.f.f.
-00000920: 5589 e557 5653 83ec 4cf6 0504 4040 0002  U..WVS..L...@@..
-00000930: 0f84 ea02 0000 e8a5 2600 0089 65c4 8904  ........&...e...
-00000940: 2489 c6e8 8025 0000 8d44 0011 c1e8 04c1  $....%...D......
-00000950: e004 e849 0b00 0029 c4c7 45e4 0000 0000  ...I...)..E.....
-00000960: c745 d400 0000 008d 4424 10c7 45d0 0000  .E......D$..E...
-00000970: 0000 89c2 8945 cca1 0440 4000 2500 4400  .....E...@@.%.D.
-00000980: 0083 c810 8945 c831 c08d b426 0000 0000  .....E.1...&....
-00000990: 83c6 010f be4e ff85 c989 cb74 7380 fb3f  .....N.....ts..?
-000009a0: 0f84 8d01 0000 0f8f b400 0000 80fb 270f  ..............'.
-000009b0: 84b0 0100 0080 fb2a 0f84 7501 0000 80fb  .......*..u.....
-000009c0: 220f 8509 0100 0089 c1d1 f90f 84d9 0200  "...............
-000009d0: 0001 d183 c201 c642 ff5c 39ca 75f5 837d  .......B.\9.u..}
-000009e0: d427 0f84 c901 0000 a801 0f85 c101 0000  .'..............
-000009f0: 83c6 0189 ca83 75d4 220f be4e ff31 c0c7  ......u."..N.1..
-00000a00: 45d0 0100 0000 85c9 89cb 7591 8d74 2600  E.........u..t&.
-00000a10: 85c0 0f84 9902 0000 01d0 8db6 0000 0000  ................
-00000a20: 83c2 01c6 42ff 5c39 c275 f539 45cc 0f82  ....B.\9.u.9E...
-00000a30: be01 0000 8b55 d085 d20f 85b3 0100 008b  .....U..........
-00000a40: 45dc a304 7040 008b 45e0 a300 7040 008b  E...p@..E...p@..
-00000a50: 65c4 8d65 f45b 5e5f 5dc3 8db6 0000 0000  e..e.[^_].......
-00000a60: 80fb 5c0f 84ea 0000 0080 fb7f 0f84 c100  ..\.............
-00000a70: 0000 80fb 5b75 59f6 0504 4040 0020 0f85  ....[uY...@@. ..
-00000a80: af00 0000 85c0 8d78 ffb9 0100 0000 7432  .......x......t2
-00000a90: 8d7c 3a01 89d0 8d76 008d bc27 0000 0000  .|:....v...'....
-00000aa0: 83c0 01c6 40ff 5c39 f875 f584 c975 118d  ....@.\9.u...u..
-00000ab0: 5001 8818 31c0 e9d5 feff ff90 8d74 2600  P...1........t&.
-00000ac0: 89c2 8d42 01c6 027f ebe5 8db6 0000 0000  ...B............
-00000ad0: 85c0 8d3c 020f 84c8 0100 0090 8d74 2600  ...<.........t&.
-00000ae0: 83c2 01c6 42ff 5c39 fa75 f58b 45d4 85c0  ....B.\9.u..E...
-00000af0: 7535 a1ac 8140 0083 3801 0f84 c500 0000  u5...@..8.......
-00000b00: c744 2404 4000 0000 890c 2489 4dc0 e82d  .D$.@.....$.M..-
-00000b10: 2400 0085 c00f 85bb 0000 008b 4dc0 83f9  $...........M...
-00000b20: 090f 84af 0000 008d 5701 881f 31c0 e95d  ........W...1..]
-00000b30: feff ff85 c08d 78ff 0f84 4e01 0000 8b45  ......x...N....E
-00000b40: d483 f97f 0f94 c185 c00f 95c0 09c1 e93d  ...............=
-00000b50: ffff ff83 7dd4 270f 84e4 0000 0083 c001  ....}.'.........
-00000b60: e92b feff fff6 0504 4040 0010 0f84 5eff  .+......@@....^.
-00000b70: ffff 89c1 d1f9 0f84 3c01 0000 01d1 6690  ........<.....f.
-00000b80: 83c2 01c6 42ff 5c39 ca75 f583 7dd4 220f  ....B.\9.u..}.".
-00000b90: 8498 0000 00a8 010f 8590 0000 0083 75d4  ..............u.
-00000ba0: 2789 ca31 c0c7 45d0 0100 0000 e9df fdff  '..1..E.........
-00000bb0: ff8d 5101 c601 2231 c0c7 45d0 0100 0000  ..Q..."1..E.....
-00000bc0: e9cb fdff ffa1 d881 4000 8b00 f604 4840  ........@.....H@
-00000bd0: 0f84 48ff ffff 397d cc72 758b 45d0 85c0  ..H...9}.ru.E...
-00000be0: 756e 89fa 31c0 c745 d000 0000 00e9 9efd  un..1..E........
-00000bf0: ffff c600 008d 45d8 c744 2408 0000 0000  ......E..D$.....
-00000c00: 8944 240c 8b45 c889 4424 048b 45cc 8904  .D$..E..D$..E...
-00000c10: 24e8 5a18 0000 e924 feff ff90 8d74 2600  $.Z....$.....t&.
-00000c20: e87b faff ff8d 65f4 5b5e 5f5d c38d 5101  .{....e.[^_]..Q.
-00000c30: c601 2731 c0c7 45d0 0100 0000 e94f fdff  ..'1..E......O..
-00000c40: ffc6 025c 83c2 01e9 44fd ffff 8d74 2600  ...\....D....t&.
-00000c50: 8d45 d8c6 0700 c744 2408 0000 0000 8944  .E.....D$......D
-00000c60: 240c 8b5d c889 5c24 048b 7dcc 893c 24e8  $..]..\$..}..<$.
-00000c70: fc17 0000 89d8 89fa c745 d000 0000 0083  .........E......
-00000c80: c801 8945 c831 c0e9 04fd ffff 8b45 d485  ...E.1.......E..
-00000c90: c00f 95c0 83f9 7f0f 94c1 09c1 89d0 e908  ................
-00000ca0: feff ff89 d7e9 41fe ffff 89d1 e92d fdff  ......A......-..
-00000cb0: ff89 d0e9 73fd ffff 89d1 e9cc feff ff90  ....s...........
-00000cc0: 9c9c 5889 c235 0000 2000 509d 9c58 9d31  ..X..5.. .P..X.1
-00000cd0: d0a9 0000 2000 0f84 e900 0000 5331 c00f  .... .......S1..
-00000ce0: a285 c00f 84db 0000 00b8 0100 0000 0fa2  ................
-00000cf0: 31c0 f6c6 0174 0383 c801 f6c5 2074 050d  1....t...... t..
-00000d00: 8000 0000 f6c6 8074 0383 c802 f7c2 0000  .......t........
-00000d10: 8000 7403 83c8 04f7 c200 0000 0174 6d83  ..t..........tm.
-00000d20: c808 5589 e581 ec00 0200 0083 e4f0 0fae  ..U.............
-00000d30: 0424 8b9c 24c8 0000 0081 b424 c800 0000  .$..$......$....
-00000d40: dec0 1300 0fae 0c24 899c 24c8 0000 000f  .......$..$.....
-00000d50: ae04 2487 9c24 c800 0000 0fae 0c24 339c  ..$..$.......$3.
-00000d60: 24c8 0000 00c9 81fb dec0 1300 751e f7c2  $...........u...
-00000d70: 0000 0002 7403 83c8 10f7 c200 0000 0474  ....t..........t
-00000d80: 0383 c820 f6c1 0174 0383 c840 a324 7040  ... ...t...@.$p@
-00000d90: 00b8 0000 0080 0fa2 3d00 0000 8076 25b8  ........=....v%.
-00000da0: 0100 0080 0fa2 31c0 85d2 7905 b800 0100  ......1...y.....
-00000db0: 00f7 c200 0000 4074 050d 0002 0000 0905  ......@t........
-00000dc0: 2470 4000 5bf3 c390 9090 9090 9090 9090  $p@.[...........
-00000dd0: a110 4040 008b 0085 c074 1f83 ec0c 6690  ..@@.....t....f.
-00000de0: ffd0 a110 4040 008d 5004 8b40 0489 1510  ....@@..P..@....
-00000df0: 4040 0085 c075 e983 c40c f3c3 8d74 2600  @@...u.......t&.
-00000e00: 5383 ec18 8b1d 403c 4000 83fb ff74 2185  S.....@<@....t!.
-00000e10: db74 0cff 149d 403c 4000 83eb 0175 f4c7  .t....@<@....u..
-00000e20: 0424 d019 4000 e8f5 f8ff ff83 c418 5bc3  .$..@.........[.
-00000e30: 31db eb02 89c3 8d43 018b 1485 403c 4000  1......C....@<@.
-00000e40: 85d2 75f0 ebc9 8d76 008d bc27 0000 0000  ..u....v...'....
-00000e50: a128 7040 0085 c074 07f3 c390 8d74 2600  .(p@...t.....t&.
-00000e60: c705 2870 4000 0100 0000 eb94 9090 9090  ..(p@...........
-00000e70: 83ec 1c8b 4424 2483 f803 7414 85c0 7410  ....D$$...t...t.
-00000e80: b801 0000 0083 c41c c20c 0090 8d74 2600  .............t&.
-00000e90: 8b54 2428 8944 2404 8b44 2420 8954 2408  .T$(.D$..D$ .T$.
-00000ea0: 8904 24e8 4802 0000 b801 0000 0083 c41c  ..$.H...........
-00000eb0: c20c 008d b600 0000 008d bc27 0000 0000  ...........'....
-00000ec0: 5653 83ec 1483 3d64 7040 0002 8b44 2424  VS....=dp@...D$$
-00000ed0: 740a c705 6470 4000 0200 0000 83f8 0274  t...dp@........t
-00000ee0: 1283 f801 743f 83c4 14b8 0100 0000 5b5e  ....t?........[^
-00000ef0: c20c 00be 1490 4000 81ee 1490 4000 83fe  ......@.....@...
-00000f00: 037e e331 db8b 8314 9040 0085 c074 02ff  .~.1.....@...t..
-00000f10: d083 c304 39de 75ed 83c4 14b8 0100 0000  ....9.u.........
-00000f20: 5b5e c20c 008b 4424 28c7 4424 0401 0000  [^....D$(.D$....
-00000f30: 0089 4424 088b 4424 2089 0424 e8af 0100  ..D$..D$ ..$....
-00000f40: 00eb a38d b600 0000 008d bc27 0000 0000  ...........'....
-00000f50: 31c0 c390 9090 9090 9090 9090 9090 9090  1...............
-00000f60: 5653 83ec 14c7 0424 4470 4000 e89f 2000  VS.....$Dp@... .
-00000f70: 008b 1d3c 7040 0083 ec04 85db 742d 6690  ...<p@......t-f.
-00000f80: 8b03 8904 24e8 1620 0000 83ec 0489 c6e8  ....$.. ........
-00000f90: 4420 0000 85c0 750c 85f6 7408 8b43 0489  D ....u...t..C..
-00000fa0: 3424 ffd0 8b5b 0885 db75 d5c7 0424 4470  4$...[...u...$Dp
-00000fb0: 4000 e801 2000 0083 ec04 83c4 145b 5ec3  @... ........[^.
-00000fc0: 5653 31f6 83ec 14a1 4070 4000 85c0 7510  VS1.....@p@...u.
-00000fd0: 83c4 1489 f05b 5ec3 908d b426 0000 0000  .....[^....&....
-00000fe0: c744 2404 0c00 0000 c704 2401 0000 00e8  .D$.......$.....
-00000ff0: 2c1f 0000 85c0 89c3 7441 8b44 2420 c704  ,.......tA.D$ ..
-00001000: 2444 7040 0089 038b 4424 2489 4304 e8fd  $Dp@....D$$.C...
-00001010: 1f00 00a1 3c70 4000 83ec 0489 1d3c 7040  ....<p@......<p@
-00001020: 00c7 0424 4470 4000 8943 08e8 881f 0000  ...$Dp@..C......
-00001030: 83ec 0489 f083 c414 5b5e c3be ffff ffff  ........[^......
-00001040: eb8e 8db4 2600 0000 008d bc27 0000 0000  ....&......'....
-00001050: 5383 ec18 a140 7040 008b 5c24 2085 c075  S....@p@..\$ ..u
-00001060: 0f83 c418 31c0 5bc3 908d b426 0000 0000  ....1.[....&....
-00001070: c704 2444 7040 00e8 941f 0000 8b15 3c70  ..$Dp@........<p
-00001080: 4000 83ec 0485 d274 178b 0239 c375 0aeb  @......t...9.u..
-00001090: 4e8b 0839 d974 2989 c28b 4208 85c0 75f1  N..9.t)...B...u.
-000010a0: c704 2444 7040 00e8 0c1f 0000 83ec 0483  ..$Dp@..........
-000010b0: c418 31c0 5bc3 8d76 008d bc27 0000 0000  ..1.[..v...'....
-000010c0: 8b48 0889 4a08 8904 24e8 4a1e 0000 c704  .H..J...$.J.....
-000010d0: 2444 7040 00e8 de1e 0000 83ec 04eb d08b  $Dp@............
-000010e0: 4208 a33c 7040 0089 d0eb db90 8d74 2600  B..<p@.......t&.
-000010f0: 83ec 1c8b 4424 2483 f801 7447 7217 83f8  ....D$$...tGr...
-00001100: 0375 09a1 4070 4000 85c0 7565 b801 0000  .u..@p@...ue....
-00001110: 0083 c41c c3a1 4070 4000 85c0 7562 a140  ......@p@...ub.@
-00001120: 7040 0083 f801 75e4 c704 2444 7040 00c7  p@....u...$Dp@..
-00001130: 0540 7040 0000 0000 00e8 da1e 0000 83ec  .@p@............
-00001140: 04eb c9a1 4070 4000 85c0 7414 c705 4070  ....@p@...t...@p
-00001150: 4000 0100 0000 b801 0000 0083 c41c c390  @...............
-00001160: c704 2444 7040 00e8 541e 0000 83ec 04eb  ..$Dp@..T.......
-00001170: dbe8 eafd ffff eb94 908d b426 0000 0000  ...........&....
-00001180: e8db fdff ffeb 9790 9090 9090 9090 9090  ................
-00001190: 5653 83ec 14a1 cc81 4000 c744 2408 1700  VS......@..D$...
-000011a0: 0000 c744 2404 0100 0000 8d74 2424 c704  ...D$......t$$..
-000011b0: 247c 5040 008d 5840 895c 240c e84f 1d00  $|P@..X@.\$..O..
-000011c0: 008b 4424 2089 7424 0889 1c24 8944 2404  ..D$ .t$...$.D$.
-000011d0: e8e3 1c00 00e8 561d 0000 8db6 0000 0000  ......V.........
-000011e0: 5557 89cf 5653 89c3 89d6 83ec 4c8d 4424  UW..VS......L.D$
-000011f0: 24c7 4424 081c 0000 0089 1c24 8944 2404  $.D$.......$.D$.
-00001200: e88b 1d00 0083 ec0c 85c0 0f84 a800 0000  ................
-00001210: 8b44 2438 83f8 4074 0583 f804 7522 897c  .D$8..@t....u".|
-00001220: 2408 8974 2404 891c 24e8 ca1c 0000 83c4  $..t$...$.......
-00001230: 4c5b 5e5f 5dc3 8d76 008d bc27 0000 0000  L[^_]..v...'....
-00001240: 8b44 2430 8d6c 2420 c744 2408 4000 0000  .D$0.l$ .D$.@...
-00001250: 896c 240c 8944 2404 8b44 2424 8904 24e8  .l$..D$..D$$..$.
-00001260: 341d 0000 83ec 108b 5424 3889 7c24 0889  4.......T$8.|$..
-00001270: 7424 0489 1c24 8954 241c e879 1c00 008b  t$...$.T$..y....
-00001280: 5424 1c83 fa40 74a6 83fa 0474 a18b 4424  T$...@t....t..D$
-00001290: 2089 6c24 0c89 4424 088b 4424 3089 4424   .l$..D$..D$0.D$
-000012a0: 048b 4424 2489 0424 e8eb 1c00 0083 ec10  ..D$$..$........
-000012b0: 83c4 4c5b 5e5f 5dc3 895c 2408 c744 2404  ..L[^_]..\$..D$.
-000012c0: 1c00 0000 c704 2494 5040 00e8 c0fe ffff  ......$.P@......
-000012d0: a15c 7040 0085 c074 07c3 8db6 0000 0000  .\p@...t........
-000012e0: b8e4 5240 00c7 055c 7040 0001 0000 002d  ..R@...\p@.....-
-000012f0: e452 4000 83f8 077e e057 5653 83ec 2083  .R@....~.WVS.. .
-00001300: f80b 0f8e e800 0000 8b35 e452 4000 85f6  .........5.R@...
-00001310: 0f85 8f00 0000 8b1d e852 4000 85db 0f85  .........R@.....
-00001320: 8100 0000 8b0d ec52 4000 bbf0 5240 0085  .......R@...R@..
-00001330: c90f 84be 0000 00bb e452 4000 8b43 0883  .........R@..C..
-00001340: f801 0f85 4301 0000 83c3 0c81 fbe4 5240  ....C.........R@
-00001350: 000f 8389 0000 008b 138b 7b04 8db2 0000  ..........{.....
-00001360: 4000 8b8a 0000 4000 0fb6 5308 8d87 0000  @.....@...S.....
-00001370: 4000 83fa 100f 8495 0000 0083 fa20 0f84  @............ ..
-00001380: ec00 0000 83fa 080f 84b3 0000 0089 5424  ..............T$
-00001390: 04c7 0424 fc50 4000 c744 241c 0000 0000  ...$.P@..D$.....
-000013a0: e8eb fdff ffbb e452 4000 81fb e452 4000  .......R@....R@.
-000013b0: 732e 8b4b 048b 1383 c308 0391 0000 4000  s..K..........@.
-000013c0: 8d81 0000 4000 b904 0000 0089 5424 1c8d  ....@.......T$..
-000013d0: 5424 1ce8 08fe ffff 81fb e452 4000 72d2  T$.........R@.r.
-000013e0: 83c4 205b 5e5f c389 f68d bc27 0000 0000  .. [^_.....'....
-000013f0: bbe4 5240 008b 1385 d275 af8b 4304 85c0  ..R@.....u..C...
-00001400: 0f84 36ff ffff eba2 908d b426 0000 0000  ..6........&....
-00001410: 0fb7 9700 0040 0066 85d2 7906 81ca 0000  .....@.f..y.....
-00001420: ffff 29f2 01d1 8d54 241c 894c 241c b902  ..)....T$..L$...
-00001430: 0000 00e8 a8fd ffff e90b ffff ff8d 7600  ..............v.
-00001440: 0fb6 3889 fa84 d279 0681 cf00 ffff ff29  ..8....y.......)
-00001450: f78d 5424 1c01 f989 4c24 1cb9 0100 0000  ..T$....L$......
-00001460: e87b fdff ffe9 defe ffff 8db6 0000 0000  .{..............
-00001470: 29f1 0308 8d54 241c 894c 241c b904 0000  )....T$..L$.....
-00001480: 00e8 5afd ffff e9bd feff ff89 4424 04c7  ..Z.........D$..
-00001490: 0424 c850 4000 e8f5 fcff ff90 9090 9090  .$.P@...........
-000014a0: 5150 3d00 1000 008d 4c24 0c72 1581 e900  QP=.....L$.r....
-000014b0: 1000 0083 0900 2d00 1000 003d 0010 0000  ......-....=....
-000014c0: 77eb 29c1 8309 0058 59c3 9090 6690 6690  w.)....XY...f.f.
-000014d0: 83ec 1c8b 4424 20c7 4424 0c80 1f00 0083  ....D$ .D$......
-000014e0: f8fd 7431 83f8 fc74 3a85 c074 4883 f8ff  ..t1...t:..tH...
-000014f0: 742d 83f8 fe74 36d9 200f b740 1c89 4424  t-...t6. ..@..D$
-00001500: 0cf6 0524 7040 0010 7405 0fae 5424 0c31  ...$p@..t...T$.1
-00001510: c083 c41c c3c7 0514 4040 00ff ffff ffdb  ........@@......
-00001520: e3eb dec7 0514 4040 00fe ffff ffff 15c4  ......@@........
-00001530: 8140 00eb cca1 1440 4000 ebb1 9090 9090  .@.....@@.......
-00001540: 85c0 0f84 8200 0000 5653 89d3 c1eb 0531  ........VS.....1
-00001550: c983 f301 83e3 0189 f68d bc27 0000 0000  ...........'....
-00001560: 0fbe 1085 d274 2984 db74 0583 fa7f 7440  .....t)..t....t@
-00001570: 83c0 0185 c975 1e83 fa2a 7444 83fa 3f74  .....u...*tD..?t
-00001580: 3f31 c983 fa5b 0fbe 100f 94c1 85d2 75d7  ?1...[........u.
-00001590: 89d0 5b5e c383 f901 7e05 83fa 5d74 2183  ..[^....~...]t!.
-000015a0: fa21 0f95 c20f b6d2 01d1 ebb4 8d74 2600  .!...........t&.
-000015b0: 8078 0100 8d70 0274 1689 f0eb b68d 7600  .x...p.t......v.
-000015c0: ba01 0000 0089 d05b 5ec3 31d2 89d0 c331  .......[^.1....1
-000015d0: d2eb bd8d b600 0000 008d bc27 0000 0000  ...........'....
-000015e0: 85c0 745c 5653 89c6 83ec 148b 400c 8d58  ..t\VS......@..X
-000015f0: 018d 049d 0000 0000 8904 24e8 0819 0000  ..........$.....
-00001600: 89c1 8946 08b8 0300 0000 85c9 7422 85db  ...F........t"..
-00001610: 89da c746 0400 0000 007e 1390 8d74 2600  ...F.....~...t&.
-00001620: 83ea 0185 d2c7 0491 0000 0000 75f2 31c0  ............u.1.
-00001630: 83c4 145b 5ec3 8d76 008d bc27 0000 0000  ...[^..v...'....
-00001640: 31c0 c38d b600 0000 008d bc27 0000 0000  1..........'....
-00001650: 5557 89c7 5653 83ec 3c0f be18 8954 241c  UW..VS..<....T$.
-00001660: 894c 2420 83fb 5d89 dd0f 8461 0100 0083  .L$ ..]....a....
-00001670: fb2d 0f84 5801 0000 8b4c 241c 89c8 f7d0  .-..X....L$.....
-00001680: 8944 2428 b801 0000 0029 c889 4424 2ceb  .D$(.....)..D$,.
-00001690: 0d89 ee2b 7424 1c85 f674 680f beda 83fb  ...+t$...th.....
-000016a0: 5d8d 7701 0f84 1a01 0000 83fb 2d0f 848d  ].w.........-...
-000016b0: 0000 0085 db0f 8409 0100 0083 fb2f 0f84  ............./..
-000016c0: 0001 0000 83fb 5c0f 84f7 0000 000f b616  ......\.........
-000016d0: 89dd 89f7 f744 2420 0040 0000 75b3 892c  .....D$ .@..u..,
-000016e0: 2488 5424 24e8 d617 0000 89c6 8b44 241c  $.T$$........D$.
-000016f0: 8904 24e8 c817 0000 29c6 0fb6 5424 2485  ..$.....)...T$$.
-00001700: f675 988b 4424 2083 e020 eb12 8d74 2600  .u..D$ .. ...t&.
-00001710: 83c7 0184 d20f 84a9 0000 000f b617 80fa  ................
-00001720: 5d0f 843e 0100 0080 fa7f 75e4 85c0 0f85  ]..>......u.....
-00001730: 3c01 0000 0fb6 5701 83c7 01eb d38d 7600  <.....W.......v.
-00001740: 0fb6 5701 80fa 5d0f 8495 0000 000f beda  ..W...].........
-00001750: 85db 7470 8b4c 2420 8d77 0281 e100 4000  ..tp.L$ .w....@.
-00001760: 0039 dd0f 8d0f 0100 0089 7424 2489 e889  .9........t$$...
-00001770: ceeb 118b 4424 288d 3c28 85ff 7429 39eb  ....D$(.<(..t)9.
-00001780: 89e8 746c 85f6 8d68 0175 e889 0424 e82d  ..tl...h.u...$.-
-00001790: 1700 0089 c78b 4424 1c89 0424 e81f 1700  ......D$...$....
-000017a0: 0029 c785 ff75 d78b 5424 208b 7424 2483  .)...u..T$ .t$$.
-000017b0: e220 0fb6 063c 5d74 613c 7f74 4383 c601  . ...<]ta<.tC...
-000017c0: 84c0 75ee 83c4 3c31 c05b 5e5f 5dc3 6690  ..u...<1.[^_].f.
-000017d0: 3b5c 241c 744f 0fbe 5f01 83c7 01e9 96fe  ;\$.tO.._.......
-000017e0: ffff bd2d 0000 0089 f7e9 e6fe ffff 6690  ...-..........f.
-000017f0: 8b74 2424 e9c2 feff ff8d b426 0000 0000  .t$$.......&....
-00001800: 85d2 750c 0fb6 4601 83c6 01eb b08d 7600  ..u...F.......v.
-00001810: 83c6 010f b606 3c5d 759f 83c4 3c8d 4601  ......<]u...<.F.
-00001820: 5b5e 5f5d c38b 5424 2083 c701 83e2 2090  [^_]..T$ ..... .
-00001830: 0fb6 073c 5d74 2e3c 7f74 1583 c701 84c0  ...<]t.<.t......
-00001840: 75ee e97d ffff ff89 f68d bc27 0000 0000  u..}.......'....
-00001850: 85d2 750c 0fb6 4701 83c7 01eb de8d 7600  ..u...G.......v.
-00001860: 83c7 01eb cb83 c43c 8d47 015b 5e5f 5dc3  .......<.G.[^_].
-00001870: 83c7 01e9 a3fe ffff 0f8e 3dfe ffff 8974  ..........=....t
-00001880: 2424 89ce eb1f 8d76 008d bc27 0000 0000  $$.....v...'....
-00001890: 8b44 242c 8d2c 3885 ed74 2d39 fb89 fd0f  .D$,.,8..t-9....
-000018a0: 844b ffff ff85 f68d 7dff 75e4 892c 24e8  .K......}.u..,$.
-000018b0: 0c16 0000 89c5 8b44 241c 8904 24e8 fe15  .......D$...$...
-000018c0: 0000 29c5 85ed 75d3 8b54 2420 8b74 2424  ..)...u..T$ .t$$
-000018d0: 83e2 200f b606 3c5d 0f84 3cff ffff 3c7f  .. ...<]..<...<.
-000018e0: 740e 83c6 0184 c075 eae9 d6fe ffff 6690  t......u......f.
-000018f0: 85d2 750c 0fb6 4601 83c6 01eb e58d 7600  ..u...F.......v.
-00001900: 83c6 01eb ce8d 7426 008d bc27 0000 0000  ......t&...'....
-00001910: 5557 89c5 5653 83ec 2c80 3a2e 894c 2414  UW..VS..,.:..L$.
-00001920: 0fb6 080f 8437 0100 008b 4424 148d 7a01  .....7....D$..z.
-00001930: c1e8 0583 f001 8944 2418 0fbe d18d 77ff  .......D$.....w.
-00001940: 8d45 0185 d20f 8469 0100 0080 f93f 0f84  .E.....i.....?..
-00001950: ed00 0000 80f9 5b0f 84b3 0000 0080 f92a  ......[........*
-00001960: 745e f644 2418 0174 0983 fa7f 0f84 2e01  t^.D$..t........
-00001970: 0000 89c5 0fbe 5fff 84db 0f84 8601 0000  ......_.........
-00001980: f744 2414 0040 0000 0f85 c200 0000 8914  .D$..@..........
-00001990: 2489 5424 1ce8 2615 0000 891c 2489 c6e8  $.T$..&.....$...
-000019a0: 1c15 0000 8b54 241c 29c6 85f6 0f84 8300  .....T$.).......
-000019b0: 0000 89d0 29d8 83c4 2c5b 5e5f 5dc3 6690  ....)...,[^_].f.
-000019c0: 0fb6 5501 89c3 80fa 2a75 1090 8d74 2600  ..U.....*u...t&.
-000019d0: 83c3 010f b613 80fa 2a74 f531 c084 d274  ........*t.1...t
-000019e0: d58b 7c24 1481 cf00 0001 00eb 0c8d 7600  ..|$..........v.
-000019f0: 83c6 0180 7eff 0074 bd89 f989 f289 d8e8  ....~..t........
-00001a00: 0cff ffff 85c0 75e8 83c4 2c5b 5e5f 5dc3  ......u...,[^_].
-00001a10: 0fbe 57ff 85d2 0f84 fb00 0000 807d 0121  ..W..........}.!
-00001a20: 7460 8b4c 2414 e825 fcff ff89 c585 ed0f  t`.L$..%........
-00001a30: 84c7 0000 000f b64d 0083 c701 e9f9 feff  .......M........
-00001a40: ff80 7fff 000f 84c2 0000 0089 c5eb e690  ................
-00001a50: 89d6 29de e951 ffff ff8d b426 0000 0000  ..)..Q.....&....
-00001a60: 80f9 2e0f 84c0 feff ff0f bec1 83e8 2ef7  ................
-00001a70: 4424 1400 0001 000f 85ac feff ffe9 34ff  D$............4.
-00001a80: ffff 8d5d 028b 4c24 1489 d8e8 c0fb ffff  ...]..L$........
-00001a90: 85c0 742a 89dd eb95 908d b426 0000 0000  ..t*.......&....
-00001aa0: 0fbe 5501 83c5 0285 d20f 85c5 feff ffe9  ..U.............
-00001ab0: befe ffff 0fbe 06f7 d8e9 f8fe ffff 0fb6  ................
-00001ac0: 4502 3c5d 745b 8b54 2414 83e2 20eb 0b90  E.<]t[.T$... ...
-00001ad0: 83c3 0184 c074 250f b603 3c5d 7416 3c7f  .....t%...<]t.<.
-00001ae0: 75ee 85d2 7509 0fb6 4301 83c3 01eb e183  u...u...C.......
-00001af0: c301 ebe3 8d6b 01e9 31ff ffff b85d 0000  .....k..1....]..
-00001b00: 00e9 b0fe ffff 31db e9a5 feff ffb8 3f00  ......1.......?.
-00001b10: 0000 e99f feff ffb8 5b00 0000 e995 feff  ........[.......
-00001b20: ff8d 5d03 0fb6 4503 eb9c 8db6 0000 0000  ..]...E.........
-00001b30: 5756 89c6 5389 d383 ec10 8b42 0c03 4204  WV..S......B..B.
-00001b40: 8d04 8508 0000 0089 4424 048b 4208 8904  ........D$..B...
-00001b50: 24e8 9213 0000 85c0 7426 8b4b 048b 530c  $.......t&.K..S.
-00001b60: 8943 088d 7901 01d1 01fa 897b 0489 3488  .C..y......{..4.
-00001b70: c704 9000 0000 0083 c410 31c0 5b5e 5fc3  ..........1.[^_.
-00001b80: 83c4 10b8 0100 0000 5b5e 5fc3 8d74 2600  ........[^_..t&.
-00001b90: 5653 89c3 89d6 83ec 148b 0085 c074 05e8  VS...........t..
-00001ba0: ecff ffff 8b43 0885 c074 0485 f675 218b  .....C...t...u!.
-00001bb0: 4304 85c0 7407 89f2 e8d3 ffff ff89 1c24  C...t..........$
-00001bc0: e853 1300 0083 c414 5b5e c390 8d74 2600  .S......[^...t&.
-00001bd0: 89f2 e859 ffff ffeb d68d b426 0000 0000  ...Y.......&....
-00001be0: 5589 e557 5653 89c3 83ec 6c89 55d0 80e6  U..WVS....l.U...
-00001bf0: 0489 4dc4 0f85 5603 0000 8965 a889 1c24  ..M...V....e...$
-00001c00: e8c3 1200 008d 5001 83c0 10c1 e804 c1e0  ......P.........
-00001c10: 04e8 8af8 ffff 29c4 8d44 240c 8954 2408  ......)..D$..T$.
-00001c20: 895c 2404 8904 24e8 cc12 0000 8904 24e8  .\$...$.......$.
-00001c30: 8c09 0000 8945 d489 c68d 45d8 c745 e400  .....E....E..E..
-00001c40: 0000 00e8 98f9 ffff 85c0 8945 cc0f 85ed  ...........E....
-00001c50: 0200 008b 7dd0 89f0 89fa e8e1 f8ff ff85  ....}...........
-00001c60: c00f 84d7 0400 008d 45d8 89fa 80ce 8089  ........E.......
-00001c70: 0424 8b4d c489 f0e8 64ff ffff 8945 cc8b  .$.M....d....E..
-00001c80: 4dcc 85c9 0f85 b602 0000 0fb6 4301 3c2f  M...........C.</
-00001c90: 7419 3c5c 7415 8b75 d4bf 2851 4000 b902  t.<\t..u..(Q@...
-00001ca0: 0000 00f3 a60f 840b 0500 008b 45d4 8904  ............E...
-00001cb0: 24e8 1212 0000 01d8 39c3 0f83 6607 0000  $.......9...f...
-00001cc0: 0fb6 0880 f92f 884d a30f 844f 0700 0080  ...../.M...O....
-00001cd0: f95c 7524 e945 0700 008d b426 0000 0000  .\u$.E.....&....
-00001ce0: 0fb6 48ff 89d0 80f9 2f0f 846b 0600 0080  ..H...../..k....
-00001cf0: f95c 0f84 6206 0000 8d50 ff39 d375 e10f  .\..b....P.9.u..
-00001d00: b640 ff89 55c8 8845 a30f b645 a33c 2f74  .@..U..E...E.</t
-00001d10: 083c 5c0f 8572 0600 008b 55c8 0fb6 75a3  .<\..r....U...u.
-00001d20: eb02 89c6 83c2 010f b602 3c2f 0f94 c33c  ..........</...<
-00001d30: 5c0f 94c1 08cb 75ea 89f0 8955 c888 45a3  \.....u....U..E.
-00001d40: 8b45 d489 45a4 8b45 e08b 7dd0 c745 cc02  .E..E..E..}..E..
-00001d50: 0000 0089 45bc 8b00 81e7 0080 0000 897d  ....E..........}
-00001d60: d485 c00f 8411 0500 0089 0424 e8cf 0d00  ...........$....
-00001d70: 0085 c089 c70f 84b8 0400 008b 45a4 85c0  ............E...
-00001d80: 0f84 7405 0000 8b45 bc8b 0089 0424 e835  ..t....E.....$.5
-00001d90: 1100 0089 45c0 8b45 c0c7 45b8 0000 0000  ....E..E..E.....
-00001da0: 83c0 0289 45ac 8d76 008d bc27 0000 0000  ....E..v...'....
-00001db0: 893c 24e8 480f 0000 85c0 89c6 0f84 1104  .<$.H...........
-00001dc0: 0000 8b45 d485 c074 0683 7e08 1075 e18d  ...E...t..~..u..
-00001dd0: 5e0c 8b4d d08b 45c8 89da e831 fbff ff85  ^..M..E....1....
-00001de0: c075 cd0f b756 068b 45ac 8965 b08d 4402  .u...V..E..e..D.
-00001df0: 0fc1 e804 c1e0 04e8 a4f6 ffff 29c4 8b45  ............)..E
-00001e00: c0c7 45b4 0000 0000 8d74 240c 85c0 0f85  ..E......t$.....
-00001e10: 7c04 0000 8b45 b483 c201 895c 2404 8954  |....E.....\$..T
-00001e20: 2408 89e3 01f0 8904 24e8 ca10 0000 8934  $.......$......4
-00001e30: 24e8 9210 0000 83c0 10c1 e804 c1e0 04e8  $...............
-00001e40: 5cf6 ffff 29c4 89f0 8d4c 240c 89ce eb0d  \...)....L$.....
-00001e50: 83c6 0183 c001 84d2 8856 ff74 1c0f b610  .........V.t....
-00001e60: 80fa 7f75 eb0f b650 0183 c001 83c6 0183  ...u...P........
-00001e70: c001 84d2 8856 ff75 e489 0c24 e8a7 1100  .....V.u...$....
-00001e80: 0085 c089 c689 dc0f 8447 0400 008b 5dcc  .........G....].
-00001e90: 83fb 020f 94c0 0fb6 c083 e801 21c3 8b45  ............!..E
-00001ea0: d089 5dcc a840 0f85 7403 0000 8b5d b885  ..]..@..t....]..
-00001eb0: db0f 84ae 0400 0025 0040 0000 897d b489  .......%.@...}..
-00001ec0: c7eb 14e8 0810 0000 85c0 8b13 8b4b 047e  .............K.~
-00001ed0: 2285 c974 2489 cb8b 4308 85ff 8934 2489  "..t$...C....4$.
-00001ee0: 4424 0475 dee8 3611 0000 85c0 8b13 8b4b  D$.u..6........K
-00001ef0: 047f de89 d185 c975 dc8b 7db4 8945 b4c7  .......u..}..E..
-00001f00: 0424 0c00 0000 e8fd 0f00 0085 c00f 8418  .$..............
-00001f10: 0300 008b 55b4 8970 08c7 4004 0000 0000  ....U..p..@.....
-00001f20: c700 0000 0000 85d2 0f8e d803 0000 8943  ...............C
-00001f30: 04e9 f502 0000 c745 cc01 0000 008d 7600  .......E......v.
-00001f40: 8b65 a88b 45cc 8d65 f45b 5e5f 5dc3 6690  .e..E..e.[^_].f.
-00001f50: 8965 c089 0424 e86d 0f00 0083 c010 c1e8  .e...$.m........
-00001f60: 04c1 e004 e837 f5ff ff29 c489 de8d 4424  .....7...)....D$
-00001f70: 0c89 c789 45c8 0fb6 033c 7f74 283c 7b74  ....E....<.t(<{t
-00001f80: 3f84 c08d 5701 8d4e 0188 070f 84bc 0400  ?...W..N........
-00001f90: 003c 7b0f 84b4 0400 000f b646 0189 d789  .<{........F....
-00001fa0: ce3c 7f75 d80f b646 01c6 077f 84c0 0f85  .<.u...F........
-00001fb0: ac00 0000 83c7 0183 c601 ebc5 8d74 2600  .............t&.
-00001fc0: 897d cc89 f78b 55cc b901 0000 000f b647  .}....U........G
-00001fd0: 013c 7f74 2683 c701 3c7d 7409 3c2c 7540  .<.t&...<}t.<,u@
-00001fe0: 83f9 0175 3b83 e901 0f84 8300 0000 8802  ...u;...........
-00001ff0: 0fb6 4701 83c2 013c 7f75 da0f b647 02c6  ..G....<.u...G..
-00002000: 027f 8d5a 0284 c088 4201 7534 c642 0200  ...Z....B.u4.B..
-00002010: c745 cc01 0000 00e9 0e01 0000 8d74 2600  .E...........t&.
-00002020: 3c7b 742c 84c0 0f95 45d4 0fb6 5dd4 84db  <{t,....E...]...
-00002030: 8d72 0188 020f 84f9 0300 0089 f2eb 8e90  .r..............
-00002040: 0fb6 4703 89da 83c7 03eb 8d90 8d74 2600  ..G..........t&.
-00002050: 83c1 01bb 0100 0000 c645 d401 ebd0 6690  .........E....f.
-00002060: 8847 0183 c602 0fb6 0683 c702 e908 ffff  .G..............
-00002070: ff3c 2c0f 85c1 0000 0089 f8be 0100 0000  .<,.............
-00002080: 0fb6 5801 8d48 0180 fb7f 0f85 1f01 0000  ..X..H..........
-00002090: 8078 0200 7512 e985 0000 0090 8d74 2600  .x..u........t&.
-000020a0: 8078 0100 747a 89c1 0fb6 5902 8d41 0280  .x..tz....Y..A..
-000020b0: fb7f 74ec 80fb 7b74 7980 fb7d 7555 83ee  ..t...{ty..}uU..
-000020c0: 0175 bd8d 4801 0fb6 4001 eb07 8d74 2600  .u..H...@....t&.
-000020d0: 0fb6 0183 c201 83c1 0184 c088 42ff 75f0  ............B.u.
-000020e0: 8b45 0889 0424 8b75 d08b 4dc4 8b45 c889  .E...$.u..M..E..
-000020f0: f283 ce01 e8e7 faff ff83 f801 8975 d00f  .............u..
-00002100: 840b ffff ff80 3f2c 0f84 b7fe ffff 8945  ......?,.......E
-00002110: cceb 1784 db0f 8565 ffff ff90 8d74 2600  .......e.....t&.
-00002120: c602 00c7 45cc 0100 0000 8b65 c0e9 11fe  ....E......e....
-00002130: ffff 83c6 01e9 46ff ffff 89f8 eb85 8b45  ......F........E
-00002140: d489 e689 0424 e87d 0d00 0083 c010 c1e8  .....$.}........
-00002150: 04c1 e004 e847 f3ff ff8b 55d4 29c4 8d7c  .....G....U.)..|
-00002160: 240c 89f9 eb17 8d76 008d bc27 0000 0000  $......v...'....
-00002170: 83c1 0183 c201 84c0 8841 ff74 100f b602  .........A.t....
-00002180: 3c7f 75ec 0fb6 4201 83c2 01eb e389 3c24  <.u...B.......<$
-00002190: e893 0e00 0085 c089 f40f 8497 fdff ff8d  ................
-000021a0: 55d8 e889 f9ff ff89 45cc e9d0 faff ff89  U.......E.......
-000021b0: c8e9 fefe ffff f645 d010 0f85 da01 0000  .......E........
-000021c0: 895d c8c6 45a3 5cc7 45a4 0000 0000 e973  .]..E.\.E......s
-000021d0: fbff ff89 3c24 e875 0b00 008b 55b8 85d2  ....<$.u....U...
-000021e0: 740b 8b55 088b 45b8 e8a3 f9ff ff8b 7dbc  t..U..E.......}.
-000021f0: 8d5f 048b 43fc 8904 24e8 1a0d 0000 8b47  ._..C...$......G
-00002200: 0485 c00f 8412 0100 0083 7dcc 0174 4789  ..........}..tG.
-00002210: 5dbc e952 fbff ff89 f68d bc27 0000 0000  ]..R.......'....
-00002220: 8b4d 0885 c90f 85c0 0000 008b 65b0 e97d  .M..........e..}
-00002230: fbff fff6 45d0 040f 84e9 0000 008b 7dbc  ....E.........}.
-00002240: 8d5f 0489 f88b 0089 0424 e8c9 0c00 008b  ._.......$......
-00002250: 4704 85c0 7417 8b45 bc8b 4004 83c3 0489  G...t..E..@.....
-00002260: 0424 e8b1 0c00 008b 0385 c075 ef8b 45e0  .$.........u..E.
-00002270: c745 cc01 0000 0089 45bc 8b45 bc89 0424  .E......E..E...$
-00002280: e893 0c00 008b 65a8 e9b6 fcff ff8d 7600  ......e.......v.
-00002290: 8b45 bc89 55b4 8b55 c08b 0089 3424 8954  .E..U..U....4$.T
-000022a0: 2408 8944 2404 e84d 0c00 008b 4dc0 8b55  $..D$..M....M..U
-000022b0: b40f b644 0c0b 3c2f 7426 3c5c 7422 89c8  ...D..</t&<\t"..
-000022c0: 83c0 0189 45b4 89c8 0fb6 4da3 880c 06e9  ....E.....M.....
-000022d0: 40fb ffff c745 cc03 0000 00e9 4bff ffff  @....E......K...
-000022e0: 8b45 c089 45b4 e929 fbff ff8b 5508 89f0  .E..E..)....U...
-000022f0: e83b f8ff ffe9 31ff ffff c745 c000 0000  .;....1....E....
-00002300: 00e9 90fa ffff 8903 8b5d b885 db0f 8518  .........]......
-00002310: ffff ff89 45b8 e910 ffff ff8b 45e0 8945  ....E.......E..E
-00002320: bce9 54ff ffff 8b7d c485 ff0f 84bc feff  ..T....}........
-00002330: ffe8 1a0c 0000 8b00 8944 2404 8b75 bc8b  .........D$..u..
-00002340: 0689 0424 ffd7 85c0 0f84 9ffe ffff 89f0  ...$............
-00002350: 8d5e 0489 f7e9 ebfe ffff 8955 c888 4da3  .^.........U..M.
-00002360: e9a4 f9ff ffc7 0424 0c00 0000 e897 0b00  .......$........
-00002370: 0085 c00f 84b2 feff ff89 7008 c740 0400  ..........p..@..
-00002380: 0000 00c7 0000 0000 00eb 888b 45d4 c645  ............E..E
-00002390: a35c 8945 a4e9 acf9 ffff 8b55 d089 d8e8  .\.E.......U....
-000023a0: 9cf1 ffff 85c0 8945 cc0f 8511 feff ff89  .......E........
-000023b0: 1c24 89e6 e80f 0b00 0083 c010 c1e8 04c1  .$..............
-000023c0: e004 e8d9 f0ff ff29 c48d 4c24 0c89 caeb  .......)..L$....
-000023d0: 0d83 c201 83c3 0184 c088 42ff 7410 0fb6  ..........B.t...
-000023e0: 033c 7f75 ec0f b643 0183 c301 ebe3 890c  .<.u...C........
-000023f0: 24e8 320c 0000 85c0 89f4 0f84 1bff ffff  $.2.............
-00002400: 8b55 0885 d20f 8410 ffff ff8b 5508 e81d  .U..........U...
-00002410: f7ff ff8b 45e0 8945 bce9 5cfe ffff 8945  ....E..E..\....E
-00002420: c8e9 e3f8 ffff 0fb6 1889 45c8 885d a3e9  ..........E..]..
-00002430: d5f8 ffff 807d d400 0f84 d2fb ffff 3c2c  .....}........<,
-00002440: 89f2 0f85 d8fc ffff e92c fcff ff3c 7b74  .........,...<{t
-00002450: 088b 65c0 e9a1 f7ff ff89 55cc 89cf e962  ..e.......U....b
-00002460: fbff ff8d b600 0000 008d bc27 0000 0000  ...........'....
-00002470: 5589 e557 5653 83ec 2c8b 7514 8b5d 088b  U..WVS..,.u..]..
-00002480: 7d0c 85f6 7408 f7c7 0200 0000 7435 813e  }...t.......t5.>
-00002490: 2a51 4000 740d 89f0 e843 f1ff ffc7 062a  *Q@.t....C.....*
-000024a0: 5140 0089 3424 8b4d 1089 fa89 d8e8 2ef7  Q@..4$.M........
-000024b0: ffff 83f8 0289 c174 178d 65f4 89c8 5b5e  .......t..e...[^
-000024c0: 5f5d c3c7 460c 0000 0000 ebc2 8d74 2600  _]..F........t&.
-000024d0: 83e7 1074 e489 45e0 8965 e489 1c24 e8e5  ...t..E..e...$..
-000024e0: 0900 0083 c010 c1e8 04c1 e004 e8af efff  ................
-000024f0: ff8b 4de0 29c4 8d7c 2404 89fa eb0f 6690  ..M.)..|$.....f.
-00002500: 83c2 0183 c301 84c0 8842 ff74 1b0f b603  .........B.t....
-00002510: 3c7f 75ec 0fb6 4301 83c3 0183 c201 83c3  <.u...C.........
-00002520: 0184 c088 42ff 75e5 894d e089 3c24 e8f5  ....B.u..M..<$..
-00002530: 0a00 0085 c08b 65e4 8b4d e00f 8478 ffff  ......e..M...x..
-00002540: ff89 f289 4de4 e8e5 f5ff ff8b 4de4 e966  ....M.......M..f
-00002550: ffff ff8d b600 0000 008d bc27 0000 0000  ...........'....
-00002560: 5756 5383 ec10 8b74 2420 813e 2a51 4000  WVS....t$ .>*Q@.
-00002570: 740e 83c4 105b 5e5f c38d b426 0000 0000  t....[^_...&....
-00002580: 8b46 048b 560c 85c0 8d78 ff8d 1c95 0000  .F..V....x......
-00002590: 0000 7e19 8b46 0883 ef01 8b04 1883 c304  ..~..F..........
-000025a0: 8904 24e8 7009 0000 83ff ff75 e78b 4608  ..$.p......u..F.
-000025b0: 8944 2420 83c4 105b 5e5f e959 0900 0090  .D$ ...[^_.Y....
-000025c0: 5589 e557 5653 83ec 2cc7 4424 0400 0000  U..WVS..,.D$....
-000025d0: 00c7 0424 0200 0000 e803 0900 0085 c089  ...$............
-000025e0: c374 0a89 0424 e83d 0a00 0089 c3c7 4424  .t...$.=......D$
-000025f0: 043c 5140 00c7 0424 0200 0000 e8df 0800  .<Q@...$........
-00002600: 008b 7508 85f6 7408 8b45 0880 3800 7571  ..u...t..E..8.uq
-00002610: c744 2408 0000 0000 c744 2404 3e51 4000  .D$......D$.>Q@.
-00002620: c704 2400 0000 00e8 8408 0000 8d70 0189  ..$..........p..
-00002630: 7424 04a1 6870 4000 8904 24e8 a808 0000  t$..hp@...$.....
-00002640: a368 7040 0089 7424 08c7 4424 043e 5140  .hp@..t$..D$.>Q@
-00002650: 0089 0424 e857 0800 0089 5c24 04c7 0424  ...$.W....\$...$
-00002660: 0200 0000 e877 0800 0089 1c24 e8a7 0800  .....w.....$....
-00002670: 008b 3568 7040 008d 65f4 5b89 f05e 5f5d  ..5hp@..e.[..^_]
-00002680: c389 65dc c744 2408 0000 0000 8b45 08c7  ..e..D$......E..
-00002690: 0424 0000 0000 8944 2404 e861 0800 0089  .$.....D$..a....
-000026a0: c28d 4400 12c1 e804 c1e0 04e8 f0ed ffff  ..D.............
-000026b0: 29c4 8954 2408 8b45 088d 7c24 0c89 3c24  )..T$..E..|$..<$
-000026c0: 8944 2404 e837 0800 0031 c989 45d8 83f8  .D$..7...1..E...
-000026d0: 0166 890c 470f b707 897d e466 8945 e276  .f..G....}.f.E.v
-000026e0: 1f66 83f8 2f0f 841c 0200 0066 83f8 5c0f  .f../......f..\.
-000026f0: 8412 0200 0066 837f 023a 0f84 4f02 0000  .....f...:..O...
-00002700: 0fb7 45e2 6685 c00f 84e1 0000 008b 4de4  ..E.f.........M.
-00002710: 89c2 89ce eb1e 8d76 008d bc27 0000 0000  .......v...'....
-00002720: 6683 fa5c 89c8 7412 0fb7 5002 8d48 0266  f..\..t...P..H.f
-00002730: 85d2 7436 6683 fa2f 75e6 0fb7 1189 c866  ..t6f../u......f
-00002740: 83fa 2f75 0c83 c002 0fb7 1066 83fa 2f74  ../u.......f../t
-00002750: f466 83fa 5c74 ee66 85d2 740e 0fb7 5002  .f..\t.f..t...P.
-00002760: 89c6 8d48 0266 85d2 75ca 3975 e40f 828d  ...H.f..u.9u....
-00002770: 0000 000f b745 e266 83f8 2f0f 84e1 0100  .....E.f../.....
-00002780: 0066 83f8 5c0f 84d7 0100 008b 75e4 b92e  .f..\.......u...
-00002790: 0000 0089 f066 890e 83c0 0231 d266 8910  .....f.....1.f..
-000027a0: c744 2408 0000 0000 897c 2404 c704 2400  .D$......|$...$.
-000027b0: 0000 00e8 f806 0000 8d50 0189 5424 04a1  .........P..T$..
-000027c0: 6870 4000 8955 e489 0424 e819 0700 008b  hp@..U...$......
-000027d0: 55e4 a368 7040 0089 c689 7c24 0489 0424  U..hp@....|$...$
-000027e0: 8954 2408 e8c7 0600 00e9 c200 0000 8b65  .T$............e
-000027f0: dce9 1afe ffff 8d76 008d bc27 0000 0000  .......v...'....
-00002800: 8d46 fe39 45e4 0f83 6101 0000 0fb7 56fe  .F.9E...a.....V.
-00002810: 89c6 6683 fa2f 74e8 6683 fa5c 74e2 31d2  ..f../t.f..\t.1.
-00002820: 89f9 6689 5002 0fb7 1766 83fa 2f74 1166  ..f.P....f../t.f
-00002830: 83fa 5c0f 8504 0100 008d b426 0000 0000  ..\........&....
-00002840: 83c1 020f b701 6683 f82f 74f4 6683 f85c  ......f../t.f..\
-00002850: 74ee 89c8 29f8 83f8 050f 8ede 0000 0089  t...)...........
-00002860: f989 c866 85d2 7421 83c1 0266 83fa 2f66  ...f..t!...f../f
-00002870: 8951 fe74 6266 8338 5c8d 7002 7457 0fb7  .Q.tbf.8\.p.tW..
-00002880: 5002 89f0 6685 d275 df8b 45d8 31f6 6689  P...f..u..E.1.f.
-00002890: 3189 7c24 0489 4424 088b 4508 8904 24e8  1.|$..D$..E...$.
-000028a0: 0c06 0000 83f8 ff8b 7508 7404 c604 0600  ........u.t.....
-000028b0: 895c 2404 c704 2402 0000 00e8 2006 0000  .\$...$..... ...
-000028c0: 891c 24e8 5006 0000 8b65 dc8d 65f4 89f0  ..$.P....e..e...
-000028d0: 5b5e 5f5d c389 f00f b710 6683 fa5c 7410  [^_]......f..\t.
-000028e0: 6683 fa2f 0f85 79ff ffff 8db6 0000 0000  f../..y.........
-000028f0: 83c0 020f b710 6683 fa2f 74f4 6683 fa5c  ......f../t.f..\
-00002900: 74ee e95c ffff ff0f b745 e266 3b47 020f  t..\.....E.f;G..
-00002910: 85eb fdff ff66 837f 0400 0f85 e0fd ffff  .....f..........
-00002920: 895c 2404 c704 2402 0000 00e8 b005 0000  .\$...$.........
-00002930: 891c 24e8 e005 0000 8b75 08eb 8b66 3957  ..$......u...f9W
-00002940: 020f 8518 ffff ff0f b711 e912 ffff ff8d  ................
-00002950: 4704 8945 e40f b747 0466 8945 e2e9 9efd  G..E...G.f.E....
-00002960: ffff 8b45 e483 c002 e92e feff ff0f 85ab  ...E............
-00002970: feff ff0f b74d e266 83f9 2f74 0a66 83f9  .....M.f../t.f..
-00002980: 5c0f 8597 feff ff0f b74d e266 3948 020f  \........M.f9H..
-00002990: 8589 feff ff0f b750 0466 83fa 2f0f 847b  .......P.f../..{
-000029a0: feff ff66 83fa 5c0f 8471 feff ff89 f0e9  ...f..\..q......
-000029b0: 6afe ffff 9090 9090 9090 9090 9090 9090  j...............
-000029c0: 5653 89d3 81ec 5401 0000 8d54 2410 8904  VS....T....T$...
-000029d0: 2489 5424 04e8 1e06 0000 83ec 0883 f8ff  $.T$............
-000029e0: 89c6 745a 31c0 8d4b 0c66 8943 0631 c0eb  ..tZ1..K.f.C.1..
-000029f0: 120f b743 0683 c001 663d 0401 6689 4306  ...C....f=..f.C.
-00002a00: 83d1 000f b7c0 0fb6 4404 3c84 c088 0175  ........D.<....u
-00002a10: e08b 4424 1024 5883 f810 7614 c743 0818  ..D$.$X...v..C..
-00002a20: 0000 0081 c454 0100 0089 f05b 5ec3 6690  .....T.....[^.f.
-00002a30: 8943 0881 c454 0100 0089 f05b 5ec3 e80d  .C...T.....[^...
-00002a40: 0500 0089 c3e8 8e05 0000 83f8 0389 0374  ...............t
-00002a50: 31e8 fa04 0000 8138 0b01 0000 7417 e8ed  1......8....t...
-00002a60: 0400 0083 3802 74bb e8e3 0400 00c7 0016  ....8.t.........
-00002a70: 0000 00eb aee8 d604 0000 c700 1400 0000  ................
-00002a80: eba1 e8c9 0400 00c7 0002 0000 00eb 9490  ................
-00002a90: 5653 89d3 81ec 5401 0000 8d54 2410 8904  VS....T....T$...
-00002aa0: 2489 5424 04e8 4605 0000 83ec 0885 c089  $.T$..F.........
-00002ab0: c674 5f31 c08d 4b0c 6689 4306 31c0 eb12  .t_1..K.f.C.1...
-00002ac0: 0fb7 4306 83c0 0166 3d04 0166 8943 0683  ..C....f=..f.C..
-00002ad0: d100 0fb7 c00f b644 043c 84c0 8801 75e0  .......D.<....u.
-00002ae0: 8b44 2410 2458 83f8 1077 1589 4308 81c4  .D$.$X...w..C...
-00002af0: 5401 0000 89f0 5b5e c38d b426 0000 0000  T.....[^...&....
-00002b00: c743 0818 0000 0081 c454 0100 0089 f05b  .C.......T.....[
-00002b10: 5ec3 e8c1 0400 0083 f812 74d2 e82f 0400  ^.........t../..
-00002b20: 00c7 0002 0000 0081 c454 0100 0089 f05b  .........T.....[
-00002b30: 5ec3 8db4 2600 0000 008d bc27 0000 0000  ^...&......'....
-00002b40: 5557 5653 81ec 2c01 0000 8b84 2440 0100  UWVS..,.....$@..
-00002b50: 0085 c00f 8483 0100 0080 3800 0f84 5e01  ..........8...^.
-00002b60: 0000 8d7c 241c c744 2408 0401 0000 8944  ...|$..D$......D
-00002b70: 2404 893c 24e8 ce03 0000 807c 241c 0089  $..<$......|$...
-00002b80: f874 4d8b 0883 c004 8d91 fffe fefe f7d1  .tM.............
-00002b90: 21ca 81e2 8080 8080 74e9 f7c2 8080 0000  !.......t.......
-00002ba0: 0f84 0a01 0000 89d1 00d1 83d8 0329 f80f  .............)..
-00002bb0: b654 041b 80fa 2f74 4380 fa5c 743e b95c  .T..../tC..\t>.\
-00002bc0: 0000 0066 890c 0783 c001 eb30 8d74 2600  ...f.......0.t&.
-00002bd0: 8b08 83c0 048d 91ff fefe fef7 d121 ca81  .............!..
-00002be0: e280 8080 8074 e9f7 c280 8000 000f 84ad  .....t..........
-00002bf0: 0000 0089 d100 d183 d803 29f8 ba2a 0000  ..........)..*..
-00002c00: 0089 fb66 8914 078b 1383 c304 8d82 fffe  ...f............
-00002c10: fefe f7d2 21d0 2580 8080 8074 eaa9 8080  ....!.%....t....
-00002c20: 0000 7506 c1e8 1083 c302 89c1 00c1 83db  ..u.............
-00002c30: 0329 fb8d 831c 0100 0089 0424 e8c7 0200  .).........$....
-00002c40: 0085 c089 c60f 8484 0000 008d a818 0100  ................
-00002c50: 0083 c301 897c 2404 895c 2408 892c 24e8  .....|$..\$..,$.
-00002c60: 9402 0000 89f2 89e8 e853 fdff ff83 f8ff  .........S......
-00002c70: 8986 1001 0000 7473 b810 0100 00c7 8614  ......ts........
-00002c80: 0100 0000 0000 00c7 0600 0000 0066 8946  .............f.F
-00002c90: 0481 c42c 0100 0089 f05b 5e5f 5dc3 6690  ...,.....[^_].f.
-00002ca0: c1ea 1083 c002 e948 ffff ff90 8d74 2600  .......H.....t&.
-00002cb0: c1ea 1083 c002 e9eb feff ff90 8d74 2600  .............t&.
-00002cc0: e88b 0200 0031 f6c7 0002 0000 00eb c2e8  .....1..........
-00002cd0: 7c02 0000 c700 0c00 0000 ebb5 e86f 0200  |............o..
-00002ce0: 0031 f6c7 0016 0000 00eb a689 3424 31f6  .1..........4$1.
-00002cf0: e823 0200 00eb 9a89 f68d bc27 0000 0000  .#.........'....
-00002d00: 5383 ec08 8b5c 2410 85db 742b 8b83 1401  S....\$...t+....
-00002d10: 0000 8d50 0185 c089 9314 0100 007e 118b  ...P.........~..
-00002d20: 8310 0100 0089 dae8 64fd ffff 85c0 7402  ........d.....t.
-00002d30: 89d8 83c4 085b c3e8 1402 0000 c700 0900  .....[..........
-00002d40: 0000 31c0 ebec 8d76 008d bc27 0000 0000  ..1....v...'....
-00002d50: 5383 ec18 8b5c 2420 85db 7424 8b83 1001  S....\$ ..t$....
-00002d60: 0000 8904 24e8 9602 0000 83ec 0485 c074  ....$..........t
-00002d70: 0f89 1c24 e89f 0100 0031 c083 c418 5bc3  ...$.....1....[.
-00002d80: e8cb 0100 00c7 0009 0000 00b8 ffff ffff  ................
-00002d90: ebe9 8db4 2600 0000 008d bc27 0000 0000  ....&......'....
-00002da0: 5383 ec18 8b5c 2420 85db 7415 8b83 1001  S....\$ ..t.....
-00002db0: 0000 8904 24e8 4602 0000 83ec 0485 c075  ....$.F........u
-00002dc0: 10e8 8a01 0000 c700 0900 0000 83c4 185b  ...............[
-00002dd0: c38d 8318 0100 0089 dae8 e2fb ffff 83f8  ................
-00002de0: ff89 8310 0100 0074 e3c7 8314 0100 0000  .......t........
-00002df0: 0000 0083 c418 5bc3 908d b426 0000 0000  ......[....&....
-00002e00: 83ec 0c8b 4424 1085 c074 0a8b 8014 0100  ....D$...t......
-00002e10: 0083 c40c c3e8 3601 0000 c700 0900 0000  ......6.........
-00002e20: b8ff ffff ffeb ea89 f68d bc27 0000 0000  ...........'....
-00002e30: 5653 83ec 148b 7424 248b 5c24 2085 f678  VS....t$$.\$ ..x
-00002e40: 4f89 1c24 e857 ffff ff85 f674 3783 bb10  O..$.W.....t7...
-00002e50: 0100 00ff 751b eb2c 908d b426 0000 0000  ....u..,...&....
-00002e60: 8b83 1001 0000 89da e823 fcff ff85 c074  .........#.....t
-00002e70: 138b 8314 0100 0083 c001 39c6 8983 1401  ..........9.....
-00002e80: 0000 7fdc 83c4 145b 5ec3 8db6 0000 0000  .......[^.......
-00002e90: e8bb 0000 00c7 0016 0000 0083 c414 5b5e  ..............[^
-00002ea0: c390 9090 9090 9090 9090 9090 9090 9090  ................
-00002eb0: ff25 2482 4000 9090 ff25 2082 4000 9090  .%$.@....% .@...
-00002ec0: ff25 1c82 4000 9090 ff25 1882 4000 9090  .%..@....%..@...
-00002ed0: ff25 1482 4000 9090 ff25 1082 4000 9090  .%..@....%..@...
-00002ee0: ff25 0c82 4000 9090 ff25 0882 4000 9090  .%..@....%..@...
-00002ef0: ff25 0482 4000 9090 ff25 0082 4000 9090  .%..@....%..@...
-00002f00: ff25 fc81 4000 9090 ff25 f881 4000 9090  .%..@....%..@...
-00002f10: ff25 f481 4000 9090 ff25 f081 4000 9090  .%..@....%..@...
-00002f20: ff25 ec81 4000 9090 ff25 e881 4000 9090  .%..@....%..@...
-00002f30: ff25 e081 4000 9090 ff25 dc81 4000 9090  .%..@....%..@...
-00002f40: ff25 d081 4000 9090 ff25 c881 4000 9090  .%..@....%..@...
-00002f50: ff25 c081 4000 9090 ff25 bc81 4000 9090  .%..@....%..@...
-00002f60: ff25 b481 4000 9090 ff25 b081 4000 9090  .%..@....%..@...
-00002f70: ff25 a881 4000 9090 ff25 3482 4000 9090  .%..@....%4.@...
-00002f80: ff25 3082 4000 9090 ff25 2c82 4000 9090  .%0.@....%,.@...
-00002f90: ff25 9481 4000 9090 ff25 9081 4000 9090  .%..@....%..@...
-00002fa0: ff25 8c81 4000 9090 ff25 8881 4000 9090  .%..@....%..@...
-00002fb0: ff25 8481 4000 9090 ff25 8081 4000 9090  .%..@....%..@...
-00002fc0: ff25 7c81 4000 9090 ff25 7881 4000 9090  .%|.@....%x.@...
-00002fd0: ff25 7481 4000 9090 ff25 7081 4000 9090  .%t.@....%p.@...
-00002fe0: ff25 6c81 4000 9090 ff25 6881 4000 9090  .%l.@....%h.@...
-00002ff0: ff25 6481 4000 9090 ff25 6081 4000 9090  .%d.@....%`.@...
-00003000: ff25 5c81 4000 9090 ff25 5881 4000 9090  .%\.@....%X.@...
-00003010: ff25 5481 4000 9090 ff25 5081 4000 9090  .%T.@....%P.@...
-00003020: ff25 a081 4000 9090 ff25 9c81 4000 9090  .%..@....%..@...
-00003030: 5589 e55d e907 d7ff ff90 9090 9090 9090  U..]............
-00003040: ffff ffff 303c 4000 0000 0000 ffff ffff  ....0<@.........
-00003050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000850: 0b89 0424 e8d7 2700 0083 ec04 c9c3 9090  ...$..'.........
+00000860: 5589 e583 ec28 8d45 f489 4424 048b 4508  U....(.E..D$..E.
+00000870: 8904 24e8 5027 0000 83ec 088b 55f4 8b45  ..$.P'......U..E
+00000880: 0c39 c275 4d8b 4508 8904 24e8 3027 0000  .9.uM.E...$.0'..
+00000890: 83ec 0485 c075 16c7 4424 0409 0000 008b  .....u..D$......
+000008a0: 4508 8904 24e8 0627 0000 83ec 088b 4508  E...$..'......E.
+000008b0: 8904 24e8 0027 0000 83ec 0485 c075 0cc7  ..$..'.......u..
+000008c0: 0424 6450 4000 e855 2600 00b8 0000 0000  .$dP@..U&.......
+000008d0: eb05 b801 0000 00c9 c208 008d 4c24 0483  ............L$..
+000008e0: e4f0 ff71 fc55 89e5 5351 83ec 2089 cbe8  ...q.U..SQ.. ...
+000008f0: 8c05 0000 833b 0274 1c8b 4304 8b00 8944  .....;.t..C....D
+00000900: 2404 c704 2488 5040 00e8 1a26 0000 b801  $...$.P@...&....
+00000910: 0000 00eb 2e8b 4304 83c0 048b 0089 0424  ......C........$
+00000920: e83b 2600 0089 45f4 8b45 f489 4424 04c7  .;&...E..E..D$..
+00000930: 0424 6014 4000 e895 2600 0083 ec08 b800  .$`.@...&.......
+00000940: 0000 008d 65f8 595b 5d8d 61fc c390 9090  ....e.Y[].a.....
+00000950: 5589 e557 5653 83ec 4cf6 0504 4040 0002  U..WVS..L...@@..
+00000960: 0f84 ea02 0000 e8bd 2600 0089 65c4 8904  ........&...e...
+00000970: 2489 c6e8 8025 0000 8d44 0011 c1e8 04c1  $....%...D......
+00000980: e004 e849 0b00 0029 c4c7 45e4 0000 0000  ...I...)..E.....
+00000990: c745 d400 0000 008d 4424 10c7 45d0 0000  .E......D$..E...
+000009a0: 0000 89c2 8945 cca1 0440 4000 2500 4400  .....E...@@.%.D.
+000009b0: 0083 c810 8945 c831 c08d b426 0000 0000  .....E.1...&....
+000009c0: 83c6 010f be4e ff85 c989 cb74 7380 fb3f  .....N.....ts..?
+000009d0: 0f84 8d01 0000 0f8f b400 0000 80fb 270f  ..............'.
+000009e0: 84b0 0100 0080 fb2a 0f84 7501 0000 80fb  .......*..u.....
+000009f0: 220f 8509 0100 0089 c1d1 f90f 84d9 0200  "...............
+00000a00: 0001 d183 c201 c642 ff5c 39ca 75f5 837d  .......B.\9.u..}
+00000a10: d427 0f84 c901 0000 a801 0f85 c101 0000  .'..............
+00000a20: 83c6 0189 ca83 75d4 220f be4e ff31 c0c7  ......u."..N.1..
+00000a30: 45d0 0100 0000 85c9 89cb 7591 8d74 2600  E.........u..t&.
+00000a40: 85c0 0f84 9902 0000 01d0 8db6 0000 0000  ................
+00000a50: 83c2 01c6 42ff 5c39 c275 f539 45cc 0f82  ....B.\9.u.9E...
+00000a60: be01 0000 8b55 d085 d20f 85b3 0100 008b  .....U..........
+00000a70: 45dc a304 7040 008b 45e0 a300 7040 008b  E...p@..E...p@..
+00000a80: 65c4 8d65 f45b 5e5f 5dc3 8db6 0000 0000  e..e.[^_].......
+00000a90: 80fb 5c0f 84ea 0000 0080 fb7f 0f84 c100  ..\.............
+00000aa0: 0000 80fb 5b75 59f6 0504 4040 0020 0f85  ....[uY...@@. ..
+00000ab0: af00 0000 85c0 8d78 ffb9 0100 0000 7432  .......x......t2
+00000ac0: 8d7c 3a01 89d0 8d76 008d bc27 0000 0000  .|:....v...'....
+00000ad0: 83c0 01c6 40ff 5c39 f875 f584 c975 118d  ....@.\9.u...u..
+00000ae0: 5001 8818 31c0 e9d5 feff ff90 8d74 2600  P...1........t&.
+00000af0: 89c2 8d42 01c6 027f ebe5 8db6 0000 0000  ...B............
+00000b00: 85c0 8d3c 020f 84c8 0100 0090 8d74 2600  ...<.........t&.
+00000b10: 83c2 01c6 42ff 5c39 fa75 f58b 45d4 85c0  ....B.\9.u..E...
+00000b20: 7535 a1b8 8140 0083 3801 0f84 c500 0000  u5...@..8.......
+00000b30: c744 2404 4000 0000 890c 2489 4dc0 e835  .D$.@.....$.M..5
+00000b40: 2400 0085 c00f 85bb 0000 008b 4dc0 83f9  $...........M...
+00000b50: 090f 84af 0000 008d 5701 881f 31c0 e95d  ........W...1..]
+00000b60: feff ff85 c08d 78ff 0f84 4e01 0000 8b45  ......x...N....E
+00000b70: d483 f97f 0f94 c185 c00f 95c0 09c1 e93d  ...............=
+00000b80: ffff ff83 7dd4 270f 84e4 0000 0083 c001  ....}.'.........
+00000b90: e92b feff fff6 0504 4040 0010 0f84 5eff  .+......@@....^.
+00000ba0: ffff 89c1 d1f9 0f84 3c01 0000 01d1 6690  ........<.....f.
+00000bb0: 83c2 01c6 42ff 5c39 ca75 f583 7dd4 220f  ....B.\9.u..}.".
+00000bc0: 8498 0000 00a8 010f 8590 0000 0083 75d4  ..............u.
+00000bd0: 2789 ca31 c0c7 45d0 0100 0000 e9df fdff  '..1..E.........
+00000be0: ff8d 5101 c601 2231 c0c7 45d0 0100 0000  ..Q..."1..E.....
+00000bf0: e9cb fdff ffa1 e481 4000 8b00 f604 4840  ........@.....H@
+00000c00: 0f84 48ff ffff 397d cc72 758b 45d0 85c0  ..H...9}.ru.E...
+00000c10: 756e 89fa 31c0 c745 d000 0000 00e9 9efd  un..1..E........
+00000c20: ffff c600 008d 45d8 c744 2408 0000 0000  ......E..D$.....
+00000c30: 8944 240c 8b45 c889 4424 048b 45cc 8904  .D$..E..D$..E...
+00000c40: 24e8 5a18 0000 e924 feff ff90 8d74 2600  $.Z....$.....t&.
+00000c50: e84b faff ff8d 65f4 5b5e 5f5d c38d 5101  .K....e.[^_]..Q.
+00000c60: c601 2731 c0c7 45d0 0100 0000 e94f fdff  ..'1..E......O..
+00000c70: ffc6 025c 83c2 01e9 44fd ffff 8d74 2600  ...\....D....t&.
+00000c80: 8d45 d8c6 0700 c744 2408 0000 0000 8944  .E.....D$......D
+00000c90: 240c 8b5d c889 5c24 048b 7dcc 893c 24e8  $..]..\$..}..<$.
+00000ca0: fc17 0000 89d8 89fa c745 d000 0000 0083  .........E......
+00000cb0: c801 8945 c831 c0e9 04fd ffff 8b45 d485  ...E.1.......E..
+00000cc0: c00f 95c0 83f9 7f0f 94c1 09c1 89d0 e908  ................
+00000cd0: feff ff89 d7e9 41fe ffff 89d1 e92d fdff  ......A......-..
+00000ce0: ff89 d0e9 73fd ffff 89d1 e9cc feff ff90  ....s...........
+00000cf0: 9c9c 5889 c235 0000 2000 509d 9c58 9d31  ..X..5.. .P..X.1
+00000d00: d0a9 0000 2000 0f84 e900 0000 5331 c00f  .... .......S1..
+00000d10: a285 c00f 84db 0000 00b8 0100 0000 0fa2  ................
+00000d20: 31c0 f6c6 0174 0383 c801 f6c5 2074 050d  1....t...... t..
+00000d30: 8000 0000 f6c6 8074 0383 c802 f7c2 0000  .......t........
+00000d40: 8000 7403 83c8 04f7 c200 0000 0174 6d83  ..t..........tm.
+00000d50: c808 5589 e581 ec00 0200 0083 e4f0 0fae  ..U.............
+00000d60: 0424 8b9c 24c8 0000 0081 b424 c800 0000  .$..$......$....
+00000d70: dec0 1300 0fae 0c24 899c 24c8 0000 000f  .......$..$.....
+00000d80: ae04 2487 9c24 c800 0000 0fae 0c24 339c  ..$..$.......$3.
+00000d90: 24c8 0000 00c9 81fb dec0 1300 751e f7c2  $...........u...
+00000da0: 0000 0002 7403 83c8 10f7 c200 0000 0474  ....t..........t
+00000db0: 0383 c820 f6c1 0174 0383 c840 a324 7040  ... ...t...@.$p@
+00000dc0: 00b8 0000 0080 0fa2 3d00 0000 8076 25b8  ........=....v%.
+00000dd0: 0100 0080 0fa2 31c0 85d2 7905 b800 0100  ......1...y.....
+00000de0: 00f7 c200 0000 4074 050d 0002 0000 0905  ......@t........
+00000df0: 2470 4000 5bf3 c390 9090 9090 9090 9090  $p@.[...........
+00000e00: a110 4040 008b 0085 c074 1f83 ec0c 6690  ..@@.....t....f.
+00000e10: ffd0 a110 4040 008d 5004 8b40 0489 1510  ....@@..P..@....
+00000e20: 4040 0085 c075 e983 c40c f3c3 8d74 2600  @@...u.......t&.
+00000e30: 5383 ec18 8b1d 903c 4000 83fb ff74 2185  S......<@....t!.
+00000e40: db74 0cff 149d 903c 4000 83eb 0175 f4c7  .t.....<@....u..
+00000e50: 0424 001a 4000 e8c5 f8ff ff83 c418 5bc3  .$..@.........[.
+00000e60: 31db eb02 89c3 8d43 018b 1485 903c 4000  1......C.....<@.
+00000e70: 85d2 75f0 ebc9 8d76 008d bc27 0000 0000  ..u....v...'....
+00000e80: a128 7040 0085 c074 07f3 c390 8d74 2600  .(p@...t.....t&.
+00000e90: c705 2870 4000 0100 0000 eb94 9090 9090  ..(p@...........
+00000ea0: 83ec 1c8b 4424 2483 f803 7414 85c0 7410  ....D$$...t...t.
+00000eb0: b801 0000 0083 c41c c20c 0090 8d74 2600  .............t&.
+00000ec0: 8b54 2428 8944 2404 8b44 2420 8954 2408  .T$(.D$..D$ .T$.
+00000ed0: 8904 24e8 4802 0000 b801 0000 0083 c41c  ..$.H...........
+00000ee0: c20c 008d b600 0000 008d bc27 0000 0000  ...........'....
+00000ef0: 5653 83ec 1483 3d64 7040 0002 8b44 2424  VS....=dp@...D$$
+00000f00: 740a c705 6470 4000 0200 0000 83f8 0274  t...dp@........t
+00000f10: 1283 f801 743f 83c4 14b8 0100 0000 5b5e  ....t?........[^
+00000f20: c20c 00be 1490 4000 81ee 1490 4000 83fe  ......@.....@...
+00000f30: 037e e331 db8b 8314 9040 0085 c074 02ff  .~.1.....@...t..
+00000f40: d083 c304 39de 75ed 83c4 14b8 0100 0000  ....9.u.........
+00000f50: 5b5e c20c 008b 4424 28c7 4424 0401 0000  [^....D$(.D$....
+00000f60: 0089 4424 088b 4424 2089 0424 e8af 0100  ..D$..D$ ..$....
+00000f70: 00eb a38d b600 0000 008d bc27 0000 0000  ...........'....
+00000f80: 31c0 c390 9090 9090 9090 9090 9090 9090  1...............
+00000f90: 5653 83ec 14c7 0424 4470 4000 e8b7 2000  VS.....$Dp@... .
+00000fa0: 008b 1d3c 7040 0083 ec04 85db 742d 6690  ...<p@......t-f.
+00000fb0: 8b03 8904 24e8 2e20 0000 83ec 0489 c6e8  ....$.. ........
+00000fc0: 5c20 0000 85c0 750c 85f6 7408 8b43 0489  \ ....u...t..C..
+00000fd0: 3424 ffd0 8b5b 0885 db75 d5c7 0424 4470  4$...[...u...$Dp
+00000fe0: 4000 e819 2000 0083 ec04 83c4 145b 5ec3  @... ........[^.
+00000ff0: 5653 31f6 83ec 14a1 4070 4000 85c0 7510  VS1.....@p@...u.
+00001000: 83c4 1489 f05b 5ec3 908d b426 0000 0000  .....[^....&....
+00001010: c744 2404 0c00 0000 c704 2401 0000 00e8  .D$.......$.....
+00001020: 341f 0000 85c0 89c3 7441 8b44 2420 c704  4.......tA.D$ ..
+00001030: 2444 7040 0089 038b 4424 2489 4304 e815  $Dp@....D$$.C...
+00001040: 2000 00a1 3c70 4000 83ec 0489 1d3c 7040   ...<p@......<p@
+00001050: 00c7 0424 4470 4000 8943 08e8 a01f 0000  ...$Dp@..C......
+00001060: 83ec 0489 f083 c414 5b5e c3be ffff ffff  ........[^......
+00001070: eb8e 8db4 2600 0000 008d bc27 0000 0000  ....&......'....
+00001080: 5383 ec18 a140 7040 008b 5c24 2085 c075  S....@p@..\$ ..u
+00001090: 0f83 c418 31c0 5bc3 908d b426 0000 0000  ....1.[....&....
+000010a0: c704 2444 7040 00e8 ac1f 0000 8b15 3c70  ..$Dp@........<p
+000010b0: 4000 83ec 0485 d274 178b 0239 c375 0aeb  @......t...9.u..
+000010c0: 4e8b 0839 d974 2989 c28b 4208 85c0 75f1  N..9.t)...B...u.
+000010d0: c704 2444 7040 00e8 241f 0000 83ec 0483  ..$Dp@..$.......
+000010e0: c418 31c0 5bc3 8d76 008d bc27 0000 0000  ..1.[..v...'....
+000010f0: 8b48 0889 4a08 8904 24e8 521e 0000 c704  .H..J...$.R.....
+00001100: 2444 7040 00e8 f61e 0000 83ec 04eb d08b  $Dp@............
+00001110: 4208 a33c 7040 0089 d0eb db90 8d74 2600  B..<p@.......t&.
+00001120: 83ec 1c8b 4424 2483 f801 7447 7217 83f8  ....D$$...tGr...
+00001130: 0375 09a1 4070 4000 85c0 7565 b801 0000  .u..@p@...ue....
+00001140: 0083 c41c c3a1 4070 4000 85c0 7562 a140  ......@p@...ub.@
+00001150: 7040 0083 f801 75e4 c704 2444 7040 00c7  p@....u...$Dp@..
+00001160: 0540 7040 0000 0000 00e8 f21e 0000 83ec  .@p@............
+00001170: 04eb c9a1 4070 4000 85c0 7414 c705 4070  ....@p@...t...@p
+00001180: 4000 0100 0000 b801 0000 0083 c41c c390  @...............
+00001190: c704 2444 7040 00e8 6c1e 0000 83ec 04eb  ..$Dp@..l.......
+000011a0: dbe8 eafd ffff eb94 908d b426 0000 0000  ...........&....
+000011b0: e8db fdff ffeb 9790 9090 9090 9090 9090  ................
+000011c0: 5653 83ec 14a1 d881 4000 c744 2408 1700  VS......@..D$...
+000011d0: 0000 c744 2404 0100 0000 8d74 2424 c704  ...D$......t$$..
+000011e0: 24a0 5040 008d 5840 895c 240c e857 1d00  $.P@..X@.\$..W..
+000011f0: 008b 4424 2089 7424 0889 1c24 8944 2404  ..D$ .t$...$.D$.
+00001200: e8e3 1c00 00e8 5e1d 0000 8db6 0000 0000  ......^.........
+00001210: 5557 89cf 5653 89c3 89d6 83ec 4c8d 4424  UW..VS......L.D$
+00001220: 24c7 4424 081c 0000 0089 1c24 8944 2404  $.D$.......$.D$.
+00001230: e8a3 1d00 0083 ec0c 85c0 0f84 a800 0000  ................
+00001240: 8b44 2438 83f8 4074 0583 f804 7522 897c  .D$8..@t....u".|
+00001250: 2408 8974 2404 891c 24e8 d21c 0000 83c4  $..t$...$.......
+00001260: 4c5b 5e5f 5dc3 8d76 008d bc27 0000 0000  L[^_]..v...'....
+00001270: 8b44 2430 8d6c 2420 c744 2408 4000 0000  .D$0.l$ .D$.@...
+00001280: 896c 240c 8944 2404 8b44 2424 8904 24e8  .l$..D$..D$$..$.
+00001290: 4c1d 0000 83ec 108b 5424 3889 7c24 0889  L.......T$8.|$..
+000012a0: 7424 0489 1c24 8954 241c e881 1c00 008b  t$...$.T$.......
+000012b0: 5424 1c83 fa40 74a6 83fa 0474 a18b 4424  T$...@t....t..D$
+000012c0: 2089 6c24 0c89 4424 088b 4424 3089 4424   .l$..D$..D$0.D$
+000012d0: 048b 4424 2489 0424 e803 1d00 0083 ec10  ..D$$..$........
+000012e0: 83c4 4c5b 5e5f 5dc3 895c 2408 c744 2404  ..L[^_]..\$..D$.
+000012f0: 1c00 0000 c704 24b8 5040 00e8 c0fe ffff  ......$.P@......
+00001300: a15c 7040 0085 c074 07c3 8db6 0000 0000  .\p@...t........
+00001310: b808 5340 00c7 055c 7040 0001 0000 002d  ..S@...\p@.....-
+00001320: 0853 4000 83f8 077e e057 5653 83ec 2083  .S@....~.WVS.. .
+00001330: f80b 0f8e e800 0000 8b35 0853 4000 85f6  .........5.S@...
+00001340: 0f85 8f00 0000 8b1d 0c53 4000 85db 0f85  .........S@.....
+00001350: 8100 0000 8b0d 1053 4000 bb14 5340 0085  .......S@...S@..
+00001360: c90f 84be 0000 00bb 0853 4000 8b43 0883  .........S@..C..
+00001370: f801 0f85 4301 0000 83c3 0c81 fb08 5340  ....C.........S@
+00001380: 000f 8389 0000 008b 138b 7b04 8db2 0000  ..........{.....
+00001390: 4000 8b8a 0000 4000 0fb6 5308 8d87 0000  @.....@...S.....
+000013a0: 4000 83fa 100f 8495 0000 0083 fa20 0f84  @............ ..
+000013b0: ec00 0000 83fa 080f 84b3 0000 0089 5424  ..............T$
+000013c0: 04c7 0424 2051 4000 c744 241c 0000 0000  ...$ Q@..D$.....
+000013d0: e8eb fdff ffbb 0853 4000 81fb 0853 4000  .......S@....S@.
+000013e0: 732e 8b4b 048b 1383 c308 0391 0000 4000  s..K..........@.
+000013f0: 8d81 0000 4000 b904 0000 0089 5424 1c8d  ....@.......T$..
+00001400: 5424 1ce8 08fe ffff 81fb 0853 4000 72d2  T$.........S@.r.
+00001410: 83c4 205b 5e5f c389 f68d bc27 0000 0000  .. [^_.....'....
+00001420: bb08 5340 008b 1385 d275 af8b 4304 85c0  ..S@.....u..C...
+00001430: 0f84 36ff ffff eba2 908d b426 0000 0000  ..6........&....
+00001440: 0fb7 9700 0040 0066 85d2 7906 81ca 0000  .....@.f..y.....
+00001450: ffff 29f2 01d1 8d54 241c 894c 241c b902  ..)....T$..L$...
+00001460: 0000 00e8 a8fd ffff e90b ffff ff8d 7600  ..............v.
+00001470: 0fb6 3889 fa84 d279 0681 cf00 ffff ff29  ..8....y.......)
+00001480: f78d 5424 1c01 f989 4c24 1cb9 0100 0000  ..T$....L$......
+00001490: e87b fdff ffe9 defe ffff 8db6 0000 0000  .{..............
+000014a0: 29f1 0308 8d54 241c 894c 241c b904 0000  )....T$..L$.....
+000014b0: 00e8 5afd ffff e9bd feff ff89 4424 04c7  ..Z.........D$..
+000014c0: 0424 ec50 4000 e8f5 fcff ff90 9090 9090  .$.P@...........
+000014d0: 5150 3d00 1000 008d 4c24 0c72 1581 e900  QP=.....L$.r....
+000014e0: 1000 0083 0900 2d00 1000 003d 0010 0000  ......-....=....
+000014f0: 77eb 29c1 8309 0058 59c3 9090 6690 6690  w.)....XY...f.f.
+00001500: 83ec 1c8b 4424 20c7 4424 0c80 1f00 0083  ....D$ .D$......
+00001510: f8fd 7431 83f8 fc74 3a85 c074 4883 f8ff  ..t1...t:..tH...
+00001520: 742d 83f8 fe74 36d9 200f b740 1c89 4424  t-...t6. ..@..D$
+00001530: 0cf6 0524 7040 0010 7405 0fae 5424 0c31  ...$p@..t...T$.1
+00001540: c083 c41c c3c7 0514 4040 00ff ffff ffdb  ........@@......
+00001550: e3eb dec7 0514 4040 00fe ffff ffff 15d0  ......@@........
+00001560: 8140 00eb cca1 1440 4000 ebb1 9090 9090  .@.....@@.......
+00001570: 85c0 0f84 8200 0000 5653 89d3 c1eb 0531  ........VS.....1
+00001580: c983 f301 83e3 0189 f68d bc27 0000 0000  ...........'....
+00001590: 0fbe 1085 d274 2984 db74 0583 fa7f 7440  .....t)..t....t@
+000015a0: 83c0 0185 c975 1e83 fa2a 7444 83fa 3f74  .....u...*tD..?t
+000015b0: 3f31 c983 fa5b 0fbe 100f 94c1 85d2 75d7  ?1...[........u.
+000015c0: 89d0 5b5e c383 f901 7e05 83fa 5d74 2183  ..[^....~...]t!.
+000015d0: fa21 0f95 c20f b6d2 01d1 ebb4 8d74 2600  .!...........t&.
+000015e0: 8078 0100 8d70 0274 1689 f0eb b68d 7600  .x...p.t......v.
+000015f0: ba01 0000 0089 d05b 5ec3 31d2 89d0 c331  .......[^.1....1
+00001600: d2eb bd8d b600 0000 008d bc27 0000 0000  ...........'....
+00001610: 85c0 745c 5653 89c6 83ec 148b 400c 8d58  ..t\VS......@..X
+00001620: 018d 049d 0000 0000 8904 24e8 1019 0000  ..........$.....
+00001630: 89c1 8946 08b8 0300 0000 85c9 7422 85db  ...F........t"..
+00001640: 89da c746 0400 0000 007e 1390 8d74 2600  ...F.....~...t&.
+00001650: 83ea 0185 d2c7 0491 0000 0000 75f2 31c0  ............u.1.
+00001660: 83c4 145b 5ec3 8d76 008d bc27 0000 0000  ...[^..v...'....
+00001670: 31c0 c38d b600 0000 008d bc27 0000 0000  1..........'....
+00001680: 5557 89c7 5653 83ec 3c0f be18 8954 241c  UW..VS..<....T$.
+00001690: 894c 2420 83fb 5d89 dd0f 8461 0100 0083  .L$ ..]....a....
+000016a0: fb2d 0f84 5801 0000 8b4c 241c 89c8 f7d0  .-..X....L$.....
+000016b0: 8944 2428 b801 0000 0029 c889 4424 2ceb  .D$(.....)..D$,.
+000016c0: 0d89 ee2b 7424 1c85 f674 680f beda 83fb  ...+t$...th.....
+000016d0: 5d8d 7701 0f84 1a01 0000 83fb 2d0f 848d  ].w.........-...
+000016e0: 0000 0085 db0f 8409 0100 0083 fb2f 0f84  ............./..
+000016f0: 0001 0000 83fb 5c0f 84f7 0000 000f b616  ......\.........
+00001700: 89dd 89f7 f744 2420 0040 0000 75b3 892c  .....D$ .@..u..,
+00001710: 2488 5424 24e8 d617 0000 89c6 8b44 241c  $.T$$........D$.
+00001720: 8904 24e8 c817 0000 29c6 0fb6 5424 2485  ..$.....)...T$$.
+00001730: f675 988b 4424 2083 e020 eb12 8d74 2600  .u..D$ .. ...t&.
+00001740: 83c7 0184 d20f 84a9 0000 000f b617 80fa  ................
+00001750: 5d0f 843e 0100 0080 fa7f 75e4 85c0 0f85  ]..>......u.....
+00001760: 3c01 0000 0fb6 5701 83c7 01eb d38d 7600  <.....W.......v.
+00001770: 0fb6 5701 80fa 5d0f 8495 0000 000f beda  ..W...].........
+00001780: 85db 7470 8b4c 2420 8d77 0281 e100 4000  ..tp.L$ .w....@.
+00001790: 0039 dd0f 8d0f 0100 0089 7424 2489 e889  .9........t$$...
+000017a0: ceeb 118b 4424 288d 3c28 85ff 7429 39eb  ....D$(.<(..t)9.
+000017b0: 89e8 746c 85f6 8d68 0175 e889 0424 e82d  ..tl...h.u...$.-
+000017c0: 1700 0089 c78b 4424 1c89 0424 e81f 1700  ......D$...$....
+000017d0: 0029 c785 ff75 d78b 5424 208b 7424 2483  .)...u..T$ .t$$.
+000017e0: e220 0fb6 063c 5d74 613c 7f74 4383 c601  . ...<]ta<.tC...
+000017f0: 84c0 75ee 83c4 3c31 c05b 5e5f 5dc3 6690  ..u...<1.[^_].f.
+00001800: 3b5c 241c 744f 0fbe 5f01 83c7 01e9 96fe  ;\$.tO.._.......
+00001810: ffff bd2d 0000 0089 f7e9 e6fe ffff 6690  ...-..........f.
+00001820: 8b74 2424 e9c2 feff ff8d b426 0000 0000  .t$$.......&....
+00001830: 85d2 750c 0fb6 4601 83c6 01eb b08d 7600  ..u...F.......v.
+00001840: 83c6 010f b606 3c5d 759f 83c4 3c8d 4601  ......<]u...<.F.
+00001850: 5b5e 5f5d c38b 5424 2083 c701 83e2 2090  [^_]..T$ ..... .
+00001860: 0fb6 073c 5d74 2e3c 7f74 1583 c701 84c0  ...<]t.<.t......
+00001870: 75ee e97d ffff ff89 f68d bc27 0000 0000  u..}.......'....
+00001880: 85d2 750c 0fb6 4701 83c7 01eb de8d 7600  ..u...G.......v.
+00001890: 83c7 01eb cb83 c43c 8d47 015b 5e5f 5dc3  .......<.G.[^_].
+000018a0: 83c7 01e9 a3fe ffff 0f8e 3dfe ffff 8974  ..........=....t
+000018b0: 2424 89ce eb1f 8d76 008d bc27 0000 0000  $$.....v...'....
+000018c0: 8b44 242c 8d2c 3885 ed74 2d39 fb89 fd0f  .D$,.,8..t-9....
+000018d0: 844b ffff ff85 f68d 7dff 75e4 892c 24e8  .K......}.u..,$.
+000018e0: 0c16 0000 89c5 8b44 241c 8904 24e8 fe15  .......D$...$...
+000018f0: 0000 29c5 85ed 75d3 8b54 2420 8b74 2424  ..)...u..T$ .t$$
+00001900: 83e2 200f b606 3c5d 0f84 3cff ffff 3c7f  .. ...<]..<...<.
+00001910: 740e 83c6 0184 c075 eae9 d6fe ffff 6690  t......u......f.
+00001920: 85d2 750c 0fb6 4601 83c6 01eb e58d 7600  ..u...F.......v.
+00001930: 83c6 01eb ce8d 7426 008d bc27 0000 0000  ......t&...'....
+00001940: 5557 89c5 5653 83ec 2c80 3a2e 894c 2414  UW..VS..,.:..L$.
+00001950: 0fb6 080f 8437 0100 008b 4424 148d 7a01  .....7....D$..z.
+00001960: c1e8 0583 f001 8944 2418 0fbe d18d 77ff  .......D$.....w.
+00001970: 8d45 0185 d20f 8469 0100 0080 f93f 0f84  .E.....i.....?..
+00001980: ed00 0000 80f9 5b0f 84b3 0000 0080 f92a  ......[........*
+00001990: 745e f644 2418 0174 0983 fa7f 0f84 2e01  t^.D$..t........
+000019a0: 0000 89c5 0fbe 5fff 84db 0f84 8601 0000  ......_.........
+000019b0: f744 2414 0040 0000 0f85 c200 0000 8914  .D$..@..........
+000019c0: 2489 5424 1ce8 2615 0000 891c 2489 c6e8  $.T$..&.....$...
+000019d0: 1c15 0000 8b54 241c 29c6 85f6 0f84 8300  .....T$.).......
+000019e0: 0000 89d0 29d8 83c4 2c5b 5e5f 5dc3 6690  ....)...,[^_].f.
+000019f0: 0fb6 5501 89c3 80fa 2a75 1090 8d74 2600  ..U.....*u...t&.
+00001a00: 83c3 010f b613 80fa 2a74 f531 c084 d274  ........*t.1...t
+00001a10: d58b 7c24 1481 cf00 0001 00eb 0c8d 7600  ..|$..........v.
+00001a20: 83c6 0180 7eff 0074 bd89 f989 f289 d8e8  ....~..t........
+00001a30: 0cff ffff 85c0 75e8 83c4 2c5b 5e5f 5dc3  ......u...,[^_].
+00001a40: 0fbe 57ff 85d2 0f84 fb00 0000 807d 0121  ..W..........}.!
+00001a50: 7460 8b4c 2414 e825 fcff ff89 c585 ed0f  t`.L$..%........
+00001a60: 84c7 0000 000f b64d 0083 c701 e9f9 feff  .......M........
+00001a70: ff80 7fff 000f 84c2 0000 0089 c5eb e690  ................
+00001a80: 89d6 29de e951 ffff ff8d b426 0000 0000  ..)..Q.....&....
+00001a90: 80f9 2e0f 84c0 feff ff0f bec1 83e8 2ef7  ................
+00001aa0: 4424 1400 0001 000f 85ac feff ffe9 34ff  D$............4.
+00001ab0: ffff 8d5d 028b 4c24 1489 d8e8 c0fb ffff  ...]..L$........
+00001ac0: 85c0 742a 89dd eb95 908d b426 0000 0000  ..t*.......&....
+00001ad0: 0fbe 5501 83c5 0285 d20f 85c5 feff ffe9  ..U.............
+00001ae0: befe ffff 0fbe 06f7 d8e9 f8fe ffff 0fb6  ................
+00001af0: 4502 3c5d 745b 8b54 2414 83e2 20eb 0b90  E.<]t[.T$... ...
+00001b00: 83c3 0184 c074 250f b603 3c5d 7416 3c7f  .....t%...<]t.<.
+00001b10: 75ee 85d2 7509 0fb6 4301 83c3 01eb e183  u...u...C.......
+00001b20: c301 ebe3 8d6b 01e9 31ff ffff b85d 0000  .....k..1....]..
+00001b30: 00e9 b0fe ffff 31db e9a5 feff ffb8 3f00  ......1.......?.
+00001b40: 0000 e99f feff ffb8 5b00 0000 e995 feff  ........[.......
+00001b50: ff8d 5d03 0fb6 4503 eb9c 8db6 0000 0000  ..]...E.........
+00001b60: 5756 89c6 5389 d383 ec10 8b42 0c03 4204  WV..S......B..B.
+00001b70: 8d04 8508 0000 0089 4424 048b 4208 8904  ........D$..B...
+00001b80: 24e8 9213 0000 85c0 7426 8b4b 048b 530c  $.......t&.K..S.
+00001b90: 8943 088d 7901 01d1 01fa 897b 0489 3488  .C..y......{..4.
+00001ba0: c704 9000 0000 0083 c410 31c0 5b5e 5fc3  ..........1.[^_.
+00001bb0: 83c4 10b8 0100 0000 5b5e 5fc3 8d74 2600  ........[^_..t&.
+00001bc0: 5653 89c3 89d6 83ec 148b 0085 c074 05e8  VS...........t..
+00001bd0: ecff ffff 8b43 0885 c074 0485 f675 218b  .....C...t...u!.
+00001be0: 4304 85c0 7407 89f2 e8d3 ffff ff89 1c24  C...t..........$
+00001bf0: e85b 1300 0083 c414 5b5e c390 8d74 2600  .[......[^...t&.
+00001c00: 89f2 e859 ffff ffeb d68d b426 0000 0000  ...Y.......&....
+00001c10: 5589 e557 5653 89c3 83ec 6c89 55d0 80e6  U..WVS....l.U...
+00001c20: 0489 4dc4 0f85 5603 0000 8965 a889 1c24  ..M...V....e...$
+00001c30: e8c3 1200 008d 5001 83c0 10c1 e804 c1e0  ......P.........
+00001c40: 04e8 8af8 ffff 29c4 8d44 240c 8954 2408  ......)..D$..T$.
+00001c50: 895c 2404 8904 24e8 d412 0000 8904 24e8  .\$...$.......$.
+00001c60: 8c09 0000 8945 d489 c68d 45d8 c745 e400  .....E....E..E..
+00001c70: 0000 00e8 98f9 ffff 85c0 8945 cc0f 85ed  ...........E....
+00001c80: 0200 008b 7dd0 89f0 89fa e8e1 f8ff ff85  ....}...........
+00001c90: c00f 84d7 0400 008d 45d8 89fa 80ce 8089  ........E.......
+00001ca0: 0424 8b4d c489 f0e8 64ff ffff 8945 cc8b  .$.M....d....E..
+00001cb0: 4dcc 85c9 0f85 b602 0000 0fb6 4301 3c2f  M...........C.</
+00001cc0: 7419 3c5c 7415 8b75 d4bf 4c51 4000 b902  t.<\t..u..LQ@...
+00001cd0: 0000 00f3 a60f 840b 0500 008b 45d4 8904  ............E...
+00001ce0: 24e8 1212 0000 01d8 39c3 0f83 6607 0000  $.......9...f...
+00001cf0: 0fb6 0880 f92f 884d a30f 844f 0700 0080  ...../.M...O....
+00001d00: f95c 7524 e945 0700 008d b426 0000 0000  .\u$.E.....&....
+00001d10: 0fb6 48ff 89d0 80f9 2f0f 846b 0600 0080  ..H...../..k....
+00001d20: f95c 0f84 6206 0000 8d50 ff39 d375 e10f  .\..b....P.9.u..
+00001d30: b640 ff89 55c8 8845 a30f b645 a33c 2f74  .@..U..E...E.</t
+00001d40: 083c 5c0f 8572 0600 008b 55c8 0fb6 75a3  .<\..r....U...u.
+00001d50: eb02 89c6 83c2 010f b602 3c2f 0f94 c33c  ..........</...<
+00001d60: 5c0f 94c1 08cb 75ea 89f0 8955 c888 45a3  \.....u....U..E.
+00001d70: 8b45 d489 45a4 8b45 e08b 7dd0 c745 cc02  .E..E..E..}..E..
+00001d80: 0000 0089 45bc 8b00 81e7 0080 0000 897d  ....E..........}
+00001d90: d485 c00f 8411 0500 0089 0424 e8cf 0d00  ...........$....
+00001da0: 0085 c089 c70f 84b8 0400 008b 45a4 85c0  ............E...
+00001db0: 0f84 7405 0000 8b45 bc8b 0089 0424 e835  ..t....E.....$.5
+00001dc0: 1100 0089 45c0 8b45 c0c7 45b8 0000 0000  ....E..E..E.....
+00001dd0: 83c0 0289 45ac 8d76 008d bc27 0000 0000  ....E..v...'....
+00001de0: 893c 24e8 480f 0000 85c0 89c6 0f84 1104  .<$.H...........
+00001df0: 0000 8b45 d485 c074 0683 7e08 1075 e18d  ...E...t..~..u..
+00001e00: 5e0c 8b4d d08b 45c8 89da e831 fbff ff85  ^..M..E....1....
+00001e10: c075 cd0f b756 068b 45ac 8965 b08d 4402  .u...V..E..e..D.
+00001e20: 0fc1 e804 c1e0 04e8 a4f6 ffff 29c4 8b45  ............)..E
+00001e30: c0c7 45b4 0000 0000 8d74 240c 85c0 0f85  ..E......t$.....
+00001e40: 7c04 0000 8b45 b483 c201 895c 2404 8954  |....E.....\$..T
+00001e50: 2408 89e3 01f0 8904 24e8 d210 0000 8934  $.......$......4
+00001e60: 24e8 9210 0000 83c0 10c1 e804 c1e0 04e8  $...............
+00001e70: 5cf6 ffff 29c4 89f0 8d4c 240c 89ce eb0d  \...)....L$.....
+00001e80: 83c6 0183 c001 84d2 8856 ff74 1c0f b610  .........V.t....
+00001e90: 80fa 7f75 eb0f b650 0183 c001 83c6 0183  ...u...P........
+00001ea0: c001 84d2 8856 ff75 e489 0c24 e8bf 1100  .....V.u...$....
+00001eb0: 0085 c089 c689 dc0f 8447 0400 008b 5dcc  .........G....].
+00001ec0: 83fb 020f 94c0 0fb6 c083 e801 21c3 8b45  ............!..E
+00001ed0: d089 5dcc a840 0f85 7403 0000 8b5d b885  ..]..@..t....]..
+00001ee0: db0f 84ae 0400 0025 0040 0000 897d b489  .......%.@...}..
+00001ef0: c7eb 14e8 0810 0000 85c0 8b13 8b4b 047e  .............K.~
+00001f00: 2285 c974 2489 cb8b 4308 85ff 8934 2489  "..t$...C....4$.
+00001f10: 4424 0475 dee8 4e11 0000 85c0 8b13 8b4b  D$.u..N........K
+00001f20: 047f de89 d185 c975 dc8b 7db4 8945 b4c7  .......u..}..E..
+00001f30: 0424 0c00 0000 e805 1000 0085 c00f 8418  .$..............
+00001f40: 0300 008b 55b4 8970 08c7 4004 0000 0000  ....U..p..@.....
+00001f50: c700 0000 0000 85d2 0f8e d803 0000 8943  ...............C
+00001f60: 04e9 f502 0000 c745 cc01 0000 008d 7600  .......E......v.
+00001f70: 8b65 a88b 45cc 8d65 f45b 5e5f 5dc3 6690  .e..E..e.[^_].f.
+00001f80: 8965 c089 0424 e86d 0f00 0083 c010 c1e8  .e...$.m........
+00001f90: 04c1 e004 e837 f5ff ff29 c489 de8d 4424  .....7...)....D$
+00001fa0: 0c89 c789 45c8 0fb6 033c 7f74 283c 7b74  ....E....<.t(<{t
+00001fb0: 3f84 c08d 5701 8d4e 0188 070f 84bc 0400  ?...W..N........
+00001fc0: 003c 7b0f 84b4 0400 000f b646 0189 d789  .<{........F....
+00001fd0: ce3c 7f75 d80f b646 01c6 077f 84c0 0f85  .<.u...F........
+00001fe0: ac00 0000 83c7 0183 c601 ebc5 8d74 2600  .............t&.
+00001ff0: 897d cc89 f78b 55cc b901 0000 000f b647  .}....U........G
+00002000: 013c 7f74 2683 c701 3c7d 7409 3c2c 7540  .<.t&...<}t.<,u@
+00002010: 83f9 0175 3b83 e901 0f84 8300 0000 8802  ...u;...........
+00002020: 0fb6 4701 83c2 013c 7f75 da0f b647 02c6  ..G....<.u...G..
+00002030: 027f 8d5a 0284 c088 4201 7534 c642 0200  ...Z....B.u4.B..
+00002040: c745 cc01 0000 00e9 0e01 0000 8d74 2600  .E...........t&.
+00002050: 3c7b 742c 84c0 0f95 45d4 0fb6 5dd4 84db  <{t,....E...]...
+00002060: 8d72 0188 020f 84f9 0300 0089 f2eb 8e90  .r..............
+00002070: 0fb6 4703 89da 83c7 03eb 8d90 8d74 2600  ..G..........t&.
+00002080: 83c1 01bb 0100 0000 c645 d401 ebd0 6690  .........E....f.
+00002090: 8847 0183 c602 0fb6 0683 c702 e908 ffff  .G..............
+000020a0: ff3c 2c0f 85c1 0000 0089 f8be 0100 0000  .<,.............
+000020b0: 0fb6 5801 8d48 0180 fb7f 0f85 1f01 0000  ..X..H..........
+000020c0: 8078 0200 7512 e985 0000 0090 8d74 2600  .x..u........t&.
+000020d0: 8078 0100 747a 89c1 0fb6 5902 8d41 0280  .x..tz....Y..A..
+000020e0: fb7f 74ec 80fb 7b74 7980 fb7d 7555 83ee  ..t...{ty..}uU..
+000020f0: 0175 bd8d 4801 0fb6 4001 eb07 8d74 2600  .u..H...@....t&.
+00002100: 0fb6 0183 c201 83c1 0184 c088 42ff 75f0  ............B.u.
+00002110: 8b45 0889 0424 8b75 d08b 4dc4 8b45 c889  .E...$.u..M..E..
+00002120: f283 ce01 e8e7 faff ff83 f801 8975 d00f  .............u..
+00002130: 840b ffff ff80 3f2c 0f84 b7fe ffff 8945  ......?,.......E
+00002140: cceb 1784 db0f 8565 ffff ff90 8d74 2600  .......e.....t&.
+00002150: c602 00c7 45cc 0100 0000 8b65 c0e9 11fe  ....E......e....
+00002160: ffff 83c6 01e9 46ff ffff 89f8 eb85 8b45  ......F........E
+00002170: d489 e689 0424 e87d 0d00 0083 c010 c1e8  .....$.}........
+00002180: 04c1 e004 e847 f3ff ff8b 55d4 29c4 8d7c  .....G....U.)..|
+00002190: 240c 89f9 eb17 8d76 008d bc27 0000 0000  $......v...'....
+000021a0: 83c1 0183 c201 84c0 8841 ff74 100f b602  .........A.t....
+000021b0: 3c7f 75ec 0fb6 4201 83c2 01eb e389 3c24  <.u...B.......<$
+000021c0: e8ab 0e00 0085 c089 f40f 8497 fdff ff8d  ................
+000021d0: 55d8 e889 f9ff ff89 45cc e9d0 faff ff89  U.......E.......
+000021e0: c8e9 fefe ffff f645 d010 0f85 da01 0000  .......E........
+000021f0: 895d c8c6 45a3 5cc7 45a4 0000 0000 e973  .]..E.\.E......s
+00002200: fbff ff89 3c24 e875 0b00 008b 55b8 85d2  ....<$.u....U...
+00002210: 740b 8b55 088b 45b8 e8a3 f9ff ff8b 7dbc  t..U..E.......}.
+00002220: 8d5f 048b 43fc 8904 24e8 220d 0000 8b47  ._..C...$."....G
+00002230: 0485 c00f 8412 0100 0083 7dcc 0174 4789  ..........}..tG.
+00002240: 5dbc e952 fbff ff89 f68d bc27 0000 0000  ]..R.......'....
+00002250: 8b4d 0885 c90f 85c0 0000 008b 65b0 e97d  .M..........e..}
+00002260: fbff fff6 45d0 040f 84e9 0000 008b 7dbc  ....E.........}.
+00002270: 8d5f 0489 f88b 0089 0424 e8d1 0c00 008b  ._.......$......
+00002280: 4704 85c0 7417 8b45 bc8b 4004 83c3 0489  G...t..E..@.....
+00002290: 0424 e8b9 0c00 008b 0385 c075 ef8b 45e0  .$.........u..E.
+000022a0: c745 cc01 0000 0089 45bc 8b45 bc89 0424  .E......E..E...$
+000022b0: e89b 0c00 008b 65a8 e9b6 fcff ff8d 7600  ......e.......v.
+000022c0: 8b45 bc89 55b4 8b55 c08b 0089 3424 8954  .E..U..U....4$.T
+000022d0: 2408 8944 2404 e855 0c00 008b 4dc0 8b55  $..D$..U....M..U
+000022e0: b40f b644 0c0b 3c2f 7426 3c5c 7422 89c8  ...D..</t&<\t"..
+000022f0: 83c0 0189 45b4 89c8 0fb6 4da3 880c 06e9  ....E.....M.....
+00002300: 40fb ffff c745 cc03 0000 00e9 4bff ffff  @....E......K...
+00002310: 8b45 c089 45b4 e929 fbff ff8b 5508 89f0  .E..E..)....U...
+00002320: e83b f8ff ffe9 31ff ffff c745 c000 0000  .;....1....E....
+00002330: 00e9 90fa ffff 8903 8b5d b885 db0f 8518  .........]......
+00002340: ffff ff89 45b8 e910 ffff ff8b 45e0 8945  ....E.......E..E
+00002350: bce9 54ff ffff 8b7d c485 ff0f 84bc feff  ..T....}........
+00002360: ffe8 220c 0000 8b00 8944 2404 8b75 bc8b  .."......D$..u..
+00002370: 0689 0424 ffd7 85c0 0f84 9ffe ffff 89f0  ...$............
+00002380: 8d5e 0489 f7e9 ebfe ffff 8955 c888 4da3  .^.........U..M.
+00002390: e9a4 f9ff ffc7 0424 0c00 0000 e89f 0b00  .......$........
+000023a0: 0085 c00f 84b2 feff ff89 7008 c740 0400  ..........p..@..
+000023b0: 0000 00c7 0000 0000 00eb 888b 45d4 c645  ............E..E
+000023c0: a35c 8945 a4e9 acf9 ffff 8b55 d089 d8e8  .\.E.......U....
+000023d0: 9cf1 ffff 85c0 8945 cc0f 8511 feff ff89  .......E........
+000023e0: 1c24 89e6 e80f 0b00 0083 c010 c1e8 04c1  .$..............
+000023f0: e004 e8d9 f0ff ff29 c48d 4c24 0c89 caeb  .......)..L$....
+00002400: 0d83 c201 83c3 0184 c088 42ff 7410 0fb6  ..........B.t...
+00002410: 033c 7f75 ec0f b643 0183 c301 ebe3 890c  .<.u...C........
+00002420: 24e8 4a0c 0000 85c0 89f4 0f84 1bff ffff  $.J.............
+00002430: 8b55 0885 d20f 8410 ffff ff8b 5508 e81d  .U..........U...
+00002440: f7ff ff8b 45e0 8945 bce9 5cfe ffff 8945  ....E..E..\....E
+00002450: c8e9 e3f8 ffff 0fb6 1889 45c8 885d a3e9  ..........E..]..
+00002460: d5f8 ffff 807d d400 0f84 d2fb ffff 3c2c  .....}........<,
+00002470: 89f2 0f85 d8fc ffff e92c fcff ff3c 7b74  .........,...<{t
+00002480: 088b 65c0 e9a1 f7ff ff89 55cc 89cf e962  ..e.......U....b
+00002490: fbff ff8d b600 0000 008d bc27 0000 0000  ...........'....
+000024a0: 5589 e557 5653 83ec 2c8b 7514 8b5d 088b  U..WVS..,.u..]..
+000024b0: 7d0c 85f6 7408 f7c7 0200 0000 7435 813e  }...t.......t5.>
+000024c0: 4e51 4000 740d 89f0 e843 f1ff ffc7 064e  NQ@.t....C.....N
+000024d0: 5140 0089 3424 8b4d 1089 fa89 d8e8 2ef7  Q@..4$.M........
+000024e0: ffff 83f8 0289 c174 178d 65f4 89c8 5b5e  .......t..e...[^
+000024f0: 5f5d c3c7 460c 0000 0000 ebc2 8d74 2600  _]..F........t&.
+00002500: 83e7 1074 e489 45e0 8965 e489 1c24 e8e5  ...t..E..e...$..
+00002510: 0900 0083 c010 c1e8 04c1 e004 e8af efff  ................
+00002520: ff8b 4de0 29c4 8d7c 2404 89fa eb0f 6690  ..M.)..|$.....f.
+00002530: 83c2 0183 c301 84c0 8842 ff74 1b0f b603  .........B.t....
+00002540: 3c7f 75ec 0fb6 4301 83c3 0183 c201 83c3  <.u...C.........
+00002550: 0184 c088 42ff 75e5 894d e089 3c24 e80d  ....B.u..M..<$..
+00002560: 0b00 0085 c08b 65e4 8b4d e00f 8478 ffff  ......e..M...x..
+00002570: ff89 f289 4de4 e8e5 f5ff ff8b 4de4 e966  ....M.......M..f
+00002580: ffff ff8d b600 0000 008d bc27 0000 0000  ...........'....
+00002590: 5756 5383 ec10 8b74 2420 813e 4e51 4000  WVS....t$ .>NQ@.
+000025a0: 740e 83c4 105b 5e5f c38d b426 0000 0000  t....[^_...&....
+000025b0: 8b46 048b 560c 85c0 8d78 ff8d 1c95 0000  .F..V....x......
+000025c0: 0000 7e19 8b46 0883 ef01 8b04 1883 c304  ..~..F..........
+000025d0: 8904 24e8 7809 0000 83ff ff75 e78b 4608  ..$.x......u..F.
+000025e0: 8944 2420 83c4 105b 5e5f e961 0900 0090  .D$ ...[^_.a....
+000025f0: 5589 e557 5653 83ec 2cc7 4424 0400 0000  U..WVS..,.D$....
+00002600: 00c7 0424 0200 0000 e803 0900 0085 c089  ...$............
+00002610: c374 0a89 0424 e855 0a00 0089 c3c7 4424  .t...$.U......D$
+00002620: 0460 5140 00c7 0424 0200 0000 e8df 0800  .`Q@...$........
+00002630: 008b 7508 85f6 7408 8b45 0880 3800 7571  ..u...t..E..8.uq
+00002640: c744 2408 0000 0000 c744 2404 6251 4000  .D$......D$.bQ@.
+00002650: c704 2400 0000 00e8 8408 0000 8d70 0189  ..$..........p..
+00002660: 7424 04a1 6870 4000 8904 24e8 a808 0000  t$..hp@...$.....
+00002670: a368 7040 0089 7424 08c7 4424 0462 5140  .hp@..t$..D$.bQ@
+00002680: 0089 0424 e857 0800 0089 5c24 04c7 0424  ...$.W....\$...$
+00002690: 0200 0000 e877 0800 0089 1c24 e8af 0800  .....w.....$....
+000026a0: 008b 3568 7040 008d 65f4 5b89 f05e 5f5d  ..5hp@..e.[..^_]
+000026b0: c389 65dc c744 2408 0000 0000 8b45 08c7  ..e..D$......E..
+000026c0: 0424 0000 0000 8944 2404 e869 0800 0089  .$.....D$..i....
+000026d0: c28d 4400 12c1 e804 c1e0 04e8 f0ed ffff  ..D.............
+000026e0: 29c4 8954 2408 8b45 088d 7c24 0c89 3c24  )..T$..E..|$..<$
+000026f0: 8944 2404 e83f 0800 0031 c989 45d8 83f8  .D$..?...1..E...
+00002700: 0166 890c 470f b707 897d e466 8945 e276  .f..G....}.f.E.v
+00002710: 1f66 83f8 2f0f 841c 0200 0066 83f8 5c0f  .f../......f..\.
+00002720: 8412 0200 0066 837f 023a 0f84 4f02 0000  .....f...:..O...
+00002730: 0fb7 45e2 6685 c00f 84e1 0000 008b 4de4  ..E.f.........M.
+00002740: 89c2 89ce eb1e 8d76 008d bc27 0000 0000  .......v...'....
+00002750: 6683 fa5c 89c8 7412 0fb7 5002 8d48 0266  f..\..t...P..H.f
+00002760: 85d2 7436 6683 fa2f 75e6 0fb7 1189 c866  ..t6f../u......f
+00002770: 83fa 2f75 0c83 c002 0fb7 1066 83fa 2f74  ../u.......f../t
+00002780: f466 83fa 5c74 ee66 85d2 740e 0fb7 5002  .f..\t.f..t...P.
+00002790: 89c6 8d48 0266 85d2 75ca 3975 e40f 828d  ...H.f..u.9u....
+000027a0: 0000 000f b745 e266 83f8 2f0f 84e1 0100  .....E.f../.....
+000027b0: 0066 83f8 5c0f 84d7 0100 008b 75e4 b92e  .f..\.......u...
+000027c0: 0000 0089 f066 890e 83c0 0231 d266 8910  .....f.....1.f..
+000027d0: c744 2408 0000 0000 897c 2404 c704 2400  .D$......|$...$.
+000027e0: 0000 00e8 f806 0000 8d50 0189 5424 04a1  .........P..T$..
+000027f0: 6870 4000 8955 e489 0424 e819 0700 008b  hp@..U...$......
+00002800: 55e4 a368 7040 0089 c689 7c24 0489 0424  U..hp@....|$...$
+00002810: 8954 2408 e8c7 0600 00e9 c200 0000 8b65  .T$............e
+00002820: dce9 1afe ffff 8d76 008d bc27 0000 0000  .......v...'....
+00002830: 8d46 fe39 45e4 0f83 6101 0000 0fb7 56fe  .F.9E...a.....V.
+00002840: 89c6 6683 fa2f 74e8 6683 fa5c 74e2 31d2  ..f../t.f..\t.1.
+00002850: 89f9 6689 5002 0fb7 1766 83fa 2f74 1166  ..f.P....f../t.f
+00002860: 83fa 5c0f 8504 0100 008d b426 0000 0000  ..\........&....
+00002870: 83c1 020f b701 6683 f82f 74f4 6683 f85c  ......f../t.f..\
+00002880: 74ee 89c8 29f8 83f8 050f 8ede 0000 0089  t...)...........
+00002890: f989 c866 85d2 7421 83c1 0266 83fa 2f66  ...f..t!...f../f
+000028a0: 8951 fe74 6266 8338 5c8d 7002 7457 0fb7  .Q.tbf.8\.p.tW..
+000028b0: 5002 89f0 6685 d275 df8b 45d8 31f6 6689  P...f..u..E.1.f.
+000028c0: 3189 7c24 0489 4424 088b 4508 8904 24e8  1.|$..D$..E...$.
+000028d0: 0c06 0000 83f8 ff8b 7508 7404 c604 0600  ........u.t.....
+000028e0: 895c 2404 c704 2402 0000 00e8 2006 0000  .\$...$..... ...
+000028f0: 891c 24e8 5806 0000 8b65 dc8d 65f4 89f0  ..$.X....e..e...
+00002900: 5b5e 5f5d c389 f00f b710 6683 fa5c 7410  [^_]......f..\t.
+00002910: 6683 fa2f 0f85 79ff ffff 8db6 0000 0000  f../..y.........
+00002920: 83c0 020f b710 6683 fa2f 74f4 6683 fa5c  ......f../t.f..\
+00002930: 74ee e95c ffff ff0f b745 e266 3b47 020f  t..\.....E.f;G..
+00002940: 85eb fdff ff66 837f 0400 0f85 e0fd ffff  .....f..........
+00002950: 895c 2404 c704 2402 0000 00e8 b005 0000  .\$...$.........
+00002960: 891c 24e8 e805 0000 8b75 08eb 8b66 3957  ..$......u...f9W
+00002970: 020f 8518 ffff ff0f b711 e912 ffff ff8d  ................
+00002980: 4704 8945 e40f b747 0466 8945 e2e9 9efd  G..E...G.f.E....
+00002990: ffff 8b45 e483 c002 e92e feff ff0f 85ab  ...E............
+000029a0: feff ff0f b74d e266 83f9 2f74 0a66 83f9  .....M.f../t.f..
+000029b0: 5c0f 8597 feff ff0f b74d e266 3948 020f  \........M.f9H..
+000029c0: 8589 feff ff0f b750 0466 83fa 2f0f 847b  .......P.f../..{
+000029d0: feff ff66 83fa 5c0f 8471 feff ff89 f0e9  ...f..\..q......
+000029e0: 6afe ffff 9090 9090 9090 9090 9090 9090  j...............
+000029f0: 5653 89d3 81ec 5401 0000 8d54 2410 8904  VS....T....T$...
+00002a00: 2489 5424 04e8 3606 0000 83ec 0883 f8ff  $.T$..6.........
+00002a10: 89c6 745a 31c0 8d4b 0c66 8943 0631 c0eb  ..tZ1..K.f.C.1..
+00002a20: 120f b743 0683 c001 663d 0401 6689 4306  ...C....f=..f.C.
+00002a30: 83d1 000f b7c0 0fb6 4404 3c84 c088 0175  ........D.<....u
+00002a40: e08b 4424 1024 5883 f810 7614 c743 0818  ..D$.$X...v..C..
+00002a50: 0000 0081 c454 0100 0089 f05b 5ec3 6690  .....T.....[^.f.
+00002a60: 8943 0881 c454 0100 0089 f05b 5ec3 e815  .C...T.....[^...
+00002a70: 0500 0089 c3e8 a605 0000 83f8 0389 0374  ...............t
+00002a80: 31e8 0205 0000 8138 0b01 0000 7417 e8f5  1......8....t...
+00002a90: 0400 0083 3802 74bb e8eb 0400 00c7 0016  ....8.t.........
+00002aa0: 0000 00eb aee8 de04 0000 c700 1400 0000  ................
+00002ab0: eba1 e8d1 0400 00c7 0002 0000 00eb 9490  ................
+00002ac0: 5653 89d3 81ec 5401 0000 8d54 2410 8904  VS....T....T$...
+00002ad0: 2489 5424 04e8 5e05 0000 83ec 0885 c089  $.T$..^.........
+00002ae0: c674 5f31 c08d 4b0c 6689 4306 31c0 eb12  .t_1..K.f.C.1...
+00002af0: 0fb7 4306 83c0 0166 3d04 0166 8943 0683  ..C....f=..f.C..
+00002b00: d100 0fb7 c00f b644 043c 84c0 8801 75e0  .......D.<....u.
+00002b10: 8b44 2410 2458 83f8 1077 1589 4308 81c4  .D$.$X...w..C...
+00002b20: 5401 0000 89f0 5b5e c38d b426 0000 0000  T.....[^...&....
+00002b30: c743 0818 0000 0081 c454 0100 0089 f05b  .C.......T.....[
+00002b40: 5ec3 e8d9 0400 0083 f812 74d2 e837 0400  ^.........t..7..
+00002b50: 00c7 0002 0000 0081 c454 0100 0089 f05b  .........T.....[
+00002b60: 5ec3 8db4 2600 0000 008d bc27 0000 0000  ^...&......'....
+00002b70: 5557 5653 81ec 2c01 0000 8b84 2440 0100  UWVS..,.....$@..
+00002b80: 0085 c00f 8483 0100 0080 3800 0f84 5e01  ..........8...^.
+00002b90: 0000 8d7c 241c c744 2408 0401 0000 8944  ...|$..D$......D
+00002ba0: 2404 893c 24e8 d603 0000 807c 241c 0089  $..<$......|$...
+00002bb0: f874 4d8b 0883 c004 8d91 fffe fefe f7d1  .tM.............
+00002bc0: 21ca 81e2 8080 8080 74e9 f7c2 8080 0000  !.......t.......
+00002bd0: 0f84 0a01 0000 89d1 00d1 83d8 0329 f80f  .............)..
+00002be0: b654 041b 80fa 2f74 4380 fa5c 743e b95c  .T..../tC..\t>.\
+00002bf0: 0000 0066 890c 0783 c001 eb30 8d74 2600  ...f.......0.t&.
+00002c00: 8b08 83c0 048d 91ff fefe fef7 d121 ca81  .............!..
+00002c10: e280 8080 8074 e9f7 c280 8000 000f 84ad  .....t..........
+00002c20: 0000 0089 d100 d183 d803 29f8 ba2a 0000  ..........)..*..
+00002c30: 0089 fb66 8914 078b 1383 c304 8d82 fffe  ...f............
+00002c40: fefe f7d2 21d0 2580 8080 8074 eaa9 8080  ....!.%....t....
+00002c50: 0000 7506 c1e8 1083 c302 89c1 00c1 83db  ..u.............
+00002c60: 0329 fb8d 831c 0100 0089 0424 e8cf 0200  .).........$....
+00002c70: 0085 c089 c60f 8484 0000 008d a818 0100  ................
+00002c80: 0083 c301 897c 2404 895c 2408 892c 24e8  .....|$..\$..,$.
+00002c90: 9c02 0000 89f2 89e8 e853 fdff ff83 f8ff  .........S......
+00002ca0: 8986 1001 0000 7473 b810 0100 00c7 8614  ......ts........
+00002cb0: 0100 0000 0000 00c7 0600 0000 0066 8946  .............f.F
+00002cc0: 0481 c42c 0100 0089 f05b 5e5f 5dc3 6690  ...,.....[^_].f.
+00002cd0: c1ea 1083 c002 e948 ffff ff90 8d74 2600  .......H.....t&.
+00002ce0: c1ea 1083 c002 e9eb feff ff90 8d74 2600  .............t&.
+00002cf0: e893 0200 0031 f6c7 0002 0000 00eb c2e8  .....1..........
+00002d00: 8402 0000 c700 0c00 0000 ebb5 e877 0200  .............w..
+00002d10: 0031 f6c7 0016 0000 00eb a689 3424 31f6  .1..........4$1.
+00002d20: e82b 0200 00eb 9a89 f68d bc27 0000 0000  .+.........'....
+00002d30: 5383 ec08 8b5c 2410 85db 742b 8b83 1401  S....\$...t+....
+00002d40: 0000 8d50 0185 c089 9314 0100 007e 118b  ...P.........~..
+00002d50: 8310 0100 0089 dae8 64fd ffff 85c0 7402  ........d.....t.
+00002d60: 89d8 83c4 085b c3e8 1c02 0000 c700 0900  .....[..........
+00002d70: 0000 31c0 ebec 8d76 008d bc27 0000 0000  ..1....v...'....
+00002d80: 5383 ec18 8b5c 2420 85db 7424 8b83 1001  S....\$ ..t$....
+00002d90: 0000 8904 24e8 ae02 0000 83ec 0485 c074  ....$..........t
+00002da0: 0f89 1c24 e8a7 0100 0031 c083 c418 5bc3  ...$.....1....[.
+00002db0: e8d3 0100 00c7 0009 0000 00b8 ffff ffff  ................
+00002dc0: ebe9 8db4 2600 0000 008d bc27 0000 0000  ....&......'....
+00002dd0: 5383 ec18 8b5c 2420 85db 7415 8b83 1001  S....\$ ..t.....
+00002de0: 0000 8904 24e8 5e02 0000 83ec 0485 c075  ....$.^........u
+00002df0: 10e8 9201 0000 c700 0900 0000 83c4 185b  ...............[
+00002e00: c38d 8318 0100 0089 dae8 e2fb ffff 83f8  ................
+00002e10: ff89 8310 0100 0074 e3c7 8314 0100 0000  .......t........
+00002e20: 0000 0083 c418 5bc3 908d b426 0000 0000  ......[....&....
+00002e30: 83ec 0c8b 4424 1085 c074 0a8b 8014 0100  ....D$...t......
+00002e40: 0083 c40c c3e8 3e01 0000 c700 0900 0000  ......>.........
+00002e50: b8ff ffff ffeb ea89 f68d bc27 0000 0000  ...........'....
+00002e60: 5653 83ec 148b 7424 248b 5c24 2085 f678  VS....t$$.\$ ..x
+00002e70: 4f89 1c24 e857 ffff ff85 f674 3783 bb10  O..$.W.....t7...
+00002e80: 0100 00ff 751b eb2c 908d b426 0000 0000  ....u..,...&....
+00002e90: 8b83 1001 0000 89da e823 fcff ff85 c074  .........#.....t
+00002ea0: 138b 8314 0100 0083 c001 39c6 8983 1401  ..........9.....
+00002eb0: 0000 7fdc 83c4 145b 5ec3 8db6 0000 0000  .......[^.......
+00002ec0: e8c3 0000 00c7 0016 0000 0083 c414 5b5e  ..............[^
+00002ed0: c390 9090 9090 9090 9090 9090 9090 9090  ................
+00002ee0: ff25 3482 4000 9090 ff25 3082 4000 9090  .%4.@....%0.@...
+00002ef0: ff25 2c82 4000 9090 ff25 2882 4000 9090  .%,.@....%(.@...
+00002f00: ff25 2482 4000 9090 ff25 2082 4000 9090  .%$.@....% .@...
+00002f10: ff25 1c82 4000 9090 ff25 1882 4000 9090  .%..@....%..@...
+00002f20: ff25 1482 4000 9090 ff25 1082 4000 9090  .%..@....%..@...
+00002f30: ff25 0c82 4000 9090 ff25 0882 4000 9090  .%..@....%..@...
+00002f40: ff25 0482 4000 9090 ff25 0082 4000 9090  .%..@....%..@...
+00002f50: ff25 fc81 4000 9090 ff25 f881 4000 9090  .%..@....%..@...
+00002f60: ff25 f481 4000 9090 ff25 ec81 4000 9090  .%..@....%..@...
+00002f70: ff25 e881 4000 9090 ff25 dc81 4000 9090  .%..@....%..@...
+00002f80: ff25 d481 4000 9090 ff25 cc81 4000 9090  .%..@....%..@...
+00002f90: ff25 c881 4000 9090 ff25 c081 4000 9090  .%..@....%..@...
+00002fa0: ff25 bc81 4000 9090 ff25 b481 4000 9090  .%..@....%..@...
+00002fb0: ff25 4c82 4000 9090 ff25 4882 4000 9090  .%L.@....%H.@...
+00002fc0: ff25 4482 4000 9090 ff25 4082 4000 9090  .%D.@....%@.@...
+00002fd0: ff25 3c82 4000 9090 ff25 a081 4000 9090  .%<.@....%..@...
+00002fe0: ff25 9c81 4000 9090 ff25 9881 4000 9090  .%..@....%..@...
+00002ff0: ff25 9481 4000 9090 ff25 9081 4000 9090  .%..@....%..@...
+00003000: ff25 8c81 4000 9090 ff25 8881 4000 9090  .%..@....%..@...
+00003010: ff25 8481 4000 9090 ff25 8081 4000 9090  .%..@....%..@...
+00003020: ff25 7c81 4000 9090 ff25 7881 4000 9090  .%|.@....%x.@...
+00003030: ff25 7481 4000 9090 ff25 7081 4000 9090  .%t.@....%p.@...
+00003040: ff25 6c81 4000 9090 ff25 6881 4000 9090  .%l.@....%h.@...
+00003050: ff25 6481 4000 9090 ff25 6081 4000 9090  .%d.@....%`.@...
+00003060: ff25 5c81 4000 9090 ff25 ac81 4000 9090  .%\.@....%..@...
+00003070: ff25 a881 4000 9090 6690 6690 6690 6690  .%..@...f.f.f.f.
+00003080: 5589 e55d e9b7 d6ff ff90 9090 9090 9090  U..]............
+00003090: ffff ffff 803c 4000 0000 0000 ffff ffff  .....<@.........
 000030a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000030b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000030c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000030d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000030e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000030f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -795,15 +795,15 @@
 000031a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003200: 0000 0000 0200 0000 fdff ffff 0040 0000  .............@..
-00003210: 503c 4000 ffff ffff 0000 0000 0000 0000  P<@.............
+00003210: a03c 4000 ffff ffff 0000 0000 0000 0000  .<@.............
 00003220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -832,57 +832,57 @@
 000033f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003400: 6c69 6267 6363 5f73 5f64 7732 2d31 2e64  libgcc_s_dw2-1.d
 00003410: 6c6c 005f 5f72 6567 6973 7465 725f 6672  ll.__register_fr
 00003420: 616d 655f 696e 666f 005f 5f64 6572 6567  ame_info.__dereg
 00003430: 6973 7465 725f 6672 616d 655f 696e 666f  ister_frame_info
 00003440: 006c 6962 6763 6a2d 3136 2e64 6c6c 005f  .libgcj-16.dll._
 00003450: 4a76 5f52 6567 6973 7465 7243 6c61 7373  Jv_RegisterClass
-00003460: 6573 0000 5573 6167 653a 2025 7320 3c50  es..Usage: %s <P
-00003470: 4944 3e0a 0000 0000 c01a 4000 4d69 6e67  ID>.......@.Ming
-00003480: 7720 7275 6e74 696d 6520 6661 696c 7572  w runtime failur
-00003490: 653a 0a00 2020 5669 7274 7561 6c51 7565  e:..  VirtualQue
-000034a0: 7279 2066 6169 6c65 6420 666f 7220 2564  ry failed for %d
-000034b0: 2062 7974 6573 2061 7420 6164 6472 6573   bytes at addres
-000034c0: 7320 2570 0000 0000 2020 556e 6b6e 6f77  s %p....  Unknow
-000034d0: 6e20 7073 6575 646f 2072 656c 6f63 6174  n pseudo relocat
-000034e0: 696f 6e20 7072 6f74 6f63 6f6c 2076 6572  ion protocol ver
-000034f0: 7369 6f6e 2025 642e 0a00 0000 2020 556e  sion %d.....  Un
-00003500: 6b6e 6f77 6e20 7073 6575 646f 2072 656c  known pseudo rel
-00003510: 6f63 6174 696f 6e20 6269 7420 7369 7a65  ocation bit size
-00003520: 2025 642e 0a00 0000 2e00 676c 6f62 2d31   %d.......glob-1
-00003530: 2e30 2d6d 696e 6777 3332 0000 0000 2e00  .0-mingw32......
-00003540: 0000 0000 4743 433a 2028 474e 5529 2036  ....GCC: (GNU) 6
-00003550: 2e33 2e30 0000 0000 4743 433a 2028 474e  .3.0....GCC: (GN
-00003560: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
-00003570: 2028 4d69 6e47 572e 6f72 6720 4743 432d   (MinGW.org GCC-
-00003580: 362e 332e 302d 3129 2036 2e33 2e30 0000  6.3.0-1) 6.3.0..
-00003590: 4743 433a 2028 474e 5529 2036 2e33 2e30  GCC: (GNU) 6.3.0
-000035a0: 0000 0000 4743 433a 2028 474e 5529 2036  ....GCC: (GNU) 6
-000035b0: 2e33 2e30 0000 0000 4743 433a 2028 474e  .3.0....GCC: (GN
-000035c0: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
-000035d0: 2028 474e 5529 2036 2e33 2e30 0000 0000   (GNU) 6.3.0....
-000035e0: 4743 433a 2028 474e 5529 2036 2e33 2e30  GCC: (GNU) 6.3.0
-000035f0: 0000 0000 4743 433a 2028 474e 5529 2036  ....GCC: (GNU) 6
-00003600: 2e33 2e30 0000 0000 4743 433a 2028 474e  .3.0....GCC: (GN
-00003610: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
-00003620: 2028 474e 5529 2036 2e33 2e30 0000 0000   (GNU) 6.3.0....
-00003630: 4743 433a 2028 474e 5529 2036 2e33 2e30  GCC: (GNU) 6.3.0
-00003640: 0000 0000 4743 433a 2028 474e 5529 2036  ....GCC: (GNU) 6
-00003650: 2e33 2e30 0000 0000 4743 433a 2028 474e  .3.0....GCC: (GN
-00003660: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
-00003670: 2028 474e 5529 2036 2e33 2e30 0000 0000   (GNU) 6.3.0....
-00003680: 4743 433a 2028 474e 5529 2036 2e33 2e30  GCC: (GNU) 6.3.0
-00003690: 0000 0000 4743 433a 2028 474e 5529 2036  ....GCC: (GNU) 6
-000036a0: 2e33 2e30 0000 0000 4743 433a 2028 474e  .3.0....GCC: (GN
-000036b0: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
-000036c0: 2028 474e 5529 2036 2e33 2e30 0000 0000   (GNU) 6.3.0....
-000036d0: 4743 433a 2028 474e 5529 2036 2e33 2e30  GCC: (GNU) 6.3.0
-000036e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000036f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003460: 6573 0000 4661 696c 6564 2074 6f20 7365  es..Failed to se
+00003470: 7420 7769 6e64 6f77 2074 6f20 666f 7265  t window to fore
+00003480: 6772 6f75 6e64 2e00 5573 6167 653a 2025  ground..Usage: %
+00003490: 7320 3c50 4944 3e0a 0000 0000 f01a 4000  s <PID>.......@.
+000034a0: 4d69 6e67 7720 7275 6e74 696d 6520 6661  Mingw runtime fa
+000034b0: 696c 7572 653a 0a00 2020 5669 7274 7561  ilure:..  Virtua
+000034c0: 6c51 7565 7279 2066 6169 6c65 6420 666f  lQuery failed fo
+000034d0: 7220 2564 2062 7974 6573 2061 7420 6164  r %d bytes at ad
+000034e0: 6472 6573 7320 2570 0000 0000 2020 556e  dress %p....  Un
+000034f0: 6b6e 6f77 6e20 7073 6575 646f 2072 656c  known pseudo rel
+00003500: 6f63 6174 696f 6e20 7072 6f74 6f63 6f6c  ocation protocol
+00003510: 2076 6572 7369 6f6e 2025 642e 0a00 0000   version %d.....
+00003520: 2020 556e 6b6e 6f77 6e20 7073 6575 646f    Unknown pseudo
+00003530: 2072 656c 6f63 6174 696f 6e20 6269 7420   relocation bit 
+00003540: 7369 7a65 2025 642e 0a00 0000 2e00 676c  size %d.......gl
+00003550: 6f62 2d31 2e30 2d6d 696e 6777 3332 0000  ob-1.0-mingw32..
+00003560: 0000 2e00 0000 0000 4743 433a 2028 474e  ........GCC: (GN
+00003570: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
+00003580: 2028 474e 5529 2036 2e33 2e30 0000 0000   (GNU) 6.3.0....
+00003590: 4743 433a 2028 4d69 6e47 572e 6f72 6720  GCC: (MinGW.org 
+000035a0: 4743 432d 362e 332e 302d 3129 2036 2e33  GCC-6.3.0-1) 6.3
+000035b0: 2e30 0000 4743 433a 2028 474e 5529 2036  .0..GCC: (GNU) 6
+000035c0: 2e33 2e30 0000 0000 4743 433a 2028 474e  .3.0....GCC: (GN
+000035d0: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
+000035e0: 2028 474e 5529 2036 2e33 2e30 0000 0000   (GNU) 6.3.0....
+000035f0: 4743 433a 2028 474e 5529 2036 2e33 2e30  GCC: (GNU) 6.3.0
+00003600: 0000 0000 4743 433a 2028 474e 5529 2036  ....GCC: (GNU) 6
+00003610: 2e33 2e30 0000 0000 4743 433a 2028 474e  .3.0....GCC: (GN
+00003620: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
+00003630: 2028 474e 5529 2036 2e33 2e30 0000 0000   (GNU) 6.3.0....
+00003640: 4743 433a 2028 474e 5529 2036 2e33 2e30  GCC: (GNU) 6.3.0
+00003650: 0000 0000 4743 433a 2028 474e 5529 2036  ....GCC: (GNU) 6
+00003660: 2e33 2e30 0000 0000 4743 433a 2028 474e  .3.0....GCC: (GN
+00003670: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
+00003680: 2028 474e 5529 2036 2e33 2e30 0000 0000   (GNU) 6.3.0....
+00003690: 4743 433a 2028 474e 5529 2036 2e33 2e30  GCC: (GNU) 6.3.0
+000036a0: 0000 0000 4743 433a 2028 474e 5529 2036  ....GCC: (GNU) 6
+000036b0: 2e33 2e30 0000 0000 4743 433a 2028 474e  .3.0....GCC: (GN
+000036c0: 5529 2036 2e33 2e30 0000 0000 4743 433a  U) 6.3.0....GCC:
+000036d0: 2028 474e 5529 2036 2e33 2e30 0000 0000   (GNU) 6.3.0....
+000036e0: 4743 433a 2028 474e 5529 2036 2e33 2e30  GCC: (GNU) 6.3.0
+000036f0: 0000 0000 4743 433a 2028 474e 5529 2036  ....GCC: (GNU) 6
+00003700: 2e33 2e30 0000 0000 0000 0000 0000 0000  .3.0............
 00003710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -910,261 +910,261 @@
 000038d0: 2800 0000 1c00 0000 68b2 ffff e100 0000  (.......h.......
 000038e0: 0041 0e08 8502 420d 0545 8603 8304 02c2  .A....B..E......
 000038f0: 0ac3 41c6 41c5 0c04 0444 0b00 1c00 0000  ..A.A....D......
 00003900: 4800 0000 2cb3 ffff 2e00 0000 0041 0e08  H...,........A..
 00003910: 8502 420d 056a c50c 0404 0000 1400 0000  ..B..j..........
 00003920: 0000 0000 017a 5200 017c 0801 1b0c 0404  .....zR..|......
 00003930: 8801 0000 1c00 0000 1c00 0000 24b3 ffff  ............$...
-00003940: 4600 0000 0041 0e08 8502 420d 0502 40c5  F....A....B...@.
-00003950: 0c04 0400 3000 0000 3c00 0000 4ab3 ffff  ....0...<...J...
+00003940: 7b00 0000 0041 0e08 8502 420d 0502 75c5  {....A....B...u.
+00003950: 0c04 0400 3000 0000 3c00 0000 7fb3 ffff  ....0...<.......
 00003960: 7200 0000 0044 0c01 0047 1005 0275 0044  r....D...G...u.D
 00003970: 0f03 7578 0610 0302 757c 025d c10c 0100  ..ux....u|.]....
 00003980: 41c3 41c5 430c 0404 1400 0000 0000 0000  A.A.C...........
 00003990: 017a 5200 017c 0801 1b0c 0404 8801 0000  .zR..|..........
-000039a0: 3c00 0000 1c00 0000 78b3 ffff 9f03 0000  <.......x.......
+000039a0: 3c00 0000 1c00 0000 a8b3 ffff 9f03 0000  <...............
 000039b0: 0041 0e08 8502 420d 0546 8703 8604 8305  .A....B..F......
 000039c0: 032d 010a c341 c641 c741 c50c 0404 470b  .-...A.A.A....G.
 000039d0: 03c9 010a c341 c641 c741 c50c 0404 410b  .....A.A.A....A.
 000039e0: 1400 0000 0000 0000 017a 5200 017c 0801  .........zR..|..
 000039f0: 1b0c 0404 8801 0000 2400 0000 1c00 0000  ........$.......
-00003a00: c0b6 ffff 0701 0000 005d 0e08 8302 0248  .........].....H
+00003a00: f0b6 ffff 0701 0000 005d 0e08 8302 0248  .........].....H
 00003a10: 0c05 0c85 0302 41c5 0c04 0802 5fc3 0e04  ......A....._...
 00003a20: 1400 0000 0000 0000 017a 5200 017c 0801  .........zR..|..
 00003a30: 1b0c 0404 8801 0000 1400 0000 1c00 0000  ................
-00003a40: 90b7 ffff 2c00 0000 004e 0e10 5c0e 0400  ....,....N..\...
-00003a50: 2000 0000 3400 0000 a8b7 ffff 4600 0000   ...4.......F...
+00003a40: c0b7 ffff 2c00 0000 004e 0e10 5c0e 0400  ....,....N..\...
+00003a50: 2000 0000 3400 0000 d8b7 ffff 4600 0000   ...4.......F...
 00003a60: 0041 0e08 8302 430e 206a 0a0e 0841 c30e  .A....C. j...A..
-00003a70: 0441 0b00 1000 0000 5800 0000 d4b7 ffff  .A......X.......
+00003a70: 0441 0b00 1000 0000 5800 0000 04b8 ffff  .A......X.......
 00003a80: 1c00 0000 0000 0000 1400 0000 0000 0000  ................
 00003a90: 017a 5200 017c 0801 1b0c 0404 8801 0000  .zR..|..........
-00003aa0: 1c00 0000 1c00 0000 c8b7 ffff 4300 0000  ............C...
+00003aa0: 1c00 0000 1c00 0000 f8b7 ffff 4300 0000  ............C...
 00003ab0: 0043 0e20 550a 0e04 480b 600e 0400 0000  .C. U...H.`.....
-00003ac0: 3800 0000 3c00 0000 f8b7 ffff 8300 0000  8...<...........
+00003ac0: 3800 0000 3c00 0000 28b8 ffff 8300 0000  8...<...(.......
 00003ad0: 0041 0e08 8602 410e 0c83 0343 0e20 640a  .A....A....C. d.
 00003ae0: 0e0c 46c3 0e08 41c6 0e04 430b 680a 0e0c  ..F...A...C.h...
 00003af0: 46c3 0e08 41c6 0e04 430b 0000 1000 0000  F...A...C.......
-00003b00: 7800 0000 4cb8 ffff 0300 0000 0000 0000  x...L...........
+00003b00: 7800 0000 7cb8 ffff 0300 0000 0000 0000  x...|...........
 00003b10: 1400 0000 0000 0000 017a 5200 017c 0801  .........zR..|..
 00003b20: 1b0c 0404 8801 0000 3800 0000 1c00 0000  ........8.......
-00003b30: 30b8 ffff 6000 0000 0041 0e08 8602 410e  0...`....A....A.
+00003b30: 60b8 ffff 6000 0000 0041 0e08 8602 410e  `...`....A....A.
 00003b40: 0c83 0343 0e20 4c0e 1c49 0e20 500e 1c43  ...C. L..I. P..C
 00003b50: 0e20 6a0e 1c43 0e20 430e 0c41 c30e 0841  . j..C. C..A...A
-00003b60: c60e 0400 4400 0000 5800 0000 54b8 ffff  ....D...X...T...
+00003b60: c60e 0400 4400 0000 5800 0000 84b8 ffff  ....D...X.......
 00003b70: 8200 0000 0041 0e08 8602 410e 0c83 0345  .....A....A....E
 00003b80: 0e20 4c0a 0e0c 43c3 0e08 41c6 0e04 490b  . L...C...A...I.
 00003b90: 730e 1c48 0e20 550e 1c43 0e20 450a 0e0c  s..H. U..C. E...
 00003ba0: 41c3 0e08 41c6 0e04 410b 0000 3c00 0000  A...A...A...<...
-00003bb0: a000 0000 9cb8 ffff 9b00 0000 0041 0e08  .............A..
+00003bb0: a000 0000 ccb8 ffff 9b00 0000 0041 0e08  .............A..
 00003bc0: 8302 430e 2050 0a0e 0843 c30e 0449 0b4c  ..C. P...C...I.L
 00003bd0: 0e1c 490e 2067 0e1c 430e 2043 0a0e 0843  ..I. g..C. C...C
 00003be0: c30e 044b 0b5a 0e1c 430e 2000 2800 0000  ...K.Z..C. .(...
-00003bf0: e000 0000 fcb8 ffff 9700 0000 0043 0e20  .............C. 
+00003bf0: e000 0000 2cb9 ffff 9700 0000 0043 0e20  ....,........C. 
 00003c00: 610a 0e04 410b 690e 1c43 0e20 5d0a 0e04  a...A.i..C. ]...
 00003c10: 420b 4c0e 1c43 0e20 1400 0000 0000 0000  B.L..C. ........
 00003c20: 017a 5200 017c 0801 1b0c 0404 8801 0000  .zR..|..........
-00003c30: 1c00 0000 1c00 0000 58b9 ffff 4a00 0000  ........X...J...
+00003c30: 1c00 0000 1c00 0000 88b9 ffff 4a00 0000  ............J...
 00003c40: 0041 0e08 8602 410e 0c83 0343 0e20 0000  .A....A....C. ..
-00003c50: 6400 0000 3c00 0000 88b9 ffff f000 0000  d...<...........
+00003c50: 6400 0000 3c00 0000 b8b9 ffff f000 0000  d...<...........
 00003c60: 0041 0e08 8502 410e 0c87 0343 0e10 8604  .A....A....C....
 00003c70: 410e 1483 0547 0e60 580e 5443 0e60 690a  A....G.`X.TC.`i.
 00003c80: 0e14 41c3 0e10 41c6 0e0c 41c7 0e08 41c5  ..A...A...A...A.
 00003c90: 0e04 4b0b 640e 5043 0e60 0246 0e50 430e  ..K.d.PC.`.F.PC.
 00003ca0: 6043 0a0e 1441 c30e 1041 c60e 0c41 c70e  `C...A...A...A..
 00003cb0: 0841 c50e 0441 0b00 3400 0000 a400 0000  .A...A..4.......
-00003cc0: 10ba ffff cb01 0000 006a 0e08 8702 410e  .........j....A.
+00003cc0: 40ba ffff cb01 0000 006a 0e08 8702 410e  @........j....A.
 00003cd0: 0c86 0341 0e10 8304 430e 3002 e40a 0e10  ...A....C.0.....
 00003ce0: 41c3 0e0c 41c6 0e08 41c7 0e04 4a0b 0000  A...A...A...J...
 00003cf0: 1400 0000 0000 0000 017a 5200 017c 0801  .........zR..|..
 00003d00: 1b0c 0404 8801 0000 1800 0000 1c00 0000  ................
-00003d10: c0bb ffff 6c00 0000 0043 0e20 0241 0a0e  ....l....C. .A..
+00003d10: f0bb ffff 6c00 0000 0043 0e20 0241 0a0e  ....l....C. .A..
 00003d20: 0441 0b00 1400 0000 0000 0000 017a 5200  .A...........zR.
 00003d30: 017c 0801 1b0c 0404 8801 0000 3400 0000  .|..........4...
-00003d40: 1c00 0000 fcbb ffff 9300 0000 0049 0e08  .............I..
+00003d40: 1c00 0000 2cbc ffff 9300 0000 0049 0e08  ....,........I..
 00003d50: 8602 410e 0c83 0302 490a c30e 0841 c60e  ..A.....I....A..
 00003d60: 0441 0b73 c30e 0841 c60e 0446 0e0c 8303  .A.s...A...F....
-00003d70: 8602 0000 2800 0000 5400 0000 64bc ffff  ....(...T...d...
+00003d70: 8602 0000 2800 0000 5400 0000 94bc ffff  ....(...T.......
 00003d80: 6300 0000 0045 0e08 8602 410e 0c83 0345  c....E....A....E
 00003d90: 0e20 0248 0e0c 41c3 0e08 41c6 0e04 0000  . .H..A...A.....
-00003da0: 6c00 0000 8000 0000 a8bc ffff b502 0000  l...............
+00003da0: 6c00 0000 8000 0000 d8bc ffff b502 0000  l...............
 00003db0: 0041 0e08 8502 410e 0c87 0343 0e10 8604  .A....A....C....
 00003dc0: 410e 1483 0543 0e50 036e 010a 0e14 43c3  A....C.P.n....C.
 00003dd0: 0e10 41c6 0e0c 41c7 0e08 41c5 0e04 430b  ..A...A...A...C.
 00003de0: 024d 0a0e 1444 c30e 1041 c60e 0c41 c70e  .M...D...A...A..
 00003df0: 0841 c50e 0441 0b02 430a 0e14 44c3 0e10  .A...A..C...D...
 00003e00: 41c6 0e0c 41c7 0e08 41c5 0e04 410b 0000  A...A...A...A...
-00003e10: 5400 0000 f000 0000 f8be ffff 1a02 0000  T...............
+00003e10: 5400 0000 f000 0000 28bf ffff 1a02 0000  T.......(.......
 00003e20: 0041 0e08 8502 410e 0c87 0343 0e10 8604  .A....A....C....
 00003e30: 410e 1483 0543 0e40 02a0 0a0e 1441 c30e  A....C.@.....A..
 00003e40: 1041 c60e 0c41 c70e 0841 c50e 0443 0b02  .A...A...A...C..
 00003e50: 4b0a 0e14 41c3 0e10 41c6 0e0c 41c7 0e08  K...A...A...A...
 00003e60: 41c5 0e04 410b 0000 4400 0000 4801 0000  A...A...D...H...
-00003e70: c0c0 ffff 5c00 0000 0041 0e08 8702 410e  ....\....A....A.
+00003e70: f0c0 ffff 5c00 0000 0041 0e08 8702 410e  ....\....A....A.
 00003e80: 0c86 0343 0e10 8304 450e 2002 400a 0e10  ...C....E. .@...
 00003e90: 43c3 0e0c 41c6 0e08 41c7 0e04 410b 430e  C...A...A...A.C.
 00003ea0: 1046 c30e 0c41 c60e 0841 c70e 0400 0000  .F...A...A......
-00003eb0: 2800 0000 9001 0000 d8c0 ffff 4900 0000  (...........I...
+00003eb0: 2800 0000 9001 0000 08c1 ffff 4900 0000  (...........I...
 00003ec0: 0041 0e08 8602 410e 0c83 0347 0e20 6f0a  .A....A....G. o.
 00003ed0: 0e0c 41c3 0e08 41c6 0e04 460b 2c00 0000  ..A...A...F.,...
-00003ee0: bc01 0000 fcc0 ffff 8308 0000 0041 0e08  .............A..
+00003ee0: bc01 0000 2cc1 ffff 8308 0000 0041 0e08  ....,........A..
 00003ef0: 8502 420d 0543 8703 8604 8305 0364 030a  ..B..C.......d..
 00003f00: c341 c641 c741 c50c 0404 430b 2c00 0000  .A.A.A....C.,...
-00003f10: ec01 0000 5cc9 ffff e300 0000 0041 0e08  ....\........A..
+00003f10: ec01 0000 8cc9 ffff e300 0000 0041 0e08  .............A..
 00003f20: 8502 420d 0546 8703 8604 8305 0246 0ac3  ..B..F.......F..
 00003f30: 41c6 41c7 41c5 0c04 0441 0b00 4000 0000  A.A.A....A..@...
-00003f40: 1c02 0000 1cca ffff 5f00 0000 0041 0e08  ........_....A..
+00003f40: 1c02 0000 4cca ffff 5f00 0000 0041 0e08  ....L..._....A..
 00003f50: 8702 410e 0c86 0341 0e10 8304 430e 204f  ..A....A....C. O
 00003f60: 0a0e 1041 c30e 0c41 c60e 0841 c70e 0448  ...A...A...A...H
 00003f70: 0b77 0e10 41c3 0e0c 41c6 0e08 41c7 0e04  .w..A...A...A...
 00003f80: 1400 0000 0000 0000 017a 5200 017c 0801  .........zR..|..
 00003f90: 1b0c 0404 8801 0000 3c00 0000 1c00 0000  ........<.......
-00003fa0: 20ca ffff f403 0000 0041 0e08 8502 420d   ........A....B.
+00003fa0: 50ca ffff f403 0000 0041 0e08 8502 420d  P........A....B.
 00003fb0: 0546 8703 8604 8305 02b2 0ac3 43c6 41c7  .F..........C.A.
 00003fc0: 41c5 0c04 0441 0b03 5002 0ac3 41c6 41c7  A....A..P...A.A.
 00003fd0: 41c5 0c04 0441 0b00 1400 0000 0000 0000  A....A..........
 00003fe0: 017a 5200 017c 0801 1b0c 0404 8801 0000  .zR..|..........
-00003ff0: 4000 0000 1c00 0000 c8cd ffff cf00 0000  @...............
+00003ff0: 4000 0000 1c00 0000 f8cd ffff cf00 0000  @...............
 00004000: 0041 0e08 8602 410e 0c83 0348 0ee0 0250  .A....A....H...P
 00004010: 0ed8 0243 0ee0 0202 4c0a 0e0c 43c3 0e08  ...C....L...C...
 00004020: 41c6 0e04 430b 490a 0e0c 43c3 0e08 41c6  A...C.I...C...A.
-00004030: 0e04 410b 4c00 0000 6000 0000 54ce ffff  ..A.L...`...T...
+00004030: 0e04 410b 4c00 0000 6000 0000 84ce ffff  ..A.L...`.......
 00004040: a200 0000 0041 0e08 8602 410e 0c83 0348  .....A....A....H
 00004050: 0ee0 0250 0ed8 0243 0ee0 0202 470a 0e0c  ...P...C....G...
 00004060: 43c3 0e08 41c6 0e04 480b 4d0a 0e0c 43c3  C...A...H.M...C.
 00004070: 0e08 41c6 0e04 410b 5b0e 0c43 c30e 0841  ..A...A.[..C...A
-00004080: c60e 0400 4000 0000 b000 0000 b4ce ffff  ....@...........
+00004080: c60e 0400 4000 0000 b000 0000 e4ce ffff  ....@...........
 00004090: b701 0000 0041 0e08 8502 410e 0c87 0341  .....A....A....A
 000040a0: 0e10 8604 410e 1483 0546 0ec0 0203 4d01  ....A....F....M.
 000040b0: 0a0e 1443 c30e 1041 c60e 0c41 c70e 0841  ...C...A...A...A
 000040c0: c50e 0443 0b00 0000 2000 0000 f400 0000  ...C.... .......
-000040d0: 30d0 ffff 4600 0000 0041 0e08 8302 430e  0...F....A....C.
+000040d0: 60d0 ffff 4600 0000 0041 0e08 8302 430e  `...F....A....C.
 000040e0: 1071 0a0e 0841 c30e 0441 0b00 2800 0000  .q...A...A..(...
-000040f0: 1801 0000 5cd0 ffff 4200 0000 0041 0e08  ....\...B....A..
+000040f0: 1801 0000 8cd0 ffff 4200 0000 0041 0e08  ........B....A..
 00004100: 8302 430e 2056 0e1c 430e 2051 0a0e 0841  ..C. V..C. Q...A
 00004110: c30e 0441 0b00 0000 2c00 0000 4401 0000  ...A....,...D...
-00004120: 80d0 ffff 5800 0000 0041 0e08 8302 430e  ....X....A....C.
+00004120: b0d0 ffff 5800 0000 0041 0e08 8302 430e  ....X....A....C.
 00004130: 2056 0e1c 430e 2052 0a0e 0841 c30e 0441   V..C. R...A...A
 00004140: 0b65 0e08 41c3 0e04 1800 0000 7401 0000  .e..A.......t...
-00004150: b0d0 ffff 2700 0000 0043 0e10 510a 0e04  ....'....C..Q...
-00004160: 410b 0000 3400 0000 9001 0000 c4d0 ffff  A...4...........
+00004150: e0d0 ffff 2700 0000 0043 0e10 510a 0e04  ....'....C..Q...
+00004160: 410b 0000 3400 0000 9001 0000 f4d0 ffff  A...4...........
 00004170: 7100 0000 0041 0e08 8602 410e 0c83 0343  q....A....A....C
 00004180: 0e20 0252 0a0e 0c41 c30e 0841 c60e 0447  . .R...A...A...G
 00004190: 0b4e 0e0c 41c3 0e08 41c6 0e04 0000 0000  .N..A...A.......
 000041a0: 1400 0000 0000 0000 017a 5200 017c 0801  .........zR..|..
 000041b0: 1b0c 0404 8801 0000 1c00 0000 1c00 0000  ................
-000041c0: 70d2 ffff 0900 0000 0041 0e08 8502 420d  p........A....B.
+000041c0: c0d2 ffff 0900 0000 0041 0e08 8502 420d  .........A....B.
 000041d0: 0541 c50c 0404 0000 0000 0000 0000 0000  .A..............
 000041e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000041f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004200: 6480 0000 0000 0000 0000 0000 9485 0000  d...............
-00004210: 5081 0000 b080 0000 0000 0000 0000 0000  P...............
-00004220: ac85 0000 9c81 0000 bc80 0000 0000 0000  ................
-00004230: 0000 0000 3886 0000 a881 0000 4081 0000  ....8.......@...
-00004240: 0000 0000 0000 0000 5086 0000 2c82 0000  ........P...,...
+00004200: 6480 0000 0000 0000 0000 0000 d485 0000  d...............
+00004210: 5c81 0000 b080 0000 0000 0000 0000 0000  \...............
+00004220: ec85 0000 a881 0000 bc80 0000 0000 0000  ................
+00004230: 0000 0000 7c86 0000 b481 0000 4481 0000  ....|.......D...
+00004240: 0000 0000 0000 0000 9c86 0000 3c82 0000  ............<...
 00004250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004260: 0000 0000 3c82 0000 5482 0000 6c82 0000  ....<...T...l...
-00004270: 7a82 0000 8682 0000 9882 0000 a882 0000  z...............
-00004280: b682 0000 c882 0000 d882 0000 ec82 0000  ................
-00004290: fe82 0000 1a83 0000 3283 0000 4283 0000  ........2...B...
-000042a0: 6083 0000 6e83 0000 8083 0000 0000 0000  `...n...........
-000042b0: 9083 0000 9a83 0000 0000 0000 a683 0000  ................
-000042c0: b683 0000 c683 0000 d683 0000 e483 0000  ................
-000042d0: f683 0000 0084 0000 0a84 0000 1684 0000  ................
-000042e0: 2284 0000 2a84 0000 3684 0000 4084 0000  "...*...6...@...
-000042f0: 4a84 0000 5684 0000 5e84 0000 6884 0000  J...V...^...h...
-00004300: 7084 0000 7a84 0000 8284 0000 8c84 0000  p...z...........
-00004310: 9684 0000 a284 0000 ac84 0000 b684 0000  ................
-00004320: c084 0000 cc84 0000 d684 0000 e084 0000  ................
-00004330: ea84 0000 f484 0000 0085 0000 0000 0000  ................
-00004340: 0c85 0000 1a85 0000 3685 0000 0000 0000  ........6.......
-00004350: 3c82 0000 5482 0000 6c82 0000 7a82 0000  <...T...l...z...
-00004360: 8682 0000 9882 0000 a882 0000 b682 0000  ................
-00004370: c882 0000 d882 0000 ec82 0000 fe82 0000  ................
-00004380: 1a83 0000 3283 0000 4283 0000 6083 0000  ....2...B...`...
-00004390: 6e83 0000 8083 0000 0000 0000 9083 0000  n...............
-000043a0: 9a83 0000 0000 0000 a683 0000 b683 0000  ................
-000043b0: c683 0000 d683 0000 e483 0000 f683 0000  ................
-000043c0: 0084 0000 0a84 0000 1684 0000 2284 0000  ............"...
-000043d0: 2a84 0000 3684 0000 4084 0000 4a84 0000  *...6...@...J...
-000043e0: 5684 0000 5e84 0000 6884 0000 7084 0000  V...^...h...p...
-000043f0: 7a84 0000 8284 0000 8c84 0000 9684 0000  z...............
-00004400: a284 0000 ac84 0000 b684 0000 c084 0000  ................
-00004410: cc84 0000 d684 0000 e084 0000 ea84 0000  ................
-00004420: f484 0000 0085 0000 0000 0000 0c85 0000  ................
-00004430: 1a85 0000 3685 0000 0000 0000 cf00 4465  ....6.........De
-00004440: 6c65 7465 4372 6974 6963 616c 5365 6374  leteCriticalSect
-00004450: 696f 6e00 ec00 456e 7465 7243 7269 7469  ion...EnterCriti
-00004460: 6361 6c53 6563 7469 6f6e 0000 1701 4578  calSection....Ex
-00004470: 6974 5072 6f63 6573 7300 2c01 4669 6e64  itProcess.,.Find
-00004480: 436c 6f73 6500 3001 4669 6e64 4669 7273  Close.0.FindFirs
-00004490: 7446 696c 6541 0000 4101 4669 6e64 4e65  tFileA..A.FindNe
-000044a0: 7874 4669 6c65 4100 6001 4672 6565 4c69  xtFileA.`.FreeLi
-000044b0: 6272 6172 7900 8401 4765 7443 6f6d 6d61  brary...GetComma
-000044c0: 6e64 4c69 6e65 4100 fe01 4765 744c 6173  ndLineA...GetLas
-000044d0: 7445 7272 6f72 0000 1102 4765 744d 6f64  tError....GetMod
-000044e0: 756c 6548 616e 646c 6541 0000 4102 4765  uleHandleA..A.Ge
-000044f0: 7450 726f 6341 6464 7265 7373 0000 de02  tProcAddress....
-00004500: 496e 6974 6961 6c69 7a65 4372 6974 6963  InitializeCritic
-00004510: 616c 5365 6374 696f 6e00 2e03 4c65 6176  alSection...Leav
-00004520: 6543 7269 7469 6361 6c53 6563 7469 6f6e  eCriticalSection
-00004530: 0000 3103 4c6f 6164 4c69 6272 6172 7941  ..1.LoadLibraryA
-00004540: 0000 7404 5365 7455 6e68 616e 646c 6564  ..t.SetUnhandled
-00004550: 4578 6365 7074 696f 6e46 696c 7465 7200  ExceptionFilter.
-00004560: 9504 546c 7347 6574 5661 6c75 6500 bd04  ..TlsGetValue...
-00004570: 5669 7274 7561 6c50 726f 7465 6374 0000  VirtualProtect..
-00004580: bf04 5669 7274 7561 6c51 7565 7279 0000  ..VirtualQuery..
-00004590: 5000 5f73 7472 6475 7000 5200 5f73 7472  P._strdup.R._str
-000045a0: 6963 6f6c 6c00 5800 5f5f 6765 746d 6169  icoll.X.__getmai
-000045b0: 6e61 7267 7300 7700 5f5f 6d62 5f63 7572  nargs.w.__mb_cur
-000045c0: 5f6d 6178 0000 8300 5f5f 705f 5f65 6e76  _max....__p__env
-000045d0: 6972 6f6e 0000 8500 5f5f 705f 5f66 6d6f  iron....__p__fmo
-000045e0: 6465 0000 9900 5f5f 7365 745f 6170 705f  de....__set_app_
-000045f0: 7479 7065 0000 db00 5f63 6578 6974 0000  type...._cexit..
-00004600: 1d01 5f65 7272 6e6f 0000 4401 5f66 7072  .._errno..D._fpr
-00004610: 6573 6574 0000 5e01 5f66 756c 6c70 6174  eset..^._fullpat
-00004620: 6800 a101 5f69 6f62 0000 a601 5f69 7363  h..._iob...._isc
-00004630: 7479 7065 0000 b102 5f6f 6e65 7869 7400  type...._onexit.
-00004640: ba02 5f70 6374 7970 6500 f102 5f73 6574  .._pctype..._set
-00004650: 6d6f 6465 0000 3b04 6162 6f72 7400 4304  mode..;.abort.C.
-00004660: 6174 6578 6974 0000 4504 6174 6f69 0000  atexit..E.atoi..
-00004670: 4a04 6361 6c6c 6f63 0000 6b04 6672 6565  J.calloc..k.free
-00004680: 0000 7604 6677 7269 7465 0000 a304 6d61  ..v.fwrite....ma
-00004690: 6c6c 6f63 0000 aa04 6d62 7374 6f77 6373  lloc....mbstowcs
-000046a0: 0000 af04 6d65 6d63 7079 0000 b804 7072  ....memcpy....pr
-000046b0: 696e 7466 0000 c404 7265 616c 6c6f 6300  intf....realloc.
-000046c0: cb04 7365 746c 6f63 616c 6500 cd04 7369  ..setlocale...si
-000046d0: 676e 616c 0000 da04 7374 7263 6f6c 6c00  gnal....strcoll.
-000046e0: e104 7374 726c 656e 0000 fd04 746f 6c6f  ..strlen....tolo
-000046f0: 7765 7200 0405 7666 7072 696e 7466 0000  wer...vfprintf..
-00004700: 2d05 7763 7374 6f6d 6273 0000 cd00 456e  -.wcstombs....En
-00004710: 756d 5769 6e64 6f77 7300 6201 4765 7457  umWindows.b.GetW
-00004720: 696e 646f 7754 6872 6561 6450 726f 6365  indowThreadProce
-00004730: 7373 4964 0000 1602 5365 7446 6f72 6567  ssId....SetForeg
-00004740: 726f 756e 6457 696e 646f 7700 0080 0000  roundWindow.....
-00004750: 0080 0000 0080 0000 0080 0000 0080 0000  ................
-00004760: 0080 0000 0080 0000 0080 0000 0080 0000  ................
-00004770: 0080 0000 0080 0000 0080 0000 0080 0000  ................
-00004780: 0080 0000 0080 0000 0080 0000 0080 0000  ................
-00004790: 0080 0000 4b45 524e 454c 3332 2e64 6c6c  ....KERNEL32.dll
-000047a0: 0000 0000 1480 0000 1480 0000 6d73 7663  ............msvc
-000047b0: 7274 2e64 6c6c 0000 2880 0000 2880 0000  rt.dll..(...(...
-000047c0: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
-000047d0: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
-000047e0: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
-000047f0: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
+00004260: 0000 0000 5482 0000 6c82 0000 8482 0000  ....T...l.......
+00004270: 9282 0000 9e82 0000 b082 0000 c082 0000  ................
+00004280: ce82 0000 e082 0000 f082 0000 0483 0000  ................
+00004290: 1683 0000 3283 0000 4a83 0000 5a83 0000  ....2...J...Z...
+000042a0: 7883 0000 8683 0000 9883 0000 0000 0000  x...............
+000042b0: a883 0000 b283 0000 0000 0000 be83 0000  ................
+000042c0: ce83 0000 de83 0000 ee83 0000 fc83 0000  ................
+000042d0: 0e84 0000 1884 0000 2284 0000 2e84 0000  ........".......
+000042e0: 3a84 0000 4284 0000 4e84 0000 5884 0000  :...B...N...X...
+000042f0: 6284 0000 6e84 0000 7684 0000 8084 0000  b...n...v.......
+00004300: 8884 0000 9284 0000 9a84 0000 a484 0000  ................
+00004310: ae84 0000 ba84 0000 c484 0000 ce84 0000  ................
+00004320: d684 0000 e084 0000 ec84 0000 f684 0000  ................
+00004330: 0085 0000 0a85 0000 1485 0000 2085 0000  ............ ...
+00004340: 0000 0000 2c85 0000 3a85 0000 5685 0000  ....,...:...V...
+00004350: 6885 0000 7e85 0000 0000 0000 5482 0000  h...~.......T...
+00004360: 6c82 0000 8482 0000 9282 0000 9e82 0000  l...............
+00004370: b082 0000 c082 0000 ce82 0000 e082 0000  ................
+00004380: f082 0000 0483 0000 1683 0000 3283 0000  ............2...
+00004390: 4a83 0000 5a83 0000 7883 0000 8683 0000  J...Z...x.......
+000043a0: 9883 0000 0000 0000 a883 0000 b283 0000  ................
+000043b0: 0000 0000 be83 0000 ce83 0000 de83 0000  ................
+000043c0: ee83 0000 fc83 0000 0e84 0000 1884 0000  ................
+000043d0: 2284 0000 2e84 0000 3a84 0000 4284 0000  ".......:...B...
+000043e0: 4e84 0000 5884 0000 6284 0000 6e84 0000  N...X...b...n...
+000043f0: 7684 0000 8084 0000 8884 0000 9284 0000  v...............
+00004400: 9a84 0000 a484 0000 ae84 0000 ba84 0000  ................
+00004410: c484 0000 ce84 0000 d684 0000 e084 0000  ................
+00004420: ec84 0000 f684 0000 0085 0000 0a85 0000  ................
+00004430: 1485 0000 2085 0000 0000 0000 2c85 0000  .... .......,...
+00004440: 3a85 0000 5685 0000 6885 0000 7e85 0000  :...V...h...~...
+00004450: 0000 0000 cf00 4465 6c65 7465 4372 6974  ......DeleteCrit
+00004460: 6963 616c 5365 6374 696f 6e00 ec00 456e  icalSection...En
+00004470: 7465 7243 7269 7469 6361 6c53 6563 7469  terCriticalSecti
+00004480: 6f6e 0000 1701 4578 6974 5072 6f63 6573  on....ExitProces
+00004490: 7300 2c01 4669 6e64 436c 6f73 6500 3001  s.,.FindClose.0.
+000044a0: 4669 6e64 4669 7273 7446 696c 6541 0000  FindFirstFileA..
+000044b0: 4101 4669 6e64 4e65 7874 4669 6c65 4100  A.FindNextFileA.
+000044c0: 6001 4672 6565 4c69 6272 6172 7900 8401  `.FreeLibrary...
+000044d0: 4765 7443 6f6d 6d61 6e64 4c69 6e65 4100  GetCommandLineA.
+000044e0: fe01 4765 744c 6173 7445 7272 6f72 0000  ..GetLastError..
+000044f0: 1102 4765 744d 6f64 756c 6548 616e 646c  ..GetModuleHandl
+00004500: 6541 0000 4102 4765 7450 726f 6341 6464  eA..A.GetProcAdd
+00004510: 7265 7373 0000 de02 496e 6974 6961 6c69  ress....Initiali
+00004520: 7a65 4372 6974 6963 616c 5365 6374 696f  zeCriticalSectio
+00004530: 6e00 2e03 4c65 6176 6543 7269 7469 6361  n...LeaveCritica
+00004540: 6c53 6563 7469 6f6e 0000 3103 4c6f 6164  lSection..1.Load
+00004550: 4c69 6272 6172 7941 0000 7404 5365 7455  LibraryA..t.SetU
+00004560: 6e68 616e 646c 6564 4578 6365 7074 696f  nhandledExceptio
+00004570: 6e46 696c 7465 7200 9504 546c 7347 6574  nFilter...TlsGet
+00004580: 5661 6c75 6500 bd04 5669 7274 7561 6c50  Value...VirtualP
+00004590: 726f 7465 6374 0000 bf04 5669 7274 7561  rotect....Virtua
+000045a0: 6c51 7565 7279 0000 5000 5f73 7472 6475  lQuery..P._strdu
+000045b0: 7000 5200 5f73 7472 6963 6f6c 6c00 5800  p.R._stricoll.X.
+000045c0: 5f5f 6765 746d 6169 6e61 7267 7300 7700  __getmainargs.w.
+000045d0: 5f5f 6d62 5f63 7572 5f6d 6178 0000 8300  __mb_cur_max....
+000045e0: 5f5f 705f 5f65 6e76 6972 6f6e 0000 8500  __p__environ....
+000045f0: 5f5f 705f 5f66 6d6f 6465 0000 9900 5f5f  __p__fmode....__
+00004600: 7365 745f 6170 705f 7479 7065 0000 db00  set_app_type....
+00004610: 5f63 6578 6974 0000 1d01 5f65 7272 6e6f  _cexit...._errno
+00004620: 0000 4401 5f66 7072 6573 6574 0000 5e01  ..D._fpreset..^.
+00004630: 5f66 756c 6c70 6174 6800 a101 5f69 6f62  _fullpath..._iob
+00004640: 0000 a601 5f69 7363 7479 7065 0000 b102  ...._isctype....
+00004650: 5f6f 6e65 7869 7400 ba02 5f70 6374 7970  _onexit..._pctyp
+00004660: 6500 f102 5f73 6574 6d6f 6465 0000 3b04  e..._setmode..;.
+00004670: 6162 6f72 7400 4304 6174 6578 6974 0000  abort.C.atexit..
+00004680: 4504 6174 6f69 0000 4a04 6361 6c6c 6f63  E.atoi..J.calloc
+00004690: 0000 6b04 6672 6565 0000 7604 6677 7269  ..k.free..v.fwri
+000046a0: 7465 0000 a304 6d61 6c6c 6f63 0000 aa04  te....malloc....
+000046b0: 6d62 7374 6f77 6373 0000 af04 6d65 6d63  mbstowcs....memc
+000046c0: 7079 0000 b804 7072 696e 7466 0000 bc04  py....printf....
+000046d0: 7075 7473 0000 c404 7265 616c 6c6f 6300  puts....realloc.
+000046e0: cb04 7365 746c 6f63 616c 6500 cd04 7369  ..setlocale...si
+000046f0: 676e 616c 0000 da04 7374 7263 6f6c 6c00  gnal....strcoll.
+00004700: e104 7374 726c 656e 0000 fd04 746f 6c6f  ..strlen....tolo
+00004710: 7765 7200 0405 7666 7072 696e 7466 0000  wer...vfprintf..
+00004720: 2d05 7763 7374 6f6d 6273 0000 cd00 456e  -.wcstombs....En
+00004730: 756d 5769 6e64 6f77 7300 6201 4765 7457  umWindows.b.GetW
+00004740: 696e 646f 7754 6872 6561 6450 726f 6365  indowThreadProce
+00004750: 7373 4964 0000 8d01 4973 5769 6e64 6f77  ssId....IsWindow
+00004760: 5669 7369 626c 6500 1602 5365 7446 6f72  Visible...SetFor
+00004770: 6567 726f 756e 6457 696e 646f 7700 4902  egroundWindow.I.
+00004780: 5368 6f77 5769 6e64 6f77 0000 0080 0000  ShowWindow......
+00004790: 0080 0000 0080 0000 0080 0000 0080 0000  ................
+000047a0: 0080 0000 0080 0000 0080 0000 0080 0000  ................
+000047b0: 0080 0000 0080 0000 0080 0000 0080 0000  ................
+000047c0: 0080 0000 0080 0000 0080 0000 0080 0000  ................
+000047d0: 0080 0000 4b45 524e 454c 3332 2e64 6c6c  ....KERNEL32.dll
+000047e0: 0000 0000 1480 0000 1480 0000 6d73 7663  ............msvc
+000047f0: 7274 2e64 6c6c 0000 2880 0000 2880 0000  rt.dll..(...(...
 00004800: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
 00004810: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
 00004820: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
-00004830: 2880 0000 2880 0000 6d73 7663 7274 2e64  (...(...msvcrt.d
-00004840: 6c6c 0000 3c80 0000 3c80 0000 3c80 0000  ll..<...<...<...
-00004850: 5553 4552 3332 2e64 6c6c 0000 0000 0000  USER32.dll......
-00004860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000048a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004830: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
+00004840: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
+00004850: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
+00004860: 2880 0000 2880 0000 2880 0000 2880 0000  (...(...(...(...
+00004870: 2880 0000 2880 0000 2880 0000 6d73 7663  (...(...(...msvc
+00004880: 7274 2e64 6c6c 0000 3c80 0000 3c80 0000  rt.dll..<...<...
+00004890: 3c80 0000 3c80 0000 3c80 0000 5553 4552  <...<...<...USER
+000048a0: 3332 2e64 6c6c 0000 0000 0000 0000 0000  32.dll..........
 000048b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000048c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000048d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000048e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000048f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1178,15 +1178,15 @@
 00004990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000049a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000049b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000049c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000049d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000049e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000049f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a00: 0000 0000 c01a 4000 701a 4000 0000 0000  ......@.p.@.....
+00004a00: 0000 0000 f01a 4000 a01a 4000 0000 0000  ......@...@.....
 00004a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1243,15 +1243,15 @@
 00004da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004e00: 1c00 0000 0200 0000 0000 0400 0000 0000  ................
-00004e10: a020 4000 2a00 0000 0000 0000 0000 0000  . @.*...........
+00004e10: d020 4000 2a00 0000 0000 0000 0000 0000  . @.*...........
 00004e20: 1400 0000 0200 a700 0000 0400 0000 0000  ................
 00004e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1275,15 +1275,15 @@
 00004fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005000: a300 0000 0200 0000 0000 0401 0000 0000  ................
-00005010: a020 4000 ca20 4000 2e2e 2f2e 2e2f 2e2e  . @.. @.../../..
+00005010: d020 4000 fa20 4000 2e2e 2f2e 2e2f 2e2e  . @.. @.../../..
 00005020: 2f73 7263 2f67 6363 2d36 2e33 2e30 2f6c  /src/gcc-6.3.0/l
 00005030: 6962 6763 632f 636f 6e66 6967 2f69 3338  ibgcc/config/i38
 00005040: 362f 6379 6777 696e 2e53 002f 686f 6d65  6/cygwin.S./home
 00005050: 2f6b 6569 7468 2f73 7263 2f6d 696e 6777  /keith/src/mingw
 00005060: 2f67 6363 2d62 7569 6c64 2f67 6363 2d36  /gcc-build/gcc-6
 00005070: 2e33 2e30 2d6d 696e 6777 3332 2d63 726f  .3.0-mingw32-cro
 00005080: 7373 2d6e 6174 6976 652f 6d69 6e67 7733  ss-native/mingw3
@@ -1736,16 +1736,16 @@
 00006c70: 706f 7063 6f75 6e74 5f74 6162 0009 eb01  popcount_tab....
 00006c80: c11b 0000 0b5f 5f63 6c7a 5f74 6162 0009  .....__clz_tab..
 00006c90: f101 c11b 0000 0766 756e 635f 7074 7200  .......func_ptr.
 00006ca0: 0a2a ff1b 0000 0604 051c 0000 1708 ef1b  .*..............
 00006cb0: 0000 111c 0000 0900 0a5f 5f43 544f 525f  .........__CTOR_
 00006cc0: 4c49 5354 5f5f 000a 2f06 1c00 000a 5f5f  LIST__../.....__
 00006cd0: 4454 4f52 5f4c 4953 545f 5f00 0a30 061c  DTOR_LIST__..0..
-00006ce0: 0000 1811 1c00 000b 0e09 0503 403c 4000  ............@<@.
-00006cf0: 1826 1c00 000b 0f09 0503 4c3c 4000 0000  .&........L<@...
+00006ce0: 0000 1811 1c00 000b 0e09 0503 903c 4000  .............<@.
+00006cf0: 1826 1c00 000b 0f09 0503 9c3c 4000 0000  .&.........<@...
 00006d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1791,15 +1791,15 @@
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 6d00 0000 0200 4900 0000 0101 fb0e 0d00  m.....I.........
 00007010: 0101 0101 0000 0001 0000 012e 2e2f 2e2e  ............./..
 00007020: 2f2e 2e2f 7372 632f 6763 632d 362e 332e  /../src/gcc-6.3.
 00007030: 302f 6c69 6267 6363 2f63 6f6e 6669 672f  0/libgcc/config/
 00007040: 6933 3836 0000 6379 6777 696e 2e53 0001  i386..cygwin.S..
-00007050: 0000 0000 0502 a020 4000 03a2 0101 2222  ....... @.....""
+00007050: 0000 0000 0502 d020 4000 03a2 0101 2222  ....... @.....""
 00007060: 594b 3067 3d59 5930 2f3e 2222 0201 0001  YK0g=YY0/>""....
 00007070: 0153 0100 0002 004d 0100 0001 01fb 0e0d  .S.....M........
 00007080: 0001 0101 0100 0000 0100 0001 2f68 6f6d  ............/hom
 00007090: 652f 6b65 6974 682f 6d69 6e67 7733 322d  e/keith/mingw32-
 000070a0: 6763 632d 362e 332e 302f 696e 636c 7564  gcc-6.3.0/includ
 000070b0: 6500 2e2e 2f2e 2e2f 2e2e 2f73 7263 2f67  e.../../../src/g
 000070c0: 6363 2d36 2e33 2e30 2f6c 6962 6763 632f  cc-6.3.0/libgcc/
@@ -1819,15 +1819,15 @@
 000071a0: 6267 6363 322e 6800 0500 0067 626c 2d63  bgcc2.h....gbl-c
 000071b0: 746f 7273 2e68 0005 0000 6c69 6267 6363  tors.h....libgcc
 000071c0: 322e 6300 0500 0000 0000 0000 0000 0000  2.c.............
 000071d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000071e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000071f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007200: 1000 0000 ffff ffff 0100 017c 080c 0404  ...........|....
-00007210: 8801 0000 2000 0000 0000 0000 a020 4000  .... ........ @.
+00007210: 8801 0000 2000 0000 0000 0000 d020 4000  .... ........ @.
 00007220: 2a00 0000 410e 0881 0241 0e0c 8003 660e  *...A....A....f.
 00007230: 08c0 410e 04c1 0000 0000 0000 0000 0000  ..A.............
 00007240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1880,771 +1880,790 @@
 00007570: 0000 0000 0000 0000 0000 2e62 7373 0000  ...........bss..
 00007580: 0000 0800 0000 0500 0000 0301 1800 0000  ................
 00007590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000075a0: 0000 dc00 0000 b800 0000 0400 0000 0301  ................
 000075b0: 6400 0000 0200 0000 0000 0000 0000 0000  d...............
 000075c0: 0000 2e72 6461 7461 0000 0000 0000 0300  ...rdata........
 000075d0: 0000 0301 6300 0000 0000 0000 0000 0000  ....c...........
-000075e0: 0000 0000 0000 0000 0000 e600 0000 5801  ..............X.
+000075e0: 0000 0000 0000 0000 0000 e600 0000 7c01  ..............|.
 000075f0: 0000 0300 0000 0301 1100 0000 0000 0000  ................
 00007600: 0000 0000 0000 0000 0000 2e6a 6372 0000  ...........jcr..
 00007610: 0000 1800 0000 0200 0000 0300 2e66 696c  .............fil
 00007620: 6500 0000 6100 0000 feff 0000 6701 666f  e...a.......g.fo
 00007630: 6375 735f 7069 642e 6300 0000 0000 0000  cus_pid.c.......
 00007640: 0000 0000 f100 0000 6004 0000 0100 2000  ........`..... .
 00007650: 0201 0000 0000 0000 0000 0000 0000 0000  ................
-00007660: 0000 0000 5f6d 6169 6e00 0000 a604 0000  ...._main.......
+00007660: 0000 0000 5f6d 6169 6e00 0000 db04 0000  ...._main.......
 00007670: 0100 2000 0200 2e74 6578 7400 0000 6004  .. ....text...`.
-00007680: 0000 0100 0000 0301 b800 0000 0800 0000  ................
+00007680: 0000 0100 0000 0301 ed00 0000 0c00 0000  ................
 00007690: 0000 0000 0000 0000 0000 2e64 6174 6100  ...........data.
 000076a0: 0000 0400 0000 0200 0000 0301 0000 0000  ................
 000076b0: 0000 0000 0000 0000 0000 0000 0000 2e62  ...............b
 000076c0: 7373 0000 0000 2000 0000 0500 0000 0301  ss.... .........
 000076d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000076e0: 0000 2e72 6461 7461 0000 6400 0000 0300  ...rdata..d.....
-000076f0: 0000 0301 1100 0000 0000 0000 0000 0000  ................
-00007700: 0000 0000 0000 0000 0000 e600 0000 6c01  ..............l.
+000076f0: 0000 0301 3500 0000 0000 0000 0000 0000  ....5...........
+00007700: 0000 0000 0000 0000 0000 e600 0000 9001  ................
 00007710: 0000 0300 0000 0301 2300 0000 0000 0000  ........#.......
 00007720: 0000 0000 0000 0000 0000 0000 0000 dc00  ................
 00007730: 0000 1c01 0000 0400 0000 0301 6c00 0000  ............l...
 00007740: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00007750: 0000 0401 0000 2005 0000 0100 2000 0201  ...... ..... ...
+00007750: 0000 0401 0000 5005 0000 0100 2000 0201  ......P..... ...
 00007760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007770: 0000 2e74 6578 7400 0000 2005 0000 0100  ...text... .....
+00007770: 0000 2e74 6578 7400 0000 5005 0000 0100  ...text...P.....
 00007780: 0000 0301 9f03 0000 0f00 0000 0000 0000  ................
-00007790: 0000 0000 0000 0000 0000 0e01 0000 c008  ................
+00007790: 0000 0000 0000 0000 0000 0e01 0000 f008  ................
 000077a0: 0000 0100 2000 0201 0000 0000 0000 0000  .... ...........
 000077b0: 0000 0000 0000 0000 0000 2e74 6578 7400  ...........text.
-000077c0: 0000 c008 0000 0100 0000 0301 0701 0000  ................
+000077c0: 0000 f008 0000 0100 0000 0301 0701 0000  ................
 000077d0: 0200 0000 0000 0000 0000 0000 0000 2e62  ...............b
 000077e0: 7373 0000 0000 2400 0000 0500 0000 0301  ss....$.........
 000077f0: 0400 0000 0000 0000 0000 0000 0000 0000  ................
-00007800: 0000 0000 0000 2301 0000 d009 0000 0100  ......#.........
+00007800: 0000 0000 0000 2301 0000 000a 0000 0100  ......#.........
 00007810: 2000 0201 0000 0000 0000 0000 0000 0000   ...............
-00007820: 0000 0000 0000 0000 0000 3601 0000 000a  ..........6.....
+00007820: 0000 0000 0000 0000 0000 3601 0000 300a  ..........6...0.
 00007830: 0000 0100 2000 0200 5f5f 5f6d 6169 6e00  .... ...___main.
-00007840: 500a 0000 0100 2000 0200 2e74 6578 7400  P..... ....text.
-00007850: 0000 d009 0000 0100 0000 0301 9c00 0000  ................
+00007840: 800a 0000 0100 2000 0200 2e74 6578 7400  ...... ....text.
+00007850: 0000 000a 0000 0100 0000 0301 9c00 0000  ................
 00007860: 0a00 0000 0000 0000 0000 0000 0000 2e64  ...............d
 00007870: 6174 6100 0000 1000 0000 0200 0000 0301  ata.............
 00007880: 0400 0000 0100 0000 0000 0000 0000 0000  ................
 00007890: 0000 2e62 7373 0000 0000 2800 0000 0500  ...bss....(.....
 000078a0: 0000 0301 0400 0000 0000 0000 0000 0000  ................
-000078b0: 0000 0000 0000 0000 0000 4901 0000 c00a  ..........I.....
+000078b0: 0000 0000 0000 0000 0000 4901 0000 f00a  ..........I.....
 000078c0: 0000 0100 2000 0200 0000 0000 5c01 0000  .... .......\...
-000078d0: 500b 0000 0100 2000 0200 2e74 6578 7400  P..... ....text.
-000078e0: 0000 700a 0000 0100 0000 0301 e300 0000  ..p.............
+000078d0: 800b 0000 0100 2000 0200 2e74 6578 7400  ...... ....text.
+000078e0: 0000 a00a 0000 0100 0000 0301 e300 0000  ................
 000078f0: 0700 0000 0000 0000 0000 0000 0000 2e62  ...............b
 00007900: 7373 0000 0000 2c00 0000 0500 0000 0301  ss....,.........
 00007910: 1000 0000 0000 0000 0000 0000 0000 0000  ................
 00007920: 0000 2e43 5254 2458 445a 1400 0000 0700  ...CRT$XDZ......
 00007930: 0000 0301 0400 0000 0000 0000 0000 0000  ................
 00007940: 0000 0000 0000 2e43 5254 2458 4441 1000  .......CRT$XDA..
 00007950: 0000 0700 0000 0301 0400 0000 0000 0000  ................
 00007960: 0000 0000 0000 0000 0000 2e43 5254 2458  ...........CRT$X
 00007970: 4c41 0000 0000 0700 0000 0301 0400 0000  LA..............
 00007980: 0000 0000 0000 0000 0000 0000 0000 2e74  ...............t
 00007990: 6c73 245a 5a5a 1c00 0000 0800 0000 0301  ls$ZZZ..........
 000079a0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 000079b0: 0000 2e74 6c73 2441 4141 0000 0000 0800  ...tls$AAA......
 000079c0: 0000 0301 0100 0000 0000 0000 0000 0000  ................
-000079d0: 0000 0000 0000 0000 0000 6901 0000 c00b  ..........i.....
+000079d0: 0000 0000 0000 0000 0000 6901 0000 f00b  ..........i.....
 000079e0: 0000 0100 2000 0200 0000 0000 8701 0000  .... ...........
-000079f0: 500c 0000 0100 2000 0200 0000 0000 a801  P..... .........
-00007a00: 0000 f00c 0000 0100 2000 0200 2e74 6578  ........ ....tex
-00007a10: 7400 0000 600b 0000 0100 0000 0301 2702  t...`.........'.
+000079f0: 800c 0000 0100 2000 0200 0000 0000 a801  ...... .........
+00007a00: 0000 200d 0000 0100 2000 0200 2e74 6578  .. ..... ....tex
+00007a10: 7400 0000 900b 0000 0100 0000 0301 2702  t.............'.
 00007a20: 0000 2300 0000 0000 0000 0000 0000 0000  ..#.............
 00007a30: 2e62 7373 0000 0000 3c00 0000 0500 0000  .bss....<.......
 00007a40: 0301 2000 0000 0000 0000 0000 0000 0000  .. .............
-00007a50: 0000 0000 0000 0000 bd01 0000 d00e 0000  ................
-00007a60: 0100 2000 0200 2e74 6578 7400 0000 900d  .. ....text.....
+00007a50: 0000 0000 0000 0000 bd01 0000 000f 0000  ................
+00007a60: 0100 2000 0200 2e74 6578 7400 0000 c00d  .. ....text.....
 00007a70: 0000 0100 0000 0301 0b03 0000 2100 0000  ............!...
 00007a80: 0000 0000 0000 0000 0000 2e62 7373 0000  ...........bss..
 00007a90: 0000 5c00 0000 0500 0000 0301 0400 0000  ..\.............
 00007aa0: 0000 0000 0000 0000 0000 0000 0000 2e72  ...............r
-00007ab0: 6461 7461 0000 7c00 0000 0300 0000 0301  data..|.........
+00007ab0: 6461 7461 0000 a000 0000 0300 0000 0301  data............
 00007ac0: aa00 0000 0000 0000 0000 0000 0000 0000  ................
 00007ad0: 0000 2e66 696c 6500 0000 7300 0000 feff  ...file...s.....
 00007ae0: 0000 6701 6661 6b65 0000 0000 0000 0000  ..g.fake........
 00007af0: 0000 0000 0000 0000 0000 d801 0000 0000  ................
 00007b00: 0000 0a00 0000 0301 a700 0000 0400 0000  ................
 00007b10: 0000 0000 0000 0000 0000 0000 0000 e401  ................
 00007b20: 0000 0000 0000 0b00 0000 0301 1400 0000  ................
 00007b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007b40: 0000 f201 0000 0000 0000 0c00 0000 0301  ................
 00007b50: 7100 0000 0100 0000 0000 0000 0000 0000  q...............
-00007b60: 0000 2e74 6578 7400 0000 a010 0000 0100  ...text.........
+00007b60: 0000 2e74 6578 7400 0000 d010 0000 0100  ...text.........
 00007b70: 0000 0301 2a00 0000 0000 0000 0000 0000  ....*...........
 00007b80: 0000 0000 0000 2e64 6174 6100 0000 1400  .......data.....
 00007b90: 0000 0200 0000 0301 0000 0000 0000 0000  ................
 00007ba0: 0000 0000 0000 0000 0000 2e62 7373 0000  ...........bss..
 00007bb0: 0000 6800 0000 0500 0000 0301 0000 0000  ..h.............
 00007bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007bd0: 0000 fe01 0000 0000 0000 0900 0000 0301  ................
 00007be0: 2000 0000 0200 0000 0000 0000 0000 0000   ...............
 00007bf0: 0000 0000 0000 0d02 0000 0000 0000 0d00  ................
 00007c00: 0000 0301 3800 0000 0200 0000 0000 0000  ....8...........
-00007c10: 0000 0000 0000 2e66 696c 6500 0000 0e01  .......file.....
+00007c10: 0000 0000 0000 2e66 696c 6500 0000 1401  .......file.....
 00007c20: 0000 feff 0000 6701 6c69 6267 6363 322e  ......g.libgcc2.
 00007c30: 6300 0000 0000 0000 0000 2e74 6578 7400  c..........text.
-00007c40: 0000 cc10 0000 0100 0000 0301 0000 0000  ................
+00007c40: 0000 fc10 0000 0100 0000 0301 0000 0000  ................
 00007c50: 0000 0000 0000 0000 0000 0000 0000 2e64  ...............d
 00007c60: 6174 6100 0000 1400 0000 0200 0000 0301  ata.............
 00007c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007c80: 0000 2e62 7373 0000 0000 6800 0000 0500  ...bss....h.....
 00007c90: 0000 0301 0000 0000 0000 0000 0000 0000  ................
 00007ca0: 0000 0000 0000 0000 0000 d801 0000 a700  ................
 00007cb0: 0000 0a00 0000 0301 581c 0000 0400 0000  ........X.......
 00007cc0: 0000 0000 0000 0000 0000 0000 0000 e401  ................
 00007cd0: 0000 1400 0000 0b00 0000 0301 1b01 0000  ................
 00007ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007cf0: 0000 fe01 0000 2000 0000 0900 0000 0301  ...... .........
 00007d00: 1800 0000 0100 0000 0000 0000 0000 0000  ................
 00007d10: 0000 0000 0000 f201 0000 7100 0000 0c00  ..........q.....
 00007d20: 0000 0301 5701 0000 0000 0000 0000 0000  ....W...........
-00007d30: 0000 0000 0000 0000 0000 e600 0000 6c02  ..............l.
+00007d30: 0000 0000 0000 0000 0000 e600 0000 9002  ................
 00007d40: 0000 0300 0000 0301 1100 0000 0000 0000  ................
 00007d50: 0000 0000 0000 0000 0000 0000 0000 1a02  ................
-00007d60: 0000 d010 0000 0100 2000 0201 0000 0000  ........ .......
+00007d60: 0000 0011 0000 0100 2000 0201 0000 0000  ........ .......
 00007d70: 0000 0000 0000 0000 0000 0000 0000 2e74  ...............t
-00007d80: 6578 7400 0000 d010 0000 0100 0000 0301  ext.............
+00007d80: 6578 7400 0000 0011 0000 0100 0000 0301  ext.............
 00007d90: 6c00 0000 0500 0000 0000 0000 0000 0000  l...............
 00007da0: 0000 2e64 6174 6100 0000 1400 0000 0200  ...data.........
 00007db0: 0000 0301 0400 0000 0000 0000 0000 0000  ................
-00007dc0: 0000 0000 0000 0000 0000 2402 0000 7020  ..........$...p 
+00007dc0: 0000 0000 0000 0000 0000 2402 0000 a020  ..........$.... 
 00007dd0: 0000 0100 2000 0200 0000 0000 3202 0000  .... .......2...
-00007de0: 6021 0000 0100 2000 0200 2e74 6578 7400  `!.... ....text.
-00007df0: 0000 4011 0000 0100 0000 0301 7f10 0000  ..@.............
+00007de0: 9021 0000 0100 2000 0200 2e74 6578 7400  .!.... ....text.
+00007df0: 0000 7011 0000 0100 0000 0301 7f10 0000  ..p.............
 00007e00: 3400 0000 0000 0000 0000 0000 0000 2e72  4..............r
-00007e10: 6461 7461 0000 2801 0000 0300 0000 0301  data..(.........
+00007e10: 6461 7461 0000 4c01 0000 0300 0000 0301  data..L.........
 00007e20: 1300 0000 0000 0000 0000 0000 0000 0000  ................
-00007e30: 0000 0000 0000 4402 0000 c021 0000 0100  ......D....!....
+00007e30: 0000 0000 0000 4402 0000 f021 0000 0100  ......D....!....
 00007e40: 2000 0201 0000 0000 0000 0000 0000 0000   ...............
-00007e50: 0000 0000 0000 2e74 6578 7400 0000 c021  .......text....!
+00007e50: 0000 0000 0000 2e74 6578 7400 0000 f021  .......text....!
 00007e60: 0000 0100 0000 0301 f403 0000 1b00 0000  ................
 00007e70: 0000 0000 0000 0000 0000 2e62 7373 0000  ...........bss..
 00007e80: 0000 6800 0000 0500 0000 0301 0400 0000  ..h.............
 00007e90: 0000 0000 0000 0000 0000 0000 0000 2e72  ...............r
-00007ea0: 6461 7461 0000 3c01 0000 0300 0000 0301  data..<.........
+00007ea0: 6461 7461 0000 6001 0000 0300 0000 0301  data..`.........
 00007eb0: 0600 0000 0000 0000 0000 0000 0000 0000  ................
-00007ec0: 0000 0000 0000 5502 0000 4027 0000 0100  ......U...@'....
-00007ed0: 2000 0200 0000 0000 6602 0000 0029 0000   .......f....)..
-00007ee0: 0100 2000 0200 0000 0000 7702 0000 5029  .. .......w...P)
+00007ec0: 0000 0000 0000 5502 0000 7027 0000 0100  ......U...p'....
+00007ed0: 2000 0200 0000 0000 6602 0000 3029 0000   .......f...0)..
+00007ee0: 0100 2000 0200 0000 0000 7702 0000 8029  .. .......w....)
 00007ef0: 0000 0100 2000 0200 0000 0000 8902 0000  .... ...........
-00007f00: a029 0000 0100 2000 0200 0000 0000 9c02  .).... .........
-00007f10: 0000 002a 0000 0100 2000 0200 0000 0000  ...*.... .......
-00007f20: ad02 0000 302a 0000 0100 2000 0200 2e74  ....0*.... ....t
-00007f30: 6578 7400 0000 c025 0000 0100 0000 0301  ext....%........
+00007f00: d029 0000 0100 2000 0200 0000 0000 9c02  .).... .........
+00007f10: 0000 302a 0000 0100 2000 0200 0000 0000  ..0*.... .......
+00007f20: ad02 0000 602a 0000 0100 2000 0200 2e74  ....`*.... ....t
+00007f30: 6578 7400 0000 f025 0000 0100 0000 0301  ext....%........
 00007f40: e104 0000 1a00 0000 0000 0000 0000 0000  ................
-00007f50: 0000 2e69 6461 7461 2435 2402 0000 0600  ...idata$5$.....
-00007f60: 0000 0300 2e69 6461 7461 2436 0005 0000  .....idata$6....
-00007f70: 0600 0000 0300 2e69 6461 7461 2435 2002  .......idata$5 .
+00007f50: 0000 2e69 6461 7461 2435 3402 0000 0600  ...idata$54.....
+00007f60: 0000 0300 2e69 6461 7461 2436 2005 0000  .....idata$6 ...
+00007f70: 0600 0000 0300 2e69 6461 7461 2435 3002  .......idata$50.
 00007f80: 0000 0600 0000 0300 2e69 6461 7461 2436  .........idata$6
-00007f90: f404 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-00007fa0: 2435 1c02 0000 0600 0000 0300 2e69 6461  $5...........ida
-00007fb0: 7461 2436 ea04 0000 0600 0000 0300 2e69  ta$6...........i
-00007fc0: 6461 7461 2435 1802 0000 0600 0000 0300  data$5..........
-00007fd0: 2e69 6461 7461 2436 e004 0000 0600 0000  .idata$6........
-00007fe0: 0300 2e69 6461 7461 2435 1402 0000 0600  ...idata$5......
-00007ff0: 0000 0300 2e69 6461 7461 2436 d604 0000  .....idata$6....
-00008000: 0600 0000 0300 2e69 6461 7461 2435 1002  .......idata$5..
+00007f90: 1405 0000 0600 0000 0300 2e69 6461 7461  ...........idata
+00007fa0: 2435 2c02 0000 0600 0000 0300 2e69 6461  $5,..........ida
+00007fb0: 7461 2436 0a05 0000 0600 0000 0300 2e69  ta$6...........i
+00007fc0: 6461 7461 2435 2802 0000 0600 0000 0300  data$5(.........
+00007fd0: 2e69 6461 7461 2436 0005 0000 0600 0000  .idata$6........
+00007fe0: 0300 2e69 6461 7461 2435 2402 0000 0600  ...idata$5$.....
+00007ff0: 0000 0300 2e69 6461 7461 2436 f604 0000  .....idata$6....
+00008000: 0600 0000 0300 2e69 6461 7461 2435 2002  .......idata$5 .
 00008010: 0000 0600 0000 0300 2e69 6461 7461 2436  .........idata$6
-00008020: cc04 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-00008030: 2435 0c02 0000 0600 0000 0300 2e69 6461  $5...........ida
-00008040: 7461 2436 c004 0000 0600 0000 0300 2e69  ta$6...........i
-00008050: 6461 7461 2435 0802 0000 0600 0000 0300  data$5..........
-00008060: 2e69 6461 7461 2436 b604 0000 0600 0000  .idata$6........
-00008070: 0300 2e69 6461 7461 2435 0402 0000 0600  ...idata$5......
-00008080: 0000 0300 2e69 6461 7461 2436 ac04 0000  .....idata$6....
-00008090: 0600 0000 0300 2e69 6461 7461 2435 0002  .......idata$5..
+00008020: ec04 0000 0600 0000 0300 2e69 6461 7461  ...........idata
+00008030: 2435 1c02 0000 0600 0000 0300 2e69 6461  $5...........ida
+00008040: 7461 2436 e004 0000 0600 0000 0300 2e69  ta$6...........i
+00008050: 6461 7461 2435 1802 0000 0600 0000 0300  data$5..........
+00008060: 2e69 6461 7461 2436 d604 0000 0600 0000  .idata$6........
+00008070: 0300 2e69 6461 7461 2435 1402 0000 0600  ...idata$5......
+00008080: 0000 0300 2e69 6461 7461 2436 ce04 0000  .....idata$6....
+00008090: 0600 0000 0300 2e69 6461 7461 2435 1002  .......idata$5..
 000080a0: 0000 0600 0000 0300 2e69 6461 7461 2436  .........idata$6
-000080b0: a204 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-000080c0: 2435 fc01 0000 0600 0000 0300 2e69 6461  $5...........ida
-000080d0: 7461 2436 9604 0000 0600 0000 0300 2e69  ta$6...........i
-000080e0: 6461 7461 2435 f801 0000 0600 0000 0300  data$5..........
-000080f0: 2e69 6461 7461 2436 8c04 0000 0600 0000  .idata$6........
-00008100: 0300 2e69 6461 7461 2435 f401 0000 0600  ...idata$5......
-00008110: 0000 0300 2e69 6461 7461 2436 8204 0000  .....idata$6....
-00008120: 0600 0000 0300 2e69 6461 7461 2435 f001  .......idata$5..
+000080b0: c404 0000 0600 0000 0300 2e69 6461 7461  ...........idata
+000080c0: 2435 0c02 0000 0600 0000 0300 2e69 6461  $5...........ida
+000080d0: 7461 2436 ba04 0000 0600 0000 0300 2e69  ta$6...........i
+000080e0: 6461 7461 2435 0802 0000 0600 0000 0300  data$5..........
+000080f0: 2e69 6461 7461 2436 ae04 0000 0600 0000  .idata$6........
+00008100: 0300 2e69 6461 7461 2435 0402 0000 0600  ...idata$5......
+00008110: 0000 0300 2e69 6461 7461 2436 a404 0000  .....idata$6....
+00008120: 0600 0000 0300 2e69 6461 7461 2435 0002  .......idata$5..
 00008130: 0000 0600 0000 0300 2e69 6461 7461 2436  .........idata$6
-00008140: 7a04 0000 0600 0000 0300 2e69 6461 7461  z..........idata
-00008150: 2435 ec01 0000 0600 0000 0300 2e69 6461  $5...........ida
-00008160: 7461 2436 7004 0000 0600 0000 0300 2e69  ta$6p..........i
-00008170: 6461 7461 2435 e801 0000 0600 0000 0300  data$5..........
-00008180: 2e69 6461 7461 2436 6804 0000 0600 0000  .idata$6h.......
-00008190: 0300 2e69 6461 7461 2436 5e04 0000 0600  ...idata$6^.....
-000081a0: 0000 0300 2e69 6461 7461 2435 e001 0000  .....idata$5....
-000081b0: 0600 0000 0300 2e69 6461 7461 2436 5604  .......idata$6V.
+00008140: 9a04 0000 0600 0000 0300 2e69 6461 7461  ...........idata
+00008150: 2435 fc01 0000 0600 0000 0300 2e69 6461  $5...........ida
+00008160: 7461 2436 9204 0000 0600 0000 0300 2e69  ta$6...........i
+00008170: 6461 7461 2435 f801 0000 0600 0000 0300  data$5..........
+00008180: 2e69 6461 7461 2436 8804 0000 0600 0000  .idata$6........
+00008190: 0300 2e69 6461 7461 2435 f401 0000 0600  ...idata$5......
+000081a0: 0000 0300 2e69 6461 7461 2436 8004 0000  .....idata$6....
+000081b0: 0600 0000 0300 2e69 6461 7461 2436 7604  .......idata$6v.
 000081c0: 0000 0600 0000 0300 2e69 6461 7461 2435  .........idata$5
-000081d0: dc01 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-000081e0: 2436 4a04 0000 0600 0000 0300 2e69 6461  $6J..........ida
-000081f0: 7461 2436 4004 0000 0600 0000 0300 2e69  ta$6@..........i
-00008200: 6461 7461 2436 3604 0000 0600 0000 0300  data$66.........
-00008210: 2e69 6461 7461 2435 d001 0000 0600 0000  .idata$5........
-00008220: 0300 2e69 6461 7461 2436 2a04 0000 0600  ...idata$6*.....
-00008230: 0000 0300 2e69 6461 7461 2436 2204 0000  .....idata$6"...
-00008240: 0600 0000 0300 2e69 6461 7461 2435 c801  .......idata$5..
+000081d0: ec01 0000 0600 0000 0300 2e69 6461 7461  ...........idata
+000081e0: 2436 6e04 0000 0600 0000 0300 2e69 6461  $6n..........ida
+000081f0: 7461 2435 e801 0000 0600 0000 0300 2e69  ta$5...........i
+00008200: 6461 7461 2436 6204 0000 0600 0000 0300  data$6b.........
+00008210: 2e69 6461 7461 2436 5804 0000 0600 0000  .idata$6X.......
+00008220: 0300 2e69 6461 7461 2436 4e04 0000 0600  ...idata$6N.....
+00008230: 0000 0300 2e69 6461 7461 2435 dc01 0000  .....idata$5....
+00008240: 0600 0000 0300 2e69 6461 7461 2436 4204  .......idata$6B.
 00008250: 0000 0600 0000 0300 2e69 6461 7461 2436  .........idata$6
-00008260: 1604 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-00008270: 2435 c001 0000 0600 0000 0300 2e69 6461  $5...........ida
-00008280: 7461 2436 0004 0000 0600 0000 0300 2e69  ta$6...........i
-00008290: 6461 7461 2435 bc01 0000 0600 0000 0300  data$5..........
-000082a0: 2e69 6461 7461 2436 f603 0000 0600 0000  .idata$6........
-000082b0: 0300 2e69 6461 7461 2435 b401 0000 0600  ...idata$5......
-000082c0: 0000 0300 2e69 6461 7461 2436 d603 0000  .....idata$6....
-000082d0: 0600 0000 0300 2e69 6461 7461 2435 b001  .......idata$5..
+00008260: 3a04 0000 0600 0000 0300 2e69 6461 7461  :..........idata
+00008270: 2435 d401 0000 0600 0000 0300 2e69 6461  $5...........ida
+00008280: 7461 2436 2e04 0000 0600 0000 0300 2e69  ta$6...........i
+00008290: 6461 7461 2435 cc01 0000 0600 0000 0300  data$5..........
+000082a0: 2e69 6461 7461 2436 1804 0000 0600 0000  .idata$6........
+000082b0: 0300 2e69 6461 7461 2435 c801 0000 0600  ...idata$5......
+000082c0: 0000 0300 2e69 6461 7461 2436 0e04 0000  .....idata$6....
+000082d0: 0600 0000 0300 2e69 6461 7461 2435 c001  .......idata$5..
 000082e0: 0000 0600 0000 0300 2e69 6461 7461 2436  .........idata$6
-000082f0: c603 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-00008300: 2436 b603 0000 0600 0000 0300 2e69 6461  $6...........ida
-00008310: 7461 2435 a801 0000 0600 0000 0300 2e69  ta$5...........i
-00008320: 6461 7461 2436 a603 0000 0600 0000 0300  data$6..........
-00008330: 2e69 6461 7461 2434 bc00 0000 0600 0000  .idata$4........
-00008340: 0300 2e69 6461 7461 2435 a801 0000 0600  ...idata$5......
-00008350: 0000 0300 2e69 6461 7461 2435 3402 0000  .....idata$54...
-00008360: 0600 0000 0300 2e69 6461 7461 2436 3605  .......idata$66.
+000082f0: ee03 0000 0600 0000 0300 2e69 6461 7461  ...........idata
+00008300: 2435 bc01 0000 0600 0000 0300 2e69 6461  $5...........ida
+00008310: 7461 2436 de03 0000 0600 0000 0300 2e69  ta$6...........i
+00008320: 6461 7461 2436 ce03 0000 0600 0000 0300  data$6..........
+00008330: 2e69 6461 7461 2435 b401 0000 0600 0000  .idata$5........
+00008340: 0300 2e69 6461 7461 2436 be03 0000 0600  ...idata$6......
+00008350: 0000 0300 2e69 6461 7461 2434 bc00 0000  .....idata$4....
+00008360: 0600 0000 0300 2e69 6461 7461 2435 b401  .......idata$5..
 00008370: 0000 0600 0000 0300 2e69 6461 7461 2435  .........idata$5
-00008380: 3002 0000 0600 0000 0300 2e69 6461 7461  0..........idata
-00008390: 2436 1a05 0000 0600 0000 0300 2e69 6461  $6...........ida
-000083a0: 7461 2435 2c02 0000 0600 0000 0300 2e69  ta$5,..........i
-000083b0: 6461 7461 2436 0c05 0000 0600 0000 0300  data$6..........
-000083c0: 2e69 6461 7461 2434 4001 0000 0600 0000  .idata$4@.......
-000083d0: 0300 2e69 6461 7461 2435 2c02 0000 0600  ...idata$5,.....
-000083e0: 0000 0300 2e69 6461 7461 2435 9401 0000  .....idata$5....
-000083f0: 0600 0000 0300 2e69 6461 7461 2436 8003  .......idata$6..
+00008380: 4c02 0000 0600 0000 0300 2e69 6461 7461  L..........idata
+00008390: 2436 7e05 0000 0600 0000 0300 2e69 6461  $6~..........ida
+000083a0: 7461 2435 4802 0000 0600 0000 0300 2e69  ta$5H..........i
+000083b0: 6461 7461 2436 6805 0000 0600 0000 0300  data$6h.........
+000083c0: 2e69 6461 7461 2435 4402 0000 0600 0000  .idata$5D.......
+000083d0: 0300 2e69 6461 7461 2436 5605 0000 0600  ...idata$6V.....
+000083e0: 0000 0300 2e69 6461 7461 2435 4002 0000  .....idata$5@...
+000083f0: 0600 0000 0300 2e69 6461 7461 2436 3a05  .......idata$6:.
 00008400: 0000 0600 0000 0300 2e69 6461 7461 2435  .........idata$5
-00008410: 9001 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-00008420: 2436 6e03 0000 0600 0000 0300 2e69 6461  $6n..........ida
-00008430: 7461 2435 8c01 0000 0600 0000 0300 2e69  ta$5...........i
-00008440: 6461 7461 2436 6003 0000 0600 0000 0300  data$6`.........
-00008450: 2e69 6461 7461 2435 8801 0000 0600 0000  .idata$5........
-00008460: 0300 2e69 6461 7461 2436 4203 0000 0600  ...idata$6B.....
-00008470: 0000 0300 2e69 6461 7461 2435 8401 0000  .....idata$5....
-00008480: 0600 0000 0300 2e69 6461 7461 2436 3203  .......idata$62.
+00008410: 3c02 0000 0600 0000 0300 2e69 6461 7461  <..........idata
+00008420: 2436 2c05 0000 0600 0000 0300 2e69 6461  $6,..........ida
+00008430: 7461 2434 4401 0000 0600 0000 0300 2e69  ta$4D..........i
+00008440: 6461 7461 2435 3c02 0000 0600 0000 0300  data$5<.........
+00008450: 2e69 6461 7461 2435 a001 0000 0600 0000  .idata$5........
+00008460: 0300 2e69 6461 7461 2436 9803 0000 0600  ...idata$6......
+00008470: 0000 0300 2e69 6461 7461 2435 9c01 0000  .....idata$5....
+00008480: 0600 0000 0300 2e69 6461 7461 2436 8603  .......idata$6..
 00008490: 0000 0600 0000 0300 2e69 6461 7461 2435  .........idata$5
-000084a0: 8001 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-000084b0: 2436 1a03 0000 0600 0000 0300 2e69 6461  $6...........ida
-000084c0: 7461 2435 7c01 0000 0600 0000 0300 2e69  ta$5|..........i
-000084d0: 6461 7461 2436 fe02 0000 0600 0000 0300  data$6..........
-000084e0: 2e69 6461 7461 2435 7801 0000 0600 0000  .idata$5x.......
-000084f0: 0300 2e69 6461 7461 2436 ec02 0000 0600  ...idata$6......
-00008500: 0000 0300 2e69 6461 7461 2435 7401 0000  .....idata$5t...
-00008510: 0600 0000 0300 2e69 6461 7461 2436 d802  .......idata$6..
+000084a0: 9801 0000 0600 0000 0300 2e69 6461 7461  ...........idata
+000084b0: 2436 7803 0000 0600 0000 0300 2e69 6461  $6x..........ida
+000084c0: 7461 2435 9401 0000 0600 0000 0300 2e69  ta$5...........i
+000084d0: 6461 7461 2436 5a03 0000 0600 0000 0300  data$6Z.........
+000084e0: 2e69 6461 7461 2435 9001 0000 0600 0000  .idata$5........
+000084f0: 0300 2e69 6461 7461 2436 4a03 0000 0600  ...idata$6J.....
+00008500: 0000 0300 2e69 6461 7461 2435 8c01 0000  .....idata$5....
+00008510: 0600 0000 0300 2e69 6461 7461 2436 3203  .......idata$62.
 00008520: 0000 0600 0000 0300 2e69 6461 7461 2435  .........idata$5
-00008530: 7001 0000 0600 0000 0300 2e69 6461 7461  p..........idata
-00008540: 2436 c802 0000 0600 0000 0300 2e69 6461  $6...........ida
-00008550: 7461 2435 6c01 0000 0600 0000 0300 2e69  ta$5l..........i
-00008560: 6461 7461 2436 b602 0000 0600 0000 0300  data$6..........
-00008570: 2e69 6461 7461 2435 6801 0000 0600 0000  .idata$5h.......
-00008580: 0300 2e69 6461 7461 2436 a802 0000 0600  ...idata$6......
-00008590: 0000 0300 2e69 6461 7461 2435 6401 0000  .....idata$5d...
-000085a0: 0600 0000 0300 2e69 6461 7461 2436 9802  .......idata$6..
+00008530: 8801 0000 0600 0000 0300 2e69 6461 7461  ...........idata
+00008540: 2436 1603 0000 0600 0000 0300 2e69 6461  $6...........ida
+00008550: 7461 2435 8401 0000 0600 0000 0300 2e69  ta$5...........i
+00008560: 6461 7461 2436 0403 0000 0600 0000 0300  data$6..........
+00008570: 2e69 6461 7461 2435 8001 0000 0600 0000  .idata$5........
+00008580: 0300 2e69 6461 7461 2436 f002 0000 0600  ...idata$6......
+00008590: 0000 0300 2e69 6461 7461 2435 7c01 0000  .....idata$5|...
+000085a0: 0600 0000 0300 2e69 6461 7461 2436 e002  .......idata$6..
 000085b0: 0000 0600 0000 0300 2e69 6461 7461 2435  .........idata$5
-000085c0: 6001 0000 0600 0000 0300 2e69 6461 7461  `..........idata
-000085d0: 2436 8602 0000 0600 0000 0300 2e69 6461  $6...........ida
-000085e0: 7461 2435 5c01 0000 0600 0000 0300 2e69  ta$5\..........i
-000085f0: 6461 7461 2436 7a02 0000 0600 0000 0300  data$6z.........
-00008600: 2e69 6461 7461 2435 5801 0000 0600 0000  .idata$5X.......
-00008610: 0300 2e69 6461 7461 2436 6c02 0000 0600  ...idata$6l.....
-00008620: 0000 0300 2e69 6461 7461 2435 5401 0000  .....idata$5T...
-00008630: 0600 0000 0300 2e69 6461 7461 2436 5402  .......idata$6T.
+000085c0: 7801 0000 0600 0000 0300 2e69 6461 7461  x..........idata
+000085d0: 2436 ce02 0000 0600 0000 0300 2e69 6461  $6...........ida
+000085e0: 7461 2435 7401 0000 0600 0000 0300 2e69  ta$5t..........i
+000085f0: 6461 7461 2436 c002 0000 0600 0000 0300  data$6..........
+00008600: 2e69 6461 7461 2435 7001 0000 0600 0000  .idata$5p.......
+00008610: 0300 2e69 6461 7461 2436 b002 0000 0600  ...idata$6......
+00008620: 0000 0300 2e69 6461 7461 2435 6c01 0000  .....idata$5l...
+00008630: 0600 0000 0300 2e69 6461 7461 2436 9e02  .......idata$6..
 00008640: 0000 0600 0000 0300 2e69 6461 7461 2435  .........idata$5
-00008650: 5001 0000 0600 0000 0300 2e69 6461 7461  P..........idata
-00008660: 2436 3c02 0000 0600 0000 0300 2e69 6461  $6<..........ida
-00008670: 7461 2434 6400 0000 0600 0000 0300 2e69  ta$4d..........i
-00008680: 6461 7461 2435 5001 0000 0600 0000 0300  data$5P.........
-00008690: 2e69 6461 7461 2435 a001 0000 0600 0000  .idata$5........
-000086a0: 0300 2e69 6461 7461 2436 9a03 0000 0600  ...idata$6......
-000086b0: 0000 0300 2e69 6461 7461 2435 9c01 0000  .....idata$5....
-000086c0: 0600 0000 0300 2e69 6461 7461 2436 9003  .......idata$6..
+00008650: 6801 0000 0600 0000 0300 2e69 6461 7461  h..........idata
+00008660: 2436 9202 0000 0600 0000 0300 2e69 6461  $6...........ida
+00008670: 7461 2435 6401 0000 0600 0000 0300 2e69  ta$5d..........i
+00008680: 6461 7461 2436 8402 0000 0600 0000 0300  data$6..........
+00008690: 2e69 6461 7461 2435 6001 0000 0600 0000  .idata$5`.......
+000086a0: 0300 2e69 6461 7461 2436 6c02 0000 0600  ...idata$6l.....
+000086b0: 0000 0300 2e69 6461 7461 2435 5c01 0000  .....idata$5\...
+000086c0: 0600 0000 0300 2e69 6461 7461 2436 5402  .......idata$6T.
 000086d0: 0000 0600 0000 0300 2e69 6461 7461 2434  .........idata$4
-000086e0: b000 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-000086f0: 2435 9c01 0000 0600 0000 0300 2e66 696c  $5...........fil
-00008700: 6500 0000 2801 0000 feff 0000 6701 6379  e...(.......g.cy
-00008710: 676d 696e 672d 6372 7465 6e64 2e63 0000  gming-crtend.c..
-00008720: 0000 0000 be02 0000 9c09 0000 0400 0000  ................
-00008730: 0300 0000 0000 cd02 0000 1800 0000 0200  ................
-00008740: 0000 0300 0000 0000 da02 0000 302c 0000  ............0,..
-00008750: 0100 2000 0301 0000 0000 0000 0000 0000  .. .............
-00008760: 0000 0000 0000 0000 2e74 6578 7400 0000  .........text...
-00008770: 302c 0000 0100 0000 0301 0000 0000 0000  0,..............
-00008780: 0000 0000 0000 0000 0000 0000 2e64 6174  .............dat
-00008790: 6100 0000 1800 0000 0200 0000 0301 0000  a...............
-000087a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000087b0: 2e62 7373 0000 0000 6c00 0000 0500 0000  .bss....l.......
+000086e0: 6400 0000 0600 0000 0300 2e69 6461 7461  d..........idata
+000086f0: 2435 5c01 0000 0600 0000 0300 2e69 6461  $5\..........ida
+00008700: 7461 2435 ac01 0000 0600 0000 0300 2e69  ta$5...........i
+00008710: 6461 7461 2436 b203 0000 0600 0000 0300  data$6..........
+00008720: 2e69 6461 7461 2435 a801 0000 0600 0000  .idata$5........
+00008730: 0300 2e69 6461 7461 2436 a803 0000 0600  ...idata$6......
+00008740: 0000 0300 2e69 6461 7461 2434 b000 0000  .....idata$4....
+00008750: 0600 0000 0300 2e69 6461 7461 2435 a801  .......idata$5..
+00008760: 0000 0600 0000 0300 2e66 696c 6500 0000  .........file...
+00008770: 2e01 0000 feff 0000 6701 6379 676d 696e  ........g.cygmin
+00008780: 672d 6372 7465 6e64 2e63 0000 0000 0000  g-crtend.c......
+00008790: be02 0000 9c09 0000 0400 0000 0300 0000  ................
+000087a0: 0000 cd02 0000 1800 0000 0200 0000 0300  ................
+000087b0: 0000 0000 da02 0000 802c 0000 0100 2000  .........,.... .
 000087c0: 0301 0000 0000 0000 0000 0000 0000 0000  ................
-000087d0: 0000 0000 0000 0000 dc00 0000 9c09 0000  ................
-000087e0: 0400 0000 0301 3c00 0000 0100 0000 0000  ......<.........
-000087f0: 0000 0000 0000 0000 2e6a 6372 0000 0000  .........jcr....
-00008800: 1800 0000 0200 0000 0301 0400 0000 0000  ................
-00008810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008820: ef02 0000 302c 0000 0100 0000 0301 0900  ....0,..........
-00008830: 0000 0100 0000 0000 0000 0000 0000 0000  ................
-00008840: 0000 0000 fd02 0000 442c 0000 0100 0000  ........D,......
-00008850: 0301 0400 0000 0100 0000 0000 0000 0000  ................
-00008860: 0000 0000 0000 0000 e600 0000 d002 0000  ................
-00008870: 0300 0000 0301 1100 0000 0000 0000 0000  ................
-00008880: 0000 0000 0000 0000 2e69 6461 7461 2435  .........idata$5
-00008890: c401 0000 0600 0000 0300 2e69 6461 7461  ...........idata
-000088a0: 2436 0a04 0000 0600 0000 0300 2e69 6461  $6...........ida
-000088b0: 7461 2435 b801 0000 0600 0000 0300 2e69  ta$5...........i
-000088c0: 6461 7461 2436 e403 0000 0600 0000 0300  data$6..........
-000088d0: 0000 0000 0a03 0000 6001 0000 0600 0000  ........`.......
-000088e0: 0200 5f5f 6365 7869 7400 582b 0000 0100  ..__cexit.X+....
-000088f0: 2000 0200 0000 0000 2203 0000 982b 0000   ......."....+..
-00008900: 0100 2000 0200 0000 0000 3503 0000 e402  .. .......5.....
-00008910: 0000 0300 0000 0200 0000 0000 5403 0000  ............T...
-00008920: c801 0000 0600 0000 0200 0000 0000 6503  ..............e.
-00008930: 0000 f82b 0000 0100 2000 0200 0000 0000  ...+.... .......
-00008940: 7703 0000 dc01 0000 0600 0000 0200 0000  w...............
-00008950: 0000 8703 0000 0000 0000 0200 0000 0200  ................
-00008960: 0000 0000 9603 0000 e82b 0000 0100 2000  .........+.... .
-00008970: 0200 0000 0000 a503 0000 4c2c 0000 0100  ..........L,....
-00008980: 0000 0200 5f66 7265 6500 0000 182b 0000  ...._free....+..
-00008990: 0100 2000 0200 0000 0000 b403 0000 9001  .. .............
-000089a0: 0000 0600 0000 0200 0000 0000 cd03 0000  ................
-000089b0: d401 0000 0600 0000 0200 0000 0000 dc03  ................
-000089c0: 0000 602b 0000 0100 2000 0200 0000 0000  ..`+.... .......
-000089d0: e803 0000 7001 0000 0600 0000 0200 0000  ....p...........
-000089e0: 0000 fe03 0000 a82b 0000 0100 2000 0200  .......+.... ...
-000089f0: 0000 0000 1d04 0000 9401 0000 0600 0000  ................
-00008a00: 0200 0000 0000 3404 0000 6401 0000 0600  ......4...d.....
-00008a10: 0000 0200 0000 0000 4b04 0000 0000 0000  ........K.......
-00008a20: 0800 0000 0200 0000 0000 5a04 0000 882b  ..........Z....+
-00008a30: 0000 0100 2000 0200 0000 0000 6904 0000  .... .......i...
-00008a40: 8c01 0000 0600 0000 0200 0000 0000 7e04  ..............~.
-00008a50: 0000 3806 0000 0600 0000 0200 0000 0000  ..8.............
-00008a60: 9204 0000 7c01 0000 0600 0000 0200 5f5f  ....|.........__
-00008a70: 6572 726e 6f00 502b 0000 0100 2000 0200  errno.P+.... ...
-00008a80: 0000 0000 b504 0000 182c 0000 0100 2000  .........,.... .
-00008a90: 0200 0000 0000 ce04 0000 e402 0000 0300  ................
-00008aa0: 0000 0200 0000 0000 e204 0000 e001 0000  ................
-00008ab0: 0600 0000 0200 5f5f 5f78 6c5f 6300 0400  ......___xl_c...
-00008ac0: 0000 0700 0000 0200 0000 0000 ef04 0000  ................
-00008ad0: 0000 0000 ffff 0000 0200 0000 0000 0705  ................
-00008ae0: 0000 0010 0000 ffff 0000 0200 0000 0000  ................
-00008af0: 2005 0000 0000 2000 ffff 0000 0200 0000   ..... .........
-00008b00: 0000 3a05 0000 0400 0000 ffff 0000 0200  ..:.............
-00008b10: 0000 0000 5605 0000 0000 0000 0700 0000  ....V...........
-00008b20: 0200 0000 0000 6805 0000 0000 0000 0700  ......h.........
-00008b30: 0000 0200 0000 0000 7a05 0000 0000 0000  ........z.......
-00008b40: 0700 0000 0200 0000 0000 8a05 0000 a001  ................
-00008b50: 0000 0600 0000 0200 5f5f 5f78 6c5f 7a00  ........___xl_z.
-00008b60: 0c00 0000 0700 0000 0200 0000 0000 9a05  ................
-00008b70: 0000 ac01 0000 0600 0000 0200 0000 0000  ................
-00008b80: ae05 0000 d82b 0000 0100 2000 0200 0000  .....+.... .....
-00008b90: 0000 be05 0000 b001 0000 0600 0000 0200  ................
-00008ba0: 0000 0000 d205 0000 d801 0000 0600 0000  ................
-00008bb0: 0200 0000 0000 e105 0000 902b 0000 0100  ...........+....
-00008bc0: 2000 0200 0000 0000 f205 0000 3c00 0000   ...........<...
-00008bd0: 0600 0000 0200 0000 0000 0506 0000 3400  ..............4.
-00008be0: 0000 0500 0000 0200 0000 0000 1e06 0000  ................
-00008bf0: cc01 0000 0600 0000 0200 0000 0000 2a06  ..............*.
-00008c00: 0000 d02b 0000 0100 2000 0200 0000 0000  ...+.... .......
-00008c10: 3e06 0000 0000 0000 0000 2000 0201 1900  >......... .....
-00008c20: 0000 0100 0000 0000 0000 0000 0000 0000  ................
-00008c30: 0000 0000 5506 0000 ac05 0000 0600 0000  ....U...........
-00008c40: 0200 0000 0000 6b06 0000 6c00 0000 0500  ......k...l.....
-00008c50: 0000 0200 0000 0000 7806 0000 0000 0000  ........x.......
-00008c60: ffff 0000 0200 0000 0000 a906 0000 9c01  ................
-00008c70: 0000 0600 0000 0200 0000 0000 b706 0000  ................
-00008c80: d001 0000 0600 0000 0200 0000 0000 c706  ................
-00008c90: 0000 0000 0000 0500 0000 0200 0000 0000  ................
-00008ca0: d506 0000 e402 0000 0300 0000 0200 0000  ................
-00008cb0: 0000 f806 0000 0000 0000 ffff 0000 0200  ................
-00008cc0: 0000 0000 0207 0000 0010 0000 ffff 0000  ................
-00008cd0: 0200 0000 0000 1a07 0000 c001 0000 0600  ................
-00008ce0: 0000 0200 0000 0000 2807 0000 682b 0000  ........(...h+..
-00008cf0: 0100 2000 0200 0000 0000 3607 0000 7801  .. .......6...x.
-00008d00: 0000 0600 0000 0200 0000 0000 4e07 0000  ............N...
-00008d10: c82b 0000 0100 2000 0200 0000 0000 6007  .+.... .......`.
-00008d20: 0000 1000 0000 0700 0000 0200 0000 0000  ................
-00008d30: 7207 0000 2402 0000 0600 0000 0200 5f73  r...$........._s
-00008d40: 7472 636f 6c6c d02a 0000 0100 2000 0200  trcoll.*.... ...
-00008d50: 0000 0000 8207 0000 e02b 0000 0100 2000  .........+.... .
-00008d60: 0200 0000 0000 9507 0000 1000 0000 0700  ................
-00008d70: 0000 0200 0000 0000 a507 0000 1002 0000  ................
-00008d80: 0600 0000 0200 5f5f 646c 6c5f 5f00 0000  ......__dll__...
-00008d90: 0000 ffff 0000 0200 0000 0000 b307 0000  ................
-00008da0: 0000 0000 ffff 0000 0200 5f66 7772 6974  .........._fwrit
-00008db0: 6500 102b 0000 0100 2000 0200 0000 0000  e..+.... .......
-00008dc0: c807 0000 e401 0000 0600 0000 0200 0000  ................
-00008dd0: 0000 d607 0000 fc01 0000 0600 0000 0200  ................
-00008de0: 0000 0000 e607 0000 2800 0000 0600 0000  ........(.......
-00008df0: 0200 0000 0000 f907 0000 0000 4000 ffff  ............@...
-00008e00: 0000 0200 0000 0000 0808 0000 402b 0000  ............@+..
-00008e10: 0100 2000 0200 0000 0000 1208 0000 0010  .. .............
-00008e20: 0000 ffff 0000 0200 5f61 746f 6900 0000  ........_atoi...
-00008e30: 282b 0000 0100 2000 0200 0000 0000 2808  (+.... .......(.
-00008e40: 0000 b02b 0000 0100 2000 0200 0000 0000  ...+.... .......
-00008e50: 3808 0000 3002 0000 0600 0000 0200 0000  8...0...........
-00008e60: 0000 5a08 0000 b02a 0000 0100 2000 0200  ..Z....*.... ...
-00008e70: 0000 0000 6408 0000 6801 0000 0600 0000  ....d...h.......
-00008e80: 0200 5f6d 656d 6370 7900 f82a 0000 0100  .._memcpy..*....
-00008e90: 2000 0200 0000 0000 7908 0000 3c02 0000   .......y...<...
-00008ea0: 0600 0000 0200 0000 0000 8508 0000 1400  ................
-00008eb0: 0000 0600 0000 0200 0000 0000 9a08 0000  ................
-00008ec0: e402 0000 0300 0000 0200 0000 0000 b808  ................
-00008ed0: 0000 e02a 0000 0100 2000 0200 0000 0000  ...*.... .......
-00008ee0: c308 0000 b401 0000 0600 0000 0200 5f5f  ..............__
-00008ef0: 6172 6763 0000 0400 0000 0500 0000 0200  argc............
-00008f00: 0000 0000 d508 0000 0000 0000 0800 0000  ................
-00008f10: 0200 0000 0000 e108 0000 082c 0000 0100  ...........,....
-00008f20: 2000 0200 0000 0000 f008 0000 2c02 0000   ...........,...
-00008f30: 0600 0000 0200 0000 0000 0509 0000 1402  ................
-00008f40: 0000 0600 0000 0200 0000 0000 1409 0000  ................
-00008f50: 1c00 0000 0200 0000 0200 0000 0000 2109  ..............!.
-00008f60: 0000 702b 0000 0100 2000 0200 0000 0000  ..p+.... .......
-00008f70: 3009 0000 002c 0000 0100 2000 0200 5f74  0....,.... ..._t
-00008f80: 6f6c 6f77 6572 c02a 0000 0100 2000 0200  olower.*.... ...
-00008f90: 5f5f 5f78 6c5f 6100 0000 0000 0700 0000  ___xl_a.........
-00008fa0: 0200 5f5f 5f78 6c5f 6400 0800 0000 0700  ..___xl_d.......
-00008fb0: 0000 0200 0000 0000 3d09 0000 402c 0000  ........=...@,..
-00008fc0: 0100 0000 0200 0000 0000 4b09 0000 002b  ..........K....+
-00008fd0: 0000 0100 2000 0200 0000 0000 5509 0000  .... .......U...
-00008fe0: 0000 0000 ffff 0000 0200 5f5f 4352 545f  ..........__CRT_
-00008ff0: 4d54 6400 0000 0500 0000 0200 0000 0000  MTd.............
-00009000: 6509 0000 7000 0000 0500 0000 0200 0000  e...p...........
-00009010: 0000 7109 0000 2000 0000 0500 0000 0200  ..q... .........
-00009020: 0000 0000 7d09 0000 0000 0000 0700 0000  ....}...........
-00009030: 0200 0000 0000 8d09 0000 3800 0000 0500  ..........8.....
-00009040: 0000 0200 0000 0000 9909 0000 0000 0000  ................
-00009050: 0700 0000 0200 5f73 7472 6475 7000 282c  ......_strdup.(,
-00009060: 0000 0100 2000 0200 5f5f 6172 6776 0000  .... ...__argv..
-00009070: 0000 0000 0500 0000 0200 0000 0000 ab09  ................
-00009080: 0000 402c 0000 0100 0000 0200 5f63 616c  ..@,........_cal
-00009090: 6c6f 6300 202b 0000 0100 2000 0200 5f5f  loc. +.... ...__
-000090a0: 666d 6f64 6500 0c00 0000 0200 0000 0200  fmode...........
-000090b0: 0000 0000 ba09 0000 0000 0000 ffff 0000  ................
-000090c0: 0200 0000 0000 cd09 0000 0002 0000 0600  ................
-000090d0: 0000 0200 0000 0000 db09 0000 f02b 0000  .............+..
-000090e0: 0100 2000 0200 0000 0000 ec09 0000 0002  .. .............
-000090f0: 0000 ffff 0000 0200 0000 0000 ff09 0000  ................
-00009100: 8001 0000 0600 0000 0200 5f72 6561 6c6c  .........._reall
-00009110: 6f63 e82a 0000 0100 2000 0200 0000 0000  oc.*.... .......
-00009120: 1d0a 0000 e801 0000 0600 0000 0200 0000  ................
-00009130: 0000 290a 0000 f801 0000 0600 0000 0200  ..).............
-00009140: 0000 0000 370a 0000 b800 0000 0400 0000  ....7...........
-00009150: 0200 0000 0000 4b0a 0000 782b 0000 0100  ......K...x+....
-00009160: 2000 0200 0000 0000 620a 0000 0400 0000   .......b.......
-00009170: ffff 0000 0200 0000 0000 770a 0000 0802  ..........w.....
-00009180: 0000 0600 0000 0200 0000 0000 860a 0000  ................
-00009190: 5001 0000 0600 0000 0200 0000 0000 940a  P...............
-000091a0: 0000 202c 0000 0100 2000 0200 0000 0000  .. ,.... .......
-000091b0: 9e0a 0000 1c00 0000 0800 0000 0200 5f5f  ..............__
-000091c0: 656e 645f 5f00 0010 0000 0800 0000 0200  end__...........
-000091d0: 0000 0000 a80a 0000 7401 0000 0600 0000  ........t.......
-000091e0: 0200 5f73 6967 6e61 6c00 d82a 0000 0100  .._signal..*....
-000091f0: 2000 0200 5f6d 616c 6c6f 6300 082b 0000   ..._malloc..+..
-00009200: 0100 2000 0200 0000 0000 c20a 0000 4c2c  .. ...........L,
-00009210: 0000 0100 0000 0200 0000 0000 d00a 0000  ................
-00009220: c401 0000 0600 0000 0200 0000 0000 e00a  ................
-00009230: 0000 0000 0000 ffff 0000 0200 0000 0000  ................
-00009240: 130b 0000 102c 0000 0100 2000 0200 0000  .....,.... .....
-00009250: 0000 2b0b 0000 482b 0000 0100 2000 0200  ..+...H+.... ...
-00009260: 0000 0000 360b 0000 0000 1000 ffff 0000  ....6...........
-00009270: 0200 0000 0000 4f0b 0000 1000 0000 0700  ......O.........
-00009280: 0000 0200 0000 0000 610b 0000 0000 4000  ........a.....@.
-00009290: ffff 0000 0200 0000 0000 6e0b 0000 0300  ..........n.....
-000092a0: 0000 ffff 0000 0200 0000 0000 7c0b 0000  ............|...
-000092b0: 1802 0000 0600 0000 0200 0000 0000 8a0b  ................
-000092c0: 0000 0000 0000 ffff 0000 0200 0000 0000  ................
-000092d0: b90b 0000 0800 0000 0200 0000 0200 0000  ................
-000092e0: 0000 c40b 0000 ec01 0000 0600 0000 0200  ................
-000092f0: 5f61 626f 7274 0000 302b 0000 0100 2000  _abort..0+.... .
-00009300: 0200 0000 0000 d20b 0000 0000 0000 0000  ................
-00009310: 2000 0201 1b00 0000 0100 0000 0000 0000   ...............
-00009320: 0000 0000 0000 0000 0000 e70b 0000 802b  ...............+
-00009330: 0000 0100 2000 0200 0000 0000 030c 0000  .... ...........
-00009340: a801 0000 0600 0000 0200 0000 0000 180c  ................
-00009350: 0000 2000 0000 0800 0000 0200 0000 0000  .. .............
-00009360: 250c 0000 5801 0000 0600 0000 0200 0000  %...X...........
-00009370: 0000 3a0c 0000 2c00 0000 0500 0000 0200  ..:...,.........
-00009380: 0000 0000 520c 0000 c02b 0000 0100 2000  ....R....+.... .
-00009390: 0200 0000 0000 6f0c 0000 2400 0000 0500  ......o...$.....
-000093a0: 0000 0200 0000 0000 7f0c 0000 f001 0000  ................
-000093b0: 0600 0000 0200 0000 0000 8b0c 0000 8801  ................
-000093c0: 0000 0600 0000 0200 0000 0000 b00c 0000  ................
-000093d0: 0000 0000 0000 2000 0201 1a00 0000 0100  ...... .........
+000087d0: 0000 0000 2e74 6578 7400 0000 782c 0000  .....text...x,..
+000087e0: 0100 0000 0301 0000 0000 0000 0000 0000  ................
+000087f0: 0000 0000 0000 0000 2e64 6174 6100 0000  .........data...
+00008800: 1800 0000 0200 0000 0301 0000 0000 0000  ................
+00008810: 0000 0000 0000 0000 0000 0000 2e62 7373  .............bss
+00008820: 0000 0000 6c00 0000 0500 0000 0301 0000  ....l...........
+00008830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008840: 0000 0000 dc00 0000 9c09 0000 0400 0000  ................
+00008850: 0301 3c00 0000 0100 0000 0000 0000 0000  ..<.............
+00008860: 0000 0000 2e6a 6372 0000 0000 1800 0000  .....jcr........
+00008870: 0200 0000 0301 0400 0000 0000 0000 0000  ................
+00008880: 0000 0000 0000 0000 0000 0000 ef02 0000  ................
+00008890: 802c 0000 0100 0000 0301 0900 0000 0100  .,..............
+000088a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000088b0: fd02 0000 942c 0000 0100 0000 0301 0400  .....,..........
+000088c0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+000088d0: 0000 0000 e600 0000 f402 0000 0300 0000  ................
+000088e0: 0301 1100 0000 0000 0000 0000 0000 0000  ................
+000088f0: 0000 0000 2e69 6461 7461 2435 d001 0000  .....idata$5....
+00008900: 0600 0000 0300 2e69 6461 7461 2436 2204  .......idata$6".
+00008910: 0000 0600 0000 0300 2e69 6461 7461 2435  .........idata$5
+00008920: c401 0000 0600 0000 0300 2e69 6461 7461  ...........idata
+00008930: 2436 fc03 0000 0600 0000 0300 0000 0000  $6..............
+00008940: 0a03 0000 6c01 0000 0600 0000 0200 5f5f  ....l.........__
+00008950: 6365 7869 7400 902b 0000 0100 2000 0200  cexit..+.... ...
+00008960: 0000 0000 2203 0000 b02b 0000 0100 2000  ...."....+.... .
+00008970: 0200 0000 0000 3003 0000 e02b 0000 0100  ......0....+....
+00008980: 2000 0200 0000 0000 4303 0000 0803 0000   .......C.......
+00008990: 0300 0000 0200 0000 0000 6203 0000 d401  ..........b.....
+000089a0: 0000 0600 0000 0200 0000 0000 7303 0000  ............s...
+000089b0: 402c 0000 0100 2000 0200 0000 0000 8503  @,.... .........
+000089c0: 0000 e801 0000 0600 0000 0200 0000 0000  ................
+000089d0: 9503 0000 0000 0000 0200 0000 0200 0000  ................
+000089e0: 0000 a403 0000 302c 0000 0100 2000 0200  ......0,.... ...
+000089f0: 0000 0000 b303 0000 9c2c 0000 0100 0000  .........,......
+00008a00: 0200 5f66 7265 6500 0000 502b 0000 0100  .._free...P+....
+00008a10: 2000 0200 0000 0000 c203 0000 9c01 0000   ...............
+00008a20: 0600 0000 0200 0000 0000 db03 0000 e001  ................
+00008a30: 0000 0600 0000 0200 0000 0000 ea03 0000  ................
+00008a40: 982b 0000 0100 2000 0200 0000 0000 f603  .+.... .........
+00008a50: 0000 7c01 0000 0600 0000 0200 0000 0000  ..|.............
+00008a60: 0c04 0000 f02b 0000 0100 2000 0200 0000  .....+.... .....
+00008a70: 0000 2b04 0000 a001 0000 0600 0000 0200  ..+.............
+00008a80: 0000 0000 4204 0000 7001 0000 0600 0000  ....B...p.......
+00008a90: 0200 0000 0000 5904 0000 0000 0000 0800  ......Y.........
+00008aa0: 0000 0200 0000 0000 6804 0000 d02b 0000  ........h....+..
+00008ab0: 0100 2000 0200 0000 0000 7704 0000 9801  .. .......w.....
+00008ac0: 0000 0600 0000 0200 0000 0000 8c04 0000  ................
+00008ad0: 7c06 0000 0600 0000 0200 0000 0000 a004  |...............
+00008ae0: 0000 8801 0000 0600 0000 0200 5f5f 6572  ............__er
+00008af0: 726e 6f00 882b 0000 0100 2000 0200 0000  rno..+.... .....
+00008b00: 0000 c304 0000 602c 0000 0100 2000 0200  ......`,.... ...
+00008b10: 0000 0000 dc04 0000 0803 0000 0300 0000  ................
+00008b20: 0200 0000 0000 f004 0000 ec01 0000 0600  ................
+00008b30: 0000 0200 5f5f 5f78 6c5f 6300 0400 0000  ....___xl_c.....
+00008b40: 0700 0000 0200 0000 0000 fd04 0000 0000  ................
+00008b50: 0000 ffff 0000 0200 0000 0000 1505 0000  ................
+00008b60: 0010 0000 ffff 0000 0200 0000 0000 2e05  ................
+00008b70: 0000 0000 2000 ffff 0000 0200 0000 0000  .... ...........
+00008b80: 4805 0000 0400 0000 ffff 0000 0200 0000  H...............
+00008b90: 0000 6405 0000 0000 0000 0700 0000 0200  ..d.............
+00008ba0: 0000 0000 7605 0000 0000 0000 0700 0000  ....v...........
+00008bb0: 0200 0000 0000 8805 0000 0000 0000 0700  ................
+00008bc0: 0000 0200 0000 0000 9805 0000 ac01 0000  ................
+00008bd0: 0600 0000 0200 5f5f 5f78 6c5f 7a00 0c00  ......___xl_z...
+00008be0: 0000 0700 0000 0200 0000 0000 a805 0000  ................
+00008bf0: b801 0000 0600 0000 0200 0000 0000 bc05  ................
+00008c00: 0000 202c 0000 0100 2000 0200 5f70 7574  .. ,.... ..._put
+00008c10: 7300 0000 202b 0000 0100 2000 0200 0000  s... +.... .....
+00008c20: 0000 cc05 0000 bc01 0000 0600 0000 0200  ................
+00008c30: 0000 0000 e005 0000 e401 0000 0600 0000  ................
+00008c40: 0200 0000 0000 ef05 0000 d82b 0000 0100  ...........+....
+00008c50: 2000 0200 0000 0000 0006 0000 3c00 0000   ...........<...
+00008c60: 0600 0000 0200 0000 0000 1306 0000 3400  ..............4.
+00008c70: 0000 0500 0000 0200 0000 0000 2c06 0000  ............,...
+00008c80: d801 0000 0600 0000 0200 0000 0000 3806  ..............8.
+00008c90: 0000 182c 0000 0100 2000 0200 0000 0000  ...,.... .......
+00008ca0: 4c06 0000 0000 0000 0000 2000 0201 1900  L......... .....
+00008cb0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+00008cc0: 0000 0000 6306 0000 ec05 0000 0600 0000  ....c...........
+00008cd0: 0200 0000 0000 7906 0000 6c00 0000 0500  ......y...l.....
+00008ce0: 0000 0200 0000 0000 8606 0000 0000 0000  ................
+00008cf0: ffff 0000 0200 0000 0000 b706 0000 a801  ................
+00008d00: 0000 0600 0000 0200 0000 0000 c506 0000  ................
+00008d10: dc01 0000 0600 0000 0200 0000 0000 d506  ................
+00008d20: 0000 0000 0000 0500 0000 0200 0000 0000  ................
+00008d30: e306 0000 0803 0000 0300 0000 0200 0000  ................
+00008d40: 0000 0607 0000 0000 0000 ffff 0000 0200  ................
+00008d50: 0000 0000 1007 0000 0010 0000 ffff 0000  ................
+00008d60: 0200 0000 0000 2807 0000 cc01 0000 0600  ......(.........
+00008d70: 0000 0200 0000 0000 3607 0000 a02b 0000  ........6....+..
+00008d80: 0100 2000 0200 0000 0000 4407 0000 8401  .. .......D.....
+00008d90: 0000 0600 0000 0200 0000 0000 5c07 0000  ............\...
+00008da0: 102c 0000 0100 2000 0200 0000 0000 6e07  .,.... .......n.
+00008db0: 0000 1000 0000 0700 0000 0200 0000 0000  ................
+00008dc0: 8007 0000 3402 0000 0600 0000 0200 5f73  ....4........._s
+00008dd0: 7472 636f 6c6c 002b 0000 0100 2000 0200  trcoll.+.... ...
+00008de0: 0000 0000 9007 0000 282c 0000 0100 2000  ........(,.... .
+00008df0: 0200 0000 0000 a307 0000 4402 0000 0600  ..........D.....
+00008e00: 0000 0200 0000 0000 bc07 0000 1000 0000  ................
+00008e10: 0700 0000 0200 0000 0000 cc07 0000 2002  .............. .
+00008e20: 0000 0600 0000 0200 5f5f 646c 6c5f 5f00  ........__dll__.
+00008e30: 0000 0000 ffff 0000 0200 0000 0000 da07  ................
+00008e40: 0000 1402 0000 0600 0000 0200 0000 0000  ................
+00008e50: e607 0000 0000 0000 ffff 0000 0200 5f66  .............._f
+00008e60: 7772 6974 6500 482b 0000 0100 2000 0200  write.H+.... ...
+00008e70: 0000 0000 fb07 0000 f001 0000 0600 0000  ................
+00008e80: 0200 0000 0000 0908 0000 0802 0000 0600  ................
+00008e90: 0000 0200 0000 0000 1908 0000 c02b 0000  .............+..
+00008ea0: 0100 2000 0200 0000 0000 2c08 0000 2800  .. .......,...(.
+00008eb0: 0000 0600 0000 0200 0000 0000 3f08 0000  ............?...
+00008ec0: 0000 4000 ffff 0000 0200 0000 0000 4e08  ..@...........N.
+00008ed0: 0000 782b 0000 0100 2000 0200 0000 0000  ..x+.... .......
+00008ee0: 5808 0000 0010 0000 ffff 0000 0200 5f61  X............._a
+00008ef0: 746f 6900 0000 602b 0000 0100 2000 0200  toi...`+.... ...
+00008f00: 0000 0000 6e08 0000 f82b 0000 0100 2000  ....n....+.... .
+00008f10: 0200 0000 0000 7e08 0000 4002 0000 0600  ......~...@.....
+00008f20: 0000 0200 0000 0000 a008 0000 e02a 0000  .............*..
+00008f30: 0100 2000 0200 0000 0000 aa08 0000 7401  .. ...........t.
+00008f40: 0000 0600 0000 0200 5f6d 656d 6370 7900  ........_memcpy.
+00008f50: 302b 0000 0100 2000 0200 0000 0000 bf08  0+.... .........
+00008f60: 0000 5402 0000 0600 0000 0200 0000 0000  ..T.............
+00008f70: cb08 0000 1400 0000 0600 0000 0200 0000  ................
+00008f80: 0000 e008 0000 0803 0000 0300 0000 0200  ................
+00008f90: 0000 0000 fe08 0000 102b 0000 0100 2000  .........+.... .
+00008fa0: 0200 0000 0000 0909 0000 c001 0000 0600  ................
+00008fb0: 0000 0200 5f5f 6172 6763 0000 0400 0000  ....__argc......
+00008fc0: 0500 0000 0200 0000 0000 1b09 0000 0000  ................
+00008fd0: 0000 0800 0000 0200 0000 0000 2709 0000  ............'...
+00008fe0: 502c 0000 0100 2000 0200 0000 0000 3609  P,.... .......6.
+00008ff0: 0000 3c02 0000 0600 0000 0200 0000 0000  ..<.............
+00009000: 4b09 0000 2402 0000 0600 0000 0200 0000  K...$...........
+00009010: 0000 5a09 0000 1c00 0000 0200 0000 0200  ..Z.............
+00009020: 0000 0000 6709 0000 a82b 0000 0100 2000  ....g....+.... .
+00009030: 0200 0000 0000 7609 0000 482c 0000 0100  ......v...H,....
+00009040: 2000 0200 5f74 6f6c 6f77 6572 f02a 0000   ..._tolower.*..
+00009050: 0100 2000 0200 5f5f 5f78 6c5f 6100 0000  .. ...___xl_a...
+00009060: 0000 0700 0000 0200 5f5f 5f78 6c5f 6400  ........___xl_d.
+00009070: 0800 0000 0700 0000 0200 0000 0000 8309  ................
+00009080: 0000 902c 0000 0100 0000 0200 0000 0000  ...,............
+00009090: 9109 0000 382b 0000 0100 2000 0200 0000  ....8+.... .....
+000090a0: 0000 9b09 0000 0000 0000 ffff 0000 0200  ................
+000090b0: 5f5f 4352 545f 4d54 6400 0000 0500 0000  __CRT_MTd.......
+000090c0: 0200 0000 0000 ab09 0000 7000 0000 0500  ..........p.....
+000090d0: 0000 0200 0000 0000 b709 0000 2000 0000  ............ ...
+000090e0: 0500 0000 0200 0000 0000 c309 0000 0000  ................
+000090f0: 0000 0700 0000 0200 0000 0000 d309 0000  ................
+00009100: 3800 0000 0500 0000 0200 0000 0000 df09  8...............
+00009110: 0000 0000 0000 0700 0000 0200 5f73 7472  ............_str
+00009120: 6475 7000 702c 0000 0100 2000 0200 5f5f  dup.p,.... ...__
+00009130: 6172 6776 0000 0000 0000 0500 0000 0200  argv............
+00009140: 0000 0000 f109 0000 902c 0000 0100 0000  .........,......
+00009150: 0200 5f63 616c 6c6f 6300 582b 0000 0100  .._calloc.X+....
+00009160: 2000 0200 5f5f 666d 6f64 6500 0c00 0000   ...__fmode.....
+00009170: 0200 0000 0200 0000 0000 000a 0000 0000  ................
+00009180: 0000 ffff 0000 0200 0000 0000 130a 0000  ................
+00009190: 0c02 0000 0600 0000 0200 0000 0000 210a  ..............!.
+000091a0: 0000 382c 0000 0100 2000 0200 0000 0000  ..8,.... .......
+000091b0: 320a 0000 0002 0000 ffff 0000 0200 0000  2...............
+000091c0: 0000 450a 0000 8c01 0000 0600 0000 0200  ..E.............
+000091d0: 5f72 6561 6c6c 6f63 182b 0000 0100 2000  _realloc.+.... .
+000091e0: 0200 0000 0000 630a 0000 f401 0000 0600  ......c.........
+000091f0: 0000 0200 0000 0000 6f0a 0000 0402 0000  ........o.......
+00009200: 0600 0000 0200 0000 0000 7d0a 0000 b800  ..........}.....
+00009210: 0000 0400 0000 0200 0000 0000 910a 0000  ................
+00009220: b82b 0000 0100 2000 0200 0000 0000 a80a  .+.... .........
+00009230: 0000 0400 0000 ffff 0000 0200 0000 0000  ................
+00009240: bd0a 0000 1802 0000 0600 0000 0200 0000  ................
+00009250: 0000 cc0a 0000 5c01 0000 0600 0000 0200  ......\.........
+00009260: 0000 0000 da0a 0000 682c 0000 0100 2000  ........h,.... .
+00009270: 0200 0000 0000 e40a 0000 1c00 0000 0800  ................
+00009280: 0000 0200 5f5f 656e 645f 5f00 0010 0000  ....__end__.....
+00009290: 0800 0000 0200 0000 0000 ee0a 0000 8001  ................
+000092a0: 0000 0600 0000 0200 5f73 6967 6e61 6c00  ........_signal.
+000092b0: 082b 0000 0100 2000 0200 5f6d 616c 6c6f  .+.... ..._mallo
+000092c0: 6300 402b 0000 0100 2000 0200 0000 0000  c.@+.... .......
+000092d0: 080b 0000 9c2c 0000 0100 0000 0200 0000  .....,..........
+000092e0: 0000 160b 0000 d001 0000 0600 0000 0200  ................
+000092f0: 0000 0000 260b 0000 0000 0000 ffff 0000  ....&...........
+00009300: 0200 0000 0000 590b 0000 582c 0000 0100  ......Y...X,....
+00009310: 2000 0200 0000 0000 710b 0000 802b 0000   .......q....+..
+00009320: 0100 2000 0200 0000 0000 7c0b 0000 0000  .. .......|.....
+00009330: 1000 ffff 0000 0200 0000 0000 950b 0000  ................
+00009340: 1000 0000 0700 0000 0200 0000 0000 a70b  ................
+00009350: 0000 0000 4000 ffff 0000 0200 0000 0000  ....@...........
+00009360: b40b 0000 0300 0000 ffff 0000 0200 0000  ................
+00009370: 0000 c20b 0000 2802 0000 0600 0000 0200  ......(.........
+00009380: 0000 0000 d00b 0000 0000 0000 ffff 0000  ................
+00009390: 0200 0000 0000 ff0b 0000 0800 0000 0200  ................
+000093a0: 0000 0200 0000 0000 0a0c 0000 f801 0000  ................
+000093b0: 0600 0000 0200 5f61 626f 7274 0000 682b  ......_abort..h+
+000093c0: 0000 0100 2000 0200 0000 0000 180c 0000  .... ...........
+000093d0: 0000 0000 0000 2000 0201 1b00 0000 0100  ...... .........
 000093e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000093f0: c90c 0000 0100 0000 ffff 0000 0200 0000  ................
-00009400: 0000 e10c 0000 0000 0000 ffff 0000 0200  ................
-00009410: 0000 0000 f20c 0000 5006 0000 0600 0000  ........P.......
-00009420: 0200 0000 0000 060d 0000 1c02 0000 0600  ................
-00009430: 0000 0200 0000 0000 150d 0000 0400 0000  ................
-00009440: 0200 0000 0200 0000 0000 200d 0000 382b  .......... ...8+
-00009450: 0000 0100 2000 0200 0000 0000 2a0d 0000  .... .......*...
-00009460: 0402 0000 0600 0000 0200 0000 0000 380d  ..............8.
-00009470: 0000 a010 0000 0100 0000 0200 0000 0000  ................
-00009480: 450d 0000 0000 0000 0600 0000 0200 0000  E...............
-00009490: 0000 5a0d 0000 e402 0000 0300 0000 0200  ..Z.............
-000094a0: 0000 0000 6c0d 0000 bc01 0000 0600 0000  ....l...........
-000094b0: 0200 0000 0000 7a0d 0000 0000 0000 ffff  ......z.........
-000094c0: 0000 0200 0000 0000 960d 0000 5c01 0000  ............\...
-000094d0: 0600 0000 0200 0000 0000 a90d 0000 0000  ................
-000094e0: 0000 ffff 0000 0200 0000 0000 c10d 0000  ................
-000094f0: 2002 0000 0600 0000 0200 5f73 7472 6c65   ........._strle
-00009500: 6e00 c82a 0000 0100 2000 0200 0000 0000  n..*.... .......
-00009510: d10d 0000 b801 0000 0600 0000 0200 0000  ................
-00009520: 0000 e70d 0000 3000 0000 0500 0000 0200  ......0.........
-00009530: 0000 0000 ff0d 0000 a02b 0000 0100 2000  .........+.... .
-00009540: 0200 0000 0000 0e0e 0000 5001 0000 0600  ..........P.....
-00009550: 0000 0200 0000 0000 2d0e 0000 b82b 0000  ........-....+..
-00009560: 0100 2000 0200 0000 0000 450e 0000 6c01  .. .......E...l.
-00009570: 0000 0600 0000 0200 0000 0000 5e0e 0000  ............^...
-00009580: 8401 0000 0600 0000 0200 5f70 7269 6e74  .........._print
-00009590: 6600 f02a 0000 0100 2000 0200 0000 0000  f..*.... .......
-000095a0: 740e 0000 0c02 0000 0600 0000 0200 0000  t...............
-000095b0: 0000 850e 0000 e402 0000 0300 0000 0200  ................
-000095c0: 0000 0000 a70e 0000 9405 0000 0600 0000  ................
-000095d0: 0200 0000 0000 bd0e 0000 7800 0000 0300  ..........x.....
-000095e0: 0000 0200 0000 0000 d60e 0000 0400 0000  ................
-000095f0: 0800 0000 0200 0000 0000 e10e 0000 3402  ..............4.
-00009600: 0000 0600 0000 0200 0000 0000 fe0e 0000  ................
-00009610: 1000 0000 0700 0000 0200 0000 0000 0e0f  ................
-00009620: 0000 b82a 0000 0100 2000 0200 0000 0000  ...*.... .......
-00009630: 180f 0000 5401 0000 0600 0000 0200 0000  ....T...........
-00009640: 0000 360f 0000 f401 0000 0600 0000 0200  ..6.............
-00009650: 440f 0000 2e65 685f 6672 616d 6500 2e64  D....eh_frame..d
-00009660: 6562 7567 5f61 7261 6e67 6573 002e 6465  ebug_aranges..de
-00009670: 6275 675f 696e 666f 002e 6465 6275 675f  bug_info..debug_
-00009680: 6162 6272 6576 002e 6465 6275 675f 6c69  abbrev..debug_li
-00009690: 6e65 002e 6465 6275 675f 6672 616d 6500  ne..debug_frame.
-000096a0: 5f5f 6d69 6e67 7733 325f 696e 6974 5f6d  __mingw32_init_m
-000096b0: 6169 6e61 7267 7300 5f6d 6169 6e43 5254  ainargs._mainCRT
-000096c0: 5374 6172 7475 7000 5f57 696e 4d61 696e  Startup._WinMain
-000096d0: 4352 5453 7461 7274 7570 005f 6465 7265  CRTStartup._dere
-000096e0: 6769 7374 6572 5f66 7261 6d65 5f66 6e00  gister_frame_fn.
-000096f0: 5f5f 5f4a 4352 5f4c 4953 545f 5f00 5f5f  ___JCR_LIST__.__
-00009700: 5f67 6363 5f72 6567 6973 7465 725f 6672  _gcc_register_fr
-00009710: 616d 6500 5f5f 5f67 6363 5f64 6572 6567  ame.___gcc_dereg
-00009720: 6973 7465 725f 6672 616d 6500 2e65 685f  ister_frame..eh_
-00009730: 6672 616d 6500 2e72 6461 7461 247a 7a7a  frame..rdata$zzz
-00009740: 005f 456e 756d 5769 6e64 6f77 7350 726f  ._EnumWindowsPro
-00009750: 6340 3800 5f5f 7365 7461 7267 7600 5f5f  c@8.__setargv.__
-00009760: 5f63 7075 5f66 6561 7475 7265 735f 696e  _cpu_features_in
-00009770: 6974 005f 5f5f 646f 5f67 6c6f 6261 6c5f  it.___do_global_
-00009780: 6474 6f72 7300 5f5f 5f64 6f5f 676c 6f62  dtors.___do_glob
-00009790: 616c 5f63 746f 7273 005f 5f5f 6479 6e5f  al_ctors.___dyn_
-000097a0: 746c 735f 696e 6974 4031 3200 5f5f 5f74  tls_init@12.___t
-000097b0: 6c72 6567 6474 6f72 005f 5f5f 5f77 3634  lregdtor.____w64
-000097c0: 5f6d 696e 6777 7468 725f 6164 645f 6b65  _mingwthr_add_ke
-000097d0: 795f 6474 6f72 005f 5f5f 5f77 3634 5f6d  y_dtor.____w64_m
-000097e0: 696e 6777 7468 725f 7265 6d6f 7665 5f6b  ingwthr_remove_k
-000097f0: 6579 5f64 746f 7200 5f5f 5f6d 696e 6777  ey_dtor.___mingw
-00009800: 5f54 4c53 6361 6c6c 6261 636b 005f 5f70  _TLScallback.__p
-00009810: 6569 3338 365f 7275 6e74 696d 655f 7265  ei386_runtime_re
-00009820: 6c6f 6361 746f 7200 2e64 6562 7567 5f69  locator..debug_i
-00009830: 6e66 6f00 2e64 6562 7567 5f61 6262 7265  nfo..debug_abbre
-00009840: 7600 2e64 6562 7567 5f6c 696e 6500 2e64  v..debug_line..d
-00009850: 6562 7567 5f61 7261 6e67 6573 002e 6465  ebug_aranges..de
-00009860: 6275 675f 6672 616d 6500 5f66 6573 6574  bug_frame._feset
-00009870: 656e 7600 5f5f 5f6d 696e 6777 5f67 6c6f  env.___mingw_glo
-00009880: 6200 5f5f 5f6d 696e 6777 5f67 6c6f 6266  b.___mingw_globf
-00009890: 7265 6500 5f5f 5f6d 696e 6777 5f64 6972  ree.___mingw_dir
-000098a0: 6e61 6d65 005f 5f5f 6d69 6e67 775f 6f70  name.___mingw_op
-000098b0: 656e 6469 7200 5f5f 5f6d 696e 6777 5f72  endir.___mingw_r
-000098c0: 6561 6464 6972 005f 5f5f 6d69 6e67 775f  eaddir.___mingw_
-000098d0: 636c 6f73 6564 6972 005f 5f5f 6d69 6e67  closedir.___ming
-000098e0: 775f 7265 7769 6e64 6469 7200 5f5f 5f6d  w_rewinddir.___m
-000098f0: 696e 6777 5f74 656c 6c64 6972 005f 5f5f  ingw_telldir.___
-00009900: 6d69 6e67 775f 7365 656b 6469 7200 5f5f  mingw_seekdir.__
-00009910: 5f46 5241 4d45 5f45 4e44 5f5f 005f 5f5f  _FRAME_END__.___
-00009920: 4a43 525f 454e 445f 5f00 5f72 6567 6973  JCR_END__._regis
-00009930: 7465 725f 6672 616d 655f 6374 6f72 002e  ter_frame_ctor..
-00009940: 7465 7874 2e73 7461 7274 7570 002e 6374  text.startup..ct
-00009950: 6f72 732e 3635 3533 3500 5f5f 696d 705f  ors.65535.__imp_
-00009960: 5f46 696e 6446 6972 7374 4669 6c65 4140  _FindFirstFileA@
-00009970: 3800 5f56 6972 7475 616c 5072 6f74 6563  8._VirtualProtec
-00009980: 7440 3136 005f 5f5f 5255 4e54 494d 455f  t@16.___RUNTIME_
-00009990: 5053 4555 444f 5f52 454c 4f43 5f4c 4953  PSEUDO_RELOC_LIS
-000099a0: 545f 5f00 5f5f 696d 705f 5f5f 6675 6c6c  T__.__imp___full
-000099b0: 7061 7468 005f 4669 6e64 4669 7273 7446  path._FindFirstF
-000099c0: 696c 6541 4038 005f 5f69 6d70 5f5f 5f73  ileA@8.__imp___s
-000099d0: 6574 6d6f 6465 005f 5f64 6174 615f 7374  etmode.__data_st
-000099e0: 6172 745f 5f00 5f46 7265 654c 6962 7261  art__._FreeLibra
-000099f0: 7279 4034 005f 5f5f 4454 4f52 5f4c 4953  ry@4.___DTOR_LIS
-00009a00: 545f 5f00 5f5f 696d 705f 5f56 6972 7475  T__.__imp__Virtu
-00009a10: 616c 5072 6f74 6563 7440 3136 005f 5f69  alProtect@16.__i
-00009a20: 6d70 5f5f 5f6f 6e65 7869 7400 5f5f 5f70  mp___onexit.___p
-00009a30: 5f5f 666d 6f64 6500 5f5f 696d 705f 5f47  __fmode.__imp__G
-00009a40: 6574 4c61 7374 4572 726f 7240 3000 5f53  etLastError@0._S
-00009a50: 6574 556e 6861 6e64 6c65 6445 7863 6570  etUnhandledExcep
-00009a60: 7469 6f6e 4669 6c74 6572 4034 005f 5f69  tionFilter@4.__i
-00009a70: 6d70 5f5f 5669 7274 7561 6c51 7565 7279  mp__VirtualQuery
-00009a80: 4031 3200 5f5f 696d 705f 5f46 696e 644e  @12.__imp__FindN
-00009a90: 6578 7446 696c 6541 4038 005f 5f5f 746c  extFileA@8.___tl
-00009aa0: 735f 7374 6172 745f 5f00 5f45 6e75 6d57  s_start__._EnumW
-00009ab0: 696e 646f 7773 4038 005f 5f69 6d70 5f5f  indows@8.__imp__
-00009ac0: 546c 7347 6574 5661 6c75 6540 3400 5f5f  TlsGetValue@4.__
-00009ad0: 6c69 626d 7376 6372 745f 615f 696e 616d  libmsvcrt_a_inam
-00009ae0: 6500 5f5f 696d 705f 5f49 6e69 7469 616c  e.__imp__Initial
-00009af0: 697a 6543 7269 7469 6361 6c53 6563 7469  izeCriticalSecti
-00009b00: 6f6e 4034 005f 4465 6c65 7465 4372 6974  on@4._DeleteCrit
-00009b10: 6963 616c 5365 6374 696f 6e40 3400 5f5f  icalSection@4.__
-00009b20: 7274 5f70 7372 656c 6f63 735f 7374 6172  rt_psrelocs_star
-00009b30: 7400 5f5f 696d 705f 5f61 626f 7274 005f  t.__imp__abort._
-00009b40: 5f64 6c6c 5f63 6861 7261 6374 6572 6973  _dll_characteris
-00009b50: 7469 6373 5f5f 005f 5f73 697a 655f 6f66  tics__.__size_of
-00009b60: 5f73 7461 636b 5f63 6f6d 6d69 745f 5f00  _stack_commit__.
-00009b70: 5f5f 7369 7a65 5f6f 665f 7374 6163 6b5f  __size_of_stack_
-00009b80: 7265 7365 7276 655f 5f00 5f5f 6d61 6a6f  reserve__.__majo
-00009b90: 725f 7375 6273 7973 7465 6d5f 7665 7273  r_subsystem_vers
-00009ba0: 696f 6e5f 5f00 5f5f 5f63 7274 5f78 6c5f  ion__.___crt_xl_
-00009bb0: 7374 6172 745f 5f00 5f5f 5f63 7274 5f78  start__.___crt_x
-00009bc0: 695f 7374 6172 745f 5f00 5f5f 5f63 7274  i_start__.___crt
-00009bd0: 5f78 695f 656e 645f 5f00 5f5f 696d 705f  _xi_end__.__imp_
-00009be0: 5f73 7472 6963 6f6c 6c00 5f5f 696d 705f  _stricoll.__imp_
-00009bf0: 5f5f 5f6d 625f 6375 725f 6d61 7800 5f47  ___mb_cur_max._G
-00009c00: 6574 4c61 7374 4572 726f 7240 3000 5f5f  etLastError@0.__
-00009c10: 696d 705f 5f5f 5f70 5f5f 656e 7669 726f  imp____p__enviro
-00009c20: 6e00 5f5f 696d 705f 5f5f 7063 7479 7065  n.__imp___pctype
-00009c30: 005f 5669 7274 7561 6c51 7565 7279 4031  ._VirtualQuery@1
-00009c40: 3200 5f5f 6865 6164 5f6c 6962 7573 6572  2.__head_libuser
-00009c50: 3332 5f61 005f 6d69 6e67 775f 696e 6974  32_a._mingw_init
-00009c60: 6c74 7364 726f 745f 666f 7263 6500 5f5f  ltsdrot_force.__
-00009c70: 696d 705f 5f5f 696f 6200 5f47 6574 4d6f  imp___iob._GetMo
-00009c80: 6475 6c65 4861 6e64 6c65 4140 3400 5f5f  duleHandleA@4.__
-00009c90: 5f72 6567 6973 7465 725f 6672 616d 655f  _register_frame_
-00009ca0: 696e 666f 005f 5f6c 6962 6d6f 6c64 6e61  info.__libmoldna
-00009cb0: 6d65 5f61 5f69 6e61 6d65 005f 686d 6f64  me_a_iname._hmod
-00009cc0: 5f6c 6962 6763 6300 2e77 6561 6b2e 5f5f  _libgcc..weak.__
-00009cd0: 5f72 6567 6973 7465 725f 6672 616d 655f  _register_frame_
-00009ce0: 696e 666f 2e5f 5f5f 4548 5f46 5241 4d45  info.___EH_FRAME
-00009cf0: 5f42 4547 494e 5f5f 005f 5f69 6d70 5f5f  _BEGIN__.__imp__
-00009d00: 7374 7264 7570 005f 5f69 6d70 5f5f 5f69  strdup.__imp___i
-00009d10: 7363 7479 7065 005f 5f62 7373 5f73 7461  sctype.__bss_sta
-00009d20: 7274 5f5f 005f 5f5f 5255 4e54 494d 455f  rt__.___RUNTIME_
-00009d30: 5053 4555 444f 5f52 454c 4f43 5f4c 4953  PSEUDO_RELOC_LIS
-00009d40: 545f 454e 445f 5f00 5f5f 6670 7265 7365  T_END__.__fprese
-00009d50: 7400 5f5f 7369 7a65 5f6f 665f 6865 6170  t.__size_of_heap
-00009d60: 5f63 6f6d 6d69 745f 5f00 5f5f 696d 705f  _commit__.__imp_
-00009d70: 5f5f 6572 726e 6f00 5f5f 5f70 5f5f 656e  __errno.___p__en
-00009d80: 7669 726f 6e00 5f5f 696d 705f 5f47 6574  viron.__imp__Get
-00009d90: 5072 6f63 4164 6472 6573 7340 3800 5f47  ProcAddress@8._G
-00009da0: 6574 5072 6f63 4164 6472 6573 7340 3800  etProcAddress@8.
-00009db0: 5f5f 5f63 7274 5f78 705f 7374 6172 745f  ___crt_xp_start_
-00009dc0: 5f00 5f5f 696d 705f 5f77 6373 746f 6d62  _.__imp__wcstomb
-00009dd0: 7300 5f47 6574 436f 6d6d 616e 644c 696e  s._GetCommandLin
-00009de0: 6541 4030 005f 5f5f 6372 745f 7870 5f65  eA@0.___crt_xp_e
-00009df0: 6e64 5f5f 005f 5f69 6d70 5f5f 7369 676e  nd__.__imp__sign
-00009e00: 616c 005f 5f6d 696e 6f72 5f6f 735f 7665  al.__minor_os_ve
-00009e10: 7273 696f 6e5f 5f00 5f5f 696d 705f 5f61  rsion__.__imp__a
-00009e20: 7465 7869 7400 5f5f 696d 705f 5f6d 6273  texit.__imp__mbs
-00009e30: 746f 7763 7300 5f5f 6865 6164 5f6c 6962  towcs.__head_lib
-00009e40: 6d73 7663 7274 5f61 005f 5f69 6d61 6765  msvcrt_a.__image
-00009e50: 5f62 6173 655f 5f00 5f5f 6973 6374 7970  _base__.__isctyp
-00009e60: 6500 5f5f 7365 6374 696f 6e5f 616c 6967  e.__section_alig
-00009e70: 6e6d 656e 745f 5f00 5f4c 6f61 644c 6962  nment__._LoadLib
-00009e80: 7261 7279 4140 3400 5f5f 696d 705f 5f47  raryA@4.__imp__G
-00009e90: 6574 5769 6e64 6f77 5468 7265 6164 5072  etWindowThreadPr
-00009ea0: 6f63 6573 7349 6440 3800 5f77 6373 746f  ocessId@8._wcsto
-00009eb0: 6d62 7300 5f5f 696d 705f 5f46 7265 654c  mbs.__imp__FreeL
-00009ec0: 6962 7261 7279 4034 005f 5f49 4154 5f65  ibrary@4.__IAT_e
-00009ed0: 6e64 5f5f 005f 5f68 6561 645f 6c69 626d  nd__.__head_libm
-00009ee0: 6f6c 646e 616d 655f 6100 5f5f 5255 4e54  oldname_a.__RUNT
-00009ef0: 494d 455f 5053 4555 444f 5f52 454c 4f43  IME_PSEUDO_RELOC
-00009f00: 5f4c 4953 545f 5f00 5f73 6574 6c6f 6361  _LIST__._setloca
-00009f10: 6c65 005f 5f69 6d70 5f5f 5f5f 705f 5f66  le.__imp____p__f
-00009f20: 6d6f 6465 005f 5f74 6c73 5f73 7461 7274  mode.__tls_start
-00009f30: 005f 4578 6974 5072 6f63 6573 7340 3400  ._ExitProcess@4.
-00009f40: 5f5f 696d 705f 5f45 6e75 6d57 696e 646f  __imp__EnumWindo
-00009f50: 7773 4038 005f 5f69 6d70 5f5f 7374 7263  ws@8.__imp__strc
-00009f60: 6f6c 6c00 5f5f 6461 7461 5f65 6e64 5f5f  oll.__data_end__
-00009f70: 005f 5f5f 6765 746d 6169 6e61 7267 7300  .___getmainargs.
-00009f80: 5f46 696e 6443 6c6f 7365 4034 005f 5f43  _FindClose@4.__C
-00009f90: 544f 525f 4c49 5354 5f5f 005f 6d62 7374  TOR_LIST__._mbst
-00009fa0: 6f77 6373 005f 5f5f 7365 745f 6170 705f  owcs.___set_app_
-00009fb0: 7479 7065 005f 5f62 7373 5f65 6e64 5f5f  type.__bss_end__
-00009fc0: 005f 5f43 5254 5f66 6d6f 6465 005f 5f5f  .__CRT_fmode.___
-00009fd0: 6372 745f 7863 5f65 6e64 5f5f 005f 5f74  crt_xc_end__.__t
-00009fe0: 6c73 5f69 6e64 6578 005f 5f5f 6372 745f  ls_index.___crt_
-00009ff0: 7863 5f73 7461 7274 5f5f 005f 5f5f 4354  xc_start__.___CT
-0000a000: 4f52 5f4c 4953 545f 5f00 5f5f 7274 5f70  OR_LIST__.__rt_p
-0000a010: 7372 656c 6f63 735f 7369 7a65 005f 5f69  srelocs_size.__i
-0000a020: 6d70 5f5f 6d65 6d63 7079 005f 4669 6e64  mp__memcpy._Find
-0000a030: 4e65 7874 4669 6c65 4140 3800 5f5f 6669  NextFileA@8.__fi
-0000a040: 6c65 5f61 6c69 676e 6d65 6e74 5f5f 005f  le_alignment__._
-0000a050: 5f69 6d70 5f5f 4c65 6176 6543 7269 7469  _imp__LeaveCriti
-0000a060: 6361 6c53 6563 7469 6f6e 4034 005f 5f69  calSection@4.__i
-0000a070: 6d70 5f5f 6174 6f69 005f 5f69 6d70 5f5f  mp__atoi.__imp__
-0000a080: 6d61 6c6c 6f63 005f 5f5f 4548 5f46 5241  malloc.___EH_FRA
-0000a090: 4d45 5f42 4547 494e 5f5f 005f 5365 7446  ME_BEGIN__._SetF
-0000a0a0: 6f72 6567 726f 756e 6457 696e 646f 7740  oregroundWindow@
-0000a0b0: 3400 5f5f 6d61 6a6f 725f 6f73 5f76 6572  4.__major_os_ver
-0000a0c0: 7369 6f6e 5f5f 005f 5f69 6d70 5f5f 7265  sion__.__imp__re
-0000a0d0: 616c 6c6f 6300 5f5f 4941 545f 7374 6172  alloc.__IAT_star
-0000a0e0: 745f 5f00 5f73 7472 6963 6f6c 6c00 5f5f  t__._stricoll.__
-0000a0f0: 746c 735f 656e 6400 5f5f 696d 705f 5f47  tls_end.__imp__G
-0000a100: 6574 4d6f 6475 6c65 4861 6e64 6c65 4140  etModuleHandleA@
-0000a110: 3400 5f5f 4454 4f52 5f4c 4953 545f 5f00  4.__DTOR_LIST__.
-0000a120: 5f5f 696d 705f 5f5f 6670 7265 7365 7400  __imp___fpreset.
-0000a130: 2e77 6561 6b2e 5f5f 5f64 6572 6567 6973  .weak.___deregis
-0000a140: 7465 725f 6672 616d 655f 696e 666f 2e5f  ter_frame_info._
-0000a150: 5f5f 4548 5f46 5241 4d45 5f42 4547 494e  __EH_FRAME_BEGIN
-0000a160: 5f5f 005f 456e 7465 7243 7269 7469 6361  __._EnterCritica
-0000a170: 6c53 6563 7469 6f6e 4034 005f 5f66 756c  lSection@4.__ful
-0000a180: 6c70 6174 6800 5f5f 7369 7a65 5f6f 665f  lpath.__size_of_
-0000a190: 6865 6170 5f72 6573 6572 7665 5f5f 005f  heap_reserve__._
-0000a1a0: 5f5f 6372 745f 7874 5f73 7461 7274 5f5f  __crt_xt_start__
-0000a1b0: 005f 5f5f 496d 6167 6542 6173 6500 5f5f  .___ImageBase.__
-0000a1c0: 7375 6273 7973 7465 6d5f 5f00 5f5f 696d  subsystem__.__im
-0000a1d0: 705f 5f73 7472 6c65 6e00 2e77 6561 6b2e  p__strlen..weak.
-0000a1e0: 5f5f 4a76 5f52 6567 6973 7465 7243 6c61  __Jv_RegisterCla
-0000a1f0: 7373 6573 2e5f 5f5f 4548 5f46 5241 4d45  sses.___EH_FRAME
-0000a200: 5f42 4547 494e 5f5f 005f 5f43 5254 5f66  _BEGIN__.__CRT_f
-0000a210: 656e 7600 5f5f 696d 705f 5f63 616c 6c6f  env.__imp__callo
-0000a220: 6300 5f5f 4a76 5f52 6567 6973 7465 7243  c.__Jv_RegisterC
-0000a230: 6c61 7373 6573 005f 4765 7457 696e 646f  lasses._GetWindo
-0000a240: 7754 6872 6561 6450 726f 6365 7373 4964  wThreadProcessId
-0000a250: 4038 005f 5f69 6d70 5f5f 5f5f 6765 746d  @8.__imp____getm
-0000a260: 6169 6e61 7267 7300 5f5f 5f74 6c73 5f65  ainargs.___tls_e
-0000a270: 6e64 5f5f 005f 5f69 6d70 5f5f 4578 6974  nd__.__imp__Exit
-0000a280: 5072 6f63 6573 7340 3400 5f6d 696e 6777  Process@4._mingw
-0000a290: 5f69 6e69 746c 7473 7375 6f5f 666f 7263  _initltssuo_forc
-0000a2a0: 6500 5f49 6e69 7469 616c 697a 6543 7269  e._InitializeCri
-0000a2b0: 7469 6361 6c53 6563 7469 6f6e 4034 005f  ticalSection@4._
-0000a2c0: 5f5f 6370 755f 6665 6174 7572 6573 005f  __cpu_features._
-0000a2d0: 5f69 6d70 5f5f 6672 6565 005f 5f69 6d70  _imp__free.__imp
-0000a2e0: 5f5f 5365 7455 6e68 616e 646c 6564 4578  __SetUnhandledEx
-0000a2f0: 6365 7074 696f 6e46 696c 7465 7240 3400  ceptionFilter@4.
-0000a300: 5f5f 5f64 6572 6567 6973 7465 725f 6672  ___deregister_fr
-0000a310: 616d 655f 696e 666f 005f 5f6d 616a 6f72  ame_info.__major
-0000a320: 5f69 6d61 6765 5f76 6572 7369 6f6e 5f5f  _image_version__
-0000a330: 005f 5f6c 6f61 6465 725f 666c 6167 735f  .__loader_flags_
-0000a340: 5f00 5f5f 6c69 6275 7365 7233 325f 615f  _.__libuser32_a_
-0000a350: 696e 616d 6500 5f5f 696d 705f 5f74 6f6c  iname.__imp__tol
-0000a360: 6f77 6572 005f 5f43 5254 5f67 6c6f 6200  ower.__CRT_glob.
-0000a370: 5f5f 7365 746d 6f64 6500 5f5f 696d 705f  __setmode.__imp_
-0000a380: 5f70 7269 6e74 6600 5f5f 5f63 686b 7374  _printf.___chkst
-0000a390: 6b5f 6d73 005f 5f68 6561 645f 6c69 626b  k_ms.__head_libk
-0000a3a0: 6572 6e65 6c33 325f 6100 5f5f 7274 5f70  ernel32_a.__rt_p
-0000a3b0: 7372 656c 6f63 735f 656e 6400 5f5f 696d  srelocs_end.__im
-0000a3c0: 705f 5f5f 6365 7869 7400 5f5f 6d69 6e6f  p___cexit.__mino
-0000a3d0: 725f 7375 6273 7973 7465 6d5f 7665 7273  r_subsystem_vers
-0000a3e0: 696f 6e5f 5f00 5f5f 696d 705f 5f46 696e  ion__.__imp__Fin
-0000a3f0: 6443 6c6f 7365 4034 005f 5f6d 696e 6f72  dClose@4.__minor
-0000a400: 5f69 6d61 6765 5f76 6572 7369 6f6e 5f5f  _image_version__
-0000a410: 005f 5f69 6d70 5f5f 7666 7072 696e 7466  .__imp__vfprintf
-0000a420: 005f 5f69 6d70 5f5f 5f5f 7365 745f 6170  .__imp____set_ap
-0000a430: 705f 7479 7065 005f 6d69 6e67 775f 696e  p_type._mingw_in
-0000a440: 6974 6c74 7364 796e 5f66 6f72 6365 005f  itltsdyn_force._
-0000a450: 546c 7347 6574 5661 6c75 6540 3400 5f5f  TlsGetValue@4.__
-0000a460: 696d 705f 5f44 656c 6574 6543 7269 7469  imp__DeleteCriti
-0000a470: 6361 6c53 6563 7469 6f6e 4034 005f 4c65  calSection@4._Le
-0000a480: 6176 6543 7269 7469 6361 6c53 6563 7469  aveCriticalSecti
-0000a490: 6f6e 4034 005f 5f69 6d70 5f5f 4765 7443  on@4.__imp__GetC
-0000a4a0: 6f6d 6d61 6e64 4c69 6e65 4140 3000 5f5f  ommandLineA@0.__
-0000a4b0: 696d 705f 5f4c 6f61 644c 6962 7261 7279  imp__LoadLibrary
-0000a4c0: 4140 3400 5f5f 696d 705f 5f73 6574 6c6f  A@4.__imp__setlo
-0000a4d0: 6361 6c65 005f 5f52 554e 5449 4d45 5f50  cale.__RUNTIME_P
-0000a4e0: 5345 5544 4f5f 5245 4c4f 435f 4c49 5354  SEUDO_RELOC_LIST
-0000a4f0: 5f45 4e44 5f5f 005f 5f6c 6962 6b65 726e  _END__.__libkern
-0000a500: 656c 3332 5f61 5f69 6e61 6d65 005f 5f5f  el32_a_iname.___
-0000a510: 6479 6e5f 746c 735f 696e 6974 5f63 616c  dyn_tls_init_cal
-0000a520: 6c62 6163 6b00 5f5f 746c 735f 7573 6564  lback.__tls_used
-0000a530: 005f 5f69 6d70 5f5f 5365 7446 6f72 6567  .__imp__SetForeg
-0000a540: 726f 756e 6457 696e 646f 7740 3400 5f5f  roundWindow@4.__
-0000a550: 5f63 7274 5f78 745f 656e 645f 5f00 5f76  _crt_xt_end__._v
-0000a560: 6670 7269 6e74 6600 5f5f 696d 705f 5f45  fprintf.__imp__E
-0000a570: 6e74 6572 4372 6974 6963 616c 5365 6374  nterCriticalSect
-0000a580: 696f 6e40 3400 5f5f 696d 705f 5f66 7772  ion@4.__imp__fwr
-0000a590: 6974 6500                                ite.
+000093f0: 2d0c 0000 c82b 0000 0100 2000 0200 0000  -....+.... .....
+00009400: 0000 490c 0000 b401 0000 0600 0000 0200  ..I.............
+00009410: 0000 0000 5e0c 0000 2000 0000 0800 0000  ....^... .......
+00009420: 0200 0000 0000 6b0c 0000 6401 0000 0600  ......k...d.....
+00009430: 0000 0200 0000 0000 800c 0000 2c00 0000  ............,...
+00009440: 0500 0000 0200 0000 0000 980c 0000 082c  ...............,
+00009450: 0000 0100 2000 0200 0000 0000 b50c 0000  .... ...........
+00009460: 2400 0000 0500 0000 0200 0000 0000 c50c  $...............
+00009470: 0000 fc01 0000 0600 0000 0200 0000 0000  ................
+00009480: d10c 0000 9401 0000 0600 0000 0200 0000  ................
+00009490: 0000 f60c 0000 0000 0000 0000 2000 0201  ............ ...
+000094a0: 1a00 0000 0100 0000 0000 0000 0000 0000  ................
+000094b0: 0000 0000 0000 0f0d 0000 0100 0000 ffff  ................
+000094c0: 0000 0200 0000 0000 270d 0000 0000 0000  ........'.......
+000094d0: ffff 0000 0200 0000 0000 380d 0000 9c06  ..........8.....
+000094e0: 0000 0600 0000 0200 0000 0000 4c0d 0000  ............L...
+000094f0: 4c02 0000 0600 0000 0200 0000 0000 600d  L.............`.
+00009500: 0000 2c02 0000 0600 0000 0200 0000 0000  ..,.............
+00009510: 6f0d 0000 0400 0000 0200 0000 0200 0000  o...............
+00009520: 0000 7a0d 0000 702b 0000 0100 2000 0200  ..z...p+.... ...
+00009530: 0000 0000 840d 0000 1002 0000 0600 0000  ................
+00009540: 0200 0000 0000 920d 0000 d010 0000 0100  ................
+00009550: 0000 0200 0000 0000 9f0d 0000 0000 0000  ................
+00009560: 0600 0000 0200 0000 0000 b40d 0000 0803  ................
+00009570: 0000 0300 0000 0200 0000 0000 c60d 0000  ................
+00009580: c801 0000 0600 0000 0200 0000 0000 d40d  ................
+00009590: 0000 0000 0000 ffff 0000 0200 0000 0000  ................
+000095a0: f00d 0000 6801 0000 0600 0000 0200 0000  ....h...........
+000095b0: 0000 030e 0000 0000 0000 ffff 0000 0200  ................
+000095c0: 0000 0000 1b0e 0000 3002 0000 0600 0000  ........0.......
+000095d0: 0200 5f73 7472 6c65 6e00 f82a 0000 0100  .._strlen..*....
+000095e0: 2000 0200 0000 0000 2b0e 0000 c401 0000   .......+.......
+000095f0: 0600 0000 0200 0000 0000 410e 0000 3000  ..........A...0.
+00009600: 0000 0500 0000 0200 0000 0000 590e 0000  ............Y...
+00009610: e82b 0000 0100 2000 0200 0000 0000 680e  .+.... .......h.
+00009620: 0000 5c01 0000 0600 0000 0200 0000 0000  ..\.............
+00009630: 870e 0000 002c 0000 0100 2000 0200 0000  .....,.... .....
+00009640: 0000 9f0e 0000 7801 0000 0600 0000 0200  ......x.........
+00009650: 0000 0000 b80e 0000 9001 0000 0600 0000  ................
+00009660: 0200 5f70 7269 6e74 6600 282b 0000 0100  .._printf.(+....
+00009670: 2000 0200 0000 0000 ce0e 0000 1c02 0000   ...............
+00009680: 0600 0000 0200 0000 0000 df0e 0000 0803  ................
+00009690: 0000 0300 0000 0200 0000 0000 010f 0000  ................
+000096a0: d405 0000 0600 0000 0200 0000 0000 170f  ................
+000096b0: 0000 9c00 0000 0300 0000 0200 0000 0000  ................
+000096c0: 300f 0000 0400 0000 0800 0000 0200 0000  0...............
+000096d0: 0000 3b0f 0000 4802 0000 0600 0000 0200  ..;...H.........
+000096e0: 0000 0000 580f 0000 1000 0000 0700 0000  ....X...........
+000096f0: 0200 0000 0000 680f 0000 e82a 0000 0100  ......h....*....
+00009700: 2000 0200 0000 0000 720f 0000 6001 0000   .......r...`...
+00009710: 0600 0000 0200 0000 0000 900f 0000 0002  ................
+00009720: 0000 0600 0000 0200 9e0f 0000 2e65 685f  .............eh_
+00009730: 6672 616d 6500 2e64 6562 7567 5f61 7261  frame..debug_ara
+00009740: 6e67 6573 002e 6465 6275 675f 696e 666f  nges..debug_info
+00009750: 002e 6465 6275 675f 6162 6272 6576 002e  ..debug_abbrev..
+00009760: 6465 6275 675f 6c69 6e65 002e 6465 6275  debug_line..debu
+00009770: 675f 6672 616d 6500 5f5f 6d69 6e67 7733  g_frame.__mingw3
+00009780: 325f 696e 6974 5f6d 6169 6e61 7267 7300  2_init_mainargs.
+00009790: 5f6d 6169 6e43 5254 5374 6172 7475 7000  _mainCRTStartup.
+000097a0: 5f57 696e 4d61 696e 4352 5453 7461 7274  _WinMainCRTStart
+000097b0: 7570 005f 6465 7265 6769 7374 6572 5f66  up._deregister_f
+000097c0: 7261 6d65 5f66 6e00 5f5f 5f4a 4352 5f4c  rame_fn.___JCR_L
+000097d0: 4953 545f 5f00 5f5f 5f67 6363 5f72 6567  IST__.___gcc_reg
+000097e0: 6973 7465 725f 6672 616d 6500 5f5f 5f67  ister_frame.___g
+000097f0: 6363 5f64 6572 6567 6973 7465 725f 6672  cc_deregister_fr
+00009800: 616d 6500 2e65 685f 6672 616d 6500 2e72  ame..eh_frame..r
+00009810: 6461 7461 247a 7a7a 005f 456e 756d 5769  data$zzz._EnumWi
+00009820: 6e64 6f77 7350 726f 6340 3800 5f5f 7365  ndowsProc@8.__se
+00009830: 7461 7267 7600 5f5f 5f63 7075 5f66 6561  targv.___cpu_fea
+00009840: 7475 7265 735f 696e 6974 005f 5f5f 646f  tures_init.___do
+00009850: 5f67 6c6f 6261 6c5f 6474 6f72 7300 5f5f  _global_dtors.__
+00009860: 5f64 6f5f 676c 6f62 616c 5f63 746f 7273  _do_global_ctors
+00009870: 005f 5f5f 6479 6e5f 746c 735f 696e 6974  .___dyn_tls_init
+00009880: 4031 3200 5f5f 5f74 6c72 6567 6474 6f72  @12.___tlregdtor
+00009890: 005f 5f5f 5f77 3634 5f6d 696e 6777 7468  .____w64_mingwth
+000098a0: 725f 6164 645f 6b65 795f 6474 6f72 005f  r_add_key_dtor._
+000098b0: 5f5f 5f77 3634 5f6d 696e 6777 7468 725f  ___w64_mingwthr_
+000098c0: 7265 6d6f 7665 5f6b 6579 5f64 746f 7200  remove_key_dtor.
+000098d0: 5f5f 5f6d 696e 6777 5f54 4c53 6361 6c6c  ___mingw_TLScall
+000098e0: 6261 636b 005f 5f70 6569 3338 365f 7275  back.__pei386_ru
+000098f0: 6e74 696d 655f 7265 6c6f 6361 746f 7200  ntime_relocator.
+00009900: 2e64 6562 7567 5f69 6e66 6f00 2e64 6562  .debug_info..deb
+00009910: 7567 5f61 6262 7265 7600 2e64 6562 7567  ug_abbrev..debug
+00009920: 5f6c 696e 6500 2e64 6562 7567 5f61 7261  _line..debug_ara
+00009930: 6e67 6573 002e 6465 6275 675f 6672 616d  nges..debug_fram
+00009940: 6500 5f66 6573 6574 656e 7600 5f5f 5f6d  e._fesetenv.___m
+00009950: 696e 6777 5f67 6c6f 6200 5f5f 5f6d 696e  ingw_glob.___min
+00009960: 6777 5f67 6c6f 6266 7265 6500 5f5f 5f6d  gw_globfree.___m
+00009970: 696e 6777 5f64 6972 6e61 6d65 005f 5f5f  ingw_dirname.___
+00009980: 6d69 6e67 775f 6f70 656e 6469 7200 5f5f  mingw_opendir.__
+00009990: 5f6d 696e 6777 5f72 6561 6464 6972 005f  _mingw_readdir._
+000099a0: 5f5f 6d69 6e67 775f 636c 6f73 6564 6972  __mingw_closedir
+000099b0: 005f 5f5f 6d69 6e67 775f 7265 7769 6e64  .___mingw_rewind
+000099c0: 6469 7200 5f5f 5f6d 696e 6777 5f74 656c  dir.___mingw_tel
+000099d0: 6c64 6972 005f 5f5f 6d69 6e67 775f 7365  ldir.___mingw_se
+000099e0: 656b 6469 7200 5f5f 5f46 5241 4d45 5f45  ekdir.___FRAME_E
+000099f0: 4e44 5f5f 005f 5f5f 4a43 525f 454e 445f  ND__.___JCR_END_
+00009a00: 5f00 5f72 6567 6973 7465 725f 6672 616d  _._register_fram
+00009a10: 655f 6374 6f72 002e 7465 7874 2e73 7461  e_ctor..text.sta
+00009a20: 7274 7570 002e 6374 6f72 732e 3635 3533  rtup..ctors.6553
+00009a30: 3500 5f5f 696d 705f 5f46 696e 6446 6972  5.__imp__FindFir
+00009a40: 7374 4669 6c65 4140 3800 5f53 686f 7757  stFileA@8._ShowW
+00009a50: 696e 646f 7740 3800 5f56 6972 7475 616c  indow@8._Virtual
+00009a60: 5072 6f74 6563 7440 3136 005f 5f5f 5255  Protect@16.___RU
+00009a70: 4e54 494d 455f 5053 4555 444f 5f52 454c  NTIME_PSEUDO_REL
+00009a80: 4f43 5f4c 4953 545f 5f00 5f5f 696d 705f  OC_LIST__.__imp_
+00009a90: 5f5f 6675 6c6c 7061 7468 005f 4669 6e64  __fullpath._Find
+00009aa0: 4669 7273 7446 696c 6541 4038 005f 5f69  FirstFileA@8.__i
+00009ab0: 6d70 5f5f 5f73 6574 6d6f 6465 005f 5f64  mp___setmode.__d
+00009ac0: 6174 615f 7374 6172 745f 5f00 5f46 7265  ata_start__._Fre
+00009ad0: 654c 6962 7261 7279 4034 005f 5f5f 4454  eLibrary@4.___DT
+00009ae0: 4f52 5f4c 4953 545f 5f00 5f5f 696d 705f  OR_LIST__.__imp_
+00009af0: 5f56 6972 7475 616c 5072 6f74 6563 7440  _VirtualProtect@
+00009b00: 3136 005f 5f69 6d70 5f5f 5f6f 6e65 7869  16.__imp___onexi
+00009b10: 7400 5f5f 5f70 5f5f 666d 6f64 6500 5f5f  t.___p__fmode.__
+00009b20: 696d 705f 5f47 6574 4c61 7374 4572 726f  imp__GetLastErro
+00009b30: 7240 3000 5f53 6574 556e 6861 6e64 6c65  r@0._SetUnhandle
+00009b40: 6445 7863 6570 7469 6f6e 4669 6c74 6572  dExceptionFilter
+00009b50: 4034 005f 5f69 6d70 5f5f 5669 7274 7561  @4.__imp__Virtua
+00009b60: 6c51 7565 7279 4031 3200 5f5f 696d 705f  lQuery@12.__imp_
+00009b70: 5f46 696e 644e 6578 7446 696c 6541 4038  _FindNextFileA@8
+00009b80: 005f 5f5f 746c 735f 7374 6172 745f 5f00  .___tls_start__.
+00009b90: 5f45 6e75 6d57 696e 646f 7773 4038 005f  _EnumWindows@8._
+00009ba0: 5f69 6d70 5f5f 546c 7347 6574 5661 6c75  _imp__TlsGetValu
+00009bb0: 6540 3400 5f5f 6c69 626d 7376 6372 745f  e@4.__libmsvcrt_
+00009bc0: 615f 696e 616d 6500 5f5f 696d 705f 5f49  a_iname.__imp__I
+00009bd0: 6e69 7469 616c 697a 6543 7269 7469 6361  nitializeCritica
+00009be0: 6c53 6563 7469 6f6e 4034 005f 4465 6c65  lSection@4._Dele
+00009bf0: 7465 4372 6974 6963 616c 5365 6374 696f  teCriticalSectio
+00009c00: 6e40 3400 5f5f 7274 5f70 7372 656c 6f63  n@4.__rt_psreloc
+00009c10: 735f 7374 6172 7400 5f5f 696d 705f 5f61  s_start.__imp__a
+00009c20: 626f 7274 005f 5f64 6c6c 5f63 6861 7261  bort.__dll_chara
+00009c30: 6374 6572 6973 7469 6373 5f5f 005f 5f73  cteristics__.__s
+00009c40: 697a 655f 6f66 5f73 7461 636b 5f63 6f6d  ize_of_stack_com
+00009c50: 6d69 745f 5f00 5f5f 7369 7a65 5f6f 665f  mit__.__size_of_
+00009c60: 7374 6163 6b5f 7265 7365 7276 655f 5f00  stack_reserve__.
+00009c70: 5f5f 6d61 6a6f 725f 7375 6273 7973 7465  __major_subsyste
+00009c80: 6d5f 7665 7273 696f 6e5f 5f00 5f5f 5f63  m_version__.___c
+00009c90: 7274 5f78 6c5f 7374 6172 745f 5f00 5f5f  rt_xl_start__.__
+00009ca0: 5f63 7274 5f78 695f 7374 6172 745f 5f00  _crt_xi_start__.
+00009cb0: 5f5f 5f63 7274 5f78 695f 656e 645f 5f00  ___crt_xi_end__.
+00009cc0: 5f5f 696d 705f 5f73 7472 6963 6f6c 6c00  __imp__stricoll.
+00009cd0: 5f5f 696d 705f 5f5f 5f6d 625f 6375 725f  __imp____mb_cur_
+00009ce0: 6d61 7800 5f47 6574 4c61 7374 4572 726f  max._GetLastErro
+00009cf0: 7240 3000 5f5f 696d 705f 5f5f 5f70 5f5f  r@0.__imp____p__
+00009d00: 656e 7669 726f 6e00 5f5f 696d 705f 5f5f  environ.__imp___
+00009d10: 7063 7479 7065 005f 5669 7274 7561 6c51  pctype._VirtualQ
+00009d20: 7565 7279 4031 3200 5f5f 6865 6164 5f6c  uery@12.__head_l
+00009d30: 6962 7573 6572 3332 5f61 005f 6d69 6e67  ibuser32_a._ming
+00009d40: 775f 696e 6974 6c74 7364 726f 745f 666f  w_initltsdrot_fo
+00009d50: 7263 6500 5f5f 696d 705f 5f5f 696f 6200  rce.__imp___iob.
+00009d60: 5f47 6574 4d6f 6475 6c65 4861 6e64 6c65  _GetModuleHandle
+00009d70: 4140 3400 5f5f 5f72 6567 6973 7465 725f  A@4.___register_
+00009d80: 6672 616d 655f 696e 666f 005f 5f6c 6962  frame_info.__lib
+00009d90: 6d6f 6c64 6e61 6d65 5f61 5f69 6e61 6d65  moldname_a_iname
+00009da0: 005f 686d 6f64 5f6c 6962 6763 6300 2e77  ._hmod_libgcc..w
+00009db0: 6561 6b2e 5f5f 5f72 6567 6973 7465 725f  eak.___register_
+00009dc0: 6672 616d 655f 696e 666f 2e5f 5f5f 4548  frame_info.___EH
+00009dd0: 5f46 5241 4d45 5f42 4547 494e 5f5f 005f  _FRAME_BEGIN__._
+00009de0: 5f69 6d70 5f5f 7374 7264 7570 005f 5f69  _imp__strdup.__i
+00009df0: 6d70 5f5f 5f69 7363 7479 7065 005f 5f62  mp___isctype.__b
+00009e00: 7373 5f73 7461 7274 5f5f 005f 5f5f 5255  ss_start__.___RU
+00009e10: 4e54 494d 455f 5053 4555 444f 5f52 454c  NTIME_PSEUDO_REL
+00009e20: 4f43 5f4c 4953 545f 454e 445f 5f00 5f5f  OC_LIST_END__.__
+00009e30: 6670 7265 7365 7400 5f5f 7369 7a65 5f6f  fpreset.__size_o
+00009e40: 665f 6865 6170 5f63 6f6d 6d69 745f 5f00  f_heap_commit__.
+00009e50: 5f5f 696d 705f 5f5f 6572 726e 6f00 5f5f  __imp___errno.__
+00009e60: 5f70 5f5f 656e 7669 726f 6e00 5f5f 696d  _p__environ.__im
+00009e70: 705f 5f47 6574 5072 6f63 4164 6472 6573  p__GetProcAddres
+00009e80: 7340 3800 5f47 6574 5072 6f63 4164 6472  s@8._GetProcAddr
+00009e90: 6573 7340 3800 5f5f 5f63 7274 5f78 705f  ess@8.___crt_xp_
+00009ea0: 7374 6172 745f 5f00 5f5f 696d 705f 5f77  start__.__imp__w
+00009eb0: 6373 746f 6d62 7300 5f47 6574 436f 6d6d  cstombs._GetComm
+00009ec0: 616e 644c 696e 6541 4030 005f 5f69 6d70  andLineA@0.__imp
+00009ed0: 5f5f 4973 5769 6e64 6f77 5669 7369 626c  __IsWindowVisibl
+00009ee0: 6540 3400 5f5f 5f63 7274 5f78 705f 656e  e@4.___crt_xp_en
+00009ef0: 645f 5f00 5f5f 696d 705f 5f73 6967 6e61  d__.__imp__signa
+00009f00: 6c00 5f5f 696d 705f 5f70 7574 7300 5f5f  l.__imp__puts.__
+00009f10: 6d69 6e6f 725f 6f73 5f76 6572 7369 6f6e  minor_os_version
+00009f20: 5f5f 005f 5f69 6d70 5f5f 6174 6578 6974  __.__imp__atexit
+00009f30: 005f 5f69 6d70 5f5f 6d62 7374 6f77 6373  .__imp__mbstowcs
+00009f40: 005f 4973 5769 6e64 6f77 5669 7369 626c  ._IsWindowVisibl
+00009f50: 6540 3400 5f5f 6865 6164 5f6c 6962 6d73  e@4.__head_libms
+00009f60: 7663 7274 5f61 005f 5f69 6d61 6765 5f62  vcrt_a.__image_b
+00009f70: 6173 655f 5f00 5f5f 6973 6374 7970 6500  ase__.__isctype.
+00009f80: 5f5f 7365 6374 696f 6e5f 616c 6967 6e6d  __section_alignm
+00009f90: 656e 745f 5f00 5f4c 6f61 644c 6962 7261  ent__._LoadLibra
+00009fa0: 7279 4140 3400 5f5f 696d 705f 5f47 6574  ryA@4.__imp__Get
+00009fb0: 5769 6e64 6f77 5468 7265 6164 5072 6f63  WindowThreadProc
+00009fc0: 6573 7349 6440 3800 5f77 6373 746f 6d62  essId@8._wcstomb
+00009fd0: 7300 5f5f 696d 705f 5f46 7265 654c 6962  s.__imp__FreeLib
+00009fe0: 7261 7279 4034 005f 5f49 4154 5f65 6e64  rary@4.__IAT_end
+00009ff0: 5f5f 005f 5f68 6561 645f 6c69 626d 6f6c  __.__head_libmol
+0000a000: 646e 616d 655f 6100 5f5f 5255 4e54 494d  dname_a.__RUNTIM
+0000a010: 455f 5053 4555 444f 5f52 454c 4f43 5f4c  E_PSEUDO_RELOC_L
+0000a020: 4953 545f 5f00 5f73 6574 6c6f 6361 6c65  IST__._setlocale
+0000a030: 005f 5f69 6d70 5f5f 5f5f 705f 5f66 6d6f  .__imp____p__fmo
+0000a040: 6465 005f 5f74 6c73 5f73 7461 7274 005f  de.__tls_start._
+0000a050: 4578 6974 5072 6f63 6573 7340 3400 5f5f  ExitProcess@4.__
+0000a060: 696d 705f 5f45 6e75 6d57 696e 646f 7773  imp__EnumWindows
+0000a070: 4038 005f 5f69 6d70 5f5f 7374 7263 6f6c  @8.__imp__strcol
+0000a080: 6c00 5f5f 6461 7461 5f65 6e64 5f5f 005f  l.__data_end__._
+0000a090: 5f5f 6765 746d 6169 6e61 7267 7300 5f46  __getmainargs._F
+0000a0a0: 696e 6443 6c6f 7365 4034 005f 5f43 544f  indClose@4.__CTO
+0000a0b0: 525f 4c49 5354 5f5f 005f 6d62 7374 6f77  R_LIST__._mbstow
+0000a0c0: 6373 005f 5f5f 7365 745f 6170 705f 7479  cs.___set_app_ty
+0000a0d0: 7065 005f 5f62 7373 5f65 6e64 5f5f 005f  pe.__bss_end__._
+0000a0e0: 5f43 5254 5f66 6d6f 6465 005f 5f5f 6372  _CRT_fmode.___cr
+0000a0f0: 745f 7863 5f65 6e64 5f5f 005f 5f74 6c73  t_xc_end__.__tls
+0000a100: 5f69 6e64 6578 005f 5f5f 6372 745f 7863  _index.___crt_xc
+0000a110: 5f73 7461 7274 5f5f 005f 5f5f 4354 4f52  _start__.___CTOR
+0000a120: 5f4c 4953 545f 5f00 5f5f 7274 5f70 7372  _LIST__.__rt_psr
+0000a130: 656c 6f63 735f 7369 7a65 005f 5f69 6d70  elocs_size.__imp
+0000a140: 5f5f 6d65 6d63 7079 005f 4669 6e64 4e65  __memcpy._FindNe
+0000a150: 7874 4669 6c65 4140 3800 5f5f 6669 6c65  xtFileA@8.__file
+0000a160: 5f61 6c69 676e 6d65 6e74 5f5f 005f 5f69  _alignment__.__i
+0000a170: 6d70 5f5f 4c65 6176 6543 7269 7469 6361  mp__LeaveCritica
+0000a180: 6c53 6563 7469 6f6e 4034 005f 5f69 6d70  lSection@4.__imp
+0000a190: 5f5f 6174 6f69 005f 5f69 6d70 5f5f 6d61  __atoi.__imp__ma
+0000a1a0: 6c6c 6f63 005f 5f5f 4548 5f46 5241 4d45  lloc.___EH_FRAME
+0000a1b0: 5f42 4547 494e 5f5f 005f 5365 7446 6f72  _BEGIN__._SetFor
+0000a1c0: 6567 726f 756e 6457 696e 646f 7740 3400  egroundWindow@4.
+0000a1d0: 5f5f 6d61 6a6f 725f 6f73 5f76 6572 7369  __major_os_versi
+0000a1e0: 6f6e 5f5f 005f 5f69 6d70 5f5f 7265 616c  on__.__imp__real
+0000a1f0: 6c6f 6300 5f5f 4941 545f 7374 6172 745f  loc.__IAT_start_
+0000a200: 5f00 5f73 7472 6963 6f6c 6c00 5f5f 746c  _._stricoll.__tl
+0000a210: 735f 656e 6400 5f5f 696d 705f 5f47 6574  s_end.__imp__Get
+0000a220: 4d6f 6475 6c65 4861 6e64 6c65 4140 3400  ModuleHandleA@4.
+0000a230: 5f5f 4454 4f52 5f4c 4953 545f 5f00 5f5f  __DTOR_LIST__.__
+0000a240: 696d 705f 5f5f 6670 7265 7365 7400 2e77  imp___fpreset..w
+0000a250: 6561 6b2e 5f5f 5f64 6572 6567 6973 7465  eak.___deregiste
+0000a260: 725f 6672 616d 655f 696e 666f 2e5f 5f5f  r_frame_info.___
+0000a270: 4548 5f46 5241 4d45 5f42 4547 494e 5f5f  EH_FRAME_BEGIN__
+0000a280: 005f 456e 7465 7243 7269 7469 6361 6c53  ._EnterCriticalS
+0000a290: 6563 7469 6f6e 4034 005f 5f66 756c 6c70  ection@4.__fullp
+0000a2a0: 6174 6800 5f5f 7369 7a65 5f6f 665f 6865  ath.__size_of_he
+0000a2b0: 6170 5f72 6573 6572 7665 5f5f 005f 5f5f  ap_reserve__.___
+0000a2c0: 6372 745f 7874 5f73 7461 7274 5f5f 005f  crt_xt_start__._
+0000a2d0: 5f5f 496d 6167 6542 6173 6500 5f5f 7375  __ImageBase.__su
+0000a2e0: 6273 7973 7465 6d5f 5f00 5f5f 696d 705f  bsystem__.__imp_
+0000a2f0: 5f73 7472 6c65 6e00 2e77 6561 6b2e 5f5f  _strlen..weak.__
+0000a300: 4a76 5f52 6567 6973 7465 7243 6c61 7373  Jv_RegisterClass
+0000a310: 6573 2e5f 5f5f 4548 5f46 5241 4d45 5f42  es.___EH_FRAME_B
+0000a320: 4547 494e 5f5f 005f 5f43 5254 5f66 656e  EGIN__.__CRT_fen
+0000a330: 7600 5f5f 696d 705f 5f63 616c 6c6f 6300  v.__imp__calloc.
+0000a340: 5f5f 4a76 5f52 6567 6973 7465 7243 6c61  __Jv_RegisterCla
+0000a350: 7373 6573 005f 4765 7457 696e 646f 7754  sses._GetWindowT
+0000a360: 6872 6561 6450 726f 6365 7373 4964 4038  hreadProcessId@8
+0000a370: 005f 5f69 6d70 5f5f 5f5f 6765 746d 6169  .__imp____getmai
+0000a380: 6e61 7267 7300 5f5f 5f74 6c73 5f65 6e64  nargs.___tls_end
+0000a390: 5f5f 005f 5f69 6d70 5f5f 4578 6974 5072  __.__imp__ExitPr
+0000a3a0: 6f63 6573 7340 3400 5f6d 696e 6777 5f69  ocess@4._mingw_i
+0000a3b0: 6e69 746c 7473 7375 6f5f 666f 7263 6500  nitltssuo_force.
+0000a3c0: 5f49 6e69 7469 616c 697a 6543 7269 7469  _InitializeCriti
+0000a3d0: 6361 6c53 6563 7469 6f6e 4034 005f 5f5f  calSection@4.___
+0000a3e0: 6370 755f 6665 6174 7572 6573 005f 5f69  cpu_features.__i
+0000a3f0: 6d70 5f5f 6672 6565 005f 5f69 6d70 5f5f  mp__free.__imp__
+0000a400: 5365 7455 6e68 616e 646c 6564 4578 6365  SetUnhandledExce
+0000a410: 7074 696f 6e46 696c 7465 7240 3400 5f5f  ptionFilter@4.__
+0000a420: 5f64 6572 6567 6973 7465 725f 6672 616d  _deregister_fram
+0000a430: 655f 696e 666f 005f 5f6d 616a 6f72 5f69  e_info.__major_i
+0000a440: 6d61 6765 5f76 6572 7369 6f6e 5f5f 005f  mage_version__._
+0000a450: 5f6c 6f61 6465 725f 666c 6167 735f 5f00  _loader_flags__.
+0000a460: 5f5f 6c69 6275 7365 7233 325f 615f 696e  __libuser32_a_in
+0000a470: 616d 6500 5f5f 696d 705f 5f53 686f 7757  ame.__imp__ShowW
+0000a480: 696e 646f 7740 3800 5f5f 696d 705f 5f74  indow@8.__imp__t
+0000a490: 6f6c 6f77 6572 005f 5f43 5254 5f67 6c6f  olower.__CRT_glo
+0000a4a0: 6200 5f5f 7365 746d 6f64 6500 5f5f 696d  b.__setmode.__im
+0000a4b0: 705f 5f70 7269 6e74 6600 5f5f 5f63 686b  p__printf.___chk
+0000a4c0: 7374 6b5f 6d73 005f 5f68 6561 645f 6c69  stk_ms.__head_li
+0000a4d0: 626b 6572 6e65 6c33 325f 6100 5f5f 7274  bkernel32_a.__rt
+0000a4e0: 5f70 7372 656c 6f63 735f 656e 6400 5f5f  _psrelocs_end.__
+0000a4f0: 696d 705f 5f5f 6365 7869 7400 5f5f 6d69  imp___cexit.__mi
+0000a500: 6e6f 725f 7375 6273 7973 7465 6d5f 7665  nor_subsystem_ve
+0000a510: 7273 696f 6e5f 5f00 5f5f 696d 705f 5f46  rsion__.__imp__F
+0000a520: 696e 6443 6c6f 7365 4034 005f 5f6d 696e  indClose@4.__min
+0000a530: 6f72 5f69 6d61 6765 5f76 6572 7369 6f6e  or_image_version
+0000a540: 5f5f 005f 5f69 6d70 5f5f 7666 7072 696e  __.__imp__vfprin
+0000a550: 7466 005f 5f69 6d70 5f5f 5f5f 7365 745f  tf.__imp____set_
+0000a560: 6170 705f 7479 7065 005f 6d69 6e67 775f  app_type._mingw_
+0000a570: 696e 6974 6c74 7364 796e 5f66 6f72 6365  initltsdyn_force
+0000a580: 005f 546c 7347 6574 5661 6c75 6540 3400  ._TlsGetValue@4.
+0000a590: 5f5f 696d 705f 5f44 656c 6574 6543 7269  __imp__DeleteCri
+0000a5a0: 7469 6361 6c53 6563 7469 6f6e 4034 005f  ticalSection@4._
+0000a5b0: 4c65 6176 6543 7269 7469 6361 6c53 6563  LeaveCriticalSec
+0000a5c0: 7469 6f6e 4034 005f 5f69 6d70 5f5f 4765  tion@4.__imp__Ge
+0000a5d0: 7443 6f6d 6d61 6e64 4c69 6e65 4140 3000  tCommandLineA@0.
+0000a5e0: 5f5f 696d 705f 5f4c 6f61 644c 6962 7261  __imp__LoadLibra
+0000a5f0: 7279 4140 3400 5f5f 696d 705f 5f73 6574  ryA@4.__imp__set
+0000a600: 6c6f 6361 6c65 005f 5f52 554e 5449 4d45  locale.__RUNTIME
+0000a610: 5f50 5345 5544 4f5f 5245 4c4f 435f 4c49  _PSEUDO_RELOC_LI
+0000a620: 5354 5f45 4e44 5f5f 005f 5f6c 6962 6b65  ST_END__.__libke
+0000a630: 726e 656c 3332 5f61 5f69 6e61 6d65 005f  rnel32_a_iname._
+0000a640: 5f5f 6479 6e5f 746c 735f 696e 6974 5f63  __dyn_tls_init_c
+0000a650: 616c 6c62 6163 6b00 5f5f 746c 735f 7573  allback.__tls_us
+0000a660: 6564 005f 5f69 6d70 5f5f 5365 7446 6f72  ed.__imp__SetFor
+0000a670: 6567 726f 756e 6457 696e 646f 7740 3400  egroundWindow@4.
+0000a680: 5f5f 5f63 7274 5f78 745f 656e 645f 5f00  ___crt_xt_end__.
+0000a690: 5f76 6670 7269 6e74 6600 5f5f 696d 705f  _vfprintf.__imp_
+0000a6a0: 5f45 6e74 6572 4372 6974 6963 616c 5365  _EnterCriticalSe
+0000a6b0: 6374 696f 6e40 3400 5f5f 696d 705f 5f66  ction@4.__imp__f
+0000a6c0: 7772 6974 6500                           write.
```

### Comparing `amiya-0.0.1/src/amiya/bin/get_active_pid.exe` & `amiya-0.0.3/src/amiya/bin/get_active_pid.exe`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 00000010: b800 0000 0000 0000 4000 0000 0000 0000  ........@.......
 00000020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000030: 0000 0000 0000 0000 0000 0000 8000 0000  ................
 00000040: 0e1f ba0e 00b4 09cd 21b8 014c cd21 5468  ........!..L.!Th
 00000050: 6973 2070 726f 6772 616d 2063 616e 6e6f  is program canno
 00000060: 7420 6265 2072 756e 2069 6e20 444f 5320  t be run in DOS 
 00000070: 6d6f 6465 2e0d 0d0a 2400 0000 0000 0000  mode....$.......
-00000080: 5045 0000 4c01 0d00 a526 2b66 0074 0000  PE..L....&+f.t..
+00000080: 5045 0000 4c01 0d00 5065 4266 0074 0000  PE..L...PeBf.t..
 00000090: e301 0000 e000 0701 0b01 021c 002e 0000  ................
 000000a0: 004a 0000 0002 0000 e012 0000 0010 0000  .J..............
 000000b0: 0040 0000 0000 4000 0010 0000 0002 0000  .@....@.........
 000000c0: 0400 0000 0100 0000 0400 0000 0000 0000  ................
-000000d0: 0010 0100 0004 0000 382d 0100 0300 0000  ........8-......
+000000d0: 0010 0100 0004 0000 fa6b 0100 0300 0000  .........k......
 000000e0: 0000 2000 0010 0000 0000 1000 0010 0000  .. .............
 000000f0: 0000 0000 1000 0000 0000 0000 0000 0000  ................
 00000100: 0080 0000 4406 0000 0000 0000 0000 0000  ....D...........
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000140: 04a0 0000 1800 0000 0000 0000 0000 0000  ................
```

### Comparing `amiya-0.0.1/src/amiya/bin/scripts/get_window_size.c` & `amiya-0.0.3/src/amiya/bin/scripts/get_window_size.c`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/entrypoints/__init__.py` & `amiya-0.0.3/src/amiya/entrypoints/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/entrypoints/entrypoint_handler.py` & `amiya-0.0.3/src/amiya/entrypoints/entrypoint_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,92 @@
 import multiprocessing
+import getpass
+import subprocess
 
-from amiya.apps_manager.apps_manager import AppsManager 
-from amiya.exceptions.exceptions import *
-from amiya.utils.helper import *
+from amiya.apps_manager.apps_manager import AppsManager
 from amiya.module_utilities.search_controller import SearchController
 from amiya.module_utilities.power_controller import PowerUtils
+from amiya.module_utilities.cursor_controller import CursorController
+from amiya.module_utilities.continuous_click_controller import ContinuousClickController
+from amiya.module_utilities.dev_features import DevController
+
+from amiya.exceptions.exceptions import *
+from amiya.utils.helper import *
+
 from amiya.scheduler.scheduler import AmiyaScheduler
 from amiya.apps_manager.sync_controller.sys_uuid_controller import SysUUIDController
 from amiya.utils import constants
-from amiya.utils.constants import VERSION
-from amiya.module_utilities.volume_controller import AmiyaVolumeControllerUI, start_volume_control_ui, start_volume_control_ui_detached
+from amiya.utils.constants import VERSION, VERSION_DESC, AUTHOR, AUTHOR_DETAIL, REPOSITORY
+from amiya.module_utilities.volume_controller import AmiyaVolumeControllerUI, start_volume_control_ui
 
 
 
 class AmiyaEntrypointHandler:
     def __init__(self):
         self.apps_manager = AppsManager()
         self.search_controller = SearchController()
         self.power_utils = PowerUtils()
+       
         # self.scheduler = AmiyaScheduler()
 
+
+    # =================================================
+    # =================| DEVELOPMENT | ================
+    # =================================================
+
+    def DEV(self, args):
+        # If "DEVELOPMENT" variable in constants is False, the dev controller cannot be created.
+        self.dev_controller = DevController()
+        
+        if args.objects:
+            self.dev_controller.verbose_objects(
+                self.apps_manager,
+                self.search_controller,
+                self.power_utils
+            )
+        if args.refresh:
+            self.dev_controller.refresh_objects()
+        if args.code:
+            self.dev_controller.open_dev_env()
+        if args.isadmin:
+            self.dev_controller.is_admin()
+    
+    
+    # =================================================
+    # ====================| ABOUT | ===================
+    # =================================================
+    
+    def version(self, args):
+        aprint(f"Amiya {VERSION_DESC}-{VERSION}")
+    
+    def author(self, args):
+        aprint(AUTHOR_DETAIL)
+    
+    def repo(self, args):
+        aprint(REPOSITORY)
+    
+    def print_help(self, args, parser):
+        help_cmd = color_cmd("help", with_quotes=True)
+        aprint(f"Command {help_cmd} is not implemented.")
     
     # =================================================
     # ============| ADD/REMOVE/SHOW APPS | ============
     # =================================================
     
     def add_app(self, args):
         self.apps_manager.create_app_automated()
     
     def remove_app(self, args):
         self.apps_manager.delete_app(args.tag)
     
     def show_apps(self, args):
         self.apps_manager.show_apps()
     
+    def show_app_config_dir(self, args):
+        self.apps_manager.verbose_app_config(args.tag)
     
     # =================================================
     # =================| START APPS | =================
     # =================================================
     
     def start(self, args):
         self.apps_manager.run_app(args.tag)
@@ -64,16 +113,17 @@
     def record_automation_sequences(self, args):
         self.apps_manager.record_sequence(args.tag)
 
     def run_automations_sequences(self, args):
         self.apps_manager.run_sequence(
             tag=args.tag, 
             seq_name=args.seq_name,
-            add_global_delay=args.add_global_delay,
-            terminate_on_finish=args.terminate
+            global_delay=args.global_delay,
+            terminate_on_finish=args.terminate,
+            no_confirmation=args.no_confirmation
         )
 
 
     # =================================================
     # ==========| APP UTILITY FEATURES | ==============
     # =================================================
 
@@ -95,48 +145,85 @@
     def search(self, args):
         if args.search_content:
             self.search_controller.search(args.search_content)
         else:
             self.search_controller.search_automated()
 
     def sleep(self, args, parser):
-        if args.delay:
-            self.power_utils.sleep_pc(args.delay)
-        else:
-            parser.print_help()
+        self.power_utils.sleep_pc(args.delay)
     
     def shutdown(self, args, parser):
-        if args.delay:
-            self.power_utils.shutdown_pc(args.delay)
-        else:
-            parser.print_help()
+        self.power_utils.shutdown_pc(args.delay)
 
 
     def display_system_uuid(self, args):
        SysUUIDController.print_uuid()
 
-
     def open_volume_control_ui(self, args):
         # A new process is used because on closing the UI, a whole bunch of nonsense if printed 
         # in stdout (only happens when using this as an module entrypoint apparantly)
         gui_process = multiprocessing.Process(target=start_volume_control_ui)
         gui_process.start()
         gui_process.join()
     
 
+    def track_cursor(self, args):
+        if args.color:
+            self.cursor_controller = CursorController(verbose_hex=True)
+        else:
+            self.cursor_controller = CursorController(verbose_hex=False)
+        
+        self.cursor_controller.track_cursor()
+
+
+    def click_continuously(self, args):
+        cc_controller = ContinuousClickController()
+        cc_controller.click_continuously(args.count, args.delay, args.hold_time, args.start_after, args.quite)
+
+    def elevate(self, args):
+        if is_admin():
+            aprint("Already running as admin.")
+            return
+        
+        if args.explain:
+            text = """Certain applications necessitate the 'amiya' process to have administrative 
+privileges to replay or record mouse and keyboard actions. To help with this, 
+the 'elevate' command is available to elevate amiya's permissions to an 
+administrative level.
+
+As an open-source project, `amiya` does not possess a Code Signing Certificate 
+due to the associated cost. Without this certificate, Windows will flag the 
+module's publisher as unknown.
+
+By invoking the elevate command, you are granting `amiya` admin access.
+"""
+            aprint(text)
+            ui = input(atext("Proceed to elevate? [y/n] "))
+            if ui.lower() != "y":
+                return
+        
+        script = os.path.abspath(sys.argv[0])
+        params = ' '.join([script])
+        try:
+            subprocess.run(["powershell", "-Command", f"Start-Process -Verb runAs {params}"])
+        except Exception as e:
+            aprint(f"Failed to elevate privileges: {e}")
+        sys.exit(0)
+
     # =================================================
     # ================| SCHEDULER | ===================
     # =================================================
 
     # def run_scheduler(self, args):
     #     self.scheduler.run_scheduler()
 
     # =================================================
     # ===============| OTHER HELPER | =================
     # =================================================
+    
     def print_title(self):
         
         # columns, _ = shutil.get_terminal_size(fallback=(80, 20))
         # bar = '▬' * (columns//1 - 12)
         # bar = Printer.to_lightblue(f"▷ ▷ ▷ {bar} ◁ ◁ ◁")
         # print(bar)
         
@@ -146,48 +233,54 @@
    / \  |  \/  |_ _\ \ / // \     / ___| |   |_ _| 
   / _ \ | |\/| || | \ V // _ \   | |   | |    | |  
  / ___ \| |  | || |  | |/ ___ \  | |___| |___ | |  
 /_/   \_\_|  |_|___| |_/_/   \_\  \____|_____|___|
 """)
         
         desc = Printer.to_purple("""A lightweight cross-platform automation tool for games and daily tasks!""")
-        postfix = Printer.to_lightgrey("https://github.com/ReZeroE/Amiya")
-        author = Printer.to_lightgrey("By Kevin L.")
+        postfix = Printer.to_lightgrey(REPOSITORY)
+        author = Printer.to_lightgrey(f"By {AUTHOR}")
         
         print(center_text(title))
         print_centered(f"{desc}\n{postfix}\n{author}\n")
     
     def print_init_help(self):
         
         access_time = colored(f"Access Time: {DatetimeHandler.get_datetime_str()}", "dark_grey")
+        username = getpass.getuser()
+        isadmin = "ADMIN" if is_admin() else "USER"
         
         quit_cmd = Printer.to_purple("exit")
         cls_cmd = Printer.to_purple("clear")
         help_cmd = Printer.to_purple("help")
         
-        welcome_str = f"Welcome to the Amiya CLI Environment (BETA {VERSION})"
+        welcome_str = f"Welcome to the Amiya CLI Environment ({VERSION_DESC}-{VERSION})"
         exit_str = f"Type '{quit_cmd}' to quit amiya CLI"
         cls_str = f"Type '{cls_cmd}' to clear terminal"
         help_str = f"Type '{help_cmd}' to display commands list"
     
         print(f"{welcome_str}\n  {help_str}\n  {exit_str}\n  {cls_str}\n")
-    
         
+    # =================================================
+    # ===============| CLI DRIVERS | ==================
+    # =================================================
     
     def check_custom_commands(self, user_input: str):
         # Return 0 to continue loop, 1 to short-circit loop and 'continue' loop, 2 to exit loop
 
         if user_input.lower() in ['exit', 'quit']:
             clear_screen()
             return 2
         
         if user_input.lower() in ['clear', "cls", "reset"]:
             clear_screen()
             self.print_title()
-            print("Terminal cleared. Type 'exit' to quit.")
+            
+            exit_cmd = color_cmd("exit", with_quotes=True)
+            print(f"Terminal cleared. Type {exit_cmd} to quit.")
             return 1
         
         if user_input.strip() == '':
             return 1
     
         return 0
     
@@ -219,21 +312,21 @@
         # =============| PARSE ARGUMENT |=============    
                 args = parser.parse_args(user_input.split())
                 if hasattr(args, 'func'):
                     try:
                         args.func(args)
                     except AmiyaExit:
                         continue
+                    # except AmiyaBaseException as ex:
+                    #     aprint(ex, log_type=LogType.ERROR)
+                    #     continue
                 else:
                     parser.print_help()
             
             
         # ==============| ON EXCEPTION |==============
             except KeyboardInterrupt:
                 # print("\nNote: Type 'exit' to quit.")
                 print("")
                 continue
             except SystemExit:
                 continue
-            # except Exception as ex:
-            #     print(ex)
-            #     continue
```

### Comparing `amiya-0.0.1/src/amiya/entrypoints/entrypoints.py` & `amiya-0.0.3/src/amiya/entrypoints/entrypoints.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,66 @@
+import os
 import sys
 import time
 import psutil
 import argparse
+
+import ctypes
+import subprocess
+
 from termcolor import colored
 from amiya.entrypoints.entrypoint_handler import AmiyaEntrypointHandler
-from amiya.utils.helper import aprint, verify_platform, is_admin, Printer
+from amiya.utils.helper import aprint, atext, verify_platform, is_admin, Printer
 from amiya.exceptions.exceptions import AmiyaOSNotSupported, AmiyaExit
 
 
 class AmiyaArgParser(argparse.ArgumentParser):
     def error(self, message):
         command = message.split("'")[1] if "invalid choice:" in message else None
         helpt = Printer.to_purple("help")
         aprint(f"Command not recognized: {command}\nType '{helpt}' for commands list")
         self.exit(2)
         
+        
+
+
 
 def start_amiya():
     entrypoint_handler = AmiyaEntrypointHandler()
     
     parser = AmiyaArgParser(prog='amiya', description="Amiya CLI Automation Package")
     subparsers = parser.add_subparsers(dest='command', help='commands')
 
     help_parser = subparsers.add_parser('help', help='Show this help message and exit')
-    help_parser.set_defaults(func=lambda args: entrypoint_handler.print_help(parser))
+    help_parser.set_defaults(func=lambda args: entrypoint_handler.print_help(args, parser))
 
+    # =================================================
+    # =================| DEVELOPMENT | ================
+    # =================================================
+
+    start_parser = subparsers.add_parser('dev', help='[DEV] Developer\'s commands.')
+    start_parser.add_argument('--objects', '-obj', action='store_true', help='Show all controller objects and their addresses.')
+    start_parser.add_argument('--refresh', '-ref', action='store_true', help='Refresh all controller objects.')
+    start_parser.add_argument('--code', '-c', action='store_true', help='Open development environment with VSCode.')
+    start_parser.add_argument('--isadmin', '-ia', action='store_true', help='Show whether the main thread has admin access.')
+    start_parser.set_defaults(func=entrypoint_handler.DEV)
+
+
+    # =================================================
+    # ====================| ABOUT | ===================
+    # =================================================
+
+    start_parser = subparsers.add_parser('version', help='Verbose module version')
+    start_parser.set_defaults(func=entrypoint_handler.version)
+                              
+    start_parser = subparsers.add_parser('author', help='Verbose module author')
+    start_parser.set_defaults(func=entrypoint_handler.author)
+    
+    start_parser = subparsers.add_parser('repo', help='Verbose module repository link')
+    start_parser.set_defaults(func=entrypoint_handler.repo)
 
     # =================================================
     # ============| ADD/REMOVE/SHOW APPS | ============
     # =================================================
 
     start_parser = subparsers.add_parser('add-app', help='Add a new application')
     start_parser.set_defaults(func=entrypoint_handler.add_app)
@@ -39,14 +71,19 @@
     
     show_apps_parser = subparsers.add_parser('show-apps', help='Show applications')
     show_apps_parser.add_argument('--short', '-s', action='store_true', help='Only show the app ID, name, and verification status')
     show_apps_parser.add_argument('--full-path', '-f', action='store_true', help='Show the full path of the applications')
     show_apps_parser.set_defaults(func=entrypoint_handler.show_apps)
 
 
+    start_parser = subparsers.add_parser('show-config', help='Show application configuration directory')
+    start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application to show the configuration directory of')
+    start_parser.add_argument('--all', '-a', action='store_true', help='Show all configuration directory paths (including automation)')
+    start_parser.set_defaults(func=entrypoint_handler.show_app_config_dir)
+
     # =================================================
     # =================| START APPS | =================
     # =================================================
     
     start_parser = subparsers.add_parser('start', help='Start an application')
     start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application to start')
     start_parser.set_defaults(func=entrypoint_handler.start)
@@ -75,54 +112,73 @@
     start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application')
     start_parser.set_defaults(func=entrypoint_handler.record_automation_sequences)
 
     
     start_parser = subparsers.add_parser('run-auto', help='[Admin Permission Req.] Record an automation sequences of the application')
     start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application')
     start_parser.add_argument('seq_name', nargs='?', default=None, help='Name of the sequence to run')
-    start_parser.add_argument('--add-global-delay', '-g', default=False, action='store_true', help='Add a global delay to the sequence during execution')
+    start_parser.add_argument('--global-delay', '-g', type=int, default=-1, help='Add a global delay to the sequence during execution')
     start_parser.add_argument('--terminate', '-t', default=False, action='store_true', help='Terminate the application on automation completion')
+    start_parser.add_argument('--no-confirmation', '-nc', default=False, action='store_true', help='Run the automation without confirmation')
     start_parser.set_defaults(func=entrypoint_handler.run_automations_sequences)
     
     
     # =================================================
     # ==========| APP UTILITY FEATURES | ==============
     # =================================================
     
-    start_parser = subparsers.add_parser('sync', help='Sync configured applications on new machine')
+    start_parser = subparsers.add_parser('sync', help='Sync configured applications on new machine OR auto configure application executable paths')
     start_parser.set_defaults(func=entrypoint_handler.sync)
     
     start_parser = subparsers.add_parser('cleanup', help='Remove all unverified applications')
     start_parser.set_defaults(func=entrypoint_handler.cleanup)
     
     
     # =================================================
     # =============| UTILITY FEATURES | ===============
     # =================================================
-        
+    
     start_parser = subparsers.add_parser('search', help='Initiate a search on the default browser')
     start_parser.add_argument('search_content', nargs='*', default=None, help='Content of the search')
     start_parser.set_defaults(func=entrypoint_handler.search)
     
     sleep_parser = subparsers.add_parser('sleep', help='Put the PC to sleep after X seconds')
-    sleep_parser.add_argument('delay', nargs='?', default=None, help='Delay in seconds before sleep')
+    sleep_parser.add_argument('delay', nargs='?', type=int, default=0, help='Delay in seconds before sleep')
     sleep_parser.set_defaults(func=lambda args: entrypoint_handler.sleep(args, sleep_parser))
     
     shutdown_parser = subparsers.add_parser('shutdown', help='Shutdown PC after X seconds')
-    shutdown_parser.add_argument('delay', nargs='?', default=None, help='Delay in seconds before shutdown')
+    shutdown_parser.add_argument('delay', nargs='?', type=int, default=0, help='Delay in seconds before shutdown')
     shutdown_parser.set_defaults(func=lambda args: entrypoint_handler.shutdown(args, shutdown_parser))
     
     
     start_parser = subparsers.add_parser('uuid', help='Display system UUID')
     start_parser.set_defaults(func=entrypoint_handler.display_system_uuid)
     
     
+    start_parser = subparsers.add_parser('pixel', help='Track cursor position and color')
+    start_parser.add_argument('--color', '-c', action='store_true', help='Show pixel coordinate as well as the pixel\'s color hex value.')
+    start_parser.set_defaults(func=entrypoint_handler.track_cursor)
+    
+    
     start_parser = subparsers.add_parser('volume', help='Open simple application volume control UI')
     start_parser.set_defaults(func=entrypoint_handler.open_volume_control_ui)
     
+    start_parser = subparsers.add_parser('click', help='Continuously click mouse.')
+    start_parser.add_argument('--count', '-c', type=int, default=-1, help='Number of clicks. Leave empty (default) to run forever')
+    start_parser.add_argument('--delay', '-d', type=int, default=1, help=' Delay (second) between clicks')
+    start_parser.add_argument('--hold-time', '-ht', type=int, default=0.1, help='Delay (second) between click press and release')
+    start_parser.add_argument('--start-after', '-sa', type=int, default=3, help='Delay (second) before the clicks start')
+    start_parser.add_argument('--quite', '-q', action="store_true", default=False, help='Run without verbosing progress')
+    start_parser.set_defaults(func=entrypoint_handler.click_continuously)
+    
+    start_parser = subparsers.add_parser('elevate', help='Elevate `amiya` permissions.')
+    start_parser.add_argument('--explain', action='store_true', help='Explain why this is needed and what will happen.')
+    start_parser.set_defaults(func=entrypoint_handler.elevate)
+    
+    
     # =================================================
     # ================| SCHEDULER | ===================
     # =================================================
     
     # start_parser = subparsers.add_parser('run-scheduler', help='Start and run the scheduler')
     # start_parser.set_defaults(func=entrypoint_handler.run_scheduler)
     
@@ -137,32 +193,33 @@
     
     sync_needed = not entrypoint_handler.apps_synced()
     if sync_needed:
         # If sync is needed, restrict all commands except 'sync'
         def blocked_func(args):
             text = colored('amiya sync', 'light_cyan')
             aprint(f"Applications under Amiya's apps manager are not fully configured to run on this machine.\n\nTo sync the apps to this machine, run `{text}`")
-            exit()
+            raise AmiyaExit()
 
         for name, subparser in subparsers.choices.items():
-            if name not in ["sync", "search", "sleep", "shutdown", "uuid"]:
+            if name not in ["sync", "search", "sleep", "shutdown", "uuid", "show-config", "version", "author", "repo"]:
                 subparser.set_defaults(func=blocked_func)
     
     
     isadmin = is_admin()
     if not isadmin:
         # Certain commands require admin permissions to execute
         def blocked_func(args):
             aprint("Insufficient permission. Please restart the terminal as an administrator.")
-            exit()
+            raise AmiyaExit()
 
         for name, subparser in subparsers.choices.items():
             if name in ["record-auto", "run-auto"]:
                 subparser.set_defaults(func=blocked_func)
     
+    
     # ===========================================================================================
     # >>> PARSER DRIVER
     # ===========================================================================================
     
     # Check if no command line arguments are provided
     if len(sys.argv) == 1:
         entrypoint_handler.start_cli(parser)
@@ -173,8 +230,32 @@
             try:
                 args.func(args)
             except KeyboardInterrupt:
                 print("\nKeyboard Interrupt! Amiya Exiting.")
             except AmiyaExit:
                 exit()
         else:
-            parser.print_help()
+            parser.print_help()
+            
+
+
+def start_amiya_cli_as_admin():
+    start_amiya()
+    
+    # # If process already have admin access
+    # if is_admin():
+    #     start_amiya()
+    #     return
+
+    # # Else, request admin permissions
+    # user_input = input(atext("Amiya is not ran as admin. Would you like to run 'amiya' as admin? [y/n] "))
+    # if user_input.lower() != "y":
+    #     start_amiya()
+    #     return
+    
+    # script = os.path.abspath(sys.argv[0])
+    # params = ' '.join([script] + sys.argv[1:])
+    # try:
+    #     subprocess.run(["powershell", "-Command", f"Start-Process -Verb runAs {params}"])
+    # except Exception as e:
+    #     aprint(f"Failed to elevate privileges: {e}")
+    # sys.exit(0)
```

### Comparing `amiya-0.0.1/src/amiya/exceptions/__init__.py` & `amiya-0.0.3/src/amiya/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/exceptions/exceptions.py` & `amiya-0.0.3/src/amiya/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/module_utilities/power_controller.py` & `amiya-0.0.3/src/amiya/module_utilities/power_controller.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/module_utilities/search_controller.py` & `amiya-0.0.3/src/amiya/module_utilities/search_controller.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/pixel_calculator/pixel_calculator.py` & `amiya-0.0.3/src/amiya/pixel_calculator/pixel_calculator.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,39 @@
         self.prev_monitor_width = monitor_info["width"]
         self.prev_monitor_height = monitor_info["height"]
     
         current_monitor_info = ResolutionDetector.get_primary_monitor_size()
         self.current_monitor_width = current_monitor_info["width"]
         self.current_monitor_height = current_monitor_info["height"]
     
-    def calculate_new_coordinate(self, prev_coor: tuple, prev_window_info: dict):
-        curr_window_info = ResolutionDetector.get_window_size()
+    
+    @staticmethod
+    def transform_coordinate(prev_coor: tuple, prev_window_info: dict):
         
-        if curr_window_info["is_fullscreen"] == True and prev_window_info["is_fullscreen"] == True:
+        try:
+            x, y = prev_coor
             
-            prev_x = prev_coor[0]
-            prev_y = prev_coor[1]
-
-            new_x = self.current_monitor_width / self.prev_monitor_width * prev_x
-            new_y = self.current_monitor_height / self.prev_monitor_height * prev_y  
+            curr_window_info = ResolutionDetector.get_window_size()
+            curr_x = curr_window_info["left"]
+            curr_y = curr_window_info["top"]
+            curr_w = curr_window_info["width"]
+            curr_h = curr_window_info["height"]
             
-            return(int(new_x), int(new_y))  
+            print(curr_x, curr_y, curr_w, curr_h)
             
-        else:
-            print(f"\nCurrent Window: (Width {curr_window_info["width"]}) (Height {curr_window_info["height"]})")
-            print(f"Current Monitor: (Width {self.current_monitor_width}) (Height {self.current_monitor_height})")
-            print(f"Previous Window: (Width {prev_window_info["width"]}) (Height {prev_window_info['height']})")
-            print(f"Previous Monitor: (Width {self.prev_monitor_width}) (Height {self.prev_monitor_height})")
+            prev_x = prev_window_info["left"]
+            prev_y = prev_window_info["top"]
+            prev_w = prev_window_info["width"]
+            prev_h = prev_window_info["height"]
             
-            aprint("[Pixel-Calc] Window size does not match monitor size, pixel calculator returning previous coordinate.", log_type=LogType.WARNING)
-            return None
-    
+            # Normalize the coordinate relative to the original window
+            normalized_x = (x - prev_x) / prev_w
+            normalized_y = (y - prev_y) / prev_h
+
+            new_x = curr_x + normalized_x * curr_w
+            new_y = curr_y + normalized_y * curr_h
+
+            return (int(new_x), int(new_y))
+    
+        except KeyError:
+            # Unavailable for pixel calculator (ver 0.0.2)
+            return prev_coor
```

### Comparing `amiya-0.0.1/src/amiya/pixel_calculator/resolution_detector.py` & `amiya-0.0.3/src/amiya/pixel_calculator/resolution_detector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 import win32process
 import pygetwindow
 from ctypes import windll
 from screeninfo import get_monitors
 
 from amiya.utils.constants import GET_WINDOW_SIZE_EXE
 from amiya.exceptions.exceptions import *
@@ -26,16 +27,18 @@
                     "height": m.height
                 }
                 return monitor_info
         return None
     
     @staticmethod
     def get_window_size():
+        windll.user32.SetProcessDPIAware()
+        
         pid = SafetyMonitor.get_focused_pid()
-        print(f"Currently focused PID: {pid}")
+        # print(f"Currently focused PID: {pid}")
         if pid == None: return None
         
         win_info: dict = ResolutionDetector.get_window_info(pid)
         if win_info == None:
             raise AmiyaBaseException(f"Failed to fetch window size. No results returned (PID {pid}).")
         
         monitor_info = ResolutionDetector.get_primary_monitor_size()
@@ -47,23 +50,26 @@
             win_info["is_fullscreen"] = True
         else:
             win_info["is_fullscreen"] = False
             
         return win_info
         
     @staticmethod
-    def get_window_info(pid):
-        windows = pygetwindow.getWindowsWithTitle('')  # Get all windows
-        for window in windows:
-            _, window_pid = win32process.GetWindowThreadProcessId(window._hWnd)
-            if window_pid == pid:
-                return {
-                    'left'          : window.left,
-                    'top'           : window.top,
-                    'width'         : window.width,
-                    'height'        : window.height,
-                    'is_fullscreen' : None
-                }
+    def get_window_info(pid, retry: int = 5):
+        for _ in range(retry):
+            windows = pygetwindow.getWindowsWithTitle('')  # Get all windows
+            for window in windows:
+                _, window_pid = win32process.GetWindowThreadProcessId(window._hWnd)
+                if window_pid == pid:
+                    if (window.left >= 0 and window.top >= 0) and (window.width > 0 and window.height > 0):
+                        return {
+                            'left'          : window.left,
+                            'top'           : window.top,
+                            'width'         : window.width,
+                            'height'        : window.height,
+                            'is_fullscreen' : None
+                        }
+            time.sleep(1)
         return None
```

### Comparing `amiya-0.0.1/src/amiya/resources/amiya-cli-2.png` & `amiya-0.0.3/src/amiya/resources/amiya-cli-2.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/resources/amiya-cli-3.png` & `amiya-0.0.3/src/amiya/resources/amiya-cli-3.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/resources/amiya-cli-4.png` & `amiya-0.0.3/src/amiya/resources/amiya-cli-4.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/resources/amiya-cli.png` & `amiya-0.0.3/src/amiya/resources/amiya-cli.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/resources/amiya.png` & `amiya-0.0.3/src/amiya/resources/amiya.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/resources/amiya_with_border.png` & `amiya-0.0.3/src/amiya/resources/amiya_with_border.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/resources/code_snippets/add-app.png` & `amiya-0.0.3/src/amiya/resources/code_snippets/add-app.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/resources/code_snippets/add-tag.png` & `amiya-0.0.3/src/amiya/resources/code_snippets/add-tag.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/resources/code_snippets/start.png` & `amiya-0.0.3/src/amiya/resources/code_snippets/start.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/scheduler/scheduler.py` & `amiya-0.0.3/src/amiya/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/scheduler/scheduler_config_handler.py` & `amiya-0.0.3/src/amiya/scheduler/scheduler_config_handler.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/utils/helper.py` & `amiya-0.0.3/src/amiya/utils/helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import os
 import re
 import sys
 import shutil
+import threading
+import pyautogui
+import psutil
+import pygetwindow as gw
+import win32gui, win32process, psutil
 from enum import Enum
+from screeninfo import get_monitors
 from datetime import datetime
 from termcolor import colored
 from amiya.utils import constants
 from amiya.utils.constants import BASENAME, DATETIME_FORMAT, TIME_FORMAT # "Amiya"
 
 def verify_platform() -> bool:
     """
@@ -39,24 +45,28 @@
     if "\n" in text and new_line_no_prefix == True:
         text = text.replace("\n", f"\n        ")
     
     rtext = atext(text, log_type)
     print(rtext, end=end, file=sys.stdout)
     sys.stdout.flush()
 
-def color_cmd(text: str):
+def color_cmd(text: str, with_quotes: bool = False):
     text = text.lower()
     
     if constants.CLI_MODE == True:
         text = text.replace("amiya ", "")
     else:
         if not text.startswith("amiya"):
             text = f"amiya {text}"
+            
+    colored_cmd = colored(text, "light_cyan")
     
-    return colored(text, "light_cyan")
+    if with_quotes:
+        return f"'{colored_cmd}'"
+    return colored_cmd
 
 # =================================================
 # ============| CENTER TEXT HELPER | ==============
 # =================================================
 
 # DON"T CHANGE THE FOLLOWING TWO CENTER TEXT FUNCTIONS. I GOT THESE TO WORK AFTER HOURS. BOTH ARE NEEDED!
 
@@ -126,21 +136,20 @@
     
     @staticmethod
     def to_lightred(text):
         return Printer.hex_text(text, "#f27e82")
 
     
 
-def bool_to_str(boolean: bool):
-    
+def bool_to_str(boolean: bool, true_text="Valid", false_text="Invalid"):
     CHECKMARK = "\u2713"
     CROSSMARK = "\u2717"
     if boolean:
-        return Printer.to_lightgreen(f"{CHECKMARK} Valid")
-    return Printer.to_lightred(f"{CROSSMARK} Invalid")
+        return Printer.to_lightgreen(f"{CHECKMARK} {true_text}")
+    return Printer.to_lightred(f"{CROSSMARK} {false_text}")
 
 # ========================================================
 # =============| PERMISSION VERIFICATION | ===============
 # ========================================================
 
 import os
 import sys
@@ -179,14 +188,15 @@
     show(0.1) # avoid div/0 
     for i, item in enumerate(it):
         yield item
         show(i+1)
     print("", flush=True, file=out)
     
 
+
 # ===================================================
 # ===============| SCREEN HELPER | ==================
 # ===================================================
 
 def clear_screen():
     os.system('cls')
     
@@ -230,8 +240,95 @@
     def datetime_to_str(datetime: datetime):
         return datetime.strftime(DATETIME_FORMAT)
     
     @staticmethod
     def str_to_datetime(datetime_str: str):
         return datetime.strptime(datetime_str, DATETIME_FORMAT)
     
-    
+    
+    
+# ===================================================
+# ===========| MESSAGE WITH SPINNER | ===============
+# ===================================================
+
+class SpinnerMessage(threading.Thread):
+    def __init__(self, start_message, end_message, spin_delay):
+        super().__init__()
+        self.running = False
+        self.start_message = start_message
+        self.end_message = end_message
+        self.spin_delay = spin_delay
+
+    def verbose_start(self):
+        self.running = True
+        self.start()
+
+    def verbose_end(self):
+        self.running = False
+        self.join()
+        time.sleep(0.1)
+        aprint(f"\n{self.end_message}")
+
+    def run(self):
+        try:
+            while self.running:
+                for char in '|/-\\':
+                    aprint(self.start_message + " " + char, end="\r", file=sys.stdout)
+                    sys.stdout.flush()
+                    time.sleep(self.spin_delay)
+        except KeyboardInterrupt:
+            pass
+        
+# ===================================================
+# ==============| TERMINAL RESIZE | =================
+# ===================================================
+        
+import shutil
+
+def get_terminal_size():
+    cols, rows = shutil.get_terminal_size()
+    return cols, rows
+
+
+def resize_terminal(min_cols, min_rows):
+    # Get the current size
+    current_cols, current_rows = shutil.get_terminal_size()
+
+    if current_cols < min_cols:
+        # Set the desired size
+        os.system(f'mode con: cols={min_cols+5} lines={current_rows}')
+        
+    if current_rows < min_rows:
+        # Set the desired size
+        os.system(f'mode con: cols={current_cols} lines={min_rows+5}')
+
+# ===================================================
+# ==============| TERMINAL RESIZE | =================
+# ===================================================
+
+class WindowUtils:
+
+    @staticmethod
+    def bring_to_foreground(pid):
+        # Try to find the window associated with the PID
+        for proc in psutil.process_iter(['pid', 'name']):
+            if proc.info['pid'] == pid:
+                # Get all windows and check if any belong to the target process
+                for window in gw.getAllWindows():
+                    if window._hWnd == win32gui.FindWindow(None, window.title):
+                        _, window_pid = win32process.GetWindowThreadProcessId(window._hWnd)
+                        if window_pid == pid:
+                            if window.isMinimized:
+                                window.restore()
+                            window.activate()
+                            pyautogui.click(window.left + window.width // 2, window.top + window.height // 2)
+                            return True
+        return False
+
+    @staticmethod
+    def active_window_process_name():
+        try:
+            _, process_ids = win32process.GetWindowThreadProcessId(win32gui.GetForegroundWindow())
+            thread_id, pid = process_ids
+            return (psutil.Process(pid).name(), thread_id, pid)
+        except:
+            return None
```

### Comparing `amiya-0.0.1/src/amiya/utils/json_handler.py` & `amiya-0.0.3/src/amiya/utils/json_handler.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya/utils/pynput_mapping.py` & `amiya-0.0.3/src/amiya/utils/pynput_mapping.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.1/src/amiya.egg-info/PKG-INFO` & `amiya-0.0.3/src/amiya.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: amiya
-Version: 0.0.1
+Version: 0.0.3
 Summary: A lightweight cross-platform automation tool for games and daily tasks!
 Home-page: http://github.com/rezeroe/amiya
 Author: Kevin L.
 Author-email: kevinliu@vt.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pywin32
 Requires-Dist: psutil
 Requires-Dist: pynput
 Requires-Dist: pyautogui
@@ -20,29 +20,32 @@
 Requires-Dist: setuptools
 Requires-Dist: elevate
 Requires-Dist: termcolor
 Requires-Dist: schedule
 Requires-Dist: screeninfo
 Requires-Dist: customtkinter
 Requires-Dist: pycaw
+Requires-Dist: Pillow
+
+# Amiya
+Amiya - a lightweight cross-platform automation tool that allows scheduled start and automation of any application from the CLI.
 
-# Amiya (in development)
-Amiya - a lightweight cross-platform automation tool that allows scheduled start and automation of any application from the CLI. 
 
 <div align="center">
     <p style="padding-bottom: 0">
         <img src="https://i.imgur.com/l6VZmHq.png" alt="Amiya Icon" width="85%" height="auto"/>
     </p>
     <!-- <span style="color: #093163">A lightweight cross-platform automation tool for daily tasks!</span> -->
 </div>
 
 
 ## Overview
-Amiya is a easy-to-use and versatile cross-platform application and game automation tool designed for efficiency and ease of use directly from the CLI. This package offers automation capabilities for any applications (including games), enabling users to start and control any application with simple CLI commands.
+_This project is currently in development (`Development Status :: 4 - Beta`)._
 
+Amiya is a easy-to-use and versatile cross-platform application and game automation tool designed for efficiency and ease of use directly from the CLI. This package offers automation capabilities for any applications (including games), enabling users to start and control any application with simple CLI commands.
 
 
 The primary features supported by the `amiya` package are:
 1. **Application Launcher**: Start and terminate any applications from the CLI
 2. **Automation Controller**: Automate any applications with recorded mouse & keyboard sequences
 3. **Scheduling**: Schedule the start/automation of any application to run at any time
 4. **Other Utilities** Other lightweight quality-of-life utilities for applications:
```

### Comparing `amiya-0.0.1/src/amiya.egg-info/SOURCES.txt` & `amiya-0.0.3/src/amiya.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,27 @@
 src/amiya/amiya.py
 src/amiya.egg-info/PKG-INFO
 src/amiya.egg-info/SOURCES.txt
 src/amiya.egg-info/dependency_links.txt
 src/amiya.egg-info/entry_points.txt
 src/amiya.egg-info/requires.txt
 src/amiya.egg-info/top_level.txt
+src/amiya/apps/afk-journey/app-config.json
+src/amiya/apps/afk-journey/automation/sequence/daily.json
+src/amiya/apps/chrome/app-config.json
+src/amiya/apps/genshin-impact/app-config.json
+src/amiya/apps/honkai-star-rail/app-config.json
+src/amiya/apps/ld-player/app-config.json
+src/amiya/apps/ld-player/automation/sequence/arknights-base.json
+src/amiya/apps/ld-player/automation/sequence/arknights-start.json
+src/amiya/apps/league-of-legends/app-config.json
+src/amiya/apps/persona-5-x/app-config.json
+src/amiya/apps/persona-5-x/automation/sequence/daily.json
+src/amiya/apps/persona-5-x/automation/sequence/test.json
+src/amiya/apps/steam/app-config.json
 src/amiya/apps_manager/__init__.py
 src/amiya/apps_manager/app.py
 src/amiya/apps_manager/apps_manager.py
 src/amiya/apps_manager/apps_viewer.py
 src/amiya/apps_manager/safety_monitor.py
 src/amiya/apps_manager/test.py
 src/amiya/apps_manager/sync_controller/__init__.py
@@ -28,23 +41,27 @@
 src/amiya/automation_handler/automation_viewer.py
 src/amiya/automation_handler/units/__init__.py
 src/amiya/automation_handler/units/action.py
 src/amiya/automation_handler/units/plate.py
 src/amiya/automation_handler/units/sequence.py
 src/amiya/bin/focus_pid.exe
 src/amiya/bin/get_active_pid.exe
+src/amiya/bin/get_window_size.exe
 src/amiya/bin/scripts/focus_pid.c
 src/amiya/bin/scripts/get_active_pid.c
 src/amiya/bin/scripts/get_window_size.c
 src/amiya/entrypoints/__init__.py
 src/amiya/entrypoints/entrypoint_handler.py
 src/amiya/entrypoints/entrypoints.py
 src/amiya/exceptions/__init__.py
 src/amiya/exceptions/exceptions.py
 src/amiya/module_utilities/__init__.py
+src/amiya/module_utilities/continuous_click_controller.py
+src/amiya/module_utilities/cursor_controller.py
+src/amiya/module_utilities/dev_features.py
 src/amiya/module_utilities/power_controller.py
 src/amiya/module_utilities/search_controller.py
 src/amiya/module_utilities/volume_controller.py
 src/amiya/pixel_calculator/__init__.py
 src/amiya/pixel_calculator/pixel_calculator.py
 src/amiya/pixel_calculator/resolution_detector.py
 src/amiya/resources/amiya-cli-2.png
@@ -59,19 +76,8 @@
 src/amiya/scheduler/__init__.py
 src/amiya/scheduler/scheduler.py
 src/amiya/scheduler/scheduler_config_handler.py
 src/amiya/utils/__init__.py
 src/amiya/utils/constants.py
 src/amiya/utils/helper.py
 src/amiya/utils/json_handler.py
-src/amiya/utils/pynput_mapping.py
-test/test1.py
-test/test10.py
-test/test11.py
-test/test2.py
-test/test3.py
-test/test4.py
-test/test5.py
-test/test6.py
-test/test7.py
-test/test8.py
-test/test9.py
+src/amiya/utils/pynput_mapping.py
```

