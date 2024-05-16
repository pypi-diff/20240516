# Comparing `tmp/seam-0.6.2.tar.gz` & `tmp/seam-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seam-0.6.2.tar", max compression
+gzip compressed data, was "seam-0.7.0.tar", max compression
```

## Comparing `seam-0.6.2.tar` & `seam-0.7.0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0     1087 2024-05-10 09:14:05.311275 seam-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     9355 2024-05-10 09:14:05.311275 seam-0.6.2/README.rst
--rw-r--r--   0        0        0      726 2024-05-10 09:14:05.311275 seam-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      323 2024-05-10 09:14:05.311275 seam-0.6.2/seam/__init__.py
--rw-r--r--   0        0        0    11938 2024-05-10 09:14:05.311275 seam-0.6.2/seam/access_codes.py
--rw-r--r--   0        0        0      903 2024-05-10 09:14:05.311275 seam-0.6.2/seam/access_codes_simulate.py
--rw-r--r--   0        0        0     3979 2024-05-10 09:14:05.311275 seam-0.6.2/seam/access_codes_unmanaged.py
--rw-r--r--   0        0        0     1746 2024-05-10 09:14:05.311275 seam-0.6.2/seam/acs.py
--rw-r--r--   0        0        0     2505 2024-05-10 09:14:05.311275 seam-0.6.2/seam/acs_access_groups.py
--rw-r--r--   0        0        0      718 2024-05-10 09:14:05.311275 seam-0.6.2/seam/acs_credential_pools.py
--rw-r--r--   0        0        0     1782 2024-05-10 09:14:05.311275 seam-0.6.2/seam/acs_credential_provisioning_automations.py
--rw-r--r--   0        0        0     4763 2024-05-10 09:14:05.311275 seam-0.6.2/seam/acs_credentials.py
--rw-r--r--   0        0        0     2172 2024-05-10 09:14:05.311275 seam-0.6.2/seam/acs_entrances.py
--rw-r--r--   0        0        0      955 2024-05-10 09:14:05.311275 seam-0.6.2/seam/acs_systems.py
--rw-r--r--   0        0        0     6476 2024-05-10 09:14:05.311275 seam-0.6.2/seam/acs_users.py
--rw-r--r--   0        0        0     3255 2024-05-10 09:14:05.311275 seam-0.6.2/seam/action_attempts.py
--rw-r--r--   0        0        0     3156 2024-05-10 09:14:05.311275 seam-0.6.2/seam/auth.py
--rw-r--r--   0        0        0     5751 2024-05-10 09:14:05.311275 seam-0.6.2/seam/client_sessions.py
--rw-r--r--   0        0        0     3292 2024-05-10 09:14:05.311275 seam-0.6.2/seam/connect_webviews.py
--rw-r--r--   0        0        0     2520 2024-05-10 09:14:05.311275 seam-0.6.2/seam/connected_accounts.py
--rw-r--r--   0        0        0     4761 2024-05-10 09:14:05.311275 seam-0.6.2/seam/devices.py
--rw-r--r--   0        0        0      517 2024-05-10 09:14:05.311275 seam-0.6.2/seam/devices_simulate.py
--rw-r--r--   0        0        0     3323 2024-05-10 09:14:05.311275 seam-0.6.2/seam/devices_unmanaged.py
--rw-r--r--   0        0        0     2385 2024-05-10 09:14:05.315275 seam-0.6.2/seam/events.py
--rw-r--r--   0        0        0     4181 2024-05-10 09:14:05.315275 seam-0.6.2/seam/locks.py
--rw-r--r--   0        0        0      765 2024-05-10 09:14:05.315275 seam-0.6.2/seam/networks.py
--rw-r--r--   0        0        0      714 2024-05-10 09:14:05.315275 seam-0.6.2/seam/noise_sensors.py
--rw-r--r--   0        0        0     4350 2024-05-10 09:14:05.315275 seam-0.6.2/seam/noise_sensors_noise_thresholds.py
--rw-r--r--   0        0        0      594 2024-05-10 09:14:05.315275 seam-0.6.2/seam/noise_sensors_simulate.py
--rw-r--r--   0        0        0     1854 2024-05-10 09:14:05.315275 seam-0.6.2/seam/options.py
--rw-r--r--   0        0        0      715 2024-05-10 09:14:05.315275 seam-0.6.2/seam/parse_options.py
--rw-r--r--   0        0        0     1063 2024-05-10 09:14:05.315275 seam-0.6.2/seam/phones.py
--rw-r--r--   0        0        0     1185 2024-05-10 09:14:05.315275 seam-0.6.2/seam/phones_simulate.py
--rw-r--r--   0        0        0     1436 2024-05-10 09:14:05.315275 seam-0.6.2/seam/routes.py
--rw-r--r--   0        0        0     3614 2024-05-10 09:14:05.315275 seam-0.6.2/seam/seam.py
--rw-r--r--   0        0        0     8926 2024-05-10 09:14:05.315275 seam-0.6.2/seam/thermostats.py
--rw-r--r--   0        0        0     6930 2024-05-10 09:14:05.315275 seam-0.6.2/seam/thermostats_climate_setting_schedules.py
--rw-r--r--   0        0        0     1027 2024-05-10 09:14:05.315275 seam-0.6.2/seam/token.py
--rw-r--r--   0        0        0    66038 2024-05-10 09:14:05.315275 seam-0.6.2/seam/types.py
--rw-r--r--   0        0        0     6700 2024-05-10 09:14:05.315275 seam-0.6.2/seam/user_identities.py
--rw-r--r--   0        0        0     2903 2024-05-10 09:14:05.315275 seam-0.6.2/seam/user_identities_enrollment_automations.py
--rw-r--r--   0        0        0      851 2024-05-10 09:14:05.315275 seam-0.6.2/seam/utils/action_attempt_errors.py
--rw-r--r--   0        0        0      864 2024-05-10 09:14:05.315275 seam-0.6.2/seam/utils/deep_attr_dict.py
--rw-r--r--   0        0        0     1815 2024-05-10 09:14:05.315275 seam-0.6.2/seam/webhooks.py
--rw-r--r--   0        0        0     2174 2024-05-10 09:14:05.315275 seam-0.6.2/seam/workspaces.py
--rw-r--r--   0        0        0    10105 1970-01-01 00:00:00.000000 seam-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-16 15:45:20.934088 seam-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     9355 2024-05-16 15:45:20.938088 seam-0.7.0/README.rst
+-rw-r--r--   0        0        0      726 2024-05-16 15:45:20.938088 seam-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      397 2024-05-16 15:45:20.938088 seam-0.7.0/seam/__init__.py
+-rw-r--r--   0        0        0     4076 2024-05-16 15:45:20.938088 seam-0.7.0/seam/auth.py
+-rw-r--r--   0        0        0       72 2024-05-16 15:45:20.938088 seam-0.7.0/seam/constants.py
+-rw-r--r--   0        0        0     2018 2024-05-16 15:45:20.938088 seam-0.7.0/seam/options.py
+-rw-r--r--   0        0        0      623 2024-05-16 15:45:20.938088 seam-0.7.0/seam/parse_options.py
+-rw-r--r--   0        0        0     1337 2024-05-16 15:45:20.938088 seam-0.7.0/seam/request.py
+-rw-r--r--   0        0        0    11981 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/access_codes.py
+-rw-r--r--   0        0        0      915 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/access_codes_simulate.py
+-rw-r--r--   0        0        0     3991 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/access_codes_unmanaged.py
+-rw-r--r--   0        0        0     1824 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs.py
+-rw-r--r--   0        0        0     2513 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_access_groups.py
+-rw-r--r--   0        0        0      730 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_credential_pools.py
+-rw-r--r--   0        0        0     1807 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_credential_provisioning_automations.py
+-rw-r--r--   0        0        0     4964 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_credentials.py
+-rw-r--r--   0        0        0     2180 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_entrances.py
+-rw-r--r--   0        0        0     1476 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_systems.py
+-rw-r--r--   0        0        0     6505 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_users.py
+-rw-r--r--   0        0        0     3982 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/action_attempts.py
+-rw-r--r--   0        0        0     5780 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/client_sessions.py
+-rw-r--r--   0        0        0     3321 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/connect_webviews.py
+-rw-r--r--   0        0        0     2549 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/connected_accounts.py
+-rw-r--r--   0        0        0     4804 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/devices.py
+-rw-r--r--   0        0        0      546 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/devices_simulate.py
+-rw-r--r--   0        0        0     3352 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/devices_unmanaged.py
+-rw-r--r--   0        0        0     2414 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/events.py
+-rw-r--r--   0        0        0     4210 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/locks.py
+-rw-r--r--   0        0        0      794 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/networks.py
+-rw-r--r--   0        0        0      757 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/noise_sensors.py
+-rw-r--r--   0        0        0     4362 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/noise_sensors_noise_thresholds.py
+-rw-r--r--   0        0        0      623 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/noise_sensors_simulate.py
+-rw-r--r--   0        0        0     1099 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/phones.py
+-rw-r--r--   0        0        0     1214 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/phones_simulate.py
+-rw-r--r--   0        0        0     1436 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/routes.py
+-rw-r--r--   0        0        0     8962 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/thermostats.py
+-rw-r--r--   0        0        0     6955 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/thermostats_climate_setting_schedules.py
+-rw-r--r--   0        0        0    64963 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/types.py
+-rw-r--r--   0        0        0     6732 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/user_identities.py
+-rw-r--r--   0        0        0     2928 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/user_identities_enrollment_automations.py
+-rw-r--r--   0        0        0      864 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0     1844 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/webhooks.py
+-rw-r--r--   0        0        0     2182 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/workspaces.py
+-rw-r--r--   0        0        0     2555 2024-05-16 15:45:20.938088 seam-0.7.0/seam/seam.py
+-rw-r--r--   0        0        0     2418 2024-05-16 15:45:20.938088 seam-0.7.0/seam/seam_multi_workspace.py
+-rw-r--r--   0        0        0     1027 2024-05-16 15:45:20.938088 seam-0.7.0/seam/token.py
+-rw-r--r--   0        0        0     3242 2024-05-16 15:45:20.938088 seam-0.7.0/seam/types.py
+-rw-r--r--   0        0        0    10105 1970-01-01 00:00:00.000000 seam-0.7.0/PKG-INFO
```

### Comparing `seam-0.6.2/LICENSE.txt` & `seam-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seam-0.6.2/README.rst` & `seam-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `seam-0.6.2/pyproject.toml` & `seam-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seam"
-version = "0.6.2"
+version = "0.7.0"
 description = "SDK for the Seam API written in Python."
 authors = ["Seam Labs, Inc. <engineering@getseam.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/seamapi/python-next"
 repository = "https://github.com/seamapi/python-next"
```

