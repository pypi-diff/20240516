# Comparing `tmp/goodwe-0.4.1.tar.gz` & `tmp/goodwe-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodwe-0.4.1.tar", last modified: Wed May  8 21:36:00 2024, max compression
+gzip compressed data, was "goodwe-0.4.2.tar", last modified: Thu May 16 21:30:15 2024, max compression
```

## Comparing `goodwe-0.4.1.tar` & `goodwe-0.4.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:36:00.141682 goodwe-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 21:35:52.000000 goodwe-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-08 21:36:00.141682 goodwe-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-08 21:35:52.000000 goodwe-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 21:35:56.000000 goodwe-0.4.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:36:00.141682 goodwe-0.4.1/goodwe/
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22545 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    43517 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/et.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/inverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    24926 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    37640 2024-05-08 21:35:52.000000 goodwe-0.4.1/goodwe/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:36:00.141682 goodwe-0.4.1/goodwe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-08 21:36:00.000000 goodwe-0.4.1/goodwe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 21:36:00.000000 goodwe-0.4.1/goodwe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 21:36:00.000000 goodwe-0.4.1/goodwe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 21:36:00.000000 goodwe-0.4.1/goodwe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 21:35:52.000000 goodwe-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-08 21:36:00.145682 goodwe-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:36:00.141682 goodwe-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-05-08 21:35:52.000000 goodwe-0.4.1/tests/test_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    29091 2024-05-08 21:35:52.000000 goodwe-0.4.1/tests/test_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    68045 2024-05-08 21:35:52.000000 goodwe-0.4.1/tests/test_et.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-08 21:35:52.000000 goodwe-0.4.1/tests/test_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-08 21:35:52.000000 goodwe-0.4.1/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    14011 2024-05-08 21:35:52.000000 goodwe-0.4.1/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:30:15.670645 goodwe-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-16 21:30:06.000000 goodwe-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-16 21:30:15.670645 goodwe-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-16 21:30:06.000000 goodwe-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 21:30:12.000000 goodwe-0.4.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:30:15.670645 goodwe-0.4.2/goodwe/
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43890 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27703 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37679 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:30:15.670645 goodwe-0.4.2/goodwe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-16 21:30:15.000000 goodwe-0.4.2/goodwe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 21:30:15.000000 goodwe-0.4.2/goodwe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:30:15.000000 goodwe-0.4.2/goodwe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 21:30:15.000000 goodwe-0.4.2/goodwe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 21:30:06.000000 goodwe-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 21:30:15.674645 goodwe-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:30:15.670645 goodwe-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29883 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73945 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_sensor.py
```

### Comparing `goodwe-0.4.1/LICENSE` & `goodwe-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.1/PKG-INFO` & `goodwe-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.4.1
+Version: 0.4.2
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.4.1/README.md` & `goodwe-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.1/goodwe/__init__.py` & `goodwe-0.4.2/goodwe/__init__.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.1/goodwe/const.py` & `goodwe-0.4.2/goodwe/const.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.1/goodwe/dt.py` & `goodwe-0.4.2/goodwe/dt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
+import logging
 from typing import Tuple
 
-from .exceptions import InverterError
+from .exceptions import InverterError, RequestRejectedException
 from .inverter import Inverter
 from .inverter import OperationMode
 from .inverter import SensorKind as Kind
+from .modbus import ILLEGAL_DATA_ADDRESS
 from .model import is_3_mppt, is_single_phase
 from .protocol import ProtocolCommand
 from .sensor import *
 
+logger = logging.getLogger(__name__)
+
 
 class DT(Inverter):
     """Class representing inverter of DT/MS/D-NS/XS or GE's GEP(PSB/PSC) families"""
 
     __all_sensors: Tuple[Sensor, ...] = (
         Timestamp("timestamp", 30100, "Timestamp"),
         Voltage("vpv1", 30103, "PV1 Voltage", Kind.PV),
@@ -119,18 +123,15 @@
 
     # Settings for three phase inverters
     __settings_three_phase: Tuple[Sensor, ...] = (
         Integer("grid_export_limit", 40336, "Grid Export Limit", "%", Kind.GRID),
     )
 
     def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
-        super().__init__(host, port, comm_addr, timeout, retries)
-        if not self.comm_addr:
-            # Set the default inverter address
-            self.comm_addr = 0x7f
+        super().__init__(host, port, comm_addr if comm_addr else 0x7f, timeout, retries)
         self._READ_DEVICE_VERSION_INFO: ProtocolCommand = self._read_command(0x7531, 0x0028)
         self._READ_DEVICE_RUNNING_DATA: ProtocolCommand = self._read_command(0x7594, 0x0049)
         self._sensors = self.__all_sensors
         self._settings: dict[str, Sensor] = {s.id_: s for s in self.__all_settings}
 
     @staticmethod
     def _single_phase_only(s: Sensor) -> bool:
@@ -173,25 +174,51 @@
     async def read_runtime_data(self) -> Dict[str, Any]:
         response = await self._read_from_socket(self._READ_DEVICE_RUNNING_DATA)
         data = self._map_response(response, self._sensors)
         return data
 
     async def read_setting(self, setting_id: str) -> Any:
         setting = self._settings.get(setting_id)
-        if not setting:
-            raise ValueError(f'Unknown setting "{setting_id}"')
-        count = (setting.size_ + (setting.size_ % 2)) // 2
-        response = await self._read_from_socket(self._read_command(setting.offset, count))
-        return setting.read_value(response)
+        if setting:
+            return await self._read_setting(setting)
+        else:
+            if setting_id.startswith("modbus"):
+                response = await self._read_from_socket(self._read_command(int(setting_id[7:]), 1))
+                return int.from_bytes(response.read(2), byteorder="big", signed=True)
+            else:
+                raise ValueError(f'Unknown setting "{setting_id}"')
+
+    async def _read_setting(self, setting: Sensor) -> Any:
+        try:
+            count = (setting.size_ + (setting.size_ % 2)) // 2
+            response = await self._read_from_socket(self._read_command(setting.offset, count))
+            return setting.read_value(response)
+        except RequestRejectedException as ex:
+            if ex.message == ILLEGAL_DATA_ADDRESS:
+                logger.debug("Unsupported setting %s", setting.id_)
+                self._settings.pop(setting.id_, None)
+            return None
 
     async def write_setting(self, setting_id: str, value: Any):
         setting = self._settings.get(setting_id)
-        if not setting:
-            raise ValueError(f'Unknown setting "{setting_id}"')
-        raw_value = setting.encode_value(value)
+        if setting:
+            await self._write_setting(setting, value)
+        else:
+            if setting_id.startswith("modbus"):
+                await self._read_from_socket(self._write_command(int(setting_id[7:]), int(value)))
+            else:
+                raise ValueError(f'Unknown setting "{setting_id}"')
+
+    async def _write_setting(self, setting: Sensor, value: Any):
+        if setting.size_ == 1:
+            # modbus can address/store only 16 bit values, read the other 8 bytes
+            response = await self._read_from_socket(self._read_command(setting.offset, 1))
+            raw_value = setting.encode_value(value, response.response_data()[0:2])
+        else:
+            raw_value = setting.encode_value(value)
         if len(raw_value) <= 2:
             value = int.from_bytes(raw_value, byteorder="big", signed=True)
             await self._read_from_socket(self._write_command(setting.offset, value))
         else:
             await self._read_from_socket(self._write_multi_command(setting.offset, raw_value))
 
     async def read_settings_data(self) -> Dict[str, Any]:
```

### Comparing `goodwe-0.4.1/goodwe/es.py` & `goodwe-0.4.2/goodwe/es.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,18 +164,15 @@
         EcoModeV2("eco_mode_3", 47559, "Eco Mode Group 3"),
         ByteH("eco_mode_3_switch", 47561, "Eco Mode Group 3 Switch"),
         EcoModeV2("eco_mode_4", 47565, "Eco Mode Group 4"),
         ByteH("eco_mode_4_switch", 47567, "Eco Mode Group 4 Switch"),
     )
 
     def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
-        super().__init__(host, port, comm_addr, timeout, retries)
-        if not self.comm_addr:
-            # Set the default inverter address
-            self.comm_addr = 0xf7
+        super().__init__(host, port, comm_addr if comm_addr else 0xf7, timeout, retries)
         self._settings: dict[str, Sensor] = {s.id_: s for s in self.__all_settings}
 
     def _supports_eco_mode_v2(self) -> bool:
         if self.arm_version < 14:
             return False
         if "EMU" in self.serial_number:
             return self.dsp1_version >= 11
@@ -216,14 +213,17 @@
             # There does not seem to be time setting/sensor available (or is not known)
             return datetime.now()
         elif setting_id in ('eco_mode_1', 'eco_mode_2', 'eco_mode_3', 'eco_mode_4'):
             setting: Sensor | None = self._settings.get(setting_id)
             if not setting:
                 raise ValueError(f'Unknown setting "{setting_id}"')
             return await self._read_setting(setting)
