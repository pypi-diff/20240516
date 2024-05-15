# Comparing `tmp/new_natnet_client-4.1.3b0.tar.gz` & `tmp/new_natnet_client-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_natnet_client-4.1.3b0.tar", max compression
+gzip compressed data, was "new_natnet_client-4.2.0.tar", max compression
```

## Comparing `new_natnet_client-4.1.3b0.tar` & `new_natnet_client-4.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.1.3b0/LICENSE
--rw-r--r--   0        0        0     1582 2024-05-11 18:54:03.498484 new_natnet_client-4.1.3b0/README.md
--rw-r--r--   0        0        0    15156 2024-05-11 19:16:24.793204 new_natnet_client-4.1.3b0/new_natnet_client/Client.py
--rw-r--r--   0        0        0     8498 2024-05-11 18:54:03.498484 new_natnet_client-4.1.3b0/new_natnet_client/NatNetTypes.py
--rw-r--r--   0        0        0    26518 2024-05-11 20:41:40.316803 new_natnet_client-4.1.3b0/new_natnet_client/Unpackers.py
--rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.1.3b0/new_natnet_client/__init__.py
--rw-r--r--   0        0        0      469 2024-05-11 20:39:29.717215 new_natnet_client-4.1.3b0/pyproject.toml
--rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 new_natnet_client-4.1.3b0/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.2.0/LICENSE
+-rw-r--r--   0        0        0     1489 2024-05-14 21:27:27.319169 new_natnet_client-4.2.0/README.md
+-rw-r--r--   0        0        0    15264 2024-05-14 21:22:17.902675 new_natnet_client-4.2.0/new_natnet_client/Client.py
+-rw-r--r--   0        0        0     8469 2024-05-14 15:13:20.057750 new_natnet_client-4.2.0/new_natnet_client/NatNetTypes.py
+-rw-r--r--   0        0        0    26511 2024-05-14 15:11:20.737017 new_natnet_client-4.2.0/new_natnet_client/Unpackers.py
+-rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.2.0/new_natnet_client/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-14 21:28:14.151008 new_natnet_client-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2026 1970-01-01 00:00:00.000000 new_natnet_client-4.2.0/PKG-INFO
```

### Comparing `new_natnet_client-4.1.3b0/LICENSE` & `new_natnet_client-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.3b0/README.md` & `new_natnet_client-4.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 I have no relationship with Optitrack
 ---
 ![image](https://github.com/IgnaciodelaTorreArias/natnet-client/assets/91571670/ca288adb-9b39-4f49-9012-5f3a3a5b8300)
 
 When firs started the client has default parameters.
 Once the client is created, inmediatly after it will try to connect, if it was succesful the property *conected* will be set.
 
-Once the client is set it will start receiving data, probably the data you want to access is MoCap (Motion Capture) which is data send every frame. This data is stored has a property.
-![image](https://github.com/IgnaciodelaTorreArias/natnet-client/assets/91571670/15bf36e3-7443-46d8-8175-cadd251901d1)
+Once the client is set it will start receiving data, probably the data you want to access is MoCap (Motion Capture) which is data send every frame. This data is stored has a property and used as an iterable.
+
 The data in this properties depends both on the natnet version used by the Motive app and its configuration.
 You can also send requests or commands with the respective methods, the responses and messages from the server (Motive app) will be stored has a queue, with a maximum size of buffer_size which is pased when you first start the client.
```

### Comparing `new_natnet_client-4.1.3b0/new_natnet_client/Client.py` & `new_natnet_client-4.2.0/new_natnet_client/Client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from dataclasses import dataclass, field, FrozenInstanceError, InitVar, asdict
 from collections import deque
 import struct
 from types import NoneType
-from typing import Any, Tuple, Dict, Callable
+from typing import Any, Tuple, Dict, Callable, Iterator
 import socket
 import logging
 from threading import Thread, Lock
 from new_natnet_client.NatNetTypes import NAT_Messages, NAT_Data, MoCap
 from new_natnet_client.Unpackers import DataUnpackerV3_0, DataUnpackerV4_1
 from copy import copy
+import time
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 @dataclass(frozen=True)
 class Server_info:
   application_name: str
   version: Tuple[int,...]
@@ -25,14 +26,15 @@
   local_ip_address: str = "127.0.0.1"
   use_multicast: bool = True
   multicast_address: str ="239.255.42.99"
   command_port: int = 1510
   data_port: int = 1511
   max_buffer_size: InitVar[int] = 255
   __mocap_bytes: bytes | None = field(init=False, default=None)
+  __new_data_flag: bool = field(init=False, default=False)
   __can_change_bitstream: bool = field(init=False, default=False)
   __running: bool = field(init=False, default=False)
   __command_socket: socket.socket | None = field(init=False, repr=False, default=None)
   __data_socket: socket.socket | None = field(init=False, repr=False, default=None)
   __freeze: bool = field(init=False, repr=False, default=False)
 
   # TODO: Add bitstream change support
@@ -43,18 +45,21 @@
 
   @property
   def server_info(self) -> Server_info:
     with self.__server_info_lock:
       return copy(self.__server_info)
 
   @property
-  def MoCap(self) -> MoCap | None:
-    with self.__mocap_bytes_lock:
-      if self.__mocap_bytes is None: return None
-      return self.__unpacker.unpack_mocap_data(self.__mocap_bytes)
+  def MoCap(self) -> Iterator[MoCap]:
+    if  self.__mocap_bytes is None: return
+    while True:
+      print("adquiring lock")
+      with self.__mocap_bytes_lock:
+        if self.__new_data_flag:
+          yield self.__unpacker.unpack_mocap_data(self.__mocap_bytes)
 
   @property
   def server_responses(self) -> deque[int | str]:
     with self.__server_responses_lock:
       return self.__server_responses.copy()
 
   @property
@@ -104,15 +109,14 @@
     self.__command_socket = self.create_socket(ip, proto)
     if type(self.__command_socket) == NoneType:
       logging.info(f"Command socket. Check Motive/Server mode requested mode agreement.  {self.use_multicast = } ")
       return False
     if self.use_multicast:
       # set to broadcast mode
       self.__command_socket.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-    self.__command_socket.settimeout(2.0)
     return True
     
   def __create__data_socket(self) -> bool:
     ip = ''
     proto = socket.IPPROTO_UDP
     port = 0
     if self.use_multicast:
@@ -150,56 +154,53 @@
       NAT_Messages.SERVER_INFO: self.__unpack_server_info,
       NAT_Messages.RESPONSE: self.__unpack_server_response,
       NAT_Messages.MESSAGE_STRING: self.__unpack_server_message,
       NAT_Messages.UNRECOGNIZED_REQUEST: self.__unpack_unrecognized_request,
       NAT_Messages.UNDEFINED: self.__unpack_undefined_nat_message
     }
 
-    self.connect()
     self.__update_unpacker_version()
 
   def __setattr__(self, name:str, value:Any):
     if self.__freeze and name in (
       "server_address",
       "local_ip_address",
       "use_multicast",
       "multicast_address",
       "command_port",
       "data_port",
     ):
       raise FrozenInstanceError("This attribute can't be changed because client is already connected")
     super().__setattr__(name, value)
 
-  def connect(self) -> bool:
-    """
-      Creates the connection sockets and starts threads for receiving messages/responses and data
-      
-      Returns:
-        bool: whether the connection was successful
-    """
-    if self.__running or not self.__create__command_socket() or not self.__create__data_socket(): return False
+  def __enter__(self) -> None:
+    if self.__running or not self.__create__command_socket() or not self.__create__data_socket(): return
     logging.info("Client connected")
-    self.send_request(NAT_Messages.CONNECT,"")
     self.__running = True
-
-    self.__command_thread = Thread(target=self.__command_thread_function)
-    self.__command_thread.start()
     self.__data_thread = Thread(target=self.__data_thread_function)
     self.__data_thread.start()
-    return True
+    self.__command_thread = Thread(target=self.__command_thread_function)
+    self.__command_thread.start()
+    self.send_request(NAT_Messages.CONNECT,"")
+    time.sleep(0.5)
+    return
+
+  def __exit__(self, exc_type, exc_value, traceback) -> None:
+    if self.__running:
+      self.shutdown()
 
   def send_request(self, NAT_command:NAT_Messages, command:str) -> int:
     """
       Send request to server
       
       Returns:
       ---
         int: number of bytes send, (-1) if something went wrong
     """
-    if not self.__running or NAT_command == NAT_Messages.UNDEFINED: return -1
+    if type(self.__command_socket) == NoneType or NAT_command == NAT_Messages.UNDEFINED: return -1
     packet_size: int = 0
     if  NAT_command == NAT_Messages.KEEP_ALIVE or \
         NAT_command == NAT_Messages.REQUEST_MODEL_DEF or \
         NAT_command == NAT_Messages.REQUEST_FRAME_OF_DATA:
       command = ""
     elif NAT_command == NAT_Messages.REQUEST:
       packet_size = len(command) + 1
@@ -213,15 +214,14 @@
                   '\x00')
       packet_size = len(command) + 1
     data = NAT_command.value.to_bytes(2, byteorder="little", signed=True)
     data += packet_size.to_bytes(2, byteorder='little',  signed=True)
     data += command.encode("utf-8")
     data += b'\0'
     with self.__command_socket_lock:
-      if self.__command_socket is None: return -1
       return self.__command_socket.sendto(data, (self.server_address, self.command_port))
 
   def send_command(self, command: str):
     """
       Tries to send the command 3 times
 
       Returns:
@@ -250,14 +250,15 @@
       NAT_Data.DEVICE: self.__unpacker.unpack_device_description,
       NAT_Data.CAMERA: self.__unpacker.unpack_camera_description,
       NAT_Data.ASSET: self.__unpacker.unpack_asset_description
     }
 
   def __unpack_mocap_data(self, data:bytes, packet_size:int):
     with self.__mocap_bytes_lock:
+      self.__new_data_flag = True
       self.__mocap_bytes = data
     return packet_size
 
   def __unpack_data_descriptions(self, data:bytes, packet_size:int):
     offset = 0
     dataset_count = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     for i in range(dataset_count):
@@ -340,14 +341,16 @@
     run = True
     while run:
       with self.__running_lock:
         run = self.__running
       try:
         if self.__data_socket is None: return
         data = self.__data_socket.recv(recv_buffer_size)
+      except socket.timeout:
+        pass
       except socket.error as msg:
         logging.error(f"Data thread {self.local_ip_address}: {msg}")
         data = bytes()
       if len(data):
         self.__process_message(data)
     logging.info("Data thread stopped")
 
@@ -381,10 +384,11 @@
         self.__command_socket.close()
     if self.__data_socket is not None:
       self.__data_socket.close()
     self.__command_socket = None
     self.__data_socket = None
     self.__data_thread.join()
     self.__command_thread.join()
+    self.__freeze = False
 
   def __del__(self):
     self.shutdown()
```

### Comparing `new_natnet_client-4.1.3b0/new_natnet_client/NatNetTypes.py` & `new_natnet_client-4.2.0/new_natnet_client/NatNetTypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,170 +72,170 @@
 class MoCapData:
   ...
 
 @dataclass(frozen=True)
 class Frame_prefix(MoCapData):
   frame_number: int
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Marker_data:
   name: str
   num_markers: int
   positions: Tuple[Position, ...]
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Marker_set_data(MoCapData):
   num_marker_sets: int
   marker_sets: Tuple[Marker_data, ...]
   marker_sets_d: Dict[str, Marker_data] = field(init=False)
 
   def __post_init__(self):
     object.__setattr__(self, "marker_sets_d", { instance.name:instance for instance in self.marker_sets})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Legacy_marker_set_data(MoCapData):
   num_markers: int
   positions: Tuple[Position, ...]
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Rigid_body:
   id: int
   pos: Position
   rot: Quaternion
   err: float
   tracking: bool
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Rigid_body_data(MoCapData):
   num_rigid_bodies: int
   rigid_bodies: Tuple[Rigid_body, ...]
   rigid_bodies_d: Dict[int, Rigid_body] = field(init=False)
   
   def __post_init__(self):
     object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.rigid_bodies})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Skeleton:
   num_rigid_bodies: int
   rigid_bodies: Tuple[Rigid_body, ...]
   rigid_bodies_d: Dict[int, Rigid_body] = field(init=False)
   
   def __post_init__(self):
     object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.rigid_bodies})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Skeleton_data(MoCapData):
   num_skeletons: int
   skeletons: Tuple[Skeleton, ...]
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Asset_RB:
   id: int
   pos: Position
   rot: Quaternion
   err: float
   param: int
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Asset_marker:
   id: int
   pos: Position
   size: float
   param: int
   residual: float
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Asset:
   id: int
   num_rigid_bodies: int
   rigid_bodies: Tuple[Asset_RB, ...]
   num_markers: int
   markers: Tuple[Asset_marker, ...]
   rigid_bodies_d: Dict[int, Asset_RB] = field(init=False)
   markers_d: Dict[int, Asset_marker] = field(init=False)
 
   def __post_init__(self):
     object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.rigid_bodies})
     object.__setattr__(self, "markers_d", { instance.id : instance for instance in self.markers})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Asset_data(MoCapData):
   num_assets: int
   assets: Tuple[Asset, ...]
   assets_d: Dict[int, Asset] = field(init=False)
 
   def __post_init__(self):
     object.__setattr__(self, "assets_d", { instance.id : instance for instance in self.assets})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Labeled_marker:
   id: int
   pos: Position
   size: int
   param: int
   residual: float
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Labeled_marker_data(MoCapData):
   num_markers: int
   markers: Tuple[Labeled_marker, ...]
   markers_d: Dict[int, Labeled_marker] = field(init=False)
 
   def __post_init__(self):
     object.__setattr__(self, "markers_d", { instance.id : instance for instance in self.markers})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Channel:
   num_frames: int
   frames: Tuple[float, ...]
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Force_plate:
   id: int
   num_channels: int
   channels: Tuple[Channel, ...]
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Force_plate_data(MoCapData):
   num_force_plates: int
   force_plates: Tuple[Force_plate, ...]
   force_plates_d: Dict[int, Force_plate] = field(init=False)
 
   def __post_init__(self):
     object.__setattr__(self, "force_plates_d", { instance.id : instance for instance in self.force_plates})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Device:
   id: int
   num_channels: int
   channels: Tuple[Channel, ...]
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Device_data(MoCapData):
   num_devices: int
   devices: Tuple[Device, ...]
   devices_d: Dict[int, Device] = field(init=False)
   
   def __post_init__(self):
     object.__setattr__(self, "devices_d", { instance.id : instance for instance in self.devices})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Frame_suffix:
   time_code: int
   time_code_sub: int
   timestamp: float
   camera_mid_exposure: int
   stamp_data: int
   stamp_transmit: int
   recording: bool
   tracked_models_changed: bool
   precision_timestamp_sec: int | None = None
   precision_timestamp_frac_sec: int | None = None
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class MoCap:
   prefix_data: Frame_prefix
   marker_set_data: Marker_set_data
   legacy_marker_set_data: Legacy_marker_set_data
   rigid_body_data: Rigid_body_data
   skeleton_data: Skeleton_data
   labeled_marker_data: Labeled_marker_data
@@ -243,88 +243,88 @@
   device_data: Device_data
   suffix_data: Frame_suffix
   asset_data: Asset_data | None = None
 
 class Descriptor:
   ...
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Marker_set_description(Descriptor):
   name: str
   num_markers:int
   markers_names: Tuple[str, ...]
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class RB_marker:
   name:str
   id: int
   pos: Position
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Rigid_body_description(Descriptor):
   name: str
   id: int
   parent_id: int
   pos: Position
   num_markers:int
   markers: Tuple[RB_marker, ...]
   markers_d: Dict[int, RB_marker] = field(init=False)
 
   def __post_init__(self):
     object.__setattr__(self, "markers_d", { instance.id : instance for instance in self.markers})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Skeleton_description(Descriptor):
   name: str
   id: int
   num_rigid_bodies: int
   rigid_bodies: Tuple[Rigid_body_description, ...]
   rigid_bodies_d: Dict[int, Rigid_body_description] = field(init=False)
 
   def __post_init__(self):
     object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.rigid_bodies})
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Force_plate_description(Descriptor):
   id:int
   serial_number: str
   dimensions: Tuple[float, float]
   origin: Position
   calibration_matrix: Tuple[float, ...]
   corners: Tuple[float, ...]
   plate_type: int
   channel_data_type: int
   num_channels: int
   channels: Tuple[str, ...]
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Device_description(Descriptor):
   id: int
   name: str
   serial_number: str
   type: int
   channel_type: int
   num_channels: int
   channels: Tuple[str, ...]
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Camera_description(Descriptor):
   name: str
   pos: Position
   orientation: Quaternion
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Marker_description(Descriptor):
   name: str
   id: int
   pos: Position
   size: float
   param: int
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Asset_description(Descriptor):
   name: str
   type: int
   id: int
   num_rigid_bodies: int
   rigid_bodies: Tuple[Rigid_body_description, ...]
   num_markers: int
```

### Comparing `new_natnet_client-4.1.3b0/new_natnet_client/Unpackers.py` & `new_natnet_client-4.2.0/new_natnet_client/Unpackers.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,75 +22,76 @@
   def unpack_marker_set_data(cls, data:bytes) -> Tuple[NatNetTypes.Marker_set_data, int]:
     offset = 0
     template = {}
     template['num_marker_sets'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
     markers = deque()
+    position_unpacker = lambda position_data: NatNetTypes.Position.unpack(bytes(position_data))
     for _ in range(template['num_marker_sets']):
       template_marker = {}
       name, _, _ = data[offset:].partition(b'\0')
       offset += len(name) + 1
       template_marker['name'] = str(name, encoding="utf-8")
       template_marker['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
       template_marker['positions'] = tuple(map(
-        lambda position_data: NatNetTypes.Position.unpack(bytes(position_data)),
-        batched(data[offset:offset:=offset+(12*template_marker['num_markers'])],12)
+        position_unpacker,
+        batched(data[offset:(offset:=offset+(12*template_marker['num_markers']))],12)
       ))
       markers.append(NatNetTypes.Marker_data(**template_marker))
     template['marker_sets'] = tuple(markers)
     return NatNetTypes.Marker_set_data(**template), offset
 
   @classmethod
   def unpack_legacy_other_markers(cls, data:bytes) -> Tuple[NatNetTypes.Legacy_marker_set_data,int]:
     offset = 0
     template = {}
     template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
     positions = deque(map(
       lambda position_data: NatNetTypes.Position.unpack(bytes(position_data)),
-      batched(data[offset:offset:=offset+(12*template['num_markers'])],12)
+      batched(data[offset:(offset:=offset+(12*template['num_markers']))],12)
     ))
     template['positions'] = tuple(positions)
     return NatNetTypes.Legacy_marker_set_data(**template), offset
 
   @classmethod
-  def unpack_rigid_body(cls, data:bytes) -> Tuple[NatNetTypes.Rigid_body, int]:
+  def unpack_rigid_body(cls, data:bytes) -> NatNetTypes.Rigid_body:
     offset = 0
     template = {}
     template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
     template['rot'] = NatNetTypes.Quaternion.unpack(data[offset:(offset:=offset+16)])
     template['err'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
     param:int = unpack( 'h', data[offset:(offset:=offset+2)])[0]
     template['tracking'] = bool(param & 0x01)
-    return NatNetTypes.Rigid_body(**template), offset
+    return NatNetTypes.Rigid_body(**template)
 
   @classmethod
   def unpack_rigid_body_data(cls, data:bytes) -> Tuple[NatNetTypes.Rigid_body_data, int]:
     offset = 0
     template = {}
     template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
     template['rigid_bodies'] = tuple(map(
-        lambda rigid_body_data: cls.unpack_rigid_body(bytes(rigid_body_data))[0],
+        lambda rigid_body_data: cls.unpack_rigid_body(bytes(rigid_body_data)),
         batched(data[offset:(offset:=offset+(cls.rigid_body_lenght*template['num_rigid_bodies']))], cls.rigid_body_lenght) 
     ))
     return NatNetTypes.Rigid_body_data(**template), offset
   
   @classmethod
   def unpack_skeleton(cls, data:bytes) -> Tuple[NatNetTypes.Skeleton, int]:
     offset = 0
     template = {}
     template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['rigid_bodies'] = tuple(map(
-        lambda rigid_body_data: cls.unpack_rigid_body(bytes(rigid_body_data))[0],
+        lambda rigid_body_data: cls.unpack_rigid_body(bytes(rigid_body_data)),
         batched(data[offset:(offset:=offset+(cls.rigid_body_lenght*template['num_rigid_bodies']))], cls.rigid_body_lenght) 
     ))
     return NatNetTypes.Skeleton(**template), offset
 
   @classmethod
   def unpack_skeleton_data(cls, data:bytes) -> Tuple[NatNetTypes.Skeleton_data, int]:
     offset = 0
@@ -126,46 +127,47 @@
   def decode_marker_id(cls, id:int) -> Tuple[int, int]:
     return (
       id >> 16,
       id & 0x0000ffff
     )
 
   @classmethod
-  def unpack_labeled_marker(cls, data:bytes) -> Tuple[NatNetTypes.Labeled_marker, int]:
+  def unpack_labeled_marker(cls, data:bytes) -> NatNetTypes.Labeled_marker:
     offset = 0
     template = {}
     template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
     template['size'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
     template['param'] = unpack( 'h', data[offset:(offset:=offset+2)])[0]
     template['residual'] = unpack('<f', data[offset:(offset:=offset+4)])[0] * 1000.0
-    return NatNetTypes.Labeled_marker(**template), offset
+    return NatNetTypes.Labeled_marker(**template)
 
   @classmethod
   def unpack_labeled_marker_data(cls, data:bytes) -> Tuple[NatNetTypes.Labeled_marker_data, int]:
     offset = 0
     template = {}
     template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
     template['markers'] = tuple(map(
-      lambda marker_data: cls.unpack_labeled_marker(bytes(marker_data))[0],
+      lambda marker_data: cls.unpack_labeled_marker(bytes(marker_data)),
       batched(data[offset:(offset:=offset+(cls.marker_lenght*template['num_markers']))],cls.marker_lenght)
     ))
     return NatNetTypes.Labeled_marker_data(**template), offset
 
   @classmethod
   def unpack_channels(cls, data:bytes, num_channels:int) -> Tuple[Tuple[NatNetTypes.Channel, ...],int]:
     offset = 0
     channels = deque()
+    frame_unpacker = lambda frame_data: unpack('<f', bytes(frame_data))[0]
     for _ in range(num_channels):
       template_channel = {}
       template_channel['num_frames'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
       template_channel['frames'] = tuple(map(
-        lambda frame_data: unpack('<f', frame_data)[0],
+        frame_unpacker,
         batched(data[offset:(offset:=offset+(4*template_channel['num_frames']))],4)
       ))
       channels.append(NatNetTypes.Channel(**template_channel))
     return tuple(channels), offset
 
   @classmethod
   def unpack_force_plate_data(cls, data:bytes) -> Tuple[NatNetTypes.Force_plate_data, int]:
@@ -424,48 +426,48 @@
   @classmethod
   def unpack_data_size(cls, data: bytes) -> Tuple[int, int]:
     offset = 0
     size_in_bytes = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     return size_in_bytes, offset
 
   @classmethod
-  def unpack_asset_rigid_body(cls, data:bytes) -> Tuple[NatNetTypes.Asset_RB, int]:
+  def unpack_asset_rigid_body(cls, data:bytes) -> NatNetTypes.Asset_RB:
     offset = 0
     template = {}
     template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
     template['rot'] = NatNetTypes.Quaternion.unpack(data[offset:(offset:=offset+16)])
     template['err'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
     template['param'] = unpack( 'h', data[offset:(offset:=offset+2)])[0]
-    return NatNetTypes.Asset_RB(**template), offset
+    return NatNetTypes.Asset_RB(**template)
 
   @classmethod
-  def unpack_asset_marker(cls, data:bytes) -> Tuple[NatNetTypes.Asset_marker, int]:
+  def unpack_asset_marker(cls, data:bytes) -> NatNetTypes.Asset_marker:
     offset = 0
     template = {}
     template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
     template['size'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
     template['param'] = unpack( 'h', data[offset:(offset:=offset+2)])[0]
     template['residual'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
-    return NatNetTypes.Asset_marker(**template),  offset
+    return NatNetTypes.Asset_marker(**template)
 
   @classmethod
   def unpack_asset(cls, data:bytes) -> Tuple[NatNetTypes.Asset, int]:
     offset = 0
     template = {}
     template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['rigid_bodies'] = tuple(map(
-      lambda rigid_body_data: cls.unpack_asset_rigid_body(bytes(rigid_body_data))[0],
+      lambda rigid_body_data: cls.unpack_asset_rigid_body(bytes(rigid_body_data)),
       batched(data[offset:(offset:=offset+(cls.asset_rigid_body_lenght*template['num_rigid_bodies']))], cls.asset_rigid_body_lenght)
     ))
     template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['markers'] = tuple(map(
-      lambda marker_data: cls.unpack_asset_marker(bytes(marker_data))[0],
+      lambda marker_data: cls.unpack_asset_marker(bytes(marker_data)),
       batched(data[offset:(offset:=offset+(cls.asset_marker_lenght*template['num_markers']))], cls.asset_marker_lenght)
     ))
     return NatNetTypes.Asset(**template), offset
 
   @classmethod
   def unpack_asset_data(cls, data:bytes) -> Tuple[NatNetTypes.Asset_data, int]:
     offset = 0
```

