# Comparing `tmp/tinyCUCM-0.2.6.tar.gz` & `tmp/tinycucm-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyCUCM-0.2.6.tar", last modified: Mon Mar 18 18:26:08 2024, max compression
+gzip compressed data, was "tinycucm-0.2.7.tar", last modified: Sat Apr 27 06:30:53 2024, max compression
```

## Comparing `tinyCUCM-0.2.6.tar` & `tinycucm-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-03-18 18:26:08.702471 tinyCUCM-0.2.6/
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     1065 2023-12-14 09:02:09.000000 tinyCUCM-0.2.6/LICENSE
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    53418 2024-03-18 18:26:08.701731 tinyCUCM-0.2.6/PKG-INFO
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    52843 2024-03-18 17:20:36.000000 tinyCUCM-0.2.6/README.md
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      655 2024-03-18 17:09:58.000000 tinyCUCM-0.2.6/pyproject.toml
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)       38 2024-03-18 18:26:08.702575 tinyCUCM-0.2.6/setup.cfg
-drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-03-18 18:26:08.687137 tinyCUCM-0.2.6/src/
-drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-03-18 18:26:08.696662 tinyCUCM-0.2.6/src/tinyCUCM/
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      102 2024-03-06 09:24:29.000000 tinyCUCM-0.2.6/src/tinyCUCM/__init__.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     1011 2024-03-06 11:07:28.000000 tinyCUCM-0.2.6/src/tinyCUCM/ccs_models.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    58379 2024-03-18 17:49:14.000000 tinyCUCM-0.2.6/src/tinyCUCM/client.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     3710 2023-12-21 12:52:06.000000 tinyCUCM-0.2.6/src/tinyCUCM/decorators.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      811 2023-12-14 16:21:28.000000 tinyCUCM-0.2.6/src/tinyCUCM/exceptions.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     1152 2024-03-06 11:07:52.000000 tinyCUCM-0.2.6/src/tinyCUCM/ris_models.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     7709 2024-03-05 12:40:59.000000 tinyCUCM-0.2.6/src/tinyCUCM/settings.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     4856 2024-03-18 16:33:58.000000 tinyCUCM-0.2.6/src/tinyCUCM/sql_models.py
-drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-03-18 18:26:08.700921 tinyCUCM-0.2.6/src/tinyCUCM.egg-info/
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    53418 2024-03-18 18:26:08.000000 tinyCUCM-0.2.6/src/tinyCUCM.egg-info/PKG-INFO
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      419 2024-03-18 18:26:08.000000 tinyCUCM-0.2.6/src/tinyCUCM.egg-info/SOURCES.txt
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        1 2024-03-18 18:26:08.000000 tinyCUCM-0.2.6/src/tinyCUCM.egg-info/dependency_links.txt
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)       28 2024-03-18 18:26:08.000000 tinyCUCM-0.2.6/src/tinyCUCM.egg-info/requires.txt
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        9 2024-03-18 18:26:08.000000 tinyCUCM-0.2.6/src/tinyCUCM.egg-info/top_level.txt
+drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-04-27 06:30:53.567836 tinycucm-0.2.7/
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     1065 2023-12-14 09:02:09.000000 tinycucm-0.2.7/LICENSE
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    53467 2024-04-27 06:30:53.566080 tinycucm-0.2.7/PKG-INFO
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    52892 2024-04-27 06:01:49.000000 tinycucm-0.2.7/README.md
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      655 2024-03-20 15:22:19.000000 tinycucm-0.2.7/pyproject.toml
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)       38 2024-04-27 06:30:53.568165 tinycucm-0.2.7/setup.cfg
+drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-04-27 06:30:53.550008 tinycucm-0.2.7/src/
+drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-04-27 06:30:53.559106 tinycucm-0.2.7/src/tinyCUCM/
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      102 2024-03-06 09:24:29.000000 tinycucm-0.2.7/src/tinyCUCM/__init__.py
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     1011 2024-03-06 11:07:28.000000 tinycucm-0.2.7/src/tinyCUCM/ccs_models.py
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    59086 2024-04-27 06:18:56.000000 tinycucm-0.2.7/src/tinyCUCM/client.py
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     3812 2024-04-27 06:18:56.000000 tinycucm-0.2.7/src/tinyCUCM/decorators.py
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      811 2023-12-14 16:21:28.000000 tinycucm-0.2.7/src/tinyCUCM/exceptions.py
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     1152 2024-03-06 11:07:52.000000 tinycucm-0.2.7/src/tinyCUCM/ris_models.py
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     7822 2024-04-05 07:35:16.000000 tinycucm-0.2.7/src/tinyCUCM/settings.py
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     4856 2024-03-18 16:33:58.000000 tinycucm-0.2.7/src/tinyCUCM/sql_models.py
+drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-04-27 06:30:53.564668 tinycucm-0.2.7/src/tinyCUCM.egg-info/
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    53467 2024-04-27 06:30:53.000000 tinycucm-0.2.7/src/tinyCUCM.egg-info/PKG-INFO
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      419 2024-04-27 06:30:53.000000 tinycucm-0.2.7/src/tinyCUCM.egg-info/SOURCES.txt
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        1 2024-04-27 06:30:53.000000 tinycucm-0.2.7/src/tinyCUCM.egg-info/dependency_links.txt
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)       28 2024-04-27 06:30:53.000000 tinycucm-0.2.7/src/tinyCUCM.egg-info/requires.txt
+-rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        9 2024-04-27 06:30:53.000000 tinycucm-0.2.7/src/tinyCUCM.egg-info/top_level.txt
```

### Comparing `tinyCUCM-0.2.6/LICENSE` & `tinycucm-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyCUCM-0.2.6/PKG-INFO` & `tinycucm-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyCUCM
-Version: 0.2.6
+Version: 0.2.7
 Summary: Cisco Unified Call Manager AXL Methods Collection.
 Author-email: Luarvick <lu.luarvick@gmail.com>
 Project-URL: Homepage, https://github.com/luarvick/tinyCUCM
 Project-URL: Issues, https://github.com/luarvick/tinyCUCM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -126,15 +126,16 @@
     "pub_version": "11.5",
     "user_login": "Your-CUCM-Account",
     "user_password": "You%wILL#&neVeR!gUEss",
     "toolkit_path": BASE_DIR / "axlsqltoolkit",
     "cert_path": BASE_DIR / "cucm.crt",
     "session_verify": False,
     "session_timeout": 15,