+        elif setting_id.startswith("modbus"):
+            response = await self._read_from_socket(self._read_command(int(setting_id[7:]), 1))
+            return int.from_bytes(response.read(2), byteorder="big", signed=True)
         else:
             all_settings = await self.read_settings_data()
             return all_settings.get(setting_id)
 
     async def _read_setting(self, setting: Sensor) -> Any:
         count = (setting.size_ + (setting.size_ % 2)) // 2
         if self._is_modbus_setting(setting):
@@ -234,29 +234,30 @@
             return setting.read_value(response)
 
     async def write_setting(self, setting_id: str, value: Any):
         if setting_id == 'time':
             await self._read_from_socket(
                 Aa55ProtocolCommand("030206" + Timestamp("time", 0, "").encode_value(value).hex(), "0382")
             )
+        elif setting_id.startswith("modbus"):
+            await self._read_from_socket(self._write_command(int(setting_id[7:]), int(value)))
         else:
             setting: Sensor | None = self._settings.get(setting_id)
             if not setting:
                 raise ValueError(f'Unknown setting "{setting_id}"')
             await self._write_setting(setting, value)
 
     async def _write_setting(self, setting: Sensor, value: Any):
         if setting.size_ == 1:
             # modbus can address/store only 16 bit values, read the other 8 bytes
             if self._is_modbus_setting(setting):
                 response = await self._read_from_socket(self._read_command(setting.offset, 1))
-                raw_value = setting.encode_value(value, response.response_data()[0:2])
             else:
                 response = await self._read_from_socket(Aa55ReadCommand(setting.offset, 1))
-                raw_value = setting.encode_value(value, response.response_data()[2:4])
+            raw_value = setting.encode_value(value, response.response_data()[0:2])
         else:
             raw_value = setting.encode_value(value)
         if len(raw_value) <= 2:
             value = int.from_bytes(raw_value, byteorder="big", signed=True)
             if self._is_modbus_setting(setting):
                 await self._read_from_socket(self._write_command(setting.offset, value))
             else:
```

### Comparing `goodwe-0.4.1/goodwe/et.py` & `goodwe-0.4.2/goodwe/et.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,18 +453,15 @@
         Integer("backup_mode_enable", 47605, "Backup Mode Switch"),
         Integer("max_charge_power", 47606, "Max Charge Power"),
         Integer("smart_charging_enable", 47609, "Smart Charging Mode Switch"),
         Integer("eco_mode_enable", 47612, "Eco Mode Switch"),
     )
 
     def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
-        super().__init__(host, port, comm_addr, timeout, retries)
-        if not self.comm_addr:
-            # Set the default inverter address
-            self.comm_addr = 0xf7
+        super().__init__(host, port, comm_addr if comm_addr else 0xf7, timeout, retries)
         self._READ_DEVICE_VERSION_INFO: ProtocolCommand = self._read_command(0x88b8, 0x0021)
         self._READ_RUNNING_DATA: ProtocolCommand = self._read_command(0x891c, 0x007d)
         self._READ_METER_DATA: ProtocolCommand = self._read_command(0x8ca0, 0x2d)
         self._READ_METER_DATA_EXTENDED: ProtocolCommand = self._read_command(0x8ca0, 0x3a)
         self._READ_BATTERY_INFO: ProtocolCommand = self._read_command(0x9088, 0x0018)
         self._READ_BATTERY2_INFO: ProtocolCommand = self._read_command(0x9858, 0x0016)
         self._READ_MPPT_DATA: ProtocolCommand = self._read_command(0x89e5, 0x3d)
@@ -607,34 +604,43 @@
                 else:
                     raise ex
 
         return data
 
     async def read_setting(self, setting_id: str) -> Any:
         setting = self._settings.get(setting_id)
-        if not setting:
-            raise ValueError(f'Unknown setting "{setting_id}"')
-        try:
+        if setting:
             return await self._read_setting(setting)
+        else:
+            if setting_id.startswith("modbus"):
+                response = await self._read_from_socket(self._read_command(int(setting_id[7:]), 1))
+                return int.from_bytes(response.read(2), byteorder="big", signed=True)
+            else:
+                raise ValueError(f'Unknown setting "{setting_id}"')
+
+    async def _read_setting(self, setting: Sensor) -> Any:
+        try:
+            count = (setting.size_ + (setting.size_ % 2)) // 2
+            response = await self._read_from_socket(self._read_command(setting.offset, count))
+            return setting.read_value(response)
         except RequestRejectedException as ex:
             if ex.message == ILLEGAL_DATA_ADDRESS:
                 logger.debug("Unsupported setting %s", setting.id_)
-                self._settings.pop(setting_id, None)
+                self._settings.pop(setting.id_, None)
             return None
 
-    async def _read_setting(self, setting: Sensor) -> Any:
-        count = (setting.size_ + (setting.size_ % 2)) // 2
-        response = await self._read_from_socket(self._read_command(setting.offset, count))
-        return setting.read_value(response)
-
     async def write_setting(self, setting_id: str, value: Any):
         setting = self._settings.get(setting_id)
-        if not setting:
-            raise ValueError(f'Unknown setting "{setting_id}"')
-        await self._write_setting(setting, value)
+        if setting:
+            await self._write_setting(setting, value)
+        else:
+            if setting_id.startswith("modbus"):
+                await self._read_from_socket(self._write_command(int(setting_id[7:]), int(value)))
+            else:
+                raise ValueError(f'Unknown setting "{setting_id}"')
 
     async def _write_setting(self, setting: Sensor, value: Any):
         if setting.size_ == 1:
             # modbus can address/store only 16 bit values, read the other 8 bytes
             response = await self._read_from_socket(self._read_command(setting.offset, 1))
             raw_value = setting.encode_value(value, response.response_data()[0:2])
         else:
```

### Comparing `goodwe-0.4.1/goodwe/exceptions.py` & `goodwe-0.4.2/goodwe/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,9 +25,23 @@
         message -- rejection reason
     """
 
     def __init__(self, message: str = ''):
         self.message: str = message
 
 
+class PartialResponseException(InverterError):
+    """
+    Indicates the received response data are incomplete and is probably fragmented to multiple packets.
+
+    Attributes:
+        length -- received data length
+        expected -- expected data lenght
+    """
+
+    def __init__(self, lenght: int, expected: int):
+        self.length: int = lenght
+        self.expected: int = expected
+
+
 class MaxRetriesException(InverterError):
     """Indicates the maximum number of retries has been reached"""
```

### Comparing `goodwe-0.4.1/goodwe/inverter.py` & `goodwe-0.4.2/goodwe/inverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,17 @@
 class Inverter(ABC):
     """
     Common superclass for various inverter models implementations.
     Represents the inverter state and its basic behavior
     """
 
     def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
-        self._protocol: InverterProtocol = self._create_protocol(host, port, timeout, retries)
+        self._protocol: InverterProtocol = self._create_protocol(host, port, comm_addr, timeout, retries)
         self._consecutive_failures_count: int = 0
-
-        self.comm_addr: int = comm_addr
+        self.keep_alive: bool = True
 
         self.model_name: str | None = None
         self.serial_number: str | None = None
         self.rated_power: int = 0
         self.ac_output_type: int | None = None
         self.firmware: str | None = None
         self.arm_firmware: str | None = None
@@ -105,36 +104,39 @@
         self.dsp2_version: int = 0
         self.dsp_svn_version: int | None = None
         self.arm_version: int = 0
         self.arm_svn_version: int | None = None
 
     def _read_command(self, offset: int, count: int) -> ProtocolCommand:
         """Create read protocol command."""
-        return self._protocol.read_command(self.comm_addr, offset, count)
+        return self._protocol.read_command(offset, count)
 
     def _write_command(self, register: int, value: int) -> ProtocolCommand:
         """Create write protocol command."""
-        return self._protocol.write_command(self.comm_addr, register, value)
+        return self._protocol.write_command(register, value)
 
     def _write_multi_command(self, offset: int, values: bytes) -> ProtocolCommand:
         """Create write multiple protocol command."""
-        return self._protocol.write_multi_command(self.comm_addr, offset, values)
+        return self._protocol.write_multi_command(offset, values)
 
     async def _read_from_socket(self, command: ProtocolCommand) -> ProtocolResponse:
         try:
             result = await command.execute(self._protocol)
             self._consecutive_failures_count = 0
             return result
         except MaxRetriesException:
             self._consecutive_failures_count += 1
             raise RequestFailedException(f'No valid response received even after {self._protocol.retries} retries',
                                          self._consecutive_failures_count) from None
         except RequestFailedException as ex:
             self._consecutive_failures_count += 1
             raise RequestFailedException(ex.message, self._consecutive_failures_count) from None
+        finally:
+            if not self.keep_alive:
+                self._protocol.close_transport()
 
     @abstractmethod
     async def read_device_info(self):
         """
         Request the device information from the inverter.
         The inverter instance variables will be loaded with relevant data.
         """
@@ -266,19 +268,19 @@
     def settings(self) -> Tuple[Sensor, ...]:
         """
         Return tuple of settings definitions
         """
         raise NotImplementedError()
 
     @staticmethod
-    def _create_protocol(host: str, port: int, timeout: int, retries: int) -> InverterProtocol:
+    def _create_protocol(host: str, port: int, comm_addr: int, timeout: int, retries: int) -> InverterProtocol:
         if port == 502:
-            return TcpInverterProtocol(host, port, timeout, retries)
+            return TcpInverterProtocol(host, port, comm_addr, timeout, retries)
         else:
-            return UdpInverterProtocol(host, port, timeout, retries)
+            return UdpInverterProtocol(host, port, comm_addr, timeout, retries)
 
     @staticmethod
     def _map_response(response: ProtocolResponse, sensors: Tuple[Sensor, ...]) -> Dict[str, Any]:
         """Process the response data and return dictionary with runtime values"""
         result = {}
         for sensor in sensors:
             try:
```

### Comparing `goodwe-0.4.1/goodwe/modbus.py` & `goodwe-0.4.2/goodwe/modbus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 from typing import Union
 
-from .exceptions import RequestRejectedException
+from .exceptions import PartialResponseException, RequestRejectedException
 
 logger = logging.getLogger(__name__)
 
 MODBUS_READ_CMD: int = 0x3
 MODBUS_WRITE_CMD: int = 0x6
 MODBUS_WRITE_MULTI_CMD: int = 0x10
 
-ILLEGAL_DATA_ADDRESS = 'ILLEGAL DATA ADDRESS'
+ILLEGAL_DATA_ADDRESS: str = 'ILLEGAL DATA ADDRESS'
 
 FAILURE_CODES = {
     1: "ILLEGAL FUNCTION",
     2: ILLEGAL_DATA_ADDRESS,
     3: "ILLEGAL DATA VALUE",
     4: "SLAVE DEVICE FAILURE",
     5: "ACKNOWLEDGE",
@@ -174,16 +174,15 @@
         return False
     if data[3] == MODBUS_READ_CMD:
         if data[4] != value * 2:
             logger.debug("Response has unexpected length: %d, expected %d.", data[4], value * 2)
             return False
         expected_length = data[4] + 7
         if len(data) < expected_length:
-            logger.debug("Response is too short: %d, expected %d.", len(data), expected_length)
-            return False
+            raise PartialResponseException(len(data), expected_length)
     elif data[3] in (MODBUS_WRITE_CMD, MODBUS_WRITE_MULTI_CMD):
         if len(data) < 10:
             logger.debug("Response has unexpected length: %d, expected %d.", len(data), 10)
             return False
         expected_length = 10
         response_offset = int.from_bytes(data[4:6], byteorder='big', signed=False)
         if response_offset != offset:
@@ -218,26 +217,26 @@
     data[6] is source address
     data[7] is command return type
     data[8] is response payload length (for read commands)
     """
     if len(data) <= 8:
         logger.debug("Response is too short.")
         return False
