# Comparing `tmp/komora_syncer-4.2.tar.gz` & `tmp/komora_syncer-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komora_syncer-4.2.tar", last modified: Wed Jan  3 12:02:04 2024, max compression
+gzip compressed data, was "komora_syncer-4.3.tar", last modified: Fri Apr 26 06:57:35 2024, max compression
```

## Comparing `komora_syncer-4.2.tar` & `komora_syncer-4.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 12:02:04.517083 komora_syncer-4.2/
--rw-r--r--   0 root         (0) root         (0)     1598 2024-01-03 12:02:04.517083 komora_syncer-4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      562 2023-08-25 10:05:04.000000 komora_syncer-4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 12:02:04.509082 komora_syncer-4.2/komora_syncer/
--rw-r--r--   0 root         (0) root         (0)       28 2022-02-03 09:20:26.000000 komora_syncer-4.2/komora_syncer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-09-14 11:14:26.000000 komora_syncer-4.2/komora_syncer/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 12:02:04.513083 komora_syncer-4.2/komora_syncer/connections/
--rw-r--r--   0 root         (0) root         (0)     6957 2023-09-14 11:14:26.000000 komora_syncer-4.2/komora_syncer/connections/KomoraApi.py
--rw-r--r--   0 root         (0) root         (0)     4273 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/connections/KomoraConnection.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/connections/NetboxConnection.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.2/komora_syncer/connections/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 12:02:04.513083 komora_syncer-4.2/komora_syncer/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.2/komora_syncer/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      221 2022-02-03 09:20:26.000000 komora_syncer-4.2/komora_syncer/helpers/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 12:02:04.513083 komora_syncer-4.2/komora_syncer/models/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.2/komora_syncer/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 12:02:04.513083 komora_syncer-4.2/komora_syncer/models/komora/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.2/komora_syncer/models/komora/__init__.py
--rw-r--r--   0 root         (0) root         (0)      747 2022-03-28 07:12:55.000000 komora_syncer-4.2/komora_syncer/models/komora/address.py
--rw-r--r--   0 root         (0) root         (0)     4500 2022-03-28 07:12:55.000000 komora_syncer-4.2/komora_syncer/models/komora/contact.py
--rw-r--r--   0 root         (0) root         (0)     1048 2022-03-28 07:12:55.000000 komora_syncer-4.2/komora_syncer/models/komora/device.py
--rw-r--r--   0 root         (0) root         (0)      271 2022-03-28 07:12:55.000000 komora_syncer-4.2/komora_syncer/models/komora/district.py
--rw-r--r--   0 root         (0) root         (0)     1329 2023-09-14 11:14:26.000000 komora_syncer-4.2/komora_syncer/models/komora/inventory.py
--rw-r--r--   0 root         (0) root         (0)      520 2022-03-28 07:12:55.000000 komora_syncer-4.2/komora_syncer/models/komora/location.py
--rw-r--r--   0 root         (0) root         (0)      381 2022-03-28 07:12:55.000000 komora_syncer-4.2/komora_syncer/models/komora/municipality.py
--rw-r--r--   0 root         (0) root         (0)     1304 2022-03-28 07:12:55.000000 komora_syncer-4.2/komora_syncer/models/komora/organization.py
--rw-r--r--   0 root         (0) root         (0)      171 2022-03-28 07:12:55.000000 komora_syncer-4.2/komora_syncer/models/komora/region.py
--rw-r--r--   0 root         (0) root         (0)     2042 2022-03-31 12:40:18.000000 komora_syncer-4.2/komora_syncer/models/komora/site.py
--rw-r--r--   0 root         (0) root         (0)      230 2022-03-28 07:12:55.000000 komora_syncer-4.2/komora_syncer/models/komora/site_contact.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 12:02:04.517083 komora_syncer-4.2/komora_syncer/models/netbox/
--rw-r--r--   0 root         (0) root         (0)     5023 2024-01-03 11:57:46.000000 komora_syncer-4.2/komora_syncer/models/netbox/NbDevice.py
--rw-r--r--   0 root         (0) root         (0)     6869 2024-01-03 11:57:46.000000 komora_syncer-4.2/komora_syncer/models/netbox/NbInventoryItem.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/models/netbox/NbLocation.py
--rw-r--r--   0 root         (0) root         (0)     3659 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/models/netbox/NbRegion.py
--rw-r--r--   0 root         (0) root         (0)     5738 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/models/netbox/NbSite.py
--rw-r--r--   0 root         (0) root         (0)     3113 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/models/netbox/NbTenant.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/models/netbox/NetboxBase.py
--rw-r--r--   0 root         (0) root         (0)     3000 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/models/netbox/NetboxCache.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.2/komora_syncer/models/netbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 12:02:04.517083 komora_syncer-4.2/komora_syncer/processors/
--rw-r--r--   0 root         (0) root         (0)     9043 2023-09-14 11:14:26.000000 komora_syncer-4.2/komora_syncer/processors/Synchronizer.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-25 10:05:04.000000 komora_syncer-4.2/komora_syncer/processors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 12:02:04.513083 komora_syncer-4.2/komora_syncer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1598 2024-01-03 12:02:04.000000 komora_syncer-4.2/komora_syncer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1554 2024-01-03 12:02:04.000000 komora_syncer-4.2/komora_syncer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-03 12:02:04.000000 komora_syncer-4.2/komora_syncer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-01-03 12:02:04.000000 komora_syncer-4.2/komora_syncer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-03 09:25:55.000000 komora_syncer-4.2/komora_syncer.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-03 12:02:04.000000 komora_syncer-4.2/komora_syncer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-01-03 12:02:04.000000 komora_syncer-4.2/komora_syncer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-03 12:02:04.517083 komora_syncer-4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1828 2024-01-03 11:59:28.000000 komora_syncer-4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:57:35.094989 komora_syncer-4.3/
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-04-26 06:57:35.094989 komora_syncer-4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      562 2023-08-25 10:05:04.000000 komora_syncer-4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:57:35.094989 komora_syncer-4.3/komora_syncer/
+-rw-r--r--   0 root         (0) root         (0)       28 2022-02-03 09:20:26.000000 komora_syncer-4.3/komora_syncer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-09-14 11:14:26.000000 komora_syncer-4.3/komora_syncer/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-08-25 10:05:04.000000 komora_syncer-4.3/komora_syncer/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:57:35.094989 komora_syncer-4.3/komora_syncer/connections/
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-09-14 11:14:26.000000 komora_syncer-4.3/komora_syncer/connections/KomoraApi.py
+-rw-r--r--   0 root         (0) root         (0)     4273 2023-08-25 10:05:04.000000 komora_syncer-4.3/komora_syncer/connections/KomoraConnection.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-08-25 10:05:04.000000 komora_syncer-4.3/komora_syncer/connections/NetboxConnection.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.3/komora_syncer/connections/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:57:35.094989 komora_syncer-4.3/komora_syncer/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.3/komora_syncer/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      221 2022-02-03 09:20:26.000000 komora_syncer-4.3/komora_syncer/helpers/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:57:35.094989 komora_syncer-4.3/komora_syncer/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.3/komora_syncer/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:57:35.094989 komora_syncer-4.3/komora_syncer/models/komora/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.3/komora_syncer/models/komora/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      747 2022-03-28 07:12:55.000000 komora_syncer-4.3/komora_syncer/models/komora/address.py
+-rw-r--r--   0 root         (0) root         (0)     4500 2022-03-28 07:12:55.000000 komora_syncer-4.3/komora_syncer/models/komora/contact.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2022-03-28 07:12:55.000000 komora_syncer-4.3/komora_syncer/models/komora/device.py
+-rw-r--r--   0 root         (0) root         (0)      271 2022-03-28 07:12:55.000000 komora_syncer-4.3/komora_syncer/models/komora/district.py
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-09-14 11:14:26.000000 komora_syncer-4.3/komora_syncer/models/komora/inventory.py
+-rw-r--r--   0 root         (0) root         (0)      520 2022-03-28 07:12:55.000000 komora_syncer-4.3/komora_syncer/models/komora/location.py
+-rw-r--r--   0 root         (0) root         (0)      381 2022-03-28 07:12:55.000000 komora_syncer-4.3/komora_syncer/models/komora/municipality.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2022-03-28 07:12:55.000000 komora_syncer-4.3/komora_syncer/models/komora/organization.py
+-rw-r--r--   0 root         (0) root         (0)      171 2022-03-28 07:12:55.000000 komora_syncer-4.3/komora_syncer/models/komora/region.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2022-03-31 12:40:18.000000 komora_syncer-4.3/komora_syncer/models/komora/site.py
+-rw-r--r--   0 root         (0) root         (0)      230 2022-03-28 07:12:55.000000 komora_syncer-4.3/komora_syncer/models/komora/site_contact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:57:35.094989 komora_syncer-4.3/komora_syncer/models/netbox/
+-rw-r--r--   0 root         (0) root         (0)     5033 2024-04-22 10:10:21.000000 komora_syncer-4.3/komora_syncer/models/netbox/NbDevice.py
+-rw-r--r--   0 root         (0) root         (0)     6849 2024-04-22 10:25:42.000000 komora_syncer-4.3/komora_syncer/models/netbox/NbInventoryItem.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-08-25 10:05:04.000000 komora_syncer-4.3/komora_syncer/models/netbox/NbLocation.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2023-08-25 10:05:04.000000 komora_syncer-4.3/komora_syncer/models/netbox/NbRegion.py
+-rw-r--r--   0 root         (0) root         (0)     5738 2023-08-25 10:05:04.000000 komora_syncer-4.3/komora_syncer/models/netbox/NbSite.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2024-04-22 10:10:16.000000 komora_syncer-4.3/komora_syncer/models/netbox/NbTenant.py
+-rw-r--r--   0 root         (0) root         (0)      166 2023-08-25 10:05:04.000000 komora_syncer-4.3/komora_syncer/models/netbox/NetboxBase.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2023-08-25 10:05:04.000000 komora_syncer-4.3/komora_syncer/models/netbox/NetboxCache.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-4.3/komora_syncer/models/netbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:57:35.094989 komora_syncer-4.3/komora_syncer/processors/
+-rw-r--r--   0 root         (0) root         (0)     9043 2023-09-14 11:14:26.000000 komora_syncer-4.3/komora_syncer/processors/Synchronizer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-25 10:05:04.000000 komora_syncer-4.3/komora_syncer/processors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:57:35.094989 komora_syncer-4.3/komora_syncer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-04-26 06:57:34.000000 komora_syncer-4.3/komora_syncer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1554 2024-04-26 06:57:35.000000 komora_syncer-4.3/komora_syncer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 06:57:34.000000 komora_syncer-4.3/komora_syncer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-26 06:57:34.000000 komora_syncer-4.3/komora_syncer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-03 09:25:55.000000 komora_syncer-4.3/komora_syncer.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-26 06:57:34.000000 komora_syncer-4.3/komora_syncer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-26 06:57:34.000000 komora_syncer-4.3/komora_syncer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 06:57:35.098989 komora_syncer-4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1828 2024-04-26 06:57:09.000000 komora_syncer-4.3/setup.py
```

### Comparing `komora_syncer-4.2/PKG-INFO` & `komora_syncer-4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komora_syncer
-Version: 4.2
+Version: 4.3
 Summary: Synchronize data between Komora and Netbox applications
 Home-page: https://gitlab.cesnet.cz/701/done/netbox_komora_syncer
 Author: Jan Krupa
 Author-email: jan.krupa@cesnet.cz
 License: UNKNOWN
 Description: Netbox and Komora synchronizer
         ===