-    "ris_wsdl_filename": "wsdlRISService70_test.xml", 
+    "ccs_wsdl_filename": "wsdlControlCenterServices_test.xml",
+    "ris_wsdl_filename": "wsdlRISService70_test.xml",
 }
 
 if __name__ == "__main__":
     cucm = CucmClient(**settings)
     # Get All AXL Method Names
     print("Result:", cucm.axlAllMethods())
     # Result: (
@@ -1879,14 +1880,15 @@
   * `sqlSearchRemoteDestination` - required keywords args: `criterion`, `value`
     * `criterion` enum: `Name`, `Destination`
   * `sqlSearchTranslationPattern` - required keywords args: `criterion`, `value`
     * `criterion` enum: `Pattern`, `Description`, `Partition`, `Calling Search Space`, `Called Party Transform Mask`,
       `Prefix Digits Out` 
 * `Validate` Methods:
   * `sqlValidateDeviceEndUserDesignation` - required keywords args: `device` (Type Class: Any)
+  * `sqlValidateEndUser` - required keywords args: `userid`
   * `sqlValidateLine` - required keywords args: `pattern` (Type Pattern Usage: Device Only)
   * `sqlValidatePattern` - required keywords args: `pattern` (Type Pattern Usage: Any)
 
 </details>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
@@ -1897,15 +1899,15 @@
 
 <details>
 <summary>Code Example:</summary>
 
 ```python
 from pathlib import Path
 from typing import Union
-from tinyCUCM import CucmSettings, cucm_logging
+from tinyCUCM import CucmClient, cucm_logging
 
 
 BASE_DIR = Path(__file__).resolve().parent
 settings = {
     "pub_fqdn": "cucm.example.com",
     "pub_version": "11.5",
     "user_login": "Your-CUCM-Account",
@@ -1914,17 +1916,15 @@
     "cert_path": BASE_DIR / "cucm.crt",
     "session_verify": False,
     "session_timeout": 15,
     "ris_wsdl_filename": "wsdlRISService70_test.xml", 
 }
 
 
-class CucmAxlCustom(CucmSettings):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+class CucmAxlCustom(CucmClient):
         
     @cucm_logging
     def axlYourOwnGetMethod(self, **kwargs: Union[dict, ...]) -> dict:
 
         """
         AXL Your Own `Get` or Any Other Method.
         :param kwargs:      Required Fields:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyCUCM Version: 0.2.6 Summary: Cisco Unified Call
+Metadata-Version: 2.1 Name: tinyCUCM Version: 0.2.7 Summary: Cisco Unified Call
 Manager AXL Methods Collection. Author-email: Luarvick
 gmail.com> Project-URL: Homepage, https://github.com/luarvick/tinyCUCM Project-
 URL: Issues, https://github.com/luarvick/tinyCUCM/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 zeep==4.2.1 Requires-Dist: pydantic==2.6.3
@@ -60,21 +60,21 @@
 object to the local variable `cucm`. **Don't store sensitive information in
 source code. For example use ".env" file.** Code Example: ```python from
 pathlib import Path from tinyCUCM import CucmClient BASE_DIR = Path
 (__file__).resolve().parent settings = { "pub_fqdn": "cucm.example.com",
 "pub_version": "11.5", "user_login": "Your-CUCM-Account", "user_password":
 "You%wILL#&neVeR!gUEss", "toolkit_path": BASE_DIR / "axlsqltoolkit",
 "cert_path": BASE_DIR / "cucm.crt", "session_verify": False, "session_timeout":
-15, "ris_wsdl_filename": "wsdlRISService70_test.xml", } if __name__ ==
-"__main__": cucm = CucmClient(**settings) # Get All AXL Method Names print
-("Result:", cucm.axlAllMethods()) # Result: ( # 'addAarGroup', #
-'addAdvertisedPatterns', # 'addAnnouncement', # 'addAppServerInfo', #
-'addAppUser', # ..., # 'updateWifiHotspot', #
-'updateWirelessAccessPointControllers', # 'updateWlanProfileGroup', #
-'wipePhone' # ) ```
+15, "ccs_wsdl_filename": "wsdlControlCenterServices_test.xml",
+"ris_wsdl_filename": "wsdlRISService70_test.xml", } if __name__ == "__main__":
+cucm = CucmClient(**settings) # Get All AXL Method Names print("Result:",
+cucm.axlAllMethods()) # Result: ( # 'addAarGroup', # 'addAdvertisedPatterns', #
+'addAnnouncement', # 'addAppServerInfo', # 'addAppUser', # ..., #
+'updateWifiHotspot', # 'updateWirelessAccessPointControllers', #
+'updateWlanProfileGroup', # 'wipePhone' # ) ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### AXL Collection #### Add Methods * `axlAddCallPickupGroup` keywords args *
 required: * `callPickupGroup` * `name` * `pattern` * expected: * `description`
 * `routePartitionName` * `members` * `pickupNotification` *
 `pickupNotificationTimer` * `callInfoForPickupNotification` *
 `axlAddDeviceProfile` keywords args * required: * `deviceProfile` * `name` *
 `product` * `class` * `protocol` * `protocolSide` * `phoneTemplateName` *
