# Comparing `tmp/TDSR-UWB-1.538.tar.gz` & `tmp/TDSR-UWB-1.539.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDSR-UWB-1.538.tar", last modified: Mon May 13 22:01:15 2024, max compression
+gzip compressed data, was "TDSR-UWB-1.539.tar", last modified: Thu May 16 03:42:37 2024, max compression
```

## Comparing `TDSR-UWB-1.538.tar` & `TDSR-UWB-1.539.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 22:01:15.244475 TDSR-UWB-1.538/
--rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.538/LICENSE.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.538/MANIFEST.in
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-13 22:01:15.244475 TDSR-UWB-1.538/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.538/README.md
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 22:01:15.240476 TDSR-UWB-1.538/TDSR-UWB/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 22:01:15.240476 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 22:01:15.244475 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/
--rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
--rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 22:01:15.244475 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
--rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
--rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/API.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 22:01:15.244475 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
--rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
--rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
--rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
--rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
--rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
--rw-rw-r--   0 senter    (1000) senter    (1000)   253686 2024-05-13 21:23:29.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     6230 2024-05-13 20:28:35.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_logging.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    14427 2024-05-13 20:49:15.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    19239 2024-05-13 21:53:26.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    83488 2024-05-13 21:05:08.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     3982 2024-05-13 20:29:15.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_settings.py
--rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/__init__.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/crc16.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2121 2024-04-15 16:20:28.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/logReader.py
--rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/logReader_Minimal.py
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-13 22:01:15.244475 TDSR-UWB-1.538/TDSR-UWB/TDSR_UWB.egg-info/
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-13 22:01:15.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-13 22:01:15.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-13 22:01:15.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-05-13 22:01:15.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-13 22:01:15.000000 TDSR-UWB-1.538/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-13 22:01:15.244475 TDSR-UWB-1.538/setup.cfg
--rw-rw-r--   0 senter    (1000) senter    (1000)     7693 2024-05-13 21:56:39.000000 TDSR-UWB-1.538/setup.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/
+-rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.539/LICENSE.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.539/MANIFEST.in
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.539/README.md
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.201335 TDSR-UWB-1.539/TDSR-UWB/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.201335 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
+-rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/API.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
+-rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)   253692 2024-05-16 02:50:22.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6303 2024-05-16 03:29:42.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_logging.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    14427 2024-05-16 01:41:06.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    19213 2024-05-16 03:23:03.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    83453 2024-05-16 01:43:15.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     3982 2024-05-16 01:40:01.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_settings.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/__init__.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/crc16.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     2280 2024-05-16 03:20:39.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/logReader.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/logReader_Minimal.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/setup.cfg
+-rw-rw-r--   0 senter    (1000) senter    (1000)     7693 2024-05-16 03:35:34.000000 TDSR-UWB-1.539/setup.py
```

### Comparing `TDSR-UWB-1.538/PKG-INFO` & `TDSR-UWB-1.539/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.538
+Version: 1.539
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/API.md` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/API.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/networking.md` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from TDSR_Support import TDSR_logging
 from TDSR_Support import TDSR_settings
 from TDSR_Support import TDSR_radioControl
 from TDSR_Support import TDSR_radioConnection
 
 # Primary window GUI class. All sub windows are launched from here as well.
-__version__ = "1.538"
+__version__ = "1.539"
 # Primary application window and GUI
 class MainWindow(QMainWindow):
     def __init__(self, app, *args, **kwargs):
         super(MainWindow, self).__init__(*args, **kwargs)
         title = "PennyWhistle Ranging GUI V" + __version__
         self.setWindowTitle(title)
         self.myScreen = app.primaryScreen()                      # self is mainwindow Widget and myScreen is the display it lives on
@@ -177,16 +177,16 @@
                 self.windowDataTransfer.radioData.reqMsgTimer.stop()
                 self.chipTempTimer.stop()
                 self.dispChipTemp.setText("-")
             else:
                 self.windowDataTransfer.radioData.reqMsgTimer.start()
                 self.radioConfigReq, addr = self.radioReq.API.radio_GetConfig_Request(self.appSettings['reqRadio'], self.configID)
                 self.radioStateReq, addr = self.radioReq.API.radio_GetState_Request(self.appSettings['reqRadio'])