```

### Comparing `komora_syncer-4.2/README.md` & `komora_syncer-4.3/README.md`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/__main__.py` & `komora_syncer-4.3/komora_syncer/__main__.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/config.py` & `komora_syncer-4.3/komora_syncer/config.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/connections/KomoraApi.py` & `komora_syncer-4.3/komora_syncer/connections/KomoraApi.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/connections/KomoraConnection.py` & `komora_syncer-4.3/komora_syncer/connections/KomoraConnection.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/connections/NetboxConnection.py` & `komora_syncer-4.3/komora_syncer/connections/NetboxConnection.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/komora/address.py` & `komora_syncer-4.3/komora_syncer/models/komora/address.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/komora/contact.py` & `komora_syncer-4.3/komora_syncer/models/komora/contact.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/komora/device.py` & `komora_syncer-4.3/komora_syncer/models/komora/device.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/komora/inventory.py` & `komora_syncer-4.3/komora_syncer/models/komora/inventory.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/komora/location.py` & `komora_syncer-4.3/komora_syncer/models/komora/location.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/komora/organization.py` & `komora_syncer-4.3/komora_syncer/models/komora/organization.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/komora/site.py` & `komora_syncer-4.3/komora_syncer/models/komora/site.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/netbox/NbDevice.py` & `komora_syncer-4.3/komora_syncer/models/netbox/NbDevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         else:
             params['custom_fields'] = {"komora_id": self.komora_id, "komora_url": self.komora_url}
 
         return params
 
     @staticmethod
     def get_nb_devices_data():
-        filter_device_roles = NetboxConnection.get_connection().dcim.device_roles.filter(name=["Passive component", "unknown"])
+        filter_device_roles = NetboxConnection.get_connection().dcim.device_roles.filter(name=["Passive component", "unknown", "Server"])
         filter_device_role_ids = json.dumps([str(role.id) for role in filter_device_roles])
         query = NbDevice.get_query(filter_device_role_ids)
 
         try:
             url = get_config()['netbox']['NETBOX_GRAPHQL_URL']
             session = requests.Session()
             req = session.post(url, json={'query': query}, headers={'Authorization': f"Token {get_config()['netbox']['NETBOX_API_TOKEN']}"})
```