@@ -578,32 +578,32 @@
 `criterion` enum: `Name`, `Member Line Number`, `Member Line Description` *
 `sqlSearchRemoteDestination` - required keywords args: `criterion`, `value` *
 `criterion` enum: `Name`, `Destination` * `sqlSearchTranslationPattern` -
 required keywords args: `criterion`, `value` * `criterion` enum: `Pattern`,
 `Description`, `Partition`, `Calling Search Space`, `Called Party Transform
 Mask`, `Prefix Digits Out` * `Validate` Methods: *
 `sqlValidateDeviceEndUserDesignation` - required keywords args: `device` (Type
-Class: Any) * `sqlValidateLine` - required keywords args: `pattern` (Type
-Pattern Usage: Device Only) * `sqlValidatePattern` - required keywords args:
-`pattern` (Type Pattern Usage: Any)
+Class: Any) * `sqlValidateEndUser` - required keywords args: `userid` *
+`sqlValidateLine` - required keywords args: `pattern` (Type Pattern Usage:
+Device Only) * `sqlValidatePattern` - required keywords args: `pattern` (Type
+Pattern Usage: Any)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Create Your Own Methods **Don't store sensitive information in source code.
 For example use ".env" file.** Code Example: ```python from pathlib import Path
-from typing import Union from tinyCUCM import CucmSettings, cucm_logging
-BASE_DIR = Path(__file__).resolve().parent settings = { "pub_fqdn":
-"cucm.example.com", "pub_version": "11.5", "user_login": "Your-CUCM-Account",
-"user_password": "You%wILL#&neVeR!gUEss", "toolkit_path": BASE_DIR /
-"axlsqltoolkit", "cert_path": BASE_DIR / "cucm.crt", "session_verify": False,
-"session_timeout": 15, "ris_wsdl_filename": "wsdlRISService70_test.xml", }
-class CucmAxlCustom(CucmSettings): def __init__(self, **kwargs): super
-().__init__(**kwargs) @cucm_logging def axlYourOwnGetMethod(self, **kwargs:
-Union[dict, ...]) -> dict: """ AXL Your Own `Get` or Any Other Method. :param
-kwargs: Required Fields: `kwargs = {"uuid": "uuid"}` or `kwargs = {"name":
-"name"}` :return: """ return self._axl.getCallManager(**kwargs)["return"] if
-__name__ == "__main__": cucm = CucmAxlCustom(**settings) print("Result:",
+from typing import Union from tinyCUCM import CucmClient, cucm_logging BASE_DIR
+= Path(__file__).resolve().parent settings = { "pub_fqdn": "cucm.example.com",
+"pub_version": "11.5", "user_login": "Your-CUCM-Account", "user_password":
+"You%wILL#&neVeR!gUEss", "toolkit_path": BASE_DIR / "axlsqltoolkit",
+"cert_path": BASE_DIR / "cucm.crt", "session_verify": False, "session_timeout":
+15, "ris_wsdl_filename": "wsdlRISService70_test.xml", } class CucmAxlCustom
+(CucmClient): @cucm_logging def axlYourOwnGetMethod(self, **kwargs: Union[dict,
+...]) -> dict: """ AXL Your Own `Get` or Any Other Method. :param kwargs:
+Required Fields: `kwargs = {"uuid": "uuid"}` or `kwargs = {"name": "name"}` :
+return: """ return self._axl.getCallManager(**kwargs)["return"] if __name__ ==
+"__main__": cucm = CucmAxlCustom(**settings) print("Result:",
 cucm.axlYourOwnGetMethod(**{"uuid": "........-....-....-....-............"})) #
 Result: { # 'callManager': { # 'name': 'CM_...', # 'description': '...', #
 'autoRegistration': {...}, # 'ports': {...}, # 'processNodeName': {...}, #
 'lbmGroup': {...}, # 'ctiid': ..., # 'uuid': '
 {........-....-....-....-............}' # } # } ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See `LICENSE` for more
```

### Comparing `tinyCUCM-0.2.6/README.md` & `tinycucm-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,16 @@
     "pub_version": "11.5",
     "user_login": "Your-CUCM-Account",
     "user_password": "You%wILL#&neVeR!gUEss",
     "toolkit_path": BASE_DIR / "axlsqltoolkit",
     "cert_path": BASE_DIR / "cucm.crt",
     "session_verify": False,
     "session_timeout": 15,
-    "ris_wsdl_filename": "wsdlRISService70_test.xml", 
+    "ccs_wsdl_filename": "wsdlControlCenterServices_test.xml",
+    "ris_wsdl_filename": "wsdlRISService70_test.xml",
 }
 
 if __name__ == "__main__":
     cucm = CucmClient(**settings)
     # Get All AXL Method Names
     print("Result:", cucm.axlAllMethods())
     # Result: (
