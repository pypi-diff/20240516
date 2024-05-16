# Comparing `tmp/rfb_driver_ea-0.0.2.tar.gz` & `tmp/rfb_driver_ea-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfb_driver_ea-0.0.2.tar", last modified: Mon Apr 22 07:19:44 2024, max compression
+gzip compressed data, was "rfb_driver_ea-0.0.3.tar", last modified: Thu May 16 09:54:09 2024, max compression
```

## Comparing `rfb_driver_ea-0.0.2.tar` & `rfb_driver_ea-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:19:44.644804 rfb_driver_ea-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-04-22 07:19:44.644804 rfb_driver_ea-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:19:44.644804 rfb_driver_ea-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:19:44.640804 rfb_driver_ea-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:19:44.640804 rfb_driver_ea-0.0.2/src/rfb_driver_ea/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    22541 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea/drv_ea.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:19:44.640804 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:54:09.706729 rfb_driver_ea-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-05-16 09:54:09.702729 rfb_driver_ea-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:54:09.706729 rfb_driver_ea-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:54:09.702729 rfb_driver_ea-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:54:09.702729 rfb_driver_ea-0.0.3/src/rfb_driver_ea/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25331 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea/drv_ea.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:54:09.702729 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/top_level.txt
```

### Comparing `rfb_driver_ea-0.0.2/LICENSE.txt` & `rfb_driver_ea-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rfb_driver_ea-0.0.2/PKG-INFO` & `rfb_driver_ea-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-driver-ea
-Version: 0.0.2
+Version: 0.0.3
 Summary: Driver to control EA Power Electronics devices.
 Author-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 Maintainer-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rfb_driver_ea-0.0.2/pyproject.toml` & `rfb_driver_ea-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rfb_driver_ea-0.0.2/src/rfb_driver_ea/context.py` & `rfb_driver_ea-0.0.3/src/rfb_driver_ea/context.py`

 * *Files identical despite different names*

### Comparing `rfb_driver_ea-0.0.2/src/rfb_driver_ea/drv_ea.py` & `rfb_driver_ea-0.0.3/src/rfb_driver_ea/drv_ea.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,19 +113,21 @@
             - None.
         '''
         super().__init__()
         self.__tx_chan = SysShdIpcChanC(name = DEFAULT_TX_CHAN)
         self.__rx_chan = SysShdIpcChanC(name = DEFAULT_RX_CHAN+'_'+config.port.split('/')[-1],
                                       max_msg = DEFAULT_MAX_MSG,
                                       max_message_size = DEFAULT_MAX_MESSAGE_SIZE)
+        sleep(1)
         self.__port = config.port
+        self.__config = config
         add_msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.ADD_DEV,
-                                  port = config.port,
-                                  payload = config,
-                                  rx_chan_name = DEFAULT_RX_CHAN+'_'+config.port.split('/')[-1])
+                                  port = self.__port,
+                                  payload = self.__config,
+                                  rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1])
         self.__tx_chan.send_data(add_msg)
         self.__rx_chan.delete_until_last()
         self.__wait_4_response: bool = False
         self.__request_data: int = 0
         self.__last_mode: DrvBasePwrModeE = DrvBasePwrModeE.DISABLE
         self.last_data: DrvEaDataC = DrvEaDataC(mode = DrvBasePwrModeE.DISABLE,
                                                 status = DrvBaseStatusE.OK,
@@ -158,65 +160,80 @@
 
         Returns:
             None
         """
         i = 0
         while i < DEFAULT_MAX_READS and not self.__rx_chan.is_empty(): #pylint: disable=too-many-nested-blocks
             msg: DrvScpiCmdDataC = self.__rx_chan.receive_data_unblocking()
-            if msg is not None and msg.data_type == DrvScpiCmdTypeE.RESP: #pylint: disable=too-many-nested-blocks
-                if hasattr(msg, 'status') and msg.status.value == DrvBaseStatusE.COMM_ERROR: #pylint: disable=attribute-defined-outside-init
-                    log.critical("ERROR READING DEVICE")
-                    self.last_data.status = DrvBaseStatusC(DrvBaseStatusE.COMM_ERROR) #pylint: disable=attribute-defined-outside-init
-                for data in msg.payload: #pylint: disable=too-many-nested-blocks #pylint: disable=attribute-defined-outside-init
-                    if len(data) >0 and not str(data).startswith(":"):
-                        if 'No error' in data:
-                            self.last_data.status = DrvBaseStatusC(DrvBaseStatusE.OK) #pylint: disable=attribute-defined-outside-init
-                        elif all (x in data for x in ("error", "Error", "ERROR")):
-                            log.error(f"Error reading device: {data}")
-                            self.last_data.status = DrvBaseStatusC(DrvBaseStatusE.COMM_ERROR) #pylint: disable=attribute-defined-outside-init
-                        elif 'OFF' in data:
-                            self.last_data.mode = self.__last_mode #pylint: disable=attribute-defined-outside-init
-                        elif ('ON' in data and self.last_data.mode in (DrvBasePwrModeE.WAIT,
-                                                                    DrvBasePwrModeE.DISABLE)):
-                            self.last_data.mode = self.__last_mode #pylint: disable=attribute-defined-outside-init
-                        elif data.startswith('EA') or data.startswith('EPS'):
-                            data = data.split(',')
-                            self.properties.model = data[1].replace(" ","") #pylint: disable=attribute-defined-outside-init
-                            self.properties.serial_number = data[2].replace(" ", "") #pylint: disable=attribute-defined-outside-init
-                            log.debug(f"Serial number: {data[2]}")
-                            log.debug(f"Model: {data[1]}")
-                        elif all(x in data for x in ("V,", "A,", "W")):
-                            meas_data = data.split(',')
-                            voltage = int(float(meas_data[0].replace('V', '')) * _MILI_UNITS)
-                            self.last_data.voltage = voltage #pylint: disable=attribute-defined-outside-init
-                            current = int(float(meas_data[1].replace('A', '')) * _MILI_UNITS)
-                            self.last_data.current = current #pylint: disable=attribute-defined-outside-init
-                            power = int(float(meas_data[2].replace('W', '')) * _MILI_UNITS)
-                            self.last_data.power = power #pylint: disable=attribute-defined-outside-init
-                            log.debug(f"Voltage: {voltage}, Current: {current}")
-                            log.debug(f"Power: {power} mW, last mode: {self.__last_mode}")
-                            if ((power != 0 or (voltage > 0 and current != 0))
-                                and self.__last_mode != DrvBasePwrModeE.DISABLE):
+            if msg is not None:
+                log.critical(f"Message received: {msg.data_type.name}")
+                if msg.data_type == DrvScpiCmdTypeE.ERROR:
+
+                    log.critical("ERROR DEVICE NOT ADDED IN SCPI")
+                    add_msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.ADD_DEV,
+                                    port = self.__port,
+                                    payload = self.__config,
+                                    rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1])
+                    self.__tx_chan.send_data(add_msg)
+                    add_msg = DrvScpiCmdDataC(data_type = msg.last_order,
+                                    port = self.__port,
+                                    payload = msg.payload,
+                                    rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1])
+                    self.__tx_chan.send_data(add_msg)
+                elif msg.data_type == DrvScpiCmdTypeE.RESP: #pylint: disable=too-many-nested-blocks
+                    if hasattr(msg, 'status') and msg.status.value == DrvBaseStatusE.COMM_ERROR: #pylint: disable=attribute-defined-outside-init
+                        log.critical("ERROR READING DEVICE")
+                        self.last_data.status = DrvBaseStatusC(DrvBaseStatusE.COMM_ERROR) #pylint: disable=attribute-defined-outside-init
+                    for data in msg.payload: #pylint: disable=too-many-nested-blocks #pylint: disable=attribute-defined-outside-init
+                        if len(data) >0 and not str(data).startswith(":"):
+                            if 'No error' in data:
+                                self.last_data.status = DrvBaseStatusC(DrvBaseStatusE.OK) #pylint: disable=attribute-defined-outside-init
+                            elif all (x in data for x in ("error", "Error", "ERROR")):
+                                log.error(f"Error reading device: {data}")
+                                self.last_data.status = DrvBaseStatusC(DrvBaseStatusE.COMM_ERROR) #pylint: disable=attribute-defined-outside-init
+                            elif 'OFF' in data:
                                 self.last_data.mode = self.__last_mode #pylint: disable=attribute-defined-outside-init
-                            else:
-                                if self.__last_mode == DrvBasePwrModeE.WAIT:
-                                    self.last_data.mode = DrvBasePwrModeE.WAIT #pylint: disable=attribute-defined-outside-init
+                            elif ('ON' in data and self.last_data.mode in (DrvBasePwrModeE.WAIT,
+                                                                        DrvBasePwrModeE.DISABLE)):
+                                self.last_data.mode = self.__last_mode #pylint: disable=attribute-defined-outside-init
+                            elif data.startswith('EA') or data.startswith('EPS'):
+                                data = data.split(',')
+                                self.properties.model = data[1].replace(" ","") #pylint: disable=attribute-defined-outside-init
+                                self.properties.serial_number = data[2].replace(" ", "") #pylint: disable=attribute-defined-outside-init
+                                log.debug(f"Serial number: {data[2]}")
+                                log.debug(f"Model: {data[1]}")
+                            elif all(x in data for x in ("V,", "A,", "W")):
+                                meas_data = data.split(',')
+                                voltage = int(float(meas_data[0].replace('V', '')) * _MILI_UNITS)
+                                self.last_data.voltage = voltage #pylint: disable=attribute-defined-outside-init
+                                current = int(float(meas_data[1].replace('A', '')) * _MILI_UNITS)
+                                self.last_data.current = current #pylint: disable=attribute-defined-outside-init
+                                power = int(float(meas_data[2].replace('W', '')) * _MILI_UNITS)
+                                self.last_data.power = power #pylint: disable=attribute-defined-outside-init
+                                log.debug(f"Voltage: {voltage}, Current: {current}")
+                                log.debug(f"Power: {power} mW, last mode: {self.__last_mode}")
+                                if ((power != 0 or (voltage > 0 and current != 0))
+                                    and self.__last_mode != DrvBasePwrModeE.DISABLE):
+                                    self.last_data.mode = self.__last_mode #pylint: disable=attribute-defined-outside-init
                                 else:
-                                    self.last_data.mode = DrvBasePwrModeE.DISABLE #pylint: disable=attribute-defined-outside-init
-                            self.__wait_4_response = False
-                        elif "W" in data and len(data.split(' ')) == 2:
-                            max_power = int(float(data.split(' ')[0]) * _MILI_UNITS)
-                            self.properties.max_power_limit = max_power #pylint: disable=attribute-defined-outside-init
-                        elif "V" in data and len(data.split(' ')) == 2:
-                            max_volt = int(float(data.split(' ')[0]) * _MILI_UNITS)
-                            self.properties.max_volt_limit = max_volt #pylint: disable=attribute-defined-outside-init
-                        elif "A" in data and len(data.split(' ')) == 2:
-                            max_curr = int(float(data.split(' ')[0]) * _MILI_UNITS)
-                            self.properties.max_current_limit = max_curr #pylint: disable=attribute-defined-outside-init
-                        log.debug(f"Response: {data}")
+                                    if self.__last_mode == DrvBasePwrModeE.WAIT:
+                                        self.last_data.mode = DrvBasePwrModeE.WAIT #pylint: disable=attribute-defined-outside-init
+                                    else:
+                                        self.last_data.mode = DrvBasePwrModeE.DISABLE #pylint: disable=attribute-defined-outside-init
+                                self.__wait_4_response = False
+                            elif "W" in data and len(data.split(' ')) == 2:
+                                max_power = int(float(data.split(' ')[0]) * _MILI_UNITS)
+                                self.properties.max_power_limit = max_power #pylint: disable=attribute-defined-outside-init
+                            elif "V" in data and len(data.split(' ')) == 2:
+                                max_volt = int(float(data.split(' ')[0]) * _MILI_UNITS)
+                                self.properties.max_volt_limit = max_volt #pylint: disable=attribute-defined-outside-init
+                            elif "A" in data and len(data.split(' ')) == 2:
+                                max_curr = int(float(data.split(' ')[0]) * _MILI_UNITS)
+                                self.properties.max_current_limit = max_curr #pylint: disable=attribute-defined-outside-init
+                            log.debug(f"Response: {data}")
             elif msg is None:
                 pass
             else:
                 log.error(f'Unknown message type received: {msg.__dict__}')
             i += 1
 
     def __initialize_control(self) -> None:
@@ -225,14 +242,15 @@
             - None.
         Returns:
             - None.
         Raises:
             - None.
         '''
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                              rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                               port = self.__port,
                               payload = _ScpiCmds.LOCK_ON.value)
         self.__tx_chan.send_data(msg)
         self.read_buffer()
         self.disable()
 
 
