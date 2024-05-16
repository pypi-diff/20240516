# Comparing `tmp/meerschaum-2.2.0.dev3.tar.gz` & `tmp/meerschaum-2.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-2.2.0.dev3.tar", last modified: Tue May 14 04:28:02 2024, max compression
+gzip compressed data, was "meerschaum-2.2.0rc1.tar", last modified: Thu May 16 05:35:41 2024, max compression
```

## Comparing `meerschaum-2.2.0.dev3.tar` & `meerschaum-2.2.0rc1.tar`

### file list

```diff
@@ -1,299 +1,300 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.039032 meerschaum-2.2.0.dev3/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0.dev3/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0.dev3/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23381 2024-05-14 04:28:02.039032 meerschaum-2.2.0.dev3/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.994032 meerschaum-2.2.0.dev3/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.995032 meerschaum-2.2.0.dev3/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.995032 meerschaum-2.2.0.dev3/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.995032 meerschaum-2.2.0.dev3/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4824 2024-03-06 17:41:41.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.995032 meerschaum-2.2.0.dev3/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.996032 meerschaum-2.2.0.dev3/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.996032 meerschaum-2.2.0.dev3/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.996032 meerschaum-2.2.0.dev3/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.997032 meerschaum-2.2.0.dev3/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:01.999032 meerschaum-2.2.0.dev3/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0.dev3/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0.dev3/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0.dev3/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0.dev3/meerschaum/actions/pause.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev3/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0.dev3/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26212 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0.dev3/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev3/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0.dev3/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/actions/tag.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.000032 meerschaum-2.2.0.dev3/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7694 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev3/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0.dev3/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.001032 meerschaum-2.2.0.dev3/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.002032 meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.002032 meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32346 2024-05-10 18:44:59.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.003032 meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18496 2024-05-10 18:08:18.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3115 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/websockets.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/api/dash/webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.003032 meerschaum-2.2.0.dev3/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0.dev3/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.003032 meerschaum-2.2.0.dev3/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.003032 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.004032 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/styles.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/xterm.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.004032 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.004032 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/js/main.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/js/terminado.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/js/xterm.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.004032 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.005032 meerschaum-2.2.0.dev3/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4443 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.005032 meerschaum-2.2.0.dev3/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1935 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6151 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_version.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/api/routes/_webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.005032 meerschaum-2.2.0.dev3/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0.dev3/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.006032 meerschaum-2.2.0.dev3/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5184 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1073 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7983 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev3/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4120 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev3/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       76 2024-05-14 04:27:49.000000 meerschaum-2.2.0.dev3/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.006032 meerschaum-2.2.0.dev3/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.006032 meerschaum-2.2.0.dev3/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9012 2024-05-10 20:46:41.000000 meerschaum-2.2.0.dev3/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.007032 meerschaum-2.2.0.dev3/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-2.2.0.dev3/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.007032 meerschaum-2.2.0.dev3/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.007032 meerschaum-2.2.0.dev3/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.007032 meerschaum-2.2.0.dev3/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.007032 meerschaum-2.2.0.dev3/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4361 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.007032 meerschaum-2.2.0.dev3/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12023 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.009032 meerschaum-2.2.0.dev3/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/_request.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.009032 meerschaum-2.2.0.dev3/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.011032 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11522 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10375 2024-03-26 20:20:31.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6447 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_instance.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   100925 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8323 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34262 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.011032 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev3/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.011032 meerschaum-2.2.0.dev3/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.013032 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.013032 meerschaum-2.2.0.dev3/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev3/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.014032 meerschaum-2.2.0.dev3/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2448 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev3/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev3/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev3/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.014032 meerschaum-2.2.0.dev3/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34013 2024-05-07 20:28:41.000000 meerschaum-2.2.0.dev3/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20760 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.016032 meerschaum-2.2.0.dev3/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/utils/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/utils/_get_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.016032 meerschaum-2.2.0.dev3/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32192 2024-03-26 19:31:51.000000 meerschaum-2.2.0.dev3/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19362 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev3/meerschaum/utils/daemon/RotatingFile.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8174 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0.dev3/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/utils/dataframe.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0.dev3/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.017032 meerschaum-2.2.0.dev3/meerschaum/utils/dtypes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0.dev3/meerschaum/utils/dtypes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/meerschaum/utils/dtypes/sql.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.017032 meerschaum-2.2.0.dev3/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev3/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev3/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev3/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.017032 meerschaum-2.2.0.dev3/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    56682 2024-05-13 18:49:36.000000 meerschaum-2.2.0.dev3/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7970 2024-05-13 21:25:38.000000 meerschaum-2.2.0.dev3/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0.dev3/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-10-04 03:17:38.000000 meerschaum-2.2.0.dev3/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10311 2024-05-14 04:27:40.000000 meerschaum-2.2.0.dev3/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev3/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2472 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0.dev3/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.018032 meerschaum-2.2.0.dev3/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev3/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev3/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev3/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0.dev3/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.019032 meerschaum-2.2.0.dev3/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23381 2024-05-14 04:28:01.000000 meerschaum-2.2.0.dev3/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8405 2024-05-14 04:28:01.000000 meerschaum-2.2.0.dev3/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-14 04:28:01.000000 meerschaum-2.2.0.dev3/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-14 04:28:01.000000 meerschaum-2.2.0.dev3/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4701 2024-05-14 04:28:01.000000 meerschaum-2.2.0.dev3/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-14 04:28:01.000000 meerschaum-2.2.0.dev3/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-14 04:28:01.000000 meerschaum-2.2.0.dev3/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-14 04:28:02.039032 meerschaum-2.2.0.dev3/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3106 2023-08-28 22:18:03.000000 meerschaum-2.2.0.dev3/setup.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-14 04:28:02.018032 meerschaum-2.2.0.dev3/tests/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev3/tests/test_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0.dev3/tests/test_pipes_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/tests/test_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21818 2024-05-10 21:08:07.000000 meerschaum-2.2.0.dev3/tests/test_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/tests/test_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev3/tests/test_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.637744 meerschaum-2.2.0rc1/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc1/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc1/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23441 2024-05-16 05:35:41.637744 meerschaum-2.2.0rc1/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.588744 meerschaum-2.2.0rc1/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.589744 meerschaum-2.2.0rc1/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0rc1/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.589744 meerschaum-2.2.0rc1/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0rc1/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0rc1/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.589744 meerschaum-2.2.0rc1/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4806 2024-05-15 15:21:26.000000 meerschaum-2.2.0rc1/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.589744 meerschaum-2.2.0rc1/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.590744 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.590744 meerschaum-2.2.0rc1/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.590744 meerschaum-2.2.0rc1/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.591745 meerschaum-2.2.0rc1/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.594744 meerschaum-2.2.0rc1/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0rc1/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0rc1/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc1/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc1/meerschaum/actions/pause.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc1/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28057 2024-05-16 03:38:37.000000 meerschaum-2.2.0rc1/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0rc1/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0rc1/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/actions/tag.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.594744 meerschaum-2.2.0rc1/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7694 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc1/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.595744 meerschaum-2.2.0rc1/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.596744 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.597744 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32346 2024-05-10 18:44:59.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.597744 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18496 2024-05-10 18:08:18.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3115 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/websockets.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.598744 meerschaum-2.2.0rc1/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0rc1/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.598744 meerschaum-2.2.0rc1/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.598744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.599744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/styles.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/xterm.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.599744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.599744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/main.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/terminado.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/xterm.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.600744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.600744 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4443 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.601744 meerschaum-2.2.0rc1/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1935 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6151 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_version.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.601744 meerschaum-2.2.0rc1/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc1/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5184 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1073 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7983 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4120 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       74 2024-05-15 19:44:53.000000 meerschaum-2.2.0rc1/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9012 2024-05-10 20:46:41.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4361 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.604744 meerschaum-2.2.0rc1/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc1/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12023 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc1/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.605744 meerschaum-2.2.0rc1/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_request.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.605744 meerschaum-2.2.0rc1/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0rc1/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.606744 meerschaum-2.2.0rc1/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11522 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10375 2024-03-26 20:20:31.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6447 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_instance.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   100925 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8323 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.606744 meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.606744 meerschaum-2.2.0rc1/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.608744 meerschaum-2.2.0rc1/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.608744 meerschaum-2.2.0rc1/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.608744 meerschaum-2.2.0rc1/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2448 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.608744 meerschaum-2.2.0rc1/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34013 2024-05-07 20:28:41.000000 meerschaum-2.2.0rc1/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20760 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.610744 meerschaum-2.2.0rc1/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/_get_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.611744 meerschaum-2.2.0rc1/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33047 2024-05-16 05:26:37.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1813 2024-05-16 05:29:15.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/FileDescriptorInterceptor.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22775 2024-05-16 05:30:05.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/RotatingFile.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8174 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/utils/dataframe.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc1/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.611744 meerschaum-2.2.0rc1/meerschaum/utils/dtypes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0rc1/meerschaum/utils/dtypes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/utils/dtypes/sql.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.611744 meerschaum-2.2.0rc1/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.612744 meerschaum-2.2.0rc1/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    57032 2024-05-15 15:40:39.000000 meerschaum-2.2.0rc1/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7968 2024-05-16 05:34:17.000000 meerschaum-2.2.0rc1/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc1/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-10-04 03:17:38.000000 meerschaum-2.2.0rc1/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10020 2024-05-16 04:42:13.000000 meerschaum-2.2.0rc1/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc1/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2472 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0rc1/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.612744 meerschaum-2.2.0rc1/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc1/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.613744 meerschaum-2.2.0rc1/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23441 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8458 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4726 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-16 05:35:41.637744 meerschaum-2.2.0rc1/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3254 2024-05-15 14:36:58.000000 meerschaum-2.2.0rc1/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.613744 meerschaum-2.2.0rc1/tests/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/tests/test_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc1/tests/test_pipes_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/tests/test_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21818 2024-05-10 21:08:07.000000 meerschaum-2.2.0rc1/tests/test_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/tests/test_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/tests/test_verify.py
```

### Comparing `meerschaum-2.2.0.dev3/LICENSE` & `meerschaum-2.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/PKG-INFO` & `meerschaum-2.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0.dev3
+Version: 2.2.0rc1
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -57,18 +57,18 @@
 Requires-Dist: aiofiles>=0.6.0; extra == "required"
 Requires-Dist: packaging>=21.3.0; extra == "required"
 Requires-Dist: prompt-toolkit>=3.0.39; extra == "required"
 Requires-Dist: more-itertools>=8.7.0; extra == "required"
 Requires-Dist: python-daemon>=0.2.3; extra == "required"
 Requires-Dist: fasteners>=0.18.0; extra == "required"
 Requires-Dist: psutil>=5.8.0; extra == "required"