@@ -1863,14 +1864,15 @@
   * `sqlSearchRemoteDestination` - required keywords args: `criterion`, `value`
     * `criterion` enum: `Name`, `Destination`
   * `sqlSearchTranslationPattern` - required keywords args: `criterion`, `value`
     * `criterion` enum: `Pattern`, `Description`, `Partition`, `Calling Search Space`, `Called Party Transform Mask`,
       `Prefix Digits Out` 
 * `Validate` Methods:
   * `sqlValidateDeviceEndUserDesignation` - required keywords args: `device` (Type Class: Any)
+  * `sqlValidateEndUser` - required keywords args: `userid`
   * `sqlValidateLine` - required keywords args: `pattern` (Type Pattern Usage: Device Only)
   * `sqlValidatePattern` - required keywords args: `pattern` (Type Pattern Usage: Any)
 
 </details>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
@@ -1881,15 +1883,15 @@
 
 <details>
 <summary>Code Example:</summary>
 
 ```python
 from pathlib import Path
 from typing import Union
-from tinyCUCM import CucmSettings, cucm_logging
+from tinyCUCM import CucmClient, cucm_logging
 
 
 BASE_DIR = Path(__file__).resolve().parent
 settings = {
     "pub_fqdn": "cucm.example.com",
     "pub_version": "11.5",
     "user_login": "Your-CUCM-Account",
@@ -1898,17 +1900,15 @@
     "cert_path": BASE_DIR / "cucm.crt",
     "session_verify": False,
     "session_timeout": 15,
     "ris_wsdl_filename": "wsdlRISService70_test.xml", 
 }
 
 
-class CucmAxlCustom(CucmSettings):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+class CucmAxlCustom(CucmClient):
         
     @cucm_logging
     def axlYourOwnGetMethod(self, **kwargs: Union[dict, ...]) -> dict:
 
         """
         AXL Your Own `Get` or Any Other Method.
         :param kwargs:      Required Fields:
```

#### html2text {}

```diff
@@ -53,21 +53,21 @@
 object to the local variable `cucm`. **Don't store sensitive information in
 source code. For example use ".env" file.** Code Example: ```python from
 pathlib import Path from tinyCUCM import CucmClient BASE_DIR = Path
 (__file__).resolve().parent settings = { "pub_fqdn": "cucm.example.com",
 "pub_version": "11.5", "user_login": "Your-CUCM-Account", "user_password":
 "You%wILL#&neVeR!gUEss", "toolkit_path": BASE_DIR / "axlsqltoolkit",
 "cert_path": BASE_DIR / "cucm.crt", "session_verify": False, "session_timeout":
-15, "ris_wsdl_filename": "wsdlRISService70_test.xml", } if __name__ ==
-"__main__": cucm = CucmClient(**settings) # Get All AXL Method Names print
-("Result:", cucm.axlAllMethods()) # Result: ( # 'addAarGroup', #
-'addAdvertisedPatterns', # 'addAnnouncement', # 'addAppServerInfo', #
-'addAppUser', # ..., # 'updateWifiHotspot', #
-'updateWirelessAccessPointControllers', # 'updateWlanProfileGroup', #
-'wipePhone' # ) ```
+15, "ccs_wsdl_filename": "wsdlControlCenterServices_test.xml",
+"ris_wsdl_filename": "wsdlRISService70_test.xml", } if __name__ == "__main__":
+cucm = CucmClient(**settings) # Get All AXL Method Names print("Result:",
+cucm.axlAllMethods()) # Result: ( # 'addAarGroup', # 'addAdvertisedPatterns', #
+'addAnnouncement', # 'addAppServerInfo', # 'addAppUser', # ..., #
+'updateWifiHotspot', # 'updateWirelessAccessPointControllers', #
+'updateWlanProfileGroup', # 'wipePhone' # ) ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### AXL Collection #### Add Methods * `axlAddCallPickupGroup` keywords args *
 required: * `callPickupGroup` * `name` * `pattern` * expected: * `description`
 * `routePartitionName` * `members` * `pickupNotification` *
 `pickupNotificationTimer` * `callInfoForPickupNotification` *
 `axlAddDeviceProfile` keywords args * required: * `deviceProfile` * `name` *
 `product` * `class` * `protocol` * `protocolSide` * `phoneTemplateName` *
