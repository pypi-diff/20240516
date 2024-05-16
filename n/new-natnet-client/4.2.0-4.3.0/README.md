# Comparing `tmp/new_natnet_client-4.2.0.tar.gz` & `tmp/new_natnet_client-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_natnet_client-4.2.0.tar", max compression
+gzip compressed data, was "new_natnet_client-4.3.0.tar", max compression
```

## Comparing `new_natnet_client-4.2.0.tar` & `new_natnet_client-4.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.2.0/LICENSE
--rw-r--r--   0        0        0     1489 2024-05-14 21:27:27.319169 new_natnet_client-4.2.0/README.md
--rw-r--r--   0        0        0    15264 2024-05-14 21:22:17.902675 new_natnet_client-4.2.0/new_natnet_client/Client.py
--rw-r--r--   0        0        0     8469 2024-05-14 15:13:20.057750 new_natnet_client-4.2.0/new_natnet_client/NatNetTypes.py
--rw-r--r--   0        0        0    26511 2024-05-14 15:11:20.737017 new_natnet_client-4.2.0/new_natnet_client/Unpackers.py
--rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.2.0/new_natnet_client/__init__.py
--rw-r--r--   0        0        0      464 2024-05-14 21:28:14.151008 new_natnet_client-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     2026 1970-01-01 00:00:00.000000 new_natnet_client-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.3.0/LICENSE
+-rw-r--r--   0        0        0     1489 2024-05-14 21:27:27.319169 new_natnet_client-4.3.0/README.md
+-rw-r--r--   0        0        0    17112 2024-05-15 23:29:45.366880 new_natnet_client-4.3.0/new_natnet_client/Client.py
+-rw-r--r--   0        0        0     9666 2024-05-15 23:03:11.095745 new_natnet_client-4.3.0/new_natnet_client/NatNetTypes.py
+-rw-r--r--   0        0        0    25548 2024-05-15 21:51:59.794498 new_natnet_client-4.3.0/new_natnet_client/Unpackers.py
+-rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.3.0/new_natnet_client/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-15 23:28:31.032548 new_natnet_client-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2026 1970-01-01 00:00:00.000000 new_natnet_client-4.3.0/PKG-INFO
```

### Comparing `new_natnet_client-4.2.0/LICENSE` & `new_natnet_client-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.2.0/README.md` & `new_natnet_client-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.2.0/new_natnet_client/Client.py` & `new_natnet_client-4.3.0/new_natnet_client/Client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from dataclasses import dataclass, field, FrozenInstanceError, InitVar, asdict
 from collections import deque
 import struct
-from types import NoneType
-from typing import Any, Tuple, Dict, Callable, Iterator
+from types import NoneType, TracebackType
+from typing import Any, Optional, Tuple, Dict, Callable, Iterator, Type
 import socket
 import logging
 from threading import Thread, Lock
-from new_natnet_client.NatNetTypes import NAT_Messages, NAT_Data, MoCap
+from new_natnet_client.NatNetTypes import NAT_Messages, NAT_Data, MoCap, Descriptor, Descriptors
 from new_natnet_client.Unpackers import DataUnpackerV3_0, DataUnpackerV4_1
-from copy import copy
+from copy import copy, deepcopy
 import time
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
-@dataclass(frozen=True)
+@dataclass(slots=True)
 class Server_info:
   application_name: str
-  version: Tuple[int,...]
+  version: Tuple[int, ...]
   nat_net_major: int
   nat_net_minor: int
 
 @dataclass(kw_only=True)
 class NatNetClient:
   server_address: str = "127.0.0.1"
   local_ip_address: str = "127.0.0.1"
   use_multicast: bool = True
   multicast_address: str ="239.255.42.99"
   command_port: int = 1510
   data_port: int = 1511
   max_buffer_size: InitVar[int] = 255
   __mocap_bytes: bytes | None = field(init=False, default=None)
   __new_data_flag: bool = field(init=False, default=False)
+  __descriptors: Descriptors = field(init=False, default_factory=Descriptors)
   __can_change_bitstream: bool = field(init=False, default=False)
   __running: bool = field(init=False, default=False)
   __command_socket: socket.socket | None = field(init=False, repr=False, default=None)
   __data_socket: socket.socket | None = field(init=False, repr=False, default=None)
   __freeze: bool = field(init=False, repr=False, default=False)
 
   # TODO: Add bitstream change support
@@ -46,17 +47,16 @@
   @property
   def server_info(self) -> Server_info:
     with self.__server_info_lock:
       return copy(self.__server_info)
 
   @property
   def MoCap(self) -> Iterator[MoCap]:
-    if  self.__mocap_bytes is None: return
+    if  self.__mocap_bytes is None: raise StopIteration
     while True:
-      print("adquiring lock")
       with self.__mocap_bytes_lock:
         if self.__new_data_flag:
           yield self.__unpacker.unpack_mocap_data(self.__mocap_bytes)
 
   @property
   def server_responses(self) -> deque[int | str]:
     with self.__server_responses_lock:
@@ -64,42 +64,50 @@
 
   @property
   def server_messages(self) -> deque[str]:
     with self.__server_messages_lock:
       return self.__server_messages.copy()
 
   @property
-  def buffer_size(self):
+  def buffer_size(self) -> int:
     """
       Buffer size for messages/responses queues
     """
     return self.__max_buffer_size
 
   @buffer_size.setter
-  def buffer_size(self, maxlen:int):
-    self.__max_buffer_size = maxlen
+  def buffer_size(self, max_len: int) -> None:
+    self.__max_buffer_size = max_len
     with self.__server_messages_lock:
-      self.__server_messages = deque(self.__server_messages,maxlen=maxlen)
+      self.__server_messages = deque(self.__server_messages,maxlen=max_len)
     with self.__server_responses_lock:
-      self.__server_responses = deque(self.__server_responses,maxlen=maxlen)
+      self.__server_responses = deque(self.__server_responses,maxlen=max_len)
+
+  @property
+  def frozen_descriptors(self) -> Descriptors:
+    return deepcopy(self.__descriptors)
+  
+  @property
+  def descriptors(self) -> Descriptors:
+    return self.__descriptors
 
   @staticmethod
   def create_socket(ip: str, proto: int, port: int = 0) -> socket.socket | None:
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, proto)
     sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
     try:
       # Connect to the IP with a dynamically assigned port
       sock.bind((ip, port))
       sock.settimeout(3)
       return sock
     except socket.error as msg:
       logging.error(msg)
       sock.close()
 
-  def __get_message_id(self, data:bytes) -> int:
+  def __get_message_id(self, data: bytes) -> int:
     message_id = int.from_bytes( data[0:2], byteorder='little',  signed=True )
     return message_id
 
   def __create__command_socket(self) -> bool:
     ip = self.local_ip_address
     proto = socket.IPPROTO_UDP
     if self.use_multicast:
@@ -127,15 +135,15 @@
     if type(self.__data_socket) == NoneType:
       logging.info(f"Data socket. Check Motive/Server mode requested mode agreement.  {self.use_multicast = } ")
       return False
     if self.use_multicast or self.multicast_address != "255.255.255.255":
       self.__data_socket.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, socket.inet_aton(self.multicast_address) + socket.inet_aton(self.local_ip_address))
     return True
 
-  def __post_init__(self, max_buffer_size):
+  def __post_init__(self, max_buffer_size: int) -> None:
     self.__running_lock = Lock()
     self.__command_socket_lock = Lock()
     self.__server_info_lock = Lock()
     self.__server_responses_lock = Lock()
     self.__server_messages_lock = Lock()
     self.__mocap_bytes_lock = Lock()
 
@@ -156,15 +164,15 @@
       NAT_Messages.MESSAGE_STRING: self.__unpack_server_message,
       NAT_Messages.UNRECOGNIZED_REQUEST: self.__unpack_unrecognized_request,
       NAT_Messages.UNDEFINED: self.__unpack_undefined_nat_message
     }
 
     self.__update_unpacker_version()
 
