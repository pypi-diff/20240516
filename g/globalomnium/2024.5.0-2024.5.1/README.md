# Comparing `tmp/globalomnium-2024.5.0.tar.gz` & `tmp/globalomnium-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalomnium-2024.5.0.tar", last modified: Thu May 16 13:17:06 2024, max compression
+gzip compressed data, was "globalomnium-2024.5.1.tar", last modified: Thu May 16 13:26:42 2024, max compression
```

## Comparing `globalomnium-2024.5.0.tar` & `globalomnium-2024.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:17:06.707360 globalomnium-2024.5.0/globalomnium/
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/go_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/globalomnium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:26:42.548077 globalomnium-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-16 13:26:42.548077 globalomnium-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:26:42.544077 globalomnium-2024.5.1/globalomnium/
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/globalomnium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/globalomnium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/globalomnium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/globalomnium/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/globalomnium/go_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/globalomnium/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/globalomnium/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:26:42.548077 globalomnium-2024.5.1/globalomnium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-16 13:26:42.000000 globalomnium-2024.5.1/globalomnium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-16 13:26:42.000000 globalomnium-2024.5.1/globalomnium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:26:42.000000 globalomnium-2024.5.1/globalomnium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 13:26:42.000000 globalomnium-2024.5.1/globalomnium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 13:26:42.000000 globalomnium-2024.5.1/globalomnium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 13:26:42.000000 globalomnium-2024.5.1/globalomnium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 13:26:42.548077 globalomnium-2024.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:26:42.548077 globalomnium-2024.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-16 13:26:38.000000 globalomnium-2024.5.1/tests/test_client.py
```

### Comparing `globalomnium-2024.5.0/LICENSE` & `globalomnium-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `globalomnium-2024.5.0/PKG-INFO` & `globalomnium-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalomnium
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Interface to globalomnium.com water data
 Home-page: https://github.com/carlos-48/globalomnium
 Author: carlos-48
 Author-email: karloselmaster@gmail.com
 Project-URL: Bug Tracker, https://github.com/carlos-48/globalomnium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `globalomnium-2024.5.0/README.md` & `globalomnium-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `globalomnium-2024.5.0/globalomnium/__init__.py` & `globalomnium-2024.5.1/globalomnium/__init__.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2024.5.0/globalomnium/__main__.py` & `globalomnium-2024.5.1/globalomnium/__main__.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2024.5.0/globalomnium/cli.py` & `globalomnium-2024.5.1/globalomnium/cli.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2024.5.0/globalomnium/client.py` & `globalomnium-2024.5.1/globalomnium/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,16 +164,16 @@
         "error": "",
         "redirectURL": "/VirtualOffice/Secure/action_login"
         }
         """
         login_payload = "login="+ self.username +"&pass="+ self.password + "&remember=true" + "&suministro="
 
 
-        #data = await self.request_json("POST", _LOGIN_ENDPOINT, data=login_payload) #cambiar entre request_json y _request
-        data = await self._request("POST", _LOGIN_ENDPOINT, data=login_payload) #cambiar entre request_json y _request
+        data = await self.request_json("POST", _LOGIN_ENDPOINT, data=login_payload) #cambiar entre request_json y _request
+        #data = await self._request("POST", _LOGIN_ENDPOINT, data=login_payload) #cambiar entre request_json y _request
         if not isinstance(data, dict):
             raise InvalidData(data)
 
         if data.get("result", "false") != True:
             raise CommandError(data)
 
         self._login_ts = datetime.now()
@@ -403,16 +403,16 @@
 
         self._logger.debug("Requesting data may take up to a minute.")
 
         end_today = datetime.now().strftime("%d/%m/%Y")
         start_yesterday = (datetime.now() - timedelta(days=1)).strftime("%d/%m/%Y")
         payload = f"start={start_yesterday}&end={end_today}"
 
-       # data = await self.request_json("GET", _MEASURE_ENDPOINT, data=payload) #cambiar entre request_json y _request
-        data = await self._request("GET", _MEASURE_ENDPOINT, data=payload) #cambiar entre request_json y _request
+        data = await self.request_json("GET", _MEASURE_ENDPOINT, data=payload) #cambiar entre request_json y _request
+        #data = await self._request("GET", _MEASURE_ENDPOINT, data=payload) #cambiar entre request_json y _request
 
         self._logger.debug(f"Got reply, raw data: {data!r}")
 
         try:
             measure = Measure(
                 accumulate=int(
                     data["table"][-1]["Lectura"]
```

### Comparing `globalomnium-2024.5.0/globalomnium/mqtt.py` & `globalomnium-2024.5.1/globalomnium/mqtt.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2024.5.0/globalomnium/parsers.py` & `globalomnium-2024.5.1/globalomnium/parsers.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2024.5.0/globalomnium.egg-info/PKG-INFO` & `globalomnium-2024.5.1/globalomnium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalomnium
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Interface to globalomnium.com water data
 Home-page: https://github.com/carlos-48/globalomnium
 Author: carlos-48
 Author-email: karloselmaster@gmail.com
 Project-URL: Bug Tracker, https://github.com/carlos-48/globalomnium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `globalomnium-2024.5.0/setup.cfg` & `globalomnium-2024.5.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = globalomnium
-version = 2024.05.0
+version = 2024.05.1
 author = carlos-48
 author_email = karloselmaster@gmail.com
 description = Interface to globalomnium.com water data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/carlos-48/globalomnium
 project_urls =
```

### Comparing `globalomnium-2024.5.0/tests/test_client.py` & `globalomnium-2024.5.1/tests/test_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     with open(f"{FIXTURES_DIR}/{fixture_name}.bin", "rb") as fh:
         return fh.read()
 
 
 class TestClient(unittest.IsolatedAsyncioTestCase):
     async def asyncSetUp(self):
         self.sess = await get_session()
-        self.client = Client(None, "x", "y")
+        #self.client = Client(None, "x", "y")
+        self.client = Client(self.sess, "x", "y") 
         self.end = datetime.now().replace(hour=0, minute=0, second=0)
         self.start = self.end - timedelta(days=7)
 
     async def asyncTearDown(self):
         await self.sess.close()
 
     async def test_login_ok(self):
@@ -66,27 +67,10 @@
             return_value=read_fixture("historical-consumption"),
         ):
             ret = await self.client.get_historical_consumption(self.start, self.end)
 
             self.assertEqual(ret["accumulated"], 97871.0)
             #self.assertEqual(ret["accumulated-co2"], 23586.91)
 
-#    @patch("globalomnium.Client.is_logged", return_value=True)
-#     async def test_historical_power_demand(self, _):
-#        with patch(
-#            "globalomnium.Client.request_bytes",
-#            new_class=AsyncMock,
-#            side_effect=[
-#                read_fixture("historical-power-demand-limits"),
-#                read_fixture("historical-power-demand"),
-#            ],
-#        ):
-#            ret = await self.client.get_historical_power_demand()
-#
-#            self.assertEqual(len(ret), 50)
-#            self.assertEqual(
-#                ret[25], {"dt": datetime(2022, 5, 28, 22, 15), "value": 2816.0}
-#            )
-
 
 if __name__ == "__main__":
     unittest.main()
```

