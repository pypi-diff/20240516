# Comparing `tmp/dapr-ext-workflow-0.4.0.tar.gz` & `tmp/dapr-ext-workflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapr-ext-workflow-0.4.0.tar", last modified: Tue Feb 13 03:56:27 2024, max compression
+gzip compressed data, was "dapr-ext-workflow-0.4.1.tar", last modified: Thu May 16 01:55:00 2024, max compression
```

## Comparing `dapr-ext-workflow-0.4.0.tar` & `dapr-ext-workflow-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 03:56:27.283814 dapr-ext-workflow-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-13 03:56:27.283814 dapr-ext-workflow-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 03:56:27.279814 dapr-ext-workflow-0.4.0/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 03:56:27.279814 dapr-ext-workflow-0.4.0/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 03:56:27.283814 dapr-ext-workflow-0.4.0/dapr/ext/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/dapr_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/dapr_workflow_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 03:56:27.283814 dapr-ext-workflow-0.4.0/dapr/ext/workflow/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/logger/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/retry_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/workflow_activity_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/workflow_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/dapr/ext/workflow/workflow_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 03:56:27.283814 dapr-ext-workflow-0.4.0/dapr_ext_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-13 03:56:27.000000 dapr-ext-workflow-0.4.0/dapr_ext_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-13 03:56:27.000000 dapr-ext-workflow-0.4.0/dapr_ext_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 03:56:27.000000 dapr-ext-workflow-0.4.0/dapr_ext_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-13 03:56:27.000000 dapr-ext-workflow-0.4.0/dapr_ext_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-13 03:56:27.000000 dapr-ext-workflow-0.4.0/dapr_ext_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-13 03:56:27.283814 dapr-ext-workflow-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-13 03:56:17.000000 dapr-ext-workflow-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:55:00.715180 dapr-ext-workflow-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-16 01:55:00.715180 dapr-ext-workflow-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:55:00.711180 dapr-ext-workflow-0.4.1/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:55:00.711180 dapr-ext-workflow-0.4.1/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:55:00.715180 dapr-ext-workflow-0.4.1/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/dapr_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/dapr_workflow_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:55:00.715180 dapr-ext-workflow-0.4.1/dapr/ext/workflow/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/logger/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/retry_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/workflow_activity_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/workflow_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/dapr/ext/workflow/workflow_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:55:00.715180 dapr-ext-workflow-0.4.1/dapr_ext_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-16 01:55:00.000000 dapr-ext-workflow-0.4.1/dapr_ext_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-16 01:55:00.000000 dapr-ext-workflow-0.4.1/dapr_ext_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:55:00.000000 dapr-ext-workflow-0.4.1/dapr_ext_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 01:55:00.000000 dapr-ext-workflow-0.4.1/dapr_ext_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 01:55:00.000000 dapr-ext-workflow-0.4.1/dapr_ext_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 01:55:00.715180 dapr-ext-workflow-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-16 01:54:51.000000 dapr-ext-workflow-0.4.1/setup.py
```

### Comparing `dapr-ext-workflow-0.4.0/LICENSE` & `dapr-ext-workflow-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/PKG-INFO` & `dapr-ext-workflow-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapr-ext-workflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: The official release of Dapr Python SDK Workflow Authoring Extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/dapr_workflow_client.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/dapr_workflow_client.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/dapr_workflow_context.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/dapr_workflow_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/logger/logger.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/logger/logger.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/logger/options.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/logger/options.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/retry_policy.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/retry_policy.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/util.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/util.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/version.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
```

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/workflow_activity_context.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/workflow_activity_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/workflow_context.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/workflow_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/workflow_runtime.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/workflow_runtime.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr/ext/workflow/workflow_state.py` & `dapr-ext-workflow-0.4.1/dapr/ext/workflow/workflow_state.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/dapr_ext_workflow.egg-info/PKG-INFO` & `dapr-ext-workflow-0.4.1/dapr_ext_workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapr-ext-workflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: The official release of Dapr Python SDK Workflow Authoring Extension.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-0.4.0/dapr_ext_workflow.egg-info/SOURCES.txt` & `dapr-ext-workflow-0.4.1/dapr_ext_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-0.4.0/setup.cfg` & `dapr-ext-workflow-0.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	Source = https://github.com/dapr/python-sdk
 
 [options]
 python_requires = >=3.8
 packages = find_namespace:
 include_package_data = True
 install_requires = 
-	dapr >= 1.13.0rc1
+	dapr >= 1.13.0
 	durabletask >= 0.1.1a1
 
 [options.packages.find]
 include = 
 	dapr.*
 exclude = 
 	tests
```

### Comparing `dapr-ext-workflow-0.4.0/setup.py` & `dapr-ext-workflow-0.4.1/setup.py`

 * *Files identical despite different names*

