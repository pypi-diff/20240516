# Comparing `tmp/geckordp-0.4.53.zip` & `tmp/geckordp-0.5.0.zip`

## zipinfo {}

```diff
@@ -1,104 +1,107 @@
-Zip file size: 97088 bytes, number of entries: 102
--rwxr-xr-x  3.0 unx     6154 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/utils.py
--rwxr-xr-x  3.0 unx     1956 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/logger.py
--rwxr-xr-x  3.0 unx     5137 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/settings.py
--rwxr-xr-x  3.0 unx      994 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/__init__.py
--rwxr-xr-x  3.0 unx     1550 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/buffers.py
--rw-rw-r--  3.0 unx    20460 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/profile.py
--rwxr-xr-x  3.0 unx     5481 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/firefox.py
--rw-rw-r--  3.0 unx    30688 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/rdp_client.py
--rwxr-xr-x  3.0 unx     1385 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/screenshot.py
--rwxr-xr-x  3.0 unx     3183 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/node.py
--rwxr-xr-x  3.0 unx     5396 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/source.py
--rw-rw-r--  3.0 unx    12633 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/walker.py
--rwxr-xr-x  3.0 unx      775 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/node_list.py
--rw-rw-r--  3.0 unx     4427 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/storage.py
--rwxr-xr-x  3.0 unx      493 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/heap_snapshot.py
--rwxr-xr-x  3.0 unx     1730 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/network_content.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/__init__.py
--rwxr-xr-x  3.0 unx      898 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/simulator.py
--rwxr-xr-x  3.0 unx      903 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/accessibility.py
--rwxr-xr-x  3.0 unx     2429 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/accessible_walker.py
--rwxr-xr-x  3.0 unx     1147 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/accessible.py
--rwxr-xr-x  3.0 unx      699 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/accessibility/parent_accessibility.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/__init__.py
--rwxr-xr-x  3.0 unx     2067 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/preference.py
--rwxr-xr-x  3.0 unx     2736 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/network_event.py
--rwxr-xr-x  3.0 unx     4023 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/memory.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/addon/__init__.py
--rwxr-xr-x  3.0 unx      672 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/addon/addons.py
--rwxr-xr-x  3.0 unx     2526 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/addon/web_extension_inspected_window.py
--rwxr-xr-x  3.0 unx     3655 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/web_console.py
--rwxr-xr-x  3.0 unx     1907 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/root.py
--rwxr-xr-x  3.0 unx      481 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/string.py
--rwxr-xr-x  3.0 unx      531 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/worker.py
--rwxr-xr-x  3.0 unx      805 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/process.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/__init__.py
--rwxr-xr-x  3.0 unx     1304 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/tab.py
--rwxr-xr-x  3.0 unx      696 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/descriptors/web_extension.py
--rwxr-xr-x  3.0 unx      549 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/web_socket.py
--rwxr-xr-x  3.0 unx     4076 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/watcher.py
--rwxr-xr-x  3.0 unx      414 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/device.py
--rwxr-xr-x  3.0 unx     8326 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/thread.py
--rwxr-xr-x  3.0 unx     7130 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/events.py
--rwxr-xr-x  3.0 unx     2244 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/network_parent.py
--rwxr-xr-x  3.0 unx      439 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/actor.py
--rwxr-xr-x  3.0 unx     2193 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/target_configuration.py
--rw-rw-r--  3.0 unx     2139 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/targets/window_global.py
--rwxr-xr-x  3.0 unx      662 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/targets/content_process.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/targets/__init__.py
--rwxr-xr-x  3.0 unx     3159 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp/actors/inspector.py
--rw-rw-r--  3.0 unx       15 t- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/top_level.txt
--rw-rw-r--  3.0 unx       99 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/requires.txt
--rw-rw-r--  3.0 unx    12070 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/PKG-INFO
--rw-rw-r--  3.0 unx        1 t- stor 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/dependency_links.txt
--rw-rw-r--  3.0 unx     3337 t- defN 81-Jan-01 02:01 geckordp-0.4.53/geckordp.egg-info/SOURCES.txt
--rwxr-xr-x  3.0 unx     2411 t- defN 81-Jan-01 02:01 geckordp-0.4.53/setup.py
--rwxr-xr-x  3.0 unx      158 t- defN 81-Jan-01 02:01 geckordp-0.4.53/setup.cfg
--rw-rw-r--  3.0 unx    12070 t- defN 81-Jan-01 02:01 geckordp-0.4.53/PKG-INFO
--rw-rw-r--  3.0 unx    11158 t- defN 81-Jan-01 02:01 geckordp-0.4.53/README.md
--rwxr-xr-x  3.0 unx     1180 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/helpers/utils.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/helpers/__init__.py
--rwxr-xr-x  3.0 unx      129 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/helpers/constants.py
--rwxr-xr-x  3.0 unx     3079 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_cookie.py
--rwxr-xr-x  3.0 unx     2772 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_source.py
--rwxr-xr-x  3.0 unx     4313 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_node.py
--rwxr-xr-x  3.0 unx     2970 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_inspector.py
--rwxr-xr-x  3.0 unx     2442 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_root.py
--rwxr-xr-x  3.0 unx     3756 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_memory.py
--rwxr-xr-x  3.0 unx     1713 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_simulator.py
--rwxr-xr-x  3.0 unx     1326 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_parent_accessibility.py
--rwxr-xr-x  3.0 unx     2363 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_accessible.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/__init__.py
--rwxr-xr-x  3.0 unx     3201 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_accessible_walker.py
--rwxr-xr-x  3.0 unx     1711 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/accessibility/test_accessibility.py
--rwxr-xr-x  3.0 unx     1467 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_heap_snapshot.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/__init__.py
--rw-rw-r--  3.0 unx     4134 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_network_event.py
--rw-rw-r--  3.0 unx     1604 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_network_content.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/addon/__init__.py
--rwxr-xr-x  3.0 unx      746 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/addon/test_addons.py
--rwxr-xr-x  3.0 unx     1601 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/addon/test_web_extension_inspected_window.py
--rwxr-xr-x  3.0 unx      735 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_device.py
--rwxr-xr-x  3.0 unx     2876 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_network_parent.py
--rwxr-xr-x  3.0 unx     2883 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_local.py
--rwxr-xr-x  3.0 unx     3532 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_watcher.py
--rwxr-xr-x  3.0 unx     1119 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/test_tab.py
--rwxr-xr-x  3.0 unx     1800 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/test_web_extension.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/__init__.py
--rwxr-xr-x  3.0 unx      859 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/test_worker.py
--rwxr-xr-x  3.0 unx     1004 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/descriptors/test_process.py
--rwxr-xr-x  3.0 unx     2425 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_cache.py
--rwxr-xr-x  3.0 unx     3785 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_web_console.py
--rwxr-xr-x  3.0 unx     1599 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_node_list.py
--rwxr-xr-x  3.0 unx      966 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_screenshot.py
--rwxr-xr-x  3.0 unx     3030 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_preference.py
--rwxr-xr-x  3.0 unx     2157 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_indexed.py
--rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/targets/__init__.py
--rw-rw-r--  3.0 unx     2886 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/targets/test_window_global.py
--rwxr-xr-x  3.0 unx     1300 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/targets/test_content_process.py
--rwxr-xr-x  3.0 unx     2931 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_session.py
--rw-rw-r--  3.0 unx     5472 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_thread.py
--rwxr-xr-x  3.0 unx      785 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_storage_extension.py
--rw-rw-r--  3.0 unx    14235 t- defN 81-Jan-01 02:01 geckordp-0.4.53/tests/actors/test_walker.py
-102 files, 299457 bytes uncompressed, 79560 bytes compressed:  73.4%
+Zip file size: 100474 bytes, number of entries: 105
+-rwxr-xr-x  3.0 unx     6179 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/utils.py
+-rwxr-xr-x  3.0 unx     1988 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/logger.py
+-rwxr-xr-x  3.0 unx     5097 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/settings.py
+-rwxr-xr-x  3.0 unx      992 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/__init__.py
+-rwxr-xr-x  3.0 unx     1518 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/buffers.py
+-rw-rw-r--  3.0 unx    20320 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/profile.py
+-rw-rw-r--  3.0 unx     5507 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/firefox.py
+-rw-rw-r--  3.0 unx    33105 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/rdp_client.py
+-rwxr-xr-x  3.0 unx     1256 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/screenshot.py
+-rwxr-xr-x  3.0 unx     3725 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/node.py
+-rwxr-xr-x  3.0 unx     5461 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/source.py
+-rw-rw-r--  3.0 unx    14924 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/walker.py
+-rwxr-xr-x  3.0 unx      883 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/node_list.py
+-rw-rw-r--  3.0 unx     4959 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/storage.py
+-rwxr-xr-x  3.0 unx      525 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/heap_snapshot.py
+-rwxr-xr-x  3.0 unx     1827 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/network_content.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/accessibility/__init__.py
+-rwxr-xr-x  3.0 unx      937 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/accessibility/simulator.py
+-rwxr-xr-x  3.0 unx     1081 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/accessibility/accessibility.py
+-rwxr-xr-x  3.0 unx     2779 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/accessibility/accessible_walker.py
+-rwxr-xr-x  3.0 unx     1365 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/accessibility/accessible.py
+-rwxr-xr-x  3.0 unx      795 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/accessibility/parent_accessibility.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/__init__.py
+-rwxr-xr-x  3.0 unx     2164 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/preference.py
+-rwxr-xr-x  3.0 unx     3058 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/network_event.py
+-rwxr-xr-x  3.0 unx     4352 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/memory.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/addon/__init__.py
+-rwxr-xr-x  3.0 unx      705 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/addon/addons.py
+-rwxr-xr-x  3.0 unx     2717 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/addon/web_extension_inspected_window.py
+-rwxr-xr-x  3.0 unx     2042 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/thread_configuration.py
+-rwxr-xr-x  3.0 unx     3889 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/web_console.py
+-rw-rw-r--  3.0 unx     2151 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/resources.py
+-rwxr-xr-x  3.0 unx     1835 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/root.py
+-rwxr-xr-x  3.0 unx      530 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/string.py
+-rwxr-xr-x  3.0 unx      593 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/descriptors/worker.py
+-rwxr-xr-x  3.0 unx      834 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/descriptors/process.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/descriptors/__init__.py
+-rwxr-xr-x  3.0 unx     1390 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/descriptors/tab.py
+-rwxr-xr-x  3.0 unx      588 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/descriptors/web_extension.py
+-rwxr-xr-x  3.0 unx     2417 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/watcher.py
+-rwxr-xr-x  3.0 unx      455 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/device.py
+-rwxr-xr-x  3.0 unx     8771 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/thread.py
+-rwxr-xr-x  3.0 unx     6977 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/events.py
+-rwxr-xr-x  3.0 unx     2625 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/network_parent.py
+-rwxr-xr-x  3.0 unx      440 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/actor.py
+-rwxr-xr-x  3.0 unx     2432 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/target_configuration.py
+-rw-rw-r--  3.0 unx     2516 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/targets/window_global.py
+-rwxr-xr-x  3.0 unx      739 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/targets/content_process.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/targets/__init__.py
+-rwxr-xr-x  3.0 unx     3433 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp/actors/inspector.py
+-rw-rw-r--  3.0 unx       15 t- stor 81-Jan-01 02:01 geckordp-0.5.0/geckordp.egg-info/top_level.txt
+-rw-rw-r--  3.0 unx       99 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp.egg-info/requires.txt
+-rw-rw-r--  3.0 unx    12017 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp.egg-info/PKG-INFO
+-rw-rw-r--  3.0 unx        1 t- stor 81-Jan-01 02:01 geckordp-0.5.0/geckordp.egg-info/dependency_links.txt
+-rw-rw-r--  3.0 unx     3460 t- defN 81-Jan-01 02:01 geckordp-0.5.0/geckordp.egg-info/SOURCES.txt
+-rwxr-xr-x  3.0 unx     2417 t- defN 81-Jan-01 02:01 geckordp-0.5.0/setup.py
+-rwxr-xr-x  3.0 unx      158 t- defN 81-Jan-01 02:01 geckordp-0.5.0/setup.cfg
+-rw-rw-r--  3.0 unx    12017 t- defN 81-Jan-01 02:01 geckordp-0.5.0/PKG-INFO
+-rw-rw-r--  3.0 unx    11106 t- defN 81-Jan-01 02:01 geckordp-0.5.0/README.md
+-rwxr-xr-x  3.0 unx     2095 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/helpers/utils.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/tests/helpers/__init__.py
+-rwxr-xr-x  3.0 unx      129 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/helpers/constants.py
+-rwxr-xr-x  3.0 unx     3110 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_storage_cookie.py
+-rw-rw-r--  3.0 unx     1166 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_target_configuration.py
+-rwxr-xr-x  3.0 unx     2746 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_source.py
+-rwxr-xr-x  3.0 unx     4314 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_node.py
+-rwxr-xr-x  3.0 unx     2963 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_inspector.py
+-rwxr-xr-x  3.0 unx     2443 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_root.py
+-rwxr-xr-x  3.0 unx     3757 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_memory.py
+-rwxr-xr-x  3.0 unx     1701 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/accessibility/test_simulator.py
+-rwxr-xr-x  3.0 unx     1318 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/accessibility/test_parent_accessibility.py
+-rwxr-xr-x  3.0 unx     2320 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/accessibility/test_accessible.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/accessibility/__init__.py
+-rwxr-xr-x  3.0 unx     3158 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/accessibility/test_accessible_walker.py
+-rwxr-xr-x  3.0 unx     1740 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/accessibility/test_accessibility.py
+-rwxr-xr-x  3.0 unx     2242 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_heap_snapshot.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/__init__.py
+-rw-rw-r--  3.0 unx     4083 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_network_event.py
+-rw-rw-r--  3.0 unx     1592 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_network_content.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/addon/__init__.py
+-rwxr-xr-x  3.0 unx      748 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/addon/test_addons.py
+-rwxr-xr-x  3.0 unx     1569 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/addon/test_web_extension_inspected_window.py
+-rwxr-xr-x  3.0 unx      727 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_device.py
+-rwxr-xr-x  3.0 unx     2912 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_network_parent.py
+-rw-rw-r--  3.0 unx     2915 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_storage_local.py
+-rwxr-xr-x  3.0 unx     3578 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_watcher.py
+-rwxr-xr-x  3.0 unx     1120 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/descriptors/test_tab.py
+-rwxr-xr-x  3.0 unx     1735 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/descriptors/test_web_extension.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/descriptors/__init__.py
+-rwxr-xr-x  3.0 unx      860 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/descriptors/test_worker.py
+-rwxr-xr-x  3.0 unx      996 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/descriptors/test_process.py
+-rwxr-xr-x  3.0 unx     2458 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_storage_cache.py
+-rwxr-xr-x  3.0 unx     3901 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_web_console.py
+-rwxr-xr-x  3.0 unx     1600 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_node_list.py
+-rwxr-xr-x  3.0 unx      958 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_screenshot.py
+-rwxr-xr-x  3.0 unx     2993 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_preference.py
+-rwxr-xr-x  3.0 unx     2195 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_storage_indexed.py
+-rwxr-xr-x  3.0 unx        0 b- stor 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/targets/__init__.py
+-rw-rw-r--  3.0 unx     2878 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/targets/test_window_global.py
+-rwxr-xr-x  3.0 unx     1282 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/targets/test_content_process.py
+-rw-rw-r--  3.0 unx     1186 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_thread_configuration.py
+-rwxr-xr-x  3.0 unx     2963 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_storage_session.py
+-rw-rw-r--  3.0 unx     5292 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_thread.py
+-rwxr-xr-x  3.0 unx      787 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_storage_extension.py
+-rw-rw-r--  3.0 unx    14215 t- defN 81-Jan-01 02:01 geckordp-0.5.0/tests/actors/test_walker.py
+105 files, 314911 bytes uncompressed, 82592 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -1,307 +1,316 @@
-Filename: geckordp-0.4.53/geckordp/utils.py
+Filename: geckordp-0.5.0/geckordp/utils.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/logger.py
+Filename: geckordp-0.5.0/geckordp/logger.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/settings.py
+Filename: geckordp-0.5.0/geckordp/settings.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/__init__.py
+Filename: geckordp-0.5.0/geckordp/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/buffers.py
+Filename: geckordp-0.5.0/geckordp/buffers.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/profile.py
+Filename: geckordp-0.5.0/geckordp/profile.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/firefox.py
+Filename: geckordp-0.5.0/geckordp/firefox.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/rdp_client.py
+Filename: geckordp-0.5.0/geckordp/rdp_client.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/screenshot.py
+Filename: geckordp-0.5.0/geckordp/actors/screenshot.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/node.py
+Filename: geckordp-0.5.0/geckordp/actors/node.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/source.py
+Filename: geckordp-0.5.0/geckordp/actors/source.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/walker.py
+Filename: geckordp-0.5.0/geckordp/actors/walker.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/node_list.py
+Filename: geckordp-0.5.0/geckordp/actors/node_list.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/storage.py
+Filename: geckordp-0.5.0/geckordp/actors/storage.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/heap_snapshot.py
+Filename: geckordp-0.5.0/geckordp/actors/heap_snapshot.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/network_content.py
+Filename: geckordp-0.5.0/geckordp/actors/network_content.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/accessibility/__init__.py
+Filename: geckordp-0.5.0/geckordp/actors/accessibility/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/accessibility/simulator.py
+Filename: geckordp-0.5.0/geckordp/actors/accessibility/simulator.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/accessibility/accessibility.py
+Filename: geckordp-0.5.0/geckordp/actors/accessibility/accessibility.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/accessibility/accessible_walker.py
+Filename: geckordp-0.5.0/geckordp/actors/accessibility/accessible_walker.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/accessibility/accessible.py
+Filename: geckordp-0.5.0/geckordp/actors/accessibility/accessible.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/accessibility/parent_accessibility.py
+Filename: geckordp-0.5.0/geckordp/actors/accessibility/parent_accessibility.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/__init__.py
+Filename: geckordp-0.5.0/geckordp/actors/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/preference.py
+Filename: geckordp-0.5.0/geckordp/actors/preference.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/network_event.py
+Filename: geckordp-0.5.0/geckordp/actors/network_event.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/memory.py
+Filename: geckordp-0.5.0/geckordp/actors/memory.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/addon/__init__.py
+Filename: geckordp-0.5.0/geckordp/actors/addon/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/addon/addons.py
+Filename: geckordp-0.5.0/geckordp/actors/addon/addons.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/addon/web_extension_inspected_window.py
+Filename: geckordp-0.5.0/geckordp/actors/addon/web_extension_inspected_window.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/web_console.py
+Filename: geckordp-0.5.0/geckordp/actors/thread_configuration.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/root.py
+Filename: geckordp-0.5.0/geckordp/actors/web_console.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/string.py
+Filename: geckordp-0.5.0/geckordp/actors/resources.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/descriptors/worker.py
+Filename: geckordp-0.5.0/geckordp/actors/root.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/descriptors/process.py
+Filename: geckordp-0.5.0/geckordp/actors/string.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/descriptors/__init__.py
+Filename: geckordp-0.5.0/geckordp/actors/descriptors/worker.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/descriptors/tab.py
+Filename: geckordp-0.5.0/geckordp/actors/descriptors/process.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/descriptors/web_extension.py
+Filename: geckordp-0.5.0/geckordp/actors/descriptors/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/web_socket.py
+Filename: geckordp-0.5.0/geckordp/actors/descriptors/tab.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/watcher.py
+Filename: geckordp-0.5.0/geckordp/actors/descriptors/web_extension.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/device.py
+Filename: geckordp-0.5.0/geckordp/actors/watcher.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/thread.py
+Filename: geckordp-0.5.0/geckordp/actors/device.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/events.py
+Filename: geckordp-0.5.0/geckordp/actors/thread.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/network_parent.py
+Filename: geckordp-0.5.0/geckordp/actors/events.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/actor.py
+Filename: geckordp-0.5.0/geckordp/actors/network_parent.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/target_configuration.py
+Filename: geckordp-0.5.0/geckordp/actors/actor.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/targets/window_global.py
+Filename: geckordp-0.5.0/geckordp/actors/target_configuration.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/targets/content_process.py
+Filename: geckordp-0.5.0/geckordp/actors/targets/window_global.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/targets/__init__.py
+Filename: geckordp-0.5.0/geckordp/actors/targets/content_process.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp/actors/inspector.py
+Filename: geckordp-0.5.0/geckordp/actors/targets/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp.egg-info/top_level.txt
+Filename: geckordp-0.5.0/geckordp/actors/inspector.py
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp.egg-info/requires.txt
+Filename: geckordp-0.5.0/geckordp.egg-info/top_level.txt
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp.egg-info/PKG-INFO
+Filename: geckordp-0.5.0/geckordp.egg-info/requires.txt
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp.egg-info/dependency_links.txt
+Filename: geckordp-0.5.0/geckordp.egg-info/PKG-INFO
 Comment: 
 
-Filename: geckordp-0.4.53/geckordp.egg-info/SOURCES.txt
+Filename: geckordp-0.5.0/geckordp.egg-info/dependency_links.txt
 Comment: 
 
-Filename: geckordp-0.4.53/setup.py
+Filename: geckordp-0.5.0/geckordp.egg-info/SOURCES.txt
 Comment: 
 
-Filename: geckordp-0.4.53/setup.cfg
+Filename: geckordp-0.5.0/setup.py
 Comment: 
 
-Filename: geckordp-0.4.53/PKG-INFO
+Filename: geckordp-0.5.0/setup.cfg
 Comment: 
 
-Filename: geckordp-0.4.53/README.md
+Filename: geckordp-0.5.0/PKG-INFO
 Comment: 
 
-Filename: geckordp-0.4.53/tests/helpers/utils.py
+Filename: geckordp-0.5.0/README.md
 Comment: 
 
-Filename: geckordp-0.4.53/tests/helpers/__init__.py
+Filename: geckordp-0.5.0/tests/helpers/utils.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/helpers/constants.py
+Filename: geckordp-0.5.0/tests/helpers/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_storage_cookie.py
+Filename: geckordp-0.5.0/tests/helpers/constants.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_source.py
+Filename: geckordp-0.5.0/tests/actors/test_storage_cookie.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_node.py
+Filename: geckordp-0.5.0/tests/actors/test_target_configuration.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_inspector.py
+Filename: geckordp-0.5.0/tests/actors/test_source.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_root.py
+Filename: geckordp-0.5.0/tests/actors/test_node.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_memory.py
+Filename: geckordp-0.5.0/tests/actors/test_inspector.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/accessibility/test_simulator.py
+Filename: geckordp-0.5.0/tests/actors/test_root.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/accessibility/test_parent_accessibility.py
+Filename: geckordp-0.5.0/tests/actors/test_memory.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/accessibility/test_accessible.py
+Filename: geckordp-0.5.0/tests/actors/accessibility/test_simulator.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/accessibility/__init__.py
+Filename: geckordp-0.5.0/tests/actors/accessibility/test_parent_accessibility.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/accessibility/test_accessible_walker.py
+Filename: geckordp-0.5.0/tests/actors/accessibility/test_accessible.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/accessibility/test_accessibility.py
+Filename: geckordp-0.5.0/tests/actors/accessibility/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_heap_snapshot.py
+Filename: geckordp-0.5.0/tests/actors/accessibility/test_accessible_walker.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/__init__.py
+Filename: geckordp-0.5.0/tests/actors/accessibility/test_accessibility.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_network_event.py
+Filename: geckordp-0.5.0/tests/actors/test_heap_snapshot.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_network_content.py
+Filename: geckordp-0.5.0/tests/actors/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/addon/__init__.py
+Filename: geckordp-0.5.0/tests/actors/test_network_event.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/addon/test_addons.py
+Filename: geckordp-0.5.0/tests/actors/test_network_content.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/addon/test_web_extension_inspected_window.py
+Filename: geckordp-0.5.0/tests/actors/addon/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_device.py
+Filename: geckordp-0.5.0/tests/actors/addon/test_addons.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_network_parent.py
+Filename: geckordp-0.5.0/tests/actors/addon/test_web_extension_inspected_window.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_storage_local.py
+Filename: geckordp-0.5.0/tests/actors/test_device.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_watcher.py
+Filename: geckordp-0.5.0/tests/actors/test_network_parent.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/descriptors/test_tab.py
+Filename: geckordp-0.5.0/tests/actors/test_storage_local.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/descriptors/test_web_extension.py
+Filename: geckordp-0.5.0/tests/actors/test_watcher.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/descriptors/__init__.py
+Filename: geckordp-0.5.0/tests/actors/descriptors/test_tab.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/descriptors/test_worker.py
+Filename: geckordp-0.5.0/tests/actors/descriptors/test_web_extension.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/descriptors/test_process.py
+Filename: geckordp-0.5.0/tests/actors/descriptors/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_storage_cache.py
+Filename: geckordp-0.5.0/tests/actors/descriptors/test_worker.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_web_console.py
+Filename: geckordp-0.5.0/tests/actors/descriptors/test_process.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_node_list.py
+Filename: geckordp-0.5.0/tests/actors/test_storage_cache.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_screenshot.py
+Filename: geckordp-0.5.0/tests/actors/test_web_console.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_preference.py
+Filename: geckordp-0.5.0/tests/actors/test_node_list.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_storage_indexed.py
+Filename: geckordp-0.5.0/tests/actors/test_screenshot.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/targets/__init__.py
+Filename: geckordp-0.5.0/tests/actors/test_preference.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/targets/test_window_global.py
+Filename: geckordp-0.5.0/tests/actors/test_storage_indexed.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/targets/test_content_process.py
+Filename: geckordp-0.5.0/tests/actors/targets/__init__.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_storage_session.py
+Filename: geckordp-0.5.0/tests/actors/targets/test_window_global.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_thread.py
+Filename: geckordp-0.5.0/tests/actors/targets/test_content_process.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_storage_extension.py
+Filename: geckordp-0.5.0/tests/actors/test_thread_configuration.py
 Comment: 
 
-Filename: geckordp-0.4.53/tests/actors/test_walker.py
+Filename: geckordp-0.5.0/tests/actors/test_storage_session.py
+Comment: 
+
+Filename: geckordp-0.5.0/tests/actors/test_thread.py
+Comment: 
+
+Filename: geckordp-0.5.0/tests/actors/test_storage_extension.py
+Comment: 
+
+Filename: geckordp-0.5.0/tests/actors/test_walker.py
 Comment: 
 
 Zip file comment:
```

## Comparing `geckordp-0.4.53/geckordp/utils.py` & `geckordp-0.5.0/geckordp/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,36 +3,44 @@
 import subprocess
 import time
 from pathlib import Path
 from socket import socket
 from sys import platform
 from time import sleep
 from typing import List
+
 import psutil
-from geckordp.logger import exlog, dlog
+
+from geckordp.logger import dlog, exlog
 
 
-class ExpireAt():
+class ExpireAt:
 
     def __init__(self, sec: float):
         self.__start = time.time()
         self.__sec = sec
 
     def __bool__(self):
         return self.expired_time() < self.__sec
 
     def expired_time(self):
-        return (time.time() - self.__start)
+        return time.time() - self.__start
 
     def expired(self):
         return not self.__bool__()
 
 
-def wait_process_loaded(pid: int, timeout_sec=15.0, check_sec=0.3, no_activity_threshold=9.0, no_activity_min_count=6) -> bool:
-    """ Waits for a process til cpu activity settles down.
+def wait_process_loaded(
+    pid: int,
+    timeout_sec=15.0,
+    check_sec=0.3,
+    no_activity_threshold=9.0,
+    no_activity_min_count=6,
+) -> bool:
+    """Waits for a process til cpu activity settles down.
 
     Args:
         pid (int): The process ID.
         timeout_sec (float, optional): Maximum wait time. Defaults to 15.0.
         check_sec (float, optional): Interval between the measurements. Defaults to 0.3.
         no_activity_threshold (float, optional): The percentage threshold which sets the activity as low. Defaults to 9.0.
         no_activity_min_count (int, optional): The minimum amount to break on low activity. Defaults to 6.
@@ -40,40 +48,46 @@
     Returns:
         bool: True: if successful waited, False: failed to wait for process.
     """
     em = f"waiting for process[{pid}] failed"
     try:
         low_activity_in_row = 0
         proc_info = psutil.Process(pid)
-        if (not proc_info):
+        if not proc_info:
             return False
 
         exp = ExpireAt(timeout_sec)
         while exp:
             cpu = proc_info.cpu_percent(check_sec)
-            if (cpu < no_activity_threshold):
+            if cpu < no_activity_threshold:
                 low_activity_in_row += 1
             else:
                 low_activity_in_row = 0
-            if (low_activity_in_row >= no_activity_min_count):
+            if low_activity_in_row >= no_activity_min_count:
                 break
 
         dlog(f"expired={exp.expired()}")
         return not exp.expired()
     except psutil.NoSuchProcess:
         exlog(f"{em}, process no longer exists")
         return False
     except Exception as ex:
         exlog(f"{em}, wait 15 seconds:\n{ex}")
         sleep(15)
         return True
 
 
-def wait_dir_changed(path: Path, timeout_sec=20.0, check_sec=0.3, min_file_age_sec=8.0, ignore_files: list | None = None) -> bool:
-    """ Waits for the latest file modification in a path to reach a specified age in seconds.
+def wait_dir_changed(
+    path: Path,
+    timeout_sec=20.0,
+    check_sec=0.3,
+    min_file_age_sec=8.0,
+    ignore_files: list | None = None,
+) -> bool:
+    """Waits for the latest file modification in a path to reach a specified age in seconds.
 
     Args:
         path (Path): The input path to check for file modifications.
         timeout_sec (float, optional): Maximum wait time. Defaults to 20.0.
         check_sec (float, optional): Interval between the probes. Defaults to 0.3.
         min_file_age_sec (float, optional): Minimum file age. Defaults to 8.0.
         ignore_files (list, optional): Ignore a file if it contains a keyword in this list. Defaults to None.
@@ -118,85 +132,85 @@
         if latest_modification > min_file_age_sec and latest_file != "":
             return True
         sleep(check_sec)
     return False
 
 
 def kill(proc: subprocess.Popen) -> bool:
-    """ Kill a process by handle.
+    """Kill a process by handle.
 
     Args:
         proc (subprocess.Popen): The process handle.
 
     Returns:
         bool: True: if successful terminated, False: failed to terminate process.
     """
     try:
         success = True
         if platform == "win32":
             proc = subprocess.Popen(
-                ["taskkill", "/F", "/T", "/PID",
-                 str(proc.pid)],
+                ["taskkill", "/F", "/T", "/PID", str(proc.pid)],
                 shell=False,
                 stdout=subprocess.DEVNULL,
-                stderr=subprocess.STDOUT)
+                stderr=subprocess.STDOUT,
+            )
             success = proc.wait(5) == 0
         else:
             proc.send_signal(signal.SIGTERM)
         return success
     except Exception as ex:
         exlog(ex)
         return False
 
 
 def kill_by_pid(pid: int) -> bool:
-    """ Kill a process by handle.
+    """Kill a process by handle.
 
     Args:
         pid (int): The process ID.
 
     Returns:
         bool: True: if successful terminated, False: failed to terminate process.
     """
     try:
         success = True
         if platform == "win32":
             proc = subprocess.Popen(
-                ["taskkill", "/F", "/T", "/PID",
-                 str(pid)],
+                ["taskkill", "/F", "/T", "/PID", str(pid)],
                 shell=False,
                 stdout=subprocess.DEVNULL,
-                stderr=subprocess.STDOUT)
+                stderr=subprocess.STDOUT,
+            )
             success = proc.wait(5) == 0
         else:
             proc = psutil.Process(pid)
             proc.send_signal(signal.SIGTERM)
         return success
     except Exception as ex:
         exlog(ex)
         return False
 
 
 def find_free_ports(n=1) -> List[int]:
-    """ Searches for free ports to use.
+    """Searches for free ports to use.
 
         .. note::
             It can't be guaranteed that the returned ports stay free.
             However it is very unlikely it happens in real-world situations as long
             the operating system doesn't allocate and free ports all the time.
 
     Args:
         n (int, optional): The amount of free ports to search. Defaults to 1.
 
     Returns:
         List[int]: A list of free ports.
     """