### Comparing `seam-0.6.2/seam/access_codes.py` & `seam-0.7.0/seam/routes/access_codes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from seam.types import AbstractAccessCodes, AbstractSeam as Seam, AccessCode
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAccessCodes, AccessCode
 from typing import Optional, Any, List, Dict, Union
-from seam.access_codes_simulate import AccessCodesSimulate
-from seam.access_codes_unmanaged import AccessCodesUnmanaged
+from seam.routes.access_codes_simulate import AccessCodesSimulate
+from seam.routes.access_codes_unmanaged import AccessCodesUnmanaged
 
 
 class AccessCodes(AbstractAccessCodes):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
```

### Comparing `seam-0.6.2/seam/access_codes_simulate.py` & `seam-0.7.0/seam/routes/access_codes_simulate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from seam.types import (
-    AbstractAccessCodesSimulate,
-    AbstractSeam as Seam,
-    UnmanagedAccessCode,
-)
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAccessCodesSimulate, UnmanagedAccessCode
 from typing import Optional, Any, List, Dict, Union
 
 
 class AccessCodesSimulate(AbstractAccessCodesSimulate):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/access_codes_unmanaged.py` & `seam-0.7.0/seam/routes/access_codes_unmanaged.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from seam.types import (
-    AbstractAccessCodesUnmanaged,
-    AbstractSeam as Seam,
-    UnmanagedAccessCode,
-)
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAccessCodesUnmanaged, UnmanagedAccessCode
 from typing import Optional, Any, List, Dict, Union
 
 
 class AccessCodesUnmanaged(AbstractAccessCodesUnmanaged):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/acs.py` & `seam-0.7.0/seam/routes/acs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from seam.types import AbstractAcs, AbstractSeam as Seam
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAcs
 from typing import Optional, Any, List, Dict, Union