@@ -571,32 +571,32 @@
 `criterion` enum: `Name`, `Member Line Number`, `Member Line Description` *
 `sqlSearchRemoteDestination` - required keywords args: `criterion`, `value` *
 `criterion` enum: `Name`, `Destination` * `sqlSearchTranslationPattern` -
 required keywords args: `criterion`, `value` * `criterion` enum: `Pattern`,
 `Description`, `Partition`, `Calling Search Space`, `Called Party Transform
 Mask`, `Prefix Digits Out` * `Validate` Methods: *
 `sqlValidateDeviceEndUserDesignation` - required keywords args: `device` (Type
-Class: Any) * `sqlValidateLine` - required keywords args: `pattern` (Type
-Pattern Usage: Device Only) * `sqlValidatePattern` - required keywords args:
-`pattern` (Type Pattern Usage: Any)
+Class: Any) * `sqlValidateEndUser` - required keywords args: `userid` *
+`sqlValidateLine` - required keywords args: `pattern` (Type Pattern Usage:
+Device Only) * `sqlValidatePattern` - required keywords args: `pattern` (Type
+Pattern Usage: Any)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Create Your Own Methods **Don't store sensitive information in source code.
 For example use ".env" file.** Code Example: ```python from pathlib import Path
-from typing import Union from tinyCUCM import CucmSettings, cucm_logging
-BASE_DIR = Path(__file__).resolve().parent settings = { "pub_fqdn":
-"cucm.example.com", "pub_version": "11.5", "user_login": "Your-CUCM-Account",
-"user_password": "You%wILL#&neVeR!gUEss", "toolkit_path": BASE_DIR /
-"axlsqltoolkit", "cert_path": BASE_DIR / "cucm.crt", "session_verify": False,
-"session_timeout": 15, "ris_wsdl_filename": "wsdlRISService70_test.xml", }
-class CucmAxlCustom(CucmSettings): def __init__(self, **kwargs): super
-().__init__(**kwargs) @cucm_logging def axlYourOwnGetMethod(self, **kwargs:
-Union[dict, ...]) -> dict: """ AXL Your Own `Get` or Any Other Method. :param
-kwargs: Required Fields: `kwargs = {"uuid": "uuid"}` or `kwargs = {"name":
-"name"}` :return: """ return self._axl.getCallManager(**kwargs)["return"] if
-__name__ == "__main__": cucm = CucmAxlCustom(**settings) print("Result:",
+from typing import Union from tinyCUCM import CucmClient, cucm_logging BASE_DIR
+= Path(__file__).resolve().parent settings = { "pub_fqdn": "cucm.example.com",
+"pub_version": "11.5", "user_login": "Your-CUCM-Account", "user_password":
+"You%wILL#&neVeR!gUEss", "toolkit_path": BASE_DIR / "axlsqltoolkit",
+"cert_path": BASE_DIR / "cucm.crt", "session_verify": False, "session_timeout":
+15, "ris_wsdl_filename": "wsdlRISService70_test.xml", } class CucmAxlCustom
+(CucmClient): @cucm_logging def axlYourOwnGetMethod(self, **kwargs: Union[dict,
+...]) -> dict: """ AXL Your Own `Get` or Any Other Method. :param kwargs:
+Required Fields: `kwargs = {"uuid": "uuid"}` or `kwargs = {"name": "name"}` :
+return: """ return self._axl.getCallManager(**kwargs)["return"] if __name__ ==
+"__main__": cucm = CucmAxlCustom(**settings) print("Result:",
 cucm.axlYourOwnGetMethod(**{"uuid": "........-....-....-....-............"})) #
 Result: { # 'callManager': { # 'name': 'CM_...', # 'description': '...', #
 'autoRegistration': {...}, # 'ports': {...}, # 'processNodeName': {...}, #
 'lbmGroup': {...}, # 'ctiid': ..., # 'uuid': '
 {........-....-....-....-............}' # } # } ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See `LICENSE` for more
```

### Comparing `tinyCUCM-0.2.6/pyproject.toml` & `tinycucm-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tinyCUCM"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Luarvick", email="lu.luarvick@gmail.com" },
 ]
 description = "Cisco Unified Call Manager AXL Methods Collection."
 readme = "README.md"
 dependencies = [
     "zeep==4.2.1",
```

### Comparing `tinyCUCM-0.2.6/src/tinyCUCM/ccs_models.py` & `tinycucm-0.2.7/src/tinyCUCM/ccs_models.py`

 * *Files identical despite different names*

### Comparing `tinyCUCM-0.2.6/src/tinyCUCM/client.py` & `tinycucm-0.2.7/src/tinyCUCM/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from collections.abc import Iterable
 from typing import Union
 from typing_extensions import Unpack
 from zeep.helpers import serialize_object
 
 from .ccs_models import CucmCcsDoControlModel, CucmCcsDoDeploymentModel
 from .decorators import cucm_logging
@@ -13,14 +14,17 @@
     CucmSqlSearchEndUserModel,
     CucmSqlSearchLineGroupModel,
     CucmSqlSearchRemoteDestinationModel,
     CucmSqlSearchTranslationPatternModel,
 )
 
 
+logger = logging.getLogger("cucm_client")
+
+
 """ ######################################################### """
 """ ******************** TINY CUCM CLIENT ******************* """
 """ ######################################################### """
 
 
 class CucmClient(CucmSettings):
 
@@ -1326,15 +1330,15 @@
         * value: Search Value String
 
         :param kwargs:  Required Fields: `kwargs = {"criterion": "Enum", "value": "str"}`
         :return:
         """
 
         validated_data = CucmSqlSearchCallPickupGroupModel(**kwargs).model_dump()
-        sql_query = """SELECT cpg.pkid AS uuid,
+        sql_query = """SELECT cpg.pkid
                               cpg.name,
                               npg.description,
                               npg.dnorpattern AS pattern,
                               rp.name AS partition,
                               npm.dnorpattern AS line,
                               rpm.name AS line_partition,
                               npm.description AS line_description
@@ -1514,15 +1518,15 @@
                         WHERE LOWER({obj}) LIKE '%{val}%'
                           AND np.tkpatternusage = '3'
                      ORDER BY np.dnorpattern""".format(
             obj=validated_data["criterion"], val=validated_data["value"].lower()
         )
         return self.__cucm_sql_execute(sql_query=sql_query)
 
-    def sqlValidateDeviceEndUserDesignation(self, device: str):
+    def sqlValidateDeviceEndUserDesignation(self, device: str) -> Union[tuple[dict], None]:
 
         """
         SQL Validate Object Method.
         :param device:      Device Name (Any Type Class)
         :return:
         """
 