-    if (n <= 0):
+    if n <= 0:
         return []
     sockets = []
     ports = []
     for _ in range(0, n):
         s = socket()
-        s.bind(('', 0))
+        s.bind(("", 0))
         sockets.append(s)
         ports.append(s.getsockname()[1])
     return ports
```

## Comparing `geckordp-0.4.53/geckordp/logger.py` & `geckordp-0.5.0/geckordp/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 import logging
-from pathlib import Path
 from json import dumps
-
+from pathlib import Path
 
 LOGGER_NAME = "geckordp"
 __STDOUT_HANDLER = None
 __FILE_HANDLER = None
 log = logging.getLogger(LOGGER_NAME).info
 dlog = logging.getLogger(LOGGER_NAME).debug
 elog = logging.getLogger(LOGGER_NAME).error
 wlog = logging.getLogger(LOGGER_NAME).warning
 clog = logging.getLogger(LOGGER_NAME).critical
 exlog = logging.getLogger(LOGGER_NAME).exception
 
 
 def init_logger(log_level=logging.ERROR):
     global __STDOUT_HANDLER
-    if (__STDOUT_HANDLER is not None):
+    if __STDOUT_HANDLER is not None:
         return
 
     logger = logging.getLogger(LOGGER_NAME)
     logger.setLevel(logging.DEBUG)
 
     __STDOUT_HANDLER = logging.StreamHandler()
     __STDOUT_HANDLER.setLevel(log_level)
-    __STDOUT_HANDLER.setFormatter(logging.Formatter(
-        f'%(asctime)s [{LOGGER_NAME}][%(levelname)s] - %(funcName)s(): %(message)s'))
+    __STDOUT_HANDLER.setFormatter(
+        logging.Formatter(
+            f"%(asctime)s [{LOGGER_NAME}][%(levelname)s] - %(funcName)s(): %(message)s"
+        )
+    )
     logger.addHandler(__STDOUT_HANDLER)
 
 
 def set_file_logger(log_path: Path, log_level=logging.DEBUG):
     global __FILE_HANDLER
-    if (log_path == ""):
+    if log_path == "":
         return
 
     logger = logging.getLogger(LOGGER_NAME)
     log_file = str(Path(log_path))
     try:
-        open(log_file, 'w', encoding='utf-8').close()
+        open(log_file, "w", encoding="utf-8").close()
     except:
         pass
 
-    if (__FILE_HANDLER is not None):
+    if __FILE_HANDLER is not None:
         logger.removeHandler(__FILE_HANDLER)
     __FILE_HANDLER = logging.FileHandler(log_file)
     __FILE_HANDLER.setLevel(log_level)
-    __FILE_HANDLER.setFormatter(logging.Formatter(
-        '%(asctime)s [%(levelname)s] [%(module)s.py:%(lineno)s in %(funcName)s] - %(message)s'))
+    __FILE_HANDLER.setFormatter(
+        logging.Formatter(
+            "%(asctime)s [%(levelname)s] [%(module)s.py:%(lineno)s in %(funcName)s] - %(message)s"
+        )
+    )
     logger.addHandler(__FILE_HANDLER)
 
 
 def set_file_log_level(log_level=logging.DEBUG):
-    if (__FILE_HANDLER is None):
-        raise RuntimeError(
-            "file logger was not initialized with 'set_file_logger()'")
+    if __FILE_HANDLER is None:
+        raise RuntimeError("file logger was not initialized with 'set_file_logger()'")
     __FILE_HANDLER.setLevel(log_level)
 
 
 def set_stdout_log_level(log_level=logging.DEBUG):
     assert __STDOUT_HANDLER is not None
     __STDOUT_HANDLER.setLevel(log_level)
```

## Comparing `geckordp-0.4.53/geckordp/settings.py` & `geckordp-0.5.0/geckordp/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,173 +1,174 @@
 from pathlib import Path
+
 from geckordp.logger import *
+
 # pylint: disable=invalid-name
 
 
-class Settings():
-    """ Global settings for geckordp.
-    """
+class Settings:
+    """Global settings for geckordp."""
 
     def __init__(self):
         self.__XDEBUG = 0
         self.__XDEBUG_EVENTS = 0
         self.__XDEBUG_REQUEST = 0
         self.__XDEBUG_REQUEST_FORMAT = 1
         self.__XDEBUG_RESPONSE = 0
         self.__XDEBUG_RESPONSE_FORMAT = 1
         self.__XLOG_FILE = ""
         self.__XLOG_LEVEL = "info"
 
     @property
     def DEBUG(self) -> int:
-        """ Sets geckordp in debug mode.
+        """Sets geckordp in debug mode.
         Environment variable: GECKORDP_DEBUG
 
         Returns:
             int: 0: disabled, 1: enabled
         """
         return self.__XDEBUG
 
     @DEBUG.setter
     def DEBUG(self, value: int):
-        if (type(self.__XDEBUG) != type(value)):
+        if type(self.__XDEBUG) != type(value):
             print(f"invalid value '{value}' for 'DEBUG'")
             return
         set_stdout_log_level(logging.DEBUG)
         self.__XDEBUG = value
 
     @property
     def DEBUG_EVENTS(self) -> int:
-        """ Logs all received events.
+        """Logs all received events.
         Environment variable: GECKORDP_DEBUG_EVENTS
 
         Returns:
             int: 0: disabled, 1: enabled
         """
         return self.__XDEBUG_EVENTS
 
     @DEBUG_EVENTS.setter
     def DEBUG_EVENTS(self, value: int):
-        if (type(self.__XDEBUG_EVENTS) != type(value)):
+        if type(self.__XDEBUG_EVENTS) != type(value):
             print(f"invalid value '{value}' for 'DEBUG_EVENTS'")
             return
         self.__XDEBUG_EVENTS = value
 
     @property
     def DEBUG_REQUEST(self) -> int:
-        """ Logs all sent requests.
+        """Logs all sent requests.
         Environment variable: GECKORDP_DEBUG_REQUEST
 
         Returns:
             int: 0: disabled, 1: enabled
         """
         return self.__XDEBUG_REQUEST
 
     @DEBUG_REQUEST.setter
     def DEBUG_REQUEST(self, value: int):
-        if (type(self.__XDEBUG_REQUEST) != type(value)):
+        if type(self.__XDEBUG_REQUEST) != type(value):
             print(f"invalid value '{value}' for 'DEBUG_REQUEST'")
             return
         self.__XDEBUG_REQUEST = value
 
     @property
     def DEBUG_REQUEST_FORMAT(self) -> int:
-        """ Formats the debug print output of the sent requests.
+        """Formats the debug print output of the sent requests.
         Environment variable: GECKORDP_DEBUG_REQUEST_FORMAT
 
         Returns:
             int: 0: disabled, 1: enabled
         """
         return self.__XDEBUG_REQUEST_FORMAT
 
     @DEBUG_REQUEST_FORMAT.setter
     def DEBUG_REQUEST_FORMAT(self, value: int):
-        if (type(self.__XDEBUG_REQUEST_FORMAT) != type(value)):
+        if type(self.__XDEBUG_REQUEST_FORMAT) != type(value):
             print(f"invalid value '{value}' for 'DEBUG_REQUEST_FORMAT'")
             return
         self.__XDEBUG_REQUEST_FORMAT = value
 
     @property
     def DEBUG_RESPONSE(self) -> int:
-        """ Logs all received responses.
+        """Logs all received responses.
         Environment variable: GECKORDP_DEBUG_RESPONSE
 
         Returns:
             int: 0: disabled, 1: enabled
         """
         return self.__XDEBUG_RESPONSE
 
     @DEBUG_RESPONSE.setter
     def DEBUG_RESPONSE(self, value: int):
-        if (type(self.__XDEBUG_RESPONSE) != type(value)):
+        if type(self.__XDEBUG_RESPONSE) != type(value):
             print(f"invalid value '{value}' for 'DEBUG_RESPONSE'")
             return
         self.__XDEBUG_RESPONSE = value
 
     @property
     def DEBUG_RESPONSE_FORMAT(self) -> int:
-        """ Formats the debug print output of the received responses.
+        """Formats the debug print output of the received responses.
         Environment variable: GECKORDP_DEBUG_RESPONSE_FORMAT
 
         Returns:
             int: 0: disabled, 1: enabled
         """
         return self.__XDEBUG_RESPONSE_FORMAT
 
     @DEBUG_RESPONSE_FORMAT.setter
     def DEBUG_RESPONSE_FORMAT(self, value: int):
-        if (type(self.__XDEBUG_RESPONSE_FORMAT) != type(value)):
+        if type(self.__XDEBUG_RESPONSE_FORMAT) != type(value):
             print(f"invalid value '{value}' for 'DEBUG_RESPONSE_FORMAT'")
             return
         self.__XDEBUG_RESPONSE_FORMAT = value
 
     @property
     def LOG_FILE(self) -> str:
-        """ Write logs to file.
+        """Write logs to file.
         Environment variable: GECKORDP_LOG_FILE
 
         Returns:
             str: "": disabled, "xyz.log": enabled
         """
         return self.__XLOG_FILE
 
     @LOG_FILE.setter
     def LOG_FILE(self, value: str):
-        if (type(self.__XLOG_FILE) != type(value)):
+        if type(self.__XLOG_FILE) != type(value):
             print(f"invalid value '{value}' for 'LOG_FILE'")
             return
         self.__XLOG_FILE = value
         set_file_logger(Path(self.__XLOG_FILE).absolute())
 
     @property
     def LOG_LEVEL(self) -> str:
-        """ The log level.
+        """The log level.
         Environment variable: GECKORDP_LOG_LEVEL
 
         Returns:
             str: "debug", "info", "warn", "error", "fatal"
         """
         return self.__XLOG_LEVEL
 
     @LOG_LEVEL.setter
     def LOG_LEVEL(self, value: str):
-        if (type(self.__XLOG_LEVEL) != type(value)):
+        if type(self.__XLOG_LEVEL) != type(value):
             print(f"invalid value '{value}' for 'LOG_LEVEL'")
             return
         self.__XLOG_LEVEL = value
         level = logging.INFO
-        if (value == "debug"):
+        if value == "debug":
             level = logging.DEBUG
-        elif (value == "info"):
+        elif value == "info":
             level = logging.INFO
-        elif (value == "warn"):
+        elif value == "warn":
             level = logging.WARN
-        elif (value == "error"):
+        elif value == "error":
             level = logging.ERROR
-        elif (value == "fatal"):
+        elif value == "fatal":
             level = logging.FATAL
         else:
             print(f"invalid value '{value}' for 'LOG_LEVEL'")
             return
         set_stdout_log_level(level)
```

## Comparing `geckordp-0.4.53/geckordp/__init__.py` & `geckordp-0.5.0/geckordp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
-from geckordp.settings import *
+
 import geckordp.settings
+from geckordp.settings import *
+
 # pylint: disable=invalid-name
 
 
 # check if environment variables are set and override it
 VAR_ID = "_Settings__X"
 for name, value in GECKORDP.__dict__.items():
     # check if correct variable
-    if (not name.startswith(VAR_ID)):
+    if not name.startswith(VAR_ID):
         continue
 
     # get required variables
     func_name = name.replace(VAR_ID, "")
     env_name = name.replace(VAR_ID, "GECKORDP_")
     env_value = os.environ.get(env_name, None)
 
     # check if environment variable was set
-    if (env_value is None):
+    if env_value is None:
         continue
 
     # try to convert value to class variable type
     try:
         env_value = type(value)(env_value)
     except Exception as ex:
         print(f"invalid type for environment variable '{env_name}':\n{ex}")
```

## Comparing `geckordp-0.4.53/geckordp/buffers.py` & `geckordp-0.5.0/geckordp/buffers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-class LinearBuffer():
+class LinearBuffer:
 
     def __init__(self, size: int):
         self.__max_size = size
         self.__alloc_size = 0
         self.__buffer = bytearray(size)
 
     def append(self, buffer: bytes):
         size = len(buffer)
-        if (self.__alloc_size + size > self.__max_size):
+        if self.__alloc_size + size > self.__max_size:
             return False
-        self.__memcpy(self.__buffer, self.__alloc_size,
-                      buffer, size)
+        self.__memcpy(self.__buffer, self.__alloc_size, buffer, size)
         self.__alloc_size += size
         return True
 
     def append_byte(self, byte: int):
         size = 1
-        if (self.__alloc_size + size > self.__max_size):
+        if self.__alloc_size + size > self.__max_size:
             return False
         self.__buffer[self.__alloc_size] = byte
         self.__alloc_size += size
         return True
 
     def clear(self):
         for i in range(0, self.__max_size):
@@ -31,20 +30,20 @@
         self.__alloc_size = 0
 
     def get(self):
         return memoryview(self.__buffer)
 
     def get_null_terminated(self):
         for i in range(0, self.__max_size):
-            if (self.__buffer[i] == 0x00):
+            if self.__buffer[i] == 0x00:
                 return memoryview(self.__buffer[0:i])
         return memoryview(self.__buffer)
 
     def get_truncated(self, size: int):
-        if (size >= self.__alloc_size):
+        if size >= self.__alloc_size:
             return None
         return memoryview(self.__buffer[0:size])
 
     def size(self):
         return self.__alloc_size
 
     def max_size(self):
```

## Comparing `geckordp-0.4.53/geckordp/profile.py` & `geckordp-0.5.0/geckordp/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-import re
-import json
 import configparser
-import subprocess
+import json
+import re
 import shutil
-from time import sleep
-from typing import List, Dict
+import subprocess
 from pathlib import Path
-from geckordp.utils import wait_dir_changed, kill
+from time import sleep
+from typing import Dict, List
+
 from geckordp.firefox import Firefox
-from geckordp.logger import log, dlog, elog, wlog, exlog
+from geckordp.logger import dlog, elog, exlog, log, wlog
+from geckordp.utils import kill, wait_dir_changed
+
 USER_PREF_REGEX = re.compile(r"\s*user_pref\(([\"'])(.+?)\1,\s*(.+?)\);")
 
 
-class FirefoxProfile():
-    """ An instance which represents the firefox profile.
+class FirefoxProfile:
+    """An instance which represents the firefox profile.
 
-        .. warning::
-            Before making changes to a profile, it is recommend
-            to clone the profile at first or creating a new one.
+    .. warning::
+        Before making changes to a profile, it is recommend
+        to clone the profile at first or creating a new one.
     """
 
     def __init__(self, name: str, is_relative: bool, path: Path | str):
         self.name = name
         self.is_relative = is_relative
         self.path = Path(path)
         self.__config_path = str(self.path.joinpath("prefs.js"))
 
     def list_config(self) -> Dict[str, str]:
-        """ Lists all configurations of the profile.
+        """Lists all configurations of the profile.
 
         Returns:
             Dict[str, str]: A dict with setting pairs.
         """
         # https://stackoverflow.com/questions/24548306/how-to-read-firefoxs-aboutconfig-entries-using-python
         entries = {}
         with open(self.__config_path, encoding="utf-8") as f:
@@ -41,20 +43,20 @@
                 if not m:
                     continue
                 key, value = m.group(2), m.group(3)
                 try:
                     entries[key] = json.loads(value)
                 except Exception as ex:
                     elog(
-                        f"failed to parse line '{line}' key:'{key}' value:'{value}' error:'{ex}'")
+                        f"failed to parse line '{line}' key:'{key}' value:'{value}' error:'{ex}'"
+                    )
         return entries
 
     def set_required_configs(self):
-        """ Sets all required settings to be able to use geckordp.
-        """
+        """Sets all required settings to be able to use geckordp."""
 
         # disable crash-recover after 'ungraceful' process termination
         self.set_config("browser.sessionstore.resume_from_crash", False)
         # disable safe-mode after 'ungraceful' process termination
         self.set_config("browser.sessionstore.max_resumed_crashes", 0)
         self.set_config("browser.sessionstore.restore_on_demand", False)
         self.set_config("browser.sessionstore.restore_tabs_lazily", False)
@@ -70,25 +72,23 @@
         self.set_config("devtools.debugger.remote-enabled", True)
         # allow tab isolation (for e.g. separate cookie-jar)
         self.set_config("privacy.userContext.enabled", True)
         # disable autoplay
         self.set_config("media.autoplay.blocking_policy", 2)
         self.set_config("media.autoplay.default", 5)
         # disable what's new
-        self.set_config(
-            "browser.messaging-system.whatsNewPanel.enabled", False)
+        self.set_config("browser.messaging-system.whatsNewPanel.enabled", False)
         self.set_config("browser.startup.homepage_override.mstone", "ignore")
         self.set_config("startup.homepage_override_url", "https://blank.org/")
         self.set_config("startup.homepage_welcome_url", "https://blank.org/")
         # misc
         self.set_config("app.normandy.first_run", False)
         self.set_config("browser.aboutConfig.showWarning", False)
         self.set_config("browser.aboutwelcome.enabled", False)
-        self.set_config(
-            "browser.shell.skipDefaultBrowserCheckOnFirstRun", True)
+        self.set_config("browser.shell.skipDefaultBrowserCheckOnFirstRun", True)
         self.set_config("browser.startup.firstrunSkipsHomepage", True)
         self.set_config("browser.suppress_first_window_animation", True)
         self.set_config("browser.tabs.warnOnClose", False)
         self.set_config("browser.tabs.warnOnCloseOtherTabs", False)
         self.set_config("browser.tabs.warnOnOpen", False)
         self.set_config("browser.warnOnQuit", False)
         self.set_config("datareporting.policy.dataSubmissionEnabled", False)
@@ -98,56 +98,57 @@
         self.set_config("extensions.formautofill.firstTimeUse", False)
         self.set_config("pdfjs.firstRun", True)
         self.set_config("toolkit.telemetry.reportingpolicy.firstRun", False)
         self.set_config("trailhead.firstrun.branches", "nofirstrun-empty")
         self.set_config("trailhead.firstrun.didSeeAboutWelcome", True)
 
     def set_config(self, name: str, value):
-        """ Sets or updates a configuration value by its name.
+        """Sets or updates a configuration value by its name.
 
         Args:
             name (str): The name of setting.
             value ([type]): The value of the setting.
         """
         input_lines = ""
         with open(self.__config_path, "r+", encoding="utf-8") as f:
             input_lines = f.readlines()
 
         # make value json compatible
-        if (isinstance(value, str)):
-            value = f"\"{value}\""
+        if isinstance(value, str):
+            value = f'"{value}"'
         else:
             value = json.dumps(value)
 
         buffer = ""
         config_set = False
         for line in input_lines:
             m = USER_PREF_REGEX.match(line)
             if not m:
                 continue
             key, val = m.group(2), m.group(3)
             try:
-                if (not config_set and key == name):
-                    line = f"user_pref(\"{name}\", {value});\n"
+                if not config_set and key == name:
+                    line = f'user_pref("{name}", {value});\n'
                     config_set = True
                 buffer += line
             except Exception as ex:
                 elog(
-                    f"failed to parse line '{line}' key:'{key}' value:'{val}' error:'{ex}'")
+                    f"failed to parse line '{line}' key:'{key}' value:'{val}' error:'{ex}'"
+                )
                 buffer += line
 
-        if (not config_set):
-            line = f"user_pref(\"{name}\", {value});\n"
+        if not config_set:
+            line = f'user_pref("{name}", {value});\n'
             buffer += line
 
         with open(self.__config_path, "w", encoding="utf-8") as f:
             f.write(buffer)
 
     def get_config(self, name):
-        """ Get a configuration value by its name.
+        """Get a configuration value by its name.
 
         Args:
             name ([type]): The name to retrieve the value from.
 
         Raises:
             JSONDecodeError: If value can not be deserialized.
 
@@ -157,20 +158,20 @@
         with open(self.__config_path, "r+", encoding="utf-8") as f:
             input_lines = f.readlines()
             for line in input_lines:
                 m = USER_PREF_REGEX.match(line)
                 if not m:
                     continue
                 key, val = m.group(2), m.group(3)
-                if (key == name):
+                if key == name:
                     return json.loads(val, strict=False)
         return None
 
     def remove_config(self, name: str) -> bool:
-        """ Removes a setting by its name.
+        """Removes a setting by its name.
 
         Args:
             name (str): The name of the setting to remove.
 
         Returns:
             bool: True: if setting found and removed, False: not found
         """
@@ -181,15 +182,15 @@
         buffer = ""
         found = False
         for line in input_lines:
             m = USER_PREF_REGEX.match(line)
             if not m:
                 continue
             key = m.group(2)
-            if (not found and key == name):
+            if not found and key == name:
                 found = True
                 continue
             buffer += line
 
         with open(self.__config_path, "w", encoding="utf-8") as f:
             f.write(buffer)
         return found
@@ -197,80 +198,80 @@
     def __str__(self) -> str:
         return f"name:{self.name} is_relative:{self.is_relative} path:{str(self.path)}"
 
     def __repr__(self) -> str:
         return str(self)
 
     def __eq__(self, rhs):
-        if (rhs is None):
+        if rhs is None:
             return False
         return self.name == rhs.name and self.path == rhs.path
 
 
-class ProfileManager():
-    """ A manager for firefox profiles.
-        The manager allows to clone, add or remove firefox profiles.
-        Each profile its configuration can be modified with 'FirefoxProfile'.
-
-        .. warning::
-            Before making changes to a profile, it is recommend
-            to clone the profile at first or creating a new one.
+class ProfileManager:
+    """A manager for firefox profiles.
+    The manager allows to clone, add or remove firefox profiles.
+    Each profile its configuration can be modified with 'FirefoxProfile'.
+
+    .. warning::
+        Before making changes to a profile, it is recommend
+        to clone the profile at first or creating a new one.
     """
 
     def __init__(self, override_firefox_path="", override_profiles_path=""):
         # pylint: disable=invalid-name
-        if (override_firefox_path == ""):
+        if override_firefox_path == "":
             override_firefox_path = Firefox.get_binary_path()
-        self.__ARGS = [override_firefox_path,
-                       "-new-window",
-                       "-new-instance",
-                       "-no-remote",
-                       "-no-default-browser-check"
-                       ]
+        self.__ARGS = [
+            override_firefox_path,
+            "-new-window",
+            "-new-instance",
+            "-no-remote",
+            "-no-default-browser-check",
+        ]
 
-        if (override_profiles_path == ""):
+        if override_profiles_path == "":
             self.__profiles_path = Firefox.get_profiles_path()
         else:
-            self.__profiles_path = Path(
-                override_profiles_path).absolute()
+            self.__profiles_path = Path(override_profiles_path).absolute()
 
-        self.__profiles_ini = Path(
-            self.__profiles_path).joinpath("profiles.ini")
+        self.__profiles_ini = Path(self.__profiles_path).joinpath("profiles.ini")
 
-        if (not self.__profiles_path.exists()):
-            raise RuntimeError(
-                f"path '{self.__profiles_path}' doesn't exist")
+        if not self.__profiles_path.exists():
+            raise RuntimeError(f"path '{self.__profiles_path}' doesn't exist")
 
-        if (not self.__profiles_ini.exists()):
+        if not self.__profiles_ini.exists():
             raise RuntimeError(
-                f"'profiles.ini' doesn't exist in path '{self.__profiles_path}'")
+                f"'profiles.ini' doesn't exist in path '{self.__profiles_path}'"
+            )
 
         bk_profiles_ini = self.__profiles_ini.parent.joinpath(
-            self.__profiles_ini.stem + "-bk" + self.__profiles_ini.suffix)
+            self.__profiles_ini.stem + "-bk" + self.__profiles_ini.suffix
+        )
 
-        if (not bk_profiles_ini.exists()):
+        if not bk_profiles_ini.exists():
             try:
                 shutil.copyfile(self.__profiles_ini, bk_profiles_ini)
                 log(f"backup file '{bk_profiles_ini}' created")
             except Exception as ex:
                 exlog(f"copy backup file '{bk_profiles_ini}' failed:\n{ex}")
 
     def create(self, profile_name: str) -> FirefoxProfile | None:
-        """ Creates and initializes a firefox profile with the specified name.
+        """Creates and initializes a firefox profile with the specified name.
 
         Args:
             profile_name (str): The name for the new profile.
 
         Raises:
             RuntimeError: If initialization of profile failed.
 
         Returns:
             FirefoxProfile | None: not None: instance of firefox profile, None: profile already exists
         """
-        if (self.exists(profile_name)):
+        if self.exists(profile_name):
             wlog(f"profile with name '{profile_name}' already exists")
             return None
         args = list(self.__ARGS)
         args.append("-CreateProfile")
         args.append(f"{profile_name}")
         subprocess.check_output(args, shell=False)
         self.__initialize_profile(profile_name)
@@ -278,261 +279,265 @@
         profile = self.get_profile_by_name(profile_name)
 
         # need to sleep til no process is attached to the related files
         sleep(1)
 
         return profile
 
-    def clone(self, source_name: str, dest_name: str, ignore_invalid_files=False) -> FirefoxProfile | None:
-        """ Clones an existing firefox profile with the specified name.
+    def clone(
+        self, source_name: str, dest_name: str, ignore_invalid_files=False
+    ) -> FirefoxProfile | None:
+        """Clones an existing firefox profile with the specified name.
 
         Args:
             source_name (str): The name of the profile to clone from.
             dest_name (str): The name of the new profile.
 
         Raises:
             ValueError: If 'source_name' and 'dest_name' are equal.
             ValueError: If 'source_name' is empty.
             ValueError: If 'dest_name' is empty.
 
         Returns:
             FirefoxProfile | None: not None: instance of firefox profile, None: source doesn't exists or destination already exists
         """
-        if (source_name == dest_name):
+        if source_name == dest_name:
             raise ValueError(
-                f"parameter 'source_name' and 'dest_name' must be different")
+                f"parameter 'source_name' and 'dest_name' must be different"
+            )
 
         # check source profile
-        if (source_name == ""):
+        if source_name == "":
             raise ValueError(f"parameter 'source_name' is empty")
         source_profile = self.get_profile_by_name(source_name)
-        if (not source_profile):
+        if not source_profile:
             elog(f"profile with name '{source_name}' doesn't exist")
             return None
-        if (not source_profile.path.exists()):
+        if not source_profile.path.exists():
             elog(f"profile with path '{source_profile.path}' doesn't exist")
             return None
 
         # check destination profile
-        if (dest_name == ""):
+        if dest_name == "":
             raise ValueError(f"parameter 'dest_name' is empty")
-        if (self.exists(dest_name)):
+        if self.exists(dest_name):
             elog(f"profile with name '{dest_name}' already exists")
             return None
 
         # create empty destination profile
         args = list(self.__ARGS)
         args.append("-CreateProfile")
         args.append(f"{dest_name}")
         subprocess.check_output(args, shell=False)
 
         dest_profile = self.get_profile_by_name(dest_name)
-        if (not dest_profile):
+        if not dest_profile:
             elog(f"profile with name '{dest_name}' doesn't exist")
             return None
 
         # copy contents
         log(f"copy from '{source_profile.path}' to '{dest_profile.path}'")
-        if (dest_profile.path.exists()):
+        if dest_profile.path.exists():
             shutil.rmtree(dest_profile.path)
         try:
             shutil.copytree(
                 source_profile.path,
                 dest_profile.path,
                 ignore_dangling_symlinks=True,
                 symlinks=True,
-                ignore=shutil.ignore_patterns("times.json", "lock", "*.lock", "sessionstore.jsonlz4"))
+                ignore=shutil.ignore_patterns(
+                    "times.json", "lock", "*.lock", "sessionstore.jsonlz4"
+                ),
+            )
         except shutil.Error as ex:
-            if (not ignore_invalid_files):
+            if not ignore_invalid_files:
                 raise shutil.Error from ex
             else:
                 wlog(f"copytree failed, some files could not be copied:\n{ex}")
 
         profile = self.get_profile_by_name(dest_name)
 
         # need to sleep til no process is attached to the related files
         sleep(1)
 
         return profile
 
     def remove(self, profile_name: str) -> bool:
-        """ Removes a firefox profile by its name.
+        """Removes a firefox profile by its name.
 
         Args:
             profile_name (str): The name of the profile to be removed.
 
         Raises:
             ValueError: If 'profile_name' is empty.
             ValueError: If 'profile_name' is 'default-release'.
 
         Returns:
             bool: True: profile found and removed, False: profile not found
         """
-        if (profile_name == ""):
+        if profile_name == "":
             raise ValueError(f"parameter 'profile_name' is empty")
-        if (profile_name == "default-release"):
+        if profile_name == "default-release":
             raise ValueError(f"parameter 'profile_name' is 'default-release'")
         config = configparser.ConfigParser()
         config.optionxform = str  # type: ignore # preserve case
 
         found = False
         with open(str(self.__profiles_ini), "r", encoding="utf-8") as f:
             config.read_file(f)
             sections = config.sections()
             for section in sections:
                 name = config.get(section, "Name", fallback="")
-                is_relative = int(config.get(
-                    section, "IsRelative", fallback="1")) == 1
+                is_relative = int(config.get(section, "IsRelative", fallback="1")) == 1
                 path = config.get(section, "Path", fallback="")
-                if (name != profile_name):
+                if name != profile_name:
                     continue
-                if (path == ""):
+                if path == "":
                     continue
-                if (is_relative):
+                if is_relative:
                     path = self.__profiles_path.joinpath(path)
                 path = Path(path).absolute()
-                if (not path.exists()):
+                if not path.exists():
                     continue
                 log(f"remove path '{path}'")
                 shutil.rmtree(path)
                 log(f"remove section '{section}' with name '{name}'")
                 config.remove_section(section)
                 found = True
                 break
 
-        if (found):
+        if found:
             with open(str(self.__profiles_ini), "w+", encoding="utf-8") as f:
                 log(f"update profiles.ini")
                 config.write(f, space_around_delimiters=False)
                 return True
 
         return False
 
     def list_profiles(self) -> List[FirefoxProfile]:
-        """ List all profiles available by firefox.
+        """List all profiles available by firefox.
 
         Raises:
 
         Returns:
             List[FirefoxProfile]: List of firefox profiles.
         """
         profiles = []
         config = configparser.ConfigParser()
         with open(str(self.__profiles_ini), "r", encoding="utf-8") as f:
             config.read_file(f)
             sections = config.sections()
             for section in sections:
                 name = config.get(section, "Name", fallback="")
-                is_relative = int(config.get(
-                    section, "IsRelative", fallback="1")) == 1
+                is_relative = int(config.get(section, "IsRelative", fallback="1")) == 1
                 path = config.get(section, "Path", fallback="")
-                if (is_relative):
+                if is_relative:
                     path = self.__profiles_path.joinpath(path)
-                profiles.append(
-                    FirefoxProfile(name, is_relative, path))
+                profiles.append(FirefoxProfile(name, is_relative, path))
         return profiles
 
     def exists(self, profile_name: str) -> bool:
-        """ Check whether a profile exists.
+        """Check whether a profile exists.
 
         Args:
             profile_name (str): The profile name to check.
 
         Raises:
 
             ValueError: If 'profile_name' is empty.
 
         Returns:
             bool: True: profile exists, False: profile doesn't exists
         """
-        if (profile_name == ""):
+        if profile_name == "":
             raise ValueError(f"parameter 'profile_name' is empty")
         return self.get_profile_by_name(profile_name) is not None
 
     def get_profile_by_name(self, profile_name: str) -> FirefoxProfile | None:
-        """ Get a profile by its name.
+        """Get a profile by its name.
 
         Args:
             profile_name (str): The name of the profile to retrieve.
 
         Raises:
             ValueError: If 'profile_name' is empty
 
         Returns:
             FirefoxProfile | None: not None: instance of firefox profile, None: not found
         """
-        if (profile_name == ""):
+        if profile_name == "":
             raise ValueError(f"parameter 'profile_name' is empty")
         config = configparser.ConfigParser()
         with open(str(self.__profiles_ini), "r", encoding="utf-8") as f:
             config.read_file(f)
             sections = config.sections()
             for section in sections:
                 name = config.get(section, "Name", fallback="")
-                is_relative = bool(config.get(
-                    section, "IsRelative", fallback=True))
+                is_relative = bool(config.get(section, "IsRelative", fallback=True))
                 path = config.get(section, "Path", fallback="")
-                if (is_relative):
+                if is_relative:
                     path = self.__profiles_path.joinpath(path)
-                if (name == profile_name):
+                if name == profile_name:
                     return FirefoxProfile(name, is_relative, path)
         return None
 
     def get_profile_path(self, profile_name: str) -> Path | None:
-        """ Get the profile path by its name.
+        """Get the profile path by its name.
 
         Args:
             profile_name (str): The name of the profile.
 
         Returns:
             Path | None: The profile path.
         """
         config = configparser.ConfigParser()
         with open(str(self.__profiles_ini), "r", encoding="utf-8") as f:
             config.read_file(f)
             sections = config.sections()
             for section in sections:
                 name = config.get(section, "Name", fallback="")
-                is_relative = int(config.get(
-                    section, "IsRelative", fallback="1")) == 1
+                is_relative = int(config.get(section, "IsRelative", fallback="1")) == 1
                 path = config.get(section, "Path", fallback="")
-                if (name != profile_name):
+                if name != profile_name:
                     continue
-                if (path == ""):
+                if path == "":
                     continue
-                if (is_relative):
+                if is_relative:
                     path = self.__profiles_path.joinpath(path)
                 path = Path(path).absolute()
-                if (not path.exists()):
+                if not path.exists():
                     continue
                 return path
         return None
 
     def __initialize_profile(self, name: str) -> bool:
         # initialize a profile by starting firefox with the specified name
         args = list(self.__ARGS)
         args.append("-headless")
         args.append("-P")
         args.append(f"{name}")
         success = False
         with subprocess.Popen(args, shell=False) as proc:
             dlog("wait for firefox to initialize profile")
             profile_path = self.get_profile_path(name)
-            if (profile_path is None):
+            if profile_path is None:
                 raise RuntimeError("Profile path could not be found.")
-            success = wait_dir_changed(profile_path, ignore_files=[
-                "recovery",
-                "prefs",
-                "xulstore",
-                ".db",
-                "-session-",
-                ".bin",
-                ".json",
-                "-wal",
-            ])
+            success = wait_dir_changed(
+                profile_path,
+                ignore_files=[
+                    "recovery",
+                    "prefs",
+                    "xulstore",
+                    ".db",
+                    "-session-",
+                    ".bin",
+                    ".json",
+                    "-wal",
+                ],
+            )
             if success:
                 dlog("profile initialized")
             else:
                 wlog("profile may not be initialized")
             kill(proc)
             proc.wait(5.0)
         return success
```

## Comparing `geckordp-0.4.53/geckordp/firefox.py` & `geckordp-0.5.0/geckordp/firefox.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,114 +1,120 @@
+import atexit
 import string
 import subprocess
-import atexit
-from threading import Lock
-from typing import List
 from os import path as ospath
-from sys import platform
 from pathlib import Path
+from sys import platform
+from threading import Lock
+from typing import List
+
 from geckordp.utils import kill_by_pid, wait_process_loaded
 
 _MTX = Lock()
 _REGISTERED = False
 _PIDS = []
 
 
 def _kill_instances():
     with _MTX:
         for pid in _PIDS:
             kill_by_pid(pid)
 
 
-class Firefox():
+class Firefox:
 
     @staticmethod
     def get_profiles_path() -> Path:
-        """ Get the path of firefox profiles.
+        """Get the path of firefox profiles.
 
         Raises:
             RuntimeError: If platform is not supported.
             RuntimeError: If "profiles.ini" is not found.
 
         Returns:
             Path: The path of firefox profiles.
         """
-        paths = []
+        paths: List[Path] = []
         if "linux" in platform:
             paths = [
                 Path.home().joinpath(".mozilla/firefox/"),
                 Path.home().joinpath(".mozilla/Firefox/"),
             ]
             for p in paths:
-                if (p.joinpath("profiles.ini").exists()):
+                if p.joinpath("profiles.ini").exists():
                     return p
         elif platform == "darwin":
             # pylint: disable=anomalous-backslash-in-string
             paths = [
                 Path.home().joinpath("Library/Application Support/Firefox/"),
                 Path.home().joinpath("Library/Application\ Support/Firefox/"),
                 Path.home().joinpath("Library/Application Support/Firefox/"),
                 Path.home().joinpath("Library/Mozilla/Firefox/"),
             ]
             for p in paths:
-                if (p.joinpath("profiles.ini").exists()):
+                if p.joinpath("profiles.ini").exists():
                     return p
         elif platform == "win32":
             paths = [
                 Path(ospath.expandvars(r"%APPDATA%\\Mozilla\\Firefox\\")),
             ]
             for p in paths:
-                if (p.joinpath("profiles.ini").exists()):
+                if p.joinpath("profiles.ini").exists():
                     return p
         else:
             raise RuntimeError(f"The platform '{platform}' is not supported")
         raise RuntimeError(
-            f"Could not find firefox profiles for '{platform}' in:\n{paths}")
+            f"Could not find firefox profiles for '{platform}' in:\n{paths}"
+        )
 
     @staticmethod
     def get_binary_path() -> str:
-        """ Get the path of the firefox binary.
+        """Get the path of the firefox binary.
 
         Raises:
             RuntimeError: If platform is not supported.
             RuntimeError: If firefox is not found.
 
         Returns:
             Path: The path of firefox profiles.
         """
         if "linux" in platform:
             return "firefox"
         elif platform == "darwin":
             return "/Applications/Firefox.app/Contents/MacOS/firefox"
         elif platform == "win32":
-            drives = [Path(f"{x}:")
-                      for x in string.ascii_uppercase if Path(f"{x}:").exists()]
+            drives = [
+                Path(f"{x}:") for x in string.ascii_uppercase if Path(f"{x}:").exists()
+            ]
             paths = []
             for d in drives:
                 p = d.joinpath("\\Program Files\\Mozilla Firefox\\firefox.exe")
-                if (not p.exists()):
+                if not p.exists():
                     paths.append(p)
                     continue
                 return str(p)
             raise RuntimeError(
-                f"Could not find firefox binary for '{platform}' in:\n{paths}")
+                f"Could not find firefox binary for '{platform}' in:\n{paths}"
+            )
         else:
             raise RuntimeError(f"The platform '{platform}' is not supported")
 
     @staticmethod
-    def start(url: str,
-              port: int,
-              profile: str,
-              append_args: List[str] | None = None,
-              override_firefox_path="",
-              auto_kill=True,
-              wait=True) -> subprocess.Popen:
-        """ Starts a firefox instance.
+    def start(
+        url: str,
+        port: int,
+        profile: str,
+        append_args: List[str] | None = None,
+        override_firefox_path="",
+        auto_kill=True,
+        wait=True,
+    ) -> subprocess.Popen:
+        """Starts a firefox instance.
 
-            .. note:: 
+            .. note::
                 The profile needs to be once configured with :func:`~geckordp.profile.FirefoxProfile.set_required_configs`.
                 To manually start firefox, this command can be used:
 
                 **firefox -new-instance -no-remote -new-window https://example.com/ -p geckordp --start-debugger-server 6000**
 
         Args:
             url (str): The url for the start page
@@ -118,37 +124,41 @@
             override_firefox_path (str, optional): Overrides the default firefox binary path.
             auto_kill (bool, optional): Enables the termination of firefox if the python process is also terminated.
             wait (bool, optional): Waits for the firefox instance to finish loading.
 
         Returns:
             subprocess.Popen: The process handle.
         """
-        if (override_firefox_path == ""):
+        if override_firefox_path == "":
             override_firefox_path = Firefox.get_binary_path()
 
-        args = [override_firefox_path,
-                "-new-instance",
-                "-no-remote",
-                "-no-default-browser-check",
-                "-new-window", url,
-                "-p", profile,
-                "--start-debugger-server", str(port)
-                ]
+        args = [
+            override_firefox_path,
+            "-new-instance",
+            "-no-remote",
+            "-no-default-browser-check",
+            "-new-window",
+            url,
+            "-p",
+            profile,
+            "--start-debugger-server",
+            str(port),
+        ]
 
-        if (append_args is not None):
+        if append_args is not None:
             for arg in append_args:
                 args.append(arg)
 
         proc = subprocess.Popen(args, shell=False)
-        if (wait):
+        if wait:
             wait_process_loaded(proc.pid)
 
         global _MTX
         global _REGISTERED
         global _PIDS
-        if (auto_kill):
+        if auto_kill:
             with _MTX:
                 _PIDS.append(proc.pid)
-                if (not _REGISTERED):
+                if not _REGISTERED:
                     _REGISTERED = True
                     atexit.register(_kill_instances)
         return proc
```

## Comparing `geckordp-0.4.53/geckordp/rdp_client.py` & `geckordp-0.5.0/geckordp/rdp_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,70 @@
 import asyncio
-import socket
 import base64
-from enum import Enum
-from threading import Thread, Lock, get_ident
-from collections import defaultdict
-import json
 import concurrent.futures
-from typing import Any, Callable, Coroutine, List, Dict, Tuple, cast
+import json
+import socket
+from collections import defaultdict
 from concurrent.futures import Future, ThreadPoolExecutor
+from enum import Enum
+from threading import Lock, Thread, get_ident
+from typing import Any, Callable, Coroutine, Dict, List, Tuple, cast
+
 from jmespath import search as get_nested_value
-from geckordp.settings import GECKORDP
-from geckordp.logger import log, dlog, elog, wlog
-from geckordp.buffers import LinearBuffer
+
 from geckordp.actors.events import Events
+from geckordp.buffers import LinearBuffer
+from geckordp.logger import dlog, elog, log, wlog
+from geckordp.settings import GECKORDP
 from geckordp.utils import ExpireAt
 
 
-class RDPClient():
+class RDPClient:
 
     __ENCODING = "utf-8"
     __READ_JSON_SINGLE_DIGITS = 10
     __READ_BULK_SINGLE_DIGITS = 90
     __MAX_READ_SIZE = 65536
-    __NUMBER_LUT = bytes([0x30, 0x31, 0x32, 0x33, 0x34,
-                          0x35, 0x36, 0x37, 0x38, 0x39])
+    __NUMBER_LUT = bytes([0x30, 0x31, 0x32, 0x33, 0x34, 0x35, 0x36, 0x37, 0x38, 0x39])
 
-    class _HandlerEntry():
+    class _HandlerEntry:
 
-        def __init__(self, handler: Callable[[dict], None] | Coroutine[Any, Any, None], is_async: bool):
+        def __init__(
+            self,
+            handler: Callable[[dict], None] | Coroutine[Any, Any, None],
+            is_async: bool,
+        ):
             self.handler = handler
             self.is_async = is_async
 
-    class _BulkHeader():
+    class _BulkHeader:
 
         def __init__(self, data: str):
             self.data = data.split(" ")
             self.is_valid = False
-            if (len(self.data) != 4):
+            if len(self.data) != 4:
                 return
-            if (self.data[0] != "bulk"):
+            if self.data[0] != "bulk":
                 return
             self.actor_id = self.data[1]
             self.type = self.data[2]
             try:
                 self.size = int(self.data[3].split(":")[0])
             except:
                 return
             self.is_valid = True
 
     def __init__(
-            self,
-            timeout_sec=3.0,
-            max_buffer_size=33554432,
-            executor_workers=3,
-            executor=None):
-        """ Initializes an instance of the remote debug protocol client.
+        self,
+        timeout_sec=3.0,
+        max_buffer_size=33554432,
+        executor_workers=3,
+        executor=None,
+    ):
+        """Initializes an instance of the remote debug protocol client.
 
         Args:
             timeout_sec (int, optional): The timeout for a response in seconds. Defaults to 3.
             max_buffer_size (int, optional): The maximum size of the read buffer.
                                              High values are only required for large data
                                              such as screenshots or raw html. Defaults to ~33mb.
             executor (Any, optional): A custom executor to use with the client.
@@ -71,56 +77,66 @@
         self.__thread_id = 0
         self.__reader = None
         self.__writer = None
         self.__connected = False
         self.__dc_fut = None
         self.__read_task = None
         self.__current_handler = None
-        self.__json_pre_buffer = LinearBuffer(
-            RDPClient.__READ_JSON_SINGLE_DIGITS)
-        self.__bulk_pre_buffer = LinearBuffer(
-            RDPClient.__READ_BULK_SINGLE_DIGITS)
+        self.__json_pre_buffer = LinearBuffer(RDPClient.__READ_JSON_SINGLE_DIGITS)
+        self.__bulk_pre_buffer = LinearBuffer(RDPClient.__READ_BULK_SINGLE_DIGITS)
         self.__read_buffer = LinearBuffer(max_buffer_size)
         self.__header: RDPClient._BulkHeader | None = None
         self.__registered_events = set()
         self.__registered_events_expr = set()
         self.__await_request_fut = Future()
         self.__await_request_id = ""
         if executor is None:
             self.__workers = ThreadPoolExecutor(executor_workers)
         else:
             self.__workers = executor
 
         self.__event_handlers_mtx = Lock()
-        self.__event_handlers: Dict[str, Dict[str, List[RDPClient._HandlerEntry]]] = defaultdict(
-            lambda: defaultdict(list))
+        self.__event_handlers: Dict[str, Dict[str, List[RDPClient._HandlerEntry]]] = (
+            defaultdict(lambda: defaultdict(list))
+        )
 
         self.__actor_handlers_mtx = Lock()
         self.__actor_handlers: Dict[str, List[RDPClient._HandlerEntry]] = defaultdict(
-            list)
+            list
+        )
+
+        self.__uni_handlers_mtx = Lock()
+        self.__uni_handlers: List[RDPClient._HandlerEntry] = []
+
+        self.__uni_handlers_mtx = Lock()
+        self.__uni_handlers: List[RDPClient._HandlerEntry] = []
 
         self.__register_events()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.disconnect()
 
     @property
     def timeout_sec(self) -> float:
-        """ Returns the timeout in seconds.
+        """Returns the timeout in seconds.
 
         Returns:
             float: The timeout.
         """
         return self.__timeout_sec
 
-    def add_actor_listener(self, actor_id: str, handler: Callable[[dict], None] | Any) -> bool:
-        """ Appends a listener for a specific actor.
+    def add_actor_listener(
+        self,
+        actor_id: str,
+        handler: Callable[[dict], None] | Any,
+    ) -> bool:
+        """Appends a listener for a specific actor.
         Multiple handlers can be added for each event type.
 
         .. warning::
             Called functions within manually registered **async** handlers on RDPClient
             can not call functions which emits :func:`~geckordp.rdp_client.RDPClient.send_receive` later in its execution path
             (instead use non-async handlers in this case)
 
@@ -132,43 +148,57 @@
 
         Returns:
             bool: True: Handler registered; False: Handler already registered
         """
         with self.__actor_handlers_mtx:
             return self.__add_actor_listener(actor_id, handler)
 
-    def __add_actor_listener(self, actor_id: str, handler: Callable[[dict], None]) -> bool:
+    def __add_actor_listener(
+        self,
+        actor_id: str,
+        handler: Callable[[dict], None],
+    ) -> bool:
         handler_entries = self.__actor_handlers[actor_id]
         for handler_entry in handler_entries:
-            if (handler_entry.handler == handler):
+            if handler_entry.handler == handler:
                 return False
         handler_entries.append(
-            RDPClient._HandlerEntry(handler, asyncio.iscoroutinefunction(handler)))
+            RDPClient._HandlerEntry(handler, asyncio.iscoroutinefunction(handler))
+        )
         return True
 
-    def remove_actor_listener(self, actor_id: str, handler: Callable[[dict], None] | Any):
-        """ Removes a listener with the specified actor ID.
+    def remove_actor_listener(
+        self,
+        actor_id: str,
+        handler: Callable[[dict], None] | Any,
+    ):
+        """Removes a listener with the specified actor ID.
 
         Args:
             actor_id (str): The ID to find.
             handler (Callable[[dict], None]): The handler to remove.
         """
         with self.__actor_handlers_mtx:
             self.__remove_actor_listener(actor_id, handler)
 
     def __remove_actor_listener(self, actor_id: str, handler):
-        if (not actor_id in self.__actor_handlers):
+        if not actor_id in self.__actor_handlers:
             return
         for entry in self.__actor_handlers[actor_id]:
-            if (entry.handler == handler):
+            if entry.handler == handler:
                 self.__actor_handlers[actor_id].remove(entry)
                 return
 
-    def add_event_listener(self, actor_id: str, event: str | Events, handler: Callable[[dict], None] | Any) -> bool:
-        """ Appends a listener for a specific actor and event.
+    def add_event_listener(
+        self,
+        actor_id: str,
+        event: str | Events,
+        handler: Callable[[dict], None] | Any,
+    ) -> bool:
+        """Appends a listener for a specific actor and event.
         Multiple handlers can be added for each event type.
 
         .. warning::
             Called functions within manually registered **async** handlers on RDPClient
             can not call functions which emits :func:`~geckordp.rdp_client.RDPClient.send_receive` later in its execution path
             (instead use non-async handlers in this case)
 
@@ -179,129 +209,166 @@
                                               Can be either async (executed with coroutine)
                                               or a common function (queued to executor).
 
         Returns:
             bool: True: Handler registered; False: Handler already registered
         """
         with self.__event_handlers_mtx:
-            return self.__add_event_listener(actor_id, event, handler)
-
-    def __add_event_listener(self, actor_id: str, event: str | Events, handler: Callable[[dict], None] | Any) -> bool:
-        event_name: str = cast(str, event)
-        if (isinstance(event, Enum)):
-            event_name = event.value
-
-        handler_entries = self.__event_handlers[event_name][actor_id]
-        for handler_entry in handler_entries:
-            if (handler_entry.handler == handler):
-                return False
-
-        handler_entries.append(
-            RDPClient._HandlerEntry(handler, asyncio.iscoroutinefunction(handler)))
-        if (GECKORDP.DEBUG_EVENTS):
-            self.__print_event_handlers("__add_event_listener")
-        return True
+            event_name: str = cast(str, event)
+            if isinstance(event, Enum):
+                event_name = event.value
+
+            handler_entries = self.__event_handlers[event_name][actor_id]
+            for handler_entry in handler_entries:
+                if handler_entry.handler == handler:
+                    return False
+
+            handler_entries.append(
+                RDPClient._HandlerEntry(handler, asyncio.iscoroutinefunction(handler))
+            )
+            if GECKORDP.DEBUG_EVENTS:
+                self.__print_event_handlers("add_event_listener")
+            return True
 
-    def remove_event_listener(self, actor_id: str, event, handler: Callable[[dict], None] | Any):
-        """ Removes a listener with the specified actor ID and event.
+    def remove_event_listener(
+        self,
+        actor_id: str,
+        event,
+        handler: Callable[[dict], None] | Any,
+    ):
+        """Removes a listener with the specified actor ID and event.
 
         Args:
             actor_id (str): The actor ID.
             event_type (Enum/str): The event type. See /actors/events.py
             handler (Callable[[dict], None]): The handler to remove.
         """
         with self.__event_handlers_mtx:
-            self.__remove_event_listener(actor_id, event, handler)
+            event_name: str = cast(str, event)
+            if isinstance(event, Enum):
+                event_name = event.value
 
-    def __remove_event_listener(self, actor_id: str, event: str | Events, handler: Callable[[dict], None]):
-        event_name: str = cast(str, event)
-        if (isinstance(event, Enum)):
-            event_name = event.value
-
-        actors = self.__event_handlers.get(event_name, None)
-        if (actors is None):
-            return
+            actors = self.__event_handlers.get(event_name, None)
+            if actors is None:
+                return
 
-        handler_entries = actors.get(actor_id, None)
-        if (handler_entries is None):
-            return
+            handler_entries = actors.get(actor_id, None)
+            if handler_entries is None:
+                return
 
-        for entry in handler_entries:
-            if (entry.handler == handler):
-                handler_entries.remove(entry)
-                break
+            for entry in handler_entries:
+                if entry.handler == handler:
+                    handler_entries.remove(entry)
+                    break
 
-        if (len(handler_entries) == 0):
-            actors.pop(actor_id, None)
+            if len(handler_entries) == 0:
+                actors.pop(actor_id, None)
 
-        if (GECKORDP.DEBUG_EVENTS):
-            self.__print_event_handlers("__remove_event_listener")
+            if GECKORDP.DEBUG_EVENTS:
+                self.__print_event_handlers("remove_event_listener")
 
     def remove_event_listeners_by_id(self, actor_id: str):
-        """ Removes all callback handlers by actor ID.
+        """Removes all callback handlers by actor ID.
 
         Args:
             actor_id (str): The actor ID.
         """
         with self.__event_handlers_mtx:
             for _event_name, handler_entries in self.__event_handlers.items():
                 try:
                     handler_entries.pop(actor_id, None)
                     dlog(f"actor '{actor_id}' removed with its handlers")
                 except KeyError:
                     pass
-            if (GECKORDP.DEBUG_EVENTS):
+            if GECKORDP.DEBUG_EVENTS:
                 self.__print_event_handlers("remove_event_listeners_by_id")
 
+    def add_universal_listener(self, handler: Callable[[dict], None] | Any) -> bool:
+        """Appends a universal listener.
+
+        .. warning::
+            Called functions within manually registered **async** handlers on RDPClient
+            can not call functions which emits :func:`~geckordp.rdp_client.RDPClient.send_receive` later in its execution path
+            (instead use non-async handlers in this case)
+
+        Args:
+            handler (Callable[[dict], None]): The handler to call on match.
+                                              Can be either async (executed with coroutine)
+                                              or a common function (queued to executor).
+
+        Returns:
+            bool: True: Handler registered; False: Handler already registered
+        """
+        with self.__uni_handlers_mtx:
+            for entry in self.__uni_handlers:
+                if entry.handler == handler:
+                    return False
+            self.__uni_handlers.append(
+                RDPClient._HandlerEntry(handler, asyncio.iscoroutinefunction(handler))
+            )
+            return True
+
+    def remove_universal_listener(self, handler: Callable[[dict], None] | Any):
+        """Removes a universal listener.
+
+        Args:
+            actor_id (str): The ID to find.
+            handler (Callable[[dict], None]): The handler to remove.
+        """
+        with self.__uni_handlers_mtx:
+            for entry in self.__uni_handlers:
+                if entry.handler == handler:
+                    self.__uni_handlers.remove(entry)
+                    return
+
     def connected(self) -> bool:
-        """ Check whether the client is currently connected to the server.
+        """Check whether the client is currently connected to the server.
 
         Returns:
             bool: True: Connected; False: Disconnected
         """
         with self.__mtx:
             return self.__connected
 
     def connect(self, host: str, port: int) -> dict | None:
-        """ Connects to the firefox debug server.
+        """Connects to the firefox debug server.
 
         Args:
             host (str): The host to connect to, usually 'localhost'
             port (int): The port to use, default '6000'
 
         Returns:
             dict | None: The server response on successful established connection.
         """
         with self.__mtx:
-            if (self.__connected):
+            if self.__connected:
                 return None
             dlog("")
             self.__await_request_id = "root"
             self.__await_request_fut = Future()
-            self.__loop_thread = Thread(
-                target=self.__connect, args=[host, port])
+            self.__loop_thread = Thread(target=self.__connect, args=[host, port])
             self.__loop_thread.start()
             try:
                 return self.__await_request_fut.result(self.__timeout_sec)
             except:
                 dlog("Timeout")
-                if (len(asyncio.all_tasks(self.__loop)) > 0):
+                if len(asyncio.all_tasks(self.__loop)) > 0:
                     dlog("Cancel read")
                     self.__loop.call_soon_threadsafe(
-                        asyncio.ensure_future, self.__disconnect())
+                        asyncio.ensure_future, self.__disconnect()
+                    )
             return None
 
     def __connect(self, host: str, port: int):
         # pylint: disable=no-member
-        if (self.__loop.is_running()):
+        if self.__loop.is_running():
             log("Queue is already running")
             return
         dlog("Queue read task")
-        self.__read_task = self.__loop.create_task(
-            self.__open_connection(host, port))
+        self.__read_task = self.__loop.create_task(self.__open_connection(host, port))
         self.__read_task.add_done_callback(self.__on_close_connection)
         try:
             dlog("Run IO loop")
             self.__loop.run_until_complete(self.__read_task)
         except socket.gaierror as e:
             elog(f"{e}")
         except concurrent.futures._base.CancelledError:
@@ -309,21 +376,23 @@
         except asyncio.exceptions.CancelledError:
             dlog("Read task cancelled: asyncio")
 
     async def __open_connection(self, host: str, port: int):
         dlog("Try to open connection")
         try:
             self.__reader = asyncio.StreamReader(
-                limit=RDPClient.__MAX_READ_SIZE, loop=self.__loop)
-            protocol = asyncio.StreamReaderProtocol(
-                self.__reader, loop=self.__loop)
+                limit=RDPClient.__MAX_READ_SIZE, loop=self.__loop
+            )
+            protocol = asyncio.StreamReaderProtocol(self.__reader, loop=self.__loop)
             transport, _ = await self.__loop.create_connection(
-                lambda: protocol, host, port)  # type: ignore
+                lambda: protocol, host, port
+            )  # type: ignore
             self.__writer = asyncio.StreamWriter(
-                transport, protocol, self.__reader, self.__loop)  # type: ignore
+                transport, protocol, self.__reader, self.__loop
+            )  # type: ignore
         except ConnectionRefusedError as e:
             elog(e)
             return
         dlog("Start listening")
         self.__connected = True
         self.__thread_id = get_ident()
         await self.__read_loop()
@@ -333,445 +402,470 @@
             dlog("Stop listening")
             self.__connected = False
             self.__dc_fut.set_result(1)
         except:
             pass
 
     def disconnect(self):
-        """ Disconnects from the debug server.
-        """
+        """Disconnects from the debug server."""
         with self.__mtx:
-            if (not self.__connected):
+            if not self.__connected:
                 return
             dlog("")
             self.__dc_fut = Future()
-            self.__loop.call_soon_threadsafe(
-                asyncio.ensure_future, self.__disconnect())
+            self.__loop.call_soon_threadsafe(asyncio.ensure_future, self.__disconnect())
             try:
                 self.__dc_fut.result(0.2)
             except:
                 dlog("Timeout")
 
     async def __disconnect(self):
         dlog(self.__connected)
         self.__read_task.cancel()
 
     def send(self, msg: dict) -> Coroutine | bool:
-        """ Starts sending a request without waiting for a response.
+        """Starts sending a request without waiting for a response.
             The dict message will be transformed to a utf-8 json string.
 
         Args:
             msg (dict): The message to send.
 
         Raises:
             ValueError: If parameter 'msg' doesn't contain key 'to'.
 
         Returns:
             Coroutine | bool: Return type depends on handler type (asnyc).
         """
         with self.__mtx:
-            if (not self.__connected):
+            if not self.__connected:
                 elog(f"Not connected on request:\n{msg}")
                 return False
             dlog("")
-            if (not "to" in msg):
+            if not "to" in msg:
                 raise ValueError("parameter 'msg' must contain 'to' field")
-            if (get_ident() == self.__thread_id):
+            if get_ident() == self.__thread_id:
                 return self.__async_send(msg)
             return self.__sync_send(msg)
 
     async def __async_send(self, msg: dict) -> dict | None:
         dlog("")
         return await self.__send(msg)
 
     def __sync_send(self, msg: dict) -> bool:
         dlog("")
-        self.__loop.call_soon_threadsafe(
-            asyncio.ensure_future, self.__send(msg))
+        self.__loop.call_soon_threadsafe(asyncio.ensure_future, self.__send(msg))
         return True
 
     def send_receive(self, msg: dict, extract_expression="") -> dict:
-        """ Starts sending a request and waiting for a response.
+        """Starts sending a request and waiting for a response.
             The dictionary message will be transformed to a utf-8 json string.
             The timeout can be specified in the class its constructor.
 