@@ -243,14 +261,15 @@
         Returns:
             - None.
         Raises:
             - ConnectionError: Device not found.
         '''
         #Model and serial number
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = _ScpiCmds.READ_INFO.value)
         self.__tx_chan.send_data(msg)
         self.read_buffer()
         #Max current limit
         self.__get_nominal_value(_ScpiCmds.CURR_NOM.value)
         #Max voltage limit
         self.__get_nominal_value(_ScpiCmds.VOLT_NOM.value)
@@ -265,14 +284,15 @@
             - payload (str): Payload of the message.
         Returns:
             - result (int): Nominal value.
         Raises:
             - None.
         '''
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = payload)
         self.__tx_chan.send_data(msg)
         # Try to read message
         self.read_buffer()
 
     def get_data(self) -> DrvEaDataC:
         '''Read the device data.
@@ -287,14 +307,15 @@
         if self.__request_data >= DEFAULT_MAX_REQUESTS:
             self.__wait_4_response = False
             self.__request_data = 0
         self.__tx_chan.close()
         self.__tx_chan = SysShdIpcChanC(name = DEFAULT_TX_CHAN)
         if not self.__wait_4_response:
             self.__tx_chan.send_data(DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
+                                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                                 port = self.__port,
                                 payload = _ScpiCmds.GET_MEAS.value))
             self.__wait_4_response = True
         else:
             self.__request_data += 1
         self.read_buffer()
         return self.last_data
@@ -333,30 +354,35 @@
         else:
             current = 0
             voltage = 0
         log.critical(self.properties.model)
         log.critical(self.properties.model.startswith("PSB"))
         if self.properties.model.startswith("PSB"):
             msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = "SINK:"+_ScpiCmds.SEND_CURR.value + str(current))
             self.__tx_chan.send_data(msg)
             self.read_buffer()
 
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = _ScpiCmds.SEND_CURR.value + str(current))
         self.__tx_chan.send_data(msg)
         self.read_buffer()
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = _ScpiCmds.SEND_VOLT.value + str(voltage))
         self.__tx_chan.send_data(msg)
         self.read_buffer()
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = _ScpiCmds.OUTPUT_ON.value)
         self.__tx_chan.send_data(msg)
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = _ScpiCmds.GET_OUTPUT.value)
         self.__tx_chan.send_data(msg)
         self.read_buffer()
 
 
     def set_cv_mode(self, volt_ref: int, current_limit: int|None= None) -> None:
         '''