-                self.radioReqNodeID, addr = self.radioReq.API.radio_GetNodeID_Request(self.appSettings['reqRadio'])
-                self.radioReqNodeID = self.radioReqNodeID['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
+                self.radioReqNodeIDMsg, addr = self.radioReq.API.radio_GetNodeID_Request(self.appSettings['reqRadio'])
+                self.radioReqNodeID = self.radioReqNodeIDMsg['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
                 self.chipTempTimer.start()
                 self.connectedRequester = 1
             self.updateConnectReq(self.radioReq.status)
 
 # Connects to responding radio. Needed to get stats and set configuration but not needed to range.
     def radioConnectResp(self):
         if self.check_connectResp.isChecked():
```

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_logging.py` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_logging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from datetime import datetime, date
 from time import time
 from pathlib import Path
 from os import path, mkdir, makedirs
 from json import dumps
 
-__version__ = "1.538"
+__version__ = "1.539"
 
 # All application data logging functions
 class logData():
     def __init__(self, gui):
         self.gui = gui
         self.settings = gui.appSettings
         self.logFile = ""
-        self.needComma = False
 # Creates a new filename and directory under the chosen log directory.
 #  Naming is cased on radio nodes and times logs were taken. Autogenerated filenames.
     def createTimeBasedLog(self, nodeIPs):
         if self.gui.connectedRequester == 1:
             print("Time Based Log")
             today = date.today()
             nodeStr = nodeIPs[0]
@@ -25,21 +24,21 @@
             dataDirectoryName = path.join(self.settings['logDirectory'],dateDirectory)
             if not path.isdir(dataDirectoryName):
                 makedirs(dataDirectoryName)
             timeNow = datetime.now()
             self.fileDateTime = timeNow.strftime("RNS_Log_%m_%d_%y_%H_%M_%S.json")
             logFileName = path.join(dataDirectoryName,self.fileDateTime)
             self.logFile = open(logFileName,"w")
-            if self.settings['logJson'] == 1:
-                self.logFile.write("[")
-            self.needComma = False
+            # if self.settings['logJson'] == 1:
             self.logFile.write(dumps(self.gui.radioStateReq))
-            self.logFile.write(",\n")
+            self.logFile.write("\n")
             self.logFile.write(dumps(self.gui.radioConfigReq))
-            self.logFile.write(",\n")
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqNodeIDMsg))
+            self.logFile.write("\n\n")
             print(logFileName)
 # Creates a new filename and directory under the chosen log directory. Subdirectory is created for Month/Year
 #  log was taken. Name is based on user entered base name with 4 digit increasing file counter at the end.
     def createNameBasedLog(self):
         if self.gui.connectedRequester == 1:
             logFileName = self.settings['logFile']
             logFilePath = self.settings['logDirectory']
@@ -66,70 +65,71 @@
                     stmp = "0000" + str(tmpNum)
                     stmp = "_" + stmp[len(stmp)-4:]
                     logFileTmp = logFileFullPath + tmp[0] + stmp
                     logFileName = Path(logFileTmp + "." + tmp[1])
                     tmpNum = tmpNum + 1
             self.logFile = logFileName
             self.logFile = open(self.logFile,"w")
-            self.logFile.write("[")
-            self.needComma = False
+            # if self.settings['logJson'] == 1:
             self.logFile.write(dumps(self.gui.radioStateReq))
-            self.logFile.write(",\n")
+            self.logFile.write("\n")
             self.logFile.write(dumps(self.gui.radioConfigReq))
-            self.logFile.write(",\n")
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqNodeIDMsg))
+            self.logFile.write("\n\n")
             print(logFileName)
 # Log data to chosen log file. Can save all messages, only range_info messages, or simply ranges and message IDs
     def logToFile(self, packet, nodeIPs):
+        # Start new log if logfile is closed
         if self.logFile == "":
             if self.settings['logRangeInfoOnly'] == 1 and "RANGE_INFO" in packet:
                 if self.settings['logDateBased'] == 0:
                     self.createNameBasedLog()
                 else:
                     self.createTimeBasedLog(nodeIPs)
             if self.settings['logRangeInfoOnly'] == 0:
                 if self.settings['logDateBased'] == 0:
                     self.createNameBasedLog()
                 else:
                     self.createTimeBasedLog(nodeIPs)
