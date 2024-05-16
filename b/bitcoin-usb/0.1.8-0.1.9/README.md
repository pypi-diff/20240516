# Comparing `tmp/bitcoin_usb-0.1.8.tar.gz` & `tmp/bitcoin_usb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_usb-0.1.8.tar", max compression
+gzip compressed data, was "bitcoin_usb-0.1.9.tar", max compression
```

## Comparing `bitcoin_usb-0.1.8.tar` & `bitcoin_usb-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-09 17:54:40.000000 bitcoin_usb-0.1.8/LICENSE
--rw-r--r--   0        0        0     1170 2024-01-13 13:12:03.000000 bitcoin_usb-0.1.8/README.md
--rw-r--r--   0        0        0       53 2023-12-22 13:21:26.000000 bitcoin_usb-0.1.8/bitcoin_usb/__init__.py
--rw-r--r--   0        0        0    12842 2024-02-17 14:52:24.532339 bitcoin_usb-0.1.8/bitcoin_usb/address_types.py
--rw-r--r--   0        0        0     4388 2024-01-13 13:12:25.000000 bitcoin_usb-0.1.8/bitcoin_usb/device.py
--rw-r--r--   0        0        0     7907 2024-02-08 12:39:42.231241 bitcoin_usb-0.1.8/bitcoin_usb/gui.py
--rw-r--r--   0        0        0     4044 2024-01-13 13:12:25.000000 bitcoin_usb-0.1.8/bitcoin_usb/seed_tools.py
--rw-r--r--   0        0        0     3936 2024-01-13 13:12:25.000000 bitcoin_usb-0.1.8/bitcoin_usb/software_signer.py
--rw-r--r--   0        0        0      742 2024-02-17 14:52:48.648827 bitcoin_usb-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 bitcoin_usb-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-09 17:54:40.000000 bitcoin_usb-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1170 2024-01-13 13:12:03.000000 bitcoin_usb-0.1.9/README.md
+-rw-r--r--   0        0        0       53 2023-12-22 13:21:26.000000 bitcoin_usb-0.1.9/bitcoin_usb/__init__.py
+-rw-r--r--   0        0        0    12955 2024-02-18 12:01:35.029512 bitcoin_usb-0.1.9/bitcoin_usb/address_types.py
+-rw-r--r--   0        0        0     4388 2024-01-13 13:12:25.000000 bitcoin_usb-0.1.9/bitcoin_usb/device.py
+-rw-r--r--   0        0        0     7995 2024-03-03 16:49:02.020201 bitcoin_usb-0.1.9/bitcoin_usb/gui.py
+-rw-r--r--   0        0        0     4044 2024-01-13 13:12:25.000000 bitcoin_usb-0.1.9/bitcoin_usb/seed_tools.py
+-rw-r--r--   0        0        0     3936 2024-01-13 13:12:25.000000 bitcoin_usb-0.1.9/bitcoin_usb/software_signer.py
+-rw-r--r--   0        0        0      742 2024-03-03 13:44:11.904597 bitcoin_usb-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 bitcoin_usb-0.1.9/PKG-INFO
```

### Comparing `bitcoin_usb-0.1.8/LICENSE` & `bitcoin_usb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_usb-0.1.8/README.md` & `bitcoin_usb-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bitcoin_usb-0.1.8/bitcoin_usb/address_types.py` & `bitcoin_usb-0.1.9/bitcoin_usb/address_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
-from typing import Callable, Dict, List
+from typing import Callable, Dict, List, Optional
 
 import bdkpython as bdk
 from hwilib.common import AddressType as HWIAddressType
 from hwilib.descriptor import (
+    Descriptor,
     MultisigDescriptor,
     PKHDescriptor,
     PubkeyProvider,
     SHDescriptor,
     TRDescriptor,
     WPKHDescriptor,
     WSHDescriptor,
@@ -235,30 +236,32 @@
         )
         return provider
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.__dict__})"
 
 
-def _get_descriptor_instances(descriptor):
+def _get_descriptor_instances(descriptor: Descriptor) -> List[Descriptor]:
     "Returns the linear chain of chained descriptors . Multiple subdescriptors return an error"
     assert len(descriptor.subdescriptors) <= 1
     if descriptor.subdescriptors:
         result = [descriptor]
         for subdescriptor in descriptor.subdescriptors:
             result += _get_descriptor_instances(subdescriptor)
         return result
     else:
         return [descriptor]
 
 