-Requires-Dist: watchgod>=0.7.0; extra == "required"
+Requires-Dist: watchfiles>=0.21.0; extra == "required"
 Requires-Dist: dill>=0.3.3; extra == "required"
 Requires-Dist: virtualenv>=20.1.0; extra == "required"
-Requires-Dist: apscheduler>=4.0.0a4; extra == "required"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "required"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
 Requires-Dist: duckdb>=0.9.0; extra == "drivers"
@@ -91,14 +91,15 @@
 Requires-Dist: twine>=3.2.0; extra == "dev-tools"
 Requires-Dist: tuna>=0.5.3; extra == "dev-tools"
 Requires-Dist: snakeviz>=2.1.0; extra == "dev-tools"
 Requires-Dist: mypy>=0.812.0; extra == "dev-tools"
 Requires-Dist: pytest>=6.2.2; extra == "dev-tools"
 Requires-Dist: pytest-xdist>=3.2.1; extra == "dev-tools"
 Requires-Dist: heartrate>=0.2.1; extra == "dev-tools"
+Requires-Dist: build>=1.2.1; extra == "dev-tools"
 Provides-Extra: setup
 Provides-Extra: docs
 Requires-Dist: mkdocs>=1.1.2; extra == "docs"
 Requires-Dist: mkdocs-material>=6.2.5; extra == "docs"
 Requires-Dist: mkdocs-material-extensions>=1.0.3; extra == "docs"
 Requires-Dist: mkdocs-autolinks-plugin>=0.2.0; extra == "docs"
 Requires-Dist: mkdocs-awesome-pages-plugin>=2.5.0; extra == "docs"
@@ -148,18 +149,18 @@
 Requires-Dist: aiofiles>=0.6.0; extra == "sql"
 Requires-Dist: packaging>=21.3.0; extra == "sql"
 Requires-Dist: prompt-toolkit>=3.0.39; extra == "sql"
 Requires-Dist: more-itertools>=8.7.0; extra == "sql"
 Requires-Dist: python-daemon>=0.2.3; extra == "sql"
 Requires-Dist: fasteners>=0.18.0; extra == "sql"
 Requires-Dist: psutil>=5.8.0; extra == "sql"
-Requires-Dist: watchgod>=0.7.0; extra == "sql"
+Requires-Dist: watchfiles>=0.21.0; extra == "sql"
 Requires-Dist: dill>=0.3.3; extra == "sql"
 Requires-Dist: virtualenv>=20.1.0; extra == "sql"
-Requires-Dist: apscheduler>=4.0.0a4; extra == "sql"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "sql"
 Provides-Extra: dash
 Requires-Dist: Flask-Compress>=1.10.1; extra == "dash"
 Requires-Dist: dash>=2.6.2; extra == "dash"
 Requires-Dist: dash-bootstrap-components>=1.2.1; extra == "dash"
 Requires-Dist: dash-ace>=0.2.1; extra == "dash"
 Requires-Dist: dash-extensions>=1.0.4; extra == "dash"
 Requires-Dist: dash-daq>=0.5.0; extra == "dash"
@@ -206,18 +207,18 @@
 Requires-Dist: aiofiles>=0.6.0; extra == "api"
 Requires-Dist: packaging>=21.3.0; extra == "api"
 Requires-Dist: prompt-toolkit>=3.0.39; extra == "api"
 Requires-Dist: more-itertools>=8.7.0; extra == "api"
 Requires-Dist: python-daemon>=0.2.3; extra == "api"
 Requires-Dist: fasteners>=0.18.0; extra == "api"
 Requires-Dist: psutil>=5.8.0; extra == "api"
-Requires-Dist: watchgod>=0.7.0; extra == "api"
+Requires-Dist: watchfiles>=0.21.0; extra == "api"
 Requires-Dist: dill>=0.3.3; extra == "api"
 Requires-Dist: virtualenv>=20.1.0; extra == "api"
-Requires-Dist: apscheduler>=4.0.0a4; extra == "api"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "api"
 Requires-Dist: pprintpp>=0.4.0; extra == "api"
 Requires-Dist: asciitree>=0.3.3; extra == "api"
 Requires-Dist: typing-extensions>=4.7.1; extra == "api"
 Requires-Dist: pygments>=2.7.2; extra == "api"
 Requires-Dist: colorama>=0.4.3; extra == "api"
 Requires-Dist: rich>=13.4.2; extra == "api"
 Requires-Dist: more-termcolor>=1.1.3; extra == "api"
@@ -253,18 +254,18 @@
 Requires-Dist: aiofiles>=0.6.0; extra == "full"
 Requires-Dist: packaging>=21.3.0; extra == "full"
 Requires-Dist: prompt-toolkit>=3.0.39; extra == "full"
 Requires-Dist: more-itertools>=8.7.0; extra == "full"
 Requires-Dist: python-daemon>=0.2.3; extra == "full"
 Requires-Dist: fasteners>=0.18.0; extra == "full"
 Requires-Dist: psutil>=5.8.0; extra == "full"
-Requires-Dist: watchgod>=0.7.0; extra == "full"
+Requires-Dist: watchfiles>=0.21.0; extra == "full"
 Requires-Dist: dill>=0.3.3; extra == "full"
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
-Requires-Dist: apscheduler>=4.0.0a4; extra == "full"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
 Requires-Dist: duckdb>=0.9.0; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
```

### Comparing `meerschaum-2.2.0.dev3/README.md` & `meerschaum-2.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/__main__.py` & `meerschaum-2.2.0rc1/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/arguments/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/arguments/_parser.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/arguments/_parser.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/docs/index.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/entry.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                     + (f"\n{args_text}" if args_text else '')
                     + f"\n    {argparse_exception}"
                 )
             )
 
     if args.get('schedule', None):
         from meerschaum.utils.schedule import schedule_function
-        return schedule_function(entry_with_args, args['schedule'], **args)
+        return schedule_function(entry_with_args, **args)
     return entry_with_args(**args)
 
 
 def entry_with_args(
         _actions: Optional[Dict[str, Callable[[Any], SuccessTuple]]] = None,
         **kw
     ) -> SuccessTuple:
```

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/gui/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/gui/app/actions.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/shell/Shell.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/term/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/_internal/term/tools.py` & `meerschaum-2.2.0rc1/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/api.py` & `meerschaum-2.2.0rc1/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/bootstrap.py` & `meerschaum-2.2.0rc1/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/clear.py` & `meerschaum-2.2.0rc1/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/copy.py` & `meerschaum-2.2.0rc1/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/deduplicate.py` & `meerschaum-2.2.0rc1/meerschaum/actions/deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/delete.py` & `meerschaum-2.2.0rc1/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/drop.py` & `meerschaum-2.2.0rc1/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/edit.py` & `meerschaum-2.2.0rc1/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/install.py` & `meerschaum-2.2.0rc1/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/login.py` & `meerschaum-2.2.0rc1/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/os.py` & `meerschaum-2.2.0rc1/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/pause.py` & `meerschaum-2.2.0rc1/meerschaum/actions/pause.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/python.py` & `meerschaum-2.2.0rc1/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/register.py` & `meerschaum-2.2.0rc1/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/setup.py` & `meerschaum-2.2.0rc1/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/sh.py` & `meerschaum-2.2.0rc1/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/show.py` & `meerschaum-2.2.0rc1/meerschaum/actions/show.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         'plugins'    : _show_plugins,
         'packages'   : _show_packages,
         'help'       : _show_help,
         'users'      : _show_users,
         'jobs'       : _show_jobs,
         'logs'       : _show_logs,
         'tags'       : _show_tags,
+        'schedules'  : _show_schedules,
     }
     return choose_subaction(action, show_options, **kw)
 
 
 def _complete_show(
         action: Optional[List[str]] = None,
         **kw: Any
@@ -573,14 +574,15 @@
     
     Usage:
         `show logs`
         `show logs --nopretty`
         `show logs myjob myotherjob`
     """
     import os, pathlib, random, asyncio
+    from datetime import datetime
     from meerschaum.utils.packages import attempt_import, import_rich
     from meerschaum.utils.daemon import get_filtered_daemons, Daemon
     from meerschaum.utils.warnings import warn, info
     from meerschaum.utils.formatting import get_console, ANSI, UNICODE
     from meerschaum.utils.misc import tail
     from meerschaum.config._paths import LOGS_RESOURCES_PATH
     from meerschaum.config import get_config
@@ -618,21 +620,30 @@
             d = Daemon(daemon_id=daemon_id)
             if d not in daemons:
                 daemons = get_filtered_daemons(action)
             _job_colors = _build_job_colors(daemons)
         return _job_colors[daemon_id]
 
     def _follow_pretty_print():
-        watchgod = attempt_import('watchgod')
+        watchfiles = attempt_import('watchfiles')
         rich = import_rich()
         rich_text = attempt_import('rich.text')
         _watch_daemon_ids = {d.daemon_id: d for d in daemons}
         info("Watching log files...")
 
         def _print_job_line(daemon, line):
+            date_prefix_str = line[:len('YYYY-MM-DD HH:mm')]
+            try:
+                line_timestamp = datetime.fromisoformat(date_prefix_str)
+            except Exception as e:
+                line_timestamp = None
+            if line_timestamp:
+                line = line[len('YYYY-MM-DD HH:mm | '):]
+            if len(line) == 0:
+                return
             text = rich_text.Text(daemon.daemon_id)
             text.append(
                 _get_buffer_spaces(daemon.daemon_id) + '| '
                 + (line[:-1] if line[-1] == '\n' else line)
             )
             if ANSI:
                 text.stylize(
@@ -672,16 +683,16 @@
             for d in daemons
         }
         for d in daemons:
             _seek_back_offset(d)
             _print_log_lines(d)
 
         _quit = False
-        async def _watch_logs():
-            async for changes in watchgod.awatch(LOGS_RESOURCES_PATH):
+        def _watch_logs():
+            for changes in watchfiles.watch(LOGS_RESOURCES_PATH):
                 if _quit:
                     return
                 for change in changes:
                     file_path_str = change[1]
                     if '.log' not in file_path_str or '.log.offset' in file_path_str:
                         continue
                     file_path = pathlib.Path(file_path_str)
@@ -695,18 +706,17 @@
                     except Exception as e:
                         daemon = None
                         warn(f"Seeing new logs for non-existent job '{daemon_id}'.", stack=False)
 
                     if daemon is not None:
                         _print_log_lines(daemon)
 
-        loop = asyncio.new_event_loop()
         try:
-            loop.run_until_complete(_watch_logs())
-        except KeyboardInterrupt:
+            _watch_logs()
+        except KeyboardInterrupt as ki:
             _quit = True
 
     def _print_nopretty_log_text():
         for d in daemons:
             log_text = d.log_text
             print(d.daemon_id)
             print(log_text)
@@ -813,13 +823,64 @@
             print(tag)
             for pipe in _pipes:
                 print(json.dumps(pipe.meta))
 
     return True, "Success"
 
 
+def _show_schedules(
+        action: Optional[List[str]] = None,
+        nopretty: bool = False,
+        **kwargs: Any
+    ) -> SuccessTuple:
+    """
+    Print the upcoming timestamps according to the given schedule.
+
+    Examples:
+        show schedule 'daily starting 00:00'
+        show schedule 'every 12 hours and mon-fri starting 2024-01-01'
+    """
+    from meerschaum.utils.schedule import parse_schedule
+    from meerschaum.utils.misc import is_int
+    from meerschaum.utils.formatting import print_options
+    if not action:
+        return False, "Provide a schedule to be parsed."
+    schedule = action[0]
+    default_num_timestamps = 5
+    num_timestamps_str = action[1] if len(action) >= 2 else str(default_num_timestamps)
+    num_timestamps = (
+        int(num_timestamps_str)
+        if is_int(num_timestamps_str)
+        else default_num_timestamps
+    )
+    try:
+        trigger = parse_schedule(schedule)
+    except ValueError as e:
+        return False, str(e)
+
+    next_datetimes = []
+    for _ in range(num_timestamps):
+        try:
+            next_dt = trigger.next()
+            next_datetimes.append(next_dt)
+        except Exception as e:
+            break
+
+    print_options(
+        next_datetimes,
+        num_cols = 1,
+        nopretty = nopretty,
+        header = (
+            f"Next {min(num_timestamps, len(next_datetimes))} timestamps "
+            + f"for schedule '{schedule}':"
+        ),
+    )
+
+    return True, "Success"
+        
+
 
 ### NOTE: This must be the final statement of the module.
 ###       Any subactions added below these lines will not
 ###       be added to the `help` docstring.
 from meerschaum.actions import choices_docstring as _choices_docstring
 show.__doc__ += _choices_docstring('show')
```

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/sql.py` & `meerschaum-2.2.0rc1/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/stack.py` & `meerschaum-2.2.0rc1/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/start.py` & `meerschaum-2.2.0rc1/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/stop.py` & `meerschaum-2.2.0rc1/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/sync.py` & `meerschaum-2.2.0rc1/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/tag.py` & `meerschaum-2.2.0rc1/meerschaum/actions/tag.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/uninstall.py` & `meerschaum-2.2.0rc1/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/upgrade.py` & `meerschaum-2.2.0rc1/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/actions/verify.py` & `meerschaum-2.2.0rc1/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/api/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/_chain.py` & `meerschaum-2.2.0rc1/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/_events.py` & `meerschaum-2.2.0rc1/meerschaum/api/_events.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/_oauth2.py` & `meerschaum-2.2.0rc1/meerschaum/api/_oauth2.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/_websockets.py` & `meerschaum-2.2.0rc1/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/actions.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/jobs.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/login.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/callbacks/register.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/components.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/components.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/connectors.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/graphs.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/jobs.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/keys.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/error.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/login.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/plugins.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/pages/register.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/pipes.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/plugins.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/users.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/websockets.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/dash/webterm.py` & `meerschaum-2.2.0rc1/meerschaum/api/dash/webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/dash.css` & `meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/static/css/xterm.css` & `meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/xterm.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-2.2.0rc1/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/static/js/terminado.js` & `meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/terminado.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/static/js/xterm.js` & `meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/xterm.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/templates/index.html` & `meerschaum-2.2.0rc1/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/templates/old_index.html` & `meerschaum-2.2.0rc1/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/resources/templates/termpage.html` & `meerschaum-2.2.0rc1/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_actions.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_connectors.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_index.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_login.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_misc.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_pipes.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_plugins.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_users.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_version.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/api/routes/_webterm.py` & `meerschaum-2.2.0rc1/meerschaum/api/routes/_webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_default.py` & `meerschaum-2.2.0rc1/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_edit.py` & `meerschaum-2.2.0rc1/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_environment.py` & `meerschaum-2.2.0rc1/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_formatting.py` & `meerschaum-2.2.0rc1/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_jobs.py` & `meerschaum-2.2.0rc1/meerschaum/config/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_patch.py` & `meerschaum-2.2.0rc1/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_paths.py` & `meerschaum-2.2.0rc1/meerschaum/config/_paths.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_preprocess.py` & `meerschaum-2.2.0rc1/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_read_config.py` & `meerschaum-2.2.0rc1/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_shell.py` & `meerschaum-2.2.0rc1/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/_sync.py` & `meerschaum-2.2.0rc1/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/stack/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/config/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/config/static/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/config/static/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/Connector.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/APIConnector.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/_actions.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/_fetch.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/_login.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/_misc.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/_pipes.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/_plugins.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/_request.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/_request.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/_uri.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/api/_users.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/parse.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/poll.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/SQLConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_cli.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_create_engine.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_fetch.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_instance.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_instance.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_pipes.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_plugins.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_sql.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_uri.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/_users.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/connectors/sql/tables/types.py` & `meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_attributes.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_clear.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_data.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_data.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_deduplicate.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_delete.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_drop.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_edit.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_fetch.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_register.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_show.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_sync.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/Pipe/_verify.py` & `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/core/User/_User.py` & `meerschaum-2.2.0rc1/meerschaum/core/User/_User.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/plugins/_Plugin.py` & `meerschaum-2.2.0rc1/meerschaum/plugins/_Plugin.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/plugins/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/_get_pipes.py` & `meerschaum-2.2.0rc1/meerschaum/utils/_get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/daemon/Daemon.py` & `meerschaum-2.2.0rc1/meerschaum/utils/daemon/Daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     Daemonize Python functions into background processes.
     """
 
     def __new__(
         cls,
         *args,
-        daemon_id : Optional[str] = None,
+        daemon_id: Optional[str] = None,
         **kw
     ):
         """
         If a daemon_id is provided and already exists, read from its pickle file.
         """
         instance = super(Daemon, cls).__new__(cls)
         if daemon_id is not None:
@@ -125,24 +125,28 @@
         NOTE: This WILL EXIT the parent process!
 
         Parameters
         ----------
         keep_daemon_output: bool, default True
             If `False`, delete the daemon's output directory upon exiting.
             
-        allow_dirty_run :
+        allow_dirty_run, bool, default False:
             If `True`, run the daemon, even if the `daemon_id` directory exists.
             This option is dangerous because if the same `daemon_id` runs twice,
             the last to finish will overwrite the output of the first.
 
         Returns
         -------
         Nothing — this will exit the parent process.
         """