+        .. note::
+            Receiving messages asynchronously is not possible since the remote debug protocol is sequential itself
+            and doesn't have a way to identify individual received packets by an ID (which the sender would transmit).
+
         Args:
             msg (dict): The message to send.
             extract_expression (str, optional): A jmespath expression to extract data from the response. Defaults to "".
 
         Raises:
             ValueError: If 'msg' parameter doesn't contain field 'to'
 
         Returns:
             Coroutine | dict | None: The response from the server.
         """
         with self.__mtx:
-            if (not self.__connected):
+            if not self.__connected:
                 elog(f"Not connected on request:\n{msg}")
                 return cast(dict, None)
-            if (not "to" in msg):
+            if not "to" in msg:
                 raise ValueError("parameter 'msg' must contain 'to' field")
             # check whether this function was called in loop thread context and directly call
             # the required functions without queue
-            if (get_ident() == self.__thread_id):
+            if get_ident() == self.__thread_id:
                 return cast(dict, self.__async_send_receive(msg, extract_expression))
             # otherwise run the sync version to queue the 'send' function call
             # and wait for the result from the server
             return cast(dict, self.__sync_send_receive(msg, extract_expression))
 
     async def __async_send_receive(self, msg: dict, extract_expression: str):
         dlog("")
         fut = Future()
         await self.__send(msg, fut)
 
         # read in loop to allow other messages to pass
         exp = ExpireAt(self.__timeout_sec)
         while exp:
             timeout_sec = self.__timeout_sec - exp.expired_time()
-            if (timeout_sec <= 0):
+            if timeout_sec <= 0:
                 break
             try:
                 await asyncio.wait_for(
-                    self.__loop.create_task(self.__read(False)),
-                    timeout_sec)
+                    self.__loop.create_task(self.__read(False)), timeout_sec
+                )
             except:
                 break
-            if (fut.done()):
+            if fut.done():
                 break
 
         # get response
-        if (fut.done()):
+        if fut.done():
             try:
                 response = fut.result(0)
-                if ("error" in response):
-                    elog(
-                        f"Error on request:\n{msg}\n{json.dumps(response, indent=2)}")
-                if (extract_expression == ""):
+                if "error" in response:
+                    elog(f"Error on request:\n{msg}\n{json.dumps(response, indent=2)}")
+                if extract_expression == "":
                     return response
                 extracted = get_nested_value(extract_expression, response)
-                if (extracted is None):
+                if extracted is None:
                     return response
                 return extracted
             except:
                 elog(f"No response on request:\n{msg}")
                 return None
         else:
             elog(f"Timeout on request:\n{msg}")
             return None
 
     def __sync_send_receive(self, msg: dict, extract_expression: str) -> dict | None:
         dlog("")
         fut = Future()
-        self.__loop.call_soon_threadsafe(
-            asyncio.ensure_future, self.__send(msg, fut))
+        self.__loop.call_soon_threadsafe(asyncio.ensure_future, self.__send(msg, fut))
         try:
-            response = fut.result(
-                self.__timeout_sec)
-            if ("error" in response):
-                elog(
-                    f"Error on request:\n{msg}\n{json.dumps(response, indent=2)}")
-            if (extract_expression == ""):
+            response = fut.result(self.__timeout_sec)
+            if "error" in response:
+                elog(f"Error on request:\n{msg}\n{json.dumps(response, indent=2)}")
+            if extract_expression == "":
                 return response
             extracted = get_nested_value(extract_expression, response)
-            if (extracted is None):
+            if extracted is None:
                 return response
             return extracted  # type: ignore
         except:
             elog(f"Timeout on request:\n{msg}")
             return None
 
     async def __send(self, msg: dict, fut: Future | None = None):
         self.__await_request_id = msg["to"]
-        if (fut is not None):
+        if fut is not None:
             self.__await_request_fut = fut
 
-        json_msg = json.dumps(msg, separators=(',', ':'))
+        json_msg = json.dumps(msg, separators=(",", ":"))
 
-        if (GECKORDP.DEBUG_REQUEST):
-            if (GECKORDP.DEBUG_REQUEST_FORMAT):
+        if GECKORDP.DEBUG_REQUEST:
+            if GECKORDP.DEBUG_REQUEST_FORMAT:
                 log(f"REQUEST->\n{json.dumps(msg, indent=2)}")
             else:
                 log(f"REQUEST->\n{len(json_msg)}:{json_msg}")
 
         self.__writer.write(
-            bytes(f"{len(json_msg)}:{json_msg}", encoding=RDPClient.__ENCODING))
+            bytes(f"{len(json_msg)}:{json_msg}", encoding=RDPClient.__ENCODING)
+        )
         await self.__writer.drain()
 
     async def __read_loop(self):
         while True:
-            if (not await self.__read(True)):
+            if not await self.__read(True):
                 break
 
     async def __read(self, lock: bool):
         # read a few single digits to get the actual size of the response:
         # at the beginning of every json server message there is a size indicator
         # it does look like this:
         # 196:{"x":"y"}
         payload_size = 0
         self.__json_pre_buffer.clear()
         self.__bulk_pre_buffer.clear()
         for _ in range(0, RDPClient.__READ_JSON_SINGLE_DIGITS):
             # read just a byte, this will "block" until a message arrives
-            byte = (await self.__reader.read(1))
-            if (len(byte) <= 0):
-                elog(
-                    f"No bytes read, connection is probably closed")
+            byte = await self.__reader.read(1)
+            if len(byte) <= 0:
+                elog(f"No bytes read, connection is probably closed")
                 return False
             byte = byte[0]
             self.__bulk_pre_buffer.append_byte(byte)
             # if byte is a digit, store it for later usage
-            if (self.__is_numeric(byte)):
+            if self.__is_numeric(byte):
                 self.__json_pre_buffer.append_byte(byte)
                 continue
             # if byte is a colon, the payload size string is finished
-            if (byte == 0x3a):  # ":"
+            if byte == 0x3A:  # ":"
                 self.__json_pre_buffer.append_byte(byte)
-                payload_size = int(self.__json_pre_buffer.get(
-                ).tobytes().decode(encoding="utf-8").split(':', 1)[0])
+                payload_size = int(
+                    self.__json_pre_buffer.get()
+                    .tobytes()
+                    .decode(encoding="utf-8")
+                    .split(":", 1)[0]
+                )
                 break
             # if execution flow arrives here, it means there's no size indicator
             # and the message probably may have a very large size
-            read_size_str = self.__json_pre_buffer.get(
-            ).tobytes().decode(encoding="utf-8")
+            read_size_str = (
+                self.__json_pre_buffer.get().tobytes().decode(encoding="utf-8")
+            )
             dlog(
-                f"probably invalid json size indicator starts with utf-8='{read_size_str}'")
+                f"probably invalid json size indicator starts with utf-8='{read_size_str}'"
+            )
             break
 
         # after a few single digits are read, and no size indicator was found,
         # check whether the received data is a bulk packet:
         # bulk server1.conn0.heapSnapshotFileActor5 heap-snapshot 34095:
         is_bulk = False
-        if (payload_size == 0):
+        if payload_size == 0:
 
             # check for bulk header if data starts with 'b' = 0x62 character
-            if (self.__bulk_pre_buffer.get(
-            ).tobytes().startswith(bytes([0x62]))):
+            if self.__bulk_pre_buffer.get().tobytes().startswith(bytes([0x62])):
                 dlog("possible bulk header found")
                 self.__header = None
                 for _ in range(0, RDPClient.__READ_BULK_SINGLE_DIGITS):
-                    byte = (await self.__reader.read(1))
+                    byte = await self.__reader.read(1)
                     byte = byte[0]
                     self.__bulk_pre_buffer.append_byte(byte)
                     # if byte is a colon, the payload size string is finished
-                    if (byte == 0x3a):  # ":"
+                    if byte == 0x3A:  # ":"
                         dlog("header read")
-                        header_data = self.__bulk_pre_buffer.get(
-                        ).tobytes().decode(encoding="utf-8", errors="ignore")
+                        header_data = (
+                            self.__bulk_pre_buffer.get()
+                            .tobytes()
+                            .decode(encoding="utf-8", errors="ignore")
+                        )
                         self.__header = RDPClient._BulkHeader(header_data)
                         break
 
-                if (self.__header is not None and self.__header.is_valid):
+                if self.__header is not None and self.__header.is_valid:
                     dlog(f"header valid: {self.__header.size}")
                     payload_size = self.__header.size
                     is_bulk = True
 
-            if (payload_size == 0):
-                elog(
-                    f"could not read size indicator, probably too large")
+            if payload_size == 0:
+                elog(f"could not read size indicator, probably too large")
                 return False
 
         # after a part of the payload was received, read the remaining message
         bytes_read = 0
         self.__read_buffer.reset()
         while bytes_read < payload_size:
 
             # truncate read size, else it will leak into the next message
             trunc_read_size = payload_size - bytes_read
             # the passed max limit to streamreader doesn't seem to take effect here
-            if (trunc_read_size > RDPClient.__MAX_READ_SIZE):
+            if trunc_read_size > RDPClient.__MAX_READ_SIZE:
                 trunc_read_size = RDPClient.__MAX_READ_SIZE
 
-            read_bytes = (await self.__reader.read(trunc_read_size))
+            read_bytes = await self.__reader.read(trunc_read_size)
             read_bytes_size = len(read_bytes)
-            if (read_bytes_size == 0):
+            if read_bytes_size == 0:
                 elog(f"EOF remote host probably closed")
                 return False
 
             bytes_read += read_bytes_size
-            if (not self.__read_buffer.append(read_bytes)):
+            if not self.__read_buffer.append(read_bytes):
                 elog(
                     f"""
                     buffer overflow while appending response: buffer is too small\n
                     buffer:{self.__read_buffer.size()}\nresponse:{read_bytes_size}
-                    """)
+                    """
+                )
                 return False
 
-            if (bytes_read < payload_size):
+            if bytes_read < payload_size:
                 dlog(f"read more data ({bytes_read} < {payload_size})")
-            elif (bytes_read == payload_size):
+            elif bytes_read == payload_size:
                 dlog(f"message complete ({bytes_read} == {payload_size})")
-            elif (bytes_read > payload_size):
+            elif bytes_read > payload_size:
                 dlog(f"message corrupted ({bytes_read} > {payload_size})")
 
         # add null termination else 'get_null_terminated()' won't work correctly
-        if (not self.__read_buffer.append_byte(0x00)):
+        if not self.__read_buffer.append_byte(0x00):
             elog(f"buffer overflow while appending null termination")
             return False
 
         # handle message by type
         response = None
         from_actor = ""
         valid = False
-        if (is_bulk):
-            response, from_actor, valid = self.__handle_bulk_response(
-                payload_size)
+        if is_bulk:
+            response, from_actor, valid = self.__handle_bulk_response(payload_size)
         else:
             response, from_actor, valid = self.__handle_json_response()
-        if (not valid):
+        if not valid:
             return True
 
+        await self.__handle_universal_listeners(response, lock)
+
         # handle actor handlers
         await self.__handle_actors(response, from_actor, lock)
 
         # check if listener event
-        if (await self.__handle_events(response, from_actor, lock)):
+        if await self.__handle_events(response, from_actor, lock):
             return True
 
         # handle single request
         self.__handle_single_request(response, from_actor)
 
         return True
 
     def __handle_json_response(self) -> Tuple[dict | None, str, bool]:
         # get string representation of bytes
         json_response = ""
         try:
-            json_response = self.__read_buffer.get_null_terminated(
-            ).tobytes().decode(encoding="utf-8")
+            json_response = (
+                self.__read_buffer.get_null_terminated()
+                .tobytes()
+                .decode(encoding="utf-8")
+            )
         except Exception as ex:
             elog(f"could not load response as decoded utf-8 string:\n{ex}")
             return None, "", False
 
         # load json string to dictionary
         response = None
         try:
             response = json.loads(json_response, strict=False)
         except:
-            elog(
-                f"couldn't load json response as dictionary:\n'{json_response}'")
+            elog(f"couldn't load json response as dictionary:\n'{json_response}'")
             return response, "", False
         self.__print_response(response)
 
         # check required response fields
         from_actor = response.get("from", None)
-        if (not from_actor):
+        if not from_actor:
             elog(
-                f"'from' field doesn't exist in response:\n{json.dumps(response, indent=2)}")
+                f"'from' field doesn't exist in response:\n{json.dumps(response, indent=2)}"
+            )
             return response, from_actor, False
 
         return response, from_actor, True
 
     def __handle_bulk_response(self, payload_size: int) -> Tuple[dict, str, bool]:
         response = {}
         response["type"] = self.__header.type
         # encoding might not be really required since it will be decoded back again anyway,
         # however the returned data will be consistent with the other similar messages
         # received from the server
         response["data"] = base64.b64encode(
-            self.__read_buffer.get_truncated(payload_size).tobytes()).decode("ascii")
+            self.__read_buffer.get_truncated(payload_size).tobytes()
+        ).decode("ascii")
         response["data-size"] = len(response["data"])
         response["data-decoded-size"] = payload_size
         response["data-encoding"] = "base64"
         response["from"] = self.__header.actor_id
         self.__print_response(response)
         return response, self.__header.actor_id, True
 
+    async def __handle_universal_listeners(self, response: dict | None, lock: bool):
+        if lock:
+            self.__uni_handlers_mtx.acquire()
+        try:
+            await self.__process_callback_handlers(response, self.__uni_handlers)
+        finally:
+            if lock:
+                self.__uni_handlers_mtx.release()
+
     async def __handle_actors(self, response: dict | None, from_actor: str, lock: bool):
-        if (lock):
+        if lock:
             self.__actor_handlers_mtx.acquire()
         try:
             entries = self.__actor_handlers.get(from_actor, None)
-            if (entries is None):
+            if entries is None:
                 return
             await self.__process_callback_handlers(response, entries)
         finally:
-            if (lock):
+            if lock:
                 self.__actor_handlers_mtx.release()
 
     async def __handle_events(self, response: dict | None, from_actor: str, lock: bool):
         event_type = response.get("type", None)
-        if (event_type is None):
+        if event_type is None:
             return False
-        if (GECKORDP.DEBUG_EVENTS):
+        if GECKORDP.DEBUG_EVENTS:
             log(f"EVENT:\n{json.dumps(response, indent=2)}")
-        if (lock):
+        if lock:
             self.__event_handlers_mtx.acquire()
         try:
             actors = self.__event_handlers.get(event_type, None)
-            if (actors):
+            if actors:
                 entries = actors.get(from_actor, None)
-                if (entries):
+                if entries:
                     await self.__process_callback_handlers(response, entries)
                     dlog(f"[{from_actor}][{event_type}] handled")
                 return True
         finally:
-            if (lock):
+            if lock:
                 self.__event_handlers_mtx.release()
 
-        if (event_type in self.__registered_events):
+        if event_type in self.__registered_events:
             dlog(f"unhandled event received")
             return True
 
         for expr in self.__registered_events_expr:
-            if (get_nested_value(expr, response) is not None):
+            if get_nested_value(expr, response) is not None:
                 dlog(f"unhandled event expression received")
                 return True
 
         return False
 
-    async def __process_callback_handlers(self, response: dict | None, entries: List[_HandlerEntry]):
+    async def __process_callback_handlers(
+        self,
+        response: dict | None,
+        entries: List[_HandlerEntry],
+    ):
         for entry in entries:
-            if (entry.handler is None):
+            if entry.handler is None:
                 continue
-            if (entry.is_async):
-                if (self.__current_handler is not None):
+            if entry.is_async:
+                if self.__current_handler is not None:
                     dlog("break recursion")
                     continue
                 self.__current_handler = entry.handler
                 await entry.handler(response)  # type: ignore
                 self.__current_handler = None
             else:
                 try:
                     self.__loop.run_in_executor(
-                        self.__workers, entry.handler, response)  # type: ignore
+                        self.__workers, entry.handler, response
+                    )  # type: ignore
                 except RuntimeError as ex:
                     # This happens with the 'ThreadPoolExecutor' class
                     # it is known that it will shutdown itself before everything else
                     # and causes this behavior
                     wlog(f"Cannot queue task: {ex}")
 
     def __handle_single_request(self, response: dict | None, from_actor: str):
-        if (self.__await_request_fut is None or from_actor != self.__await_request_id):
+        if self.__await_request_fut is None or from_actor != self.__await_request_id:
             return
         try:
             dlog("response valid, set result")
             self.__await_request_fut.set_result(response)
         except:
             pass
 
     def __register_events(self):
         for name, value in Events.__dict__.items():
-            if ("enum" in str(value)):
+            if "enum" in str(value):
                 event_type = getattr(Events, name)
                 for event in event_type:
-                    if ("$EXPR:" in event.value):
+                    if "$EXPR:" in event.value:
                         self.__registered_events_expr.add(
-                            event.value.replace("$EXPR:", ""))
+                            event.value.replace("$EXPR:", "")
+                        )
                     else:
                         self.__registered_events.add(event.value)
 
     def __is_numeric(self, byte):
         return byte in RDPClient.__NUMBER_LUT
 
     def __print_event_handlers(self, name: str):
         log(f"____________________________{name}")
         for event_name, handler_entries in self.__event_handlers.items():
             log(f"event:{event_name}:")
             for actor, handler in handler_entries.items():
                 log(f"\tactor:{actor} handlers:{len(handler)}")
 
     def __print_response(self, response: dict):
-        if (GECKORDP.DEBUG_RESPONSE):
-            if (GECKORDP.DEBUG_RESPONSE_FORMAT):
+        if GECKORDP.DEBUG_RESPONSE:
+            if GECKORDP.DEBUG_RESPONSE_FORMAT:
                 log(f"RESPONSE<-\n{json.dumps(response, indent=2)}")
             else:
                 log(f"RESPONSE<-\n{response}")
```

## Comparing `geckordp-0.4.53/geckordp/actors/screenshot.py` & `geckordp-0.5.0/geckordp/actors/screenshot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 from geckordp.actors.actor import Actor
 
 
 class ScreenshotActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/screenshot.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/screenshot.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def capture(self,
-                browsing_context_id: int,
-                fullpage=True,
-                file=False,
-                copy_clipboard=False,
-                selector="",
-                dpr=2,
-                delay_sec=0,
-                snapshot_scale=1,
-                left: int | None = None,
-                top: int | None = None,
-                width: int | None = None,
-                height: int | None = None):
+    def capture(
+        self,
+        browsing_context_id: int,
+        fullpage=True,
+        file=False,
+        copy_clipboard=False,
+        selector="",
+        dpr=2,
+        delay_sec=0,
+        snapshot_scale=1,
+        left: int | None = None,
+        top: int | None = None,
+        width: int | None = None,
+        height: int | None = None,
+    ):
         args = {
             "fullpage": fullpage,
             "file": file,
             "clipboard": copy_clipboard,
             "selector": selector,
             "dpr": str(dpr),
             "delay": str(delay_sec),
             "snapshotScale": snapshot_scale,
             "browsingContextID": browsing_context_id,
         }
-        if (left and top and width and height):
-            args["rect"] = {
-                "left": left,
-                "top": top,
-                "width": width,
-                "height": height
+        if left and top and width and height:
+            args["rect"] = {"left": left, "top": top, "width": width, "height": height}
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "capture",
+                "args": args,
             }
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "capture",
-            "args": args,
-        })
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/node.py` & `geckordp-0.5.0/geckordp/actors/targets/window_global.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,98 @@
-from typing import Any, Dict
 from geckordp.actors.actor import Actor
 
 
-class NodeActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/node.js
+class WindowGlobalActor(Actor):
+    """https://github.com/mozilla/gecko-dev/blob/c07fae4f8a15991f019d70cd7b9900338d72eba2/devtools/shared/specs/targets/browsing-context.js
+    https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/targets/window-global.js
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def get_node_value(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getNodeValue",
-        }, "value")
-
-    def set_node_value(self, value):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setNodeValue",
-            "value": value,
-        })
-
-    def get_unique_selector(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getUniqueSelector",
-        }, "value")
-
-    def get_css_path(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getCssPath",
-        }, "value")
-
-    def get_x_path(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getXPath",
-        }, "value")
-
-    def scroll_into_view(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "scrollIntoView",
-        })
-
-    def get_image_data(self, max_dim=0):
-        args: Dict[str, Any] = {
-            "to": self.actor_id,
-            "type": "getImageData",
-        }
-        if (max_dim > 0):
-            args["maxDim"] = max_dim
-        return self.client.send_receive(args)
-
-    def get_event_listener_info(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getEventListenerInfo",
-        }, "events")
-
-    def modify_attributes(self, modifications: list):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "modifyAttributes",
-            "modifications": modifications,
-        })
-
-    def get_font_family_data_url(self, font: str, fill_style=""):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getFontFamilyDataURL",
-            "font": font,
-            "fillStyle": fill_style,
-        })
-
-    def get_closest_background_color(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getClosestBackgroundColor",
-        }, "value")
-
-    def get_background_color(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getBackgroundColor",
-        }, "value")
-
-    def get_owner_global_dimensions(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getOwnerGlobalDimensions",
-        })
-
-    """ def connect_to_remote_frame(self):
-        # "Spec for 'domnode' specifies a 'connectToRemoteFrame' method that isn't implemented by the actor"
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "connectToRemoteFrame",
-        }) """
-
-    def wait_for_frame_load(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "waitForFrameLoad",
-        })
+    def detach(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "detach",
+            }
+        )
+
+    def focus(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "focus",
+            }
+        )
+
+    def go_forward(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "goForward",
+            }
+        )
+
+    def go_back(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "goBack",
+            }
+        )
+
+    def reload(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "reload",
+            }
+        )
+
+    def navigate_to(self, url: str):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "navigateTo",
+                "url": url,
+            }
+        )
+
+    def switch_to_frame(self, window_id: str):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "switchToFrame",
+                "windowId": window_id,
+            }
+        )
+
+    def list_frames(self):
+        # todo: replace with extract expression
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "listFrames",
+            }
+        )[
+            "frames"
+        ]  # type: ignore
+
+    def list_workers(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "listWorkers",
+            }
+        )
+
+    def log_in_page(self, text="", category="", flags=""):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "logInPage",
+                "text": text,
+                "category": category,
+                "flags": flags,
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/source.py` & `geckordp-0.5.0/geckordp/actors/source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,105 @@
 from geckordp.actors.actor import Actor
 
 
 class SourceActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/source.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/source.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def get_breakpoint_positions(self,
-                                 start_line=0,
-                                 start_column=0,
-                                 end_line=10**10,
-                                 end_column=10**10):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getBreakpointPositions",
-            "query": {
-                "start": {
-                    "line": start_line,
-                    "column": start_column,
-                },
-                "end": {
-                    "line": end_line,
-                    "column": end_column,
-                },
-            }
-        }, "positions")
-
-    def get_breakpoint_positions_compressed(self,
-                                            start_line=0,
-                                            start_column=0,
-                                            end_line=10**10,
-                                            end_column=10**10):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getBreakpointPositionsCompressed",
-            "query": {
-                "start": {
-                    "line": start_line,
-                    "column": start_column,
-                },
-                "end": {
-                    "line": end_line,
-                    "column": end_column,
+    def get_breakpoint_positions(
+        self,
+        start_line=0,
+        start_column=0,
+        end_line=10**10,
+        end_column=10**10,
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getBreakpointPositions",
+                "query": {
+                    "start": {
+                        "line": start_line,
+                        "column": start_column,
+                    },
+                    "end": {
+                        "line": end_line,
+                        "column": end_column,
+                    },
+                },
+            },
+            "positions",
+        )
+
+    def get_breakpoint_positions_compressed(
+        self,
+        start_line=0,
+        start_column=0,
+        end_line=10**10,
+        end_column=10**10,
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getBreakpointPositionsCompressed",
+                "query": {
+                    "start": {
+                        "line": start_line,
+                        "column": start_column,
+                    },
+                    "end": {
+                        "line": end_line,
+                        "column": end_column,
+                    },
                 },
             }
-        })
+        )
 
     def get_breakable_lines(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getBreakableLines",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getBreakableLines",
+            }
+        )
 
     def source(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "source",
-        })
-
-    def set_pause_point(self,
-                        line: int,
-                        column: int,
-                        breakpoint_=True,
-                        stepover=True):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "source",
+            }
+        )
+
+    def set_pause_point(self, line: int, column: int, breakpoint_=True, stepover=True):
         # https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/server/tests/xpcshell/test_stepping-with-skip-breakpoints.js#L34
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setPausePoints",
-            "pausePoints": [
-                {
-                    "location": {
-                        "line": line,
-                        "column": column,
-                    },
-                    "types": {
-                        "breakpoint": breakpoint_,
-                        "stepOver": stepover,
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setPausePoints",
+                "pausePoints": [
+                    {
+                        "location": {
+                            "line": line,
+                            "column": column,
+                        },
+                        "types": {
+                            "breakpoint": breakpoint_,
+                            "stepOver": stepover,
+                        },
                     },
-                },
-            ],
-        })
+                ],
+            }
+        )
 
     def set_pause_points(self, pause_points: list | None = None):
         # https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/server/tests/xpcshell/test_stepping-with-skip-breakpoints.js#L34
-        if (pause_points is None):
+        if pause_points is None:
             pause_points = [
                 # point 1
                 {
                     "location": {
                         "line": 0,
                         "column": 0,
                     },
@@ -106,54 +116,56 @@
                     },
                     "types": {
                         "breakpoint": True,
                         "stepOver": True,
                     },
                 },
             ]
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setPausePoints",
-            "pausePoints": pause_points,
-        })
-
-    def blackbox(self,
-                 start_line: int,
-                 start_column: int,
-                 end_line: int,
-                 end_column: int):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setPausePoints",
+                "pausePoints": pause_points,
+            }
+        )
+
+    def blackbox(
+        self, start_line: int, start_column: int, end_line: int, end_column: int
+    ):
         # https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/server/tests/xpcshell/test_blackboxing-03.js#L62
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "blackbox",
-            "range": {
-                "start": {
-                    "line": start_line,
-                    "column": start_column,
-                },
-                "end": {
-                    "line": end_line,
-                    "column": end_column,
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "blackbox",
+                "range": {
+                    "start": {
+                        "line": start_line,
+                        "column": start_column,
+                    },
+                    "end": {
+                        "line": end_line,
+                        "column": end_column,
+                    },
                 },
-            },
-        })
+            }
+        )
 
-    def unblackbox(self,
-                   start_line: int,
-                   start_column: int,
-                   end_line: int,
-                   end_column: int):
+    def unblackbox(
+        self, start_line: int, start_column: int, end_line: int, end_column: int
+    ):
         # https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/server/tests/xpcshell/test_blackboxing-03.js#L62
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "unblackbox",
-            "ranges": {
-                "start": {
-                    "line": start_line,
-                    "column": start_column,
-                },
-                "end": {
-                    "line": end_line,
-                    "column": end_column,
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "unblackbox",
+                "ranges": {
+                    "start": {
+                        "line": start_line,
+                        "column": start_column,
+                    },
+                    "end": {
+                        "line": end_line,
+                        "column": end_column,
+                    },
                 },
-            },
-        })
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/walker.py` & `geckordp-0.5.0/geckordp/actors/walker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,381 +1,514 @@
 from enum import Enum
 from typing import List, cast
+
 from geckordp.actors.actor import Actor
 
 
 class WalkerActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/walker.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/walker.js"""
 
     class Position(str, Enum):
-        """ https://developer.mozilla.org/en-US/docs/Web/API/Element/insertAdjacentHTML#parameters
-        """
+        """https://developer.mozilla.org/en-US/docs/Web/API/Element/insertAdjacentHTML#parameters"""
+
         BEFORE_BEGIN = "beforeBegin"
         AFTER_BEGIN = "afterBegin"
         BEFORE_END = "beforeEnd"
         AFTER_END = "afterEnd"
 
     class PseudoClass(str, Enum):
-        """ https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/How_to/Examine_and_edit_CSS#viewing_common_pseudo-classes
-        """
+        """https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/How_to/Examine_and_edit_CSS#viewing_common_pseudo-classes"""
+
         HOVER = ":hover"
         ACTIVE = ":active"
         FOCUS = ":focus"
         FOCUS_VISIBLE = ":focus-visible"
         FOCUS_WITHIN = ":focus-within"
         VISITED = ":visited"
         TARGET = ":target"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def release(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "release",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "release",
+            }
+        )
 
     def document(self, dom_node_actor=""):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "document",
-            "node": dom_node_actor,
-        }, "node")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "document",
+                "node": dom_node_actor,
+            },
+            "node",
+        )
 
     def document_element(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "documentElement",
-            "node": dom_node_actor,
-        }, "node")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "documentElement",
+                "node": dom_node_actor,
+            },
+            "node",
+        )
 
     def retain_node(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "retainNode",
-            "node": dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "retainNode",
+                "node": dom_node_actor,
+            }
+        )
 
     def unretain_node(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "unretainNode",
-            "node": dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "unretainNode",
+                "node": dom_node_actor,
+            }
+        )
 
     def release_node(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "releaseNode",
-            "node": dom_node_actor,
-        })
-
-    def children(self, dom_node_actor: str, max_nodes=1000, center_node="", start_node="", what_to_show=""):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "children",
-            "node": dom_node_actor,
-            "maxNodes": max_nodes,
-            "center": center_node,
-            "start": start_node,
-            "whatToShow": what_to_show,
-        }, "nodes")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "releaseNode",
+                "node": dom_node_actor,
+            }
+        )
+
+    def children(
+        self,
+        dom_node_actor: str,
+        max_nodes=1000,
+        center_node="",
+        start_node="",
+        what_to_show="",
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "children",
+                "node": dom_node_actor,
+                "maxNodes": max_nodes,
+                "center": center_node,
+                "start": start_node,
+                "whatToShow": what_to_show,
+            },
+            "nodes",
+        )
 
     def next_sibling(self, dom_node_actor: str, what_to_show=""):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "nextSibling",
-            "node": dom_node_actor,
-            "whatToShow": what_to_show,
-        }, "node")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "nextSibling",
+                "node": dom_node_actor,
+                "whatToShow": what_to_show,
+            },
+            "node",
+        )
 
     def previous_sibling(self, dom_node_actor: str, what_to_show=""):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "previousSibling",
-            "node": dom_node_actor,
-            "whatToShow": what_to_show,
-        }, "node")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "previousSibling",
+                "node": dom_node_actor,
+                "whatToShow": what_to_show,
+            },
+            "node",
+        )
 
     def find_inspecting_node(self):
         # "Spec for 'domwalker' specifies a 'findInspectingNode' method that isn't implemented by the actor"
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "findInspectingNode",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "findInspectingNode",
+            }
+        )
 
     def query_selector(self, dom_node_actor: str, selector: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "querySelector",
-            "node": dom_node_actor,
-            "selector": selector,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "querySelector",
+                "node": dom_node_actor,
+                "selector": selector,
+            }
+        )
 
     def query_selector_all(self, dom_node_actor: str, selector: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "querySelectorAll",
-            "node": dom_node_actor,
-            "selector": selector,
-        }, "list")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "querySelectorAll",
+                "node": dom_node_actor,
+                "selector": selector,
+            },
+            "list",
+        )
 
     def search(self, query):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "search",
-            "query": query,
-        }, "list")
-
-    def get_suggestions_for_query(self, completing: str, query="", selector_state="tag"):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getSuggestionsForQuery",
-            "query": query,
-            "completing": completing,
-            "selectorState": selector_state,
-        })
-
-    def add_pseudo_class_lock(self, dom_node_actor: str, pseudo_class: PseudoClass, parents: bool):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "addPseudoClassLock",
-            "node": dom_node_actor,
-            "pseudoClass": pseudo_class.value,
-            "parents": parents,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "search",
+                "query": query,
+            },
+            "list",
+        )
+
+    def get_suggestions_for_query(
+        self, completing: str, query="", selector_state="tag"
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getSuggestionsForQuery",
+                "query": query,
+                "completing": completing,
+                "selectorState": selector_state,
+            }
+        )
+
+    def add_pseudo_class_lock(
+        self, dom_node_actor: str, pseudo_class: PseudoClass, parents: bool
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "addPseudoClassLock",
+                "node": dom_node_actor,
+                "pseudoClass": pseudo_class.value,
+                "parents": parents,
+            }
+        )
 
     def hide_node(self, dom_node_actor: str):
         # "node.rawNode.classList is undefined"
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "hideNode",
-            "node": dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "hideNode",
+                "node": dom_node_actor,
+            }
+        )
 
     def unhide_node(self, dom_node_actor: str):
         # "node.rawNode.classList is undefined"
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "unhideNode",
-            "node": dom_node_actor,
-        })
-
-    def remove_pseudo_class_lock(self, dom_node_actor: str, pseudo_class: PseudoClass, parents: bool):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removePseudoClassLock",
-            "node": dom_node_actor,
-            "pseudoClass": pseudo_class.value,
-            "parents": parents,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "unhideNode",
+                "node": dom_node_actor,
+            }
+        )
+
+    def remove_pseudo_class_lock(
+        self, dom_node_actor: str, pseudo_class: PseudoClass, parents: bool
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removePseudoClassLock",
+                "node": dom_node_actor,
+                "pseudoClass": pseudo_class.value,
+                "parents": parents,
+            }
+        )
 
     def clear_pseudo_class_locks(self, dom_node_actor: str):
         # "InspectorUtils.clearPseudoClassLocks: Argument 1 does not implement interface Element."
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "clearPseudoClassLocks",
-            "node": dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "clearPseudoClassLocks",
+                "node": dom_node_actor,
+            }
+        )
 
     def inner_html(self, dom_node_actor: str):
-        return cast(str, self.client.send_receive({
-            "to": self.actor_id,
-            "type": "innerHTML",
-            "node": dom_node_actor,
-        }, "value"))
+        return cast(
+            str,
+            self.client.send_receive(
+                {
+                    "to": self.actor_id,
+                    "type": "innerHTML",
+                    "node": dom_node_actor,
+                },
+                "value",
+            ),
+        )
 
     def set_inner_html(self, dom_node_actor: str, value: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setInnerHTML",
-            "node": dom_node_actor,
-            "value": value,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setInnerHTML",
+                "node": dom_node_actor,
+                "value": value,
+            }
+        )
 
     def outer_html(self, dom_node_actor: str):
-        return cast(str, self.client.send_receive({
-            "to": self.actor_id,
-            "type": "outerHTML",
-            "node": dom_node_actor,
-        }, "value"))
+        return cast(
+            str,
+            self.client.send_receive(
+                {
+                    "to": self.actor_id,
+                    "type": "outerHTML",
+                    "node": dom_node_actor,
+                },
+                "value",
+            ),
+        )
 
     def set_outer_html(self, dom_node_actor: str, value: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setOuterHTML",
-            "node": dom_node_actor,
-            "value": value,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setOuterHTML",
+                "node": dom_node_actor,
+                "value": value,
+            }
+        )
 
     def insert_adjacent_html(self, dom_node_actor: str, position: Position, value: str):