@@ -1535,14 +1539,31 @@
                               d.tkclass AS device_type
                          FROM enduser eu
                     LEFT JOIN enduserdevicemap eudm ON eudm.fkenduser = eu.pkid
                     LEFT JOIN device d ON eudm.fkdevice = d.pkid
                         WHERE LOWER(d.name) = '{val}'""".format(val=device.lower())
         return self.__cucm_sql_execute(sql_query=sql_query)
 
+    def sqlValidateEndUser(self, userid: str) -> Union[tuple[dict], None]:
+
+        """
+        SQL Validate Object Method.
+        :param userid:      User ID
+        :return:
+        """
+
+        sql_query = """SELECT eu.pkid AS enduser_pkid,
+                              eu.userid,
+                              eu.displayname AS enduser_displayname
+                         FROM enduser eu
+                        WHERE LOWER(eu.userid) = '{val}'
+                          AND eu.status = '1'
+                     ORDER BY eu.userid""".format(val=userid.lower())
+        return self.__cucm_sql_execute(sql_query=sql_query)
+
     def sqlValidateLine(self, pattern: str) -> Union[tuple[dict], None]:
 
         """
         SQL Validate Object Method.
         :param pattern:     Pattern (`tkpatternusage = '2'` - Type Pattern Usage: Device Only)
         :return:
         """
```

### Comparing `tinyCUCM-0.2.6/src/tinyCUCM/decorators.py` & `tinycucm-0.2.7/src/tinyCUCM/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import logging
 from requests.exceptions import ConnectionError, HTTPError, ProxyError, RequestException, Timeout
 from zeep.exceptions import Fault, ValidationError
+
 from .exceptions import (
     CucmAxlSessionError,
     CucmBadRequestError,
     CucmConnectionError,
     CucmUnauthorizedError,
     CucmUnexpectedError
 )
 
 
+logger = logging.getLogger("cucm_client")
+
+
 """ ######################################################### """
 """ ****************** TINY CUCM DECORATORS ***************** """
 """ ######################################################### """
 
 
 def cucm_logging(cucm_method):
 
@@ -22,15 +26,15 @@
     :param cucm_method: CUCM Method
     :return:
     """
 
     def wrapped(self, *args, **kwargs):
 
         """