-from seam.acs_access_groups import AcsAccessGroups
-from seam.acs_credential_pools import AcsCredentialPools
-from seam.acs_credential_provisioning_automations import (
+from seam.routes.acs_access_groups import AcsAccessGroups
+from seam.routes.acs_credential_pools import AcsCredentialPools
+from seam.routes.acs_credential_provisioning_automations import (
     AcsCredentialProvisioningAutomations,
 )
-from seam.acs_credentials import AcsCredentials
-from seam.acs_entrances import AcsEntrances
-from seam.acs_systems import AcsSystems
-from seam.acs_users import AcsUsers
+from seam.routes.acs_credentials import AcsCredentials
+from seam.routes.acs_entrances import AcsEntrances
+from seam.routes.acs_systems import AcsSystems
+from seam.routes.acs_users import AcsUsers
 
 
 class Acs(AbstractAcs):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
```

### Comparing `seam-0.6.2/seam/acs_access_groups.py` & `seam-0.7.0/seam/routes/acs_access_groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from seam.types import (
-    AbstractAcsAccessGroups,
-    AbstractSeam as Seam,
-    AcsAccessGroup,
-    AcsUser,
-)
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAcsAccessGroups, AcsAccessGroup, AcsUser
 from typing import Optional, Any, List, Dict, Union
 
 
 class AcsAccessGroups(AbstractAcsAccessGroups):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/acs_credential_pools.py` & `seam-0.7.0/seam/routes/acs_credential_pools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from seam.types import (
-    AbstractAcsCredentialPools,
-    AbstractSeam as Seam,
-    AcsCredentialPool,
-)
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAcsCredentialPools, AcsCredentialPool
 from typing import Optional, Any, List, Dict, Union
 
 
 class AcsCredentialPools(AbstractAcsCredentialPools):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/acs_credential_provisioning_automations.py` & `seam-0.7.0/seam/routes/acs_credential_provisioning_automations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from seam.types import (
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import (
     AbstractAcsCredentialProvisioningAutomations,
-    AbstractSeam as Seam,
     AcsCredentialProvisioningAutomation,
 )
 from typing import Optional, Any, List, Dict, Union
 
 
 class AcsCredentialProvisioningAutomations(
     AbstractAcsCredentialProvisioningAutomations
```

### Comparing `seam-0.6.2/seam/acs_credentials.py` & `seam-0.7.0/seam/routes/acs_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractAcsCredentials, AbstractSeam as Seam, AcsCredential
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAcsCredentials, AcsCredential
 from typing import Optional, Any, List, Dict, Union
 
 
 class AcsCredentials(AbstractAcsCredentials):
     seam: Seam
 
     def __init__(self, seam: Seam):
@@ -117,18 +118,26 @@
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
         self.seam.make_request("POST", "/acs/credentials/unassign", json=json_payload)
 
         return None
 
-    def update(self, *, acs_credential_id: str, code: str) -> None:
+    def update(
+        self,
+        *,
+        acs_credential_id: str,
+        code: Optional[str] = None,
+        ends_at: Optional[str] = None
+    ) -> None:
         json_payload = {}
 
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
         if code is not None:
             json_payload["code"] = code
+        if ends_at is not None:
+            json_payload["ends_at"] = ends_at
 
         self.seam.make_request("POST", "/acs/credentials/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.6.2/seam/acs_entrances.py` & `seam-0.7.0/seam/routes/acs_entrances.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from seam.types import (
-    AbstractAcsEntrances,
-    AbstractSeam as Seam,
-    AcsEntrance,
-    AcsCredential,
-)
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAcsEntrances, AcsEntrance, AcsCredential
 from typing import Optional, Any, List, Dict, Union
 
 
 class AcsEntrances(AbstractAcsEntrances):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/acs_systems.py` & `seam-0.7.0/seam/routes/acs_systems.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractAcsSystems, AbstractSeam as Seam, AcsSystem
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAcsSystems, AcsSystem
 from typing import Optional, Any, List, Dict, Union
 
 
 class AcsSystems(AbstractAcsSystems):
     seam: Seam
 
     def __init__(self, seam: Seam):
@@ -23,7 +24,23 @@
 
         if connected_account_id is not None:
             json_payload["connected_account_id"] = connected_account_id
 
         res = self.seam.make_request("POST", "/acs/systems/list", json=json_payload)
 
         return [AcsSystem.from_dict(item) for item in res["acs_systems"]]
+
+    def list_compatible_credential_manager_acs_systems(
+        self, *, acs_system_id: str
+    ) -> List[AcsSystem]:
+        json_payload = {}
+
+        if acs_system_id is not None:
+            json_payload["acs_system_id"] = acs_system_id
+
+        res = self.seam.make_request(
+            "POST",
+            "/acs/systems/list_compatible_credential_manager_acs_systems",
+            json=json_payload,
+        )
+
+        return [AcsSystem.from_dict(item) for item in res["acs_systems"]]
```

### Comparing `seam-0.6.2/seam/acs_users.py` & `seam-0.7.0/seam/routes/acs_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractAcsUsers, AbstractSeam as Seam, AcsUser, AcsEntrance
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractAcsUsers, AcsUser, AcsEntrance
 from typing import Optional, Any, List, Dict, Union
 
 
 class AcsUsers(AbstractAcsUsers):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/action_attempts.py` & `seam-0.7.0/seam/routes/action_attempts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,46 @@
-from seam.types import AbstractActionAttempts, AbstractSeam as Seam, ActionAttempt
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractActionAttempts, ActionAttempt
 from typing import Optional, Any, List, Dict, Union
 
 import time
 
-from seam.utils.action_attempt_errors import (
-    SeamActionAttemptFailedError,
-    SeamActionAttemptTimeoutError,
-)
+
+class SeamActionAttemptError(Exception):
+    def __init__(self, message: str, action_attempt: ActionAttempt):
+        super().__init__(message)
+        self.name = self.__class__.__name__
+        self.action_attempt = action_attempt
+
+
+class SeamActionAttemptFailedError(SeamActionAttemptError):
+    def __init__(self, action_attempt: ActionAttempt):
+        super().__init__(action_attempt.error.message, action_attempt)
+        self.name = self.__class__.__name__
+        self.code = action_attempt.error.type
+
+
+class SeamActionAttemptTimeoutError(SeamActionAttemptError):
+    def __init__(self, action_attempt: ActionAttempt, timeout: str):
+        message = f"Timed out waiting for action attempt after {timeout}s"
+        super().__init__(message, action_attempt)
+        self.name = self.__class__.__name__
 
 
 class ActionAttempts(AbstractActionAttempts):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def get(
         self,
         *,
         action_attempt_id: str,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
     ) -> ActionAttempt:
         json_payload = {}
 
         if action_attempt_id is not None:
             json_payload["action_attempt_id"] = action_attempt_id
 
         res = self.seam.make_request("POST", "/action_attempts/get", json=json_payload)
@@ -44,15 +61,15 @@
         return [ActionAttempt.from_dict(item) for item in res["action_attempts"]]
 
     def poll_until_ready(
         self,
         *,
         action_attempt_id: str,
         timeout: Optional[float] = 5.0,
-        polling_interval: Optional[float] = 0.5
+        polling_interval: Optional[float] = 0.5,
     ) -> ActionAttempt:
         seam = self.seam
         time_waiting = 0.0
 
         action_attempt = seam.action_attempts.get(
             action_attempt_id=action_attempt_id, wait_for_action_attempt=False
         )
@@ -74,15 +91,15 @@
 
         return action_attempt
 
     def decide_and_wait(
         self,
         *,
         action_attempt: ActionAttempt,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
     ) -> ActionAttempt:
         wait_decision = (
             self.seam.wait_for_action_attempt
             if wait_for_action_attempt is None
             else wait_for_action_attempt
         )
```

### Comparing `seam-0.6.2/seam/auth.py` & `seam-0.7.0/seam/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -95,7 +95,35 @@
             f"Unknown or invalid personal_access_token format, expected token to start with {ACCESS_TOKEN_PREFIX}"
         )
 
     return {
         "authorization": f"Bearer {personal_access_token}",
         "seam-workspace": workspace_id,
     }
+
+
+def get_auth_headers_for_multi_workspace_personal_access_token(
+    personal_access_token: str,
+) -> dict:
+    if is_jwt(personal_access_token):
+        raise SeamHttpInvalidTokenError(
+            "A JWT cannot be used as a personal_access_token"
+        )
+
+    if is_client_session_token(personal_access_token):
+        raise SeamHttpInvalidTokenError(
+            "A Client Session Token cannot be used as a personal_access_token"
+        )
+
+    if is_publishable_key(personal_access_token):
+        raise SeamHttpInvalidTokenError(
+            "A Publishable Key cannot be used as a personal_access_token"
+        )
+
+    if not is_access_token(personal_access_token):
+        raise SeamHttpInvalidTokenError(
+            f"Unknown or invalid personal_access_token format, expected token to start with {ACCESS_TOKEN_PREFIX}"
+        )
+
+    return {
+        "authorization": f"Bearer {personal_access_token}",
+    }
```

### Comparing `seam-0.6.2/seam/client_sessions.py` & `seam-0.7.0/seam/routes/client_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractClientSessions, AbstractSeam as Seam, ClientSession
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractClientSessions, ClientSession
 from typing import Optional, Any, List, Dict, Union
 
 
 class ClientSessions(AbstractClientSessions):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/connect_webviews.py` & `seam-0.7.0/seam/routes/connect_webviews.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractConnectWebviews, AbstractSeam as Seam, ConnectWebview
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractConnectWebviews, ConnectWebview
 from typing import Optional, Any, List, Dict, Union
 
 
 class ConnectWebviews(AbstractConnectWebviews):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/connected_accounts.py` & `seam-0.7.0/seam/routes/connected_accounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractConnectedAccounts, AbstractSeam as Seam, ConnectedAccount
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractConnectedAccounts, ConnectedAccount
 from typing import Optional, Any, List, Dict, Union
 
 
 class ConnectedAccounts(AbstractConnectedAccounts):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/devices.py` & `seam-0.7.0/seam/routes/devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from seam.types import AbstractDevices, AbstractSeam as Seam, Device, DeviceProvider
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractDevices, Device, DeviceProvider
 from typing import Optional, Any, List, Dict, Union
-from seam.devices_simulate import DevicesSimulate
-from seam.devices_unmanaged import DevicesUnmanaged
+from seam.routes.devices_simulate import DevicesSimulate
+from seam.routes.devices_unmanaged import DevicesUnmanaged
 
 
 class Devices(AbstractDevices):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
```

### Comparing `seam-0.6.2/seam/devices_simulate.py` & `seam-0.7.0/seam/routes/noise_sensors_simulate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from seam.types import AbstractDevicesSimulate, AbstractSeam as Seam
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractNoiseSensorsSimulate
 from typing import Optional, Any, List, Dict, Union
 
 
-class DevicesSimulate(AbstractDevicesSimulate):
+class NoiseSensorsSimulate(AbstractNoiseSensorsSimulate):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
-    def remove(self, *, device_id: str) -> None:
+    def trigger_noise_threshold(self, *, device_id: str) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        self.seam.make_request("POST", "/devices/simulate/remove", json=json_payload)
+        self.seam.make_request(
+            "POST", "/noise_sensors/simulate/trigger_noise_threshold", json=json_payload
+        )
 
         return None
```

### Comparing `seam-0.6.2/seam/devices_unmanaged.py` & `seam-0.7.0/seam/routes/devices_unmanaged.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractDevicesUnmanaged, AbstractSeam as Seam, UnmanagedDevice
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractDevicesUnmanaged, UnmanagedDevice
 from typing import Optional, Any, List, Dict, Union
 
 
 class DevicesUnmanaged(AbstractDevicesUnmanaged):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/events.py` & `seam-0.7.0/seam/routes/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractEvents, AbstractSeam as Seam, Event
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractEvents, Event
 from typing import Optional, Any, List, Dict, Union
 
 
 class Events(AbstractEvents):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/locks.py` & `seam-0.7.0/seam/routes/locks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractLocks, AbstractSeam as Seam, Device, ActionAttempt
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractLocks, Device, ActionAttempt
 from typing import Optional, Any, List, Dict, Union
 
 
 class Locks(AbstractLocks):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/networks.py` & `seam-0.7.0/seam/routes/networks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractNetworks, AbstractSeam as Seam, Network
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractNetworks, Network
 from typing import Optional, Any, List, Dict, Union
 
 
 class Networks(AbstractNetworks):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/noise_sensors.py` & `seam-0.7.0/seam/routes/noise_sensors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from seam.types import AbstractNoiseSensors, AbstractSeam as Seam
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractNoiseSensors
 from typing import Optional, Any, List, Dict, Union
-from seam.noise_sensors_noise_thresholds import NoiseSensorsNoiseThresholds
-from seam.noise_sensors_simulate import NoiseSensorsSimulate
+from seam.routes.noise_sensors_noise_thresholds import NoiseSensorsNoiseThresholds
+from seam.routes.noise_sensors_simulate import NoiseSensorsSimulate
 
 
 class NoiseSensors(AbstractNoiseSensors):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
```

### Comparing `seam-0.6.2/seam/noise_sensors_noise_thresholds.py` & `seam-0.7.0/seam/routes/noise_sensors_noise_thresholds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from seam.types import (
-    AbstractNoiseSensorsNoiseThresholds,
-    AbstractSeam as Seam,
-    NoiseThreshold,
-)
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractNoiseSensorsNoiseThresholds, NoiseThreshold
 from typing import Optional, Any, List, Dict, Union
 
 
 class NoiseSensorsNoiseThresholds(AbstractNoiseSensorsNoiseThresholds):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/noise_sensors_simulate.py` & `seam-0.7.0/seam/routes/devices_simulate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from seam.types import AbstractNoiseSensorsSimulate, AbstractSeam as Seam
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractDevicesSimulate
 from typing import Optional, Any, List, Dict, Union
 
 
-class NoiseSensorsSimulate(AbstractNoiseSensorsSimulate):
+class DevicesSimulate(AbstractDevicesSimulate):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
-    def trigger_noise_threshold(self, *, device_id: str) -> None:
+    def remove(self, *, device_id: str) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        self.seam.make_request(
-            "POST", "/noise_sensors/simulate/trigger_noise_threshold", json=json_payload
-        )
+        self.seam.make_request("POST", "/devices/simulate/remove", json=json_payload)
 
         return None
```

### Comparing `seam-0.6.2/seam/options.py` & `seam-0.7.0/seam/options.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import os
 from typing import Optional
 
+from seam.constants import DEFAULT_ENDPOINT
+
+
+def get_endpoint(endpoint: Optional[str] = None):
+    return endpoint or get_endpoint_from_env() or DEFAULT_ENDPOINT
+
 
 def get_endpoint_from_env():
     seam_api_url = os.getenv("SEAM_API_URL")
     seam_endpoint = os.getenv("SEAM_ENDPOINT")
 
     if seam_api_url is not None:
         print(
```

### Comparing `seam-0.6.2/seam/parse_options.py` & `seam-0.7.0/seam/parse_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 from typing import Optional
 
 from seam.auth import get_auth_headers
-from seam.options import get_endpoint_from_env
-
-DEFAULT_ENDPOINT = "https://connect.getseam.com"
+from seam.options import get_endpoint
 
 
 def parse_options(
     api_key: Optional[str] = None,
     personal_access_token: Optional[str] = None,
     workspace_id: Optional[str] = None,
     endpoint: Optional[str] = None,
@@ -17,10 +15,10 @@
         api_key = api_key or os.getenv("SEAM_API_KEY")
 
     auth_headers = get_auth_headers(
         api_key=api_key,
         personal_access_token=personal_access_token,
         workspace_id=workspace_id,
     )
-    endpoint = endpoint or get_endpoint_from_env() or DEFAULT_ENDPOINT
+    endpoint = get_endpoint(endpoint)
 
     return auth_headers, endpoint
```

### Comparing `seam-0.6.2/seam/phones.py` & `seam-0.7.0/seam/routes/phones.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from seam.types import AbstractPhones, AbstractSeam as Seam, Phone
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractPhones, Phone
 from typing import Optional, Any, List, Dict, Union
-from seam.phones_simulate import PhonesSimulate
+from seam.routes.phones_simulate import PhonesSimulate
 
 
 class Phones(AbstractPhones):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
```

### Comparing `seam-0.6.2/seam/phones_simulate.py` & `seam-0.7.0/seam/routes/phones_simulate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractPhonesSimulate, AbstractSeam as Seam, Phone
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractPhonesSimulate, Phone
 from typing import Optional, Any, List, Dict, Union
 
 
 class PhonesSimulate(AbstractPhonesSimulate):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/routes.py` & `seam-0.7.0/seam/routes/routes.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.2/seam/seam.py` & `seam-0.7.0/seam/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,118 +1,115 @@
-import requests
-from importlib.metadata import version
-from typing import Optional, Union, Dict
+from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Self
+import abc
 
-from seam.parse_options import parse_options
-from .routes import Routes
-from .types import AbstractSeam, SeamApiException
+from seam.routes.types import AbstractRoutes, Workspace
 
 
-class Seam(AbstractSeam):
-    """
-    Initial Seam class used to interact with Seam API
-    """
+class SeamApiException(Exception):
+    def __init__(
+        self,
+        response,
+    ):
+        self.status_code = response.status_code
+        self.request_id = response.headers.get("seam-request-id", None)
+
+        self.metadata = None
+        if "application/json" in response.headers["content-type"]:
+            parsed_response = response.json()
+            self.metadata = parsed_response.get("error", None)
+
+        super().__init__(
+            f"SeamApiException: status={self.status_code}, request_id={self.request_id}, metadata={self.metadata}"
+        )
+
+
+class AbstractRequestMixin(abc.ABC):
+    @abc.abstractmethod
+    def make_request(self, method: str, path: str, **kwargs):
+        raise NotImplementedError
+
 
-    lts_version: str = "1.0.0"
+class AbstractSeam(AbstractRoutes, AbstractRequestMixin):
+    lts_version: str
+    wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]]
 
+    @abc.abstractmethod
     def __init__(
         self,
         api_key: Optional[str] = None,
         *,
         personal_access_token: Optional[str] = None,
         workspace_id: Optional[str] = None,
         endpoint: Optional[str] = None,
         wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
     ):
-        """
-        Parameters
-        ----------
-        api_key : str, optional
-          API key.
-        personal_access_token : str, optional
-          Personal access token.
-        workspace_id : str, optional
-          Workspace id.
-        endpoint : str, optional
-          The API endpoint to which the request should be sent.
-        wait_for_action_attempt : bool or dict, optional
-          Controls whether to wait for an action attempt to complete, either as a boolean or as a dictionary specifying `timeout` and `poll_interval`. Defaults to `False`.
-        """
-
-        Routes.__init__(self)
-
-        self.lts_version = Seam.lts_version
-        self.wait_for_action_attempt = wait_for_action_attempt
-        auth_headers, endpoint = parse_options(
-            api_key=api_key,
-            personal_access_token=personal_access_token,
-            workspace_id=workspace_id,
-            endpoint=endpoint,
-        )
-        self.__auth_headers = auth_headers
-        self.__endpoint = endpoint
-
-    def make_request(self, method: str, path: str, **kwargs):
-        """
-        Makes a request to the API
-
-        Parameters
-        ----------
-        method : str
-          Request method
-        path : str
-          Request path
-        **kwargs
-          Keyword arguments passed to requests.request
-        """
-
-        url = self.__endpoint + path
-        sdk_version = version("seam")
-        headers = {
-            **self.__auth_headers,
-            "Content-Type": "application/json",
-            "User-Agent": "Python SDK v"
-            + sdk_version
-            + " (https://github.com/seamapi/python-next)",
-            "seam-sdk-name": "seamapi/python",
-            "seam-sdk-version": sdk_version,
-            "seam-lts-version": self.lts_version,
-        }
-
-        response = requests.request(method, url, headers=headers, **kwargs)
-
-        if response.status_code != 200:
-            raise SeamApiException(response)
-
-        if "application/json" in response.headers["content-type"]:
-            return response.json()
-
-        return response.text
+        raise NotImplementedError
 
     @classmethod
+    @abc.abstractmethod
     def from_api_key(
         cls,
         api_key: str,
         *,
         endpoint: Optional[str] = None,
         wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
     ) -> Self:
-        return cls(
-            api_key, endpoint=endpoint, wait_for_action_attempt=wait_for_action_attempt
-        )
+        raise NotImplementedError
 
     @classmethod
+    @abc.abstractmethod
     def from_personal_access_token(
         cls,
         personal_access_token: str,
         workspace_id: str,
         *,
         endpoint: Optional[str] = None,
         wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
     ) -> Self:
-        return cls(
-            personal_access_token=personal_access_token,
-            workspace_id=workspace_id,
-            endpoint=endpoint,
-            wait_for_action_attempt=wait_for_action_attempt,
-        )
+        raise NotImplementedError
+
+
+class AbstractSeamMultiWorkspaceWorkspaces(abc.ABC):
+    @abc.abstractmethod
+    def create(
+        self,
+        *,
+        connect_partner_name: str,
+        name: str,
+        is_sandbox: Optional[bool] = None,
+        webview_logo_shape: Optional[str] = None,
+        webview_primary_button_color: Optional[str] = None,
+    ) -> Workspace:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def list(
+        self,
+    ) -> List[Workspace]:
+        raise NotImplementedError()
+
+
+class AbstractSeamMultiWorkspace(AbstractRequestMixin):
+    lts_version: str
+    wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]]
+
+    @abc.abstractmethod
+    def __init__(
+        self,
+        personal_access_token: str,
+        *,
+        endpoint: Optional[str] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
+    ):
+        raise NotImplementedError
+
+    @classmethod
+    @abc.abstractmethod
+    def from_personal_access_token(
+        cls,
+        personal_access_token: str,
+        *,
+        endpoint: Optional[str] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
+    ) -> Self:
+        raise NotImplementedError
```

### Comparing `seam-0.6.2/seam/thermostats.py` & `seam-0.7.0/seam/routes/thermostats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from seam.types import AbstractThermostats, AbstractSeam as Seam, ActionAttempt, Device
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractThermostats, ActionAttempt, Device
 from typing import Optional, Any, List, Dict, Union