-        import platform, sys, os
+        import platform, sys, os, traceback
+        from meerschaum.config._paths import LOGS_RESOURCES_PATH
+        from meerschaum.utils.warnings import warn
+        daemons_error_log_path = LOGS_RESOURCES_PATH / 'daemons_error.log'
+
         daemon = attempt_import('daemon')
 
         if platform.system() == 'Windows':
             return False, "Windows is no longer supported."
 
         self._setup(allow_dirty_run)
 
@@ -158,37 +162,45 @@
                 signal.SIGTERM: self._handle_sigterm,
             },
         )
 
         log_refresh_seconds = get_config('jobs', 'logs', 'refresh_files_seconds')
         self._log_refresh_timer = RepeatTimer(log_refresh_seconds, self.rotating_log.refresh_files)
 
-        with self._daemon_context:
-            try:
-                with open(self.pid_path, 'w+') as f:
-                    f.write(str(os.getpid()))
+        try:
+            with self._daemon_context:
+                try:
+                    with open(self.pid_path, 'w+', encoding='utf-8') as f:
+                        f.write(str(os.getpid()))
 
-                self._log_refresh_timer.start()
-                result = self.target(*self.target_args, **self.target_kw)
-                self.properties['result'] = result
-            except Exception as e:
-                warn(e, stacklevel=3)
-                result = e
-            finally:
-                self._log_refresh_timer.cancel()
-                self.rotating_log.close()
-                if self.pid is None and self.pid_path.exists():
-                    self.pid_path.unlink()
+                    self._log_refresh_timer.start()
+                    result = self.target(*self.target_args, **self.target_kw)
+                    self.properties['result'] = result
+                except Exception as e:
+                    warn(e, stacklevel=3)
+                    result = e
+                finally:
+                    self._log_refresh_timer.cancel()
+                    self.rotating_log.close()
+                    if self.pid is None and self.pid_path.exists():
+                        self.pid_path.unlink()
+
+                if keep_daemon_output:
+                    self._capture_process_timestamp('ended')
+                else:
+                    self.cleanup()
 
-            if keep_daemon_output:
-                self._capture_process_timestamp('ended')
-            else:
-                self.cleanup()
+                return result
+        except Exception as e:
+            daemon_error = traceback.format_exc()
+            with open(LOGS_RESOURCES_PATH, 'a+', encoding='utf-8') as f:
+                f.write(daemon_error)
 
-            return result
+        if daemon_error:
+            warn("Encountered an error while starting the daemon '{self}':\n{daemon_error}")
 
 
     def _capture_process_timestamp(
             self,
             process_key: str,
             write_properties: bool = True,
         ) -> None:
@@ -448,18 +460,18 @@
         if timer is not None:
             timer.cancel()
 
         daemon_context = self.__dict__.get('_daemon_context', None)
         if daemon_context is not None:
             daemon_context.close()
 
-        _close_pools()
+        self.rotating_log.stop_log_fd_interception()
 
-        ### NOTE: SystemExit() does not work here.
-        sys.exit(0)
+        _close_pools()
+        raise SystemExit(0)
 
 
     def _handle_sigterm(self, signal_number: int, stack_frame: 'frame') -> None:
         """
         Handle `SIGTERM` within the `Daemon` context.
         This method is injected into the `DaemonContext`.
         """
@@ -467,17 +479,18 @@
         if timer is not None:
             timer.cancel()
 
         daemon_context = self.__dict__.get('_daemon_context', None)
         if daemon_context is not None:
             daemon_context.close()
 
-        _close_pools()
+        self.rotating_log.stop_log_fd_interception()
 
-        raise SystemExit()
+        _close_pools()
+        raise SystemExit(1)
 
  
     def _send_signal(
             self,
             signal_to_send,
             timeout: Union[float, int, None] = None,
             check_timeout_interval: Union[float, int, None] = None,
@@ -646,27 +659,32 @@
 
     
     @property
     def rotating_log(self) -> RotatingFile:
         if '_rotating_log' in self.__dict__:
             return self._rotating_log
 
-        self._rotating_log = RotatingFile(self.log_path, redirect_streams=True)
+        self._rotating_log = RotatingFile(
+            self.log_path,
+            redirect_streams = True,
+            write_timestamps = True,
+        )
         return self._rotating_log
 
 
     @property
     def log_text(self) -> Optional[str]:
         """Read the log files and return their contents.
         Returns `None` if the log file does not exist.
         """
         new_rotating_log = RotatingFile(
             self.rotating_log.file_path,
             num_files_to_keep = self.rotating_log.num_files_to_keep,
             max_file_size = self.rotating_log.max_file_size,
+            write_timestamps = True,
         )
         return new_rotating_log.read()
 
 
     def readlines(self) -> List[str]:
         """
         Read the next log lines, persisting the cursor for later use.
@@ -710,15 +728,15 @@
     def pid(self) -> Union[int, None]:
         """Read the PID file and return its contents.
         Returns `None` if the PID file does not exist.
         """
         if not self.pid_path.exists():
             return None
         try:
-            with open(self.pid_path, 'r') as f:
+            with open(self.pid_path, 'r', encoding='utf-8') as f:
                 text = f.read()
             pid = int(text.rstrip())
         except Exception as e:
             warn(e)
             text = None
             pid = None
         return pid
@@ -811,15 +829,15 @@
         """Write the properties dictionary to the properties JSON file
         (only if self.properties exists).
         """
         success, msg = False, f"No properties to write for daemon '{self.daemon_id}'."
         if self.properties is not None:
             try:
                 self.path.mkdir(parents=True, exist_ok=True)
-                with open(self.properties_path, 'w+') as properties_file:
+                with open(self.properties_path, 'w+', encoding='utf-8') as properties_file:
                     json.dump(self.properties, properties_file)
                 success, msg = True, 'Success'
             except Exception as e:
                 success, msg = False, str(e)
         return success, msg
```

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/daemon/RotatingFile.py` & `meerschaum-2.2.0rc1/meerschaum/utils/daemon/RotatingFile.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 import os
 import io
 import re
 import pathlib
 import traceback
 import sys
 import atexit
+from datetime import datetime, timezone, timedelta
 from typing import List, Union, Optional, Tuple
 from meerschaum.config import get_config
 from meerschaum.utils.warnings import warn
+from meerschaum.utils.misc import round_time
+from meerschaum.utils.daemon.FileDescriptorInterceptor import FileDescriptorInterceptor
+from meerschaum.utils.threading import Thread
 import meerschaum as mrsm
 daemon = mrsm.attempt_import('daemon')
 
 class RotatingFile(io.IOBase):
     """
     A `RotatingFile` may be treated like a normal file-like object.
     Under the hood, however, it will create new sub-files and delete old ones.
@@ -29,14 +33,16 @@
 
     def __init__(
             self,
             file_path: pathlib.Path,
             num_files_to_keep: Optional[int] = None,
             max_file_size: Optional[int] = None,
             redirect_streams: bool = False,
+            write_timestamps: bool = False,
+            timestamps_format: str = '%Y-%m-%d %H:%M | ',
         ):
         """
         Create a file-like object which manages other files.
 
         Parameters
         ----------
         num_files_to_keep: int, default None
@@ -50,28 +56,33 @@
             Defaults to the configured value (100_000).
 
         redirect_streams: bool, default False
             If `True`, redirect previous file streams when opening a new file descriptor.
             
             NOTE: Only set this to `True` if you are entering into a daemon context.
             Doing so will redirect `sys.stdout` and `sys.stderr` into the log files.
+
+        write_timestamps: bool, default False
+            If `True`, prepend the current UTC timestamp to each line of the file.
         """
         self.file_path = pathlib.Path(file_path)
         if num_files_to_keep is None:
             num_files_to_keep = get_config('jobs', 'logs', 'num_files_to_keep')
         if max_file_size is None:
             max_file_size = get_config('jobs', 'logs', 'max_file_size')
         if num_files_to_keep < 2:
             raise ValueError("At least 2 files must be kept.")
         if max_file_size < 1:
             raise ValueError("Subfiles must contain at least one byte.")
 
         self.num_files_to_keep = num_files_to_keep
         self.max_file_size = max_file_size
         self.redirect_streams = redirect_streams
+        self.write_timestamps = write_timestamps
+        self.timestamps_format = timestamps_format
         self.subfile_regex_pattern = re.compile(
             r'^'
             + self.file_path.name
             + r'(?:\.\d+)?$'
         )
 
         ### When subfiles are opened, map from their index to the file objects.
@@ -83,22 +94,42 @@
         ### When reading, keep track of the file index and position.
         self._cursor: Tuple[int, int] = (0, 0)
 
         ### Don't forget to close any stray files.
         atexit.register(self.close)
 
 
+
     def fileno(self):
         """
         Return the file descriptor for the latest subfile.
         """
+        import inspect
+        stack = inspect.stack()
+        parent_level = stack[1]
+        parent_module = parent_level[0].f_globals.get('__file__')
+        #  if parent_module.endswith('daemon.py'):
+            #  self._monkey_patch_os_write()
         self.refresh_files()
         return self._current_file_obj.fileno()
 
 
+    def _monkey_patch_os_write(self):
+        import os
+        import sys
+        import pathlib
+        path = pathlib.Path('/home/bmeares/test1.log')
+        original_write = os.write
+        def intercept(*args, **kwargs):
+            with open(path, 'w', encoding='utf-8') as f:
+                f.write(str(args))
+            original_write(*args, **kwargs)
+        os.write = intercept
+
+
     def get_latest_subfile_path(self) -> pathlib.Path:
         """
         Return the path for the latest subfile to which to write into.
         """
         return self.get_subfile_path_from_index(
             self.get_latest_subfile_index()
         )
@@ -243,16 +274,18 @@
             self._current_file_obj is not None
             and
             self.get_index_from_subfile_name(self._current_file_obj.name) == -1
         )
         if is_first_run_with_logs or lost_latest_handle:
             self._current_file_obj = open(latest_subfile_path, 'a+', encoding='utf-8')
             if self.redirect_streams:
+                self.stop_log_fd_interception()
                 daemon.daemon.redirect_stream(sys.stdout, self._current_file_obj)
                 daemon.daemon.redirect_stream(sys.stderr, self._current_file_obj)
+                self.start_log_fd_interception()
 
         create_new_file = (
             (latest_subfile_index == -1)
             or
             self._current_file_obj is None
             or
             self.is_subfile_too_large(latest_subfile_index, potential_new_len)
@@ -265,24 +298,28 @@
             self._current_file_obj = open(new_file_path, 'a+', encoding='utf-8')
             self.subfile_objects[new_subfile_index] = self._current_file_obj
             self.flush()
 
             if self._previous_file_obj is not None:
                 if self.redirect_streams:
                     self._redirected_subfile_objects[old_subfile_index] = self._previous_file_obj
+                    self.stop_log_fd_interception()
                     daemon.daemon.redirect_stream(self._previous_file_obj, self._current_file_obj)
                     daemon.daemon.redirect_stream(sys.stdout, self._current_file_obj)
                     daemon.daemon.redirect_stream(sys.stderr, self._current_file_obj)
+                    self.start_log_fd_interception()
                 self.close(unused_only=True)
 
             ### Sanity check in case writing somehow fails.
             if self._previous_file_obj is self._current_file_obj:
                 self._previous_file_obj is None
 
             self.delete(unused_only=True)
+
+
         return self._current_file_obj
 
 
     def close(self, unused_only: bool = False) -> None:
         """
         Close any open file descriptors.
 
@@ -307,31 +344,44 @@
                 warn(f"Failed to close an open subfile:\n{traceback.format_exc()}")
 
         if not unused_only:
             self._previous_file_obj = None
             self._current_file_obj = None
 
 
+    def get_timestamp_prefix_str(self) -> str:
+        """
+        Return the current minute prefixm string.
+        """
+        return datetime.now(timezone.utc).strftime(self.timestamps_format)
+
+
     def write(self, data: str) -> None:
         """
         Write the given text into the latest subfile.
         If the subfile will be too large, create a new subfile.
         If too many subfiles exist at once, the oldest one will be deleted.
 
         NOTE: This will not split data across multiple files.
         As such, if data is larger than max_file_size, then the corresponding subfile
         may exceed this limit.
         """
         self.file_path.parent.mkdir(exist_ok=True, parents=True)
         if isinstance(data, bytes):
             data = data.decode('utf-8')
 
-        self.refresh_files(potential_new_len=len(data))
+        prefix_str = self.get_timestamp_prefix_str() if self.write_timestamps else ""
+        suffix_str = "\n" if self.write_timestamps else ""
+        self.refresh_files(potential_new_len=len(prefix_str + data + suffix_str))
         try:
+            if prefix_str:
+                self._current_file_obj.write(prefix_str)
             self._current_file_obj.write(data)
+            if suffix_str:
+                self._current_file_obj.write(suffix_str)
         except Exception as e:
             warn(f"Failed to write to subfile:\n{traceback.format_exc()}")
         self.flush()
         self.delete(unused_only=True)
 
 
     def delete(self, unused_only: bool = False) -> None:
@@ -467,15 +517,15 @@
                 subfile_index in self.subfile_objects
                 and
                 subfile_index not in self._redirected_subfile_objects
             ):
                 subfile_object = self.subfile_objects[subfile_index]
                 for i in range(self.SEEK_BACK_ATTEMPTS):
                     try:
-                        subfile_object.seek(max(seek_ix - i), 0)
+                        subfile_object.seek(max((seek_ix - i), 0))
                         subfile_lines = subfile_object.readlines()
                     except UnicodeDecodeError:
                         continue
                     break
             else:
                 with open(subfile_path, 'r', encoding='utf-8') as f:
                     for i in range(self.SEEK_BACK_ATTEMPTS):
@@ -534,14 +584,51 @@
                 except Exception as e:
                     warn(f"Failed to flush subfile:\n{traceback.format_exc()}")
         if self.redirect_streams:
             sys.stdout.flush()
             sys.stderr.flush()
 
 
+    def start_log_fd_interception(self):
+        """
+        Start the file descriptor monitoring threads.
+        """
+        self._stdout_interceptor = FileDescriptorInterceptor(
+            sys.stdout.fileno(),
+            self.get_timestamp_prefix_str,
+        )
+        self._stderr_interceptor = FileDescriptorInterceptor(
+            sys.stderr.fileno(),
+            self.get_timestamp_prefix_str,
+        )
+        self._stdout_interceptor_thread = Thread(target=self._stdout_interceptor.start_interception)
+        self._stderr_interceptor_thread = Thread(target=self._stderr_interceptor.start_interception)
+        self._stdout_interceptor_thread.start()
+        self._stderr_interceptor_thread.start()
+
+
+    def stop_log_fd_interception(self):
+        """
+        Stop the file descriptor monitoring threads.
+        """
+        stdout_interceptor = self.__dict__.get('_stdout_interceptor', None)
+        stderr_interceptor = self.__dict__.get('_stderr_interceptor', None)
+        stdout_interceptor_thread = self.__dict__.get('_stdout_interceptor_thread', None)
+        stderr_interceptor_thread = self.__dict__.get('_stderr_interceptor_thread', None)
+        if stdout_interceptor is None:
+            return
+        stdout_interceptor.stop_interception()
+        stderr_interceptor.stop_interception()
+        try:
+            stdout_interceptor_thread.join()
+            stderr_interceptor_thread.join()
+        except Exception:
+            pass
+
+
     def __repr__(self) -> str:
         """
         Return basic info for this `RotatingFile`.
         """
         return (
             "RotatingFile("
             + f"'{self.file_path.as_posix()}', "
```

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/daemon/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/utils/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/daemon/_names.py` & `meerschaum-2.2.0rc1/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/dataframe.py` & `meerschaum-2.2.0rc1/meerschaum/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/debug.py` & `meerschaum-2.2.0rc1/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/dtypes/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/utils/dtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/dtypes/sql.py` & `meerschaum-2.2.0rc1/meerschaum/utils/dtypes/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/formatting/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/formatting/_jobs.py` & `meerschaum-2.2.0rc1/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/formatting/_pipes.py` & `meerschaum-2.2.0rc1/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/formatting/_pprint.py` & `meerschaum-2.2.0rc1/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/formatting/_shell.py` & `meerschaum-2.2.0rc1/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/interactive.py` & `meerschaum-2.2.0rc1/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/misc.py` & `meerschaum-2.2.0rc1/meerschaum/utils/misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/networking.py` & `meerschaum-2.2.0rc1/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/packages/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/utils/packages/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     'import_versions': RLock(),
     '_checked_for_updates': RLock(),
     '_is_installed_first_check': RLock(),
     'emitted_pandas_warning': RLock(),
 }
 _checked_for_updates = set()
 _is_installed_first_check: Dict[str, bool] = {}
+_MRSM_PACKAGE_ARCHIVES_PREFIX: str = "https://meerschaum.io/files/archives/"
 
 def get_module_path(
         import_name: str,
         venv: Optional[str] = 'mrsm',
         debug: bool = False,
         _try_install_name_on_fail: bool = True,
     ) -> Union[pathlib.Path, None]:
@@ -636,17 +637,23 @@
             return (
                 packaging_version.parse(result.available_version) > 
                 packaging_version.parse(version)
             )
 
     ### We might be depending on a prerelease.
     ### Sanity check that the required version is not greater than the installed version. 
+    required_version = (
+        required_version.replace(_MRSM_PACKAGE_ARCHIVES_PREFIX, '')
+        .replace(' @ ', '').replace('wheels', '').replace('+mrsm', '').replace('/-', '')
+        .replace('-py3-none-any.whl', '')
+    )
+
     if 'a' in required_version:
-        required_version = required_version.replace('a', '-dev')
-        version = version.replace('a', '-dev')
+        required_version = required_version.replace('a', '-dev').replace('+mrsm', '')
+        version = version.replace('a', '-dev').replace('+mrsm', '')
     try:
         return (
             (not semver.Version.parse(version).match(required_version))
             if required_version else False
         )
     except AttributeError as e:
         pip_install(_import_to_install_name('semver'), venv='mrsm', debug=debug)
```

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/packages/_packages.py` & `meerschaum-2.2.0rc1/meerschaum/utils/packages/_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,18 @@
         'aiofiles'                   : 'aiofiles>=0.6.0',
         'packaging'                  : 'packaging>=21.3.0',
         'prompt_toolkit'             : 'prompt-toolkit>=3.0.39',
         'more_itertools'             : 'more-itertools>=8.7.0',
         'daemon'                     : 'python-daemon>=0.2.3',
         'fasteners'                  : 'fasteners>=0.18.0',
         'psutil'                     : 'psutil>=5.8.0',
-        'watchgod'                   : 'watchgod>=0.7.0',
+        'watchfiles'                 : 'watchfiles>=0.21.0',
         'dill'                       : 'dill>=0.3.3',
         'virtualenv'                 : 'virtualenv>=20.1.0',
-        'apscheduler'                : 'apscheduler>=4.0.0a4',
+        'apscheduler'                : 'APScheduler>=4.0.0a5',
     },
     'drivers': {
         'cryptography'               : 'cryptography>=38.0.1',
         'psycopg'                    : 'psycopg[binary]>=3.1.18',
         'pymysql'                    : 'PyMySQL>=0.9.0',
         'aiomysql'                   : 'aiomysql>=0.0.21',
         'sqlalchemy_cockroachdb'     : 'sqlalchemy-cockroachdb>=2.0.0',
@@ -85,14 +85,15 @@
         'twine'                      : 'twine>=3.2.0',
         'tuna'                       : 'tuna>=0.5.3',
         'snakeviz'                   : 'snakeviz>=2.1.0',
         'mypy'                       : 'mypy>=0.812.0',
         'pytest'                     : 'pytest>=6.2.2',
         'pytest_xdist'               : 'pytest-xdist>=3.2.1',
         'heartrate'                  : 'heartrate>=0.2.1',
+        'build'                      : 'build>=1.2.1',
     },
     'setup': {
     },
     'docs': {
         'mkdocs'                     : 'mkdocs>=1.1.2',
         'mkdocs_material'            : 'mkdocs-material>=6.2.5',
         'mkdocs_material_extensions' : 'mkdocs-material-extensions>=1.0.3',
@@ -145,15 +146,14 @@
     'gunicorn'                       : 'gunicorn>=20.1.0',
     'dotenv'                         : 'python-dotenv>=0.20.0',
     'websockets'                     : 'websockets>=11.0.3',
     'fastapi'                        : 'fastapi>=0.100.0',
     'passlib'                        : 'passlib>=1.7.4',
     'fastapi_login'                  : 'fastapi-login>=1.7.2',
     'multipart'                      : 'python-multipart>=0.0.5',
-    #  'pydantic'                       : 'pydantic>2.0.0',
     'httpx'                          : 'httpx>=0.24.1',
     'websockets'                     : 'websockets>=11.0.3',
 }
 packages['api'].update(packages['sql'])
 packages['api'].update(packages['formatting'])
 packages['api'].update(packages['dash'])
```

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-2.2.0rc1/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/pool.py` & `meerschaum-2.2.0rc1/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/process.py` & `meerschaum-2.2.0rc1/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/prompt.py` & `meerschaum-2.2.0rc1/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/schedule.py` & `meerschaum-2.2.0rc1/meerschaum/utils/schedule.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,32 @@
 
 from __future__ import annotations
 import sys
 from datetime import datetime, timezone, timedelta, timedelta
 import meerschaum as mrsm
 from meerschaum.utils.typing import Callable, Any, Optional, List, Dict
 
-INTERVAL_UNITS: List[str] = ['months', 'weeks', 'days', 'hours', 'minutes', 'seconds']
+STARTING_KEYWORD: str = 'starting'
+INTERVAL_UNITS: List[str] = ['months', 'weeks', 'days', 'hours', 'minutes', 'seconds', 'years']
 FREQUENCY_ALIASES: Dict[str, str] = {
     'daily': 'every 1 day',
     'hourly': 'every 1 hour',
     'minutely': 'every 1 minute',
     'weekly': 'every 1 week',
     'monthly': 'every 1 month',
     'secondly': 'every 1 second',
+    'yearly': 'every 1 year',
 }
 LOGIC_ALIASES: Dict[str, str] = {
     'and': '&',
     'or': '|',
     ' through ': '-',
     ' thru ': '-',
     ' - ': '-',
-    'beginning': 'starting',
+    'beginning': STARTING_KEYWORD,
 }
 CRON_DAYS_OF_WEEK: List[str] = ['mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun']
 CRON_DAYS_OF_WEEK_ALIASES: Dict[str, str] = {
     'monday': 'mon',
     'tuesday': 'tue',
     'tues': 'tue',
     'wednesday': 'wed',
@@ -61,16 +63,16 @@
 }
 SCHEDULE_ALIASES: Dict[str, str] = {
     **FREQUENCY_ALIASES,
     **LOGIC_ALIASES,
     **CRON_DAYS_OF_WEEK_ALIASES,
     **CRON_MONTHS_ALIASES,
 }
-STARTING_KEYWORD: str = 'starting'
 
+_scheduler = None
 def schedule_function(
         function: Callable[[Any], Any],
         schedule: str,
         *args,
         debug: bool = False,
         **kw
     ) -> None:
@@ -83,31 +85,43 @@
     function: Callable[[Any], Any]
         The function to execute.
 
     schedule: str
         The frequency schedule at which `function` should be executed (e.g. `'daily'`).
 
     """
-    import warnings
+    import asyncio
     from meerschaum.utils.warnings import warn
     from meerschaum.utils.misc import filter_keywords, round_time
+    global _scheduler
     kw['debug'] = debug
     kw = filter_keywords(function, **kw)
 
     apscheduler = mrsm.attempt_import('apscheduler', lazy=False)
     now = round_time(datetime.now(timezone.utc), timedelta(minutes=1))
     trigger = parse_schedule(schedule, now=now)
+    _scheduler = apscheduler.AsyncScheduler()
+    try:
+        loop = asyncio.get_running_loop()
+    except RuntimeError:
+        loop = asyncio.new_event_loop()
+
+    async def run_scheduler():
+        async with _scheduler:
+            job = await _scheduler.add_schedule(function, trigger, args=args, kwargs=kw)
+            try:
+                await _scheduler.run_until_stopped()
+            except (KeyboardInterrupt, SystemExit) as e:
+                await _stop_scheduler()
+                raise e
 
-    with apscheduler.Scheduler() as scheduler:
-        job = scheduler.add_schedule(function, trigger, args=args, kwargs=kw)
-        try:
-            scheduler.run_until_stopped()
-        except KeyboardInterrupt as e:
-            scheduler.stop()
-            scheduler.wait_until_stopped()
+    try:
+        loop.run_until_complete(run_scheduler())
+    except (KeyboardInterrupt, SystemExit) as e:
+        loop.run_until_complete(_stop_scheduler())
 
 
 def parse_schedule(schedule: str, now: Optional[datetime] = None):
     """
     Parse a schedule string (e.g. 'daily') into a Trigger object.
     """
     from meerschaum.utils.warnings import error
@@ -130,15 +144,15 @@
     starting_ts = parse_start_time(schedule, now=now)
     schedule = schedule.split(STARTING_KEYWORD)[0].strip()
     for alias_keyword, true_keyword in SCHEDULE_ALIASES.items():
         schedule = schedule.replace(alias_keyword, true_keyword)
 
     ### TODO Allow for combining `and` + `or` logic.
     if '&' in schedule and '|' in schedule:
-        error(f"Cannot accept both 'and' + 'or' logic in the schedule frequency.", ValueError)
+        raise ValueError(f"Cannot accept both 'and' + 'or' logic in the schedule frequency.")
 
     join_str = '|' if '|' in schedule else '&'
     join_trigger = (
         apscheduler_triggers_combining.OrTrigger
         if join_str == '|'
         else apscheduler_triggers_combining.AndTrigger
     )
@@ -148,91 +162,64 @@
     } if join_str == '&' else {}
 
     schedule_parts = [part.strip() for part in schedule.split(join_str)]
     triggers = []
 
     has_seconds = 'second' in schedule
     has_minutes = 'minute' in schedule