### Comparing `komora_syncer-4.2/komora_syncer/models/netbox/NbInventoryItem.py` & `komora_syncer-4.3/komora_syncer/models/netbox/NbInventoryItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,19 +66,18 @@
     @property
     def params(self):
         params = {}
 
         if self.api_object:
             #TODO: Workaround for multiple asset_numbers per item
             if ";" in self.api_object.custom_fields["asset_numbers"] and self.inventory_number in self.api_object.custom_fields["asset_numbers"].split(";"):
-                print("a")
                 params['custom_fields'] = self.api_object.custom_fields
                 params['custom_fields']['komora_id'] = self.api_object.custom_fields["komora_id"]
                 params['custom_fields']['komora_url'] = self.api_object.custom_fields["komora_url"]
-                print(params)
+                logger.debug(params)
 
             elif isinstance(self.api_object.custom_fields, dict):
                 params['custom_fields'] = self.api_object.custom_fields
                 params['custom_fields']['komora_id'] = self.komora_id
                 params['custom_fields']['komora_url'] = self.komora_url
         else:
             params['custom_fields'] = {
```

### Comparing `komora_syncer-4.2/komora_syncer/models/netbox/NbLocation.py` & `komora_syncer-4.3/komora_syncer/models/netbox/NbLocation.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/netbox/NbRegion.py` & `komora_syncer-4.3/komora_syncer/models/netbox/NbRegion.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/netbox/NbSite.py` & `komora_syncer-4.3/komora_syncer/models/netbox/NbSite.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/models/netbox/NbTenant.py` & `komora_syncer-4.3/komora_syncer/models/netbox/NbTenant.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
 class NbTenant(NetboxBase):
     def __init__(self, komora_obj=None):
         super().__init__()
 
         self.name = build_tenant_name(komora_obj.clientId, komora_obj.name)
         self.slug = slugify(self.name)
-        self.description = komora_obj.vipNote.strip()
+        try:
+            self.description = komora_obj.vipNote.strip()
+        except AttributeError:
+            self.description = ""
 
         self.custom_fields = {
             "client_id": komora_obj.clientId,
             "komora_id": komora_obj.id,
             "client_name": komora_obj.name,
             "komora_is_customer": komora_obj.isCustomer
         }
```

### Comparing `komora_syncer-4.2/komora_syncer/models/netbox/NetboxCache.py` & `komora_syncer-4.3/komora_syncer/models/netbox/NetboxCache.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer/processors/Synchronizer.py` & `komora_syncer-4.3/komora_syncer/processors/Synchronizer.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/komora_syncer.egg-info/PKG-INFO` & `komora_syncer-4.3/komora_syncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komora-syncer
-Version: 4.2
+Version: 4.3
 Summary: Synchronize data between Komora and Netbox applications
 Home-page: https://gitlab.cesnet.cz/701/done/netbox_komora_syncer
 Author: Jan Krupa
 Author-email: jan.krupa@cesnet.cz
 License: UNKNOWN
 Description: Netbox and Komora synchronizer
         ===
```

### Comparing `komora_syncer-4.2/komora_syncer.egg-info/SOURCES.txt` & `komora_syncer-4.3/komora_syncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `komora_syncer-4.2/setup.py` & `komora_syncer-4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
       include_package_data=True,
       keywords="netbox,komora",
       packages=find_packages(),
       setup_requires=setup_requirements,
       test_suite="tests",
       tests_require=test_requirements,
       url="https://gitlab.cesnet.cz/701/done/netbox_komora_syncer",
-      version='4.2',
+      version='4.3',
       zip_safe=False,
       python_requires='>=3.6, <4',
       entry_points={
           'console_scripts': [
             'komora_syncer=komora_syncer.__main__:cli',
             ]
       },
```

