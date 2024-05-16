# Comparing `tmp/opentelemetry_resource_detector_azure-0.1.4.tar.gz` & `tmp/opentelemetry_resource_detector_azure-0.1.5.tar.gz`

## Comparing `opentelemetry_resource_detector_azure-0.1.4.tar` & `opentelemetry_resource_detector_azure-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/app_service.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/version.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/vm.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/tests/test_app_service.py
--rw-r--r--   0        0        0    14075 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/tests/test_vm.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/.gitignore
--rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/LICENSE
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/README.rst
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/src/opentelemetry/resource/detector/azure/__init__.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/src/opentelemetry/resource/detector/azure/_constants.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/src/opentelemetry/resource/detector/azure/_utils.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/src/opentelemetry/resource/detector/azure/app_service.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/src/opentelemetry/resource/detector/azure/functions.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/src/opentelemetry/resource/detector/azure/version.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/src/opentelemetry/resource/detector/azure/vm.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/tests/test_app_service.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/tests/test_functions.py
+-rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/tests/test_vm.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/README.rst
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.5/PKG-INFO
```

### Comparing `opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/version.py` & `opentelemetry_resource_detector_azure-0.1.5/src/opentelemetry/resource/detector/azure/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright The OpenTelemetry Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-__version__ = "0.1.4"
+# Copyright The OpenTelemetry Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+__version__ = "0.1.5"
```

### Comparing `opentelemetry_resource_detector_azure-0.1.4/tests/test_app_service.py` & `opentelemetry_resource_detector_azure-0.1.5/tests/test_app_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,154 +1,193 @@
-# Copyright The OpenTelemetry Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-import unittest
-from unittest.mock import patch
-
-# pylint: disable=no-name-in-module
-from opentelemetry.resource.detector.azure.app_service import (
-    AzureAppServiceResourceDetector,
-)
-
-TEST_WEBSITE_SITE_NAME = "TEST_WEBSITE_SITE_NAME"
-TEST_REGION_NAME = "TEST_REGION_NAME"
-TEST_WEBSITE_SLOT_NAME = "TEST_WEBSITE_SLOT_NAME"
-TEST_WEBSITE_HOSTNAME = "TEST_WEBSITE_HOSTNAME"
-TEST_WEBSITE_INSTANCE_ID = "TEST_WEBSITE_INSTANCE_ID"
-TEST_WEBSITE_HOME_STAMPNAME = "TEST_WEBSITE_HOME_STAMPNAME"
-
-TEST_WEBSITE_RESOURCE_GROUP = "TEST_WEBSITE_RESOURCE_GROUP"
-TEST_WEBSITE_OWNER_NAME = "TEST_WEBSITE_OWNER_NAME"
-
-
-class TestAzureAppServiceResourceDetector(unittest.TestCase):
-    @patch.dict(
-        "os.environ",
-        {
-            "WEBSITE_SITE_NAME": TEST_WEBSITE_SITE_NAME,
-            "REGION_NAME": TEST_REGION_NAME,
-            "WEBSITE_SLOT_NAME": TEST_WEBSITE_SLOT_NAME,
-            "WEBSITE_HOSTNAME": TEST_WEBSITE_HOSTNAME,
-            "WEBSITE_INSTANCE_ID": TEST_WEBSITE_INSTANCE_ID,
-            "WEBSITE_HOME_STAMPNAME": TEST_WEBSITE_HOME_STAMPNAME,
-            "WEBSITE_RESOURCE_GROUP": TEST_WEBSITE_RESOURCE_GROUP,
-            "WEBSITE_OWNER_NAME": TEST_WEBSITE_OWNER_NAME,
-        },
-        clear=True,
-    )
-    def test_on_app_service(self):
-        resource = AzureAppServiceResourceDetector().detect()
-        attributes = resource.attributes
-        self.assertEqual(attributes["service.name"], TEST_WEBSITE_SITE_NAME)
-        self.assertEqual(attributes["cloud.provider"], "azure")
-        self.assertEqual(attributes["cloud.platform"], "azure_app_service")
-
-        self.assertEqual(
-            attributes["cloud.resource_id"],
-            f"/subscriptions/{TEST_WEBSITE_OWNER_NAME}/resourceGroups/{TEST_WEBSITE_RESOURCE_GROUP}/providers/Microsoft.Web/sites/{TEST_WEBSITE_SITE_NAME}",
-        )
-
-        self.assertEqual(attributes["cloud.region"], TEST_REGION_NAME)
-        self.assertEqual(
-            attributes["deployment.environment"], TEST_WEBSITE_SLOT_NAME
-        )
-        self.assertEqual(attributes["host.id"], TEST_WEBSITE_HOSTNAME)
-        self.assertEqual(
-            attributes["service.instance.id"], TEST_WEBSITE_INSTANCE_ID
-        )
-        self.assertEqual(
-            attributes["azure.app.service.stamp"], TEST_WEBSITE_HOME_STAMPNAME
-        )
-
-    @patch.dict(
-        "os.environ",
-        {
-            "WEBSITE_SITE_NAME": TEST_WEBSITE_SITE_NAME,
-            "REGION_NAME": TEST_REGION_NAME,
-            "WEBSITE_SLOT_NAME": TEST_WEBSITE_SLOT_NAME,
-            "WEBSITE_HOSTNAME": TEST_WEBSITE_HOSTNAME,
-            "WEBSITE_INSTANCE_ID": TEST_WEBSITE_INSTANCE_ID,
-            "WEBSITE_HOME_STAMPNAME": TEST_WEBSITE_HOME_STAMPNAME,
-            "WEBSITE_OWNER_NAME": TEST_WEBSITE_OWNER_NAME,
-        },
-        clear=True,
-    )
-    def test_on_app_service_no_resource_group(self):
-        resource = AzureAppServiceResourceDetector().detect()
-        attributes = resource.attributes
-        self.assertEqual(attributes["service.name"], TEST_WEBSITE_SITE_NAME)
-        self.assertEqual(attributes["cloud.provider"], "azure")
-        self.assertEqual(attributes["cloud.platform"], "azure_app_service")
-
-        self.assertTrue("cloud.resource_id" not in attributes)
-
-        self.assertEqual(attributes["cloud.region"], TEST_REGION_NAME)
-        self.assertEqual(
-            attributes["deployment.environment"], TEST_WEBSITE_SLOT_NAME
-        )
-        self.assertEqual(attributes["host.id"], TEST_WEBSITE_HOSTNAME)
-        self.assertEqual(
-            attributes["service.instance.id"], TEST_WEBSITE_INSTANCE_ID
-        )
-        self.assertEqual(
-            attributes["azure.app.service.stamp"], TEST_WEBSITE_HOME_STAMPNAME
-        )
-
-    @patch.dict(
-        "os.environ",
-        {
-            "WEBSITE_SITE_NAME": TEST_WEBSITE_SITE_NAME,
-            "REGION_NAME": TEST_REGION_NAME,
-            "WEBSITE_SLOT_NAME": TEST_WEBSITE_SLOT_NAME,
-            "WEBSITE_HOSTNAME": TEST_WEBSITE_HOSTNAME,
-            "WEBSITE_INSTANCE_ID": TEST_WEBSITE_INSTANCE_ID,
-            "WEBSITE_HOME_STAMPNAME": TEST_WEBSITE_HOME_STAMPNAME,
-            "WEBSITE_OWNER_NAME": TEST_WEBSITE_OWNER_NAME,
-        },
-        clear=True,
-    )
-    def test_on_app_service_no_owner(self):
-        resource = AzureAppServiceResourceDetector().detect()
-        attributes = resource.attributes
-        self.assertEqual(attributes["service.name"], TEST_WEBSITE_SITE_NAME)
-        self.assertEqual(attributes["cloud.provider"], "azure")
-        self.assertEqual(attributes["cloud.platform"], "azure_app_service")
-
-        self.assertTrue("cloud.resource_id" not in attributes)
-
-        self.assertEqual(attributes["cloud.region"], TEST_REGION_NAME)
-        self.assertEqual(
-            attributes["deployment.environment"], TEST_WEBSITE_SLOT_NAME
-        )
-        self.assertEqual(attributes["host.id"], TEST_WEBSITE_HOSTNAME)
-        self.assertEqual(
-            attributes["service.instance.id"], TEST_WEBSITE_INSTANCE_ID
-        )
-        self.assertEqual(
-            attributes["azure.app.service.stamp"], TEST_WEBSITE_HOME_STAMPNAME
-        )
-
-    @patch.dict(
-        "os.environ",
-        {
-            "REGION_NAME": TEST_REGION_NAME,
-            "WEBSITE_SLOT_NAME": TEST_WEBSITE_SLOT_NAME,
-            "WEBSITE_HOSTNAME": TEST_WEBSITE_HOSTNAME,
-            "WEBSITE_INSTANCE_ID": TEST_WEBSITE_INSTANCE_ID,
-            "WEBSITE_HOME_STAMPNAME": TEST_WEBSITE_HOME_STAMPNAME,
-            "WEBSITE_OWNER_NAME": TEST_WEBSITE_OWNER_NAME,
-        },
-        clear=True,
-    )
-    def test_off_app_service(self):
-        resource = AzureAppServiceResourceDetector().detect()
-        self.assertEqual(resource.attributes, {})
+# Copyright The OpenTelemetry Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import unittest
+from unittest.mock import patch
+
+# pylint: disable=no-name-in-module
+from opentelemetry.resource.detector.azure.app_service import (
+    AzureAppServiceResourceDetector,
+)
+
+TEST_WEBSITE_SITE_NAME = "TEST_WEBSITE_SITE_NAME"
+TEST_REGION_NAME = "TEST_REGION_NAME"
+TEST_WEBSITE_SLOT_NAME = "TEST_WEBSITE_SLOT_NAME"
+TEST_WEBSITE_HOSTNAME = "TEST_WEBSITE_HOSTNAME"
+TEST_WEBSITE_INSTANCE_ID = "TEST_WEBSITE_INSTANCE_ID"
+TEST_WEBSITE_HOME_STAMPNAME = "TEST_WEBSITE_HOME_STAMPNAME"
+
+TEST_WEBSITE_RESOURCE_GROUP = "TEST_WEBSITE_RESOURCE_GROUP"
+TEST_WEBSITE_OWNER_NAME = "TEST_WEBSITE_OWNER_NAME"
+
+
+class TestAzureAppServiceResourceDetector(unittest.TestCase):
+    @patch.dict(
+        "os.environ",
+        {
+            "WEBSITE_SITE_NAME": TEST_WEBSITE_SITE_NAME,
+            "REGION_NAME": TEST_REGION_NAME,
+            "WEBSITE_SLOT_NAME": TEST_WEBSITE_SLOT_NAME,
+            "WEBSITE_HOSTNAME": TEST_WEBSITE_HOSTNAME,
+            "WEBSITE_INSTANCE_ID": TEST_WEBSITE_INSTANCE_ID,
+            "WEBSITE_HOME_STAMPNAME": TEST_WEBSITE_HOME_STAMPNAME,
+            "WEBSITE_RESOURCE_GROUP": TEST_WEBSITE_RESOURCE_GROUP,
+            "WEBSITE_OWNER_NAME": TEST_WEBSITE_OWNER_NAME,
+        },
+        clear=True,
+    )
+    def test_on_app_service(self):
+        resource = AzureAppServiceResourceDetector().detect()
+        attributes = resource.attributes
+        self.assertEqual(attributes["service.name"], TEST_WEBSITE_SITE_NAME)
+        self.assertEqual(attributes["cloud.provider"], "azure")
+        self.assertEqual(attributes["cloud.platform"], "azure_app_service")
+
+        self.assertEqual(
+            attributes["cloud.resource_id"],
+            f"/subscriptions/{TEST_WEBSITE_OWNER_NAME}/resourceGroups/{TEST_WEBSITE_RESOURCE_GROUP}/providers/Microsoft.Web/sites/{TEST_WEBSITE_SITE_NAME}",
+        )
+
+        self.assertEqual(attributes["cloud.region"], TEST_REGION_NAME)
+        self.assertEqual(
+            attributes["deployment.environment"], TEST_WEBSITE_SLOT_NAME
+        )
+        self.assertEqual(attributes["host.id"], TEST_WEBSITE_HOSTNAME)
+        self.assertEqual(
+            attributes["service.instance.id"], TEST_WEBSITE_INSTANCE_ID
+        )
+        self.assertEqual(
+            attributes["azure.app.service.stamp"], TEST_WEBSITE_HOME_STAMPNAME
+        )
+    
+    @patch.dict(
+        "os.environ",
+        {
+            "FUNCTIONS_WORKER_RUNTIME": "1",
+            "WEBSITE_SITE_NAME": TEST_WEBSITE_SITE_NAME,
+            "REGION_NAME": TEST_REGION_NAME,
+            "WEBSITE_SLOT_NAME": TEST_WEBSITE_SLOT_NAME,
+            "WEBSITE_HOSTNAME": TEST_WEBSITE_HOSTNAME,
+            "WEBSITE_INSTANCE_ID": TEST_WEBSITE_INSTANCE_ID,
+            "WEBSITE_HOME_STAMPNAME": TEST_WEBSITE_HOME_STAMPNAME,
+            "WEBSITE_RESOURCE_GROUP": TEST_WEBSITE_RESOURCE_GROUP,
+            "WEBSITE_OWNER_NAME": TEST_WEBSITE_OWNER_NAME,
+        },
+        clear=True,
+    )
+    def test_on_app_service_with_functions(self):
+        resource = AzureAppServiceResourceDetector().detect()
+        attributes = resource.attributes
+        self.assertIsNone(attributes.get("service.name"))
+        self.assertEqual(attributes["cloud.provider"], "azure")
+        self.assertIsNone(attributes.get("cloud.platform"))
+
+        self.assertEqual(
+            attributes["cloud.resource_id"],
+            f"/subscriptions/{TEST_WEBSITE_OWNER_NAME}/resourceGroups/{TEST_WEBSITE_RESOURCE_GROUP}/providers/Microsoft.Web/sites/{TEST_WEBSITE_SITE_NAME}",
+        )
+
+        self.assertEqual(attributes["cloud.region"], TEST_REGION_NAME)
+        self.assertEqual(
+            attributes["deployment.environment"], TEST_WEBSITE_SLOT_NAME
+        )
+        self.assertEqual(attributes["host.id"], TEST_WEBSITE_HOSTNAME)
+        self.assertEqual(
+            attributes["service.instance.id"], TEST_WEBSITE_INSTANCE_ID
+        )
+        self.assertEqual(
+            attributes["azure.app.service.stamp"], TEST_WEBSITE_HOME_STAMPNAME
+        )
+
+    @patch.dict(
+        "os.environ",
+        {
+            "WEBSITE_SITE_NAME": TEST_WEBSITE_SITE_NAME,
+            "REGION_NAME": TEST_REGION_NAME,
+            "WEBSITE_SLOT_NAME": TEST_WEBSITE_SLOT_NAME,
+            "WEBSITE_HOSTNAME": TEST_WEBSITE_HOSTNAME,
+            "WEBSITE_INSTANCE_ID": TEST_WEBSITE_INSTANCE_ID,
+            "WEBSITE_HOME_STAMPNAME": TEST_WEBSITE_HOME_STAMPNAME,
+            "WEBSITE_OWNER_NAME": TEST_WEBSITE_OWNER_NAME,
+        },
+        clear=True,
+    )
+    def test_on_app_service_no_resource_group(self):
+        resource = AzureAppServiceResourceDetector().detect()
+        attributes = resource.attributes
+        self.assertEqual(attributes["service.name"], TEST_WEBSITE_SITE_NAME)
+        self.assertEqual(attributes["cloud.provider"], "azure")
+        self.assertEqual(attributes["cloud.platform"], "azure_app_service")
+
+        self.assertTrue("cloud.resource_id" not in attributes)
+
+        self.assertEqual(attributes["cloud.region"], TEST_REGION_NAME)
+        self.assertEqual(
+            attributes["deployment.environment"], TEST_WEBSITE_SLOT_NAME
+        )
+        self.assertEqual(attributes["host.id"], TEST_WEBSITE_HOSTNAME)
+        self.assertEqual(
+            attributes["service.instance.id"], TEST_WEBSITE_INSTANCE_ID
+        )
+        self.assertEqual(
+            attributes["azure.app.service.stamp"], TEST_WEBSITE_HOME_STAMPNAME
+        )
+
+    @patch.dict(
+        "os.environ",
+        {
+            "WEBSITE_SITE_NAME": TEST_WEBSITE_SITE_NAME,
+            "REGION_NAME": TEST_REGION_NAME,
+            "WEBSITE_SLOT_NAME": TEST_WEBSITE_SLOT_NAME,
+            "WEBSITE_HOSTNAME": TEST_WEBSITE_HOSTNAME,
+            "WEBSITE_INSTANCE_ID": TEST_WEBSITE_INSTANCE_ID,
+            "WEBSITE_HOME_STAMPNAME": TEST_WEBSITE_HOME_STAMPNAME,
+            "WEBSITE_OWNER_NAME": TEST_WEBSITE_OWNER_NAME,
+        },
+        clear=True,
+    )
+    def test_on_app_service_no_owner(self):
+        resource = AzureAppServiceResourceDetector().detect()
+        attributes = resource.attributes
+        self.assertEqual(attributes["service.name"], TEST_WEBSITE_SITE_NAME)
+        self.assertEqual(attributes["cloud.provider"], "azure")
+        self.assertEqual(attributes["cloud.platform"], "azure_app_service")
+
+        self.assertTrue("cloud.resource_id" not in attributes)
+
+        self.assertEqual(attributes["cloud.region"], TEST_REGION_NAME)
+        self.assertEqual(
+            attributes["deployment.environment"], TEST_WEBSITE_SLOT_NAME
+        )
+        self.assertEqual(attributes["host.id"], TEST_WEBSITE_HOSTNAME)
+        self.assertEqual(
+            attributes["service.instance.id"], TEST_WEBSITE_INSTANCE_ID
+        )
+        self.assertEqual(
+            attributes["azure.app.service.stamp"], TEST_WEBSITE_HOME_STAMPNAME
+        )
+
+    @patch.dict(
+        "os.environ",
+        {
+            "REGION_NAME": TEST_REGION_NAME,
+            "WEBSITE_SLOT_NAME": TEST_WEBSITE_SLOT_NAME,
+            "WEBSITE_HOSTNAME": TEST_WEBSITE_HOSTNAME,
+            "WEBSITE_INSTANCE_ID": TEST_WEBSITE_INSTANCE_ID,
+            "WEBSITE_HOME_STAMPNAME": TEST_WEBSITE_HOME_STAMPNAME,
+            "WEBSITE_OWNER_NAME": TEST_WEBSITE_OWNER_NAME,
+        },
+        clear=True,
+    )
+    def test_off_app_service(self):
+        resource = AzureAppServiceResourceDetector().detect()
+        self.assertEqual(resource.attributes, {})
```

### Comparing `opentelemetry_resource_detector_azure-0.1.4/tests/test_vm.py` & `opentelemetry_resource_detector_azure-0.1.5/tests/test_vm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,380 +1,390 @@
-# Copyright The OpenTelemetry Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-import unittest
-from unittest.mock import patch
-
-# pylint: disable=no-name-in-module
-from opentelemetry.resource.detector.azure.vm import AzureVMResourceDetector
-
-LINUX_JSON = """
-{
-    "additionalCapabilities": {
-        "hibernationEnabled": "false"
-    },
-    "azEnvironment": "AzurePublicCloud",
-    "customData": "",
-    "evictionPolicy": "",
-    "extendedLocation": {
-        "name": "",
-        "type": ""
-    },
-    "host": {
-        "id": ""
-    },
-    "hostGroup": {
-        "id": ""
-    },
-    "isHostCompatibilityLayerVm": "true",
-    "licenseType": "",
-    "location": "westus",
-    "name": "examplevmname",
-    "offer": "0001-com-ubuntu-server-focal",
-    "osProfile": {
-        "adminUsername": "azureuser",
-        "computerName": "examplevmname",
-        "disablePasswordAuthentication": "true"
-    },
-    "osType": "Linux",
-    "placementGroupId": "",
-    "plan": {
-        "name": "",
-        "product": "",
-        "publisher": ""
-    },
-    "platformFaultDomain": "0",
-    "platformSubFaultDomain": "",
-    "platformUpdateDomain": "0",
-    "priority": "",
-    "provider": "Microsoft.Compute",
-    "publicKeys": [
-        {
-            "keyData": "ssh-rsa 0",
-            "path": "/home/user/.ssh/authorized_keys0"
-        },
-        {
-            "keyData": "ssh-rsa 1",
-            "path": "/home/user/.ssh/authorized_keys1"
-        }
-    ],
-    "publisher": "canonical",
-    "resourceGroupName": "macikgo-test-may-23",
-    "resourceId": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/virtualMachines/examplevmname",
-    "securityProfile": {
-        "encryptionAtHost": "false",
-        "secureBootEnabled": "true",
-        "securityType": "TrustedLaunch",
-        "virtualTpmEnabled": "true"
-    },
-    "sku": "20_04-lts-gen2",
-    "storageProfile": {
-        "dataDisks": [
-            {
-                "bytesPerSecondThrottle": "979202048",
-                "caching": "None",
-                "createOption": "Empty",
-                "diskCapacityBytes": "274877906944",
-                "diskSizeGB": "1024",
-                "image": {
-                    "uri": ""
-                },
-                "isSharedDisk": "false",
-                "isUltraDisk": "true",
-                "lun": "0",
-                "managedDisk": {
-                    "id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/disks/exampledatadiskname",
-                    "storageAccountType": "StandardSSD_LRS"
-                },
-                "name": "exampledatadiskname",
-                "opsPerSecondThrottle": "65280",
-                "vhd": {
-                    "uri": ""
-                },
-                "writeAcceleratorEnabled": "false"
-            }
-        ],
-        "imageReference": {
-            "id": "",
-            "offer": "0001-com-ubuntu-server-focal",
-            "publisher": "canonical",
-            "sku": "20_04-lts-gen2",
-            "version": "latest"
-        },
-        "osDisk": {
-            "caching": "ReadWrite",
-            "createOption": "FromImage",
-            "diffDiskSettings": {
-                "option": ""
-            },
-            "diskSizeGB": "30",
-            "encryptionSettings": {
-                "enabled": "false",
-                "diskEncryptionKey": {
-                    "sourceVault": {
-                        "id": "/subscriptions/test-source-guid/resourceGroups/testrg/providers/Microsoft.KeyVault/vaults/test-kv"
-                    },
-                    "secretUrl": "https://test-disk.vault.azure.net/secrets/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx"
-                },
-                "keyEncryptionKey": {
-                    "sourceVault": {
-                        "id": "/subscriptions/test-key-guid/resourceGroups/testrg/providers/Microsoft.KeyVault/vaults/test-kv"
-                    },
-                    "keyUrl": "https://test-key.vault.azure.net/secrets/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx"
-                }
-            },
-            "image": {
-                "uri": ""
-            },
-            "managedDisk": {
-                "id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/disks/exampleosdiskname",
-                "storageAccountType": "StandardSSD_LRS"
-            },
-            "name": "exampledatadiskname",
-            "osType": "Linux",
-            "vhd": {
-                "uri": ""
-            },
-            "writeAcceleratorEnabled": "false"
-        },
-        "resourceDisk": {
-            "size": "16384"
-        }
-    },
-    "subscriptionId": "xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx",
-    "tags": "azsecpack:nonprod;platformsettings.host_environment.service.platform_optedin_for_rootcerts:true",
-    "tagsList": [
-        {
-            "name": "azsecpack",
-            "value": "nonprod"
-        },
-        {
-            "name": "platformsettings.host_environment.service.platform_optedin_for_rootcerts",
-            "value": "true"
-        }
-    ],
-    "userData": "",
-    "version": "20.04.202307240",
-    "virtualMachineScaleSet": {
-        "id": "/subscriptions/xxxxxxxx-xxxxx-xxx-xxx-xxxx/resourceGroups/resource-group-name/providers/Microsoft.Compute/virtualMachineScaleSets/virtual-machine-scale-set-name"
-    },
-    "vmId": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
-    "vmScaleSetName": "crpteste9vflji9",
-    "vmSize": "Standard_A3",
-    "zone": "1"
-}
-"""
-WINDOWS_JSON = """
-{
-    "additionalCapabilities": {
-        "hibernationEnabled": "false"
-    },
-    "azEnvironment": "AzurePublicCloud",
-    "customData": "",
-    "evictionPolicy": "",
-    "extendedLocation": {
-        "name": "",
-        "type": ""
-    },
-    "host": {
-        "id": ""
-    },
-    "hostGroup": {
-        "id": ""
-    },
-    "isHostCompatibilityLayerVm": "true",
-    "licenseType": "Windows_Client",
-    "location": "westus",
-    "name": "examplevmname",
-    "offer": "WindowsServer",
-    "osProfile": {
-        "adminUsername": "azureuser",
-        "computerName": "examplevmname",
-        "disablePasswordAuthentication": "true"
-    },
-    "osType": "Windows",
-    "placementGroupId": "",
-    "plan": {
-        "name": "",
-        "product": "",
-        "publisher": ""
-    },
-    "platformFaultDomain": "0",
-    "platformSubFaultDomain": "",
-    "platformUpdateDomain": "0",
-    "priority": "",
-    "provider": "Microsoft.Compute",
-    "publicKeys": [
-        {
-            "keyData": "ssh-rsa 0",
-            "path": "/home/user/.ssh/authorized_keys0"
-        },
-        {
-            "keyData": "ssh-rsa 1",
-            "path": "/home/user/.ssh/authorized_keys1"
-        }
-    ],
-    "publisher": "RDFE-Test-Microsoft-Windows-Server-Group",
-    "resourceGroupName": "macikgo-test-may-23",
-    "resourceId": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/virtualMachines/examplevmname",
-    "securityProfile": {
-        "encryptionAtHost": "false",
-        "secureBootEnabled": "true",
-        "securityType": "TrustedLaunch",
-        "virtualTpmEnabled": "true"
-    },
-    "sku": "2019-Datacenter",
-    "storageProfile": {
-        "dataDisks": [
-            {
-                "bytesPerSecondThrottle": "979202048",
-                "caching": "None",
-                "createOption": "Empty",
-                "diskCapacityBytes": "274877906944",
-                "diskSizeGB": "1024",
-                "image": {
-                    "uri": ""
-                },
-                "isSharedDisk": "false",
-                "isUltraDisk": "true",
-                "lun": "0",
-                "managedDisk": {
-                    "id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/disks/exampledatadiskname",
-                    "storageAccountType": "StandardSSD_LRS"
-                },
-                "name": "exampledatadiskname",
-                "opsPerSecondThrottle": "65280",
-                "vhd": {
-                    "uri": ""
-                },
-                "writeAcceleratorEnabled": "false"
-            }
-        ],
-        "imageReference": {
-            "id": "",
-            "offer": "WindowsServer",
-            "publisher": "MicrosoftWindowsServer",
-            "sku": "2019-Datacenter",
-            "version": "latest"
-        },
-        "osDisk": {
-            "caching": "ReadWrite",
-            "createOption": "FromImage",
-            "diffDiskSettings": {
-                "option": ""
-            },
-            "diskSizeGB": "30",
-            "encryptionSettings": {
-                "enabled": "false",
-                "diskEncryptionKey": {
-                    "sourceVault": {
-                        "id": "/subscriptions/test-source-guid/resourceGroups/testrg/providers/Microsoft.KeyVault/vaults/test-kv"
-                    },
-                    "secretUrl": "https://test-disk.vault.azure.net/secrets/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx"
-                },
-                "keyEncryptionKey": {
-                    "sourceVault": {
-                        "id": "/subscriptions/test-key-guid/resourceGroups/testrg/providers/Microsoft.KeyVault/vaults/test-kv"
-                    },
-                    "keyUrl": "https://test-key.vault.azure.net/secrets/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx"
-                }
-            },
-            "image": {
-                "uri": ""
-            },
-            "managedDisk": {
-                "id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/disks/exampleosdiskname",
-                "storageAccountType": "StandardSSD_LRS"
-            },
-            "name": "exampledatadiskname",
-            "osType": "Windows",
-            "vhd": {
-                "uri": ""
-            },
-            "writeAcceleratorEnabled": "false"
-        },
-        "resourceDisk": {
-            "size": "16384"
-        }
-    },
-    "subscriptionId": "xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx",
-    "tags": "azsecpack:nonprod;platformsettings.host_environment.service.platform_optedin_for_rootcerts:true",
-    "userData": "Zm9vYmFy",
-    "tagsList": [
-        {
-            "name": "azsecpack",
-            "value": "nonprod"
-        },
-        {
-            "name": "platformsettings.host_environment.service.platform_optedin_for_rootcerts",
-            "value": "true"
-        }
-    ],
-    "userData": "",
-    "version": "20.04.202307240",
-    "virtualMachineScaleSet": {
-        "id": "/subscriptions/xxxxxxxx-xxxxx-xxx-xxx-xxxx/resourceGroups/resource-group-name/providers/Microsoft.Compute/virtualMachineScaleSets/virtual-machine-scale-set-name"
-    },
-    "vmId": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
-    "vmScaleSetName": "crpteste9vflji9",
-    "vmSize": "Standard_A3",
-    "zone": "1"
-}
-"""
-LINUX_ATTRIBUTES = {
-    "azure.vm.scaleset.name": "crpteste9vflji9",
-    "azure.vm.sku": "20_04-lts-gen2",
-    "cloud.platform": "azure_vm",
-    "cloud.provider": "azure",
-    "cloud.region": "westus",
-    "cloud.resource_id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/virtualMachines/examplevmname",
-    "host.id": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
-    "host.name": "examplevmname",
-    "host.type": "Standard_A3",
-    "os.type": "Linux",
-    "os.version": "20.04.202307240",
-    "service.instance.id": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
-}
-WINDOWS_ATTRIBUTES = {
-    "azure.vm.scaleset.name": "crpteste9vflji9",
-    "azure.vm.sku": "2019-Datacenter",
-    "cloud.platform": "azure_vm",
-    "cloud.provider": "azure",
-    "cloud.region": "westus",
-    "cloud.resource_id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/virtualMachines/examplevmname",
-    "host.id": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
-    "host.name": "examplevmname",
-    "host.type": "Standard_A3",
-    "os.type": "Windows",
-    "os.version": "20.04.202307240",
-    "service.instance.id": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
-}
-
-
-class TestAzureVMResourceDetector(unittest.TestCase):
-    @patch("opentelemetry.resource.detector.azure.vm.urlopen")
-    def test_linux(self, mock_urlopen):
-        mock_urlopen.return_value.__enter__.return_value.read.return_value = (
-            LINUX_JSON
-        )
-        attributes = AzureVMResourceDetector().detect().attributes
-        for attribute_key, attribute_value in LINUX_ATTRIBUTES.items():
-            self.assertEqual(attributes[attribute_key], attribute_value)
-
-    @patch("opentelemetry.resource.detector.azure.vm.urlopen")
-    def test_windows(self, mock_urlopen):
-        mock_urlopen.return_value.__enter__.return_value.read.return_value = (
-            WINDOWS_JSON
-        )
-        attributes = AzureVMResourceDetector().detect().attributes
-        for attribute_key, attribute_value in WINDOWS_ATTRIBUTES.items():
-            self.assertEqual(attributes[attribute_key], attribute_value)
+# Copyright The OpenTelemetry Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import unittest
+from unittest.mock import patch
+
+# pylint: disable=no-name-in-module
+from opentelemetry.resource.detector.azure.vm import AzureVMResourceDetector
+
+LINUX_JSON = """
+{
+    "additionalCapabilities": {
+        "hibernationEnabled": "false"
+    },
+    "azEnvironment": "AzurePublicCloud",
+    "customData": "",
+    "evictionPolicy": "",
+    "extendedLocation": {
+        "name": "",
+        "type": ""
+    },
+    "host": {
+        "id": ""
+    },
+    "hostGroup": {
+        "id": ""
+    },
+    "isHostCompatibilityLayerVm": "true",
+    "licenseType": "",
+    "location": "westus",
+    "name": "examplevmname",
+    "offer": "0001-com-ubuntu-server-focal",
+    "osProfile": {
+        "adminUsername": "azureuser",
+        "computerName": "examplevmname",
+        "disablePasswordAuthentication": "true"
+    },
+    "osType": "Linux",
+    "placementGroupId": "",
+    "plan": {
+        "name": "",
+        "product": "",
+        "publisher": ""
+    },
+    "platformFaultDomain": "0",
+    "platformSubFaultDomain": "",
+    "platformUpdateDomain": "0",
+    "priority": "",
+    "provider": "Microsoft.Compute",
+    "publicKeys": [
+        {
+            "keyData": "ssh-rsa 0",
+            "path": "/home/user/.ssh/authorized_keys0"
+        },
+        {
+            "keyData": "ssh-rsa 1",
+            "path": "/home/user/.ssh/authorized_keys1"
+        }
+    ],
+    "publisher": "canonical",
+    "resourceGroupName": "macikgo-test-may-23",
+    "resourceId": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/virtualMachines/examplevmname",
+    "securityProfile": {
+        "encryptionAtHost": "false",
+        "secureBootEnabled": "true",
+        "securityType": "TrustedLaunch",
+        "virtualTpmEnabled": "true"
+    },
+    "sku": "20_04-lts-gen2",
+    "storageProfile": {
+        "dataDisks": [
+            {
+                "bytesPerSecondThrottle": "979202048",
+                "caching": "None",
+                "createOption": "Empty",
+                "diskCapacityBytes": "274877906944",
+                "diskSizeGB": "1024",
+                "image": {
+                    "uri": ""
+                },
+                "isSharedDisk": "false",
+                "isUltraDisk": "true",
+                "lun": "0",
+                "managedDisk": {
+                    "id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/disks/exampledatadiskname",
+                    "storageAccountType": "StandardSSD_LRS"
+                },
+                "name": "exampledatadiskname",
+                "opsPerSecondThrottle": "65280",
+                "vhd": {
+                    "uri": ""
+                },
+                "writeAcceleratorEnabled": "false"
+            }
+        ],
+        "imageReference": {
+            "id": "",
+            "offer": "0001-com-ubuntu-server-focal",
+            "publisher": "canonical",
+            "sku": "20_04-lts-gen2",
+            "version": "latest"
+        },
+        "osDisk": {
+            "caching": "ReadWrite",
+            "createOption": "FromImage",
+            "diffDiskSettings": {
+                "option": ""
+            },
+            "diskSizeGB": "30",
+            "encryptionSettings": {
+                "enabled": "false",
+                "diskEncryptionKey": {
+                    "sourceVault": {
+                        "id": "/subscriptions/test-source-guid/resourceGroups/testrg/providers/Microsoft.KeyVault/vaults/test-kv"
+                    },
+                    "secretUrl": "https://test-disk.vault.azure.net/secrets/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx"
+                },
+                "keyEncryptionKey": {
+                    "sourceVault": {
+                        "id": "/subscriptions/test-key-guid/resourceGroups/testrg/providers/Microsoft.KeyVault/vaults/test-kv"
+                    },
+                    "keyUrl": "https://test-key.vault.azure.net/secrets/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx"
+                }
+            },
+            "image": {
+                "uri": ""
+            },
+            "managedDisk": {
+                "id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/disks/exampleosdiskname",
+                "storageAccountType": "StandardSSD_LRS"
+            },
+            "name": "exampledatadiskname",
+            "osType": "Linux",
+            "vhd": {
+                "uri": ""
+            },
+            "writeAcceleratorEnabled": "false"
+        },
+        "resourceDisk": {
+            "size": "16384"
+        }
+    },
+    "subscriptionId": "xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx",
+    "tags": "azsecpack:nonprod;platformsettings.host_environment.service.platform_optedin_for_rootcerts:true",
+    "tagsList": [
+        {
+            "name": "azsecpack",
+            "value": "nonprod"
+        },
+        {
+            "name": "platformsettings.host_environment.service.platform_optedin_for_rootcerts",
+            "value": "true"
+        }
+    ],
+    "userData": "",
+    "version": "20.04.202307240",
+    "virtualMachineScaleSet": {
+        "id": "/subscriptions/xxxxxxxx-xxxxx-xxx-xxx-xxxx/resourceGroups/resource-group-name/providers/Microsoft.Compute/virtualMachineScaleSets/virtual-machine-scale-set-name"
+    },
+    "vmId": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
+    "vmScaleSetName": "crpteste9vflji9",
+    "vmSize": "Standard_A3",
+    "zone": "1"
+}
+"""
+WINDOWS_JSON = """
+{
+    "additionalCapabilities": {
+        "hibernationEnabled": "false"
+    },
+    "azEnvironment": "AzurePublicCloud",
+    "customData": "",
+    "evictionPolicy": "",
+    "extendedLocation": {
+        "name": "",
+        "type": ""
+    },
+    "host": {
+        "id": ""
+    },
+    "hostGroup": {
+        "id": ""
+    },
+    "isHostCompatibilityLayerVm": "true",
+    "licenseType": "Windows_Client",
+    "location": "westus",
+    "name": "examplevmname",
+    "offer": "WindowsServer",
+    "osProfile": {
+        "adminUsername": "azureuser",
+        "computerName": "examplevmname",
+        "disablePasswordAuthentication": "true"
+    },
+    "osType": "Windows",
+    "placementGroupId": "",
+    "plan": {
+        "name": "",
+        "product": "",
+        "publisher": ""
+    },
+    "platformFaultDomain": "0",
+    "platformSubFaultDomain": "",
+    "platformUpdateDomain": "0",
+    "priority": "",
+    "provider": "Microsoft.Compute",
+    "publicKeys": [
+        {
+            "keyData": "ssh-rsa 0",
+            "path": "/home/user/.ssh/authorized_keys0"
+        },
+        {
+            "keyData": "ssh-rsa 1",
+            "path": "/home/user/.ssh/authorized_keys1"
+        }
+    ],
+    "publisher": "RDFE-Test-Microsoft-Windows-Server-Group",
+    "resourceGroupName": "macikgo-test-may-23",
+    "resourceId": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/virtualMachines/examplevmname",
+    "securityProfile": {
+        "encryptionAtHost": "false",
+        "secureBootEnabled": "true",
+        "securityType": "TrustedLaunch",
+        "virtualTpmEnabled": "true"
+    },
+    "sku": "2019-Datacenter",
+    "storageProfile": {
+        "dataDisks": [
+            {
+                "bytesPerSecondThrottle": "979202048",
+                "caching": "None",
+                "createOption": "Empty",
+                "diskCapacityBytes": "274877906944",
+                "diskSizeGB": "1024",
+                "image": {
+                    "uri": ""
+                },
+                "isSharedDisk": "false",
+                "isUltraDisk": "true",
+                "lun": "0",
+                "managedDisk": {
+                    "id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/disks/exampledatadiskname",
+                    "storageAccountType": "StandardSSD_LRS"
+                },
+                "name": "exampledatadiskname",
+                "opsPerSecondThrottle": "65280",
+                "vhd": {
+                    "uri": ""
+                },
+                "writeAcceleratorEnabled": "false"
+            }
+        ],
+        "imageReference": {
+            "id": "",
+            "offer": "WindowsServer",
+            "publisher": "MicrosoftWindowsServer",
+            "sku": "2019-Datacenter",
+            "version": "latest"
+        },
+        "osDisk": {
+            "caching": "ReadWrite",
+            "createOption": "FromImage",
+            "diffDiskSettings": {
+                "option": ""
+            },
+            "diskSizeGB": "30",
+            "encryptionSettings": {
+                "enabled": "false",
+                "diskEncryptionKey": {
+                    "sourceVault": {
+                        "id": "/subscriptions/test-source-guid/resourceGroups/testrg/providers/Microsoft.KeyVault/vaults/test-kv"
+                    },
+                    "secretUrl": "https://test-disk.vault.azure.net/secrets/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx"
+                },
+                "keyEncryptionKey": {
+                    "sourceVault": {
+                        "id": "/subscriptions/test-key-guid/resourceGroups/testrg/providers/Microsoft.KeyVault/vaults/test-kv"
+                    },
+                    "keyUrl": "https://test-key.vault.azure.net/secrets/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx"
+                }
+            },
+            "image": {
+                "uri": ""
+            },
+            "managedDisk": {
+                "id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/disks/exampleosdiskname",
+                "storageAccountType": "StandardSSD_LRS"
+            },
+            "name": "exampledatadiskname",
+            "osType": "Windows",
+            "vhd": {
+                "uri": ""
+            },
+            "writeAcceleratorEnabled": "false"
+        },
+        "resourceDisk": {
+            "size": "16384"
+        }
+    },
+    "subscriptionId": "xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx",
+    "tags": "azsecpack:nonprod;platformsettings.host_environment.service.platform_optedin_for_rootcerts:true",
+    "userData": "Zm9vYmFy",
+    "tagsList": [
+        {
+            "name": "azsecpack",
+            "value": "nonprod"
+        },
+        {
+            "name": "platformsettings.host_environment.service.platform_optedin_for_rootcerts",
+            "value": "true"
+        }
+    ],
+    "userData": "",
+    "version": "20.04.202307240",
+    "virtualMachineScaleSet": {
+        "id": "/subscriptions/xxxxxxxx-xxxxx-xxx-xxx-xxxx/resourceGroups/resource-group-name/providers/Microsoft.Compute/virtualMachineScaleSets/virtual-machine-scale-set-name"
+    },
+    "vmId": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
+    "vmScaleSetName": "crpteste9vflji9",
+    "vmSize": "Standard_A3",
+    "zone": "1"
+}
+"""
+LINUX_ATTRIBUTES = {
+    "azure.vm.scaleset.name": "crpteste9vflji9",
+    "azure.vm.sku": "20_04-lts-gen2",
+    "cloud.platform": "azure_vm",
+    "cloud.provider": "azure",
+    "cloud.region": "westus",
+    "cloud.resource_id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/virtualMachines/examplevmname",
+    "host.id": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
+    "host.name": "examplevmname",
+    "host.type": "Standard_A3",
+    "os.type": "Linux",
+    "os.version": "20.04.202307240",
+    "service.instance.id": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
+}
+WINDOWS_ATTRIBUTES = {
+    "azure.vm.scaleset.name": "crpteste9vflji9",
+    "azure.vm.sku": "2019-Datacenter",
+    "cloud.platform": "azure_vm",
+    "cloud.provider": "azure",
+    "cloud.region": "westus",
+    "cloud.resource_id": "/subscriptions/xxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx/resourceGroups/macikgo-test-may-23/providers/Microsoft.Compute/virtualMachines/examplevmname",
+    "host.id": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
+    "host.name": "examplevmname",
+    "host.type": "Standard_A3",
+    "os.type": "Windows",
+    "os.version": "20.04.202307240",
+    "service.instance.id": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
+}
+
+
+class TestAzureVMResourceDetector(unittest.TestCase):
+    @patch("opentelemetry.resource.detector.azure.vm.urlopen")
+    def test_linux(self, mock_urlopen):
+        mock_urlopen.return_value.__enter__.return_value.read.return_value = (
+            LINUX_JSON
+        )
+        attributes = AzureVMResourceDetector().detect().attributes
+        for attribute_key, attribute_value in LINUX_ATTRIBUTES.items():
+            self.assertEqual(attributes[attribute_key], attribute_value)
+
+    @patch("opentelemetry.resource.detector.azure.vm.urlopen")
+    def test_windows(self, mock_urlopen):
+        mock_urlopen.return_value.__enter__.return_value.read.return_value = (
+            WINDOWS_JSON
+        )
+        attributes = AzureVMResourceDetector().detect().attributes
+        for attribute_key, attribute_value in WINDOWS_ATTRIBUTES.items():
+            self.assertEqual(attributes[attribute_key], attribute_value)
+
+    @patch("opentelemetry.resource.detector.azure.vm._can_ignore_vm_detect")
+    @patch("opentelemetry.resource.detector.azure.vm.urlopen")
+    def test_in_another_rp(self, mock_urlopen, detect_mock):
+        mock_urlopen.return_value.__enter__.return_value.read.return_value = (
+            LINUX_JSON
+        )
+        detect_mock.return_value = True
+        attributes = AzureVMResourceDetector().detect().attributes
+        self.assertEqual(attributes, {})
```

### Comparing `opentelemetry_resource_detector_azure-0.1.4/LICENSE` & `opentelemetry_resource_detector_azure-0.1.5/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright The OpenTelemetry Authors
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `opentelemetry_resource_detector_azure-0.1.4/pyproject.toml` & `opentelemetry_resource_detector_azure-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "opentelemetry-resource-detector-azure"
-dynamic = ["version"]
-description = "Azure Resource Detector for OpenTelemetry"
-readme = "README.rst"
-license = "Apache-2.0"
-requires-python = ">=3.8"
-authors = [
-  { name = "OpenTelemetry Authors", email = "cncf-opentelemetry-contributors@lists.cncf.io" },
-]
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Intended Audience :: Developers",
-  "License :: OSI Approved :: Apache Software License",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-]
-dependencies = [
-  "opentelemetry-sdk ~= 1.21",
-]
-
-[project.entry-points.opentelemetry_resource_detector]
-azure_app_service = "opentelemetry.resource.detector.azure.app_service:AzureAppServiceResourceDetector"
-azure_vm = "opentelemetry.resource.detector.azure.vm:AzureVMResourceDetector"
-
-[project.urls]
-Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/resource/opentelemetry-resource-detector-azure"
-
-[tool.hatch.version]
-path = "src/opentelemetry/resource/detector/azure/version.py"
-
-[tool.hatch.build.targets.sdist]
-include = [
-  "/src",
-  "/tests",
-]
-
-[tool.hatch.build.targets.wheel]
-packages = ["src/opentelemetry"]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "opentelemetry-resource-detector-azure"
+dynamic = ["version"]
+description = "Azure Resource Detector for OpenTelemetry"
+readme = "README.rst"
+license = "Apache-2.0"
+requires-python = ">=3.8"
+authors = [
+  { name = "OpenTelemetry Authors", email = "cncf-opentelemetry-contributors@lists.cncf.io" },
+]
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: Apache Software License",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+]
+dependencies = [
+  "opentelemetry-sdk ~= 1.21",
+]
+
+[project.entry-points.opentelemetry_resource_detector]
+azure_app_service = "opentelemetry.resource.detector.azure.app_service:AzureAppServiceResourceDetector"
+azure_functions = "opentelemetry.resource.detector.azure.functions:AzureFunctionsResourceDetector"
+azure_vm = "opentelemetry.resource.detector.azure.vm:AzureVMResourceDetector"
+
+[project.urls]
+Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/resource/opentelemetry-resource-detector-azure"
+
+[tool.hatch.version]
+path = "src/opentelemetry/resource/detector/azure/version.py"
+
+[tool.hatch.build.targets.sdist]
+include = [
+  "/src",
+  "/tests",
+]
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/opentelemetry"]
```