+        # check on segmented flag and start new at the right time
         if self.settings['logSegmented'] == 1:
             if (int((time() - self.startDataTime)) > int(self.settings['segmentTime'])):
                 if (self.logFile != ""):
-                    self.logFile.write("]")
                     self.closeLogFile()
                     self.startDataTime = time()
                     if self.settings['logDateBased'] == 1:
                         self.createTimeBasedLog(nodeIPs)
                     else:
                         self.createNameBasedLog()
+        # do the logging
         if packet != None:
-            if self.settings['logJson'] == 1:
-                if self.settings['logRangeInfoOnly'] == 1:
-                    if "RANGE_INFO" in packet:
-                        if self.needComma:
-                            self.logFile.write(",\n")
-                            self.needComma = False
-                        self.logFile.write(dumps(packet))
-                        self.needComma = True
-                else:
-                    if self.needComma:
-                        self.logFile.write(",\n")
-                        self.needComma = False
+            # if Json
+            # if self.settings['logJson'] == 1:
+            # if range info only
+            if self.settings['logRangeInfoOnly'] == 1:
+                if "RANGE_INFO" in packet.keys():
                     self.logFile.write(dumps(packet))
-                    self.needComma = True
+                    self.logFile.write("\n")
             else:
-                if "RANGE_INFO" in packet:
-                    if self.needComma:
-                        self.logFile.write(",\n")
-                        self.needComma = False
-                    tmp = dict()
-                    tmp['RANGE_ONLY'] = dict()
-                    tmp['RANGE_ONLY']['msgId'] = packet['RANGE_INFO']['msgId']
-                    tmp['RANGE_ONLY']['precisionRangeM'] = packet['RANGE_INFO']['precisionRangeM']
-                    self.logFile.write(dumps(tmp))
-                    self.needComma = True
+                self.logFile.write(dumps(packet))
+                self.logFile.write("\n")
+            # if csv
+            # else:
+                # if "RANGE_INFO" in packet.keys():
+                #         msg = packet['RANGE_INFO']
+                #         text = ""
+                #         for field in msg.keys():
+                #             text = text + str(msg[field]) + ","
+                #         text = text[:len(text)-1] + "\n"
+                #         self.logFile.write(text)
+                #     tmp = dict()
+                #     tmp['RANGE_ONLY'] = dict()
+                #     tmp['RANGE_ONLY']['msgId'] = packet['RANGE_INFO']['msgId']
+                #     tmp['RANGE_ONLY']['precisionRangeM'] = packet['RANGE_INFO']['precisionRangeM']
+                #     self.logFile.write(dumps(tmp))
 # Closes logfile if open
     def closeLogFile(self):
         if self.logFile != "":
-            self.logFile.write("]")
             self.logFile.close()
             self.logFile = ""
             print("Closed Log")
```

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from json import dumps
 from time import sleep
 
-__version__ = "1.538"
+__version__ = "1.539"
 
 class RadioAPI:
     _msgId = 0
 
     def __init__(self, messageQueues, messageList, TxQueue):
         self.TxQueue = TxQueue
         self.messageList = messageList
```

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 import serial
 import serial.tools.list_ports
 import ipaddress
 import netifaces
 
 from TDSR_Support import TDSR_radioAPI
 
-__version__ = "1.538"
-
-if os.name == "nt":
-    import winreg as compat_winreg
+__version__ = "1.539"
 
 # Use netifaces to find local IP addresses.
 netifaces_available = False
 try:
     import netifaces
     netifaces_available = True
 
@@ -118,15 +115,15 @@
                                     ...
                                     # print("Dumping Request")
                     else:
                         print("RX Thread: MessageType not in API keys")
                         print(f"   Type: {msgType}")
                         print(f"   Keys: {self.API.messageList.keys()}")
                         print(f"   Type: {packet}")