-  def __setattr__(self, name:str, value:Any):
+  def __setattr__(self, name: str, value: Any) -> None:
     if self.__freeze and name in (
       "server_address",
       "local_ip_address",
       "use_multicast",
       "multicast_address",
       "command_port",
       "data_port",
@@ -176,23 +184,22 @@
     if self.__running or not self.__create__command_socket() or not self.__create__data_socket(): return
     logging.info("Client connected")
     self.__running = True
     self.__data_thread = Thread(target=self.__data_thread_function)
     self.__data_thread.start()
     self.__command_thread = Thread(target=self.__command_thread_function)
     self.__command_thread.start()
+    time.sleep(1) # wait to get threads running for receiving data
     self.send_request(NAT_Messages.CONNECT,"")
-    time.sleep(0.5)
-    return
 
-  def __exit__(self, exc_type, exc_value, traceback) -> None:
+  def __exit__(self, exc_type: Optional[Type[BaseException]], exc_value: Optional[BaseException], traceback: Optional[TracebackType]) -> None:
     if self.__running:
       self.shutdown()
 
-  def send_request(self, NAT_command:NAT_Messages, command:str) -> int:
+  def send_request(self, NAT_command: NAT_Messages, command: str) -> int:
     """
       Send request to server
       
       Returns:
       ---
         int: number of bytes send, (-1) if something went wrong
     """
@@ -216,83 +223,103 @@
     data = NAT_command.value.to_bytes(2, byteorder="little", signed=True)
     data += packet_size.to_bytes(2, byteorder='little',  signed=True)
     data += command.encode("utf-8")
     data += b'\0'
     with self.__command_socket_lock:
       return self.__command_socket.sendto(data, (self.server_address, self.command_port))
 
-  def send_command(self, command: str):
+  def send_command(self, command: str) -> bool:
     """
       Tries to send the command 3 times
 
       Returns:
         bool: whether the was send successfully
     """
     res:int = -1
     for _ in range(3):
       res = self.send_request(NAT_Messages.REQUEST, command)
       if res != -1:
         break
     return res != -1
 
-  def __update_unpacker_version(self):
+  def __update_unpacker_version(self) -> None:
     """
       Changes unpacker version based on server's bit stream version
     """
     self.__unpacker = DataUnpackerV3_0
     with self.__server_info_lock:
       if (self.__server_info.nat_net_major == 4 and self.__server_info.nat_net_minor >= 1) or self.__server_info.nat_net_major == 0:
         self.__unpacker = DataUnpackerV4_1
-    self.__mapped_data_descriptors: Dict[NAT_Data, Callable[[bytes], Tuple[Dict, int]]] = {
+    self.__mapped_data_descriptors: Dict[NAT_Data, Callable[[bytes], Tuple[Descriptor, int]]] = {
       NAT_Data.MARKER_SET: self.__unpacker.unpack_marker_set_description,
       NAT_Data.RIGID_BODY: self.__unpacker.unpack_rigid_body_description,
       NAT_Data.SKELETON: self.__unpacker.unpack_skeleton_description,
       NAT_Data.FORCE_PLATE: self.__unpacker.unpack_force_plate_description,
       NAT_Data.DEVICE: self.__unpacker.unpack_device_description,
       NAT_Data.CAMERA: self.__unpacker.unpack_camera_description,
       NAT_Data.ASSET: self.__unpacker.unpack_asset_description
     }
 
-  def __unpack_mocap_data(self, data:bytes, packet_size:int):
+  def __unpack_mocap_data(self, data: bytes, packet_size: int) -> int:
     with self.__mocap_bytes_lock:
       self.__new_data_flag = True
       self.__mocap_bytes = data
     return packet_size
 
-  def __unpack_data_descriptions(self, data:bytes, packet_size:int):
+  def __unpack_data_descriptions(self, data: bytes, packet_size: int) -> int:
     offset = 0
     dataset_count = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    for i in range(dataset_count):
-      t = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    size_in_bytes = -1
+    for _ in range(dataset_count):
+      tag = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+      data_description_type = NAT_Data(tag)
       if self.__unpacker == DataUnpackerV4_1:
         size_in_bytes = int.from_bytes( data[offset:(offset:=offset+4)], byteorder='little',  signed=True )
-      data_description_type = NAT_Data(t)
-      if data_description_type == NAT_Data.UNDEFINED:
-        logging.error(f"{data_description_type = } - ID: {t}")
-        continue
-      d, tmp_offset = self.__mapped_data_descriptors[data_description_type](data[offset:])
-      # TODO: Updater de datos
+      match data_description_type:
+        case NAT_Data.MARKER_SET:
+          description, tmp_offset = self.__unpacker.unpack_marker_set_description(data[offset:])
+          self.__descriptors.marker_set_description.update(description)
+        case NAT_Data.RIGID_BODY:
+          description, tmp_offset = self.__unpacker.unpack_rigid_body_description(data[offset:])
+          self.__descriptors.rigid_body_description.update(description)
+        case NAT_Data.SKELETON:
+          description, tmp_offset = self.__unpacker.unpack_skeleton_description(data[offset:])
+          self.__descriptors.skeleton_description.update(description)
+        case NAT_Data.FORCE_PLATE:
+          description, tmp_offset = self.__unpacker.unpack_force_plate_description(data[offset:])
+          self.__descriptors.force_plate_description.update(description)
+        case NAT_Data.DEVICE:
+          description, tmp_offset = self.__unpacker.unpack_device_description(data[offset:])
+          self.__descriptors.device_description.update(description)
+        case NAT_Data.CAMERA:
+          description, tmp_offset = self.__unpacker.unpack_camera_description(data[offset:])
+          self.__descriptors.camera_description.update(description)
+        case NAT_Data.ASSET:
+          description, tmp_offset = self.__unpacker.unpack_asset_description(data[offset:])
+          self.__descriptors.asset_description.update(description)
+        case NAT_Data.UNDEFINED:
+          logging.error(f"ID: {tag} - Size: {size_in_bytes}")
+          continue
       offset += tmp_offset
     return offset
 
-  def __unpack_server_info(self, data: bytes, __:int) -> int:
+  def __unpack_server_info(self, data: bytes, __: int) -> int:
     offset = 0
-    template = {}
     application_name, _, _ = data[offset:(offset:=offset+256)].partition(b'\0')
-    template['application_name'] = str(application_name, "utf-8")
-    template['version'] = struct.unpack( 'BBBB', data[offset:(offset:=offset+4)] )
-    template['nat_net_major'], template['nat_net_minor'], _, _ = struct.unpack( 'BBBB', data[offset:(offset:=offset+4)] )
+    application_name = str(application_name, "utf-8")
+    version = struct.unpack( 'BBBB', data[offset:(offset:=offset+4)] )
+    nat_net_major, nat_net_minor, _, _ = struct.unpack( 'BBBB', data[offset:(offset:=offset+4)] )
     with self.__server_info_lock:
-      self.__server_info = Server_info(**template)
+      self.__server_info = Server_info(application_name, version, nat_net_major, nat_net_minor)
     self.__update_unpacker_version
-    if template['nat_net_major'] >= 4 and self.use_multicast == False:
+    if nat_net_major >= 4 and self.use_multicast == False:
       self.__can_change_bitstream = True
     return offset
 
-  def __unpack_server_response(self, data:bytes, packet_size:int) -> int:
+  def __unpack_server_response(self, data: bytes, packet_size: int) -> int:
     if packet_size == 4:
       with self.__server_responses_lock:
         self.__server_responses.append(int.from_bytes(data, byteorder='little',  signed=True ))
       return 4
     response, _, _ = data[:256].partition(b'\0')
     if len(response) < 30:
       response = response.decode('utf-8')
@@ -308,29 +335,29 @@
             with self.__server_info_lock:
               self.__server_info = Server_info(**template)
             self.__update_unpacker_version()
       with self.__server_responses_lock:
         self.__server_responses.append(response)
     return len(response)
 
-  def __unpack_server_message(self, data:bytes, __:int):
+  def __unpack_server_message(self, data: bytes, __: int) -> int:
     message, _, _ = data.partition(b'\0')
     with self.__server_messages_lock:
       self.__server_messages.append(str(message, encoding='utf-8'))
     return len(message) + 1
 
-  def __unpack_unrecognized_request(self, _:bytes, packet_size:int) -> int:
+  def __unpack_unrecognized_request(self, _: bytes, packet_size: int) -> int:
     logging.error(f"{NAT_Messages.UNRECOGNIZED_REQUEST} - {packet_size = }")
     return packet_size
 
-  def __unpack_undefined_nat_message(self, _:bytes, packet_size:int) -> int:
+  def __unpack_undefined_nat_message(self, _: bytes, packet_size: int) -> int:
     logging.error(f"{NAT_Messages.UNDEFINED} - {packet_size = }")
     return packet_size
 
-  def __process_message(self, data: bytes):
+  def __process_message(self, data: bytes) -> None:
     offset = 0
     message_id = NAT_Messages(self.__get_message_id(data[offset:(offset:=offset+2)]))
     packet_size = int.from_bytes( data[offset:(offset:=offset+2)], byteorder='little', signed=True)
     if message_id not in self.__mapped:
       return
     self.__mapped[message_id](data[offset:], packet_size)
 
@@ -371,24 +398,24 @@
       except socket.error as msg:
         logging.error(f"Command thread {self.local_ip_address}: {msg}")
         data = bytes()
       if len(data):
         self.__process_message(data)
     logging.info("Command thread stopped")
 
-  def shutdown(self):
+  def shutdown(self) -> None:
     logging.info(f"Shuting down client {self.server_address}")
     with self.__running_lock:
       self.__running = False
     with self.__command_socket_lock:
       if self.__command_socket is not None:
         self.__command_socket.close()
     if self.__data_socket is not None:
       self.__data_socket.close()
     self.__command_socket = None
     self.__data_socket = None
     self.__data_thread.join()
     self.__command_thread.join()
     self.__freeze = False
 
-  def __del__(self):
+  def __del__(self) -> None:
     self.shutdown()
```

### Comparing `new_natnet_client-4.2.0/new_natnet_client/NatNetTypes.py` & `new_natnet_client-4.3.0/new_natnet_client/NatNetTypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import dataclass, field
 import struct
 from math import atan2, asin
-from typing import Dict, Tuple
+from typing import Any, Dict, Tuple
 from enum import Enum
 
 class NAT_Data(Enum):
   MARKER_SET     = 0
   RIGID_BODY    = 1
   SKELETON      = 2
   FORCE_PLATE   = 3
   DEVICE        = 4
   CAMERA        = 5
   ASSET         = 6
   UNDEFINED     = -1
 
   @classmethod
-  def _missing_(cls, _: object):
+  def _missing(cls, _: object):
     return cls.UNDEFINED
 
 class NAT_Messages(Enum):
   # Client/server message ids
   CONNECT               = 0
   SERVER_INFO           = 1
   REQUEST               = 2
@@ -31,20 +31,20 @@
   MESSAGE_STRING        = 8
   DISCONNECT            = 9
   KEEP_ALIVE            = 10
   UNRECOGNIZED_REQUEST  = 100
   UNDEFINED             = 999999
 
   @classmethod
-  def _missing_(cls, _: object):
+  def _missing(cls, _: object):
     return cls.UNDEFINED
 
 class Data:
   @classmethod
-  def unpack(cls, data:bytes):
+  def unpack(cls, data: bytes) -> Any:
     raise NotImplementedError("Subclasses must implement the unpack method")
 
 @dataclass(frozen=True)
 class Position(Data):
   x: float
   y: float
   z: float
@@ -94,133 +94,134 @@
 @dataclass(slots=True)
 class Legacy_marker_set_data(MoCapData):
   num_markers: int
   positions: Tuple[Position, ...]
 
 @dataclass(slots=True)
 class Rigid_body:
-  id: int
+  identifier: int
   pos: Position
   rot: Quaternion
   err: float
   tracking: bool
 
 @dataclass(slots=True)
 class Rigid_body_data(MoCapData):
   num_rigid_bodies: int
   rigid_bodies: Tuple[Rigid_body, ...]
   rigid_bodies_d: Dict[int, Rigid_body] = field(init=False)
   
   def __post_init__(self):
-    object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.rigid_bodies})
+    object.__setattr__(self, "rigid_bodies_d", { instance.identifier : instance for instance in self.rigid_bodies})
 
 @dataclass(slots=True)
 class Skeleton:
+  identifier: int
   num_rigid_bodies: int
   rigid_bodies: Tuple[Rigid_body, ...]
   rigid_bodies_d: Dict[int, Rigid_body] = field(init=False)
   
   def __post_init__(self):
-    object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.rigid_bodies})
+    object.__setattr__(self, "rigid_bodies_d", { instance.identifier : instance for instance in self.rigid_bodies})
 
 @dataclass(slots=True)
 class Skeleton_data(MoCapData):
   num_skeletons: int
   skeletons: Tuple[Skeleton, ...]
 
 @dataclass(slots=True)
 class Asset_RB:
-  id: int
+  identifier: int
   pos: Position
   rot: Quaternion
   err: float
   param: int
 
 @dataclass(slots=True)
 class Asset_marker:
-  id: int
+  identifier: int
   pos: Position
   size: float
   param: int
   residual: float
 
 @dataclass(slots=True)
 class Asset:
-  id: int
+  identifier: int
   num_rigid_bodies: int
   rigid_bodies: Tuple[Asset_RB, ...]
   num_markers: int
   markers: Tuple[Asset_marker, ...]
   rigid_bodies_d: Dict[int, Asset_RB] = field(init=False)
   markers_d: Dict[int, Asset_marker] = field(init=False)
 
   def __post_init__(self):
-    object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.rigid_bodies})
-    object.__setattr__(self, "markers_d", { instance.id : instance for instance in self.markers})
+    object.__setattr__(self, "rigid_bodies_d", { instance.identifier : instance for instance in self.rigid_bodies})
+    object.__setattr__(self, "markers_d", { instance.identifier : instance for instance in self.markers})
 
 @dataclass(slots=True)
 class Asset_data(MoCapData):
   num_assets: int
   assets: Tuple[Asset, ...]
   assets_d: Dict[int, Asset] = field(init=False)
 
   def __post_init__(self):
-    object.__setattr__(self, "assets_d", { instance.id : instance for instance in self.assets})
+    object.__setattr__(self, "assets_d", { instance.identifier : instance for instance in self.assets})
 
 @dataclass(slots=True)
 class Labeled_marker:
-  id: int
+  identifier: int
   pos: Position
   size: int
   param: int
   residual: float
 
 @dataclass(slots=True)
 class Labeled_marker_data(MoCapData):
   num_markers: int
   markers: Tuple[Labeled_marker, ...]
   markers_d: Dict[int, Labeled_marker] = field(init=False)
 
   def __post_init__(self):
-    object.__setattr__(self, "markers_d", { instance.id : instance for instance in self.markers})
+    object.__setattr__(self, "markers_d", { instance.identifier : instance for instance in self.markers})
 
 @dataclass(slots=True)
 class Channel:
   num_frames: int
   frames: Tuple[float, ...]
 
 @dataclass(slots=True)
 class Force_plate:
-  id: int
+  identifier: int
   num_channels: int
   channels: Tuple[Channel, ...]
 
 @dataclass(slots=True)
 class Force_plate_data(MoCapData):
   num_force_plates: int
   force_plates: Tuple[Force_plate, ...]
   force_plates_d: Dict[int, Force_plate] = field(init=False)
 
   def __post_init__(self):
-    object.__setattr__(self, "force_plates_d", { instance.id : instance for instance in self.force_plates})
+    object.__setattr__(self, "force_plates_d", { instance.identifier : instance for instance in self.force_plates})
 
 @dataclass(slots=True)
 class Device:
-  id: int
+  identifier: int
   num_channels: int
   channels: Tuple[Channel, ...]
 
 @dataclass(slots=True)
 class Device_data(MoCapData):
   num_devices: int
   devices: Tuple[Device, ...]
   devices_d: Dict[int, Device] = field(init=False)
   
   def __post_init__(self):
-    object.__setattr__(self, "devices_d", { instance.id : instance for instance in self.devices})
+    object.__setattr__(self, "devices_d", { instance.identifier : instance for instance in self.devices})
 
 @dataclass(slots=True)
 class Frame_suffix:
   time_code: int
   time_code_sub: int
   timestamp: float
   camera_mid_exposure: int
@@ -240,96 +241,116 @@
   skeleton_data: Skeleton_data
   labeled_marker_data: Labeled_marker_data
   force_plate_data: Force_plate_data
   device_data: Device_data
   suffix_data: Frame_suffix
   asset_data: Asset_data | None = None
 
-class Descriptor:
-  ...
-
 @dataclass(slots=True)
-class Marker_set_description(Descriptor):
+class Marker_set_description:
   name: str
   num_markers:int
   markers_names: Tuple[str, ...]
 
 @dataclass(slots=True)
 class RB_marker:
   name:str
-  id: int
+  identifier: int
   pos: Position
 
 @dataclass(slots=True)
-class Rigid_body_description(Descriptor):
+class Rigid_body_description:
   name: str
-  id: int
+  identifier: int
   parent_id: int
   pos: Position
   num_markers:int
   markers: Tuple[RB_marker, ...]
   markers_d: Dict[int, RB_marker] = field(init=False)
 
   def __post_init__(self):
-    object.__setattr__(self, "markers_d", { instance.id : instance for instance in self.markers})
+    object.__setattr__(self, "markers_d", { instance.identifier : instance for instance in self.markers})
 
 @dataclass(slots=True)
-class Skeleton_description(Descriptor):
+class Skeleton_description:
   name: str
-  id: int
+  identifier: int
   num_rigid_bodies: int
   rigid_bodies: Tuple[Rigid_body_description, ...]
   rigid_bodies_d: Dict[int, Rigid_body_description] = field(init=False)
 
   def __post_init__(self):