-from seam.thermostats_climate_setting_schedules import (
+from seam.routes.thermostats_climate_setting_schedules import (
     ThermostatsClimateSettingSchedules,
 )
 
 
 class Thermostats(AbstractThermostats):
     seam: Seam
```

### Comparing `seam-0.6.2/seam/thermostats_climate_setting_schedules.py` & `seam-0.7.0/seam/routes/thermostats_climate_setting_schedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from seam.types import (
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import (
     AbstractThermostatsClimateSettingSchedules,
-    AbstractSeam as Seam,
     ClimateSettingSchedule,
 )
 from typing import Optional, Any, List, Dict, Union
 
 
 class ThermostatsClimateSettingSchedules(AbstractThermostatsClimateSettingSchedules):
     seam: Seam
```

### Comparing `seam-0.6.2/seam/token.py` & `seam-0.7.0/seam/token.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.2/seam/types.py` & `seam-0.7.0/seam/routes/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Self
 import abc
 from dataclasses import dataclass
-from seam.utils.deep_attr_dict import DeepAttrDict
+from seam.routes.utils.deep_attr_dict import DeepAttrDict
 
 
 @dataclass
 class AccessCode:
     access_code_id: str
     code: str
     common_code_key: str
@@ -186,24 +186,26 @@
 
 @dataclass
 class AcsEntrance:
     acs_entrance_id: str
     acs_system_id: str
     created_at: str
     display_name: str
+    errors: List[Dict[str, Any]]
     latch_metadata: Dict[str, Any]
     visionline_metadata: Dict[str, Any]
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return AcsEntrance(
             acs_entrance_id=d.get("acs_entrance_id", None),
             acs_system_id=d.get("acs_system_id", None),
             created_at=d.get("created_at", None),
             display_name=d.get("display_name", None),
+            errors=d.get("errors", None),
             latch_metadata=DeepAttrDict(d.get("latch_metadata", None)),
             visionline_metadata=DeepAttrDict(d.get("visionline_metadata", None)),
         )
 
 
 @dataclass
 class AcsSystem:
@@ -545,28 +547,38 @@
             user_identity_id=d.get("user_identity_id", None),
             workspace_id=d.get("workspace_id", None),
         )
 
 
 @dataclass
 class Event:
+    acs_credential_id: str
+    acs_system_id: str
+    acs_user_id: str
     action_attempt_id: str
+    client_session_id: str
     created_at: str
     device_id: str
+    enrollment_automation_id: str
     event_id: str
     event_type: str
     occurred_at: str
     workspace_id: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return Event(
+            acs_credential_id=d.get("acs_credential_id", None),
+            acs_system_id=d.get("acs_system_id", None),
+            acs_user_id=d.get("acs_user_id", None),
             action_attempt_id=d.get("action_attempt_id", None),
+            client_session_id=d.get("client_session_id", None),
             created_at=d.get("created_at", None),
             device_id=d.get("device_id", None),
+            enrollment_automation_id=d.get("enrollment_automation_id", None),
             event_id=d.get("event_id", None),
             event_type=d.get("event_type", None),
             occurred_at=d.get("occurred_at", None),
             workspace_id=d.get("workspace_id", None),
         )
 
 
@@ -805,32 +817,14 @@
             connect_partner_name=d.get("connect_partner_name", None),
             is_sandbox=d.get("is_sandbox", None),
             name=d.get("name", None),
             workspace_id=d.get("workspace_id", None),
         )
 
 