-        """ see https://developer.mozilla.org/en-US/docs/Web/API/Element/insertAdjacentHTML
-        """
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "insertAdjacentHTML",
-            "node": dom_node_actor,
-            "position": position.value,
-            "value": value,
-        })
+        """see https://developer.mozilla.org/en-US/docs/Web/API/Element/insertAdjacentHTML"""
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "insertAdjacentHTML",
+                "node": dom_node_actor,
+                "position": position.value,
+                "value": value,
+            }
+        )
 
     def duplicate_node(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "duplicateNode",
-            "node": dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "duplicateNode",
+                "node": dom_node_actor,
+            }
+        )
 
     def remove_node(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removeNode",
-            "node": dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removeNode",
+                "node": dom_node_actor,
+            }
+        )
 
     def remove_nodes(self, dom_node_actors: List[str]):
         # "Cannot remove document, document elements or dead nodes."
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removeNode",
-            "node": dom_node_actors,
-        })
-
-    def insert_before(self, dom_node_actor: str, parent_dom_node_actor: str, sibling_dom_node_actor=""):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "insertBefore",
-            "node": dom_node_actor,
-            "parent": parent_dom_node_actor,
-            "sibling": sibling_dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removeNode",
+                "node": dom_node_actors,
+            }
+        )
+
+    def insert_before(
+        self, dom_node_actor: str, parent_dom_node_actor: str, sibling_dom_node_actor=""
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "insertBefore",
+                "node": dom_node_actor,
+                "parent": parent_dom_node_actor,
+                "sibling": sibling_dom_node_actor,
+            }
+        )
 
     def edit_tag_name(self, dom_node_actor: str, tag_name: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "editTagName",
-            "node": dom_node_actor,
-            "tagName": tag_name,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "editTagName",
+                "node": dom_node_actor,
+                "tagName": tag_name,
+            }
+        )
 
     def get_mutations(self, cleanup: bool):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getMutations",
-            "cleanup": cleanup,
-        }, "mutations")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getMutations",
+                "cleanup": cleanup,
+            },
+            "mutations",
+        )
 
     def is_in_dom_tree(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "isInDOMTree",
-            "node": dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "isInDOMTree",
+                "node": dom_node_actor,
+            }
+        )
 
     def get_node_actor_from_window_id(self, window_id: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getNodeActorFromWindowID",
-            "windowID": window_id,
-        }, "nodeFront")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getNodeActorFromWindowID",
+                "windowID": window_id,
+            },
+            "nodeFront",
+        )
 
     def get_node_actor_from_content_dom_reference(self, content_dom_ref: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getNodeActorFromContentDomReference",
-            "contentDomReference": content_dom_ref,
-        }, "nodeFront")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getNodeActorFromContentDomReference",
+                "contentDomReference": content_dom_ref,
+            },
+            "nodeFront",
+        )
 
     def get_style_sheet_owner_node(self, style_sheet_actor_id: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getStyleSheetOwnerNode",
-            "styleSheetActorID": style_sheet_actor_id,
-        }, "ownerNode")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getStyleSheetOwnerNode",
+                "styleSheetActorID": style_sheet_actor_id,
+            },
+            "ownerNode",
+        )
 
     def get_node_from_actor(self, actor_id: str, paths: List[str] | None = None):
-        if (paths is None):
+        if paths is None:
             paths = []
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getNodeFromActor",
-            "actorID": actor_id,
-            "path": paths,
-        }, "node")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getNodeFromActor",
+                "actorID": actor_id,
+                "path": paths,
+            },
+            "node",
+        )
 
     def get_layout_inspector(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getLayoutInspector",
-        }, "actor")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getLayoutInspector",
+            },
+            "actor",
+        )
 
     def get_parent_grid_node(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getParentGridNode",
-            "node": dom_node_actor,
-        }, "node")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getParentGridNode",
+                "node": dom_node_actor,
+            },
+            "node",
+        )
 
     def get_offset_parent(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getOffsetParent",
-            "node": dom_node_actor,
-        }, "node")
-
-    def set_mutation_breakpoints(self, dom_node_actor: str, subtree: bool, removal: bool, attribute: bool):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setMutationBreakpoints",
-            "node": dom_node_actor,
-            "subtree": subtree,
-            "removal": removal,
-            "attribute": attribute,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getOffsetParent",
+                "node": dom_node_actor,
+            },
+            "node",
+        )
+
+    def set_mutation_breakpoints(
+        self, dom_node_actor: str, subtree: bool, removal: bool, attribute: bool
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setMutationBreakpoints",
+                "node": dom_node_actor,
+                "subtree": subtree,
+                "removal": removal,
+                "attribute": attribute,
+            }
+        )
 
     def get_embedder_element(self, browsing_context_id: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getEmbedderElement",
-            "browsingContextID": browsing_context_id,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getEmbedderElement",
+                "browsingContextID": browsing_context_id,
+            }
+        )
 
     def pick(self, focus: bool, is_local_tab: bool):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "pick",
-            "doFocus": focus,
-            "isLocalTab": is_local_tab,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "pick",
+                "doFocus": focus,
+                "isLocalTab": is_local_tab,
+            }
+        )
 
     def cancel_pick(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "cancelPick",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "cancelPick",
+            }
+        )
 
     def clear_picker(self):
-        self.client.send({
-            "to": self.actor_id,
-            "type": "clearPicker",
-        })
+        self.client.send(
+            {
+                "to": self.actor_id,
+                "type": "clearPicker",
+            }
+        )
 
     def watch_root_node(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "watchRootNode",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "watchRootNode",
+            }
+        )
 
     def get_overflow_causing_elements(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getOverflowCausingElements",
-            "node": dom_node_actor,
-        }, "list")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getOverflowCausingElements",
+                "node": dom_node_actor,
+            },
+            "list",
+        )
 
     def get_scrollable_ancestor_node(self, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getScrollableAncestorNode",
-            "node": dom_node_actor,
-        }, "node")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getScrollableAncestorNode",
+                "node": dom_node_actor,
+            },
+            "node",
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/node_list.py` & `geckordp-0.5.0/geckordp/actors/node_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from geckordp.actors.actor import Actor
 
 
 class NodeListActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/node.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/node.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def item(self, index: int):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "item",
-            "item": index,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "item",
+                "item": index,
+            }
+        )
 
     def items(self, start: int, end: int):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "items",
-            "start": start,
-            "end": end,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "items",
+                "start": start,
+                "end": end,
+            }
+        )
 
     def release(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "release",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "release",
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/storage.py` & `geckordp-0.5.0/geckordp/actors/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,150 +1,186 @@
 from typing import List
+
 from geckordp.actors.actor import Actor
 
 
 # pylint: disable=invalid-name
 class _impl_storage(Actor):
 
-    def get_store_objects(self, host: str, names: List[str] | None = None, options: dict | None = None):
-        if (options is None):
+    def get_store_objects(
+        self,
+        host: str,
+        names: List[str] | None = None,
+        options: dict | None = None,
+    ):
+        if options is None:
             options = {}
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getStoreObjects",
-            "host": host,
-            "names": names,
-            "options": options,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getStoreObjects",
+                "host": host,
+                "names": names,
+                "options": options,
+            }
+        )
 
     def get_fields(self, sub_type: str | None = None):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getFields",
-            "subType": sub_type,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getFields",
+                "subType": sub_type,
+            }
+        )
 
 
 # pylint: disable=invalid-name
 class _impl_remove_item(Actor):
 
     def remove_item(self, host: str, name: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removeItem",
-            "host": host,
-            "name": name,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removeItem",
+                "host": host,
+                "name": name,
+            }
+        )
 
 
 # pylint: disable=invalid-name
 class _impl_add_item(Actor):
 
     def add_item(self, guid: str, host: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "addItem",
-            "guid": guid,
-            "host": host,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "addItem",
+                "guid": guid,
+                "host": host,
+            }
+        )
 
 
 # pylint: disable=invalid-name
 class _impl_edit_item(Actor):
 
     def edit_item(self, data: dict):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "editItem",
-            "data": data,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "editItem",
+                "data": data,
+            }
+        )
 
 
 # pylint: disable=invalid-name
 class _impl_remove_all__host(Actor):
 
     def remove_all(self, host: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removeAll",
-            "host": host,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removeAll",
+                "host": host,
+            }
+        )
 
 
 # pylint: disable=invalid-name
 class _impl_remove_all__host_name(Actor):
 
     def remove_all(self, host: str, name: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removeAll",
-            "host": host,
-            "name": name,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removeAll",
+                "host": host,
+                "name": name,
+            }
+        )
 
 
 class CookieStorageActor(_impl_storage, _impl_add_item, _impl_remove_item):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js"""
 
     def edit_item(self, host: str, field: str, old_value, new_value, cookie_data: dict):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "editItem",
-            "data": {
-                "host": host,
-                "key": "uniqueKey",
-                "field": field,
-                "oldValue": old_value,
-                "newValue": new_value,
-                "items": cookie_data,
-            },
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "editItem",
+                "data": {
+                    "host": host,
+                    "key": "uniqueKey",
+                    "field": field,
+                    "oldValue": old_value,
+                    "newValue": new_value,
+                    "items": cookie_data,
+                },
+            }
+        )
 
     def remove_all(self, host: str, domain: str | None = None):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removeAll",
-            "host": host,
-            "domain": domain,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removeAll",
+                "host": host,
+                "domain": domain,
+            }
+        )
 
     def remove_all_session_cookies(self, host: str, domain: str | None = None):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removeAllSessionCookies",
-            "host": host,
-            "domain": domain,
-        })
-
-
-class LocalStorageActor(_impl_storage, _impl_add_item, _impl_remove_item, _impl_edit_item, _impl_remove_all__host):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js
-    """
-
-
-class SessionStorageActor(_impl_storage, _impl_add_item, _impl_remove_item, _impl_edit_item, _impl_remove_all__host):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js
-    """
-
-
-class ExtensionStorageActor(_impl_storage, _impl_remove_item, _impl_edit_item, _impl_remove_all__host):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js
-    """
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removeAllSessionCookies",
+                "host": host,
+                "domain": domain,
+            }
+        )
+
+
+class LocalStorageActor(
+    _impl_storage,
+    _impl_add_item,
+    _impl_remove_item,
+    _impl_edit_item,
+    _impl_remove_all__host,
+):
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js"""
+
+
+class SessionStorageActor(
+    _impl_storage,
+    _impl_add_item,
+    _impl_remove_item,
+    _impl_edit_item,
+    _impl_remove_all__host,
+):
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js"""
+
+
+class ExtensionStorageActor(
+    _impl_storage, _impl_remove_item, _impl_edit_item, _impl_remove_all__host
+):
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js"""
 
 
 class CacheStorageActor(_impl_storage, _impl_remove_item, _impl_remove_all__host_name):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js"""
 
 
 class IndexedDBStorageActor(_impl_storage, _impl_remove_item):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js"""
 
     def remove_database(self, host: str, name: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removeDatabase",
-            "host": host,
-            "name": name,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removeDatabase",
+                "host": host,
+                "name": name,
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/network_content.py` & `geckordp-0.5.0/geckordp/actors/network_content.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 from geckordp.actors.actor import Actor
 
 
 class NetworkContentActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/network-content.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/network-content.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def send_http_request(self,
-                          url: str,
-                          method="GET",
-                          headers: dict | None = None,
-                          body=""):
-        if (headers is None):
+    def send_http_request(
+        self,
+        url: str,
+        method="GET",
+        headers: dict | None = None,
+        body="",
+    ):
+        if headers is None:
             """
             {
                 "Host": "www.duckduckgo.com",
                 "User-Agent": "my-user-agent",
             }
             """
             headers = {}
         nheaders = []
         for name, value in headers.items():
-            nheaders.append({
-                "name": name,
-                "value": value,
-            })
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "sendHTTPRequest",
-            "request": {
-                "cause": {
-                    "type": "document",
-                    "loadingDocumentUri": None,
-                    "stacktraceAvailable": True,
-                    "lastFrame": {},
+            nheaders.append(
+                {
+                    "name": name,
+                    "value": value,
+                }
+            )
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "sendHTTPRequest",
+                "request": {
+                    "cause": {
+                        "type": "document",
+                        "loadingDocumentUri": None,
+                        "stacktraceAvailable": True,
+                        "lastFrame": {},
+                    },
+                    "url": url,
+                    "method": method.upper(),
+                    "headers": nheaders,
+                    "body": body,
                 },
-                "url": url,
-                "method": method.upper(),
-                "headers": nheaders,
-                "body": body,
-            },
-        })
+            }
+        )
 
     def get_stack_trace(self, resource_id: int):
         # todo: on firefox-100.0 'get_stack_trace()' doesn't seem to work anymore,
         # even if 'WatcherActor.watch_resources()' was successful
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getStackTrace",
-            "resourceId": resource_id,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getStackTrace",
+                "resourceId": resource_id,
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/accessibility/simulator.py` & `geckordp-0.5.0/geckordp/actors/accessibility/simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from enum import Enum
+
 from geckordp.actors.actor import Actor
 
 
 class SimulatorActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L212
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L212"""
 
     class Types(str, Enum):
         NONE = "NONE"
         PROTANOPIA = "PROTANOPIA"
         DEUTERANOPIA = "DEUTERANOPIA"
         TRITANOPIA = "TRITANOPIA"
         ACHROMATOPSIA = "ACHROMATOPSIA"
         CONTRAST_LOSS = "CONTRAST_LOSS"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def simulate(self, simulate_matrix: Types = Types.NONE):
         args = []
-        if (simulate_matrix != SimulatorActor.Types.NONE):
+        if simulate_matrix != SimulatorActor.Types.NONE:
             args.append(simulate_matrix.value)
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "simulate",
-            "options": {
-                "types": args,
-            },
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "simulate",
+                "options": {
+                    "types": args,
+                },
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/accessibility/accessibility.py` & `geckordp-0.5.0/geckordp/actors/accessibility/accessibility.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 from geckordp.actors.actor import Actor
 
 
 class AccessibilityActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L225
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L225"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def get_traits(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getTraits",
-        }, "traits")
-    
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getTraits",
+            },
+            "traits",
+        )
+
     def bootstrap(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "bootstrap",
-        }, "state")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "bootstrap",
+            },
+            "state",
+        )
 
     def get_walker(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getWalker",
-        }, "walker")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getWalker",
+            },
+            "walker",
+        )
 
     def get_simulator(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getSimulator",
-        }, "simulator")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getSimulator",
+            },
+            "simulator",
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/accessibility/accessible_walker.py` & `geckordp-0.5.0/geckordp/actors/accessibility/accessible_walker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,97 @@
 from geckordp.actors.actor import Actor
 
 
 class AccessibleWalkerActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L130
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L130"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def children(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "children",
-        }, "children")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "children",
+            },
+            "children",
+        )
 
     def get_accessible_for(self, dom_node_actor: str):
         # 'dom_node_actor' can be retrieved from WalkerActor
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getAccessibleFor",
-            "node": dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getAccessibleFor",
+                "node": dom_node_actor,
+            }
+        )
 
     def get_ancestry(self, accessible):
         # probably needs the accesible object from 'get_accessible_for()'
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getAncestry",
-            "accessible": accessible,
-        }, "ancestry")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getAncestry",
+                "accessible": accessible,
+            },
+            "ancestry",
+        )
 
     def start_audit(self, options: dict | None = None):
-        if (options is None):
+        if options is None:
             options = {}
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "startAudit",
-            "options": options,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "startAudit",
+                "options": options,
+            }
+        )
 
     def highlight_accessible(self, accessible, options: dict | None = None):
         # probably needs the accesible object from 'get_accessible_for()'
-        if (options is None):
+        if options is None:
             options = {}
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "highlightAccessible",
-            "accessible": accessible,
-            "options": options,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "highlightAccessible",
+                "accessible": accessible,
+                "options": options,
+            }
+        )
 
     def unhighlight(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "unhighlight",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "unhighlight",
+            }
+        )
 
     def cancel_pick(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "cancelPick",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "cancelPick",
+            }
+        )
 
     def pick_and_focus(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "pickAndFocus",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "pickAndFocus",
+            }
+        )
 
     def show_tabbing_order(self, dom_node_actor: str, index: int):
         # 'dom_node_actor' can be retrieved from WalkerActor
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "showTabbingOrder",
-            "elm": dom_node_actor,
-            "index": index,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "showTabbingOrder",
+                "elm": dom_node_actor,
+                "index": index,
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/accessibility/accessible.py` & `geckordp-0.5.0/geckordp/actors/accessibility/accessible.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 from geckordp.actors.actor import Actor
 
 
 class AccessibleActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L46
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L46"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def audit(self, options: dict | None = None):
-        if (options is None):
+        if options is None:
             options = {}
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "audit",
-            "options": options,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "audit",
+                "options": options,
+            }
+        )
 
     def children(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "children",
-        }, "children")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "children",
+            },
+            "children",
+        )
 
     def get_relations(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getRelations",
-        }, "relations")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getRelations",
+            },
+            "relations",
+        )
 
     def hydrate(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "hydrate",
-        }, "properties")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "hydrate",
+            },
+            "properties",
+        )
 
     def snapshot(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "snapshot",
-        }, "snapshot")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "snapshot",
+            },
+            "snapshot",
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/accessibility/parent_accessibility.py` & `geckordp-0.5.0/geckordp/actors/descriptors/worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from geckordp.actors.actor import Actor
 
 
-class ParentAccessibilityActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L263
-    """
+class WorkerActor(Actor):
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/descriptors/worker.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def bootstrap(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "bootstrap",
-        })
-
-    def enable(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "enable",
-        })
-
-    def disable(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "disable",
-        })
+    def detach(self):
+        self.client.send(
+            {
+                "to": self.actor_id,
+                "type": "detach",
+            }
+        )
+
+    def get_target(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getTarget",
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/preference.py` & `geckordp-0.5.0/geckordp/actors/preference.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 from typing import Any
+
 from geckordp.actors.actor import Actor
 
 
 class PreferenceActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/preference.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/preference.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def get_traits(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getTraits",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getTraits",
+            }
+        )
 
     def get_bool_pref(self, value: Any):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getBoolPref",
-            "value": value
-        })
+        return self.client.send_receive(
+            {"to": self.actor_id, "type": "getBoolPref", "value": value}
+        )
 
     def get_char_pref(self, value: Any):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getCharPref",
-            "value": value
-        })
+        return self.client.send_receive(
+            {"to": self.actor_id, "type": "getCharPref", "value": value}
+        )
 
     def get_int_pref(self, value: Any):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getIntPref",
-            "value": value
-        })
+        return self.client.send_receive(
+            {"to": self.actor_id, "type": "getIntPref", "value": value}
+        )
 
     def get_all_prefs(self, value: Any):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getAllPrefs",
-            "value": value
-        }, "value")
+        return self.client.send_receive(
+            {"to": self.actor_id, "type": "getAllPrefs", "value": value}, "value"
+        )
 
     def set_bool_pref(self, name: str, value: Any):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setBoolPref",
-            "name": name,
-            "value": value,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setBoolPref",
+                "name": name,
+                "value": value,
+            }
+        )
 
     def set_char_pref(self, name: str, value: Any):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setCharPref",
-            "name": name,
-            "value": value,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setCharPref",
+                "name": name,
+                "value": value,
+            }
+        )
 
     def set_int_pref(self, name: str, value: Any):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setIntPref",
-            "name": name,
-            "value": value,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setIntPref",
+                "name": name,
+                "value": value,
+            }
+        )
 
     def clear_user_pref(self, name: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "clearUserPref",
-            "name": name,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "clearUserPref",
+                "name": name,
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/network_event.py` & `geckordp-0.5.0/geckordp/actors/network_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,103 @@
 from geckordp.actors.actor import Actor
 
 
 class NetworkEventActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/network-event.js
-        https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/client/netmonitor/src/actions/search.js#L105
-        https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/client/netmonitor/src/constants.js#L153
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/network-event.js
+    https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/client/netmonitor/src/actions/search.js#L105
+    https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/client/netmonitor/src/constants.js#L153
 
-        .. note:: The 'actor_id' a.k.a. 'netEvent' must be taken from ["type": "resource-available-form"] event and not ["type": "networkEvent"].
+    .. note:: The 'actor_id' a.k.a. 'netEvent' must be taken from ["type": "resource-available-form"] event and not ["type": "networkEvent"].
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def release(self):
-        """ If data is not needed anymore, it can be freed on the serverside.
-            Following calls to other functions after 'release()' will fail.
+        """If data is not needed anymore, it can be freed on the serverside.
+        Following calls to other functions after 'release()' will fail.
         """
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "release",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "release",
+            }
+        )
 
     def get_request_headers(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getRequestHeaders",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getRequestHeaders",
+            }
+        )
 
     def get_request_cookies(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getRequestCookies",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getRequestCookies",
+            }
+        )
 
     def get_request_post_data(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getRequestPostData",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getRequestPostData",
+            }
+        )
 
     def get_response_headers(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getResponseHeaders",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getResponseHeaders",
+            }
+        )
 
     def get_response_cookies(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getResponseCookies",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getResponseCookies",
+            }
+        )
 
     def get_response_cache(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getResponseCache",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getResponseCache",
+            }
+        )
 
     def get_response_content(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getResponseContent",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getResponseContent",
+            }
+        )
 
     def get_event_timings(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getEventTimings",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getEventTimings",
+            }
+        )
 
     def get_security_info(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getSecurityInfo",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getSecurityInfo",
+            }
+        )
 
     # todo: "Spec for 'netEvent' specifies a 'getStackTrace' method that isn't implemented by the actor",
     """ def get_stack_trace(self):
         return self.client.send_receive({
             "to": self.actor_id,
             "type": "getStackTrace",
         }) """
```

## Comparing `geckordp-0.4.53/geckordp/actors/memory.py` & `geckordp-0.5.0/geckordp/actors/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,113 +1,137 @@
 from typing import Any, Dict, cast
+
 from geckordp.actors.actor import Actor
 
 
 class MemoryActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/memory.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/memory.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def attach(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "attach",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "attach",
+            }
+        )
 
     def detach(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "detach",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "detach",
+            }
+        )
 
     def get_state(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getState",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getState",
+            }
+        )
 
     def take_census(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "takeCensus",
-        })
-
-    def start_recording_allocations(self, probability: float | None = None, max_log_length: int | None = None):
-        if (probability is not None and (probability < 0.0 or probability > 1.0)):
-            raise ValueError(
-                "parameter 'probability' must be in range of 0.0 and 1.0")
-        if (max_log_length is not None and max_log_length < 0.0):
-            raise ValueError(
-                "parameter 'max_log_length' cannot be negative")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "takeCensus",
+            }
+        )
+
+    def start_recording_allocations(
+        self,
+        probability: float | None = None,
+        max_log_length: int | None = None,
+    ):
+        if probability is not None and (probability < 0.0 or probability > 1.0):
+            raise ValueError("parameter 'probability' must be in range of 0.0 and 1.0")
+        if max_log_length is not None and max_log_length < 0.0:
+            raise ValueError("parameter 'max_log_length' cannot be negative")
         args: Dict[str, Any] = {
             "to": self.actor_id,
             "type": "startRecordingAllocations",
         }
-        if (probability is not None or max_log_length is not None):
+        if probability is not None or max_log_length is not None:
             args["options"] = {}
-        if (probability is not None):
+        if probability is not None:
             args["options"]["probability"] = probability
-        if (max_log_length is not None):
+        if max_log_length is not None:
             args["options"]["maxLogLength"] = max_log_length
 
         return self.client.send_receive(args)
 
     def stop_recording_allocations(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "stopRecordingAllocations",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "stopRecordingAllocations",
+            }
+        )
 
     def get_allocations_settings(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getAllocationsSettings",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getAllocationsSettings",
+            }
+        )
 
     def get_allocations(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getAllocations",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getAllocations",
+            }
+        )
 
     def force_garbage_collection(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "forceGarbageCollection",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "forceGarbageCollection",
+            }
+        )
 
     def force_cycle_collection(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "forceCycleCollection",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "forceCycleCollection",
+            }
+        )
 
     def measure(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "measure",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "measure",
+            }
+        )
 
     def resident_unique(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "residentUnique",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "residentUnique",
+            }
+        )
 
     def save_heap_snapshot(self, boundaries: dict | None = None):
-        """ 
-            It seems like it will be handled automatically if no arguments are passed.
-            A wireshark rdp session also doesn't pass any additional arguments nor any toggleable functions exists in the menu.
-            I belive for many cases the snapshot should be ideal in the end.
-            https://github.com/mozilla/gecko-dev/blob/d36cf98aa85f24ceefd07521b3d16b9edd2abcb7/devtools/shared/heapsnapshot/tests/xpcshell/test_SaveHeapSnapshot.js
-            https://github.com/mozilla/gecko-dev/blob/d36cf98aa85f24ceefd07521b3d16b9edd2abcb7/devtools/server/performance/memory.js#L170
-            https://github.com/mozilla/gecko-dev/blob/d36cf98aa85f24ceefd07521b3d16b9edd2abcb7/devtools/server/performance/memory.js#L170
+        """
+        It seems like it will be handled automatically if no arguments are passed.
+        A wireshark rdp session also doesn't pass any additional arguments nor any toggleable functions exists in the menu.
+        I belive for many cases the snapshot should be ideal in the end.
+        https://github.com/mozilla/gecko-dev/blob/d36cf98aa85f24ceefd07521b3d16b9edd2abcb7/devtools/shared/heapsnapshot/tests/xpcshell/test_SaveHeapSnapshot.js
+        https://github.com/mozilla/gecko-dev/blob/d36cf98aa85f24ceefd07521b3d16b9edd2abcb7/devtools/server/performance/memory.js#L170
+        https://github.com/mozilla/gecko-dev/blob/d36cf98aa85f24ceefd07521b3d16b9edd2abcb7/devtools/server/performance/memory.js#L170
         """
         args: Dict[str, Any] = {
             "to": self.actor_id,
             "type": "saveHeapSnapshot",
         }
-        if (boundaries is not None):
+        if boundaries is not None:
             args["boundaries"] = boundaries
         return cast(str, self.client.send_receive(args, "snapshotId"))
```

## Comparing `geckordp-0.4.53/geckordp/actors/addon/addons.py` & `geckordp-0.5.0/geckordp/actors/addon/addons.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from geckordp.actors.actor import Actor
 
 
 class AddonsActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/addon/addons.js
-        https://github.com/mozilla/web-ext/blob/master/src/firefox/remote.js
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/addon/addons.js
+    https://github.com/mozilla/web-ext/blob/master/src/firefox/remote.js
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def install_temporary_addon(self, addon_path: str):
-        response = self.client.send_receive({
-            "to": self.actor_id,
-            "type": "installTemporaryAddon",
-            "addonPath": addon_path,
-        })
+        response = self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "installTemporaryAddon",
+                "addonPath": addon_path,
+            }
+        )
         # todo: replace with extract expression
         return response.get("addon", response)  # type: ignore
```

## Comparing `geckordp-0.4.53/geckordp/actors/addon/web_extension_inspected_window.py` & `geckordp-0.5.0/geckordp/actors/addon/web_extension_inspected_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 from geckordp.actors.actor import Actor
 
 
 class WebExtensionInspectedWindowActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/addon/webextension-inspected-window.js
-        https://github.com/mozilla/gecko-dev/blob/master/devtools/server/actors/addon/webextension-inspected-window.js
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/addon/webextension-inspected-window.js
+    https://github.com/mozilla/gecko-dev/blob/master/devtools/server/actors/addon/webextension-inspected-window.js
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def reload(self, url: str, line: int, addon_id: str, ignore_cache=False, user_agent="", injected_script=""):
-        response = self.client.send_receive({
-            "to": self.actor_id,
-            "type": "reload",
-            "webExtensionCallerInfo": {
-                "url": url,
-                "lineNumber": line,
-                "addonId": addon_id,
-            },
-            "options": {
-                "ignoreCache": ignore_cache,
-                "userAgent": user_agent,
-                "injectedScript": injected_script,
+    def reload(
+        self,
+        url: str,
+        line: int,
+        addon_id: str,
+        ignore_cache=False,
+        user_agent="",
+        injected_script="",
+    ):
+        response = self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "reload",
+                "webExtensionCallerInfo": {
+                    "url": url,
+                    "lineNumber": line,
+                    "addonId": addon_id,
+                },
+                "options": {
+                    "ignoreCache": ignore_cache,
+                    "userAgent": user_agent,
+                    "injectedScript": injected_script,
+                },
             }
-        })
+        )
         # todo: replace with extract expression
         return response.get("walker", response)  # type: ignore
 
     def eval(self, expression: str, url: str, line: int, addon_id: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "eval",
-            "webExtensionCallerInfo": {
-                "url": url,
-                "lineNumber": line,
-                "addonId": addon_id,
-            },
-            "expression": expression,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "eval",
+                "webExtensionCallerInfo": {
+                    "url": url,
+                    "lineNumber": line,
+                    "addonId": addon_id,
+                },
+                "expression": expression,
+            }
+        )
 
     # options not supported yet
     """def eval(self, expression: str, url: str, line: int, addon_id: str,
              use_content_script_context=True, frame_url="",
              context_security_origin="", eval_result_as_grip=False,
              toolbox_selected_node_actor_id="", toolbox_console_actor_id=""):
         return self.client.send_receive({
```

## Comparing `geckordp-0.4.53/geckordp/actors/web_console.py` & `geckordp-0.5.0/geckordp/actors/web_console.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from enum import Enum
 from typing import List
+
 from geckordp.actors.actor import Actor
 
 
 class WebConsoleActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/webconsole.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/webconsole.js"""
 
     class Listeners(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/aa3ccd258b64abfd4c5ce56c1f512bc7f65b844c/devtools/server/actors/webconsole.js#LL548C17-L548C17
-            Listeners != Events
+        """https://github.com/mozilla/gecko-dev/blob/aa3ccd258b64abfd4c5ce56c1f512bc7f65b844c/devtools/server/actors/webconsole.js#LL548C17-L548C17
+        Listeners != Events
         """
+
         PAGE_ERROR = "PageError"
         CONSOLE_API = "ConsoleAPI"
         FILE_ACTIVITY = "FileActivity"
         REFLOW_ACTIVITY = "ReflowActivity"
         DOCUMENT_EVENTS = "DocumentEvents"
 
     class MessageTypes(str, Enum):
@@ -24,82 +25,100 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def start_listeners(self, listeners: List[Listeners]):
         nlisteners = []
         for listener in listeners:
             nlisteners.append(str(listener.value))
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "startListeners",
-            "listeners": nlisteners,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "startListeners",
+                "listeners": nlisteners,
+            }
+        )
 
     def stop_listeners(self, listeners: List[Listeners]):
         nlisteners = []
         for listener in listeners:
             nlisteners.append(str(listener.value))
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "stopListeners",
-            "listeners": nlisteners,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "stopListeners",
+                "listeners": nlisteners,
+            }
+        )
 
     def get_cached_messages(self, message_types: List[MessageTypes]):
         nmessage_types = []
         for message_type in message_types:
             nmessage_types.append(str(message_type.value))
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getCachedMessages",
-            "messageTypes": nmessage_types,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getCachedMessages",
+                "messageTypes": nmessage_types,
+            }
+        )
 
     def evaluate_js_async(
-        self, text: str,
+        self,
+        text: str,
         eager=False,
         frame_actor="",
         selected_node_actor="",
         selected_object_actor="",
         inner_window_id=-1,
-        mapped: dict | None = None
+        mapped: dict | None = None,
     ):
         args = {
             "to": self.actor_id,
             "type": "evaluateJSAsync",
             "text": text,
             "eager": eager,
         }
-        if (frame_actor != ""):
+        if frame_actor != "":
             args["frameActor"] = frame_actor
-        if (selected_node_actor != ""):
+        if selected_node_actor != "":
             args["selectedNodeActor"] = selected_node_actor
-        if (selected_object_actor != ""):
+        if selected_object_actor != "":
             args["selectedObjectActor"] = selected_object_actor
-        if (inner_window_id != -1):
+        if inner_window_id != -1:
             args["innerWindowID"] = inner_window_id
-        if (mapped is not None):
+        if mapped is not None:
             args["mapped"] = mapped
         return self.client.send_receive(args)
 
-    def autocomplete(self, text: str, cursor=0, frame_actor="",
-                     selected_node_actor="", authorized_evaluations_json: dict | None = None, expression_vars_json: dict | None = None):
-        if (authorized_evaluations_json is None):
+    def autocomplete(
+        self,
+        text: str,
+        cursor=0,
+        frame_actor="",
+        selected_node_actor="",
+        authorized_evaluations_json: dict | None = None,
+        expression_vars_json: dict | None = None,
+    ):
+        if authorized_evaluations_json is None:
             authorized_evaluations_json = {}
-        if (expression_vars_json is None):
+        if expression_vars_json is None:
             expression_vars_json = {}
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "autocomplete",
-            "text": text,
-            "cursor": cursor,
-            "frameActor": frame_actor,
-            "selectedNodeActor": selected_node_actor,
-            "authorizedEvaluations": authorized_evaluations_json,
-            "expressionVars": expression_vars_json,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "autocomplete",
+                "text": text,
+                "cursor": cursor,
+                "frameActor": frame_actor,
+                "selectedNodeActor": selected_node_actor,
+                "authorizedEvaluations": authorized_evaluations_json,
+                "expressionVars": expression_vars_json,
+            }
+        )
 
     def clear_messages_cache(self):
-        return self.client.send({
-            "to": self.actor_id,
-            "type": "clearMessagesCache",
-        })
+        return self.client.send(
+            {
+                "to": self.actor_id,
+                "type": "clearMessagesCache",
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/root.py` & `geckordp-0.5.0/geckordp/actors/root.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,61 @@
-from geckordp.actors.actor import Actor
+from geckordp.actors.resources import ResourceActor
 
 
-class RootActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/root.js
-    """
+class RootActor(ResourceActor):
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/root.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.actor_id = "root"
 
     def get_root(self):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "getRoot"
-        })
+        return self.client.send_receive({"to": "root", "type": "getRoot"})
 
     def list_tabs(self):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "listTabs"