-    object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.rigid_bodies})
+    object.__setattr__(self, "rigid_bodies_d", { instance.identifier : instance for instance in self.rigid_bodies})
 
 @dataclass(slots=True)
-class Force_plate_description(Descriptor):
-  id:int
+class Force_plate_description:
+  identifier:int
   serial_number: str
   dimensions: Tuple[float, float]
   origin: Position
   calibration_matrix: Tuple[float, ...]
   corners: Tuple[float, ...]
   plate_type: int
   channel_data_type: int
   num_channels: int
   channels: Tuple[str, ...]
 
 @dataclass(slots=True)
-class Device_description(Descriptor):
-  id: int
+class Device_description:
+  identifier: int
   name: str
   serial_number: str
   type: int
   channel_type: int
   num_channels: int
   channels: Tuple[str, ...]
 
 @dataclass(slots=True)
-class Camera_description(Descriptor):
+class Camera_description:
   name: str
   pos: Position
   orientation: Quaternion
 
 @dataclass(slots=True)
-class Marker_description(Descriptor):
+class Marker_description:
   name: str
-  id: int
+  identifier: int
   pos: Position
   size: float
   param: int
 
 @dataclass(slots=True)
-class Asset_description(Descriptor):
+class Asset_description:
   name: str
   type: int
-  id: int
+  identifier: int
   num_rigid_bodies: int
   rigid_bodies: Tuple[Rigid_body_description, ...]
   num_markers: int
-  markers: Tuple
+  markers: Tuple[Marker_description, ...]
   rigid_bodies_d: Dict[int, Rigid_body_description] = field(init=False)
 
   def __post_init__(self):
-    object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.rigid_bodies})
+    object.__setattr__(self, "rigid_bodies_d", { instance.identifier : instance for instance in self.rigid_bodies})
+
+
+type Descriptor = \
+  Dict[str, Marker_set_description] | \
+  Dict[int, Rigid_body_description] | \
+  Dict[int, Skeleton_description] | \
+  Dict[str, Force_plate_description]  | \
+  Dict[str, Device_description] | \
+  Dict[str, Camera_description] | \
+  Dict[int, Asset_description]
+
+@dataclass(slots=True)
+class Descriptors:
+  """
+    Object for storing descriptions
+  """  
+  marker_set_description: Dict[str, Marker_set_description] = field(init=False, default_factory=dict)
+  rigid_body_description: Dict[int, Rigid_body_description] = field(init=False, default_factory=dict)
+  skeleton_description: Dict[int, Skeleton_description] = field(init=False, default_factory=dict)
+  force_plate_description: Dict[str, Force_plate_description] = field(init=False, default_factory=dict)
+  device_description: Dict[str, Device_description] = field(init=False, default_factory=dict)
+  camera_description: Dict[str, Camera_description] = field(init=False, default_factory=dict)
+  asset_description: Dict[int, Asset_description] = field(init=False, default_factory=dict)
```

### Comparing `new_natnet_client-4.2.0/new_natnet_client/Unpackers.py` & `new_natnet_client-4.3.0/new_natnet_client/Unpackers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,553 +1,520 @@
 import new_natnet_client.NatNetTypes as NatNetTypes
-from dataclasses import asdict
-from typing import Tuple, Dict
+from typing import Callable, Iterable, Tuple, Dict
 from collections import deque
 from struct import unpack
 from itertools import batched
 
 class DataUnpackerV3_0:
-  rigid_body_lenght:int = 38
-  marker_lenght:int = 26
+  rigid_body_lenght: int = 38
+  marker_lenght: int = 26
+  frame_suffix_lenght: int = 42
   @classmethod
-  def unpack_data_size(cls, data:bytes) -> Tuple[int, int]:
-    return 0,0
+  def unpack_data_size(cls, data: bytes) -> Tuple[int, int]:
+    return 0, 0
 
   @classmethod
-  def unpack_frame_prefix_data(cls, data:bytes) -> Tuple[NatNetTypes.Frame_prefix, int]:
+  def unpack_frame_prefix_data(cls, data: bytes) -> Tuple[NatNetTypes.Frame_prefix, int]:
     offset = 0
-    prefix = NatNetTypes.Frame_prefix(int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True))
+    prefix = NatNetTypes.Frame_prefix(int.from_bytes(data[offset : (offset:=offset+4)], byteorder='little', signed=True))
     return prefix, offset
 
   @classmethod
-  def unpack_marker_set_data(cls, data:bytes) -> Tuple[NatNetTypes.Marker_set_data, int]:
+  def unpack_marker_set_data(cls, data: bytes) -> Tuple[NatNetTypes.Marker_set_data, int]:
     offset = 0