### Comparing `opentelemetry_resource_detector_azure-0.1.4/PKG-INFO` & `opentelemetry_resource_detector_azure-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opentelemetry-resource-detector-azure
-Version: 0.1.4
+Version: 0.1.5
 Summary: Azure Resource Detector for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/resource/opentelemetry-resource-detector-azure
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -77,15 +77,25 @@
  * ``cloud.resource_id`` set using the ``WEBSITE_RESOURCE_GROUP``, ``WEBSITE_OWNER_NAME``, and ``WEBSITE_SITE_NAME`` environment variables.
  * ``cloud.region`` set to the value of the ``REGION_NAME`` environment variable.
  * ``deployment.environment`` set to the value of the ``WEBSITE_SLOT_NAME`` environment variable.
  * ``host.id`` set to the value of the ``WEBSITE_HOSTNAME`` environment variable.
  * ``service.instance.id`` set to the value of the ``WEBSITE_INSTANCE_ID`` environment variable.
  * ``azure.app.service.stamp`` set to the value of the ``WEBSITE_HOME_STAMPNAME`` environment variable.
 
-The Azure VM Resource Detector sets the following Resource Attributes according to the response from the `Azure Metadata Service <https://learn.microsoft.com/en-us/azure/virtual-machines/instance-metadata-service?tabs=windows>`_:
+ The Azure Functions Resource Detector sets the following Resource Attributes:
+ * ``service.name`` set to the value of the ``WEBSITE_SITE_NAME`` environment variable.
+ * ``process.id`` set to the process ID collected from the running process.
+ * ``cloud.platform`` set to ``azure_functions``.
+ * ``cloud.provider`` set to ``azure``.
+ * ``cloud.resource_id`` set using the ``WEBSITE_RESOURCE_GROUP``, ``WEBSITE_OWNER_NAME``, and ``WEBSITE_SITE_NAME`` environment variables.
+ * ``cloud.region`` set to the value of the ``REGION_NAME`` environment variable.
+ * ``faas.instance`` set to the value of the ``WEBSITE_INSTANCE_ID`` environment variable.
+ * ``faas.max_memory`` set to the value of the ``WEBSITE_MEMORY_LIMIT_MB`` environment variable.
+
+The Azure VM Resource Detector sets the following Resource Attributes according to the response from the `Azure Metadata Service <https://learn.microsoft.com/azure/virtual-machines/instance-metadata-service?tabs=windows>`_:
  * ``azure.vm.scaleset.name`` set to the value of the ``vmScaleSetName`` field.
  * ``azure.vm.sku`` set to the value of the ``sku`` field.
  * ``cloud.platform`` set to the value of the ``azure_vm``.
  * ``cloud.provider`` set to the value of the ``azure``.
  * ``cloud.region`` set to the value of the ``location`` field.
  * ``cloud.resource_id`` set to the value of the ``resourceId`` field.
  * ``host.id`` set to the value of the ``vmId`` field.
```