-        }, "tabs")
+        return self.client.send_receive({"to": "root", "type": "listTabs"}, "tabs")
 
     def get_tab(self, browser_id: int):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "getTab",
-            "browserId": browser_id,
-        })
+        return self.client.send_receive(
+            {
+                "to": "root",
+                "type": "getTab",
+                "browserId": browser_id,
+            }
+        )
 
     def list_addons(self):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "listAddons"
-        }, "addons")
+        return self.client.send_receive({"to": "root", "type": "listAddons"}, "addons")
 
     def list_workers(self):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "listWorkers"
-        }, "workers")
+        return self.client.send_receive(
+            {"to": "root", "type": "listWorkers"}, "workers"
+        )
 
     def list_service_worker_registrations(self):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "listServiceWorkerRegistrations"
-        }, "registrations")
+        return self.client.send_receive(
+            {"to": "root", "type": "listServiceWorkerRegistrations"}, "registrations"
+        )
 
     def list_processes(self):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "listProcesses"
-        }, "processes")
+        return self.client.send_receive(
+            {"to": "root", "type": "listProcesses"}, "processes"
+        )
 
     def get_process(self, pid: int):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "getProcess",
-            "id": pid,
-        })
+        return self.client.send_receive(
+            {
+                "to": "root",
+                "type": "getProcess",
+                "id": pid,
+            }
+        )
 
     def request_types(self):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "requestTypes"
-        }, "requestTypes")
+        return self.client.send_receive(
+            {"to": "root", "type": "requestTypes"}, "requestTypes"
+        )
 
     def current_tab(self):
-        return self.client.send_receive({
-            "to": "root",
-            "type": "listTabs"
-        }, "tabs[?selected==`true`] | [0]")
+        return self.client.send_receive(
+            {"to": "root", "type": "listTabs"}, "tabs[?selected==`true`] | [0]"
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/descriptors/tab.py` & `geckordp-0.5.0/geckordp/actors/descriptors/tab.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from typing import Any, Dict
+
 from geckordp.actors.actor import Actor
 
 
 class TabActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/descriptors/tab.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/descriptors/tab.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def get_target(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getTarget"
-        }, "frame")
+        return self.client.send_receive(
+            {"to": self.actor_id, "type": "getTarget"}, "frame"
+        )
 
     def get_favicon(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getFavicon"
-        }, "favicon")
-
-    def get_watcher(self, is_server_target_switching_enabled: bool | None = None, is_popup_debugging_enabled: bool | None = None):
+        return self.client.send_receive(
+            {"to": self.actor_id, "type": "getFavicon"}, "favicon"
+        )
+
+    def get_watcher(
+        self,
+        is_server_target_switching_enabled: bool = True,
+        is_popup_debugging_enabled: bool = False,
+    ):
+        # note:
+        # passing wrong arguments can lead to issues with related watcher events
         args: Dict[str, Any] = {
             "to": self.actor_id,
             "type": "getWatcher",
             "isServerTargetSwitchingEnabled": is_server_target_switching_enabled,
             "isPopupDebuggingEnabled": is_popup_debugging_enabled,
         }
         if is_server_target_switching_enabled is not None:
```

## Comparing `geckordp-0.4.53/geckordp/actors/descriptors/web_extension.py` & `geckordp-0.5.0/geckordp/actors/accessibility/parent_accessibility.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from geckordp.actors.actor import Actor
 
 
-class WebExtensionActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/descriptors/webextension.js
-    """
+class ParentAccessibilityActor(Actor):
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L263"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def reload(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "reload"
-        })
-
-    def connect(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "connect"
-        })
-
-    def get_target(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getTarget"
-        })
+    def bootstrap(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "bootstrap",
+            }
+        )
+
+    def enable(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "enable",
+            }
+        )
+
+    def disable(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "disable",
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/thread.py` & `geckordp-0.5.0/geckordp/actors/thread.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,241 +1,283 @@
 from enum import Enum
 from typing import Any, Dict
+
 from geckordp.actors.actor import Actor
 
 
 class ThreadActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/thread.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/thread.js"""
 
     class ResumeLimit(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/client/fronts/thread.js#L129
-        """
+        """https://github.com/mozilla/gecko-dev/blob/7ef5cefd0468b8f509efe38e0212de2398f4c8b3/devtools/client/fronts/thread.js#L129"""
+
         NONE = None
         BREAK = "break"
         NEXT = "next"
         STEP = "step"
         FINISH = "finish"
         RESTART = "restart"
 
     class When(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/f1451cbda60df2f90ed2d5637dcc38615019a07c/devtools/server/actors/thread.js#L1579
-        """
+        """https://github.com/mozilla/gecko-dev/blob/f1451cbda60df2f90ed2d5637dcc38615019a07c/devtools/server/actors/thread.js#L1579"""
+
         NOW = ""
         ON_NEXT = "onNext"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def attach(self,
-               pause_on_exceptions=False,
-               ignore_caught_exceptions=True,
-               should_show_overlay=False,
-               should_include_saved_frames=True,
-               should_include_async_live_frames=False,
-               skip_breakpoints=False,
-               log_event_breakpoints=False,
-               observe_asm_js=True,
-               breakpoints: dict | None = None,
-               event_breakpoints: list | None = None):
-        if (breakpoints is None):
+    def attach(
+        self,
+        pause_on_exceptions=False,
+        ignore_caught_exceptions=True,
+        should_show_overlay=False,
+        should_include_saved_frames=True,
+        should_include_async_live_frames=False,
+        skip_breakpoints=False,
+        log_event_breakpoints=False,
+        observe_asm_js=True,
+        breakpoints: dict | None = None,
+        event_breakpoints: list | None = None,
+    ):
+        if breakpoints is None:
             breakpoints = {}
-        if (event_breakpoints is None):
+        if event_breakpoints is None:
             event_breakpoints = []
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "attach",
-            "options": {
-                "pauseOnExceptions": pause_on_exceptions,
-                "ignoreCaughtExceptions": ignore_caught_exceptions,
-                "shouldShowOverlay": should_show_overlay,
-                "shouldIncludeSavedFrames": should_include_saved_frames,
-                "shouldIncludeAsyncLiveFrames": should_include_async_live_frames,
-                "skipBreakpoints": skip_breakpoints,
-                "logEventBreakpoints": log_event_breakpoints,
-                "observeAsmJS": observe_asm_js,
-                "breakpoints": breakpoints,
-                "eventBreakpoints": event_breakpoints,
-            },
-        })
-
-    def reconfigure(self,
-                    observe_asm_js=True,
-                    pause_workers_until_attach=True,
-                    skip_breakpoints: dict | None = None,
-                    log_event_breakpoints: list | None = None):
-        if (skip_breakpoints is None):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "attach",
+                "options": {
+                    "pauseOnExceptions": pause_on_exceptions,
+                    "ignoreCaughtExceptions": ignore_caught_exceptions,
+                    "shouldShowOverlay": should_show_overlay,
+                    "shouldIncludeSavedFrames": should_include_saved_frames,
+                    "shouldIncludeAsyncLiveFrames": should_include_async_live_frames,
+                    "skipBreakpoints": skip_breakpoints,
+                    "logEventBreakpoints": log_event_breakpoints,
+                    "observeAsmJS": observe_asm_js,
+                    "breakpoints": breakpoints,
+                    "eventBreakpoints": event_breakpoints,
+                },
+            }
+        )
+
+    def reconfigure(
+        self,
+        observe_asm_js=True,
+        pause_workers_until_attach=True,
+        skip_breakpoints: dict | None = None,
+        log_event_breakpoints: list | None = None,
+    ):
+        if skip_breakpoints is None:
             skip_breakpoints = {}
-        if (log_event_breakpoints is None):
+        if log_event_breakpoints is None:
             log_event_breakpoints = []
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "reconfigure",
-            "options": {
-                "observeAsmJS": observe_asm_js,
-                "pauseWorkersUntilAttach": pause_workers_until_attach,
-                "skipBreakpoints": skip_breakpoints,
-                "logEventBreakpoints": log_event_breakpoints,
-            },
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "reconfigure",
+                "options": {
+                    "observeAsmJS": observe_asm_js,
+                    "pauseWorkersUntilAttach": pause_workers_until_attach,
+                    "skipBreakpoints": skip_breakpoints,
+                    "logEventBreakpoints": log_event_breakpoints,
+                },
+            }
+        )
 
     def resume(self, resume_limit=ResumeLimit.NONE, frame_actor_id=""):
         args: Dict[str, Any] = {
             "to": self.actor_id,
             "type": "resume",
         }
-        if (resume_limit == ThreadActor.ResumeLimit.NONE):
+        if resume_limit == ThreadActor.ResumeLimit.NONE:
             args["resumeLimit"] = None
         else:
             args["resumeLimit"] = resume_limit.value
-        if (frame_actor_id != ""):
+        if frame_actor_id != "":
             args["frameActorID"] = frame_actor_id
         return self.client.send_receive(args)
 
     def frames(self, start: int, count: int):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "frames",
-            "start": start,
-            "count": count,
-        }, "frames")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "frames",
+                "start": start,
+                "count": count,
+            },
+            "frames",
+        )
 
     def interrupt(self, when=When.NOW):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "interrupt",
-            "when": when.value,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "interrupt",
+                "when": when.value,
+            }
+        )
 
     def sources(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "sources",
-        }, "sources")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "sources",
+            },
+            "sources",
+        )
 
     def skip_breakpoints(self, skip_breakpoints: dict | None = None):
-        if (skip_breakpoints is None):
+        if skip_breakpoints is None:
             skip_breakpoints = {}
         # todo couldn't find any correct usage
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "skipBreakpoints",
-            "skip": skip_breakpoints,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "skipBreakpoints",
+                "skip": skip_breakpoints,
+            }
+        )
 
     def dump_thread(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "dumpThread",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "dumpThread",
+            }
+        )
 
     def dump_pools(self):
         # todo response doesn't follow the usual structure
         # and won't work with rdpclient, maybe
         # firefox devs will change this in the future
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "dumpPools",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "dumpPools",
+            }
+        )
 
-    def set_breakpoint(self,
-                       line: int,
-                       column: int,
-                       source_url="",
-                       source_id="",
-                       condition="",
-                       log_value=""):
-        """ https://github.com/mozilla/gecko-dev/blob/f1451cbda60df2f90ed2d5637dcc38615019a07c/devtools/server/actors/thread.js#L568
-        """
+    def set_breakpoint(
+        self,
+        line: int,
+        column: int,
+        source_url="",
+        source_id="",
+        condition="",
+        log_value="",
+    ):
+        """https://github.com/mozilla/gecko-dev/blob/f1451cbda60df2f90ed2d5637dcc38615019a07c/devtools/server/actors/thread.js#L568"""
         args = {
             "to": self.actor_id,
             "type": "setBreakpoint",
             "location": {
                 "line": line,
                 "column": column,
             },
-            "options": {}
+            "options": {},
         }
-        if (source_url != ""):
+        if source_url != "":
             args["location"]["sourceUrl"] = source_url
-        if (source_id != ""):
+        if source_id != "":
             args["location"]["sourceId"] = source_id
-        if (condition != ""):
+        if condition != "":
             args["options"]["condition"] = condition
-        if (log_value != ""):
+        if log_value != "":
             args["options"]["logValue"] = log_value
         return self.client.send_receive(args)
 
-    def remove_breakpoint(self,
-                          line: int,
-                          column: int,
-                          source_url="",
-                          source_id=""):
+    def remove_breakpoint(self, line: int, column: int, source_url="", source_id=""):
         args = {
             "to": self.actor_id,
             "type": "removeBreakpoint",
             "location": {
                 "line": line,
                 "column": column,
-            }
+            },
         }
-        if (source_url != ""):
+        if source_url != "":
             args["location"]["sourceUrl"] = source_url
-        if (source_id != ""):
+        if source_id != "":
             args["location"]["sourceId"] = source_id
         return self.client.send_receive(args)
 
     def set_xhr_breakpoint(self, path: str, method="ANY"):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setXHRBreakpoint",
-            "path": path,
-            "method": method,
-        }, "value")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setXHRBreakpoint",
+                "path": path,
+                "method": method,
+            },
+            "value",
+        )
 
     def remove_xhr_breakpoint(self, path: str, method: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "removeXHRBreakpoint",
-            "path": path,
-            "method": method,
-        }, "value")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "removeXHRBreakpoint",
+                "path": path,
+                "method": method,
+            },
+            "value",
+        )
 
     def get_available_event_breakpoints(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getAvailableEventBreakpoints",
-        }, "value")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getAvailableEventBreakpoints",
+            },
+            "value",
+        )
 
     def get_active_event_breakpoints(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getActiveEventBreakpoints",
-        }, "ids")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getActiveEventBreakpoints",
+            },
+            "ids",
+        )
 
     def set_active_event_breakpoints(self, ids: list):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setActiveEventBreakpoints",
-            "ids": ids,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setActiveEventBreakpoints",
+                "ids": ids,
+            }
+        )
 
-    def pause_on_exceptions(self, pause_on_exceptions: str, ignore_caught_exceptions: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "pauseOnExceptions",
-            "pauseOnExceptions": pause_on_exceptions,
-            "ignoreCaughtExceptions": ignore_caught_exceptions,
-        })
+    def pause_on_exceptions(
+        self, pause_on_exceptions: str, ignore_caught_exceptions: str
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "pauseOnExceptions",
+                "pauseOnExceptions": pause_on_exceptions,
+                "ignoreCaughtExceptions": ignore_caught_exceptions,
+            }
+        )
 
     def toggle_event_logging(self, log_event_breakpoints: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "toggleEventLogging",
-            "logEventBreakpoints": log_event_breakpoints,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "toggleEventLogging",
+                "logEventBreakpoints": log_event_breakpoints,
+            }
+        )
 
     def is_attached(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "isAttached",
-        }, "value")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "isAttached",
+            },
+            "value",
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/events.py` & `geckordp-0.5.0/geckordp/actors/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,177 +1,181 @@
 from enum import Enum
 
 
-class Events():
-    """ A list of all events which can be received by the rdp server.
+class Events:
+    """A list of all events which can be received by the rdp server.
 
-        These events will be once registered in 'RDPClient' to handle responses.
+    These events will be once registered in 'RDPClient' to handle responses.
     """
 
     class Accessible(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L46
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L46"""
+
         ACTIONS_CHANGE = "actionsChange"
         NAME_CHANGE = "nameChange"
         VALUE_CHANGE = "valueChange"
         DESCRIPTION_CHANGE = "descriptionChange"
         STATES_CHANGE = "statesChange"
         ATTRIBUTES_CHANGE = "attributesChange"
         SHORTCUT_CHANGE = "shortcutChange"
         REORDER = "reorder"
         TEXT_CHANGE = "textChange"
         INDEX_IN_PARENT_CHANGE = "indexInParentChange"
         AUDITED = "audited"
 
     class AccessibleWalker(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L130
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L130"""
+
         DOCUMENT_READY = "documentReady"
         PICKER_ACCESSIBLE_PICKED = "pickerAccessiblePicked"
         PICKER_ACCESSIBLE_PREVIEWED = "pickerAccessiblePreviewed"
         PICKER_ACCESSIBLE_HOVERED = "pickerAccessibleHovered"
         PICKER_ACCESSIBLE_CANCELED = "pickerAccessibleCanceled"
         HIGHLIGHTER_EVENT = "highlighter-event"
         AUDIT_EVENT = "audit-event"
 
     class Accessibility(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L225
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L225"""
+
         INIT = "init"
         SHUTDOWN = "shutdown"
 
     class Browser(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/targets/window-global.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/targets/window-global.js"""
+
         TAB_NAVIGATED = "tabNavigated"
         FRAME_UPDATE = "frameUpdate"
         TAB_DETACHED = "tabDetached"
         WORKER_LIST_CHANGED = "workerListChanged"
 
     class ContentProcess(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/targets/content-process.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/targets/content-process.js"""
+
         WORKER_LIST_CHANGED = "workerListChanged"
         TAB_DETACHED = "tabDetached"
 
     class EventSource(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/eventsource.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/eventsource.js"""
+
         EVENT_SOURCE_CONNECTION_CLOSED = "eventSourceConnectionClosed"
         EVENT_RECEIVED = "eventReceived"
 
     class Inspector(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/inspector.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/inspector.js"""
+
         COLOR_PICKED = "colorPicked"
         COLOR_PICK_CANCELED = "colorPickCanceled"
 
     class Memory(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/memory.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/memory.js"""
+
         GARBAGE_COLLECTION = "garbage-collection"
         ALLOCATIONS = "allocations"
 
     class Network(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/network-event.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/network-event.js"""
+
         NETWORK_EVENT_UPDATE = "networkEventUpdate"
 
     class ParentAccessibility(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L263
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/accessibility.js#L263"""
+
         INIT = "canBeDisabledChange"
         SHUTDOWN = "canBeEnabledChange"
 
     class Performance(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/performance.js
-            deprecated
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/performance.js
+        deprecated
         """
+
         RECORDING_STARTED = "recording-started"
         RECORDING_STOPPING = "recording-stopping"
         RECORDING_STOPPED = "recording-stopped"
         PROFILER_STATUS = "profiler-status"
         CONSOLE_PROFILE_START = "console-profile-start"
         TIMELINE_DATA = "timeline-data"
 
     class Process(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/descriptors/process.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/descriptors/process.js"""
+
         DESCRIPTOR_DESTROYED = "descriptor-destroyed"
 
     class Root(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/root.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/root.js"""
+
         TAB_LIST_CHANGED = "tabListChanged"
         WORKER_LIST_CHANGED = "workerListChanged"
         ADDON_LIST_CHANGED = "addonListChanged"
-        SERVICE_WORKER_REGISTRATION_LIST_CHANGED = "serviceWorkerRegistrationListChanged"
+        SERVICE_WORKER_REGISTRATION_LIST_CHANGED = (
+            "serviceWorkerRegistrationListChanged"
+        )
         PROCESS_LIST_CHANGED = "processListChanged"
         # not listed event
         FORWARDING_CANCELLED = "forwardingCancelled"
 
     class Storage(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/storage.js"""
+
         STORES_UPDATE = "storesUpdate"
         STORES_CLEARED = "storesCleared"
         STORES_RELOADED = "storesReloaded"
 
     class Thread(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/thread.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/thread.js"""
+
         PAUSED = "paused"
         RESUMED = "resumed"
         WILL_INTERRUPT = "willInterrupt"
         NEW_SOURCE = "newSource"
 
     class Walker(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/walker.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/walker.js"""
+
         NEW_MUTATIONS = "newMutations"
         ROOT_AVAILABLE = "root-available"
         ROOT_DESTROYED = "root-destroyed"
         PICKER_NODE_PICKED = "pickerNodePicked"
         PICKER_NODE_PREVIEWED = "pickerNodePreviewed"
         PICKER_NODE_HOVERED = "pickerNodeHovered"
         PICKER_NODE_CANCELED = "pickerNodeCanceled"
         DISPLAY_CHANGE = "display-change"
         SCROLLABLE_CHANGE = "scrollable-change"
         OVERFLOW_CHANGE = "overflow-change"
         RESIZE = "resize"
 
     class Watcher(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/watcher.js
-            events reside in webconsole, however its origin (and its actor) comes actually from watcher
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/watcher.js
+        events reside in webconsole, however its origin (and its actor) comes actually from watcher
         """
+
         TARGET_AVAILABLE_FORM = "target-available-form"
         TARGET_DESTROYED_FORM = "target-destroyed-form"
         RESOURCE_AVAILABLE_FORM = "resource-available-form"
         RESOURCE_DESTROYED_FORM = "resource-destroyed-form"
         RESOURCE_UPDATED_FORM = "resource-updated-form"
 
     class WebConsole(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/webconsole.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/webconsole.js"""
+
         EVALUATION_RESULT = "evaluationResult"
         FILE_ACTIVITY = "fileActivity"
         PAGE_ERROR = "pageError"
         LOG_MESSAGE = "logMessage"
         CONSOLE_API_CALL = "consoleAPICall"
         REFLOW_ACTIVITY = "reflowActivity"
         NETWORK_EVENT = "networkEvent"
         INSPECT_OBJECT = "inspectObject"
         LAST_PRIVATE_CONTEXT_EXITED = "lastPrivateContextExited"
         DOCUMENT_EVENT = "documentEvent"
 
     class WebSocket(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/websocket.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/websocket.js"""
+
         WEB_SOCKET_OPENED = "webSocketOpened"
         WEB_SOCKET_CLOSED = "webSocketClosed"
         FRAME_RECEIVED = "frameReceived"
         FRAME_SENT = "frameSent"
 
     class Worker(str, Enum):
-        """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/descriptors/worker.js
-        """
+        """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/descriptors/worker.js"""
+
         DESCRIPTOR_DESTROYED = "descriptor-destroyed"
```

## Comparing `geckordp-0.4.53/geckordp/actors/network_parent.py` & `geckordp-0.5.0/geckordp/actors/network_parent.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,97 @@
 from typing import List
+
 from geckordp.actors.actor import Actor
 
 
 class NetworkParentActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/network-parent.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/network-parent.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def set_persist(self, enabled: bool):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setPersist",
-            "options": enabled,
-        })
-
-    def set_network_throttling(self, download_throughput: int, upload_throughput: int, latency_ms: int):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setNetworkThrottling",
-            "options": {
-                "downloadThroughput": download_throughput,
-                "uploadThroughput": upload_throughput,
-                "latency": latency_ms
-            },
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setPersist",
+                "options": enabled,
+            }
+        )
+
+    def set_network_throttling(
+        self,
+        download_throughput: int,
+        upload_throughput: int,
+        latency_ms: int,
+    ):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setNetworkThrottling",
+                "options": {
+                    "downloadThroughput": download_throughput,
+                    "uploadThroughput": upload_throughput,
+                    "latency": latency_ms,
+                },
+            }
+        )
 
     def get_network_throttling(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getNetworkThrottling",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getNetworkThrottling",
+            }
+        )
 
     def clear_network_throttling(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "clearNetworkThrottling",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "clearNetworkThrottling",
+            }
+        )
 
     def set_save_request_and_response_bodies(self, save: bool):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setSaveRequestAndResponseBodies",
-            "save": save,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setSaveRequestAndResponseBodies",
+                "save": save,
+            }
+        )
 
     def set_blocked_urls(self, urls: List[str]):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "setBlockedUrls",
-            "urls": urls,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "setBlockedUrls",
+                "urls": urls,
+            }
+        )
 
     def get_blocked_urls(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getBlockedUrls",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getBlockedUrls",
+            }
+        )
 
     def block_request(self, filters: dict):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "blockRequest",
-            "filters": filters,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "blockRequest",
+                "filters": filters,
+            }
+        )
 
     def unblock_request(self, filters: dict):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "unblockRequest",
-            "filters": filters,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "unblockRequest",
+                "filters": filters,
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/target_configuration.py` & `geckordp-0.5.0/geckordp/actors/target_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,71 @@
 from geckordp.actors.actor import Actor
 
 
 class TargetConfigurationActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/target-configuration.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/target-configuration.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def update_configuration(self,
-                             cache_disabled: bool | None = None,
-                             color_scheme_simulation: bool | None = None,
-                             custom_user_agent="",
-                             javascript_enabled: bool | None = None,
-                             override_dppx=-1,
-                             paint_flashing: bool | None = None,
-                             print_simulation_enabled: bool | None = None,
-                             restore_focus: bool | None = None,
-                             service_workers_testing_enabled: bool | None = None,
-                             touch_events_override=""):
+    def update_configuration(
+        self,
+        cache_disabled: bool | None = None,
+        custom_formatters: bool | None = None,
+        color_scheme_simulation: bool | None = None,
+        custom_user_agent="",
+        javascript_enabled: bool | None = None,
+        override_dppx=-1,
+        paint_flashing: bool | None = None,
+        print_simulation_enabled: bool | None = None,
+        restore_focus: bool | None = None,
+        service_workers_testing_enabled: bool | None = None,
+        use_simple_highlighters_for_reduced_motion: bool | None = None,
+        touch_events_override="",
+    ):
         args = {}
 
-        if (cache_disabled is not None):
+        if cache_disabled is not None:
             args["cacheDisabled"] = cache_disabled
 
-        if (color_scheme_simulation is not None):
+        if custom_formatters is not None:
+            args["customFormatters"] = custom_formatters
+
+        if color_scheme_simulation is not None:
             args["colorSchemeSimulation"] = color_scheme_simulation
 
-        if (custom_user_agent != ""):
+        if custom_user_agent != "":
             args["customUserAgent"] = custom_user_agent
 
-        if (javascript_enabled is not None):
+        if javascript_enabled is not None:
             args["javascriptEnabled"] = javascript_enabled
 
-        if (override_dppx != -1):
+        if override_dppx != -1:
             args["overrideDPPX"] = override_dppx
 
-        if (paint_flashing is not None):
+        if paint_flashing is not None:
             args["paintFlashing"] = paint_flashing
 
-        if (print_simulation_enabled is not None):
+        if print_simulation_enabled is not None:
             args["printSimulationEnabled"] = print_simulation_enabled
 
-        if (restore_focus is not None):
+        if restore_focus is not None:
             args["restoreFocus"] = restore_focus
 
-        if (service_workers_testing_enabled is not None):
+        if service_workers_testing_enabled is not None:
             args["serviceWorkersTestingEnabled"] = service_workers_testing_enabled
 
-        if (touch_events_override != ""):
+        if use_simple_highlighters_for_reduced_motion is not None:
+            args["useSimpleHighlightersForReducedMotion"] = (
+                use_simple_highlighters_for_reduced_motion
+            )
+
+        if touch_events_override != "":
             args["touchEventsOverride"] = touch_events_override
 
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "updateConfiguration",
-            "configuration": args,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "updateConfiguration",
+                "configuration": args,
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/targets/window_global.py` & `geckordp-0.5.0/geckordp/actors/watcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,86 @@
-from geckordp.actors.actor import Actor
+from enum import Enum
 
+from geckordp.actors.resources import ResourceActor
 
-class WindowGlobalActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/c07fae4f8a15991f019d70cd7b9900338d72eba2/devtools/shared/specs/targets/browsing-context.js
-        https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/targets/window-global.js
-    """
+
+class WatcherActor(ResourceActor):
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/watcher.js"""
+
+    class Targets(str, Enum):
+        """https://github.com/mozilla/gecko-dev/blob/6178b9bfde68881523a8a30bbc0b78eac1f95159/devtools/server/actors/targets/index.js#L7"""
+
+        FRAME = "frame"
+        PROCESS = "process"
+        WORKER = "worker"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def detach(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "detach",
-        })
-
-    def focus(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "focus",
-        })
-
-    def go_forward(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "goForward",
-        })
-
-    def go_back(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "goBack",
-        })
-
-    def reload(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "reload",
-        })
-
-    def navigate_to(self, url: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "navigateTo",
-            "url": url,
-        })
-
-    def switch_to_frame(self, window_id: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "switchToFrame",
-            "windowId": window_id,
-        })
-
-    def list_frames(self):
-        # todo: replace with extract expression
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "listFrames",
-        })["frames"]  # type: ignore
-
-    def list_workers(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "listWorkers",
-        })
-
-    def log_in_page(self, text="", category="", flags=""):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "logInPage",
-            "text": text,
-            "category": category,
-            "flags": flags,
-        })
+    def watch_targets(self, target: Targets):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "watchTargets",
+                "targetType": str(target.value),
+            }
+        )
+
+    def unwatch_targets(self, target: Targets):
+        self.client.send(
+            {
+                "to": self.actor_id,
+                "type": "unwatchTargets",
+                "targetType": str(target.value),
+            }
+        )
+
+    def get_parent_browsing_context_id(self, ctx_id: int):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getParentBrowsingContextID",
+                "browsingContextID": ctx_id,
+            }
+        )
+
+    def get_network_parent_actor(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getNetworkParentActor",
+            }
+        )
+
+    def get_blackboxing_actor(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getBlackboxingActor",
+            }
+        )
+
+    def get_breakpoint_list_actor(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getBreakpointListActor",
+            }
+        )
+
+    def get_target_configuration_actor(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getTargetConfigurationActor",
+            },
+            "configuration",
+        )
+
+    def get_thread_configuration_actor(self):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getThreadConfigurationActor",
+            },
+            "configuration",
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/targets/content_process.py` & `geckordp-0.5.0/geckordp/actors/targets/content_process.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from geckordp.actors.actor import Actor
 
 
 class ContentProcessActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/targets/content-process.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/targets/content-process.js"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def list_workers(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "listWorkers",
-        }, "workers")
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "listWorkers",
+            },
+            "workers",
+        )
 
-    def pause_matching_service_workers(self, origin = ""):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "pauseMatchingServiceWorkers",
-            "origin": origin,
-        })
+    def pause_matching_service_workers(self, origin=""):
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "pauseMatchingServiceWorkers",
+                "origin": origin,
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp/actors/inspector.py` & `geckordp-0.5.0/geckordp/actors/inspector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from enum import Enum
 from typing import Any, Dict
+
 from geckordp.actors.actor import Actor
 
 
 class InspectorActor(Actor):
-    """ https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/inspector.js
-    """
+    """https://github.com/mozilla/gecko-dev/blob/master/devtools/shared/specs/inspector.js"""
 
     class Highlighters(str, Enum):