@@ -387,30 +413,35 @@
         elif voltage > self.properties.max_volt_limit:
             voltage = self.properties.max_volt_limit
         else:
             current = 0
             voltage = 0
         if self.properties.model.startswith("PSB"):
             msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = "SINK:"+_ScpiCmds.SEND_CURR.value + str(current))
             self.__tx_chan.send_data(msg)
             self.read_buffer()
 
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = _ScpiCmds.SEND_CURR.value + str(current))
         self.__tx_chan.send_data(msg)
         self.read_buffer()
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = _ScpiCmds.SEND_VOLT.value + str(voltage))
         self.__tx_chan.send_data(msg)
         self.read_buffer()
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = _ScpiCmds.OUTPUT_ON.value)
         self.__tx_chan.send_data(msg)
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
+                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = _ScpiCmds.GET_OUTPUT.value)
         self.__tx_chan.send_data(msg)
         self.read_buffer()
 
     def set_wait_mode(self) -> None:
         ''' Set the device in standby mode.
         Args:
@@ -421,18 +452,20 @@
             - None 
         '''
         log.debug("Disabling SOURCE...")
         self.__tx_chan.close()
         self.__tx_chan = SysShdIpcChanC(name = DEFAULT_TX_CHAN)
         self.__change_last_mode(DrvBasePwrModeE.WAIT)
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                                 port = self.__port,
                                 payload = _ScpiCmds.OUTPUT_OFF.value)
         self.__tx_chan.send_data(msg)
         self.__tx_chan.send_data(DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
+                                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                                 port = self.__port,
                                 payload = _ScpiCmds.GET_OUTPUT.value))
 
     def disable(self) -> None:
         ''' Set the device in standby mode.
         Args:
             - None
@@ -442,18 +475,20 @@
             - None 
         '''
         log.debug("Disabling SOURCE...")
         self.__tx_chan.close()
         self.__tx_chan = SysShdIpcChanC(name = DEFAULT_TX_CHAN)
         self.__change_last_mode(DrvBasePwrModeE.DISABLE)
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
+                                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                                 port = self.__port,
                                 payload = _ScpiCmds.OUTPUT_OFF.value)
         self.__tx_chan.send_data(msg)
         self.__tx_chan.send_data(DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
+                                rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                                 port = self.__port,
                                 payload = _ScpiCmds.GET_OUTPUT.value))
 
 
     def close(self) -> None:
         ''' Close the serial port.
         Args:
@@ -461,15 +496,16 @@
         Returns:
             - None.
         Raises:
             - None.
         '''
         self.disable()
         self.__tx_chan.send_data(DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
-                                                 port = self.__port,
-                                                 payload = _ScpiCmds.LOCK_OFF.value))
+                                    rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
+                                    port = self.__port,
+                                    payload = _ScpiCmds.LOCK_OFF.value))
         del_msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.DEL_DEV,
-                                  port = self.__port) # pylint: disable=no-member
+                                port = self.__port) # pylint: disable=no-member
         self.__tx_chan.send_data(del_msg)
         self.__tx_chan.close()
         self.read_buffer()
         self.__rx_chan.terminate()
```

### Comparing `rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/PKG-INFO` & `rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-driver-ea
-Version: 0.0.2
+Version: 0.0.3
 Summary: Driver to control EA Power Electronics devices.
 Author-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 Maintainer-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

