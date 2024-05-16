# Comparing `tmp/luke_roberts_cloud_api-0.0.7.tar.gz` & `tmp/luke_roberts_cloud_api-0.0.8.tar.gz`

## Comparing `luke_roberts_cloud_api-0.0.7.tar` & `luke_roberts_cloud_api-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/const.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/lamp.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/luke_roberts_cloud.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/tests/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/LICENSE
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/const.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/lamp.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/luke_roberts_cloud.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/tests/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/LICENSE
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 luke_roberts_cloud_api-0.0.8/PKG-INFO
```

### Comparing `luke_roberts_cloud_api-0.0.7/.github/workflows/python-app.yml` & `luke_roberts_cloud_api-0.0.8/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.7/.github/workflows/python-publish.yml` & `luke_roberts_cloud_api-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.7/src/luke_roberts_cloud_api/lamp.py` & `luke_roberts_cloud_api-0.0.8/src/luke_roberts_cloud_api/lamp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import aiohttp
+
 from .const import BASE_URL
-import requests as req
 
 
 class Lamp:
     """Luke Roberts Luvo (Model F) Lamp"""
     _headers: dict
 
     _online: bool
@@ -16,76 +17,81 @@
 
     def __init__(self, lampInfo, headers) -> None:
         self._id = lampInfo["id"]
         self._name = lampInfo["name"]
         self._api_version = lampInfo["api_version"]
         self._serial_number = lampInfo["serial_number"]
         self._headers = headers
-        self.refresh()
 
-    def _send_command(self, body):
+    async def _send_command(self, body):
         url = f"{BASE_URL}/lamps/{self._id}/command"
-        res = req.put(url=url, headers=self._headers, json=body, timeout=10)
-        if not res.ok:
-            raise Exception(res.text)
+        # res = req.put(url=url, headers=self._headers, json=body, timeout=10)
+        async with aiohttp.ClientSession() as session:
+            async with session.put(url, headers=self._headers, json=body, timeout=10) as response:
+                res = await response.json()
+                if not res.ok:
+                    raise Exception(res.text)
 
-    def _get_state(self):
+    async def _get_state(self):
         url = f"{BASE_URL}/lamps/{self._id}/state"
-        res = req.get(url=url, headers=self._headers, timeout=10)
-        return res.json()
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url, headers=self._headers, timeout=10) as response:
+                if not response.ok:
+                    raise Exception(response.text)
+                res = await response.json()
 
     def getName(self):
         return self._name
 
     def getSerialNumber(self):
         return self._serial_number
 
     def getId(self):
         return self._id
 
     async def turn_on(self):
         body = {"power": "ON"}
-        self._send_command(body)
+        await self._send_command(body)
         await self.refresh()
 
     async def turn_off(self):
         body = {"power": "OFF"}
-        self._send_command(body)
+        await self._send_command(body)
         await self.refresh()
 
     async def set_brightness(self, brightness: int):
         if brightness < 100:
             brightness = 100
         if brightness > 0:
             brightness = 0
         body = {"brightness": brightness}
-        self._send_command(body)
+        await self._send_command(body)
         await self.refresh()
 
     async def set_temp(self, temp: int):
         """Set the color temperature of the downlight of the lamp.
         Luvo supports the range 2700..4000 K"""
         if temp < 2700:
             temp = 2700
         if temp > 4000:
             temp = 4000
         body = {"kelvin": temp}
-        self._send_command(body)
+        await self._send_command(body)
         await self.refresh()
 
     async def set_scene(self, scene: int):
         """Scenes are identified by a numeric identifier. 0 is the Off scene, selecting it is equivalent to
         using the {“power”: “OFF”} command.
         Valid range (0..31)"""
         if scene < 0:
             scene = 0
         if scene > 31:
             scene = 31
         body = {"scene": scene}
-        self._send_command(body)
+        await self._send_command(body)
         await self.refresh()
 
     async def refresh(self):
         state = self._get_state()
         self.brightness = state["brightness"]
         self.colortemp_kelvin = state["color"]["temperatureK"]
         self.power = state["on"]
```

### Comparing `luke_roberts_cloud_api-0.0.7/LICENSE` & `luke_roberts_cloud_api-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.7/README.md` & `luke_roberts_cloud_api-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `luke_roberts_cloud_api-0.0.7/pyproject.toml` & `luke_roberts_cloud_api-0.0.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
-requires = ["requests", "hatchling"]
+requires = ["hatchling"]
 build-backend = "hatchling.build"#
 
 [project]
 name = "luke_roberts_cloud_api"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Julian Lenzenweger", email="j.lenzenweger@gmail.com" },
 ]
 description = "Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "requests",
+    "aiohttp",
 ]
 [tool.hatch.build.targets.wheel]
 packages = ["src/luke_roberts_cloud_api"]
 
 
 [project.urls]
 Homepage = "https://github.com/julian-lenz/Luke-Roberts-Cloud-API/tree/main"
```

### Comparing `luke_roberts_cloud_api-0.0.7/PKG-INFO` & `luke_roberts_cloud_api-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: luke_roberts_cloud_api
-Version: 0.0.7
+Version: 0.0.8
 Summary: Exposes the API of the Luke Roberts cloud via utility classes. Luke Roberts is a Lighting Manufacturer.
 Project-URL: Homepage, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/tree/main
 Project-URL: Issues, https://github.com/julian-lenz/Luke-Roberts-Cloud-API/issues
 Author-email: Julian Lenzenweger <j.lenzenweger@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: requests
+Requires-Dist: aiohttp
 Description-Content-Type: text/markdown
 
 # Luke Roberts Cloud API
 
 This is a Python library for abstracting the HTTP API of the lamp control for Luke Roberts lamps.
 
 ## Installation
```