-class SeamApiException(Exception):
-    def __init__(
-        self,
-        response,
-    ):
-        self.status_code = response.status_code
-        self.request_id = response.headers.get("seam-request-id", None)
-
-        self.metadata = None
-        if "application/json" in response.headers["content-type"]:
-            parsed_response = response.json()
-            self.metadata = parsed_response.get("error", None)
-
-        super().__init__(
-            f"SeamApiException: status={self.status_code}, request_id={self.request_id}, metadata={self.metadata}"
-        )
-
-
 class AbstractAccessCodesSimulate(abc.ABC):
 
     @abc.abstractmethod
     def create_unmanaged_access_code(
         self, *, code: str, device_id: str, name: str
     ) -> UnmanagedAccessCode:
         raise NotImplementedError()
@@ -842,29 +836,29 @@
     def convert_to_managed(
         self,
         *,
         access_code_id: str,
         allow_external_modification: Optional[bool] = None,
         force: Optional[bool] = None,
         is_external_modification_allowed: Optional[bool] = None,
-        sync: Optional[bool] = None,
+        sync: Optional[bool] = None
     ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, access_code_id: str, sync: Optional[bool] = None) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
         self,
         *,
         access_code_id: Optional[str] = None,
         code: Optional[str] = None,
-        device_id: Optional[str] = None,
+        device_id: Optional[str] = None
     ) -> UnmanagedAccessCode:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self, *, device_id: str, user_identifier_key: Optional[str] = None
     ) -> List[UnmanagedAccessCode]:
@@ -874,15 +868,15 @@
     def update(
         self,
         *,
         access_code_id: str,
         is_managed: bool,
         allow_external_modification: Optional[bool] = None,
         force: Optional[bool] = None,
-        is_external_modification_allowed: Optional[bool] = None,
+        is_external_modification_allowed: Optional[bool] = None
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractAcsAccessGroups(abc.ABC):
 
     @abc.abstractmethod
@@ -921,15 +915,15 @@
     def launch(
         self,
         *,
         credential_manager_acs_system_id: str,
         user_identity_id: str,
         acs_credential_pool_id: Optional[str] = None,
         create_credential_manager_user: Optional[bool] = None,
-        credential_manager_acs_user_id: Optional[str] = None,
+        credential_manager_acs_user_id: Optional[str] = None
     ) -> AcsCredentialProvisioningAutomation:
         raise NotImplementedError()
 
 
 class AbstractAcsCredentials(abc.ABC):
 
     @abc.abstractmethod
@@ -944,15 +938,15 @@
         acs_user_id: str,
         allowed_acs_entrance_ids: Optional[List[str]] = None,
         code: Optional[str] = None,
         credential_manager_acs_system_id: Optional[str] = None,
         ends_at: Optional[str] = None,
         is_multi_phone_sync_credential: Optional[bool] = None,
         starts_at: Optional[str] = None,
-        visionline_metadata: Optional[Dict[str, Any]] = None,
+        visionline_metadata: Optional[Dict[str, Any]] = None
     ) -> AcsCredential:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, acs_credential_id: str) -> None:
         raise NotImplementedError()
 
@@ -963,24 +957,30 @@
     @abc.abstractmethod
     def list(
         self,
         *,
         acs_user_id: Optional[str] = None,
         acs_system_id: Optional[str] = None,
         user_identity_id: Optional[str] = None,
-        is_multi_phone_sync_credential: Optional[bool] = None,
+        is_multi_phone_sync_credential: Optional[bool] = None
     ) -> List[AcsCredential]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def unassign(self, *, acs_credential_id: str, acs_user_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def update(self, *, acs_credential_id: str, code: str) -> None:
+    def update(
+        self,
+        *,
+        acs_credential_id: str,
+        code: Optional[str] = None,
+        ends_at: Optional[str] = None
+    ) -> None:
         raise NotImplementedError()
 
 
 class AbstractAcsEntrances(abc.ABC):
 
     @abc.abstractmethod
     def get(self, *, acs_entrance_id: str) -> AcsEntrance:
@@ -991,15 +991,15 @@
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
         acs_credential_id: Optional[str] = None,
-        acs_system_id: Optional[str] = None,
+        acs_system_id: Optional[str] = None
     ) -> List[AcsEntrance]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list_credentials_with_access(
         self, *, acs_entrance_id: str, include_if: Optional[List[str]] = None
     ) -> List[AcsCredential]:
@@ -1012,14 +1012,20 @@
     def get(self, *, acs_system_id: str) -> AcsSystem:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(self, *, connected_account_id: Optional[str] = None) -> List[AcsSystem]:
         raise NotImplementedError()
 
+    @abc.abstractmethod
+    def list_compatible_credential_manager_acs_systems(
+        self, *, acs_system_id: str
+    ) -> List[AcsSystem]:
+        raise NotImplementedError()
+
 
 class AbstractAcsUsers(abc.ABC):
 
     @abc.abstractmethod
     def add_to_access_group(
         self, *, acs_access_group_id: str, acs_user_id: str
     ) -> None:
@@ -1032,15 +1038,15 @@
         acs_system_id: str,
         access_schedule: Optional[Dict[str, Any]] = None,
         acs_access_group_ids: Optional[List[str]] = None,
         email: Optional[str] = None,
         email_address: Optional[str] = None,
         full_name: Optional[str] = None,
         phone_number: Optional[str] = None,
-        user_identity_id: Optional[str] = None,
+        user_identity_id: Optional[str] = None
     ) -> AcsUser:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, acs_user_id: str) -> None:
         raise NotImplementedError()
 
@@ -1051,15 +1057,15 @@
     @abc.abstractmethod
     def list(
         self,
         *,
         acs_system_id: Optional[str] = None,
         user_identity_email_address: Optional[str] = None,
         user_identity_id: Optional[str] = None,
-        user_identity_phone_number: Optional[str] = None,
+        user_identity_phone_number: Optional[str] = None
     ) -> List[AcsUser]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list_accessible_entrances(self, *, acs_user_id: str) -> List[AcsEntrance]:
         raise NotImplementedError()
 
@@ -1087,114 +1093,114 @@
         *,
         acs_user_id: str,
         access_schedule: Optional[Dict[str, Any]] = None,
         email: Optional[str] = None,
         email_address: Optional[str] = None,
         full_name: Optional[str] = None,
         hid_acs_system_id: Optional[str] = None,
-        phone_number: Optional[str] = None,
+        phone_number: Optional[str] = None
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractActionAttempts(abc.ABC):
 
     @abc.abstractmethod
     def get(
         self,
         *,
         action_attempt_id: str,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(self, *, action_attempt_ids: List[str]) -> List[ActionAttempt]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def poll_until_ready(
         self,
         *,
         action_attempt_id: str,
         timeout: Optional[float] = 5.0,
-        polling_interval: Optional[float] = 0.5,
+        polling_interval: Optional[float] = 0.5
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def decide_and_wait(
         self,
         *,
         action_attempt: ActionAttempt,
-        wait_for_action_attempt: Union[bool, Dict[str, float]],
+        wait_for_action_attempt: Union[bool, Dict[str, float]]
     ) -> ActionAttempt:
         raise NotImplementedError()
 
 
 class AbstractClientSessions(abc.ABC):
 
     @abc.abstractmethod
     def create(
         self,
         *,
         connect_webview_ids: Optional[List[str]] = None,
         connected_account_ids: Optional[List[str]] = None,
         expires_at: Optional[str] = None,
         user_identifier_key: Optional[str] = None,
-        user_identity_ids: Optional[List[str]] = None,
+        user_identity_ids: Optional[List[str]] = None
     ) -> ClientSession:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, client_session_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
         self,
         *,
         client_session_id: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> ClientSession:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get_or_create(
         self,
         *,
         connect_webview_ids: Optional[List[str]] = None,
         connected_account_ids: Optional[List[str]] = None,
         expires_at: Optional[str] = None,
         user_identifier_key: Optional[str] = None,
-        user_identity_ids: Optional[List[str]] = None,
+        user_identity_ids: Optional[List[str]] = None
     ) -> ClientSession:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def grant_access(
         self,
         *,
         client_session_id: Optional[str] = None,
         connect_webview_ids: Optional[List[str]] = None,
         connected_account_ids: Optional[List[str]] = None,
         user_identifier_key: Optional[str] = None,
-        user_identity_ids: Optional[List[str]] = None,
+        user_identity_ids: Optional[List[str]] = None
     ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
         client_session_id: Optional[str] = None,
         connect_webview_id: Optional[str] = None,
         user_identifier_key: Optional[str] = None,
         user_identity_id: Optional[str] = None,
-        without_user_identifier_key: Optional[bool] = None,
+        without_user_identifier_key: Optional[bool] = None
     ) -> List[ClientSession]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def revoke(self, *, client_session_id: str) -> None:
         raise NotImplementedError()
 
@@ -1208,15 +1214,15 @@
         accepted_providers: Optional[List[str]] = None,
         automatically_manage_new_devices: Optional[bool] = None,
         custom_metadata: Optional[Dict[str, Any]] = None,
         custom_redirect_failure_url: Optional[str] = None,
         custom_redirect_url: Optional[str] = None,
         device_selection_mode: Optional[str] = None,
         provider_category: Optional[str] = None,
-        wait_for_device_creation: Optional[bool] = None,
+        wait_for_device_creation: Optional[bool] = None
     ) -> ConnectWebview:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, connect_webview_id: str) -> None:
         raise NotImplementedError()
 
@@ -1225,15 +1231,15 @@
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
         custom_metadata_has: Optional[Dict[str, Any]] = None,