+    expected_length = int.from_bytes(data[4:6], byteorder='big', signed=False) + 6
+    if len(data) < expected_length:
+        raise PartialResponseException(len(data), expected_length)
+
     if data[7] == MODBUS_READ_CMD:
         if data[8] != value * 2:
             logger.debug("Response has unexpected length: %d, expected %d.", data[8], value * 2)
             return False
-        expected_length = data[8] + 9
-        if len(data) < expected_length:
-            logger.debug("Response is too short: %d, expected %d.", len(data), expected_length)
-            return False
     elif data[7] in (MODBUS_WRITE_CMD, MODBUS_WRITE_MULTI_CMD):
         if len(data) < 12:
             logger.debug("Response has unexpected length: %d, expected %d.", len(data), 14)
-            return False
+            raise PartialResponseException(len(data), expected_length)
         response_offset = int.from_bytes(data[8:10], byteorder='big', signed=False)
         if response_offset != offset:
             logger.debug("Response has wrong offset: %X, expected %X.", response_offset, offset)
             return False
         response_value = int.from_bytes(data[10:12], byteorder='big', signed=True)
         if response_value != value:
             logger.debug("Response has wrong value: %X, expected %X.", response_value, value)
```

### Comparing `goodwe-0.4.1/goodwe/model.py` & `goodwe-0.4.2/goodwe/model.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.1/goodwe/protocol.py` & `goodwe-0.4.2/goodwe/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 from __future__ import annotations
 
 import asyncio
 import io
 import logging
+import platform
+import socket
 from asyncio.futures import Future
 from typing import Tuple, Optional, Callable
 
-from .exceptions import MaxRetriesException, RequestFailedException, RequestRejectedException
+from .exceptions import MaxRetriesException, PartialResponseException, RequestFailedException, RequestRejectedException
 from .modbus import create_modbus_rtu_request, create_modbus_rtu_multi_request, create_modbus_tcp_request, \
     create_modbus_tcp_multi_request, validate_modbus_rtu_response, validate_modbus_tcp_response, MODBUS_READ_CMD, \
     MODBUS_WRITE_CMD, MODBUS_WRITE_MULTI_CMD
 
 logger = logging.getLogger(__name__)
 
+_modbus_tcp_tx = 0
+
+
+def _next_tx() -> bytes:
+    global _modbus_tcp_tx
+    _modbus_tcp_tx += 1
+    if _modbus_tcp_tx == 0xFFFF:
+        _modbus_tcp_tx = 1
+    return int.to_bytes(_modbus_tcp_tx, length=2, byteorder="big", signed=False)
+
 
 class InverterProtocol:
 
-    def __init__(self, host: str, port: int, timeout: int, retries: int):
+    def __init__(self, host: str, port: int, comm_addr: int, timeout: int, retries: int):
         self._host: str = host
         self._port: int = port
+        self._comm_addr: int = comm_addr
         self._running_loop: asyncio.AbstractEventLoop | None = None
         self._lock: asyncio.Lock | None = None
         self._timer: asyncio.TimerHandle | None = None
         self.timeout: int = timeout
         self.retries: int = retries
         self.protocol: asyncio.Protocol | None = None
         self.response_future: Future | None = None
         self.command: ProtocolCommand | None = None
+        self._partial_data: bytes | None = None
 
     def _ensure_lock(self) -> asyncio.Lock:
         """Validate (or create) asyncio Lock.
 
            The asyncio.Lock must always be created from within's asyncio loop,
            so it cannot be eagerly created in constructor.
            Additionally, since asyncio.run() creates and closes its own loop,
@@ -39,53 +53,55 @@
         """
         if self._lock and self._running_loop == asyncio.get_event_loop():
             return self._lock
         else:
             logger.debug("Creating lock instance for current event loop.")
             self._lock = asyncio.Lock()
             self._running_loop = asyncio.get_event_loop()
-            self._close_transport()
+            self.close_transport()
             return self._lock
 
-    def _close_transport(self) -> None:
+    def close_transport(self) -> None:
+        """Close the underlying transport/connection."""
         raise NotImplementedError()
 
     async def send_request(self, command: ProtocolCommand) -> Future:
+        """Convert command to request and send it to inverter."""
         raise NotImplementedError()
 
-    def read_command(self, comm_addr: int, offset: int, count: int) -> ProtocolCommand:
+    def read_command(self, offset: int, count: int) -> ProtocolCommand:
         """Create read protocol command."""
         raise NotImplementedError()
 
-    def write_command(self, comm_addr: int, register: int, value: int) -> ProtocolCommand:
+    def write_command(self, register: int, value: int) -> ProtocolCommand:
         """Create write protocol command."""
         raise NotImplementedError()
 
-    def write_multi_command(self, comm_addr: int, offset: int, values: bytes) -> ProtocolCommand:
+    def write_multi_command(self, offset: int, values: bytes) -> ProtocolCommand:
         """Create write multiple protocol command."""
         raise NotImplementedError()
 
 
 class UdpInverterProtocol(InverterProtocol, asyncio.DatagramProtocol):
-    def __init__(self, host: str, port: int, timeout: int = 1, retries: int = 3):
-        super().__init__(host, port, timeout, retries)
+    def __init__(self, host: str, port: int, comm_addr: int, timeout: int = 1, retries: int = 3):
+        super().__init__(host, port, comm_addr, timeout, retries)
         self._transport: asyncio.transports.DatagramTransport | None = None
         self._retry: int = 0
 
-    def read_command(self, comm_addr: int, offset: int, count: int) -> ProtocolCommand:
+    def read_command(self, offset: int, count: int) -> ProtocolCommand:
         """Create read protocol command."""
-        return ModbusRtuReadCommand(comm_addr, offset, count)
+        return ModbusRtuReadCommand(self._comm_addr, offset, count)
 
-    def write_command(self, comm_addr: int, register: int, value: int) -> ProtocolCommand:
+    def write_command(self, register: int, value: int) -> ProtocolCommand:
         """Create write protocol command."""
-        return ModbusRtuWriteCommand(comm_addr, register, value)
+        return ModbusRtuWriteCommand(self._comm_addr, register, value)
 
-    def write_multi_command(self, comm_addr: int, offset: int, values: bytes) -> ProtocolCommand:
+    def write_multi_command(self, offset: int, values: bytes) -> ProtocolCommand:
         """Create write multiple protocol command."""
