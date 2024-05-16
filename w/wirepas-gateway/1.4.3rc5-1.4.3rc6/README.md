# Comparing `tmp/wirepas_gateway-1.4.3rc5.tar.gz` & `tmp/wirepas_gateway-1.4.3rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wirepas_gateway-1.4.3rc5.tar", last modified: Mon Oct 16 15:20:00 2023, max compression
+gzip compressed data, was "wirepas_gateway-1.4.3rc6.tar", last modified: Mon Jan 29 14:41:00 2024, max compression
```

## Comparing `wirepas_gateway-1.4.3rc5.tar` & `wirepas_gateway-1.4.3rc6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-10-16 15:20:00.072994 wirepas_gateway-1.4.3rc5/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    11341 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/LICENSE
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2837 2023-10-16 15:20:00.072994 wirepas_gateway-1.4.3rc5/PKG-INFO
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2165 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/README.md
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      120 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/requirements.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)       38 2023-10-16 15:20:00.072994 wirepas_gateway-1.4.3rc5/setup.cfg
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     3102 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/setup.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-10-16 15:20:00.052994 wirepas_gateway-1.4.3rc5/wirepas_gateway/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      858 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/__about__.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      580 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/__init__.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      350 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/__main__.py
--rwxr-xr-x   0 wirepas   (1000) wirepas   (1000)     9859 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/configure_node.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-10-16 15:20:00.068994 wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      119 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/__init__.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-10-16 15:20:00.068994 wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/c-extension/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     6089 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/c-extension/dbus_c.c
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5617 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/dbus_client.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5047 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/return_code.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    25029 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/sink_manager.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2010 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus_print_client.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-10-16 15:20:00.068994 wirepas_gateway-1.4.3rc5/wirepas_gateway/protocol/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)        0 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/protocol/__init__.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    13443 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/protocol/mqtt_wrapper.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5060 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/protocol/topic_helper.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    34541 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/transport_service.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-10-16 15:20:00.072994 wirepas_gateway-1.4.3rc5/wirepas_gateway/utils/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      200 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/utils/__init__.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    17230 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/utils/argument_tools.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      852 2023-10-16 15:18:21.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway/utils/serialization_tools.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-10-16 15:20:00.056994 wirepas_gateway-1.4.3rc5/wirepas_gateway.egg-info/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2837 2023-10-16 15:19:59.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway.egg-info/PKG-INFO
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      894 2023-10-16 15:20:00.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)        1 2023-10-16 15:19:59.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      171 2023-10-16 15:19:59.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway.egg-info/entry_points.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)       75 2023-10-16 15:19:59.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway.egg-info/requires.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)       31 2023-10-16 15:19:59.000000 wirepas_gateway-1.4.3rc5/wirepas_gateway.egg-info/top_level.txt
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2024-01-29 14:41:00.241561 wirepas_gateway-1.4.3rc6/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    11341 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/LICENSE
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2837 2024-01-29 14:41:00.237561 wirepas_gateway-1.4.3rc6/PKG-INFO
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2165 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/README.md
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      120 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/requirements.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)       38 2024-01-29 14:41:00.241561 wirepas_gateway-1.4.3rc6/setup.cfg
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     3102 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/setup.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2024-01-29 14:41:00.229561 wirepas_gateway-1.4.3rc6/wirepas_gateway/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      858 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/__about__.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      580 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/__init__.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      350 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/__main__.py
+-rwxr-xr-x   0 wirepas   (1000) wirepas   (1000)     9859 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/configure_node.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2024-01-29 14:41:00.233561 wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      119 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/__init__.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2024-01-29 14:41:00.233561 wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/c-extension/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     6089 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/c-extension/dbus_c.c
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5617 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/dbus_client.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5047 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/return_code.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    25029 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/sink_manager.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2010 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus_print_client.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2024-01-29 14:41:00.237561 wirepas_gateway-1.4.3rc6/wirepas_gateway/protocol/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)        0 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/protocol/__init__.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    13519 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/protocol/mqtt_wrapper.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5060 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/protocol/topic_helper.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    34541 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/transport_service.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2024-01-29 14:41:00.237561 wirepas_gateway-1.4.3rc6/wirepas_gateway/utils/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      200 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/utils/__init__.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    17230 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/utils/argument_tools.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      852 2024-01-29 14:40:04.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway/utils/serialization_tools.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2024-01-29 14:41:00.233561 wirepas_gateway-1.4.3rc6/wirepas_gateway.egg-info/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2837 2024-01-29 14:41:00.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      894 2024-01-29 14:41:00.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)        1 2024-01-29 14:41:00.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      171 2024-01-29 14:41:00.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway.egg-info/entry_points.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)       75 2024-01-29 14:41:00.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway.egg-info/requires.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)       31 2024-01-29 14:41:00.000000 wirepas_gateway-1.4.3rc6/wirepas_gateway.egg-info/top_level.txt
```

### Comparing `wirepas_gateway-1.4.3rc5/LICENSE` & `wirepas_gateway-1.4.3rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/PKG-INFO` & `wirepas_gateway-1.4.3rc6/wirepas_gateway.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wirepas_gateway
-Version: 1.4.3rc5
+Name: wirepas-gateway
+Version: 1.4.3rc6
 Summary: Wirepas gateway transport service that connects the local dbus to a remote MQTT broker.
 Home-page: https://github.com/wirepas/gateway
 Author: Wirepas Ltd
 Author-email: opensource@wirepas.com
 License: Apache-2
 Keywords: wirepas connectivity iot mesh
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wirepas_gateway-1.4.3rc5/README.md` & `wirepas_gateway-1.4.3rc6/README.md`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/setup.py` & `wirepas_gateway-1.4.3rc6/setup.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/__about__.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 ]
 __copyright__ = "2019 Wirepas Ltd"
 __description__ = "Wirepas gateway transport service that connects the local dbus to a remote MQTT broker."
 __license__ = "Apache-2"
 __pkg_name__ = "wirepas_gateway"
 __title__ = "Wirepas Gateway Transport Service"
 __url__ = "https://github.com/wirepas/gateway"
-__version__ = "1.4.3rc5"
+__version__ = "1.4.3rc6"
 __keywords__ = "wirepas connectivity iot mesh"
```

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/__init__.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/configure_node.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/configure_node.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/c-extension/dbus_c.c` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/c-extension/dbus_c.c`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/dbus_client.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/dbus_client.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/return_code.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/return_code.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus/sink_manager.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus/sink_manager.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/dbus_print_client.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/dbus_print_client.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/protocol/mqtt_wrapper.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/protocol/mqtt_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,30 +236,30 @@
         # Set Last wil message
         self._client.will_set(topic, data, qos=2, retain=True)
 
     def run(self):
         self.running = True
 
         while self.running:
-
             try:
-                # check if we are connected
-                # Get client socket to select on it
-                # This function manage the reconnect
-                sock = self._get_socket()
-                if sock is None:
-                    # Cannot get the socket, probably an issue
-                    # with connection. Exit the thread
-                    logging.error("Cannot get MQTT socket, exit...")
-                    self.running = False
-                else:
-                    self._do_select(sock)
-            except TimeoutError:
-                logging.error("Timeout in connection, force a reconnect")
-                self._client.reconnect()
+                try:
+                    # check if we are connected
+                    # Get client socket to select on it
+                    # This function manage the reconnect
+                    sock = self._get_socket()
+                    if sock is None:
+                        # Cannot get the socket, probably an issue
+                        # with connection. Exit the thread
+                        logging.error("Cannot get MQTT socket, exit...")
+                        self.running = False
+                    else:
+                        self._do_select(sock)
+                except TimeoutError:
+                    logging.error("Timeout in connection, force a reconnect")
+                    self._client.reconnect()
             except Exception:
                 # If an exception is not caught before this point
                 # All the transport module must be stopped in order to be fully
                 # restarted by the managing agent
                 logging.exception("Unexpected exception in MQTT wrapper Thread")
                 self.running = False
```

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/protocol/topic_helper.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/protocol/topic_helper.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/transport_service.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/transport_service.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/utils/argument_tools.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/utils/argument_tools.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway/utils/serialization_tools.py` & `wirepas_gateway-1.4.3rc6/wirepas_gateway/utils/serialization_tools.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway.egg-info/PKG-INFO` & `wirepas_gateway-1.4.3rc6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wirepas-gateway
-Version: 1.4.3rc5
+Name: wirepas_gateway
+Version: 1.4.3rc6
 Summary: Wirepas gateway transport service that connects the local dbus to a remote MQTT broker.
 Home-page: https://github.com/wirepas/gateway
 Author: Wirepas Ltd
 Author-email: opensource@wirepas.com
 License: Apache-2
 Keywords: wirepas connectivity iot mesh
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wirepas_gateway-1.4.3rc5/wirepas_gateway.egg-info/SOURCES.txt` & `wirepas_gateway-1.4.3rc6/wirepas_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