-        user_identifier_key: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[ConnectWebview]:
         raise NotImplementedError()
 
 
 class AbstractConnectedAccounts(abc.ABC):
 
     @abc.abstractmethod
@@ -1254,15 +1260,15 @@
 
     @abc.abstractmethod
     def update(
         self,
         *,
         connected_account_id: str,
         automatically_manage_new_devices: Optional[bool] = None,
-        custom_metadata: Optional[Dict[str, Any]] = None,
+        custom_metadata: Optional[Dict[str, Any]] = None
     ) -> ConnectedAccount:
         raise NotImplementedError()
 
 
 class AbstractDevicesSimulate(abc.ABC):
 
     @abc.abstractmethod
@@ -1290,15 +1296,15 @@
         device_ids: Optional[List[str]] = None,
         device_type: Optional[str] = None,
         device_types: Optional[List[str]] = None,
         exclude_if: Optional[List[str]] = None,
         include_if: Optional[List[str]] = None,
         limit: Optional[float] = None,
         manufacturer: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[UnmanagedDevice]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(self, *, device_id: str, is_managed: bool) -> None:
         raise NotImplementedError()
 
@@ -1307,15 +1313,15 @@
 
     @abc.abstractmethod
     def get(
         self,
         *,
         device_id: Optional[str] = None,
         event_id: Optional[str] = None,
-        event_type: Optional[str] = None,
+        event_type: Optional[str] = None
     ) -> Event:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
@@ -1324,15 +1330,15 @@
         between: Optional[List[str]] = None,
         connected_account_id: Optional[str] = None,
         device_id: Optional[str] = None,
         device_ids: Optional[List[str]] = None,
         event_type: Optional[str] = None,
         event_types: Optional[List[str]] = None,
         limit: Optional[float] = None,
-        since: Optional[str] = None,
+        since: Optional[str] = None
     ) -> List[Event]:
         raise NotImplementedError()
 
 
 class AbstractLocks(abc.ABC):
 
     @abc.abstractmethod
@@ -1353,35 +1359,35 @@
         device_ids: Optional[List[str]] = None,
         device_type: Optional[str] = None,
         device_types: Optional[List[str]] = None,
         exclude_if: Optional[List[str]] = None,
         include_if: Optional[List[str]] = None,
         limit: Optional[float] = None,
         manufacturer: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[Device]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def lock_door(
         self,
         *,
         device_id: str,
         sync: Optional[bool] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def unlock_door(
         self,
         *,
         device_id: str,
         sync: Optional[bool] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         raise NotImplementedError()
 
 
 class AbstractNetworks(abc.ABC):
 
     @abc.abstractmethod
@@ -1403,15 +1409,15 @@
         *,
         device_id: str,
         ends_daily_at: str,
         starts_daily_at: str,
         name: Optional[str] = None,
         noise_threshold_decibels: Optional[float] = None,
         noise_threshold_nrs: Optional[float] = None,
-        sync: Optional[bool] = None,
+        sync: Optional[bool] = None
     ) -> NoiseThreshold:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(
         self, *, device_id: str, noise_threshold_id: str, sync: Optional[bool] = None
     ) -> None:
@@ -1434,15 +1440,15 @@
         device_id: str,
         noise_threshold_id: str,
         ends_daily_at: Optional[str] = None,
         name: Optional[str] = None,
         noise_threshold_decibels: Optional[float] = None,
         noise_threshold_nrs: Optional[float] = None,
         starts_daily_at: Optional[str] = None,
-        sync: Optional[bool] = None,
+        sync: Optional[bool] = None
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractNoiseSensorsSimulate(abc.ABC):
 
     @abc.abstractmethod
@@ -1455,15 +1461,15 @@
     @abc.abstractmethod
     def create_sandbox_phone(
         self,
         *,
         user_identity_id: str,
         assa_abloy_metadata: Optional[Dict[str, Any]] = None,
         custom_sdk_installation_id: Optional[str] = None,
-        phone_metadata: Optional[Dict[str, Any]] = None,
+        phone_metadata: Optional[Dict[str, Any]] = None
     ) -> Phone:
         raise NotImplementedError()
 
 
 class AbstractThermostatsClimateSettingSchedules(abc.ABC):
 
     @abc.abstractmethod
@@ -1478,28 +1484,28 @@
         cooling_set_point_celsius: Optional[float] = None,
         cooling_set_point_fahrenheit: Optional[float] = None,
         heating_set_point_celsius: Optional[float] = None,
         heating_set_point_fahrenheit: Optional[float] = None,
         hvac_mode_setting: Optional[str] = None,
         manual_override_allowed: Optional[bool] = None,
         name: Optional[str] = None,
-        schedule_type: Optional[str] = None,
+        schedule_type: Optional[str] = None
     ) -> ClimateSettingSchedule:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, climate_setting_schedule_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
         self,
         *,
         climate_setting_schedule_id: Optional[str] = None,
-        device_id: Optional[str] = None,
+        device_id: Optional[str] = None
     ) -> ClimateSettingSchedule:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self, *, device_id: str, user_identifier_key: Optional[str] = None
     ) -> List[ClimateSettingSchedule]:
@@ -1517,15 +1523,15 @@
         heating_set_point_celsius: Optional[float] = None,
         heating_set_point_fahrenheit: Optional[float] = None,
         hvac_mode_setting: Optional[str] = None,
         manual_override_allowed: Optional[bool] = None,
         name: Optional[str] = None,
         schedule_ends_at: Optional[str] = None,
         schedule_starts_at: Optional[str] = None,
-        schedule_type: Optional[str] = None,
+        schedule_type: Optional[str] = None
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractUserIdentitiesEnrollmentAutomations(abc.ABC):
 
     @abc.abstractmethod
@@ -1540,15 +1546,15 @@
     def launch(
         self,
         *,
         credential_manager_acs_system_id: str,
         user_identity_id: str,
         acs_credential_pool_id: Optional[str] = None,
         create_credential_manager_user: Optional[bool] = None,
-        credential_manager_acs_user_id: Optional[str] = None,
+        credential_manager_acs_user_id: Optional[str] = None
     ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(self, *, user_identity_id: str) -> List[EnrollmentAutomation]:
         raise NotImplementedError()
 
@@ -1584,15 +1590,15 @@
     def create(
         self,
         *,
         connect_partner_name: str,
         name: str,
         is_sandbox: Optional[bool] = None,
         webview_logo_shape: Optional[str] = None,
-        webview_primary_button_color: Optional[str] = None,
+        webview_primary_button_color: Optional[str] = None
     ) -> Workspace:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
         self,
     ) -> Workspace:
@@ -1638,15 +1644,15 @@
     def cool(
         self,
         *,
         device_id: str,
         cooling_set_point_celsius: Optional[float] = None,
         cooling_set_point_fahrenheit: Optional[float] = None,
         sync: Optional[bool] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
         self, *, device_id: Optional[str] = None, name: Optional[str] = None
     ) -> Device:
@@ -1656,29 +1662,29 @@
     def heat(
         self,
         *,
         device_id: str,
         heating_set_point_celsius: Optional[float] = None,
         heating_set_point_fahrenheit: Optional[float] = None,
         sync: Optional[bool] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def heat_cool(
         self,
         *,
         device_id: str,
         cooling_set_point_celsius: Optional[float] = None,
         cooling_set_point_fahrenheit: Optional[float] = None,
         heating_set_point_celsius: Optional[float] = None,
         heating_set_point_fahrenheit: Optional[float] = None,
         sync: Optional[bool] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
@@ -1690,37 +1696,37 @@
         device_ids: Optional[List[str]] = None,
         device_type: Optional[str] = None,
         device_types: Optional[List[str]] = None,
         exclude_if: Optional[List[str]] = None,
         include_if: Optional[List[str]] = None,
         limit: Optional[float] = None,
         manufacturer: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[Device]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def off(
         self,
         *,
         device_id: str,
         sync: Optional[bool] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def set_fan_mode(
         self,
         *,
         device_id: str,
         fan_mode: Optional[str] = None,
         fan_mode_setting: Optional[str] = None,
         sync: Optional[bool] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(
         self, *, default_climate_setting: Dict[str, Any], device_id: str
     ) -> None:
@@ -1741,28 +1747,28 @@
     @abc.abstractmethod
     def create(
         self,
         *,
         email_address: Optional[str] = None,
         full_name: Optional[str] = None,
         phone_number: Optional[str] = None,
-        user_identity_key: Optional[str] = None,
+        user_identity_key: Optional[str] = None
     ) -> UserIdentity:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, user_identity_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
         self,
         *,
         user_identity_id: Optional[str] = None,
-        user_identity_key: Optional[str] = None,
+        user_identity_key: Optional[str] = None
     ) -> UserIdentity:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def grant_access_to_device(self, *, device_id: str, user_identity_id: str) -> None:
         raise NotImplementedError()
 
@@ -1796,15 +1802,15 @@
     def update(
         self,
         *,
         user_identity_id: str,
         email_address: Optional[str] = None,
         full_name: Optional[str] = None,
         phone_number: Optional[str] = None,
-        user_identity_key: Optional[str] = None,
+        user_identity_key: Optional[str] = None
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractAccessCodes(abc.ABC):
 
     @property
@@ -1832,15 +1838,15 @@
         is_one_time_use: Optional[bool] = None,
         max_time_rounding: Optional[str] = None,
         name: Optional[str] = None,
         prefer_native_scheduling: Optional[bool] = None,
         starts_at: Optional[str] = None,
         sync: Optional[bool] = None,
         use_backup_access_code_pool: Optional[bool] = None,
-        use_offline_access_code: Optional[bool] = None,
+        use_offline_access_code: Optional[bool] = None
     ) -> AccessCode:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def create_multiple(
         self,
         *,
@@ -1855,49 +1861,49 @@
         is_one_time_use: Optional[bool] = None,
         max_time_rounding: Optional[str] = None,
         name: Optional[str] = None,
         prefer_native_scheduling: Optional[bool] = None,
         preferred_code_length: Optional[float] = None,
         starts_at: Optional[str] = None,
         use_backup_access_code_pool: Optional[bool] = None,
-        use_offline_access_code: Optional[bool] = None,
+        use_offline_access_code: Optional[bool] = None
     ) -> List[AccessCode]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(
         self,
         *,
         access_code_id: str,
         device_id: Optional[str] = None,
-        sync: Optional[bool] = None,
+        sync: Optional[bool] = None
     ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def generate_code(self, *, device_id: str) -> AccessCode:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
         self,
         *,
         access_code_id: Optional[str] = None,
         code: Optional[str] = None,
-        device_id: Optional[str] = None,
+        device_id: Optional[str] = None
     ) -> AccessCode:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
         access_code_ids: Optional[List[str]] = None,
         device_id: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[AccessCode]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def pull_backup_access_code(self, *, access_code_id: str) -> AccessCode:
         raise NotImplementedError()
 
@@ -1918,15 +1924,15 @@
         max_time_rounding: Optional[str] = None,
         name: Optional[str] = None,
         prefer_native_scheduling: Optional[bool] = None,
         starts_at: Optional[str] = None,
         sync: Optional[bool] = None,
         type: Optional[str] = None,
         use_backup_access_code_pool: Optional[bool] = None,
-        use_offline_access_code: Optional[bool] = None,
+        use_offline_access_code: Optional[bool] = None
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractDevices(abc.ABC):
 
     @property
@@ -1961,15 +1967,15 @@
         device_ids: Optional[List[str]] = None,
         device_type: Optional[str] = None,
         device_types: Optional[List[str]] = None,
         exclude_if: Optional[List[str]] = None,
         include_if: Optional[List[str]] = None,
         limit: Optional[float] = None,
         manufacturer: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[Device]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list_device_providers(
         self, *, provider_category: Optional[str] = None
     ) -> List[DeviceProvider]:
@@ -1979,15 +1985,15 @@
     def update(
         self,
         *,
         device_id: str,
         custom_metadata: Optional[Dict[str, Any]] = None,
         is_managed: Optional[bool] = None,
         name: Optional[str] = None,
-        properties: Optional[Dict[str, Any]] = None,
+        properties: Optional[Dict[str, Any]] = None
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractNoiseSensors(abc.ABC):
     pass
 
@@ -2057,51 +2063,7 @@
     networks: AbstractNetworks
     noise_sensors: AbstractNoiseSensors
     phones: AbstractPhones
     thermostats: AbstractThermostats
     user_identities: AbstractUserIdentities
     webhooks: AbstractWebhooks
     workspaces: AbstractWorkspaces
-
-
-class AbstractSeam(AbstractRoutes):
-    lts_version: str
-
-    @abc.abstractmethod
-    def __init__(
-        self,
-        api_key: Optional[str] = None,
-        *,
-        personal_access_token: Optional[str] = None,
-        workspace_id: Optional[str] = None,
-        endpoint: Optional[str] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
-    ):
-        self.wait_for_action_attempt = wait_for_action_attempt
-        self.lts_version = AbstractSeam.lts_version
-
-    @abc.abstractmethod
-    def make_request(self, method: str, path: str, **kwargs) -> Any:
-        raise NotImplementedError
-
-    @classmethod
-    @abc.abstractmethod
-    def from_api_key(
-        cls,
-        api_key: str,
-        *,
-        endpoint: Optional[str] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
-    ) -> Self:
-        raise NotImplementedError
-
-    @classmethod
-    @abc.abstractmethod
-    def from_personal_access_token(
-        cls,
-        personal_access_token: str,
-        workspace_id: str,
-        *,
-        endpoint: Optional[str] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
-    ) -> Self:
-        raise NotImplementedError
```

### Comparing `seam-0.6.2/seam/user_identities.py` & `seam-0.7.0/seam/routes/user_identities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from seam.types import (
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import (
     AbstractUserIdentities,
-    AbstractSeam as Seam,
     UserIdentity,
     Device,
     AcsSystem,
     AcsUser,
 )
 from typing import Optional, Any, List, Dict, Union
-from seam.user_identities_enrollment_automations import (
+from seam.routes.user_identities_enrollment_automations import (
     UserIdentitiesEnrollmentAutomations,
 )
 
 
 class UserIdentities(AbstractUserIdentities):
     seam: Seam
```

### Comparing `seam-0.6.2/seam/user_identities_enrollment_automations.py` & `seam-0.7.0/seam/routes/user_identities_enrollment_automations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from seam.types import (
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import (
     AbstractUserIdentitiesEnrollmentAutomations,
-    AbstractSeam as Seam,
     EnrollmentAutomation,
 )
 from typing import Optional, Any, List, Dict, Union
 
 
 class UserIdentitiesEnrollmentAutomations(AbstractUserIdentitiesEnrollmentAutomations):
     seam: Seam
```

### Comparing `seam-0.6.2/seam/utils/deep_attr_dict.py` & `seam-0.7.0/seam/routes/utils/deep_attr_dict.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.2/seam/webhooks.py` & `seam-0.7.0/seam/routes/webhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from seam.types import AbstractWebhooks, AbstractSeam as Seam, Webhook
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractWebhooks, Webhook
 from typing import Optional, Any, List, Dict, Union
 
 
 class Webhooks(AbstractWebhooks):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/seam/workspaces.py` & `seam-0.7.0/seam/routes/workspaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from seam.types import (
-    AbstractWorkspaces,
-    AbstractSeam as Seam,
-    Workspace,
-    ActionAttempt,
-)
+from seam.types import AbstractSeam as Seam
+from seam.routes.types import AbstractWorkspaces, Workspace, ActionAttempt
 from typing import Optional, Any, List, Dict, Union
 
 
 class Workspaces(AbstractWorkspaces):
     seam: Seam
 
     def __init__(self, seam: Seam):
```

### Comparing `seam-0.6.2/PKG-INFO` & `seam-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seam
-Version: 0.6.2
+Version: 0.7.0
 Summary: SDK for the Seam API written in Python.
 Home-page: https://github.com/seamapi/python-next
 License: MIT
 Author: Seam Labs, Inc.
 Author-email: engineering@getseam.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

