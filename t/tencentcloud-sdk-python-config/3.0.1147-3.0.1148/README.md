# Comparing `tmp/tencentcloud-sdk-python-config-3.0.1147.tar.gz` & `tmp/tencentcloud-sdk-python-config-3.0.1148.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-config-3.0.1147.tar", last modified: Wed May 15 21:14:44 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-config-3.0.1148.tar", last modified: Thu May 16 08:09:46 2024, max compression
```

## Comparing `tencentcloud-sdk-python-config-3.0.1147.tar` & `tencentcloud-sdk-python-config-3.0.1148.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/
--rw-r--r--   0 root         (0) root         (0)      746 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud_sdk_python_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud_sdk_python_config.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud_sdk_python_config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1675 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud_sdk_python_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud_sdk_python_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      528 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud_sdk_python_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/v20220802/
--rw-r--r--   0 root         (0) root         (0)    40671 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/v20220802/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/v20220802/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/v20220802/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3670 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/v20220802/config_client.py
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1079 2024-05-15 21:14:44.000000 tencentcloud-sdk-python-config-3.0.1147/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-16 08:09:45.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 08:09:45.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/v20220802/
+-rw-r--r--   0 root         (0) root         (0)     3670 2024-05-16 08:09:45.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/v20220802/config_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 08:09:45.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/v20220802/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2024-05-16 08:09:45.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/v20220802/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    40671 2024-05-16 08:09:45.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/v20220802/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud_sdk_python_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud_sdk_python_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud_sdk_python_config.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud_sdk_python_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      528 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud_sdk_python_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/tencentcloud_sdk_python_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2024-05-16 08:09:45.000000 tencentcloud-sdk-python-config-3.0.1148/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1079 2024-05-16 08:09:45.000000 tencentcloud-sdk-python-config-3.0.1148/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-05-16 08:09:46.000000 tencentcloud-sdk-python-config-3.0.1148/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-config-3.0.1147/README.rst` & `tencentcloud-sdk-python-config-3.0.1148/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-config-3.0.1147/tencentcloud_sdk_python_config.egg-info/PKG-INFO` & `tencentcloud-sdk-python-config-3.0.1148/tencentcloud_sdk_python_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-config
-Version: 3.0.1147
+Version: 3.0.1148
 Summary: Tencent Cloud Config SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-config-3.0.1147/tencentcloud_sdk_python_config.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-config-3.0.1148/tencentcloud_sdk_python_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/v20220802/models.py` & `tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/v20220802/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/v20220802/errorcodes.py` & `tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/v20220802/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-config-3.0.1147/tencentcloud/config/v20220802/config_client.py` & `tencentcloud-sdk-python-config-3.0.1148/tencentcloud/config/v20220802/config_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-config-3.0.1147/tencentcloud/__init__.py` & `tencentcloud-sdk-python-config-3.0.1148/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1147'
+__version__ = '3.0.1148'
```

### Comparing `tencentcloud-sdk-python-config-3.0.1147/PKG-INFO` & `tencentcloud-sdk-python-config-3.0.1148/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-config
-Version: 3.0.1147
+Version: 3.0.1148
 Summary: Tencent Cloud Config SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-config-3.0.1147/setup.py` & `tencentcloud-sdk-python-config-3.0.1148/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-config',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1147"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1148"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Config SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```