-    template = {}
-    template['num_marker_sets'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_marker_sets = int.from_bytes(data[offset : (offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    markers = deque()
-    position_unpacker = lambda position_data: NatNetTypes.Position.unpack(bytes(position_data))
-    for _ in range(template['num_marker_sets']):
-      template_marker = {}
+    markers: Iterable[NatNetTypes.Marker_data] = deque()
+    position_unpacker: Callable[[Iterable[int]], NatNetTypes.Position] = lambda position_data: NatNetTypes.Position.unpack(bytes(position_data))
+    for _ in range(num_marker_sets):
       name, _, _ = data[offset:].partition(b'\0')
       offset += len(name) + 1
-      template_marker['name'] = str(name, encoding="utf-8")
-      template_marker['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      template_marker['positions'] = tuple(map(
+      name = str(name, encoding="utf-8")
+      num_markers = int.from_bytes(data[offset : (offset:=offset+4)], byteorder='little', signed=True)
+      positions = tuple(map(
         position_unpacker,
-        batched(data[offset:(offset:=offset+(12*template_marker['num_markers']))],12)
+        batched(data[offset : (offset:=offset+(12*num_markers))], 12)
       ))
-      markers.append(NatNetTypes.Marker_data(**template_marker))
-    template['marker_sets'] = tuple(markers)
-    return NatNetTypes.Marker_set_data(**template), offset
+      markers.append(NatNetTypes.Marker_data(name, num_markers, positions))
+    marker_sets = tuple(markers)
+    return NatNetTypes.Marker_set_data(num_marker_sets, marker_sets), offset
 
   @classmethod
-  def unpack_legacy_other_markers(cls, data:bytes) -> Tuple[NatNetTypes.Legacy_marker_set_data,int]:
+  def unpack_legacy_other_markers(cls, data: bytes) -> Tuple[NatNetTypes.Legacy_marker_set_data,int]:
     offset = 0
-    template = {}
-    template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_markers = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
     positions = deque(map(
       lambda position_data: NatNetTypes.Position.unpack(bytes(position_data)),
-      batched(data[offset:(offset:=offset+(12*template['num_markers']))],12)
+      batched(data[offset:(offset:=offset+(12*num_markers))], 12)
     ))
-    template['positions'] = tuple(positions)
-    return NatNetTypes.Legacy_marker_set_data(**template), offset
+    positions = tuple(positions)
+    return NatNetTypes.Legacy_marker_set_data(num_markers, positions), offset
 
   @classmethod
-  def unpack_rigid_body(cls, data:bytes) -> NatNetTypes.Rigid_body:
+  def unpack_rigid_body(cls, data: bytes) -> NatNetTypes.Rigid_body:
     offset = 0
-    template = {}
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
-    template['rot'] = NatNetTypes.Quaternion.unpack(data[offset:(offset:=offset+16)])
-    template['err'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
-    param:int = unpack( 'h', data[offset:(offset:=offset+2)])[0]
-    template['tracking'] = bool(param & 0x01)
-    return NatNetTypes.Rigid_body(**template)
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    pos = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
+    rot = NatNetTypes.Quaternion.unpack(data[offset:(offset:=offset+16)])
+    err = unpack('<f', data[offset:(offset:=offset+4)])[0]
+    param: int = unpack( 'h', data[offset:(offset:=offset+2)])[0]
+    tracking = bool(param & 0x01)
+    return NatNetTypes.Rigid_body(identifier, pos, rot, err, tracking)
 
   @classmethod
-  def unpack_rigid_body_data(cls, data:bytes) -> Tuple[NatNetTypes.Rigid_body_data, int]:
+  def unpack_rigid_body_data(cls, data: bytes) -> Tuple[NatNetTypes.Rigid_body_data, int]:
     offset = 0
-    template = {}
-    template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_rigid_bodies = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    template['rigid_bodies'] = tuple(map(
+    rigid_bodies = tuple(map(
         lambda rigid_body_data: cls.unpack_rigid_body(bytes(rigid_body_data)),
-        batched(data[offset:(offset:=offset+(cls.rigid_body_lenght*template['num_rigid_bodies']))], cls.rigid_body_lenght) 
+        batched(data[offset:(offset:=offset+(cls.rigid_body_lenght*num_rigid_bodies))], cls.rigid_body_lenght) 
     ))
-    return NatNetTypes.Rigid_body_data(**template), offset
+    return NatNetTypes.Rigid_body_data(num_rigid_bodies, rigid_bodies), offset
   
   @classmethod
-  def unpack_skeleton(cls, data:bytes) -> Tuple[NatNetTypes.Skeleton, int]:
+  def unpack_skeleton(cls, data: bytes) -> Tuple[NatNetTypes.Skeleton, int]:
     offset = 0
-    template = {}
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['rigid_bodies'] = tuple(map(
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_rigid_bodies = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    rigid_bodies = tuple(map(
         lambda rigid_body_data: cls.unpack_rigid_body(bytes(rigid_body_data)),
-        batched(data[offset:(offset:=offset+(cls.rigid_body_lenght*template['num_rigid_bodies']))], cls.rigid_body_lenght) 
+        batched(data[offset:(offset:=offset+(cls.rigid_body_lenght*num_rigid_bodies))], cls.rigid_body_lenght) 
     ))
-    return NatNetTypes.Skeleton(**template), offset
+    return NatNetTypes.Skeleton(identifier, num_rigid_bodies, rigid_bodies), offset
 
   @classmethod
-  def unpack_skeleton_data(cls, data:bytes) -> Tuple[NatNetTypes.Skeleton_data, int]:
+  def unpack_skeleton_data(cls, data: bytes) -> Tuple[NatNetTypes.Skeleton_data, int]:
     offset = 0
-    template = {}
-    template['num_skeletons'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_skeletons = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    skeletons = deque()
-    for _ in range(template['num_skeletons']):
+    skeletons: Iterable[NatNetTypes.Skeleton] = deque()
+    for _ in range(num_skeletons):
       skeleton, tmp_offset = cls.unpack_skeleton(data[offset:])
       offset += tmp_offset
       skeletons.append(skeleton)
-    template['skeletons'] = tuple(skeletons)
-    return NatNetTypes.Skeleton_data(**template), offset
+    skeletons = tuple(skeletons)
+    return NatNetTypes.Skeleton_data(num_skeletons, skeletons), offset
 
   @classmethod
-  def unpack_asset_rigid_body(cls, data:bytes) -> Tuple[NatNetTypes.Asset_RB, int]:
+  def unpack_asset_rigid_body(cls, data: bytes) -> NatNetTypes.Asset_RB:
     raise NotImplementedError("Subclasses must implement the unpack method")
 
   @classmethod
-  def unpack_asset_marker(cls, data:bytes) -> Tuple[NatNetTypes.Asset_marker, int]:
+  def unpack_asset_marker(cls, data: bytes) -> NatNetTypes.Asset_marker:
     raise NotImplementedError("Subclasses must implement the unpack method")
 
   @classmethod
-  def unpack_asset(cls, data:bytes) -> Tuple[NatNetTypes.Asset, int]:
+  def unpack_asset(cls, data: bytes) -> Tuple[NatNetTypes.Asset, int]:
     raise NotImplementedError("Subclasses must implement the unpack method")
 
   @classmethod
-  def unpack_asset_data(cls, data:bytes) -> Tuple[NatNetTypes.Asset_data, int]:
+  def unpack_asset_data(cls, data: bytes) -> Tuple[NatNetTypes.Asset_data, int]:
     raise NotImplementedError("Subclasses must implement the unpack method")
 
   @classmethod
-  def decode_marker_id(cls, id:int) -> Tuple[int, int]:
+  def decode_marker_id(cls, identifier: int) -> Tuple[int, int]:
     return (
-      id >> 16,
-      id & 0x0000ffff
+      identifier >> 16,
+      identifier & 0x0000ffff
     )
 
   @classmethod
-  def unpack_labeled_marker(cls, data:bytes) -> NatNetTypes.Labeled_marker:
+  def unpack_labeled_marker(cls, data: bytes) -> NatNetTypes.Labeled_marker:
     offset = 0
-    template = {}
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
-    template['size'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
-    template['param'] = unpack( 'h', data[offset:(offset:=offset+2)])[0]
-    template['residual'] = unpack('<f', data[offset:(offset:=offset+4)])[0] * 1000.0
-    return NatNetTypes.Labeled_marker(**template)
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    pos = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
+    size = unpack('<f', data[offset:(offset:=offset+4)])[0]
+    param = unpack( 'h', data[offset:(offset:=offset+2)])[0]
+    residual = unpack('<f', data[offset:(offset:=offset+4)])[0] * 1000.0
+    return NatNetTypes.Labeled_marker(identifier, pos, size, param, residual)
 
   @classmethod
-  def unpack_labeled_marker_data(cls, data:bytes) -> Tuple[NatNetTypes.Labeled_marker_data, int]:
+  def unpack_labeled_marker_data(cls, data: bytes) -> Tuple[NatNetTypes.Labeled_marker_data, int]:
     offset = 0
-    template = {}
-    template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_markers = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    template['markers'] = tuple(map(
+    markers = tuple(map(
       lambda marker_data: cls.unpack_labeled_marker(bytes(marker_data)),
-      batched(data[offset:(offset:=offset+(cls.marker_lenght*template['num_markers']))],cls.marker_lenght)
+      batched(data[offset:(offset:=offset+(cls.marker_lenght*num_markers))],cls.marker_lenght)
     ))
-    return NatNetTypes.Labeled_marker_data(**template), offset
+    return NatNetTypes.Labeled_marker_data(num_markers, markers), offset
 
   @classmethod
-  def unpack_channels(cls, data:bytes, num_channels:int) -> Tuple[Tuple[NatNetTypes.Channel, ...],int]:
+  def unpack_channels(cls, data: bytes, num_channels: int) -> Tuple[Tuple[NatNetTypes.Channel, ...], int]:
     offset = 0
-    channels = deque()
-    frame_unpacker = lambda frame_data: unpack('<f', bytes(frame_data))[0]
+    channels: Iterable[NatNetTypes.Channel] = deque()
+    frame_unpacker: Callable[[Iterable[int]], float] = lambda frame_data: unpack('<f', bytes(frame_data))[0]
     for _ in range(num_channels):
-      template_channel = {}
-      template_channel['num_frames'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      template_channel['frames'] = tuple(map(
+      num_frames = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+      frames = tuple(map(
         frame_unpacker,
-        batched(data[offset:(offset:=offset+(4*template_channel['num_frames']))],4)
+        batched(data[offset:(offset:=offset+(4*num_frames))],4)
       ))
-      channels.append(NatNetTypes.Channel(**template_channel))
+      channels.append(NatNetTypes.Channel(num_frames, frames))
     return tuple(channels), offset
 
   @classmethod
-  def unpack_force_plate_data(cls, data:bytes) -> Tuple[NatNetTypes.Force_plate_data, int]:
+  def unpack_force_plate_data(cls, data: bytes) -> Tuple[NatNetTypes.Force_plate_data, int]:
     offset = 0
-    template = {}
-    template['num_force_plates'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_force_plates = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    force_plates = deque()
-    for _ in range(template['num_force_plates']):
-      template_force_plate = {}
-      template_force_plate['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      template_force_plate['num_channels'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      template_force_plate['channels'], tmp_offset = cls.unpack_channels(data[offset:], template_force_plate['num_channels'])
+    force_plates: Iterable[NatNetTypes.Force_plate] = deque()
+    for _ in range(num_force_plates):
+      identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+      num_channels = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+      channels, tmp_offset = cls.unpack_channels(data[offset:], num_channels)
       offset += tmp_offset
-      force_plates.append(NatNetTypes.Force_plate(**template_force_plate))
-    template['force_plates'] = tuple(force_plates)
-    return NatNetTypes.Force_plate_data(**template), offset
+      force_plates.append(NatNetTypes.Force_plate(identifier, num_channels, channels))
+    force_plates = tuple(force_plates)
+    return NatNetTypes.Force_plate_data(num_force_plates, force_plates), offset
 
   @classmethod
-  def unpack_device_data(cls, data:bytes) -> Tuple[NatNetTypes.Device_data, int]:
+  def unpack_device_data(cls, data: bytes) -> Tuple[NatNetTypes.Device_data, int]:
     offset = 0
-    template = {}
-    template['num_devices'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_devices = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    devices = deque()
-    for _ in range(template['num_devices']):
-      template_device = {}
-      template_device['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      template_device['num_channels'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      template_device['channels'], tmp_offset = cls.unpack_channels(data[offset:], template_device['num_channels'])
+    devices: Iterable[NatNetTypes.Device] = deque()
+    for _ in range(num_devices):
+      identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+      num_channels = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+      channels, tmp_offset = cls.unpack_channels(data[offset:], num_channels)
       offset += tmp_offset
-      devices.append(NatNetTypes.Device(**template_device))
-    template['devices'] = tuple(devices)
-    return NatNetTypes.Device_data(**template), offset
+      devices.append(NatNetTypes.Device(identifier, num_channels, channels))
+    devices = tuple(devices)
+    return NatNetTypes.Device_data(num_devices, devices), offset
 
   @classmethod
-  def unpack_frame_suffix_data(cls, data:bytes) -> Tuple[NatNetTypes.Frame_suffix, int]:
-    offset = 0
-    template = {}
-    template['time_code'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['time_code_sub'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['timestamp'] = unpack('<d', data[offset:(offset:=offset+8)])[0]
-    template['camera_mid_exposure'] = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
-    template['stamp_data'] = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
-    template['stamp_transmit'] = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
+  def unpack_frame_suffix_data(cls, data: bytes) -> NatNetTypes.Frame_suffix:
+    offset = 0
+    time_code = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    time_code_sub = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    timestamp = unpack('<d', data[offset:(offset:=offset+8)])[0]
+    camera_mid_exposure = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
+    stamp_data = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
+    stamp_transmit = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
     param = unpack( 'h', data[offset:(offset:=offset+2)])[0]
-    template['recording'] = bool(param & 0x01)
-    template['tracked_models_changed'] = bool(param & 0x02)
-    return NatNetTypes.Frame_suffix(**template), offset
+    recording = bool(param & 0x01)
+    tracked_models_changed = bool(param & 0x02)
+    return NatNetTypes.Frame_suffix(time_code, time_code_sub, timestamp, camera_mid_exposure, stamp_data, stamp_transmit, recording, tracked_models_changed)
 
   @classmethod
-  def unpack_mocap_data(cls, data:bytes) -> NatNetTypes.MoCap:
+  def unpack_mocap_data(cls, data: bytes) -> NatNetTypes.MoCap:
     offset = 0
     tmp_offset = 0
-    template = {}
 
-    template['prefix_data'], tmp_offset = cls.unpack_frame_prefix_data(data[offset:])
+    prefix_data, tmp_offset = cls.unpack_frame_prefix_data(data[offset:])
     offset += tmp_offset
 
-    template['marker_set_data'], tmp_offset = cls.unpack_marker_set_data(data[offset:])
+    marker_set_data, tmp_offset = cls.unpack_marker_set_data(data[offset:])
     offset += tmp_offset
 
-    template['legacy_marker_set_data'], tmp_offset = cls.unpack_legacy_other_markers(data[offset:])
+    legacy_marker_set_data, tmp_offset = cls.unpack_legacy_other_markers(data[offset:])
     offset += tmp_offset
 
-    template['rigid_body_data'], tmp_offset = cls.unpack_rigid_body_data(data[offset:])
+    rigid_body_data, tmp_offset = cls.unpack_rigid_body_data(data[offset:])
     offset += tmp_offset
 
-    template['skeleton_data'], tmp_offset = cls.unpack_skeleton_data(data[offset:])
+    skeleton_data, tmp_offset = cls.unpack_skeleton_data(data[offset:])
     offset += tmp_offset
 
-    template['labeled_marker_data'], tmp_offset = cls.unpack_labeled_marker_data(data[offset:])
+    labeled_marker_data, tmp_offset = cls.unpack_labeled_marker_data(data[offset:])
     offset += tmp_offset
 
-    template['force_plate_data'], tmp_offset = cls.unpack_force_plate_data(data[offset:])
+    force_plate_data, tmp_offset = cls.unpack_force_plate_data(data[offset:])
     offset += tmp_offset
 
-    template['device_data'], tmp_offset = cls.unpack_device_data(data[offset:])
+    device_data, tmp_offset = cls.unpack_device_data(data[offset:])
     offset += tmp_offset
 
-    template['suffix_data'], tmp_offset = cls.unpack_frame_suffix_data(data[offset:])
-    offset += tmp_offset
+    suffix_data = cls.unpack_frame_suffix_data(data[offset:])
 
-    return NatNetTypes.MoCap(**template)
+    return NatNetTypes.MoCap(prefix_data, marker_set_data, legacy_marker_set_data, rigid_body_data, skeleton_data, labeled_marker_data, force_plate_data, device_data, suffix_data)
 
   @classmethod
-  def unpack_marker_set_description(cls, data:bytes) -> Tuple[Dict[str, NatNetTypes.Marker_set_description], int]:
+  def unpack_marker_set_description(cls, data: bytes) -> Tuple[Dict[str, NatNetTypes.Marker_set_description], int]:
     offset = 0
-    template = {}
     name, _, _ = data[offset:].partition(b'\0')
     offset += len(name) + 1
-    template['name'] = str(name, encoding="utf-8")
-    template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    names = deque()
-    for _ in range(template['num_markers']):
-      name, _, _ = data[offset:].partition(b'\0')
+    name = str(name, encoding="utf-8")
+    num_markers = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    markers_names: Iterable[str] = deque()
+    for _ in range(num_markers):
+      marker_name, _, _ = data[offset:].partition(b'\0')
       offset += len(name) + 1
-      names.append(str(name, encoding="utf-8"))
-    template['markers_names'] = tuple(names)
-    return {template['name']:NatNetTypes.Marker_set_description(**template)}, offset
+      markers_names.append(str(marker_name, encoding="utf-8"))
+    markers_names = tuple(markers_names)
+    return {name : NatNetTypes.Marker_set_description(name, num_markers, markers_names)}, offset
 
   @classmethod
-  def unpack_rigid_body_description(cls, data:bytes) -> Tuple[Dict[int, NatNetTypes.Rigid_body_description], int]:
+  def unpack_rigid_body_description(cls, data: bytes) -> Tuple[Dict[int, NatNetTypes.Rigid_body_description], int]:
     offset = 0
-    template = {}
     name, _, _ = data[offset:].partition(b'\0')
     offset += len(name) + 1
-    template['name'] = str(name, encoding="utf-8")
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['parent_id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
-    template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    name = str(name, encoding="utf-8")
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    parent_id = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    pos = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
+    num_markers = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     offset_pos = offset
-    offset_id = offset_pos + (12*template['num_markers'])
-    offset_name = offset_id + (4*template['num_markers'])
-    template["name"] = ""
-    markers = deque()
-    for _ in range(template['num_markers']):
-      template['pos'] = NatNetTypes.Position.unpack(data[offset_pos:(offset_pos:=offset_pos+12)])
-      template['id'] = int.from_bytes(data[offset_Y:(offset_Y:=offset_Y+4)], byteorder='little', signed=True)
-      markers.append(NatNetTypes.RB_marker(**template))
-    template['markers'] = tuple(markers)
-    return {template['id']:NatNetTypes.Rigid_body_description(**template)}, offset_name
+    offset_id = offset_pos + (12*num_markers)
+    offset_name = offset_id + (4*num_markers)
+    marker_name = ""
+    markers: Iterable[NatNetTypes.RB_marker] = deque()
+    for _ in range(num_markers):
+      marker_pos = NatNetTypes.Position.unpack(data[offset_pos:(offset_pos:=offset_pos+12)])
+      marker_id = int.from_bytes(data[offset_id:(offset_id:=offset_id+4)], byteorder='little', signed=True)
+      markers.append(NatNetTypes.RB_marker(marker_name, marker_id, marker_pos))
+    markers = tuple(markers)
+    return {identifier : NatNetTypes.Rigid_body_description(name, identifier, parent_id, pos, num_markers, markers)}, offset_name
 
   @classmethod
-  def unpack_skeleton_description(cls, data:bytes) -> Tuple[Dict[int, NatNetTypes.Skeleton_description], int]:
+  def unpack_skeleton_description(cls, data: bytes) -> Tuple[Dict[int, NatNetTypes.Skeleton_description], int]:
     offset = 0
-    template = {}
     name, _, _ = data[offset:].partition(b'\0')
     offset += len(name) + 1
-    template['name'] = str(name, encoding="utf-8")
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    rigid_bodies = deque()
-    for _ in range(template['num_rigid_bodies']):
+    name = str(name, encoding="utf-8")
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_rigid_bodies = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    rigid_bodies: Iterable[NatNetTypes.Rigid_body_description] = deque()
+    for _ in range(num_rigid_bodies):
       d, offset_tmp = cls.unpack_rigid_body_description(data[offset:])
       rigid_body = list(d.values())[0]
       rigid_bodies.append(rigid_body)
       offset += offset_tmp
-    template['rigid_bodies'] = tuple(rigid_bodies)
-    return {template['id']:NatNetTypes.Skeleton_description(**template)}, offset
+    rigid_bodies = tuple(rigid_bodies)
+    return {identifier : NatNetTypes.Skeleton_description(name, identifier, num_rigid_bodies, rigid_bodies)}, offset
 
   @classmethod
   def unpack_force_plate_description(cls, data: bytes) -> Tuple[Dict[str, NatNetTypes.Force_plate_description], int]:
     offset = 0
-    template = {}
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
 
     serial_number, _, _ = data[offset:].partition(b'\0')
     offset += len(serial_number) + 1
-    template['serial_number'] = str(serial_number, encoding='utf-8')
+    serial_number = str(serial_number, encoding='utf-8')
 
-    f_width:float = unpack('<f', data[offset:(offset:=offset+4)])[0]
-    f_length:float = unpack('<f', data[offset:(offset:=offset+4)])[0]
-    template['dimensions'] = (f_width, f_length)
+    f_width: float = unpack('<f', data[offset:(offset:=offset+4)])[0]
+    f_length: float = unpack('<f', data[offset:(offset:=offset+4)])[0]
+    dimensions = (f_width, f_length)
 
-    template['origin'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
+    origin = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
 
     # Not tested
-    template['calibration_matrix'] = tuple(unpack('<f', data[offset:(offset:=offset+4)])[0] for _ in range(12*12))
-    template['corners'] = tuple(unpack('<f', data[offset:(offset:=offset+4)])[0] for _ in range(4*3))
+    calibration_matrix = tuple(unpack('<f', data[offset:(offset:=offset+4)])[0] for _ in range(12*12))
+    corners = tuple(unpack('<f', data[offset:(offset:=offset+4)])[0] for _ in range(4*3))
 
-    template['plate_type'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    template['channel_data_type'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    template['num_channels'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    channels = deque()
-    for _ in range(template['num_channels']):
+    plate_type = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    channel_data_type = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    num_channels = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    
+    channels: Iterable[str] = deque()
+    for _ in range(num_channels):
       channel_name, _, _ = data[offset:].partition(b'\0')
       offset += len(channel_name) + 1
       channels.append(str(channel_name, encoding='utf-8'))
-    template['channels'] = tuple(channels)
-    return {template['serial_number']:NatNetTypes.Force_plate_description(**template)}, offset
+    channels = tuple(channels)
+    return {serial_number : NatNetTypes.Force_plate_description(identifier, serial_number, dimensions, origin, calibration_matrix, corners, plate_type, channel_data_type, num_channels, channels)}, offset
 
   @classmethod
   def unpack_device_description(cls, data: bytes) -> Tuple[Dict[str, NatNetTypes.Device_description], int]:
     offset = 0
-    template = {}
     
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
     
     name, _, _ = data[offset:].partition(b'\0')
     offset += len(name) + 1
-    template['name'] = str(name, encoding='utf-8')
+    name = str(name, encoding='utf-8')
     
     serial_number, _, _ = data[offset:].partition(b'\0')
     offset += len(serial_number) + 1
-    template['serial_number'] = str(serial_number, encoding='utf-8')
+    serial_number = str(serial_number, encoding='utf-8')
 
-    template['device_type'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    template['channel_data_type'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    template['num_channels'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    channels = deque()
-    for _ in range(template['num_channels']):
+    device_type = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    channel_data_type = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    num_channels = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    channels: Iterable[str] = deque()
+    for _ in range(num_channels):
       channel_name,_,_ = data[offset:].partition(b'\0')
       offset += len(channel_name) + 1
       channels.append(str(channel_name, encoding='utf-8'))
-    template['channels'] = tuple(channels)
-    return {template['serial_number']:NatNetTypes.Device_description(**template)}, offset
+    channels = tuple(channels)
+    return {serial_number : NatNetTypes.Device_description(identifier, name, serial_number, device_type, channel_data_type, num_channels, channels)}, offset
 
   @classmethod
-  def unpack_camera_description(cls, data:bytes) -> Tuple[Dict[bytes, NatNetTypes.Camera_description], int]:
+  def unpack_camera_description(cls, data: bytes) -> Tuple[Dict[str, NatNetTypes.Camera_description], int]:
     offset = 0
-    template = {}
     name, _, _ = data[offset:].partition(b'\0')
     offset += len(name) + 1
-    template['name'] = str(name, encoding="utf-8")
-    template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
-    template['orientation'] = NatNetTypes.Quaternion.unpack(data[offset:(offset:=offset+16)])
-    return {name:NatNetTypes.Camera_description(**template)}, offset
+    name = str(name, encoding="utf-8")
+    pos = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
+    orientation = NatNetTypes.Quaternion.unpack(data[offset:(offset:=offset+16)])
+    return {name : NatNetTypes.Camera_description(name, pos, orientation)}, offset
 
   @classmethod
-  def unpack_marker_description(cls, data:bytes) -> Tuple[Dict[int, NatNetTypes.Marker_description], int]:
+  def unpack_marker_description(cls, data: bytes) -> Tuple[Dict[int, NatNetTypes.Marker_description], int]:
     offset = 0
-    template = {}
     name, _, _ = data[offset:].partition(b'\0')
     offset += len(name) + 1
-    template['name'] = str(name, encoding="utf-8")
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
-    template['size'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
-    template['param'] = unpack( 'h', data[offset:(offset:=offset+2)])[0]
-    return {template['id']:NatNetTypes.Marker_description(**template)}, offset
+    name = str(name, encoding="utf-8")
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    pos = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
+    size = unpack('<f', data[offset:(offset:=offset+4)])[0]
+    param = unpack( 'h', data[offset:(offset:=offset+2)])[0]
+    return {identifier : NatNetTypes.Marker_description(name, identifier, pos, size, param)}, offset
 
   @classmethod
-  def unpack_asset_description(cls, data:bytes) -> Tuple[Dict[int, NatNetTypes.Asset_description], int]:
+  def unpack_asset_description(cls, data: bytes) -> Tuple[Dict[int, NatNetTypes.Asset_description], int]:
     offset = 0
-    template = {}
     name, _, _ = data[offset:].partition(b'\0')
     offset += len(name) + 1
-    template['name'] = str(name, encoding="utf-8")
-    template['type'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    rigid_bodies = deque()
-    for _ in range(template['num_rigid_bodies']):
+    name = str(name, encoding="utf-8")
+    asset_type = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    num_rigid_bodies = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    rigid_bodies: Iterable[NatNetTypes.Rigid_body_description] = deque()
+    for _ in range(num_rigid_bodies):
       d, offset_tmp = cls.unpack_rigid_body_description(data[offset:])
       rigid_body = list(d.values())[0]
       rigid_bodies.append(rigid_body)
       offset += offset_tmp
-    template['rigid_bodies'] = tuple(rigid_bodies)
-    template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
-    markers = deque()
-    for _ in range(template['num_markers']):
+    rigid_bodies = tuple(rigid_bodies)
+    num_markers = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little',  signed=True)
+    markers: Iterable[NatNetTypes.Marker_description] = deque()
+    for _ in range(num_markers):
       d,offset_tmp = cls.unpack_marker_description(data[offset:])
       marker = list(d.values())[0]
       markers.append(marker)
       offset += offset_tmp
-    template['markers'] = tuple(markers)
-    return {template['id']:NatNetTypes.Asset_description(**template)}, offset
+    markers = tuple(markers)
+    return {identifier : NatNetTypes.Asset_description(name, asset_type, identifier, num_rigid_bodies, rigid_bodies, num_markers, markers)}, offset
 
 class DataUnpackerV4_1(DataUnpackerV3_0):
-  asset_rigid_body_lenght:int = 38
+  asset_rigid_body_lenght: int = 38
   asset_marker_lenght: int = 26
+  frame_suffix_lenght: int = 50
+
   @classmethod
   def unpack_data_size(cls, data: bytes) -> Tuple[int, int]:
     offset = 0
     size_in_bytes = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     return size_in_bytes, offset
 
   @classmethod
-  def unpack_asset_rigid_body(cls, data:bytes) -> NatNetTypes.Asset_RB:
+  def unpack_asset_rigid_body(cls, data: bytes) -> NatNetTypes.Asset_RB:
     offset = 0
-    template = {}
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
-    template['rot'] = NatNetTypes.Quaternion.unpack(data[offset:(offset:=offset+16)])
-    template['err'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
-    template['param'] = unpack( 'h', data[offset:(offset:=offset+2)])[0]
-    return NatNetTypes.Asset_RB(**template)
-
-  @classmethod
-  def unpack_asset_marker(cls, data:bytes) -> NatNetTypes.Asset_marker:
-    offset = 0
-    template = {}
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
-    template['size'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
-    template['param'] = unpack( 'h', data[offset:(offset:=offset+2)])[0]
-    template['residual'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
-    return NatNetTypes.Asset_marker(**template)
-
-  @classmethod
-  def unpack_asset(cls, data:bytes) -> Tuple[NatNetTypes.Asset, int]:
-    offset = 0
-    template = {}
-    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['rigid_bodies'] = tuple(map(
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    pos = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
+    rot = NatNetTypes.Quaternion.unpack(data[offset:(offset:=offset+16)])
+    err = unpack('<f', data[offset:(offset:=offset+4)])[0]
+    param = unpack( 'h', data[offset:(offset:=offset+2)])[0]
+    return NatNetTypes.Asset_RB(identifier, pos, rot, err, param)
+
+  @classmethod
+  def unpack_asset_marker(cls, data: bytes) -> NatNetTypes.Asset_marker:
+    offset = 0
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    pos = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
+    size = unpack('<f', data[offset:(offset:=offset+4)])[0]
+    param = unpack( 'h', data[offset:(offset:=offset+2)])[0]
+    residual = unpack('<f', data[offset:(offset:=offset+4)])[0]
+    return NatNetTypes.Asset_marker(identifier, pos, size, param, residual)
+
+  @classmethod
+  def unpack_asset(cls, data: bytes) -> Tuple[NatNetTypes.Asset, int]:
+    offset = 0
+    identifier = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_rigid_bodies = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    rigid_bodies = tuple(map(
       lambda rigid_body_data: cls.unpack_asset_rigid_body(bytes(rigid_body_data)),
-      batched(data[offset:(offset:=offset+(cls.asset_rigid_body_lenght*template['num_rigid_bodies']))], cls.asset_rigid_body_lenght)
+      batched(data[offset:(offset:=offset+(cls.asset_rigid_body_lenght*num_rigid_bodies))], cls.asset_rigid_body_lenght)
     ))
-    template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['markers'] = tuple(map(
+    num_markers = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    markers = tuple(map(
       lambda marker_data: cls.unpack_asset_marker(bytes(marker_data)),
-      batched(data[offset:(offset:=offset+(cls.asset_marker_lenght*template['num_markers']))], cls.asset_marker_lenght)
+      batched(data[offset:(offset:=offset+(cls.asset_marker_lenght*num_markers))], cls.asset_marker_lenght)
     ))
-    return NatNetTypes.Asset(**template), offset
+    return NatNetTypes.Asset(identifier, num_rigid_bodies, rigid_bodies, num_markers, markers), offset
 
   @classmethod
-  def unpack_asset_data(cls, data:bytes) -> Tuple[NatNetTypes.Asset_data, int]:
+  def unpack_asset_data(cls, data: bytes) -> Tuple[NatNetTypes.Asset_data, int]:
     offset = 0
-    template = {}
-    template['num_assets'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    num_assets = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    assets = deque()
-    for _ in range(template['num_assets']):
+    assets: Iterable[NatNetTypes.Asset] = deque()
+    for _ in range(num_assets):
       asset, tmp_offset = cls.unpack_asset(data[offset:])
       offset += tmp_offset
       assets.append(asset)
-    template['assets'] = tuple(assets)
-    return NatNetTypes.Asset_data(**template), offset
+    assets = tuple(assets)
+    return NatNetTypes.Asset_data(num_assets, assets), offset
 
   @classmethod
-  def unpack_frame_suffix_data(cls, data:bytes) -> Tuple[NatNetTypes.Frame_suffix, int]:
+  def unpack_frame_suffix_data(cls, data: bytes) -> NatNetTypes.Frame_suffix:
     offset = 0
-    template = {}
-    template['time_code'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['time_code_sub'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['timestamp'] = unpack('<d', data[offset:(offset:=offset+8)])[0]
-    template['camera_mid_exposure'] = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
-    template['stamp_data'] = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
-    template['stamp_transmit'] = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
-    template['precision_timestamp_sec'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    template['precision_timestamp_frac_sec'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    time_code = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    time_code_sub = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    timestamp = unpack('<d', data[offset:(offset:=offset+8)])[0]
+    camera_mid_exposure = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
+    stamp_data = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
+    stamp_transmit = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
+    precision_timestamp_sec = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    precision_timestamp_frac_sec = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     param = unpack( 'h', data[offset:(offset:=offset+2)])[0]
-    template['recording'] = bool(param & 0x01)
-    template['tracked_models_changed'] = bool(param & 0x02)
-    return NatNetTypes.Frame_suffix(**template), offset
+    recording = bool(param & 0x01)
+    tracked_models_changed = bool(param & 0x02)
+    return NatNetTypes.Frame_suffix(time_code, time_code_sub, timestamp, camera_mid_exposure, stamp_data, stamp_transmit, recording, tracked_models_changed, precision_timestamp_sec, precision_timestamp_frac_sec)
 
   @classmethod
-  def unpack_mocap_data(cls, data:bytes) -> NatNetTypes.MoCap:
+  def unpack_mocap_data(cls, data: bytes) -> NatNetTypes.MoCap:
     offset = 0
     tmp_offset = 0
-    template = {}
 
-    template['prefix_data'], tmp_offset = cls.unpack_frame_prefix_data(data[offset:])
+    prefix_data, tmp_offset = cls.unpack_frame_prefix_data(data[offset:])
     offset += tmp_offset
 
-    template['marker_set_data'], tmp_offset = cls.unpack_marker_set_data(data[offset:])
+    marker_set_data, tmp_offset = cls.unpack_marker_set_data(data[offset:])
     offset += tmp_offset
 
-    template['legacy_marker_set_data'], tmp_offset = cls.unpack_legacy_other_markers(data[offset:])
+    legacy_marker_set_data, tmp_offset = cls.unpack_legacy_other_markers(data[offset:])
     offset += tmp_offset
 
-    template['rigid_body_data'], tmp_offset = cls.unpack_rigid_body_data(data[offset:])
+    rigid_body_data, tmp_offset = cls.unpack_rigid_body_data(data[offset:])
     offset += tmp_offset
 
-    template['skeleton_data'], tmp_offset = cls.unpack_skeleton_data(data[offset:])
+    skeleton_data, tmp_offset = cls.unpack_skeleton_data(data[offset:])
     offset += tmp_offset
 
-    template['asset_data'], tmp_offset = cls.unpack_asset_data(data[offset:])
+    asset_data, tmp_offset = cls.unpack_asset_data(data[offset:])
     offset += tmp_offset
 
-    template['labeled_marker_data'], tmp_offset = cls.unpack_labeled_marker_data(data[offset:])
+    labeled_marker_data, tmp_offset = cls.unpack_labeled_marker_data(data[offset:])
     offset += tmp_offset
 
-    template['force_plate_data'], tmp_offset = cls.unpack_force_plate_data(data[offset:])
+    force_plate_data, tmp_offset = cls.unpack_force_plate_data(data[offset:])
     offset += tmp_offset
 
-    template['device_data'], tmp_offset = cls.unpack_device_data(data[offset:])
+    device_data, tmp_offset = cls.unpack_device_data(data[offset:])
     offset += tmp_offset
 
-    template['suffix_data'], tmp_offset = cls.unpack_frame_suffix_data(data[offset:])
-    offset += tmp_offset
+    suffix_data = cls.unpack_frame_suffix_data(data[offset:])
 
-    return NatNetTypes.MoCap(**template)
+    return NatNetTypes.MoCap(prefix_data, marker_set_data, legacy_marker_set_data, rigid_body_data, skeleton_data, labeled_marker_data, force_plate_data, device_data, suffix_data, asset_data)
 
   @classmethod
   def unpack_rigid_body_description(cls, data: bytes) -> Tuple[Dict[int, NatNetTypes.Rigid_body_description], int]:
     d, offset = super().unpack_rigid_body_description(data)
-    rb_desc = asdict(list(d.values())[0])
-    markers = deque()
-    for marker in rb_desc['markers']:
-      template_marker = asdict(marker)
+    rb_desc = tuple(d.values())[0]
+    for marker in rb_desc.markers:
       name, _, _ = data[offset:].partition(b'\0')
       offset += len(name) + 1
-      template_marker['name'] = str(name, encoding="utf-8")
-      markers.append(NatNetTypes.RB_marker(**template_marker))
-    rb_desc['markers'] = tuple(markers)
-    return {rb_desc['id']:NatNetTypes.Rigid_body_description(**rb_desc)}, offset
+      marker.name = str(name, encoding="utf-8")
+    return d, offset
```

### Comparing `new_natnet_client-4.2.0/PKG-INFO` & `new_natnet_client-4.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: new-natnet-client
-Version: 4.2.0
+Version: 4.3.0
 Summary: natnet client for motive application for python
 Home-page: https://optitrack.com/
 License: GLWTPL
 Author: Ignacio de la Torre Arias
 Author-email: ignaciodlta@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
```