-        return ModbusRtuWriteMultiCommand(comm_addr, offset, values)
+        return ModbusRtuWriteMultiCommand(self._comm_addr, offset, values)
 
     async def _connect(self) -> None:
         if not self._transport or self._transport.is_closing():
             self._transport, self.protocol = await asyncio.get_running_loop().create_datagram_endpoint(
                 lambda: self,
                 remote_addr=(self._host, self._port),
             )
@@ -96,38 +112,51 @@
 
     def connection_lost(self, exc: Optional[Exception]) -> None:
         """On connection lost"""
         if exc:
             logger.debug("Socket closed with error: %s.", exc)
         else:
             logger.debug("Socket closed.")
-        self._close_transport()
+        self.close_transport()
 
     def datagram_received(self, data: bytes, addr: Tuple[str, int]) -> None:
         """On datagram received"""
         if self._timer:
             self._timer.cancel()
             self._timer = None
         try:
+            if self._partial_data:
+                logger.debug("Received another response fragment: %s.", data.hex())
+                data = self._partial_data + data
             if self.command.validator(data):
-                logger.debug("Received: %s", data.hex())
+                if self._partial_data:
+                    logger.debug("Composed fragmented response: %s", data.hex())
+                else:
+                    logger.debug("Received: %s", data.hex())
+                self._partial_data = None
                 self.response_future.set_result(data)
             else:
                 logger.debug("Received invalid response: %s", data.hex())
                 asyncio.get_running_loop().call_soon(self._retry_mechanism)
+        except PartialResponseException:
+            logger.debug("Received response fragment: %s", data.hex())
+            self._partial_data = data
+            return
+        except asyncio.InvalidStateError:
+            logger.debug("Response already handled: %s", data.hex())
         except RequestRejectedException as ex:
             logger.debug("Received exception response: %s", data.hex())
             self.response_future.set_exception(ex)
-            self._close_transport()
+            self.close_transport()
 
     def error_received(self, exc: Exception) -> None:
         """On error received"""
         logger.debug("Received error: %s", exc)
         self.response_future.set_exception(exc)
-        self._close_transport()
+        self.close_transport()
 
     async def send_request(self, command: ProtocolCommand) -> Future:
         """Send message via transport"""
         async with self._ensure_lock():
             await self._connect()
             response_future = asyncio.get_running_loop().create_future()
             self._retry = 0
@@ -135,111 +164,135 @@
             await response_future
             return response_future
 
     def _send_request(self, command: ProtocolCommand, response_future: Future) -> None:
         """Send message via transport"""
         self.command = command
         self.response_future = response_future
-        logger.debug("Sending: %s%s", self.command,
-                     f' - retry #{self._retry}/{self.retries}' if self._retry > 0 else '')
-        self._transport.sendto(self.command.request)
+        payload = command.request_bytes()
+        if self._retry > 0:
+            logger.debug("Sending: %s - retry #%s/%s", self.command, self._retry, self.retries)
+        else:
+            logger.debug("Sending: %s", self.command)
+        self._transport.sendto(payload)
         self._timer = asyncio.get_running_loop().call_later(self.timeout, self._retry_mechanism)
 
     def _retry_mechanism(self) -> None:
         """Retry mechanism to prevent hanging transport"""
         if self.response_future.done():
             logger.debug("Response already received.")
         elif self._retry < self.retries:
             if self._timer:
                 logger.debug("Failed to receive response to %s in time (%ds).", self.command, self.timeout)
             self._retry += 1
             self._send_request(self.command, self.response_future)
         else:
             logger.debug("Max number of retries (%d) reached, request %s failed.", self.retries, self.command)
             self.response_future.set_exception(MaxRetriesException)
-            self._close_transport()
+            self.close_transport()
 
-    def _close_transport(self) -> None:
+    def close_transport(self) -> None:
         if self._transport:
             try:
                 self._transport.close()
             except RuntimeError:
                 logger.debug("Failed to close transport.")
             self._transport = None
         # Cancel Future on connection close
         if self.response_future and not self.response_future.done():
             self.response_future.cancel()
 
 
 class TcpInverterProtocol(InverterProtocol, asyncio.Protocol):
-    def __init__(self, host: str, port: int, timeout: int = 1, retries: int = 0):
-        super().__init__(host, port, timeout, retries)
+    def __init__(self, host: str, port: int, comm_addr: int, timeout: int = 1, retries: int = 0):
+        super().__init__(host, port, comm_addr, timeout, retries)
         self._transport: asyncio.transports.Transport | None = None
         self._retry: int = 0
 
-    def read_command(self, comm_addr: int, offset: int, count: int) -> ProtocolCommand:
+    def read_command(self, offset: int, count: int) -> ProtocolCommand:
         """Create read protocol command."""
-        return ModbusTcpReadCommand(comm_addr, offset, count)
+        return ModbusTcpReadCommand(self._comm_addr, offset, count)
 
-    def write_command(self, comm_addr: int, register: int, value: int) -> ProtocolCommand:
+    def write_command(self, register: int, value: int) -> ProtocolCommand:
         """Create write protocol command."""
-        return ModbusTcpWriteCommand(comm_addr, register, value)
+        return ModbusTcpWriteCommand(self._comm_addr, register, value)
 
-    def write_multi_command(self, comm_addr: int, offset: int, values: bytes) -> ProtocolCommand:
+    def write_multi_command(self, offset: int, values: bytes) -> ProtocolCommand:
         """Create write multiple protocol command."""
-        return ModbusTcpWriteMultiCommand(comm_addr, offset, values)
+        return ModbusTcpWriteMultiCommand(self._comm_addr, offset, values)
 
     async def _connect(self) -> None:
         if not self._transport or self._transport.is_closing():
             logger.debug("Opening connection.")
             self._transport, self.protocol = await asyncio.get_running_loop().create_connection(
                 lambda: self,
                 host=self._host, port=self._port,
             )
+            sock = self._transport.get_extra_info('socket')
+            if sock is not None:
+                sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+                sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPIDLE, 10)
+                sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPINTVL, 10)
+                sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPCNT, 3)
+                if platform.system() == 'Windows':
+                    sock.ioctl(socket.SIO_KEEPALIVE_VALS, (1, 10000, 10000))
 
     def connection_made(self, transport: asyncio.DatagramTransport) -> None:
         """On connection made"""
         logger.debug("Connection opened.")
         pass
 
     def eof_received(self) -> None:
         logger.debug("EOF received.")
-        self._close_transport()
+        self.close_transport()
 
     def connection_lost(self, exc: Optional[Exception]) -> None:
         """On connection lost"""
         if exc:
             logger.debug("Connection closed with error: %s.", exc)
         else:
             logger.debug("Connection closed.")
-        self._close_transport()
+        self.close_transport()
 
     def data_received(self, data: bytes) -> None:
         """On data received"""
         if self._timer:
             self._timer.cancel()
         try:
+            if self._partial_data:
+                logger.debug("Received another response fragment: %s.", data.hex())
+                data = self._partial_data + data
             if self.command.validator(data):
-                logger.debug("Received: %s", data.hex())
+                if self._partial_data:
+                    logger.debug("Composed fragmented response: %s", data.hex())
+                else:
+                    logger.debug("Received: %s", data.hex())
                 self._retry = 0
+                self._partial_data = None
                 self.response_future.set_result(data)
             else:
                 logger.debug("Received invalid response: %s", data.hex())
                 self.response_future.set_exception(RequestRejectedException())
-                self._close_transport()
+                self.close_transport()
+        except PartialResponseException:
+            logger.debug("Received response fragment: %s", data.hex())
+            self._partial_data = data
+            return
+        except asyncio.InvalidStateError:
+            logger.debug("Response already handled: %s", data.hex())
         except RequestRejectedException as ex:
             logger.debug("Received exception response: %s", data.hex())
             self.response_future.set_exception(ex)
-            # self._close_transport()
+            # self.close_transport()
 
     def error_received(self, exc: Exception) -> None:
         """On error received"""
         logger.debug("Received error: %s", exc)
         self.response_future.set_exception(exc)
-        self._close_transport()
+        self.close_transport()
 
     async def send_request(self, command: ProtocolCommand) -> Future:
         """Send message via transport"""
         await self._ensure_lock().acquire()
         try:
             await asyncio.wait_for(self._connect(), timeout=5)
             response_future = asyncio.get_running_loop().create_future()
@@ -249,19 +302,19 @@
         except asyncio.CancelledError:
             if self._retry < self.retries:
                 if self._timer:
                     logger.debug("Connection broken error.")
                 self._retry += 1
                 if self._lock and self._lock.locked():
                     self._lock.release()
-                self._close_transport()
+                self.close_transport()
                 return await self.send_request(command)
             else:
                 return self._max_retries_reached()
-        except (ConnectionRefusedError, TimeoutError, OSError, asyncio.TimeoutError) as exc:
+        except (ConnectionRefusedError, TimeoutError, OSError, asyncio.TimeoutError):
             if self._retry < self.retries:
                 logger.debug("Connection refused error.")
                 self._retry += 1
                 if self._lock and self._lock.locked():
                     self._lock.release()
                 return await self.send_request(command)
             else:
@@ -270,37 +323,40 @@
             if self._lock and self._lock.locked():
                 self._lock.release()
 
     def _send_request(self, command: ProtocolCommand, response_future: Future) -> None:
         """Send message via transport"""
         self.command = command
         self.response_future = response_future
-        logger.debug("Sending: %s%s", self.command,
-                     f' - retry #{self._retry}/{self.retries}' if self._retry > 0 else '')
-        self._transport.write(self.command.request)
+        payload = command.request_bytes()
+        if self._retry > 0:
+            logger.debug("Sending: %s - retry #%s/%s", self.command, self._retry, self.retries)
+        else:
+            logger.debug("Sending: %s", self.command)
+        self._transport.write(payload)
         self._timer = asyncio.get_running_loop().call_later(self.timeout, self._timeout_mechanism)
 
     def _timeout_mechanism(self) -> None:
         """Retry mechanism to prevent hanging transport"""
         if self.response_future.done():
             self._retry = 0
         else:
             if self._timer:
                 logger.debug("Failed to receive response to %s in time (%ds).", self.command, self.timeout)
                 self._timer = None
-            self._close_transport()
+            self.close_transport()
 
     def _max_retries_reached(self) -> Future:
         logger.debug("Max number of retries (%d) reached, request %s failed.", self.retries, self.command)
-        self._close_transport()
+        self.close_transport()
         self.response_future = asyncio.get_running_loop().create_future()
         self.response_future.set_exception(MaxRetriesException)
         return self.response_future
 
-    def _close_transport(self) -> None:
+    def close_transport(self) -> None:
         if self._transport:
             try:
                 self._transport.close()
             except RuntimeError:
                 logger.debug("Failed to close transport.")
             self._transport = None
         # Cancel Future on connection lost
@@ -350,14 +406,18 @@
 
     def __hash__(self):
         return hash(self.request)
 
     def __repr__(self):
         return self.request.hex()
 
+    def request_bytes(self) -> bytes:
+        """Return raw bytes payload, optionally pre-processed"""
+        return self.request
+
     def trim_response(self, raw_response: bytes):
         """Trim raw response from header and checksum data"""
         return raw_response
 
     def get_offset(self, address: int):
         """Calculate relative offset to start of the response bytes"""
         return address
@@ -563,14 +623,20 @@
         super().__init__(
             request,
             lambda x: validate_modbus_tcp_response(x, cmd, offset, value),
         )
         self.first_address: int = offset
         self.value = value
 
+    def request_bytes(self) -> bytes:
+        """Return raw bytes payload, optionally pre-processed"""
+        # Apply sequential Modbus/TCP transaction identifier
+        self.request = _next_tx() + self.request[2:]
+        return self.request
+
     def trim_response(self, raw_response: bytes):
         """Trim raw response from header and checksum data"""
         return raw_response[9:]
 
     def get_offset(self, address: int):
         """Calculate relative offset to start of the response bytes"""
         return (address - self.first_address) * 2
```

### Comparing `goodwe-0.4.1/goodwe/sensor.py` & `goodwe-0.4.2/goodwe/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,26 +179,26 @@
     """Sensor representing energy [kWh] value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "kWh", kind)
 
     def read_value(self, data: ProtocolResponse):
         value = read_bytes2(data)
-        return float(value) / 10 if value else None
+        return float(value) / 10 if value is not None else None
 
 
 class Energy4(Sensor):
     """Sensor representing energy [kWh] value encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 4, "kWh", kind)
 
     def read_value(self, data: ProtocolResponse):
         value = read_bytes4(data)