-                    if self.gui.appSettings['enableLogging'] == 1:
+                    if self.gui.appSettings['enableLogging'] == 1 and self.gui.radioMode != "idle":
                         self.gui.logFile.logToFile(packet, self.gui.appSettings['reqRadio'])
             except:
                 pass
 
     def findUsbRadios(self):
         radios = []
         ports = [port for port in serial.tools.list_ports.comports() if port != "n/a" and port.vid == 0x1027 and port.pid == 0x1234]
```

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_radioControl.py` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from time import time, sleep
 from math import sqrt, log10
 from numpy import power
 from pathlib import Path
 from base64 import b64encode, b64decode
 from threading import Thread
 
-__version__ = "1.538"
+__version__ = "1.539"
 
 # Primary ranging functions
 class rangeCmds():
     def __init__(self, gui):
         self.gui = gui
         self.appSetup()
 
@@ -118,15 +118,14 @@
                     if mode != 'networking':
                         print("Unabled to connect to responder. Make sure it is in active mode.")
                         text =  "Unabled to connect to responder. Make sure it is in active mode.\n"
                         self.gui.updateConsole(text)
         if self.gui.connectedRequester == 1:
             status, packet, addr = self.gui.radioReq.API.radio_GetInfo_Request(self.gui.appSettings['reqRadio'])
             self.gui.radioStateReq, addr = self.gui.radioReq.API.radio_GetState_Request(self.gui.appSettings['reqRadio'])
-            self.needComma = False
             status = True
         else:   # If couldn't connect, then shutdown run and reset
             status = False
             if mode != 'networking':
                 self.running = 1
                 print("Ranging setup error, can't reach requester, aborting run.")
                 self.rangeTimer.stop()
@@ -401,15 +400,15 @@
             self.rangeFilteredArray = self.rangeFilteredArray[1:]
             self.chartPointsX = self.chartPointsX[1:]
         if len(self.rangeArrayAll) > int(self.gui.appSettings['memoryDepth']):
             self.rxPowerArrayAll = self.rxPowerArrayAll[1:]
             self.maxNoiseArrayAll = self.maxNoiseArrayAll[1:]
             self.stdNoiseArrayAll = self.stdNoiseArrayAll[1:]
             self.rangeArrayAll = self.rangeArrayAll[1:]
-            self.rangeArrayFilteredAll = self.rangeArrayFilteredAll[1:]
+            self.rangeFilteredArrayAll = self.rangeFilteredArrayAll[1:]
             self.chartPointsXAll = self.chartPointsXAll[1:]
     # Update GUI
         # self.gui.guiPacketUpdates(packet)
         self.packetDisplay = packet
 
 # computes various stats abot the radio run upon completion. Prints output to GUI Console.
     def computeRunStats(self):
```

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/TDSR_settings.py` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from json import dumps, loads
 
-__version__ = "1.538"
+__version__ = "1.539"
 
 # loads and saves GUI settings. Also sets default values if settings file does not include all keys.
 class appSettings():
     def __init__(self):
         self.settings = {}
 
     def settingsSetup(self):
```

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/crc16.py` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/crc16.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_Support/logReader.py` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/logReader.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,20 @@
     def __init__(self, *args, **kwargs):
         super(MainWindow, self).__init__(*args, **kwargs)
         self.filename = QFileDialog.getOpenFileName(self, 'Open Requester File', './logfiles', 'Logs (*.log *.json)')
         print("FileName:", self.filename[0])
         self.graphSizeX = 600
         self.graphSizeY = 600
         logfile = open(self.filename[0],"r")
-        data = json.loads(logfile.read())
+        dataLines = logfile.readlines()
+        dataLines = dataLines[4:]
+        data = []
+        for dataLine in dataLines:
+            print(dataLine)
+            data.append(json.loads(dataLine))
         logfile.close()
         self.setGeometry(10,10,self.graphSizeX,self.graphSizeY)
         self.initGUI()
         self.show()
         self.processData(data)
 
     def processData(self, data):
```

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.538
+Version: 1.539
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.538/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt` & `TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.538/setup.py` & `TDSR-UWB-1.539/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="TDSR-UWB",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.538",  # Required
+    version="1.539",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Support libraries for TDSR LLC UWB Radios",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