-        """ https://firefox-source-docs.mozilla.org/devtools/tools/highlighters.html#using-highlighters
-        """
+        """https://firefox-source-docs.mozilla.org/devtools/tools/highlighters.html#using-highlighters"""
+
         CSS_GRID_HIGHLIGHTER = "CssGridHighlighter"
         BOX_MODEL_HIGHLIGHTER = "BoxModelHighlighter"
         CSS_TRANSFORM_HIGHLIGHTER = "CssTransformHighlighter"
         FLEXBOX_HIGHLIGHTER = "FlexboxHighlighter"
         FONTS_HIGHLIGHTER = "FontsHighlighter"
         GEOMETRY_EDITOR_HIGHLIGHTER = "GeometryEditorHighlighter"
         MEASURING_TOOL_HIGHLIGHTER = "MeasuringToolHighlighter"
@@ -22,72 +22,88 @@
         SELECTOR_HIGHLIGHTER = "SelectorHighlighter"
         SHAPES_HIGHLIGHTER = "ShapesHighlighter"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def get_walker(self, options_json: dict | None = None):
-        if (options_json is None):
+        if options_json is None:
             options_json = {}
-        response = self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getWalker",
-            "options": options_json,
-        })
+        response = self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getWalker",
+                "options": options_json,
+            }
+        )
         # todo: replace with extract expression
         return response.get("walker", response)  # type: ignore
 
     def get_page_style(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getPageStyle",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getPageStyle",
+            }
+        )
 
     def get_compatibility(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getCompatibility",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getCompatibility",
+            }
+        )
 
     def get_highlighter_by_type(self, hightligher_type: Highlighters):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "getHighlighterByType",
-            "typeName": hightligher_type.value,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "getHighlighterByType",
+                "typeName": hightligher_type.value,
+            }
+        )
 
     def get_image_data_from_url(self, url: str, max_dim=0):
         args: Dict[str, Any] = {
             "to": self.actor_id,
             "type": "getImageDataFromURL",
             "url": url,
         }
-        if (max_dim > 0):
+        if max_dim > 0:
             args["maxDim"] = max_dim
         return self.client.send_receive(args)
 
     def resolve_relative_url(self, url: str, dom_node_actor: str):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "resolveRelativeURL",
-            "url": url,
-            "node": dom_node_actor,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "resolveRelativeURL",
+                "url": url,
+                "node": dom_node_actor,
+            }
+        )
 
     def pick_color_from_page(self, options_json: dict):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "pickColorFromPage",
-            "options": options_json,
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "pickColorFromPage",
+                "options": options_json,
+            }
+        )
 
     def cancel_pick_color_from_page(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "cancelPickColorFromPage",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "cancelPickColorFromPage",
+            }
+        )
 
     def supports_highlighters(self):
-        return self.client.send_receive({
-            "to": self.actor_id,
-            "type": "supportsHighlighters",
-        })
+        return self.client.send_receive(
+            {
+                "to": self.actor_id,
+                "type": "supportsHighlighters",
+            }
+        )
```

## Comparing `geckordp-0.4.53/geckordp.egg-info/PKG-INFO` & `geckordp-0.5.0/geckordp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geckordp
-Version: 0.4.53
+Version: 0.5.0
 Summary: A client implementation of Firefox DevTools over remote debug protocol
 Home-page: https://github.com/jpramosi/geckordp
 Author: jpramosi
 Author-email: jimmy.pramosi@protonmail.com
 License: MIT
 Project-URL: Documentation, https://jpramosi.github.io/geckordp
 Project-URL: Source, https://github.com/jpramosi/geckordp
@@ -75,70 +75,68 @@
 ```
 
 ## Usage
 <!-- SEPARATOR -->
 
 ```python
 import json
-from geckordp.rdp_client import RDPClient
+
 from geckordp.actors.root import RootActor
-from geckordp.profile import ProfileManager
 from geckordp.firefox import Firefox
-
+from geckordp.profile import ProfileManager
+from geckordp.rdp_client import RDPClient
 
 """ Uncomment to enable debug output
 """
-#from geckordp.settings import GECKORDP
-#GECKORDP.DEBUG = 1
-#GECKORDP.DEBUG_REQUEST = 1
-#GECKORDP.DEBUG_RESPONSE = 1
+# from geckordp.settings import GECKORDP
+# GECKORDP.DEBUG = 1
+# GECKORDP.DEBUG_REQUEST = 1
+# GECKORDP.DEBUG_RESPONSE = 1
 
 
 def main():
     # clone default profile to 'geckordp'
     pm = ProfileManager()
     profile_name = "geckordp"
     port = 6000
     pm.clone("default-release", profile_name)
     profile = pm.get_profile_by_name(profile_name)
     profile.set_required_configs()
 
     # start firefox with specified profile
-    Firefox.start("https://example.com/",
-                  port,
-                  profile_name,
-                  ["-headless"])
+    Firefox.start("https://example.com/", port, profile_name, ["-headless"])
 
     # create client and connect to firefox
     client = RDPClient()
     client.connect("localhost", port)
 
     # initialize root
     root = RootActor(client)
 
     # get a list of tabs
     tabs = root.list_tabs()
     print(json.dumps(tabs, indent=2))
 
     input()
 
+
 if __name__ == "__main__":
     main()
 ```
 See also [examples](https://jpramosi.github.io/geckordp/examples/modules.html) and [tests](https://github.com/jpramosi/geckordp/tree/master/tests/actors).
 
 
 ## Tested Platforms
 <!-- SEPARATOR -->
 
 | Tested Platform                            | Working                 | Firefox-Version         | Geckordp-Version        |
 | -------------------------------------------| ------------------------| ------------------------| ------------------------|
-| Windows (x64)                              | yes                     |  113.0                   |  0.4.53                  |
-| Ubuntu 20.04                               | yes                     |  113.0                   |  0.4.53                  |
-| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  113.0                   |  0.4.53                  |
+| Windows (x64)                              | yes                     |  113.0                   |  0.5.0                  |
+| Ubuntu 20.04                               | yes                     |  113.0                   |  0.5.0                  |
+| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  113.0                   |  0.5.0                  |
 
 Geckordp requires minimum Python 3.10 and the latest Firefox build. Older versions of Firefox may also work as long the API changes are not too drastically. In case of doubt, clone and run tests with:
 ```bash
 cd <your-repositories-path>
 git clone https://github.com/jpramosi/geckordp
 cd geckordp
 python -m pip uninstall geckordp
@@ -294,15 +292,15 @@
 
 
 ## License
 <!-- SEPARATOR -->
 ```
 MIT License
 
-Copyright (c) 2023 jpramosi
+Copyright (c) 2024 jpramosi
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

## Comparing `geckordp-0.4.53/geckordp.egg-info/SOURCES.txt` & `geckordp-0.5.0/geckordp.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 geckordp/actors/memory.py
 geckordp/actors/network_content.py
 geckordp/actors/network_event.py
 geckordp/actors/network_parent.py
 geckordp/actors/node.py
 geckordp/actors/node_list.py
 geckordp/actors/preference.py
+geckordp/actors/resources.py
 geckordp/actors/root.py
 geckordp/actors/screenshot.py
 geckordp/actors/source.py
 geckordp/actors/storage.py
 geckordp/actors/string.py
 geckordp/actors/target_configuration.py
 geckordp/actors/thread.py
+geckordp/actors/thread_configuration.py
 geckordp/actors/walker.py
 geckordp/actors/watcher.py
 geckordp/actors/web_console.py
-geckordp/actors/web_socket.py
 geckordp/actors/accessibility/__init__.py
 geckordp/actors/accessibility/accessibility.py
 geckordp/actors/accessibility/accessible.py
 geckordp/actors/accessibility/accessible_walker.py
 geckordp/actors/accessibility/parent_accessibility.py
 geckordp/actors/accessibility/simulator.py
 geckordp/actors/addon/__init__.py
@@ -71,15 +72,17 @@
 tests/actors/test_source.py
 tests/actors/test_storage_cache.py
 tests/actors/test_storage_cookie.py
 tests/actors/test_storage_extension.py
 tests/actors/test_storage_indexed.py
 tests/actors/test_storage_local.py
 tests/actors/test_storage_session.py
+tests/actors/test_target_configuration.py
 tests/actors/test_thread.py
+tests/actors/test_thread_configuration.py
 tests/actors/test_walker.py
 tests/actors/test_watcher.py
 tests/actors/test_web_console.py
 tests/actors/accessibility/__init__.py
 tests/actors/accessibility/test_accessibility.py
 tests/actors/accessibility/test_accessible.py
 tests/actors/accessibility/test_accessible_walker.py
```

## Comparing `geckordp-0.4.53/setup.py` & `geckordp-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 NAME = "geckordp"
 EMAIL = "jimmy.pramosi@protonmail.com"
