# Comparing `tmp/alttester_driver-2.1.0.tar.gz` & `tmp/alttester_driver-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alttester_driver-2.1.0.tar", last modified: Mon Apr 15 10:33:03 2024, max compression
+gzip compressed data, was "alttester_driver-2.1.1.tar", last modified: Thu May 16 09:09:50 2024, max compression
```

## Comparing `alttester_driver-2.1.0.tar` & `alttester_driver-2.1.1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.206964 alttester_driver-2.1.0/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.204364 alttester_driver-2.1.0/AltTester_Driver.egg-info/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3560 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/PKG-INFO
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4559 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/SOURCES.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/dependency_links.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/not-zip-safe
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       51 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/requires.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       16 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/top_level.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       56 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/MANIFEST.in
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3560 2024-04-15 10:33:03.205752 alttester_driver-2.1.0/PKG-INFO
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1601 2024-03-31 06:05:52.000000 alttester_driver-2.1.0/README.md
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:02.972165 alttester_driver-2.1.0/alttester/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1040 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      718 2024-03-25 09:42:14.000000 alttester_driver-2.1.0/alttester/__version__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    12267 2024-04-10 07:45:53.000000 alttester_driver-2.1.0/alttester/_websocket.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    37704 2024-04-01 07:09:49.000000 alttester_driver-2.1.0/alttester/altdriver.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    12119 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/altobject.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      977 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/by.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:02.980078 alttester_driver-2.1.0/alttester/commands/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.013066 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      990 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2538 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/add_notification_listener.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1824 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/remove_notification_listener.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      992 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/reset_input.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1908 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/set_server_logging.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.044821 alttester_driver-2.1.0/alttester/commands/FindObjects/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1321 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2042 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_object.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1247 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_object_at_coordinates.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2063 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_object_which_contains.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2043 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_objects.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2064 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_objects_which_contains.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2461 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_component_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2496 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2598 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2654 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object_which_contains.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.059878 alttester_driver-2.1.0/alttester/commands/InputActions/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1447 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1225 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/begin_touch.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1614 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/click_coordinates.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1219 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/end_touch.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1951 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/keys_down.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1882 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/keys_up.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1534 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/move_mouse.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1347 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/move_touch.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1515 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/multi_point_swipe.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2239 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/press_keys.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1623 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/scroll_mouse.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1574 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/swipe.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1610 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/tap_coordinates.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1532 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/tilt.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.105713 alttester_driver-2.1.0/alttester/commands/Notifications/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1149 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1579 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/base_notification_callbacks.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      894 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/load_scene_mode.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      869 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/load_scene_notification_result.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      878 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/log_notification_result.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      838 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/notification_type.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.117539 alttester_driver-2.1.0/alttester/commands/ObjectCommands/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1448 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2587 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/call_method.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1499 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/click_element.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1209 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_all_components.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1605 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_component_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1175 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_text.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1209 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_down.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1209 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_enter.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1189 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_exit.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1189 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_up.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1610 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/set_component_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1321 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/set_text.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1495 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/tap_element.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.134176 alttester_driver-2.1.0/alttester/commands/UnityCommands/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1578 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      940 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/delete_player_pref.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1179 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/delete_player_pref_key.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      944 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/get_all_loaded_scenes.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      974 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/get_current_scene.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1668 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/get_player_pref_key.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1075 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/get_time_scale.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1409 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/load_scene.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2037 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/set_player_pref_key.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1410 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/set_time_scale.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1337 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/unload_scene.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1710 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1256 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     7982 2024-04-01 07:09:49.000000 alttester_driver-2.1.0/alttester/commands/base_command.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1187 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/get_png_screenshot.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      940 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/get_server_version.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1574 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/get_static_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1554 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/set_static_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     5039 2024-04-10 07:45:53.000000 alttester_driver-2.1.0/alttester/exceptions.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     8202 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/keycode.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1033 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/logging.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      960 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/playerpref.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1680 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/reverse_port_forwarding.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      300 2024-04-15 07:14:09.000000 alttester_driver-2.1.0/requirements-dev.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       50 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/requirements.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       38 2024-04-15 10:33:03.207659 alttester_driver-2.1.0/setup.cfg
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3351 2024-01-09 14:51:06.000000 alttester_driver-2.1.0/setup.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:02.947278 alttester_driver-2.1.0/tests/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.198107 alttester_driver-2.1.0/tests/integration/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      699 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/integration/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     7353 2024-04-15 07:14:09.000000 alttester_driver-2.1.0/tests/integration/conftest.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     5110 2024-04-01 07:09:49.000000 alttester_driver-2.1.0/tests/integration/test_driver.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4366 2024-01-09 14:51:06.000000 alttester_driver-2.1.0/tests/integration/test_notifications.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1512 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/integration/test_reverse_port_forwarding.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    21323 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene01_part1.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    18718 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene01_part2.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     5202 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene02.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     6527 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene03.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     5191 2024-04-10 07:45:53.000000 alttester_driver-2.1.0/tests/integration/test_scene05.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4478 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene07.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2306 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene09.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4259 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene10.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1114 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/integration/utils.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.202908 alttester_driver-2.1.0/tests/unit/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      699 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/unit/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2368 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/unit/test_altobject.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2229 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/unit/test_commands.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     6103 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/unit/test_websocket.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.334379 alttester_driver-2.1.1/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.332059 alttester_driver-2.1.1/AltTester_Driver.egg-info/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3560 2024-05-16 09:09:50.000000 alttester_driver-2.1.1/AltTester_Driver.egg-info/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4559 2024-05-16 09:09:50.000000 alttester_driver-2.1.1/AltTester_Driver.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-05-16 09:09:50.000000 alttester_driver-2.1.1/AltTester_Driver.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-05-16 09:09:50.000000 alttester_driver-2.1.1/AltTester_Driver.egg-info/not-zip-safe
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       51 2024-05-16 09:09:50.000000 alttester_driver-2.1.1/AltTester_Driver.egg-info/requires.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       16 2024-05-16 09:09:50.000000 alttester_driver-2.1.1/AltTester_Driver.egg-info/top_level.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       56 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/MANIFEST.in
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3560 2024-05-16 09:09:50.333258 alttester_driver-2.1.1/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1601 2024-03-31 06:05:52.000000 alttester_driver-2.1.1/README.md
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.257825 alttester_driver-2.1.1/alttester/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1040 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      718 2024-05-14 05:13:02.000000 alttester_driver-2.1.1/alttester/__version__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    12271 2024-05-16 07:56:12.000000 alttester_driver-2.1.1/alttester/_websocket.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    37707 2024-05-16 07:56:12.000000 alttester_driver-2.1.1/alttester/altdriver.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    12119 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/altobject.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      977 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/by.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.263108 alttester_driver-2.1.1/alttester/commands/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.267644 alttester_driver-2.1.1/alttester/commands/AltTesterCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      990 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/AltTesterCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2538 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/AltTesterCommands/add_notification_listener.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1824 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/AltTesterCommands/remove_notification_listener.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      992 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/AltTesterCommands/reset_input.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1908 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/AltTesterCommands/set_server_logging.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.276190 alttester_driver-2.1.1/alttester/commands/FindObjects/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1321 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2042 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/find_object.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1247 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/find_object_at_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2063 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/find_object_which_contains.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2043 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/find_objects.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2064 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/find_objects_which_contains.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2461 2024-03-25 08:05:11.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/wait_for_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2496 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/wait_for_object.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2598 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2654 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/FindObjects/wait_for_object_which_contains.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.291248 alttester_driver-2.1.1/alttester/commands/InputActions/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1447 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1225 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/begin_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1614 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/click_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1219 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/end_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1951 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/keys_down.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1882 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/keys_up.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1534 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/move_mouse.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1347 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/move_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1515 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/multi_point_swipe.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2239 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/press_keys.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1623 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/scroll_mouse.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1574 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/swipe.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1610 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/tap_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1532 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/InputActions/tilt.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.295115 alttester_driver-2.1.1/alttester/commands/Notifications/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1149 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/Notifications/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1579 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/Notifications/base_notification_callbacks.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      894 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/Notifications/load_scene_mode.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      869 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/Notifications/load_scene_notification_result.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      878 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/Notifications/log_notification_result.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      838 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/Notifications/notification_type.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.303182 alttester_driver-2.1.1/alttester/commands/ObjectCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1448 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2587 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/call_method.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1499 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/click_element.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1209 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/get_all_components.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1605 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/get_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1175 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/get_text.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1209 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/pointer_down.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1209 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/pointer_enter.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1189 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/pointer_exit.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1189 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/pointer_up.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1610 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/set_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1321 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/set_text.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1495 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/ObjectCommands/tap_element.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.313381 alttester_driver-2.1.1/alttester/commands/UnityCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1578 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      940 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/delete_player_pref.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1179 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/delete_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      944 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/get_all_loaded_scenes.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      974 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/get_current_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1668 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/get_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1075 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/get_time_scale.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1409 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/load_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2037 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/set_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1410 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/set_time_scale.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1337 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/unload_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1710 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1256 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     7982 2024-04-01 07:09:49.000000 alttester_driver-2.1.1/alttester/commands/base_command.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1187 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/get_png_screenshot.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      940 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/get_server_version.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1574 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/get_static_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1554 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/commands/set_static_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5039 2024-04-10 07:45:53.000000 alttester_driver-2.1.1/alttester/exceptions.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     8202 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/keycode.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1033 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/logging.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      960 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/playerpref.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1680 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/alttester/reverse_port_forwarding.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      300 2024-04-15 07:14:09.000000 alttester_driver-2.1.1/requirements-dev.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       50 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/requirements.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       38 2024-05-16 09:09:50.334577 alttester_driver-2.1.1/setup.cfg
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3351 2024-01-09 14:51:06.000000 alttester_driver-2.1.1/setup.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.243133 alttester_driver-2.1.1/tests/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.327886 alttester_driver-2.1.1/tests/integration/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      699 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/tests/integration/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     7353 2024-04-15 07:14:09.000000 alttester_driver-2.1.1/tests/integration/conftest.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5110 2024-04-01 07:09:49.000000 alttester_driver-2.1.1/tests/integration/test_driver.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4366 2024-01-09 14:51:06.000000 alttester_driver-2.1.1/tests/integration/test_notifications.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1512 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/tests/integration/test_reverse_port_forwarding.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    21323 2024-03-25 08:05:11.000000 alttester_driver-2.1.1/tests/integration/test_scene01_part1.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    18718 2024-03-25 08:05:11.000000 alttester_driver-2.1.1/tests/integration/test_scene01_part2.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5202 2024-03-25 08:05:11.000000 alttester_driver-2.1.1/tests/integration/test_scene02.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     6527 2024-03-25 08:05:11.000000 alttester_driver-2.1.1/tests/integration/test_scene03.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5191 2024-04-10 07:45:53.000000 alttester_driver-2.1.1/tests/integration/test_scene05.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4478 2024-03-25 08:05:11.000000 alttester_driver-2.1.1/tests/integration/test_scene07.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2306 2024-03-25 08:05:11.000000 alttester_driver-2.1.1/tests/integration/test_scene09.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4259 2024-03-25 08:05:11.000000 alttester_driver-2.1.1/tests/integration/test_scene10.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1114 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/tests/integration/utils.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-05-16 09:09:50.331145 alttester_driver-2.1.1/tests/unit/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      699 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/tests/unit/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2368 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/tests/unit/test_altobject.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2229 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/tests/unit/test_commands.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     6103 2023-11-07 12:46:27.000000 alttester_driver-2.1.1/tests/unit/test_websocket.py
```

### Comparing `alttester_driver-2.1.0/AltTester_Driver.egg-info/PKG-INFO` & `alttester_driver-2.1.1/AltTester_Driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AltTester-Driver
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python bindings for the AltTester® framework. AltTester® is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
 Home-page: https://alttester.com/docs/sdk/latest/
 Author: Altom Consulting
 Author-email: contact@alttester.com
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
 Project-URL: Documentation, https://alttester.com/docs/sdk/latest