-        return float(value) / 10 if value else None
+        return float(value) / 10 if value is not None else None
 
 
 class Apparent(Sensor):
     """Sensor representing apparent power [VA] value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "VA", kind)
@@ -906,15 +906,15 @@
 
 
 def read_temp(buffer: ProtocolResponse, offset: int = None) -> float | None:
     """Retrieve temperature [C] value (2 bytes) from buffer"""
     if offset is not None:
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(2), byteorder="big", signed=True)
-    if value == 32767:
+    if value == -1 or value == 32767:
         return None
     else:
         return float(value) / 10
 
 
 def read_datetime(buffer: ProtocolResponse, offset: int = None) -> datetime:
     """Retrieve datetime value (6 bytes) from buffer"""
```

### Comparing `goodwe-0.4.1/goodwe.egg-info/PKG-INFO` & `goodwe-0.4.2/goodwe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.4.1
+Version: 0.4.2
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.4.1/setup.cfg` & `goodwe-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.1/tests/test_dt.py` & `goodwe-0.4.2/tests/test_dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         self.assertSensor('work_mode', 0, '', data)
         self.assertSensor('work_mode_label', 'Wait Mode', '', data)
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('warning_code', 0, '', data)
         self.assertSensor("apparent_power", -1, "VA", data),
         self.assertSensor("reactive_power", -1, "var", data),
         self.assertSensor('temperature', 1.4, 'C', data)
-        self.assertSensor('e_day', None, 'kWh', data)
+        self.assertSensor('e_day', 0, 'kWh', data)
         self.assertSensor('e_total', 881.7, 'kWh', data)
         self.assertSensor('h_total', 955, 'h', data)
         self.assertSensor('safety_country', 73, '', data)
         self.assertSensor('safety_country_label', 'Australia Victoria', '', data)
         self.assertSensor('funbit', 2400, '', data)
         self.assertSensor('vbus', 291.7, 'V', data)
         self.assertSensor('vnbus', 0, 'V', data)
```

### Comparing `goodwe-0.4.1/tests/test_es.py` & `goodwe-0.4.2/tests/test_es.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime
 from unittest import TestCase
 
 from goodwe import DISCOVERY_COMMAND
 from goodwe.es import ES
 from goodwe.exceptions import RequestFailedException
 from goodwe.inverter import OperationMode
-from goodwe.protocol import ProtocolCommand, ProtocolResponse
+from goodwe.protocol import Aa55ReadCommand, ProtocolCommand, ProtocolResponse
 
 
 class EsMock(TestCase, ES):
 
     def __init__(self, methodName='runTest'):
         TestCase.__init__(self, methodName)
         ES.__init__(self, "localhost", 8899)
@@ -22,14 +22,16 @@
         self._mock_responses[command] = filename
 
     async def _read_from_socket(self, command: ProtocolCommand) -> ProtocolResponse:
         """Mock UDP communication"""
         root_dir = os.path.dirname(os.path.abspath(__file__))
         filename = self._mock_responses.get(command)
         if filename is not None:
+            if filename.startswith('aa55'):
+                return ProtocolResponse(bytes.fromhex(filename), command)
             with open(root_dir + '/sample/es/' + filename, 'r') as f:
                 response = bytes.fromhex(f.read())
                 if not command.validator(response):
                     raise RequestFailedException
                 return ProtocolResponse(response, command)
         else:
             self.request = command.request
@@ -48,14 +50,16 @@
 class GW5048D_ES_Test(EsMock):
 
     def __init__(self, methodName='runTest'):
         EsMock.__init__(self, methodName)
         self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW5048D-ES_device_info.hex')
         self.mock_response(self._READ_DEVICE_RUNNING_DATA, 'GW5048D-ES_running_data.hex')
         self.mock_response(self._READ_DEVICE_SETTINGS_DATA, 'GW5048D-ES_settings_data.hex')
+        self.mock_response(Aa55ReadCommand(1793, 1), 'aa557fc0019a08000000000000007f0360')
+        self.mock_response(Aa55ReadCommand(1800, 1), 'aa557fc0019a02007f035a')
 
     def test_GW5048D_ES_device_info(self):
         self.loop.run_until_complete(self.read_device_info())
         self.assertEqual('GW5048D-ES', self.model_name)
         self.assertEqual('95048ESU227W0000', self.serial_number)
         self.assertEqual('2323G', self.firmware)
         self.assertEqual(23, self.dsp1_version)
@@ -159,14 +163,24 @@
         data = self.loop.run_until_complete(self.read_setting('discharge_v'))
         self.assertEqual(44.5, data)
         data = self.loop.run_until_complete(self.read_setting('dod'))
         self.assertEqual(0, data)
         data = self.loop.run_until_complete(self.read_setting('grid_export_limit'))
         self.assertEqual(10000, data)
 
+        data = self.loop.run_until_complete(self.read_setting('eco_mode_1'))
+        self.assertEqual(
+            "EcoModeV1(id_='eco_mode_1', offset=1793, name='Eco Mode Group 1', size_=8, unit='', kind=<SensorKind.BAT: 4>)",
+            repr(data))
+        data = self.loop.run_until_complete(self.read_setting('eco_mode_2_switch'))
+        self.assertEqual(0, data)
+
+    def test_write_setting(self):
+        self.loop.run_until_complete(self.write_setting('eco_mode_2_switch', 0))
+
 
 class GW5048_EM_Test(EsMock):
 
     def __init__(self, methodName='runTest'):
         EsMock.__init__(self, methodName)
         self.mock_response(self._READ_DEVICE_RUNNING_DATA, 'GW5048-EM_running_data.hex')
         self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW5048-EM_device_info.hex')
```

### Comparing `goodwe-0.4.1/tests/test_et.py` & `goodwe-0.4.2/tests/test_et.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,17 @@
 
     def __init__(self, methodName='runTest'):
         EtMock.__init__(self, methodName)
         self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW10K-ET_device_info_fw617.hex')
         self.mock_response(self._READ_RUNNING_DATA, 'GW10K-ET_running_data.hex')
         self.mock_response(self._READ_METER_DATA, 'GW10K-ET_meter_data.hex')
         self.mock_response(self._READ_BATTERY_INFO, 'GW10K-ET_battery_info.hex')
-        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47547, 6), ILLEGAL_DATA_ADDRESS)
-        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47589, 6), ILLEGAL_DATA_ADDRESS)
-        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47515, 4), 'eco_mode_v1.hex')
+        self.mock_response(ModbusRtuReadCommand(0xf7, 47547, 6), ILLEGAL_DATA_ADDRESS)
+        self.mock_response(ModbusRtuReadCommand(0xf7, 47589, 6), ILLEGAL_DATA_ADDRESS)
+        self.mock_response(ModbusRtuReadCommand(0xf7, 47515, 4), 'eco_mode_v1.hex')
 
     def test_GW10K_ET_device_info(self):
         self.loop.run_until_complete(self.read_device_info())
         self.assertEqual('GW10K-ET', self.model_name)
         self.assertEqual('9010KETU000W0000', self.serial_number)
         self.assertEqual(10000, self.rated_power)
         self.assertEqual(1, self.modbus_version)
@@ -163,15 +163,15 @@
         self.assertSensor('errors', '', '', data)
         self.assertSensor("e_total", 6085.3, 'kWh', data)
         self.assertSensor("e_day", 12.5, 'kWh', data)
         self.assertSensor("e_total_exp", 4718.6, 'kWh', data)
         self.assertSensor('h_total', 9246, 'h', data)
         self.assertSensor("e_day_exp", 9.8, 'kWh', data)
         self.assertSensor("e_total_imp", 58.0, 'kWh', data)
-        self.assertSensor("e_day_imp", None, 'kWh', data)
+        self.assertSensor("e_day_imp", 0, 'kWh', data)
         self.assertSensor("e_load_total", 8820.2, 'kWh', data)
         self.assertSensor("e_load_day", 11.6, 'kWh', data)
         self.assertSensor("e_bat_charge_total", 2758.1, 'kWh', data)
         self.assertSensor("e_bat_charge_day", 5.3, 'kWh', data)
         self.assertSensor("e_bat_discharge_total", 2442.1, 'kWh', data)
         self.assertSensor("e_bat_discharge_day", 2.9, 'kWh', data)
         self.assertSensor('diagnose_result', 117442560, '', data)
@@ -251,18 +251,24 @@
 
         self.loop.run_until_complete(self.read_setting('grid_export_limit'))
         self.assertEqual('f703b996000155ec', self.request.hex())
 
         self.loop.run_until_complete(self.read_setting('time'))
         self.assertEqual('f703b090000337b0', self.request.hex())
 
+        self.loop.run_until_complete(self.read_setting('modbus_47000'))
+        self.assertEqual('f703b798000136c7', self.request.hex())
+
     def test_GW10K_ET_write_setting(self):
         self.loop.run_until_complete(self.write_setting('grid_export_limit', 100))
         self.assertEqual('f706b996006459c7', self.request.hex())
 
+        self.loop.run_until_complete(self.write_setting('modbus_47510', 100))
+        self.assertEqual('f706b996006459c7', self.request.hex())
+
         self.loop.run_until_complete(self.write_setting('time', datetime(2022, 1, 4, 18, 30, 25)))
         self.assertEqual('f710b090000306160104121e19a961', self.request.hex())
 
     def test_get_grid_export_limit(self):
         self.loop.run_until_complete(self.get_grid_export_limit())
         self.assertEqual('f703b996000155ec', self.request.hex())
 
@@ -309,16 +315,16 @@
 
 
 class GW10K_ET_fw819_Test(EtMock):
 
     def __init__(self, methodName='runTest'):
         EtMock.__init__(self, methodName)
         self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW10K-ET_device_info_fw819.hex')
-        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47547, 6), 'eco_mode_v2.hex')
-        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47589, 6), ILLEGAL_DATA_ADDRESS)
+        self.mock_response(ModbusRtuReadCommand(0xf7, 47547, 6), 'eco_mode_v2.hex')
+        self.mock_response(ModbusRtuReadCommand(0xf7, 47589, 6), ILLEGAL_DATA_ADDRESS)
         asyncio.get_event_loop().run_until_complete(self.read_device_info())
 
     def test_GW10K_ET_fw819_device_info(self):
         self.assertEqual('0GW10K-ET', self.model_name)
         self.assertEqual('9010KETU00000000', self.serial_number)
         self.assertEqual(10000, self.rated_power)
         self.assertEqual(1, self.modbus_version)
@@ -351,14 +357,15 @@
 
 
 class GW10K_ET_fw1023_Test(EtMock):
 
     def __init__(self, methodName='runTest'):
         EtMock.__init__(self, methodName)
         self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW10K-ET_device_info_fw1023.hex')
+        self.mock_response(self._READ_RUNNING_DATA, 'GW10K-ET_running_data_fw1023.hex')
         asyncio.get_event_loop().run_until_complete(self.read_device_info())
 
     def test_GW10K_ET_fw1023_device_info(self):
         self.assertEqual('GW10K-ET', self.model_name)
         self.assertEqual('9010KETU000W0000', self.serial_number)
         self.assertEqual(10000, self.rated_power)
         self.assertEqual(2, self.modbus_version)
@@ -372,14 +379,114 @@
         self.assertEqual('02041-23-S00', self.arm_firmware)
 
     def test_GW10K_ET_setting_fw1023(self):
         self.assertEqual(80, len(self.settings()))
         settings = {s.id_: s for s in self.settings()}
         self.assertEqual('PeakShavingMode', type(settings.get("peak_shaving_mode")).__name__)
 
+    def test_GW10K_ET_runtime_data_fw1023(self):
+        # Reset sensors
+        self.loop.run_until_complete(self.read_device_info())
+        self.sensor_map = {s.id_: s.unit for s in self.sensors()}
+
+        data = self.loop.run_until_complete(self.read_runtime_data())
+        self.assertEqual(145, len(data))
+
+        self.assertSensor('timestamp', datetime.strptime('2024-05-11 00:03:34', '%Y-%m-%d %H:%M:%S'), '', data)
+        self.assertSensor('vpv1', 0.0, 'V', data)
+        self.assertSensor('ipv1', 0.0, 'A', data)
+        self.assertSensor('ppv1', 0, 'W', data)
+        self.assertSensor('vpv2', 0.0, 'V', data)
+        self.assertSensor('ipv2', 0.0, 'A', data)
+        self.assertSensor('ppv2', 0, 'W', data)
+        self.assertSensor('ppv', 0, 'W', data)
+        self.assertSensor('pv2_mode', 0, '', data)
+        self.assertSensor('pv2_mode_label', 'PV panels not connected', '', data)
+        self.assertSensor('pv1_mode', 0, '', data)
+        self.assertSensor('pv1_mode_label', 'PV panels not connected', '', data)
+        self.assertSensor('vgrid', 244.4, 'V', data)
+        self.assertSensor('igrid', 2.0, 'A', data)
+        self.assertSensor('fgrid', 49.92, 'Hz', data)
+        self.assertSensor('pgrid', 435, 'W', data)
+        self.assertSensor('vgrid2', 244.3, 'V', data)
+        self.assertSensor('igrid2', 1.2, 'A', data)
+        self.assertSensor('fgrid2', 49.92, 'Hz', data)
+        self.assertSensor('pgrid2', 241, 'W', data)
+        self.assertSensor('vgrid3', 244.9, 'V', data)
+        self.assertSensor('igrid3', 0.8, 'A', data)
+        self.assertSensor('fgrid3', 49.92, 'Hz', data)
+        self.assertSensor('pgrid3', 132, 'W', data)
+        self.assertSensor('grid_mode', 1, '', data)
+        self.assertSensor('grid_mode_label', 'Connected to grid', '', data)
+        self.assertSensor('total_inverter_power', 812, 'W', data)
+        self.assertSensor('active_power', -11, 'W', data)
+        self.assertSensor('grid_in_out', 0, '', data)
+        self.assertSensor('grid_in_out_label', 'Idle', '', data)
+        self.assertSensor('reactive_power', 0, 'var', data)
+        self.assertSensor('apparent_power', 0, 'VA', data)
+        self.assertSensor('backup_v1', 244.2, 'V', data)
+        self.assertSensor('backup_i1', 1.3, 'A', data)
+        self.assertSensor('backup_f1', 49.92, 'Hz', data)
+        self.assertSensor('load_mode1', 1, '', data)
+        self.assertSensor('backup_p1', 217, 'W', data)
+        self.assertSensor('backup_v2', 243.8, 'V', data)
+        self.assertSensor('backup_i2', 0.6, 'A', data)
+        self.assertSensor('backup_f2', 49.92, 'Hz', data)
+        self.assertSensor('load_mode2', 1, '', data)
+        self.assertSensor('backup_p2', 114, 'W', data)
+        self.assertSensor('backup_v3', 244.7, 'V', data)
+        self.assertSensor('backup_i3', 0.3, 'A', data)
+        self.assertSensor('backup_f3', 49.92, 'Hz', data)
+        self.assertSensor('load_mode3', 1, '', data)
+        self.assertSensor('backup_p3', 5, 'W', data)
+        self.assertSensor('load_p1', 129, 'W', data)
+        self.assertSensor('load_p2', 108, 'W', data)
+        self.assertSensor('load_p3', 247, 'W', data)
+        self.assertSensor('backup_ptotal', 321, 'W', data)
+        self.assertSensor('load_ptotal', 502, 'W', data)
+        self.assertSensor('ups_load', 5, '%', data)
+        self.assertSensor('temperature_air', 36.4, 'C', data)
+        self.assertSensor('temperature_module', 0.0, 'C', data)
+        self.assertSensor('temperature', 32.5, 'C', data)
+        self.assertSensor('function_bit', 16384, '', data)
+        self.assertSensor('bus_voltage', 790.7, 'V', data)
+        self.assertSensor('nbus_voltage', 395.1, 'V', data)
+        self.assertSensor('vbattery1', 397.1, 'V', data)
+        self.assertSensor('ibattery1', 2.0, 'A', data)
+        self.assertSensor('pbattery1', 820, 'W', data)
+        self.assertSensor('battery_mode', 2, '', data)
+        self.assertSensor('battery_mode_label', 'Discharge', '', data)
+        self.assertSensor('warning_code', 0, '', data)
+        self.assertSensor('safety_country', 32, '', data)
+        self.assertSensor('safety_country_label', '50Hz 230Vac Default', '', data)
+        self.assertSensor('work_mode', 1, '', data)
+        self.assertSensor('work_mode_label', 'Normal (On-Grid)', '', data)
+        self.assertSensor('operation_mode', 0, '', data)
+        self.assertSensor('error_codes', 0, '', data)
+        self.assertSensor('errors', '', '', data)
+        self.assertSensor('e_total', 30630.9, 'kWh', data)
+        self.assertSensor('e_day', 0, 'kWh', data)
+        self.assertSensor('e_total_exp', 27208.5, 'kWh', data)
+        self.assertSensor('h_total', 33055, 'h', data)
+        self.assertSensor('e_day_exp', 0, 'kWh', data)
+        self.assertSensor('e_total_imp', 70.3, 'kWh', data)
+        self.assertSensor('e_day_imp', 0, 'kWh', data)
+        self.assertSensor('e_load_total', 35366.4, 'kWh', data)
+        self.assertSensor('e_load_day', 0, 'kWh', data)
+        self.assertSensor('e_bat_charge_total', 9884.3, 'kWh', data)
+        self.assertSensor('e_bat_charge_day', 0, 'kWh', data)
+        self.assertSensor('e_bat_discharge_total', 8642.2, 'kWh', data)
+        self.assertSensor('e_bat_discharge_day', 0.1, 'kWh', data)
+        self.assertSensor('diagnose_result', 33554496, '', data)
+        self.assertSensor('diagnose_result_label', 'Discharge Driver On, PF value set', '', data)
+        self.assertSensor('house_consumption', 831, 'W', data)
+        self.assertSensor('commode', 515, '', data)
+        self.assertSensor('rssi', 1029, '', data)
+        self.assertSensor('manufacture_code', 1543, '', data)
+
 
 class GW6000_EH_Test(EtMock):
 
     def __init__(self, methodName='runTest'):
         EtMock.__init__(self, methodName)
         self.mock_response(self._READ_RUNNING_DATA, 'GW6000_EH_running_data.hex')
         self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW6000_EH_device_info.hex')
@@ -456,22 +563,22 @@
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('errors', '', '', data)
         self.assertSensor("e_total", 59.4, 'kWh', data)
         self.assertSensor("e_day", 22.0, 'kWh', data)
         self.assertSensor("e_total_exp", 58.6, 'kWh', data)
         self.assertSensor('h_total', 33, 'h', data)
         self.assertSensor("e_day_exp", 21.6, 'kWh', data)
-        self.assertSensor("e_total_imp", None, 'kWh', data)
-        self.assertSensor("e_day_imp", None, 'kWh', data)
+        self.assertSensor("e_total_imp", 0, 'kWh', data)
+        self.assertSensor("e_day_imp", 0, 'kWh', data)
         self.assertSensor("e_load_total", 70.1, 'kWh', data)
         self.assertSensor("e_load_day", 27.1, 'kWh', data)
-        self.assertSensor("e_bat_charge_total", None, 'kWh', data)
-        self.assertSensor("e_bat_charge_day", None, 'kWh', data)
-        self.assertSensor("e_bat_discharge_total", None, 'kWh', data)
-        self.assertSensor("e_bat_discharge_day", None, 'kWh', data)
+        self.assertSensor("e_bat_charge_total", 0, 'kWh', data)
+        self.assertSensor("e_bat_charge_day", 0, 'kWh', data)
+        self.assertSensor("e_bat_discharge_total", 0, 'kWh', data)
+        self.assertSensor("e_bat_discharge_day", 0, 'kWh', data)
         self.assertSensor('diagnose_result', 117983303, '', data)
         self.assertSensor('diagnose_result_label',
                           'Battery voltage low, Battery SOC low, Battery SOC in back, Discharge Driver On, Self-use load light, Battery Disconnected, Self-use off, Export power limit set, PF value set, Real power limit set',
                           '', data)
         self.assertSensor('house_consumption', 1712, 'W', data)
 
 
@@ -557,16 +664,16 @@
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('errors', '', '', data)
         self.assertSensor('e_total', 10225.8, 'kWh', data)
         self.assertSensor('e_day', 23.1, 'kWh', data)
         self.assertSensor('e_total_exp', 10273.3, 'kWh', data)
         self.assertSensor('h_total', 3256, 'h', data)
         self.assertSensor('e_day_exp', 16.6, 'kWh', data)
-        self.assertSensor('e_total_imp', None, 'kWh', data)
-        self.assertSensor('e_day_imp', None, 'kWh', data)
+        self.assertSensor('e_total_imp', 0, 'kWh', data)
+        self.assertSensor('e_day_imp', 0, 'kWh', data)
         self.assertSensor('e_load_total', 4393.9, 'kWh', data)
         self.assertSensor('e_load_day', 10.7, 'kWh', data)
         self.assertSensor('e_bat_charge_total', 141.9, 'kWh', data)
         self.assertSensor('e_bat_charge_day', 9.6, 'kWh', data)
         self.assertSensor('e_bat_discharge_total', 117.5, 'kWh', data)
         self.assertSensor('e_bat_discharge_day', 2.6, 'kWh', data)
         self.assertSensor('diagnose_result', 33556864, '', data)
@@ -770,15 +877,15 @@
         self.assertSensor('e_total_imp', 14.8, 'kWh', data)
         self.assertSensor('e_day_imp', 1.0, 'kWh', data)
         self.assertSensor('e_load_total', 17.2, 'kWh', data)
         self.assertSensor('e_load_day', 0.2, 'kWh', data)
         self.assertSensor('e_bat_charge_total', 91.3, 'kWh', data)
         self.assertSensor('e_bat_charge_day', 11.0, 'kWh', data)
         self.assertSensor('e_bat_discharge_total', 69.6, 'kWh', data)
-        self.assertSensor('e_bat_discharge_day', None, 'kWh', data)
+        self.assertSensor('e_bat_discharge_day', 0, 'kWh', data)
         self.assertSensor('diagnose_result', 33816960, '', data)
         self.assertSensor('diagnose_result_label',
                           'BMS: Discharge current low, APP: Discharge current too low, BMS: Charge disabled, PF value set',
                           '', data)
         self.assertSensor('house_consumption', 503, 'W', data)
         self.assertSensor('battery_bms', 255, '', data)
         self.assertSensor('battery_index', 311, '', data)
@@ -1041,21 +1148,21 @@
         self.assertSensor('errors', '', '', data)
         self.assertSensor('e_total', 4562.3, 'kWh', data)
         self.assertSensor('e_day', 0.9, 'kWh', data)
         self.assertSensor('e_total_exp', 4489.7, 'kWh', data)
         self.assertSensor('h_total', 1175, 'h', data)
         self.assertSensor('e_day_exp', 1.2, 'kWh', data)
         self.assertSensor('e_total_imp', 8.7, 'kWh', data)
-        self.assertSensor('e_day_imp', None, 'kWh', data)
+        self.assertSensor('e_day_imp', 0, 'kWh', data)
         self.assertSensor('e_load_total', 10742.2, 'kWh', data)
         self.assertSensor('e_load_day', 43.8, 'kWh', data)
-        self.assertSensor('e_bat_charge_total', None, 'kWh', data)
-        self.assertSensor('e_bat_charge_day', None, 'kWh', data)
-        self.assertSensor('e_bat_discharge_total', None, 'kWh', data)
-        self.assertSensor('e_bat_discharge_day', None, 'kWh', data)
+        self.assertSensor('e_bat_charge_total', 0, 'kWh', data)
+        self.assertSensor('e_bat_charge_day', 0, 'kWh', data)
+        self.assertSensor('e_bat_discharge_total', 0, 'kWh', data)
+        self.assertSensor('e_bat_discharge_day', 0, 'kWh', data)
         self.assertSensor('diagnose_result', 33816782, '', data)
         self.assertSensor('diagnose_result_label',
                           'Battery SOC low, Battery SOC in back, BMS: Discharge disabled, '
                           'Discharge Driver On, BMS: Discharge current low, BMS: Charge disabled, PF value set',
                           '', data)
         self.assertSensor('house_consumption', 6950, 'W', data)
         self.assertSensor('commode', 0, '', data)
@@ -1202,15 +1309,15 @@
 
 
 class GW5K_BT_Test(EtMock):
 
     def __init__(self, methodName='runTest'):
         EtMock.__init__(self, methodName)
         self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW5K-BT_device_info.hex')
-        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47547, 6), 'NO RESPONSE')
+        self.mock_response(ModbusRtuReadCommand(0xf7, 47547, 6), 'NO RESPONSE')
 
     def test_GW5K_BT_device_info(self):
         self.loop.run_until_complete(self.read_device_info())
         self.assertEqual('GW5K-BT', self.model_name)
         self.assertEqual('95000BTU203W0000', self.serial_number)
         self.assertEqual(5000, self.rated_power)
         self.assertEqual(0, self.modbus_version)
```

### Comparing `goodwe-0.4.1/tests/test_modbus.py` & `goodwe-0.4.2/tests/test_modbus.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
     def assert_rtu_response_ok(self, response: str, cmd: int, offset: int, value: int):
         self.assertTrue(validate_modbus_rtu_response(bytes.fromhex(response), cmd, offset, value))
 
     def assert_rtu_response_fail(self, response: str, cmd: int, offset: int, value: int):
         self.assertFalse(validate_modbus_rtu_response(bytes.fromhex(response), cmd, offset, value))
 
+    def assert_rtu_response_partial(self, response: str, cmd: int, offset: int, value: int):
+        self.assertRaises(PartialResponseException,
+                          lambda: validate_modbus_rtu_response(bytes.fromhex(response), cmd, offset, value))
+
     def assert_rtu_response_rejected(self, response: str, cmd: int, offset: int, value: int):
         self.assertRaises(RequestRejectedException,
                           lambda: validate_modbus_rtu_response(bytes.fromhex(response), cmd, offset, value))
 
     def test_create_modbus_rtu_request(self):
         request = create_modbus_rtu_request(0x11, 0x3, 0x006b, 0x0003)
         self.assertEqual('1103006b00037687', request.hex())
@@ -31,15 +35,15 @@
         self.assertEqual('f71088b8000306010203040506102e', request.hex())
 
     def test_validate_modbus_rtu_read_response(self):
         self.assert_rtu_response_ok('aa55f7030401020304cd33', 0x03, 0x0401, 2)
         # some garbage after response end
         self.assert_rtu_response_ok('aa55f7030401020304cd33ffffff', 0x03, 0x0401, 2)
         # length too short
-        self.assert_rtu_response_fail('aa55f7030401020304', 0x03, 0x0401, 2)
+        self.assert_rtu_response_partial('aa55f7030401020304', 0x03, 0x0401, 2)
         # wrong checksum
         self.assert_rtu_response_fail('aa55f70304010203043346', 0x03, 0x0401, 2)
         # failure code
         self.assert_rtu_response_rejected('aa55f783040102030405b35e', 0x03, 0x0401, 2)
         # unexpected message length
         self.assert_rtu_response_fail('aa55f70306010203040506b417', 0x03, 0x0401, 2)
 
@@ -68,14 +72,18 @@
 
     def assert_tcp_response_ok(self, response: str, cmd: int, offset: int, value: int):
         self.assertTrue(validate_modbus_tcp_response(bytes.fromhex(response), cmd, offset, value))
 
     def assert_tcp_response_fail(self, response: str, cmd: int, offset: int, value: int):
         self.assertFalse(validate_modbus_tcp_response(bytes.fromhex(response), cmd, offset, value))
 
+    def assert_tcp_response_partial(self, response: str, cmd: int, offset: int, value: int):
+        self.assertRaises(PartialResponseException,
+                          lambda: validate_modbus_tcp_response(bytes.fromhex(response), cmd, offset, value))
+
     def assert_tcp_response_rejected(self, response: str, cmd: int, offset: int, value: int):
         self.assertRaises(RequestRejectedException,
                           lambda: validate_modbus_tcp_response(bytes.fromhex(response), cmd, offset, value))
 
     def test_create_modbus_tcp_request(self):
         request = create_modbus_tcp_request(0x11, 0x3, 0x006b, 0x0003)
         self.assertEqual('0001000000061103006b0003', request.hex())
@@ -89,23 +97,23 @@
         request = create_modbus_tcp_request(0xf7, 0x6, 0x88b8, -1)
         self.assertEqual('000100000006f70688b8ffff', request.hex())
 
     def test_create_modbus_tcp_multi_request(self):
         request = create_modbus_tcp_multi_request(0xf7, 0x10, 0x88b8, b'\x01\x02\x03\x04\x05\x06')
         self.assertEqual('00010000000df71088b8000306010203040506', request.hex())
 
-    def test_validate_modbus_rtu_read_response(self):
+    def test_validate_modbus_tcp_read_response(self):
         self.assert_tcp_response_ok('000100000007b4030445565345', 0x3, 310, 2)
         self.assert_tcp_response_ok('000100000007b4030400000002', 0x3, 331, 2)
         # length too short
-        self.assert_tcp_response_fail('000100000007b403040000', 0x03, 331, 2)
+        self.assert_tcp_response_partial('000100000007b403040000', 0x03, 331, 2)
         # failure code
         self.assert_tcp_response_rejected('000100000007b4830400000002', 0x03, 331, 2)
 
     def test_validate_modbus_tcp_write_response(self):
         self.assert_tcp_response_ok('000100000006b40601364556', 0x06, 310, 0x4556)
         self.assert_tcp_response_ok('000100000006f70688b80021', 0x06, 0x88b8, 0x0021)
         #        self.assert_tcp_response_ok('000100000006f70688b800ff', 0x06, 0xb12c, -1)
         # length too short
-        self.assert_tcp_response_fail('000100000006f70388b8', 0x6, 0x88b8, 0x0021)
+        self.assert_tcp_response_partial('000100000006f70388b8', 0x6, 0x88b8, 0x0021)
         # wrong value written
         self.assert_rtu_response_fail('aa55f706b12c0012fba4', 0x06, 0xb12c, 0x14)
```

### Comparing `goodwe-0.4.1/tests/test_protocol.py` & `goodwe-0.4.2/tests/test_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest import TestCase, mock
 
 from goodwe.protocol import *
 
 
 class TestUDPClientProtocol(TestCase):
     def setUp(self) -> None:
-        self.protocol = UdpInverterProtocol('127.0.0.1', 1337, 1, 3)
+        self.protocol = UdpInverterProtocol('127.0.0.1', 1337, 0xf7, 1, 3)
         self.protocol.command = ProtocolCommand(bytes.fromhex('636f666665650d0a'), lambda x: True)
         self.protocol.response_future = mock.Mock()
 
     def test_datagram_received(self):
         data = b'this is mock data'
         self.protocol.datagram_received(data, ('127.0.0.1', 1337))
         self.protocol.response_future.set_result.assert_called_once()
```

### Comparing `goodwe-0.4.1/tests/test_sensor.py` & `goodwe-0.4.2/tests/test_sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,22 @@
         testee = Energy4("", 0, "", None)
 
         data = MockResponse("00020972")
         self.assertEqual(13349.0, testee.read(data))
         data = MockResponse("ffffffff")
         self.assertIsNone(testee.read(data))
 
+    def test_temp(self):
+        testee = Temp("", 0, "", None)
+
+        data = MockResponse("0177")
+        self.assertEqual(37.5, testee.read(data))
+        data = MockResponse("ffff")
+        self.assertIsNone(testee.read(data))
+
     def test_timestamp(self):
         testee = Timestamp("", 0, "", None)
 
         data = MockResponse("160104121e19")
         self.assertEqual(datetime(2022, 1, 4, 18, 30, 25), testee.read(data))
         self.assertEqual("160104121e19", testee.encode_value(datetime(2022, 1, 4, 18, 30, 25)).hex())
         self.assertEqual("160104121e19", testee.encode_value("2022-01-04T18:30:25").hex())
```