-        Connection & Methods Log Wrapper
+        Method Wrapper
         :return:
         """
 
         log_message = f"@ CUCM {repr(cucm_method.__name__)} Method @ - {{message}}"
         logging.debug(log_message.format(message=f"Query Params:\nArgs: {args}\nKwargs: {kwargs}."))
 
         try:
@@ -55,28 +59,29 @@
 
         except (Fault, ValidationError) as err:
             history = self._cucm_history_show()
             if "HTTP Status 401" in history:
                 raise CucmUnauthorizedError("Unauthorized error occurred.")
             elif "<axlcode>5003</axlcode>" in history or "<axlcode>5007</axlcode>" in history:
                 # Only for AXL Requests - 404 Not Found
-                # Do or Get Request - AXLCode: <axlcode>5007</axlcode>
-                # ("Item not valid: The specified {{CUCM Object}} was not found")
-                # UpdateRequest - AXLCode: <axlcode>5003</axlcode> ("{{CUCM Object}} not found")
+                # Do or Get Request - AXLCode: 5007 - "Item not valid: The specified {{CUCM Object}} was not found"
+                # UpdateRequest - AXLCode: 5003 - "{{CUCM Object}} not found"
                 logging.warning(log_message.format(message=f"Error Detail:\n{repr(err)}."))
                 return None
             else:
-                # For Invalid SQL Queries. AXLCode: 201 ("A syntax error has occurred")
+                # For Invalid SQL Queries.
+                # AXLCode: 201 - "A syntax error has occurred"
+                # AXLCode: 217 - "Column ({{column_names}}) not found..."
                 logging.error(log_message.format(message=f"Error Detail:\n{repr(err)}."))
                 logging.error(log_message.format(message=f"History:\n{history}."))
-                raise CucmBadRequestError("BadRequest error occurred.")
+                raise CucmBadRequestError(f"BadRequest error occurred. {repr(err)}")
 
         except (ConnectionError, HTTPError, ProxyError, RequestException, Timeout) as err:
             logging.error(log_message.format(message=f"Error Detail:\n{repr(err)}"))
-            raise CucmConnectionError("Connection has been failed.")
+            raise CucmConnectionError(f"Connection has been failed. {repr(err)}")
 
         except Exception as err:
             logging.error(log_message.format(message=f"Error Detail: {repr(err)}."))
             logging.error(log_message.format(message=f"History:\n{self._cucm_history_show()}"))
-            raise CucmUnexpectedError("Unexpected error occurred.")
+            raise CucmUnexpectedError(f"Unexpected error occurred. {repr(err)}")
 
     return wrapped
```

### Comparing `tinyCUCM-0.2.6/src/tinyCUCM/exceptions.py` & `tinycucm-0.2.7/src/tinyCUCM/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinyCUCM-0.2.6/src/tinyCUCM/ris_models.py` & `tinycucm-0.2.7/src/tinyCUCM/ris_models.py`

 * *Files identical despite different names*

### Comparing `tinyCUCM-0.2.6/src/tinyCUCM/settings.py` & `tinycucm-0.2.7/src/tinyCUCM/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
     def __init__(self, **kwargs):
         super(CucmSettings, self).__init__()
 
         disable_warnings(InsecureRequestWarning)
 
         self._axl = None
-        self._axl_client = None
-        self._axl_transport = None
+        self._axl_client = None     # Workaround for CSCvq98025 (axlAddRemoteDestination)
+        self._axl_transport = None  # Workaround for CSCvq98025 (axlAddRemoteDestination)
         self._ccs = None            # Control Center Services
         self._ris = None            # Real-time Information Server
         self._ris_factory = None    # Real-time Information Server
 
         self.__pub_fqdn: str = kwargs.get("pub_fqdn")
         self.__pub_version: str = kwargs.get("pub_version")
         self.__user_login: str = kwargs.get("user_login")
```

### Comparing `tinyCUCM-0.2.6/src/tinyCUCM/sql_models.py` & `tinycucm-0.2.7/src/tinyCUCM/sql_models.py`

 * *Files identical despite different names*

### Comparing `tinyCUCM-0.2.6/src/tinyCUCM.egg-info/PKG-INFO` & `tinycucm-0.2.7/src/tinyCUCM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyCUCM
-Version: 0.2.6
+Version: 0.2.7
 Summary: Cisco Unified Call Manager AXL Methods Collection.
 Author-email: Luarvick <lu.luarvick@gmail.com>
 Project-URL: Homepage, https://github.com/luarvick/tinyCUCM
 Project-URL: Issues, https://github.com/luarvick/tinyCUCM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -126,15 +126,16 @@
     "pub_version": "11.5",
     "user_login": "Your-CUCM-Account",
     "user_password": "You%wILL#&neVeR!gUEss",
     "toolkit_path": BASE_DIR / "axlsqltoolkit",
     "cert_path": BASE_DIR / "cucm.crt",
     "session_verify": False,
     "session_timeout": 15,
-    "ris_wsdl_filename": "wsdlRISService70_test.xml", 
+    "ccs_wsdl_filename": "wsdlControlCenterServices_test.xml",
+    "ris_wsdl_filename": "wsdlRISService70_test.xml",
 }
 
 if __name__ == "__main__":
     cucm = CucmClient(**settings)
     # Get All AXL Method Names
     print("Result:", cucm.axlAllMethods())
     # Result: (
@@ -1879,14 +1880,15 @@
   * `sqlSearchRemoteDestination` - required keywords args: `criterion`, `value`
     * `criterion` enum: `Name`, `Destination`
   * `sqlSearchTranslationPattern` - required keywords args: `criterion`, `value`
     * `criterion` enum: `Pattern`, `Description`, `Partition`, `Calling Search Space`, `Called Party Transform Mask`,
       `Prefix Digits Out` 
 * `Validate` Methods:
   * `sqlValidateDeviceEndUserDesignation` - required keywords args: `device` (Type Class: Any)
+  * `sqlValidateEndUser` - required keywords args: `userid`
   * `sqlValidateLine` - required keywords args: `pattern` (Type Pattern Usage: Device Only)
   * `sqlValidatePattern` - required keywords args: `pattern` (Type Pattern Usage: Any)
 
 </details>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
@@ -1897,15 +1899,15 @@
 
 <details>
 <summary>Code Example:</summary>
 
 ```python
 from pathlib import Path
 from typing import Union
-from tinyCUCM import CucmSettings, cucm_logging
+from tinyCUCM import CucmClient, cucm_logging
 
 
 BASE_DIR = Path(__file__).resolve().parent
 settings = {
     "pub_fqdn": "cucm.example.com",
     "pub_version": "11.5",
     "user_login": "Your-CUCM-Account",
@@ -1914,17 +1916,15 @@
     "cert_path": BASE_DIR / "cucm.crt",
     "session_verify": False,
     "session_timeout": 15,
     "ris_wsdl_filename": "wsdlRISService70_test.xml", 
 }
 
 
-class CucmAxlCustom(CucmSettings):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+class CucmAxlCustom(CucmClient):
         
     @cucm_logging
     def axlYourOwnGetMethod(self, **kwargs: Union[dict, ...]) -> dict:
 
         """
         AXL Your Own `Get` or Any Other Method.
         :param kwargs:      Required Fields:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyCUCM Version: 0.2.6 Summary: Cisco Unified Call
+Metadata-Version: 2.1 Name: tinyCUCM Version: 0.2.7 Summary: Cisco Unified Call
 Manager AXL Methods Collection. Author-email: Luarvick
 gmail.com> Project-URL: Homepage, https://github.com/luarvick/tinyCUCM Project-
 URL: Issues, https://github.com/luarvick/tinyCUCM/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 zeep==4.2.1 Requires-Dist: pydantic==2.6.3