-def _find_matching_address_type(instance_tuple, address_types: List[AddressType]):
+def _find_matching_address_type(
+    descriptor_tuple: List[Descriptor], address_types: List[AddressType]
+) -> Optional[AddressType]:
     for address_type in address_types:
-        if len(instance_tuple) == len(address_type.hwi_descriptor_classes) and all(
-            isinstance(i, c) for i, c in zip(instance_tuple, address_type.hwi_descriptor_classes)
+        if len(descriptor_tuple) == len(address_type.hwi_descriptor_classes) and all(
+            isinstance(i, c) for i, c in zip(descriptor_tuple, address_type.hwi_descriptor_classes)
         ):
             return address_type
     return None
 
 
 class DescriptorInfo:
     def __init__(
```

### Comparing `bitcoin_usb-0.1.8/bitcoin_usb/device.py` & `bitcoin_usb-0.1.9/bitcoin_usb/device.py`

 * *Files identical despite different names*

### Comparing `bitcoin_usb-0.1.8/bitcoin_usb/gui.py` & `bitcoin_usb-0.1.9/bitcoin_usb/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,17 @@
         self.accept()
 
     def get_selected_device(self):
         return self.selected_device
 
 
 class InfoDialog(QDialog):
-    def __init__(self, message):
+    def __init__(self, message, title="Info"):
         super().__init__()
+        self.setWindowTitle(title)
 
         # Set up the dialog layout
         layout = QVBoxLayout()
 
         # Add a label with the information message
         message_label = QLabel(message)
         layout.addWidget(message_label)
@@ -67,24 +68,24 @@
         self.autoselect_if_1_device = autoselect_if_1_device
         self.network = network
         self.parent = parent
 
     def get_device(self) -> Dict:
         devices = hwi_commands.enumerate()
         if not devices:
-            InfoDialog("No USB devices found").exec_()
+            InfoDialog("No USB devices found", title="USB Devices").exec()
             return {}
         if len(devices) == 1 and self.autoselect_if_1_device:
             return devices[0]
         else:
             dialog = DeviceDialog(self.parent, devices, self.network)
-            if dialog.exec_():
+            if dialog.exec():
                 return dialog.get_selected_device()
             else:
-                InfoDialog("No device selected").exec_()
+                InfoDialog("No device selected", title="USB Devices").exec()
         return {}
 
     def sign(self, psbt: bdk.PartiallySignedTransaction) -> bdk.PartiallySignedTransaction:
         selected_device = self.get_device()
         if selected_device:
             with USBDevice(selected_device, self.network) as dev:
                 return dev.sign_psbt(psbt)
```

### Comparing `bitcoin_usb-0.1.8/bitcoin_usb/seed_tools.py` & `bitcoin_usb-0.1.9/bitcoin_usb/seed_tools.py`

 * *Files identical despite different names*

### Comparing `bitcoin_usb-0.1.8/bitcoin_usb/software_signer.py` & `bitcoin_usb-0.1.9/bitcoin_usb/software_signer.py`

 * *Files identical despite different names*

### Comparing `bitcoin_usb-0.1.8/pyproject.toml` & `bitcoin_usb-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 show_error_codes = true 
 disable_error_code = "assignment"
 
 
 
 [tool.poetry]
 name = "bitcoin-usb"
-version = "0.1.8"
+version = "0.1.9"
 authors = ["andreasgriffin <andreasgriffin@proton.me>"]
 license = "GPL-3.0"
 readme = "README.md"
 description = "Wrapper around hwi, such that one can sign bdk PSBTs directly"
 homepage = "https://github.com/andreasgriffin/bitcoin-usb"
 
 [tool.poetry.dependencies]
```

### Comparing `bitcoin_usb-0.1.8/PKG-INFO` & `bitcoin_usb-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin-usb
-Version: 0.1.8
+Version: 0.1.9
 Summary: Wrapper around hwi, such that one can sign bdk PSBTs directly
 Home-page: https://github.com/andreasgriffin/bitcoin-usb
 License: GPL-3.0
 Author: andreasgriffin
 Author-email: andreasgriffin@proton.me
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