-__version__ = "0.4.53"
+__version__ = "0.5.0"
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 10)
 
 # check version
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     sys.stderr.write(
         """
@@ -25,17 +26,19 @@
         )
     )
     sys.exit(1)
 
 # set metadata
 URL = "https://github.com/jpramosi/geckordp"
 DESCRIPTION = "A client implementation of Firefox DevTools over remote debug protocol"
-LONG_DESCRIPTION = open('README.md', 'r', encoding='utf-8').read()
+LONG_DESCRIPTION = open("README.md", "r", encoding="utf-8").read()
 LONG_DESCRIPTION = LONG_DESCRIPTION.replace(
-    '<img src="actor-hierarchy.png">', "![](https://raw.githubusercontent.com/jpramosi/geckordp/master/actor-hierarchy.png)")
+    '<img src="actor-hierarchy.png">',
+    "![](https://raw.githubusercontent.com/jpramosi/geckordp/master/actor-hierarchy.png)",
+)
 classifiers = [
     # http://www.python.org/pypi?%3Aaction=list_classifiers
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -45,23 +48,23 @@
 
 # install package itself
 setup(
     name=NAME,
     version=__version__,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     classifiers=classifiers,
     keywords="rdp remote-debug-protocol firefox crawler debug webconsole ui-testing",
     author="jpramosi",
     author_email=EMAIL,
     url=URL,
     project_urls={
-        'Documentation': 'https://jpramosi.github.io/geckordp',
-        'Source': URL,
+        "Documentation": "https://jpramosi.github.io/geckordp",
+        "Source": URL,
     },
     extras_require={
         "develop": [
             "pytest",
             "twine",
             "ipython",
             "scapy",
```

## Comparing `geckordp-0.4.53/PKG-INFO` & `geckordp-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geckordp
-Version: 0.4.53
+Version: 0.5.0
 Summary: A client implementation of Firefox DevTools over remote debug protocol
 Home-page: https://github.com/jpramosi/geckordp
 Author: jpramosi
 Author-email: jimmy.pramosi@protonmail.com
 License: MIT
 Project-URL: Documentation, https://jpramosi.github.io/geckordp
 Project-URL: Source, https://github.com/jpramosi/geckordp
@@ -75,70 +75,68 @@
 ```
 
 ## Usage
 <!-- SEPARATOR -->
 
 ```python
 import json
-from geckordp.rdp_client import RDPClient
+
 from geckordp.actors.root import RootActor
-from geckordp.profile import ProfileManager
 from geckordp.firefox import Firefox
-
+from geckordp.profile import ProfileManager
+from geckordp.rdp_client import RDPClient
 
 """ Uncomment to enable debug output
 """
-#from geckordp.settings import GECKORDP
-#GECKORDP.DEBUG = 1
-#GECKORDP.DEBUG_REQUEST = 1
-#GECKORDP.DEBUG_RESPONSE = 1
+# from geckordp.settings import GECKORDP
+# GECKORDP.DEBUG = 1
+# GECKORDP.DEBUG_REQUEST = 1
+# GECKORDP.DEBUG_RESPONSE = 1
 
 
 def main():
     # clone default profile to 'geckordp'
     pm = ProfileManager()
     profile_name = "geckordp"
     port = 6000
     pm.clone("default-release", profile_name)
     profile = pm.get_profile_by_name(profile_name)
     profile.set_required_configs()
 
     # start firefox with specified profile
-    Firefox.start("https://example.com/",
-                  port,
-                  profile_name,
-                  ["-headless"])
+    Firefox.start("https://example.com/", port, profile_name, ["-headless"])
 
     # create client and connect to firefox
     client = RDPClient()
     client.connect("localhost", port)
 
     # initialize root
     root = RootActor(client)
 
     # get a list of tabs
     tabs = root.list_tabs()
     print(json.dumps(tabs, indent=2))
 
     input()
 
+
 if __name__ == "__main__":
     main()
 ```
 See also [examples](https://jpramosi.github.io/geckordp/examples/modules.html) and [tests](https://github.com/jpramosi/geckordp/tree/master/tests/actors).
 
 
 ## Tested Platforms
 <!-- SEPARATOR -->
 
 | Tested Platform                            | Working                 | Firefox-Version         | Geckordp-Version        |
 | -------------------------------------------| ------------------------| ------------------------| ------------------------|
-| Windows (x64)                              | yes                     |  113.0                   |  0.4.53                  |
-| Ubuntu 20.04                               | yes                     |  113.0                   |  0.4.53                  |
-| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  113.0                   |  0.4.53                  |
+| Windows (x64)                              | yes                     |  113.0                   |  0.5.0                  |
+| Ubuntu 20.04                               | yes                     |  113.0                   |  0.5.0                  |
+| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  113.0                   |  0.5.0                  |
 
 Geckordp requires minimum Python 3.10 and the latest Firefox build. Older versions of Firefox may also work as long the API changes are not too drastically. In case of doubt, clone and run tests with:
 ```bash
 cd <your-repositories-path>
 git clone https://github.com/jpramosi/geckordp
 cd geckordp
 python -m pip uninstall geckordp
@@ -294,15 +292,15 @@
 
 
 ## License
 <!-- SEPARATOR -->
 ```
 MIT License
 
-Copyright (c) 2023 jpramosi
+Copyright (c) 2024 jpramosi
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

## Comparing `geckordp-0.4.53/README.md` & `geckordp-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,70 +53,68 @@
 ```
 
 ## Usage
 <!-- SEPARATOR -->
 
 ```python
 import json
-from geckordp.rdp_client import RDPClient
+
 from geckordp.actors.root import RootActor
-from geckordp.profile import ProfileManager
 from geckordp.firefox import Firefox
-
+from geckordp.profile import ProfileManager
+from geckordp.rdp_client import RDPClient
 
 """ Uncomment to enable debug output
 """
-#from geckordp.settings import GECKORDP
-#GECKORDP.DEBUG = 1
-#GECKORDP.DEBUG_REQUEST = 1
-#GECKORDP.DEBUG_RESPONSE = 1
+# from geckordp.settings import GECKORDP
+# GECKORDP.DEBUG = 1
+# GECKORDP.DEBUG_REQUEST = 1
+# GECKORDP.DEBUG_RESPONSE = 1
 
 
 def main():
     # clone default profile to 'geckordp'
     pm = ProfileManager()
     profile_name = "geckordp"
     port = 6000
     pm.clone("default-release", profile_name)
     profile = pm.get_profile_by_name(profile_name)
     profile.set_required_configs()
 
     # start firefox with specified profile
-    Firefox.start("https://example.com/",
-                  port,
-                  profile_name,
-                  ["-headless"])
+    Firefox.start("https://example.com/", port, profile_name, ["-headless"])
 
     # create client and connect to firefox
     client = RDPClient()
     client.connect("localhost", port)
 
     # initialize root
     root = RootActor(client)
 
     # get a list of tabs
     tabs = root.list_tabs()
     print(json.dumps(tabs, indent=2))
 
     input()
 
+
 if __name__ == "__main__":
     main()
 ```
 See also [examples](https://jpramosi.github.io/geckordp/examples/modules.html) and [tests](https://github.com/jpramosi/geckordp/tree/master/tests/actors).
 
 
 ## Tested Platforms
 <!-- SEPARATOR -->
 
 | Tested Platform                            | Working                 | Firefox-Version         | Geckordp-Version        |
 | -------------------------------------------| ------------------------| ------------------------| ------------------------|
-| Windows (x64)                              | yes                     |  113.0                   |  0.4.53                  |
-| Ubuntu 20.04                               | yes                     |  113.0                   |  0.4.53                  |
-| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  113.0                   |  0.4.53                  |
+| Windows (x64)                              | yes                     |  113.0                   |  0.5.0                  |
+| Ubuntu 20.04                               | yes                     |  113.0                   |  0.5.0                  |
+| macOS 12                                   | [?](https://github.com/jpramosi/geckordp/issues/new)                       |  113.0                   |  0.5.0                  |
 
 Geckordp requires minimum Python 3.10 and the latest Firefox build. Older versions of Firefox may also work as long the API changes are not too drastically. In case of doubt, clone and run tests with:
 ```bash
 cd <your-repositories-path>
 git clone https://github.com/jpramosi/geckordp
 cd geckordp
 python -m pip uninstall geckordp
@@ -272,15 +270,15 @@
 
 
 ## License
 <!-- SEPARATOR -->
 ```
 MIT License
 
-Copyright (c) 2023 jpramosi
+Copyright (c) 2024 jpramosi
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

## Comparing `geckordp-0.4.53/tests/actors/test_storage_cookie.py` & `geckordp-0.5.0/tests/actors/test_storage_cookie.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 # pylint: disable=unused-import
 from concurrent.futures import Future
+
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.events import Events
-from geckordp.actors.watcher import WatcherActor
+from geckordp.actors.resources import Resources
+from geckordp.actors.root import RootActor
 from geckordp.actors.storage import CookieStorageActor
+from geckordp.actors.watcher import WatcherActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     watcher_ctx = tab.get_watcher()
-    watcher = WatcherActor(
-        cl, watcher_ctx["actor"])
+    watcher = WatcherActor(cl, watcher_ctx["actor"])
 
     resource = {}
     fut = Future()
 
     async def on_resource(data: dict):
         resources = data.get("resources", [])
         for resource in resources:
-            if ("cookie" in resource.get("actor", "")):
+            if "cookie" in resource.get("actor", ""):
                 fut.set_result(resource)
 
     cl.add_event_listener(
-        watcher.actor_id, Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource)
+        watcher.actor_id, Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource
+    )
 
     watcher.watch_targets(WatcherActor.Targets.FRAME)
-    watcher.watch_resources([WatcherActor.Resources.COOKIE])
+    watcher.watch_resources([Resources.COOKIE])
 
     resource = fut.result(3.0)
     assert "actor" in resource
 
     storage_actor_id = resource.get("actor", "")
     cookie = CookieStorageActor(cl, storage_actor_id)
```

## Comparing `geckordp-0.4.53/tests/actors/test_source.py` & `geckordp-0.5.0/tests/actors/test_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
+from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.root import RootActor
-from geckordp.actors.thread import ThreadActor
 from geckordp.actors.source import SourceActor
-from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.thread import ThreadActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     actor_ids = tab.get_target()
-    thread = ThreadActor(
-        cl, actor_ids["threadActor"])
+    thread = ThreadActor(cl, actor_ids["threadActor"])
     thread.attach()
     sources = thread.sources()
     source = None
     for s in sources:
-        if (s.get("actor", None) is not None):
+        if s.get("actor", None) is not None:
             source = SourceActor(cl, s["actor"])
             break
-    if (source is None):
+    if source is None:
         print("WARNING: no source available")
     return cl, source
 
 
 def test_get_breakpoint_positions():
     cl = None
     try:
         cl, source = init()
-        if (source is None):
+        if source is None:
             return
         val = source.get_breakpoint_positions()
         assert len(val) > 0
     finally:
         cl.disconnect()
 
 
 def test_get_breakpoint_positions_compressed():
     cl = None
     try:
         cl, source = init()
-        if (source is None):
+        if source is None:
             return
         val = source.get_breakpoint_positions_compressed()
         assert len(val) > 0
     finally:
         cl.disconnect()
 
 
 def test_get_breakable_lines():
     cl = None
     try:
         cl, source = init()
-        if (source is None):
+        if source is None:
             return
         val = source.get_breakable_lines()
         assert len(val) > 0
     finally:
         cl.disconnect()
 
 
 def test_source():
     cl = None
     try:
         cl, source = init()
-        if (source is None):
+        if source is None:
             return
         val = source.source()["source"]
         assert len(val) > 3
     finally:
         cl.disconnect()
 
 
 def test_set_pause_point():
     cl = None
     try:
         cl, source = init()
-        if (source is None):
+        if source is None:
             return
         val = source.set_pause_point(0, 0)
         assert response_valid("source", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_blackbox():
     cl = None
     try:
         cl, source = init()
-        if (source is None):
+        if source is None:
             return
         val = source.blackbox(0, 0, 10000, 0).get("pausedInSource", "0")
         assert val != "0"
     finally:
         cl.disconnect()
 
 
 def test_unblackbox():
     cl = None
     try:
         cl, source = init()
-        if (source is None):
+        if source is None:
             return
         val = source.unblackbox(0, 0, 10000, 0)
         assert response_valid("source", val), str(val)
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.53/tests/actors/test_node.py` & `geckordp-0.5.0/tests/actors/test_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
-from geckordp.actors.node import NodeActor
 from geckordp.actors.inspector import InspectorActor
+from geckordp.actors.node import NodeActor
+from geckordp.actors.root import RootActor
 from geckordp.actors.walker import WalkerActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
```

## Comparing `geckordp-0.4.53/tests/actors/test_inspector.py` & `geckordp-0.5.0/tests/actors/test_inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.inspector import InspectorActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
@@ -51,48 +52,48 @@
 
 
 def test_get_highlighter_by_type():
     cl = None
     try:
         cl, inspector = init()
         val = inspector.get_highlighter_by_type(
-            InspectorActor.Highlighters.SELECTOR_HIGHLIGHTER)
+            InspectorActor.Highlighters.SELECTOR_HIGHLIGHTER
+        )
         assert response_valid("inspector", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_get_image_data_from_url():
     cl = None
     try:
         cl, inspector = init()
         val = inspector.get_image_data_from_url(
-            "https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/Example.jpg/116px-Example.jpg")["data"]["length"]
+            "https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/Example.jpg/116px-Example.jpg"
+        )["data"]["length"]
         assert int(val) >= 0
     finally:
         cl.disconnect()
 
 
 def test_resolve_relative_url():
     cl = None
     try:
         cl, inspector = init()
-        val = inspector.resolve_relative_url(
-            "https://duckduckgo.com/", "")["value"]
+        val = inspector.resolve_relative_url("https://duckduckgo.com/", "")["value"]
         assert val == "https://duckduckgo.com/"
     finally:
         cl.disconnect()
 
 
 def test_pick_color_from_page():
     cl = None
     try:
         cl, inspector = init()
-        val = inspector.pick_color_from_page(
-            {"copyOnSelect": True, "fromMenu": True})
+        val = inspector.pick_color_from_page({"copyOnSelect": True, "fromMenu": True})
         assert response_valid("inspectorActor", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_cancel_pick_color_from_page():
     cl = None
```

## Comparing `geckordp-0.4.53/tests/actors/test_root.py` & `geckordp-0.5.0/tests/actors/test_root.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
 from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     return cl, root
@@ -59,15 +60,15 @@
 
 
 def test_list_workers():
     cl = None
     try:
         cl, root = init()
         workers = root.list_workers()
-        assert len(workers) >= 2
+        assert len(workers) >= 1
         val = workers[0]["actor"]
         assert "server" in val and "conn" in val and "workerDescriptor" in val
     finally:
         cl.disconnect()
 
 
 def test_list_service_worker_registrations():
```

## Comparing `geckordp-0.4.53/tests/actors/test_memory.py` & `geckordp-0.5.0/tests/actors/test_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.memory import MemoryActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
```

## Comparing `geckordp-0.4.53/tests/actors/accessibility/test_simulator.py` & `geckordp-0.5.0/tests/actors/accessibility/test_simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
-from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.accessibility.accessibility import AccessibilityActor
-from geckordp.actors.accessibility.simulator import SimulatorActor
 from geckordp.actors.accessibility.parent_accessibility import ParentAccessibilityActor
+from geckordp.actors.accessibility.simulator import SimulatorActor
+from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     actor_ids = tab.get_target()
     root_ids = root.get_root()
     accessibility = AccessibilityActor(cl, actor_ids["accessibilityActor"])
     simulator_id = accessibility.get_simulator().get("actor", None)
-    if (simulator_id is None):
+    if simulator_id is None:
         log("No simulator actor found, firefox is probably running in headless mode")
         return cl, None
     simulator = SimulatorActor(cl, simulator_id)
     accessibility.bootstrap()
-    parent = ParentAccessibilityActor(
-        cl, root_ids["parentAccessibilityActor"])
+    parent = ParentAccessibilityActor(cl, root_ids["parentAccessibilityActor"])
     parent.bootstrap()
     parent.enable()
     return cl, simulator
 
 
 def test_simulate():
     cl = None
     try:
         cl, simulator = init()
-        if (simulator is None):
+        if simulator is None:
             return
         val = simulator.simulate(SimulatorActor.Types.PROTANOPIA)
         assert val.get("value", None) is not None
         val = simulator.simulate(SimulatorActor.Types.NONE)
         assert val.get("value", None) is not None
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.53/tests/actors/accessibility/test_parent_accessibility.py` & `geckordp-0.5.0/tests/actors/accessibility/test_parent_accessibility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
-from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.accessibility.parent_accessibility import ParentAccessibilityActor
+from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     root_ids = root.get_root()
-    accessibility = ParentAccessibilityActor(
-        cl, root_ids["parentAccessibilityActor"])
+    accessibility = ParentAccessibilityActor(cl, root_ids["parentAccessibilityActor"])
     accessibility.bootstrap()
     return cl, accessibility
 
 
 def test_bootstrap():
     cl = None
     try:
```

## Comparing `geckordp-0.4.53/tests/actors/accessibility/test_accessible.py` & `geckordp-0.5.0/tests/actors/accessibility/test_accessible.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
-from geckordp.actors.descriptors.tab import TabActor
-from geckordp.actors.accessibility.accessible import AccessibleActor
 from geckordp.actors.accessibility.accessibility import AccessibilityActor
+from geckordp.actors.accessibility.accessible import AccessibleActor
 from geckordp.actors.accessibility.accessible_walker import AccessibleWalkerActor
 from geckordp.actors.accessibility.parent_accessibility import ParentAccessibilityActor
+from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     actor_ids = tab.get_target()
     root_ids = root.get_root()
     accessibility = AccessibilityActor(cl, actor_ids["accessibilityActor"])
     accessibility.bootstrap()
-    parent = ParentAccessibilityActor(
-        cl, root_ids["parentAccessibilityActor"])
+    parent = ParentAccessibilityActor(cl, root_ids["parentAccessibilityActor"])
     parent.bootstrap()
     parent.enable()
 
-    walker = AccessibleWalkerActor(cl,
-                                   accessibility.get_walker()["actor"])
+    walker = AccessibleWalkerActor(cl, accessibility.get_walker()["actor"])
     children = walker.children()
 
     accessible = AccessibleActor(cl, children[0]["actor"])
     return cl, accessible
 
 
 def test_audit():
```

## Comparing `geckordp-0.4.53/tests/actors/accessibility/test_accessible_walker.py` & `geckordp-0.5.0/tests/actors/accessibility/test_accessible_walker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
-from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.accessibility.accessibility import AccessibilityActor
 from geckordp.actors.accessibility.accessible_walker import AccessibleWalkerActor
 from geckordp.actors.accessibility.parent_accessibility import ParentAccessibilityActor
+from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     actor_ids = tab.get_target()
     root_ids = root.get_root()
     accessibility = AccessibilityActor(cl, actor_ids["accessibilityActor"])
-    walker = AccessibleWalkerActor(cl,
-                                   accessibility.get_walker()["actor"])
+    walker = AccessibleWalkerActor(cl, accessibility.get_walker()["actor"])
     accessibility.bootstrap()
-    parent = ParentAccessibilityActor(
-        cl, root_ids["parentAccessibilityActor"])
+    parent = ParentAccessibilityActor(cl, root_ids["parentAccessibilityActor"])
     parent.bootstrap()
     parent.enable()
     return cl, walker
 
 
 def test_children():
     cl = None
```

## Comparing `geckordp-0.4.53/tests/actors/accessibility/test_accessibility.py` & `geckordp-0.5.0/tests/actors/accessibility/test_accessibility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
-from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.accessibility.accessibility import AccessibilityActor
+from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
@@ -53,11 +54,13 @@
 
 def test_get_simulator():
     cl = None
     try:
         cl, accessibility = init()
         val = accessibility.get_simulator()
         simulator_id = val.get("actor", None)
-        if (simulator_id is None):
-            log("No simulator actor found, firefox is probably running in headless mode")
+        if simulator_id is None:
+            log(
+                "No simulator actor found, firefox is probably running in headless mode"
+            )
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.53/tests/actors/test_network_event.py` & `geckordp-0.5.0/tests/actors/test_network_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 # pylint: disable=unused-import
 from time import sleep
+
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
+from geckordp.actors.descriptors.process import ProcessActor
 from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.events import Events
 from geckordp.actors.network_event import NetworkEventActor
-from geckordp.actors.web_console import WebConsoleActor
+from geckordp.actors.resources import Resources
+from geckordp.actors.root import RootActor
 from geckordp.actors.targets.window_global import WindowGlobalActor
-from geckordp.actors.watcher import WatcherActor
-from geckordp.actors.descriptors.process import ProcessActor
 from geckordp.actors.thread import ThreadActor
-from geckordp.actors.events import Events
+from geckordp.actors.watcher import WatcherActor
+from geckordp.actors.web_console import WebConsoleActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def test_network_event():
     cl = None
     try:
         cl = RDPClient(3)
         cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
         root = RootActor(cl)
         process_descriptors = root.list_processes()
 
         for descriptor in process_descriptors:
             actor_id = descriptor["actor"]
-            process_actor_ids = ProcessActor(
-                cl, actor_id).get_target()
+            process_actor_ids = ProcessActor(cl, actor_id).get_target()
 
-            console = WebConsoleActor(
-                cl, process_actor_ids["consoleActor"])
+            console = WebConsoleActor(cl, process_actor_ids["consoleActor"])
             console.start_listeners([])
 
         current_tab = root.current_tab()
         tab = TabActor(cl, current_tab["actor"])
         actor_ids = tab.get_target()
 
-        browser = WindowGlobalActor(
-            cl, actor_ids["actor"])
+        browser = WindowGlobalActor(cl, actor_ids["actor"])
 
-        console = WebConsoleActor(
-            cl, actor_ids["consoleActor"])
+        console = WebConsoleActor(cl, actor_ids["consoleActor"])
         console.start_listeners([])
 
         watcher_ctx = tab.get_watcher()
-        watcher = WatcherActor(
-            cl, watcher_ctx["actor"])
+        watcher = WatcherActor(cl, watcher_ctx["actor"])
 
-        thread = ThreadActor(
-            cl, actor_ids["threadActor"])
+        thread = ThreadActor(cl, actor_ids["threadActor"])
         thread.attach()
 
         # todo add TargetConfigurationActor
 
-        watcher.watch_resources([
-            WatcherActor.Resources.CONSOLE_MESSAGE,
-            WatcherActor.Resources.ERROR_MESSAGE,
-            WatcherActor.Resources.NETWORK_EVENT,
-            WatcherActor.Resources.NETWORK_EVENT_STACKTRACE,
-            WatcherActor.Resources.DOCUMENT_EVENT,
-        ])
+        watcher.watch_resources(
+            [
+                Resources.CONSOLE_MESSAGE,
+                Resources.ERROR_MESSAGE,
+                Resources.NETWORK_EVENT,
+                Resources.NETWORK_EVENT_STACKTRACE,
+                Resources.DOCUMENT_EVENT,
+            ]
+        )
 
         network_event_ids = []
 
         def on_resource_available(data):
             resources = data["resources"]
-            if (len(resources) <= 0):
+            if len(resources) <= 0:
                 return
             resources = resources[0]
-            if (resources["resourceType"] != "network-event"):
+            if resources["resourceType"] != "network-event":
                 return
             network_event_actor_id = resources["actor"]
             resource_id = resources.get("resourceId", -1)
-            if (resource_id == -1):
+            if resource_id == -1:
                 return
             network_event_ids.append(network_event_actor_id)
 
         cl.add_event_listener(
             watcher_ctx["actor"],
             Events.Watcher.RESOURCE_AVAILABLE_FORM,
-            on_resource_available)
+            on_resource_available,
+        )
 
         browser.navigate_to("https://example.com/")
         sleep(1.5)
         network_event = NetworkEventActor(cl, network_event_ids[0])
 
         # get_request_headers
         val = network_event.get_request_headers()["headers"]
```

## Comparing `geckordp-0.4.53/tests/actors/test_network_content.py` & `geckordp-0.5.0/tests/actors/test_network_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # pylint: disable=unused-import
 import pytest
-import tests.helpers.utils as utils
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
+import tests.helpers.utils as utils
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.network_content import NetworkContentActor
+from geckordp.actors.root import RootActor
 from geckordp.actors.watcher import WatcherActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
@@ -25,15 +26,15 @@
 
 # todo see function itself
 # def test_send_http_request_get_stack_trace():
 #     cl = None
 #     try:
 #         cl, network_content, watcher = init()
 #         watcher.watch_resources(
-#             [WatcherActor.Resources.NETWORK_EVENT_STACKTRACE])
+#             [Resources.NETWORK_EVENT_STACKTRACE])
 #         val = network_content.send_http_request(
 #             method="GET",
 #             url="https://example.com/",
 #             headers={
 #                 "Host": "example.com",
 #                 "User-Agent": "special-agent-007"
 #             },
```

## Comparing `geckordp-0.4.53/tests/actors/addon/test_addons.py` & `geckordp-0.5.0/tests/actors/addon/test_addons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.addon.addons import AddonsActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     root_ids = root.get_root()
@@ -18,10 +19,10 @@
 
 
 def test_install_temporary_addon():
     cl = None
     try:
         cl, _addons = init()
         # todo may not change anyway
-        #val = addons.install_temporary_addon("")
+        # val = addons.install_temporary_addon("")
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.53/tests/actors/addon/test_web_extension_inspected_window.py` & `geckordp-0.5.0/tests/actors/addon/test_web_extension_inspected_window.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
+from geckordp.actors.addon.web_extension_inspected_window import (
+    WebExtensionInspectedWindowActor,
+)
 from geckordp.actors.descriptors.tab import TabActor
-from geckordp.actors.addon.web_extension_inspected_window import WebExtensionInspectedWindowActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     addons = root.list_addons()
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     actor_ids = tab.get_target()
     webext = WebExtensionInspectedWindowActor(
-        cl, actor_ids["webExtensionInspectedWindowActor"])
+        cl, actor_ids["webExtensionInspectedWindowActor"]
+    )
     addon = None
     for a in addons:
-        if (a.get("url", None) is not None):
+        if a.get("url", None) is not None:
             addon = a
             break
-    if (addon is None):
+    if addon is None:
         print("WARNING: no addon available")
     return cl, addon, webext
 
 
 def test_reload():
     cl = None
     try:
         cl, addon, webext = init()
-        if (addon is None):
+        if addon is None:
             return
-        val = webext.reload(
-            addon["url"], 1, addon["id"])
-        assert response_valid(
-            "webExtensionInspectedWindowActor", val), str(val)
+        val = webext.reload(addon["url"], 1, addon["id"])
+        assert response_valid("webExtensionInspectedWindowActor", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_eval():
     cl = None
     try:
         cl, addon, webext = init()
-        if (addon is None):
+        if addon is None:
             return
-        val = webext.eval(
-            "v = 10;", addon["url"], 1, addon["id"])
+        val = webext.eval("v = 10;", addon["url"], 1, addon["id"])
         assert "evalResult" in val
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.53/tests/actors/test_device.py` & `geckordp-0.5.0/tests/actors/test_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.device import DeviceActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     root_ids = root.get_root()
-    device = DeviceActor(
-        cl, root_ids["deviceActor"])
+    device = DeviceActor(cl, root_ids["deviceActor"])
     return cl, device
 
 
 def test_get_description():
     cl = None
     try:
         cl, device = init()
```

## Comparing `geckordp-0.4.53/tests/actors/test_network_parent.py` & `geckordp-0.5.0/tests/actors/test_network_parent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.network_parent import NetworkParentActor
+from geckordp.actors.resources import Resources
+from geckordp.actors.root import RootActor
 from geckordp.actors.watcher import WatcherActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     tab.get_target()
     watcher = WatcherActor(cl, tab.get_watcher()["actor"])
-    watcher.watch_resources([
-        WatcherActor.Resources.CONSOLE_MESSAGE,
-        WatcherActor.Resources.ERROR_MESSAGE,
-        WatcherActor.Resources.NETWORK_EVENT,
-        WatcherActor.Resources.NETWORK_EVENT_STACKTRACE,
-        WatcherActor.Resources.DOCUMENT_EVENT,
-    ])
+    watcher.watch_resources(
+        [
+            Resources.CONSOLE_MESSAGE,
+            Resources.ERROR_MESSAGE,
+            Resources.NETWORK_EVENT,
+            Resources.NETWORK_EVENT_STACKTRACE,
+            Resources.DOCUMENT_EVENT,
+        ]
+    )
     network_parent = NetworkParentActor(
-        cl, watcher.get_network_parent_actor()["network"]["actor"])
+        cl, watcher.get_network_parent_actor()["network"]["actor"]
+    )
     return cl, network_parent
 
 
 def test_set_persist():
     cl = None
     try:
         cl, network_parent = init()
@@ -81,15 +86,16 @@
 
 
 def test_set_blocked_urls():
     cl = None
     try:
         cl, network_parent = init()
         val = network_parent.set_blocked_urls(
-            ["example.com", ".js", "https://www.google.com/"])
+            ["example.com", ".js", "https://www.google.com/"]
+        )
         assert response_valid("networkParent", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_get_blocked_urls():
     cl = None
```

## Comparing `geckordp-0.4.53/tests/actors/test_storage_local.py` & `geckordp-0.5.0/tests/actors/test_storage_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 # pylint: disable=unused-import
 from concurrent.futures import Future
+
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.events import Events
-from geckordp.actors.watcher import WatcherActor
+from geckordp.actors.resources import Resources
+from geckordp.actors.root import RootActor
 from geckordp.actors.storage import LocalStorageActor
+from geckordp.actors.watcher import WatcherActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     watcher_ctx = tab.get_watcher()
-    watcher = WatcherActor(
-        cl, watcher_ctx["actor"])
+    watcher = WatcherActor(cl, watcher_ctx["actor"])
+
+    target = get_available_target(cl, watcher, current_tab["browsingContextID"])
+    assert "actor" in target
 
     resource = {}
-    fut = Future()
+    resource_fut = Future()
 
     async def on_resource(data: dict):
         resources = data.get("resources", [])
         for resource in resources:
-            if ("local" in resource.get("actor", "")):
-                fut.set_result(resource)
+            if "local" in resource.get("actor", ""):
+                resource_fut.set_result(resource)
 
-    actor_ids = tab.get_target()
-    window_global_actor = actor_ids["actor"]
     cl.add_event_listener(
-        window_global_actor, Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource)
-
-    watcher.watch_targets(WatcherActor.Targets.FRAME)
-    watcher.watch_resources([WatcherActor.Resources.LOCAL_STORAGE])
+        target["actor"], Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource
+    )
+    watcher.watch_resources([Resources.LOCAL_STORAGE])
 
-    resource = fut.result(3.0)
+    resource = resource_fut.result(3.0)
     assert "actor" in resource
 
     storage_actor_id = resource.get("actor", "")
     local = LocalStorageActor(cl, storage_actor_id)
 
     return cl, local
```

## Comparing `geckordp-0.4.53/tests/actors/test_watcher.py` & `geckordp-0.5.0/tests/actors/test_watcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.resources import Resources
+from geckordp.actors.root import RootActor
 from geckordp.actors.watcher import WatcherActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
@@ -49,46 +51,52 @@
         cl.disconnect()
 
 
 def test_watch_resources():
     cl = None
     try:
         cl, watcher = init()
-        val = watcher.watch_resources([
-            WatcherActor.Resources.NETWORK_EVENT,
-            WatcherActor.Resources.NETWORK_EVENT_STACKTRACE,
-            WatcherActor.Resources.DOCUMENT_EVENT,
-        ])
+        val = watcher.watch_resources(
+            [
+                Resources.NETWORK_EVENT,
+                Resources.NETWORK_EVENT_STACKTRACE,
+                Resources.DOCUMENT_EVENT,
+            ]
+        )
         assert response_valid("watcher", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_unwatch_resources():
     cl = None
     try:
         cl, watcher = init()
-        watcher.unwatch_resources([
-            WatcherActor.Resources.NETWORK_EVENT,
-            WatcherActor.Resources.NETWORK_EVENT_STACKTRACE,
-            WatcherActor.Resources.DOCUMENT_EVENT,
-        ])
+        watcher.unwatch_resources(
+            [
+                Resources.NETWORK_EVENT,
+                Resources.NETWORK_EVENT_STACKTRACE,
+                Resources.DOCUMENT_EVENT,
+            ]
+        )
     finally:
         cl.disconnect()
 
 
 def test_clear_resources():
     cl = None
     try:
         cl, watcher = init()
-        watcher.clear_resources([
-            WatcherActor.Resources.NETWORK_EVENT,
-            WatcherActor.Resources.NETWORK_EVENT_STACKTRACE,
-            WatcherActor.Resources.DOCUMENT_EVENT,
-        ])
+        watcher.clear_resources(
+            [
+                Resources.NETWORK_EVENT,
+                Resources.NETWORK_EVENT_STACKTRACE,
+                Resources.DOCUMENT_EVENT,
+            ]
+        )
     finally:
         cl.disconnect()
 
 
 def test_get_network_parent_actor():
     cl = None
     try:
```

## Comparing `geckordp-0.4.53/tests/actors/descriptors/test_tab.py` & `geckordp-0.5.0/tests/actors/descriptors/test_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
```

## Comparing `geckordp-0.4.53/tests/actors/descriptors/test_web_extension.py` & `geckordp-0.5.0/tests/actors/descriptors/test_web_extension.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.descriptors.web_extension import WebExtensionActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     addons = root.list_addons()
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     actor_ids = tab.get_target()
     webext = None
     addon = None
     for a in addons:
-        if (a.get("url", None) is not None):
+        if a.get("url", None) is not None:
             addon = a
-            webext = WebExtensionActor(
-                cl, addon["actor"])
+            webext = WebExtensionActor(cl, addon["actor"])
             break
-    if (addon is None):
+    if addon is None:
         print("WARNING: no addon available")
     return cl, addon, webext
 
 
 def test_reload():
     cl = None
     try:
         cl, addon, webext = init()
-        if (addon is None):
+        if addon is None:
             return
         val = webext.reload()
-        assert response_valid(
-            "webExtensionDescriptor", val), str(val)
+        assert response_valid("webExtensionDescriptor", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_connect():
     cl = None
     try:
         cl, addon, webext = init()
-        if (addon is None):
+        if addon is None:
             return
         val = webext.connect()
-        assert response_valid(
-            "webExtensionDescriptor", val), str(val)
+        assert response_valid("webExtensionDescriptor", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_get_target():
     cl = None
     try:
         cl, addon, webext = init()
-        if (addon is None):
+        if addon is None:
             return
         val = webext.get_target()
-        assert response_valid(
-            "webExtensionDescriptor", val), str(val)
+        assert response_valid("webExtensionDescriptor", val), str(val)
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.53/tests/actors/descriptors/test_worker.py` & `geckordp-0.5.0/tests/actors/descriptors/test_worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.worker import WorkerActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     workers = root.list_workers()
```

## Comparing `geckordp-0.4.53/tests/actors/descriptors/test_process.py` & `geckordp-0.5.0/tests/actors/descriptors/test_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
-from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.descriptors.process import ProcessActor
+from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     processes = root.list_processes()
-    process = ProcessActor(
-        cl, processes[0]["actor"])
+    process = ProcessActor(cl, processes[0]["actor"])
     return cl, process
 
 
 def test_get_target():
     cl = None
     try:
         cl, process = init()
```

## Comparing `geckordp-0.4.53/tests/actors/test_storage_cache.py` & `geckordp-0.5.0/tests/actors/test_storage_cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 # pylint: disable=unused-import
 from concurrent.futures import Future
+
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.events import Events
-from geckordp.actors.watcher import WatcherActor
+from geckordp.actors.resources import Resources
+from geckordp.actors.root import RootActor
 from geckordp.actors.storage import CacheStorageActor
+from geckordp.actors.watcher import WatcherActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     watcher_ctx = tab.get_watcher()
-    watcher = WatcherActor(
-        cl, watcher_ctx["actor"])
+    watcher = WatcherActor(cl, watcher_ctx["actor"])
+
+    target = get_available_target(cl, watcher, current_tab["browsingContextID"])
+    assert "actor" in target
 
     resource = {}
-    fut = Future()
+    resource_fut = Future()
 
     async def on_resource(data: dict):
         resources = data.get("resources", [])
         for resource in resources:
-            if ("Cache" in resource.get("actor", "")):
-                fut.set_result(resource)
+            if "Cache" in resource.get("actor", ""):
+                resource_fut.set_result(resource)
 
-    actor_ids = tab.get_target()
-    window_global_actor = actor_ids["actor"]
     cl.add_event_listener(
-        window_global_actor, Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource)
+        target["actor"], Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource
+    )
 
-    watcher.watch_targets(WatcherActor.Targets.FRAME)
-    watcher.watch_resources([WatcherActor.Resources.CACHE_STORAGE])
+    watcher.watch_resources([Resources.CACHE_STORAGE])
 
-    resource = fut.result(3.0)
+    resource = resource_fut.result(3.0)
     assert "actor" in resource
 
     storage_actor_id = resource.get("actor", "")
     cache = CacheStorageActor(cl, storage_actor_id)
 
     return cl, cache
```

## Comparing `geckordp-0.4.53/tests/actors/test_web_console.py` & `geckordp-0.5.0/tests/actors/test_web_console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # pylint: disable=unused-import
 from time import sleep
+
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
+from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.events import Events
 from geckordp.actors.root import RootActor
 from geckordp.actors.string import StringActor
 from geckordp.actors.web_console import WebConsoleActor
-from geckordp.actors.descriptors.tab import TabActor
-from geckordp.actors.events import Events
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
@@ -56,17 +58,20 @@
         cl.disconnect()
 
 
 def test_get_cached_messages():
     cl = None
     try:
         cl, console = init()
-        val = console.get_cached_messages([
-            WebConsoleActor.MessageTypes.PAGE_ERROR,
-            WebConsoleActor.MessageTypes.CONSOLE_API])
+        val = console.get_cached_messages(
+            [
+                WebConsoleActor.MessageTypes.PAGE_ERROR,
+                WebConsoleActor.MessageTypes.CONSOLE_API,
+            ]
+        )
         assert len(val["messages"]) >= 0
     finally:
         cl.disconnect()
 
 
 def test_evaluate_js_async():
     cl = None
@@ -77,15 +82,16 @@
 
         def on_eval(data):
             log(f"XXX:{data}")
             assert result_id == data["resultID"]
             assert data["result"] == "Example Domain"
 
         cl.add_event_listener(
-            console.actor_id, Events.WebConsole.EVALUATION_RESULT, on_eval)
+            console.actor_id, Events.WebConsole.EVALUATION_RESULT, on_eval
+        )
 
         response = console.evaluate_js_async(wrap_js("return document.title;"))
         result_id = response["resultID"]
         sleep(0.1)
     finally:
         cl.disconnect()
 
@@ -102,23 +108,28 @@
             assert result_id == data["resultID"]
             assert data["result"]["type"] == "longString"
             string = StringActor(cl, data["result"]["actor"])
             val = string.substring(0, data["result"]["length"])
             assert len(val) == size
 
         cl.add_event_listener(
-            console.actor_id, Events.WebConsole.EVALUATION_RESULT, on_eval)
+            console.actor_id, Events.WebConsole.EVALUATION_RESULT, on_eval
+        )
 
-        response = console.evaluate_js_async(wrap_js(f"""
+        response = console.evaluate_js_async(
+            wrap_js(
+                f"""
             var size = {size}
             var buf = new Array(size);
             for(let i=0; i<size;i++)
                 buf[i] = 'x';
             return buf.join('');
-        """))
+        """
+            )
+        )
         result_id = response["resultID"]
         sleep(0.1)
     finally:
         cl.disconnect()
 
 
 def test_autocomplete():
```

## Comparing `geckordp-0.4.53/tests/actors/test_node_list.py` & `geckordp-0.5.0/tests/actors/test_node_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
-from geckordp.actors.node_list import NodeListActor
 from geckordp.actors.inspector import InspectorActor
+from geckordp.actors.node_list import NodeListActor
+from geckordp.actors.root import RootActor
 from geckordp.actors.walker import WalkerActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
```

## Comparing `geckordp-0.4.53/tests/actors/test_screenshot.py` & `geckordp-0.5.0/tests/actors/test_screenshot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.root import RootActor
 from geckordp.actors.screenshot import ScreenshotActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     actor_ids = tab.get_target()
     ctx_id = actor_ids["browsingContextID"]
-    screenshot = ScreenshotActor(
-        cl, root.get_root()["screenshotActor"])
+    screenshot = ScreenshotActor(cl, root.get_root()["screenshotActor"])
     return cl, ctx_id, screenshot
 
 
 def test_capture():
     cl = None
     try:
         cl, ctx_id, screenshot = init()
```

## Comparing `geckordp-0.4.53/tests/actors/test_preference.py` & `geckordp-0.5.0/tests/actors/test_preference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.preference import PreferenceActor
+from geckordp.actors.root import RootActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     root_ids = root.get_root()
-    preference = PreferenceActor(
-        cl, root_ids["preferenceActor"])
+    preference = PreferenceActor(cl, root_ids["preferenceActor"])
     return cl, preference
 
 
 def test_get_traits():
     cl = None
     try:
         cl, preference = init()
@@ -28,38 +28,41 @@
         cl.disconnect()
 
 
 def test_get_bool_pref():
     cl = None
     try:
         cl, preference = init()
-        val = preference.get_bool_pref(
-            "toolkit.tabbox.switchByScrolling").get("value", None)
+        val = preference.get_bool_pref("toolkit.tabbox.switchByScrolling").get(
+            "value", None
+        )
         assert val == True or val == False
     finally:
         cl.disconnect()
 
 
 def test_get_char_pref():
     cl = None
     try:
         cl, preference = init()
-        val = preference.get_char_pref(
-            "devtools.debugger.chrome-debugging-host").get("value", "")
+        val = preference.get_char_pref("devtools.debugger.chrome-debugging-host").get(
+            "value", ""
+        )
         assert "localhost" in val
     finally:
         cl.disconnect()
 
 
 def test_get_int_pref():
     cl = None
     try:
         cl, preference = init()
-        val = preference.get_int_pref(
-            "devtools.debugger.end-panel-size").get("value", 0)
+        val = preference.get_int_pref("devtools.debugger.end-panel-size").get(
+            "value", 0
+        )
         assert val > 0
     finally:
         cl.disconnect()
 
 
 def test_get_all_prefs():
     cl = None
@@ -71,49 +74,45 @@
         cl.disconnect()
 
 
 def test_set_bool_pref():
     cl = None
     try:
         cl, preference = init()
-        val = preference.set_bool_pref(
-            "toolkit.tabbox.switchByScrolling", False)
+        val = preference.set_bool_pref("toolkit.tabbox.switchByScrolling", False)
         assert response_valid("preferenceActor", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_set_char_pref():
     cl = None
     try:
         cl, preference = init()
         val = preference.set_char_pref(
-            "devtools.debugger.chrome-debugging-host", "localhost")
+            "devtools.debugger.chrome-debugging-host", "localhost"
+        )
         assert response_valid("preferenceActor", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_set_int_pref():
     cl = None
     try:
         cl, preference = init()
-        val = preference.set_int_pref(
-            "devtools.debugger.end-panel-size", 300)
+        val = preference.set_int_pref("devtools.debugger.end-panel-size", 300)
         assert response_valid("preferenceActor", val), str(val)
     finally:
         cl.disconnect()
 
 
 def test_clear_user_pref():
     cl = None
     try:
         cl, preference = init()
-        preference.clear_user_pref(
-            "toolkit.tabbox.switchByScrolling")
-        preference.clear_user_pref(
-            "devtools.debugger.chrome-debugging-host")
-        val = preference.clear_user_pref(
-            "devtools.debugger.end-panel-size")
+        preference.clear_user_pref("toolkit.tabbox.switchByScrolling")
+        preference.clear_user_pref("devtools.debugger.chrome-debugging-host")
+        val = preference.clear_user_pref("devtools.debugger.end-panel-size")
         assert response_valid("preferenceActor", val), str(val)
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.53/tests/actors/test_storage_indexed.py` & `geckordp-0.5.0/tests/actors/test_storage_indexed.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 # pylint: disable=unused-import
 from concurrent.futures import Future
+
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.events import Events
-from geckordp.actors.watcher import WatcherActor
+from geckordp.actors.resources import Resources
+from geckordp.actors.root import RootActor
 from geckordp.actors.storage import IndexedDBStorageActor
+from geckordp.actors.watcher import WatcherActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     watcher_ctx = tab.get_watcher()
-    watcher = WatcherActor(
-        cl, watcher_ctx["actor"])
+    watcher = WatcherActor(cl, watcher_ctx["actor"])
+
+    # if the tests fail, see "test_storage_local.py:init()"
 
     resource = {}
     fut = Future()
 
     async def on_resource(data: dict):
         resources = data.get("resources", [])
         for resource in resources:
-            if ("indexedDB" in resource.get("actor", "")):
+            if "indexedDB" in resource.get("actor", ""):
                 fut.set_result(resource)
 
     cl.add_event_listener(
-        watcher.actor_id, Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource)
+        watcher.actor_id, Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource
+    )
 
-    watcher.watch_targets(WatcherActor.Targets.FRAME)
-    watcher.watch_resources([WatcherActor.Resources.INDEXED_DB])
+    watcher.watch_resources([Resources.INDEXED_DB])
 
     resource = fut.result(3.0)
     assert "actor" in resource
 
     storage_actor_id = resource.get("actor", "")
     indexed = IndexedDBStorageActor(cl, storage_actor_id)
```

## Comparing `geckordp-0.4.53/tests/actors/targets/test_window_global.py` & `geckordp-0.5.0/tests/actors/targets/test_window_global.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
+from geckordp.actors.root import RootActor
 from geckordp.actors.targets.window_global import WindowGlobalActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     actor_ids = tab.get_target()
-    browser = WindowGlobalActor(
-        cl, actor_ids["actor"])
+    browser = WindowGlobalActor(cl, actor_ids["actor"])
     return cl, browser
 
 
 def test_detach():
     cl = None
     try:
         cl, browser = init()
```

## Comparing `geckordp-0.4.53/tests/actors/targets/test_content_process.py` & `geckordp-0.5.0/tests/actors/targets/test_content_process.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.process import ProcessActor
+from geckordp.actors.root import RootActor
 from geckordp.actors.targets.content_process import ContentProcessActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     processes = root.list_processes()
     content_process = None
     for p in processes:
-        if (not p["isParent"]):
+        if not p["isParent"]:
             process = ProcessActor(cl, p["actor"])
-            content_process = ContentProcessActor(
-                cl, process.get_target()["actor"])
+            content_process = ContentProcessActor(cl, process.get_target()["actor"])
             break
     return cl, content_process
 
 
 def test_list_workers():
     cl = None
     try:
```

## Comparing `geckordp-0.4.53/tests/actors/test_storage_session.py` & `geckordp-0.5.0/tests/actors/test_storage_session.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 # pylint: disable=unused-import
 from concurrent.futures import Future
+
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.events import Events
-from geckordp.actors.watcher import WatcherActor
+from geckordp.actors.resources import Resources
+from geckordp.actors.root import RootActor
 from geckordp.actors.storage import SessionStorageActor
+from geckordp.actors.watcher import WatcherActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     watcher_ctx = tab.get_watcher()
-    watcher = WatcherActor(
-        cl, watcher_ctx["actor"])
+    watcher = WatcherActor(cl, watcher_ctx["actor"])
+
+    target = get_available_target(cl, watcher, current_tab["browsingContextID"])
+    assert "actor" in target
 
     resource = {}
-    fut = Future()
+    resource_fut = Future()
 
     async def on_resource(data: dict):
         resources = data.get("resources", [])
         for resource in resources:
-            if ("session" in resource.get("actor", "")):
-                fut.set_result(resource)
+            if "session" in resource.get("actor", ""):
+                resource_fut.set_result(resource)
 
-    actor_ids = tab.get_target()
-    window_global_actor = actor_ids["actor"]
     cl.add_event_listener(
-        window_global_actor, Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource)
-
-    watcher.watch_targets(WatcherActor.Targets.FRAME)
-    watcher.watch_resources([WatcherActor.Resources.SESSION_STORAGE])
+        target["actor"], Events.Watcher.RESOURCE_AVAILABLE_FORM, on_resource
+    )
+    watcher.watch_resources([Resources.SESSION_STORAGE])
 
-    resource = fut.result(3.0)
+    resource = resource_fut.result(3.0)
     assert "actor" in resource
 
     storage_actor_id = resource.get("actor", "")
     session = SessionStorageActor(cl, storage_actor_id)
 
     return cl, session
```

## Comparing `geckordp-0.4.53/tests/actors/test_thread.py` & `geckordp-0.5.0/tests/actors/test_thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # pylint: disable=unused-import
 from logging import warning
+
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
+from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.root import RootActor
 from geckordp.actors.thread import ThreadActor
-from geckordp.actors.descriptors.tab import TabActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
     tab = TabActor(cl, current_tab["actor"])
     actor_ids = tab.get_target()
-    # todo add TargetConfigurationActor
-    thread = ThreadActor(
-        cl, actor_ids["threadActor"])
+    thread = ThreadActor(cl, actor_ids["threadActor"])
     val = thread.attach()
     assert response_valid("thread", val), str(val)
     return cl, thread
 
 
 def test_reconfigure():
     cl = None
@@ -105,57 +105,47 @@
 
 
 def test_set_breakpoint():
     cl = None
     try:
         cl, thread = init()
         sources = thread.sources()
-        if (len(sources) >= 0):
+        if len(sources) >= 0:
             print("WARNING: no sources available")
             return
         source = None
         for s in sources:
-            if (s.get("actor", None) is not None):
+            if s.get("actor", None) is not None:
                 source = s
                 break
-        val = thread.set_breakpoint(
-            0,
-            0,
-            source["sourceMapBaseURL"],
-            source["actor"])
+        val = thread.set_breakpoint(0, 0, source["sourceMapBaseURL"], source["actor"])
         assert response_valid("thread", val), str(val)
         val = thread.dump_thread()["breakpoints"][0]
         assert source["sourceMapBaseURL"] in val
     finally:
         cl.disconnect()
 
 
 def test_remove_breakpoint():
     cl = None
     try:
         cl, thread = init()
         sources = thread.sources()
-        if (len(sources) >= 0):
+        if len(sources) >= 0:
             print("WARNING: no sources available")
             return
         source = None
         for s in sources:
-            if (s.get("actor", None) is not None):
+            if s.get("actor", None) is not None:
                 source = s
                 break
-        thread.set_breakpoint(
-            0,
-            0,
-            source["sourceMapBaseURL"],
-            source["actor"])
+        thread.set_breakpoint(0, 0, source["sourceMapBaseURL"], source["actor"])
         val = thread.remove_breakpoint(
-            0,
-            0,
-            source["sourceMapBaseURL"],
-            source["actor"])
+            0, 0, source["sourceMapBaseURL"], source["actor"]
+        )
         assert response_valid("thread", val), str(val)
         val = thread.dump_thread()["breakpoints"]
         assert len(val) == 0
     finally:
         cl.disconnect()
```

## Comparing `geckordp-0.4.53/tests/actors/test_storage_extension.py` & `geckordp-0.5.0/tests/actors/test_storage_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # pylint: disable=unused-import
 from concurrent.futures import Future
+
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.events import Events
-from geckordp.actors.watcher import WatcherActor
+from geckordp.actors.root import RootActor
 from geckordp.actors.storage import ExtensionStorageActor
+from geckordp.actors.watcher import WatcherActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 """ todo: ExtensionStorageActor requires to inspect extension's page. However it seems it may not be possible
     to retrieve the actor id.
     If you encounter this issue and found the identifier of the actor,
     please open an issue here https://github.com/jpramosi/geckordp/issues/new.
 """
```

## Comparing `geckordp-0.4.53/tests/actors/test_walker.py` & `geckordp-0.5.0/tests/actors/test_walker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # pylint: disable=unused-import
 import pytest
+
 import tests.helpers.constants as constants
-from tests.helpers.utils import *
-from geckordp.rdp_client import RDPClient
-from geckordp.actors.root import RootActor
 from geckordp.actors.descriptors.tab import TabActor
 from geckordp.actors.inspector import InspectorActor
+from geckordp.actors.root import RootActor
 from geckordp.actors.walker import WalkerActor
 from geckordp.logger import log, logdict
+from geckordp.rdp_client import RDPClient
+from tests.helpers.utils import *
 
 
 def init():
     cl = RDPClient(3)
     cl.connect(constants.REMOTE_HOST, constants.REMOTE_PORT)
     root = RootActor(cl)
     current_tab = root.current_tab()
@@ -158,15 +159,16 @@
 
 def test_add_pseudo_class_lock():
     cl = None
     try:
         cl, walker = init()
         val = walker.document()
         val = walker.add_pseudo_class_lock(
-            val["actor"], WalkerActor.PseudoClass.FOCUS, True)
+            val["actor"], WalkerActor.PseudoClass.FOCUS, True
+        )
         assert response_valid("domwalker", val), str(val)
     finally:
         cl.disconnect()
 
 
 # "node.rawNode.classList is undefined"
 """ def test_hide_node():
@@ -194,18 +196,18 @@
 
 
 def test_remove_pseudo_class_lock():
     cl = None
     try:
         cl, walker = init()
         val = walker.document()
-        walker.add_pseudo_class_lock(
-            val["actor"], WalkerActor.PseudoClass.FOCUS, True)
+        walker.add_pseudo_class_lock(val["actor"], WalkerActor.PseudoClass.FOCUS, True)
         val = walker.remove_pseudo_class_lock(
-            val["actor"], WalkerActor.PseudoClass.FOCUS, True)
+            val["actor"], WalkerActor.PseudoClass.FOCUS, True
+        )
         assert response_valid("domwalker", val), str(val)
     finally:
         cl.disconnect()
 
 
 # "InspectorUtils.clearPseudoClassLocks: Argument 1 does not implement interface Element."
 """ def test_clear_pseudo_class_locks():
@@ -441,19 +443,17 @@
 
 def test_set_mutation_breakpoints():
     cl = None
     try:
         cl, walker = init()
         val = walker.document()
         val = walker.query_selector(val["actor"], "body h1")["node"]
-        res = walker.set_mutation_breakpoints(
-            val["actor"], False, False, False)
+        res = walker.set_mutation_breakpoints(val["actor"], False, False, False)
         assert response_valid("domwalker", res), str(res)
-        res = walker.set_mutation_breakpoints(
-            val["actor"], False, True, False)
+        res = walker.set_mutation_breakpoints(val["actor"], False, True, False)
         assert response_valid("domwalker", res), str(res)
     finally:
         cl.disconnect()
 
 
 def test_get_embedder_element():
     cl = None
```