@@ -60,21 +60,21 @@
 object to the local variable `cucm`. **Don't store sensitive information in
 source code. For example use ".env" file.** Code Example: ```python from
 pathlib import Path from tinyCUCM import CucmClient BASE_DIR = Path
 (__file__).resolve().parent settings = { "pub_fqdn": "cucm.example.com",
 "pub_version": "11.5", "user_login": "Your-CUCM-Account", "user_password":
 "You%wILL#&neVeR!gUEss", "toolkit_path": BASE_DIR / "axlsqltoolkit",
 "cert_path": BASE_DIR / "cucm.crt", "session_verify": False, "session_timeout":
-15, "ris_wsdl_filename": "wsdlRISService70_test.xml", } if __name__ ==
-"__main__": cucm = CucmClient(**settings) # Get All AXL Method Names print
-("Result:", cucm.axlAllMethods()) # Result: ( # 'addAarGroup', #
-'addAdvertisedPatterns', # 'addAnnouncement', # 'addAppServerInfo', #
-'addAppUser', # ..., # 'updateWifiHotspot', #
-'updateWirelessAccessPointControllers', # 'updateWlanProfileGroup', #
-'wipePhone' # ) ```
+15, "ccs_wsdl_filename": "wsdlControlCenterServices_test.xml",
+"ris_wsdl_filename": "wsdlRISService70_test.xml", } if __name__ == "__main__":
+cucm = CucmClient(**settings) # Get All AXL Method Names print("Result:",
+cucm.axlAllMethods()) # Result: ( # 'addAarGroup', # 'addAdvertisedPatterns', #
+'addAnnouncement', # 'addAppServerInfo', # 'addAppUser', # ..., #
+'updateWifiHotspot', # 'updateWirelessAccessPointControllers', #
+'updateWlanProfileGroup', # 'wipePhone' # ) ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### AXL Collection #### Add Methods * `axlAddCallPickupGroup` keywords args *
 required: * `callPickupGroup` * `name` * `pattern` * expected: * `description`
 * `routePartitionName` * `members` * `pickupNotification` *
 `pickupNotificationTimer` * `callInfoForPickupNotification` *
 `axlAddDeviceProfile` keywords args * required: * `deviceProfile` * `name` *
 `product` * `class` * `protocol` * `protocolSide` * `phoneTemplateName` *
@@ -578,32 +578,32 @@
 `criterion` enum: `Name`, `Member Line Number`, `Member Line Description` *
 `sqlSearchRemoteDestination` - required keywords args: `criterion`, `value` *
 `criterion` enum: `Name`, `Destination` * `sqlSearchTranslationPattern` -
 required keywords args: `criterion`, `value` * `criterion` enum: `Pattern`,
 `Description`, `Partition`, `Calling Search Space`, `Called Party Transform
 Mask`, `Prefix Digits Out` * `Validate` Methods: *
 `sqlValidateDeviceEndUserDesignation` - required keywords args: `device` (Type
-Class: Any) * `sqlValidateLine` - required keywords args: `pattern` (Type
-Pattern Usage: Device Only) * `sqlValidatePattern` - required keywords args:
-`pattern` (Type Pattern Usage: Any)
+Class: Any) * `sqlValidateEndUser` - required keywords args: `userid` *
+`sqlValidateLine` - required keywords args: `pattern` (Type Pattern Usage:
+Device Only) * `sqlValidatePattern` - required keywords args: `pattern` (Type
+Pattern Usage: Any)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Create Your Own Methods **Don't store sensitive information in source code.
 For example use ".env" file.** Code Example: ```python from pathlib import Path
-from typing import Union from tinyCUCM import CucmSettings, cucm_logging
-BASE_DIR = Path(__file__).resolve().parent settings = { "pub_fqdn":
-"cucm.example.com", "pub_version": "11.5", "user_login": "Your-CUCM-Account",
-"user_password": "You%wILL#&neVeR!gUEss", "toolkit_path": BASE_DIR /
-"axlsqltoolkit", "cert_path": BASE_DIR / "cucm.crt", "session_verify": False,
-"session_timeout": 15, "ris_wsdl_filename": "wsdlRISService70_test.xml", }
-class CucmAxlCustom(CucmSettings): def __init__(self, **kwargs): super
-().__init__(**kwargs) @cucm_logging def axlYourOwnGetMethod(self, **kwargs:
-Union[dict, ...]) -> dict: """ AXL Your Own `Get` or Any Other Method. :param
-kwargs: Required Fields: `kwargs = {"uuid": "uuid"}` or `kwargs = {"name":
-"name"}` :return: """ return self._axl.getCallManager(**kwargs)["return"] if
-__name__ == "__main__": cucm = CucmAxlCustom(**settings) print("Result:",
+from typing import Union from tinyCUCM import CucmClient, cucm_logging BASE_DIR
+= Path(__file__).resolve().parent settings = { "pub_fqdn": "cucm.example.com",
+"pub_version": "11.5", "user_login": "Your-CUCM-Account", "user_password":
+"You%wILL#&neVeR!gUEss", "toolkit_path": BASE_DIR / "axlsqltoolkit",
+"cert_path": BASE_DIR / "cucm.crt", "session_verify": False, "session_timeout":
+15, "ris_wsdl_filename": "wsdlRISService70_test.xml", } class CucmAxlCustom
+(CucmClient): @cucm_logging def axlYourOwnGetMethod(self, **kwargs: Union[dict,
+...]) -> dict: """ AXL Your Own `Get` or Any Other Method. :param kwargs:
+Required Fields: `kwargs = {"uuid": "uuid"}` or `kwargs = {"name": "name"}` :
+return: """ return self._axl.getCallManager(**kwargs)["return"] if __name__ ==
+"__main__": cucm = CucmAxlCustom(**settings) print("Result:",
 cucm.axlYourOwnGetMethod(**{"uuid": "........-....-....-....-............"})) #
 Result: { # 'callManager': { # 'name': 'CM_...', # 'description': '...', #
 'autoRegistration': {...}, # 'ports': {...}, # 'processNodeName': {...}, #
 'lbmGroup': {...}, # 'ctiid': ..., # 'uuid': '
 {........-....-....-....-............}' # } # } ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See `LICENSE` for more
```