```

### Comparing `alttester_driver-2.1.0/AltTester_Driver.egg-info/SOURCES.txt` & `alttester_driver-2.1.1/AltTester_Driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/PKG-INFO` & `alttester_driver-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AltTester-Driver
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python bindings for the AltTester® framework. AltTester® is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
 Home-page: https://alttester.com/docs/sdk/latest/
 Author: Altom Consulting
 Author-email: contact@alttester.com
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
 Project-URL: Documentation, https://alttester.com/docs/sdk/latest
```

### Comparing `alttester_driver-2.1.0/README.md` & `alttester_driver-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/__init__.py` & `alttester_driver-2.1.1/alttester/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/__version__.py` & `alttester_driver-2.1.1/alttester/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program. If not, see <https://www.gnu.org/licenses/>.
 """
 
-VERSION = "2.1.0"
+VERSION = "2.1.1"
```

### Comparing `alttester_driver-2.1.0/alttester/_websocket.py` & `alttester_driver-2.1.1/alttester/_websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
                 raise exceptions.MultipleDriversTryingToConnectException(
                     reason)
             if close_message[0] == 4009:
                 raise exceptions.MaxNoOfConnectionsDriversExceeded(
                     reason)
 
             raise exceptions.ConnectionError(
-                "Connection closed by AltTester® Server with reason: {}.".format(reason))
+                "Connection closed by AltTester(R) Server with reason: {}.".format(reason))
 
     def _check_errors(self):
         if self._errors:
             error = self._errors.pop()
             self.close()
             raise exceptions.ConnectionError(error)
 
@@ -259,15 +259,15 @@
         logger.error("Error: {}", error)
         self._errors.append(error)
 
     def _on_close(self, ws, close_status_code, close_msg):
         """A callback which is called when the connection is closed."""
 
         logger.debug(
-            "Connection to AltTester® Server closed with status code: {} and message: '{}'.",
+            "Connection to AltTester(R) Server closed with status code: {} and message: '{}'.",
             close_status_code,
             close_msg
         )
 
         self._close_message = (close_status_code, close_msg)
         self._driver_registered_called = False
         self._is_open = False
@@ -310,15 +310,15 @@
 
             if self._is_open:  # Added this to be also backward compatible but it will be slower
                 return
 
         self._check_close_message(last_close_message)
         self._check_errors()
         raise exceptions.ConnectionTimeoutError(
-            "Failed to connect to AltTester® Server host: {} port: {}.".format(
+            "Failed to connect to AltTester(R) Server host: {} port: {}.".format(
                 self.host, self.port)
         )
 
     def send(self, data):
         self._ensure_connection_is_open()
 
         message = json.dumps(data)
@@ -341,15 +341,15 @@
 
         if elapsed_time > self.command_timeout:
             self._command_handler.timeout()
             raise exceptions.CommandResponseTimeoutException()
 
     def close(self):
         logger.info(
-            "Closing connection to AltTester® Server on host: {} port: {}", self.host, self.port)
+            "Closing connection to AltTester(R) Server on host: {} port: {}", self.host, self.port)
 
         if self._websocket:
             self._websocket.close()
             self._websocket = None
 
         if self._thread:
             self._thread.join(0)
```

### Comparing `alttester_driver-2.1.0/alttester/altdriver.py` & `alttester_driver-2.1.1/alttester/altdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         self.platform_version = platform_version
         self.device_instance_id = device_instance_id
         self.app_id = app_id
 
         self._config_logging(self.enable_logging)
 
         logger.debug(
-            "Connecting to AltTester® on host: '{}', port: '{}' and app name: '{}'.",
+            "Connecting to AltTester(R) on host: '{}', port: '{}' and app name: '{}'.",
             self.host,
             self.port,
             self.app_name
         )
 
         self._command_handler = CommandHandler()
         self._notification_handler = NotificationHandler()
@@ -127,21 +127,21 @@
     @staticmethod
     def _split_version(version):
         parts = version.split(".")
         return (parts[0], parts[1]) if len(parts) > 1 else ("", "")
 
     def _check_server_version(self):
         server_version = commands.GetServerVersion.run(self._connection)
-        logger.info("Connection established with instrumented Unity app. AltTester® Version: {}", server_version)
+        logger.info("Connection established with instrumented Unity app. AltTester(R) Version: {}", server_version)
 
         major_server, minor_server = self._split_version(server_version)
         major_driver, minor_driver = self._split_version(VERSION)
 
         if major_server != major_driver or minor_server != minor_driver:
-            message = "Version mismatch. AltDriver version is {}. AltTester® version is {}.".format(
+            message = "Version mismatch. AltDriver version is {}. AltTester(R) version is {}.".format(
                 VERSION,
                 server_version
             )
 
             logger.warning(message)
 
     def _get_alt_object(self, data):
```

### Comparing `alttester_driver-2.1.0/alttester/altobject.py` & `alttester_driver-2.1.1/alttester/altobject.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/by.py` & `alttester_driver-2.1.1/alttester/by.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/AltTesterCommands/__init__.py` & `alttester_driver-2.1.1/alttester/commands/AltTesterCommands/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/AltTesterCommands/add_notification_listener.py` & `alttester_driver-2.1.1/alttester/commands/AltTesterCommands/add_notification_listener.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/AltTesterCommands/remove_notification_listener.py` & `alttester_driver-2.1.1/alttester/commands/AltTesterCommands/remove_notification_listener.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/AltTesterCommands/reset_input.py` & `alttester_driver-2.1.1/alttester/commands/AltTesterCommands/reset_input.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/AltTesterCommands/set_server_logging.py` & `alttester_driver-2.1.1/alttester/commands/AltTesterCommands/set_server_logging.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/__init__.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/find_object.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/find_object.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/find_object_at_coordinates.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/find_object_at_coordinates.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/find_object_which_contains.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/find_object_which_contains.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/find_objects.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/find_objects.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/find_objects_which_contains.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/find_objects_which_contains.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_component_property.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/wait_for_component_property.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/wait_for_object.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object_which_contains.py` & `alttester_driver-2.1.1/alttester/commands/FindObjects/wait_for_object_which_contains.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/__init__.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/begin_touch.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/begin_touch.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/click_coordinates.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/click_coordinates.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/end_touch.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/end_touch.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/keys_down.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/keys_down.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/keys_up.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/keys_up.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/move_mouse.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/move_mouse.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/move_touch.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/move_touch.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/multi_point_swipe.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/multi_point_swipe.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/press_keys.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/press_keys.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/scroll_mouse.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/scroll_mouse.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/swipe.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/swipe.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/tap_coordinates.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/tap_coordinates.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/InputActions/tilt.py` & `alttester_driver-2.1.1/alttester/commands/InputActions/tilt.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/Notifications/__init__.py` & `alttester_driver-2.1.1/alttester/commands/Notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/Notifications/base_notification_callbacks.py` & `alttester_driver-2.1.1/alttester/commands/Notifications/base_notification_callbacks.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/Notifications/load_scene_mode.py` & `alttester_driver-2.1.1/alttester/commands/Notifications/load_scene_mode.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/Notifications/load_scene_notification_result.py` & `alttester_driver-2.1.1/alttester/commands/Notifications/load_scene_notification_result.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/Notifications/log_notification_result.py` & `alttester_driver-2.1.1/alttester/commands/Notifications/log_notification_result.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/Notifications/notification_type.py` & `alttester_driver-2.1.1/alttester/commands/Notifications/notification_type.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/__init__.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/call_method.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/call_method.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/click_element.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/click_element.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_all_components.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/get_all_components.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_component_property.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/get_component_property.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_text.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/get_text.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_down.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/pointer_down.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_enter.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/pointer_enter.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_exit.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/pointer_exit.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_up.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/pointer_up.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/set_component_property.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/set_component_property.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/set_text.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/set_text.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/ObjectCommands/tap_element.py` & `alttester_driver-2.1.1/alttester/commands/ObjectCommands/tap_element.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/__init__.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/delete_player_pref.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/delete_player_pref.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/delete_player_pref_key.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/delete_player_pref_key.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/get_all_loaded_scenes.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/get_all_loaded_scenes.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/get_current_scene.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/get_current_scene.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/get_player_pref_key.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/get_player_pref_key.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/get_time_scale.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/get_time_scale.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/load_scene.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/load_scene.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/set_player_pref_key.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/set_player_pref_key.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/set_time_scale.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/set_time_scale.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/unload_scene.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/unload_scene.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py` & `alttester_driver-2.1.1/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/__init__.py` & `alttester_driver-2.1.1/alttester/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/base_command.py` & `alttester_driver-2.1.1/alttester/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/get_png_screenshot.py` & `alttester_driver-2.1.1/alttester/commands/get_png_screenshot.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/get_server_version.py` & `alttester_driver-2.1.1/alttester/commands/get_server_version.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/get_static_property.py` & `alttester_driver-2.1.1/alttester/commands/get_static_property.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/commands/set_static_property.py` & `alttester_driver-2.1.1/alttester/commands/set_static_property.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/exceptions.py` & `alttester_driver-2.1.1/alttester/exceptions.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/keycode.py` & `alttester_driver-2.1.1/alttester/keycode.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/logging.py` & `alttester_driver-2.1.1/alttester/logging.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/playerpref.py` & `alttester_driver-2.1.1/alttester/playerpref.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/alttester/reverse_port_forwarding.py` & `alttester_driver-2.1.1/alttester/reverse_port_forwarding.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/setup.py` & `alttester_driver-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/__init__.py` & `alttester_driver-2.1.1/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/conftest.py` & `alttester_driver-2.1.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_driver.py` & `alttester_driver-2.1.1/tests/integration/test_driver.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_notifications.py` & `alttester_driver-2.1.1/tests/integration/test_notifications.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_reverse_port_forwarding.py` & `alttester_driver-2.1.1/tests/integration/test_reverse_port_forwarding.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_scene01_part1.py` & `alttester_driver-2.1.1/tests/integration/test_scene01_part1.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_scene01_part2.py` & `alttester_driver-2.1.1/tests/integration/test_scene01_part2.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_scene02.py` & `alttester_driver-2.1.1/tests/integration/test_scene02.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_scene03.py` & `alttester_driver-2.1.1/tests/integration/test_scene03.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_scene05.py` & `alttester_driver-2.1.1/tests/integration/test_scene05.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_scene07.py` & `alttester_driver-2.1.1/tests/integration/test_scene07.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_scene09.py` & `alttester_driver-2.1.1/tests/integration/test_scene09.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/test_scene10.py` & `alttester_driver-2.1.1/tests/integration/test_scene10.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/integration/utils.py` & `alttester_driver-2.1.1/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/unit/__init__.py` & `alttester_driver-2.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/unit/test_altobject.py` & `alttester_driver-2.1.1/tests/unit/test_altobject.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/unit/test_commands.py` & `alttester_driver-2.1.1/tests/unit/test_commands.py`

 * *Files identical despite different names*

### Comparing `alttester_driver-2.1.0/tests/unit/test_websocket.py` & `alttester_driver-2.1.1/tests/unit/test_websocket.py`

 * *Files identical despite different names*