-    has_days = 'day' in schedule
-    has_weeks = 'week' in schedule
-    has_hours = 'hour' in schedule
-    num_hourly_intervals = schedule.count('hour')
-    divided_days = False
-    divided_hours = False
 
     for schedule_part in schedule_parts:
 
         ### Intervals must begin with 'every' (after alias substitution).
         if schedule_part.lower().startswith('every '):
             schedule_num_str, schedule_unit = (
                 schedule_part[len('every '):].split(' ', maxsplit=1)
             )
             schedule_unit = schedule_unit.rstrip('s') + 's'
             if schedule_unit not in INTERVAL_UNITS:
-                error(
+                raise ValueError(
                     f"Invalid interval '{schedule_unit}'.\n"
-                    + f"    Accepted values are {items_str(INTERVAL_UNITS)}.",
-                    ValueError,
+                    + f"    Accepted values are {items_str(INTERVAL_UNITS)}."
                 )
 
             schedule_num = (
                 int(schedule_num_str)
                 if is_int(schedule_num_str)
                 else float(schedule_num_str)
             )
 
-            ### NOTE: When combining days or weeks with other schedules,
-            ### we must divide one of the day-schedules by 2.
-            ### TODO Remove this when APScheduler is patched.
-            if (
-                join_str == '&'
-                and (has_days or has_weeks)
-                and len(schedule_parts) > 1
-                and not divided_days
-            ):
-                schedule_num /= 2
-                divided_days = True
-
-            ### NOTE: When combining multiple hourly intervals,
-            ### one must be divided by 2.
-            if (
-                join_str == '&'
-                #  and num_hourly_intervals > 1
-                and len(schedule_parts) > 1
-                and not divided_hours
-            ):
-                schedule_num /= 2
-                #  divided_hours = True
-
             trigger = (
                 apscheduler_triggers_interval.IntervalTrigger(
                     **{
                         schedule_unit: schedule_num,
                         'start_time': starting_ts,
                     }
                 )
-                if schedule_unit != 'months' else (
+                if schedule_unit not in ('months', 'years') else (
                     apscheduler_triggers_calendarinterval.CalendarIntervalTrigger(
                         **{
                             schedule_unit: schedule_num,
                             'start_date': starting_ts,
-                            #  'timezone': starting_ts.tzinfo, TODO Re-enable once APScheduler updates.
+                            'timezone': starting_ts.tzinfo,
                         }
                     )
                 )
             )
 
         ### Determine whether this is a pure cron string or a cron subset (e.g. 'may-aug')_.
         else:
-            first_three_prefix = schedule_part[:3] 
+            first_three_prefix = schedule_part[:3].lower()
+            first_four_prefix = schedule_part[:4].lower()
             cron_kw = {}
             if first_three_prefix in CRON_DAYS_OF_WEEK:
                 cron_kw['day_of_week'] = schedule_part
             elif first_three_prefix in CRON_MONTHS:
                 cron_kw['month'] = schedule_part
+            elif is_int(first_four_prefix) and len(first_four_prefix) == 4:
+                cron_kw['year'] = int(first_four_prefix)
             trigger = (
                 apscheduler_triggers_cron.CronTrigger(
                     **{
                         **cron_kw,
                         'hour': '*',
                         'minute': '*' if has_minutes else starting_ts.minute,
                         'second': '*' if has_seconds else starting_ts.second,
@@ -297,7 +284,14 @@
         warn(f"Unable to parse starting time from '{starting_str}'.", stack=False)
         schedule_parse_error = str(e)
     if schedule_parse_error:
         error(schedule_parse_error, ValueError, stack=False)
     if not starting_ts.tzinfo:
         starting_ts = starting_ts.replace(tzinfo=timezone.utc)
     return starting_ts
+
+
+async def _stop_scheduler():
+    if _scheduler is None:
+        return
+    await _scheduler.stop()
+    await _scheduler.wait_until_stopped()
```

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/sql.py` & `meerschaum-2.2.0rc1/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/threading.py` & `meerschaum-2.2.0rc1/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/typing.py` & `meerschaum-2.2.0rc1/meerschaum/utils/typing.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/venv/_Venv.py` & `meerschaum-2.2.0rc1/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/venv/__init__.py` & `meerschaum-2.2.0rc1/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/warnings.py` & `meerschaum-2.2.0rc1/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum/utils/yaml.py` & `meerschaum-2.2.0rc1/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/meerschaum.egg-info/PKG-INFO` & `meerschaum-2.2.0rc1/meerschaum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0.dev3
+Version: 2.2.0rc1
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -57,18 +57,18 @@
 Requires-Dist: aiofiles>=0.6.0; extra == "required"
 Requires-Dist: packaging>=21.3.0; extra == "required"
 Requires-Dist: prompt-toolkit>=3.0.39; extra == "required"
 Requires-Dist: more-itertools>=8.7.0; extra == "required"
 Requires-Dist: python-daemon>=0.2.3; extra == "required"
 Requires-Dist: fasteners>=0.18.0; extra == "required"
 Requires-Dist: psutil>=5.8.0; extra == "required"
-Requires-Dist: watchgod>=0.7.0; extra == "required"
+Requires-Dist: watchfiles>=0.21.0; extra == "required"
 Requires-Dist: dill>=0.3.3; extra == "required"
 Requires-Dist: virtualenv>=20.1.0; extra == "required"
-Requires-Dist: apscheduler>=4.0.0a4; extra == "required"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "required"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
 Requires-Dist: duckdb>=0.9.0; extra == "drivers"
@@ -91,14 +91,15 @@
 Requires-Dist: twine>=3.2.0; extra == "dev-tools"
 Requires-Dist: tuna>=0.5.3; extra == "dev-tools"
 Requires-Dist: snakeviz>=2.1.0; extra == "dev-tools"
 Requires-Dist: mypy>=0.812.0; extra == "dev-tools"
 Requires-Dist: pytest>=6.2.2; extra == "dev-tools"
 Requires-Dist: pytest-xdist>=3.2.1; extra == "dev-tools"
 Requires-Dist: heartrate>=0.2.1; extra == "dev-tools"
+Requires-Dist: build>=1.2.1; extra == "dev-tools"
 Provides-Extra: setup
 Provides-Extra: docs
 Requires-Dist: mkdocs>=1.1.2; extra == "docs"
 Requires-Dist: mkdocs-material>=6.2.5; extra == "docs"
 Requires-Dist: mkdocs-material-extensions>=1.0.3; extra == "docs"
 Requires-Dist: mkdocs-autolinks-plugin>=0.2.0; extra == "docs"
 Requires-Dist: mkdocs-awesome-pages-plugin>=2.5.0; extra == "docs"
@@ -148,18 +149,18 @@
 Requires-Dist: aiofiles>=0.6.0; extra == "sql"
 Requires-Dist: packaging>=21.3.0; extra == "sql"
 Requires-Dist: prompt-toolkit>=3.0.39; extra == "sql"
 Requires-Dist: more-itertools>=8.7.0; extra == "sql"
 Requires-Dist: python-daemon>=0.2.3; extra == "sql"
 Requires-Dist: fasteners>=0.18.0; extra == "sql"
 Requires-Dist: psutil>=5.8.0; extra == "sql"
-Requires-Dist: watchgod>=0.7.0; extra == "sql"
+Requires-Dist: watchfiles>=0.21.0; extra == "sql"
 Requires-Dist: dill>=0.3.3; extra == "sql"
 Requires-Dist: virtualenv>=20.1.0; extra == "sql"
-Requires-Dist: apscheduler>=4.0.0a4; extra == "sql"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "sql"
 Provides-Extra: dash
 Requires-Dist: Flask-Compress>=1.10.1; extra == "dash"
 Requires-Dist: dash>=2.6.2; extra == "dash"
 Requires-Dist: dash-bootstrap-components>=1.2.1; extra == "dash"
 Requires-Dist: dash-ace>=0.2.1; extra == "dash"
 Requires-Dist: dash-extensions>=1.0.4; extra == "dash"
 Requires-Dist: dash-daq>=0.5.0; extra == "dash"
@@ -206,18 +207,18 @@
 Requires-Dist: aiofiles>=0.6.0; extra == "api"
 Requires-Dist: packaging>=21.3.0; extra == "api"
 Requires-Dist: prompt-toolkit>=3.0.39; extra == "api"
 Requires-Dist: more-itertools>=8.7.0; extra == "api"
 Requires-Dist: python-daemon>=0.2.3; extra == "api"
 Requires-Dist: fasteners>=0.18.0; extra == "api"
 Requires-Dist: psutil>=5.8.0; extra == "api"
-Requires-Dist: watchgod>=0.7.0; extra == "api"
+Requires-Dist: watchfiles>=0.21.0; extra == "api"
 Requires-Dist: dill>=0.3.3; extra == "api"
 Requires-Dist: virtualenv>=20.1.0; extra == "api"
-Requires-Dist: apscheduler>=4.0.0a4; extra == "api"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "api"
 Requires-Dist: pprintpp>=0.4.0; extra == "api"
 Requires-Dist: asciitree>=0.3.3; extra == "api"
 Requires-Dist: typing-extensions>=4.7.1; extra == "api"
 Requires-Dist: pygments>=2.7.2; extra == "api"
 Requires-Dist: colorama>=0.4.3; extra == "api"
 Requires-Dist: rich>=13.4.2; extra == "api"
 Requires-Dist: more-termcolor>=1.1.3; extra == "api"
@@ -253,18 +254,18 @@
 Requires-Dist: aiofiles>=0.6.0; extra == "full"
 Requires-Dist: packaging>=21.3.0; extra == "full"
 Requires-Dist: prompt-toolkit>=3.0.39; extra == "full"
 Requires-Dist: more-itertools>=8.7.0; extra == "full"
 Requires-Dist: python-daemon>=0.2.3; extra == "full"
 Requires-Dist: fasteners>=0.18.0; extra == "full"
 Requires-Dist: psutil>=5.8.0; extra == "full"
-Requires-Dist: watchgod>=0.7.0; extra == "full"
+Requires-Dist: watchfiles>=0.21.0; extra == "full"
 Requires-Dist: dill>=0.3.3; extra == "full"
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
-Requires-Dist: apscheduler>=4.0.0a4; extra == "full"
+Requires-Dist: APScheduler>=4.0.0a5; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
 Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
 Requires-Dist: duckdb>=0.9.0; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
```

### Comparing `meerschaum-2.2.0.dev3/meerschaum.egg-info/SOURCES.txt` & `meerschaum-2.2.0rc1/meerschaum.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -218,14 +218,15 @@
 meerschaum/utils/schedule.py
 meerschaum/utils/sql.py
 meerschaum/utils/threading.py
 meerschaum/utils/typing.py
 meerschaum/utils/warnings.py
 meerschaum/utils/yaml.py
 meerschaum/utils/daemon/Daemon.py
+meerschaum/utils/daemon/FileDescriptorInterceptor.py
 meerschaum/utils/daemon/RotatingFile.py
 meerschaum/utils/daemon/__init__.py
 meerschaum/utils/daemon/_names.py
 meerschaum/utils/dtypes/__init__.py
 meerschaum/utils/dtypes/sql.py
 meerschaum/utils/formatting/__init__.py
 meerschaum/utils/formatting/_jobs.py
```

### Comparing `meerschaum-2.2.0.dev3/meerschaum.egg-info/requires.txt` & `meerschaum-2.2.0rc1/meerschaum.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 aiofiles>=0.6.0
 packaging>=21.3.0
 prompt-toolkit>=3.0.39
 more-itertools>=8.7.0
 python-daemon>=0.2.3
 fasteners>=0.18.0
 psutil>=5.8.0
-watchgod>=0.7.0
+watchfiles>=0.21.0
 dill>=0.3.3
 virtualenv>=20.1.0
-apscheduler>=4.0.0a4
+APScheduler>=4.0.0a5
 
 [api]
 uvicorn[standard]>=0.22.0
 gunicorn>=20.1.0
 python-dotenv>=0.20.0
 websockets>=11.0.3
 fastapi>=0.100.0
@@ -68,18 +68,18 @@
 aiofiles>=0.6.0
 packaging>=21.3.0
 prompt-toolkit>=3.0.39
 more-itertools>=8.7.0
 python-daemon>=0.2.3
 fasteners>=0.18.0
 psutil>=5.8.0
-watchgod>=0.7.0
+watchfiles>=0.21.0
 dill>=0.3.3
 virtualenv>=20.1.0
-apscheduler>=4.0.0a4
+APScheduler>=4.0.0a5
 pprintpp>=0.4.0
 asciitree>=0.3.3
 typing-extensions>=4.7.1
 pygments>=2.7.2
 colorama>=0.4.3
 rich>=13.4.2
 more-termcolor>=1.1.3
@@ -118,14 +118,15 @@
 twine>=3.2.0
 tuna>=0.5.3
 snakeviz>=2.1.0
 mypy>=0.812.0
 pytest>=6.2.2
 pytest-xdist>=3.2.1
 heartrate>=0.2.1
+build>=1.2.1
 
 [docs]
 mkdocs>=1.1.2
 mkdocs-material>=6.2.5
 mkdocs-material-extensions>=1.0.3
 mkdocs-autolinks-plugin>=0.2.0
 mkdocs-awesome-pages-plugin>=2.5.0
@@ -183,18 +184,18 @@
 aiofiles>=0.6.0
 packaging>=21.3.0
 prompt-toolkit>=3.0.39
 more-itertools>=8.7.0
 python-daemon>=0.2.3
 fasteners>=0.18.0
 psutil>=5.8.0
-watchgod>=0.7.0
+watchfiles>=0.21.0
 dill>=0.3.3
 virtualenv>=20.1.0
-apscheduler>=4.0.0a4
+APScheduler>=4.0.0a5
 cryptography>=38.0.1
 psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
 duckdb>=0.9.0
 duckdb-engine>=0.9.2
@@ -272,14 +273,14 @@
 aiofiles>=0.6.0
 packaging>=21.3.0
 prompt-toolkit>=3.0.39
 more-itertools>=8.7.0
 python-daemon>=0.2.3
 fasteners>=0.18.0
 psutil>=5.8.0
-watchgod>=0.7.0
+watchfiles>=0.21.0
 dill>=0.3.3
 virtualenv>=20.1.0
-apscheduler>=4.0.0a4
+APScheduler>=4.0.0a5
 
 [stack]
 docker-compose>=1.29.2
```

### Comparing `meerschaum-2.2.0.dev3/setup.py` & `meerschaum-2.2.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 # vim:fenc=utf-8
 
 import setuptools, sys, platform
 from setuptools import setup
 from setuptools.command.install import install
 cx_Freeze, Executable = None, None
 
-### read values from within the package
-exec(open('meerschaum/config/_version.py').read())
-exec(open('meerschaum/utils/packages/_packages.py').read())
-exec(open('meerschaum/config/static/__init__.py').read())
-setup_cf = _static_config()['setup']
+with open('meerschaum/config/_version.py', encoding='utf-8') as version_file:
+    exec(version_file.read())
+with open('meerschaum/utils/packages/_packages.py', encoding='utf-8') as packages_file:
+    exec(packages_file.read())
+with open('meerschaum/config/static/__init__.py', encoding='utf-8') as static_file:
+    exec(static_file.read())
+with open('README.md', 'r', encoding='utf-8') as readme_file:
+    readme = readme_file.read()
+
+setup_cf = STATIC_CONFIG['setup']
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
         from meerschaum.actions import actions
         try:
@@ -24,17 +29,14 @@
             pass
 
 extras = {}
 ### NOTE: package dependencies are defined in meerschaum.utils.packages._packages
 for group in packages:
     extras[group] = [ install_name for import_name, install_name in packages[group].items() ]
 
-with open('README.md', 'r', encoding='utf-8') as f:
-    readme = f.read()
-
 setup_kw_args = {
     'name'                          : setup_cf['name'],
     'version'                       : __version__,
     'description'                   : setup_cf['description'],
     'long_description'              : readme,
     'long_description_content_type' : 'text/markdown',
     'url'                           : setup_cf['url'],
```

### Comparing `meerschaum-2.2.0.dev3/tests/test_deduplicate.py` & `meerschaum-2.2.0rc1/tests/test_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/tests/test_pipes_dtypes.py` & `meerschaum-2.2.0rc1/tests/test_pipes_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/tests/test_sql.py` & `meerschaum-2.2.0rc1/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/tests/test_sync.py` & `meerschaum-2.2.0rc1/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/tests/test_users.py` & `meerschaum-2.2.0rc1/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0.dev3/tests/test_verify.py` & `meerschaum-2.2.0rc1/tests/test_verify.py`

 * *Files identical despite different names*

