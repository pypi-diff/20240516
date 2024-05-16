# Comparing `tmp/connectlife-0.0.4.tar.gz` & `tmp/connectlife-0.0.5.tar.gz`

## Comparing `connectlife-0.0.4.tar` & `connectlife-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 connectlife-0.0.4/.github/workflows/python-publish.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 connectlife-0.0.4/connectlife/__init__.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 connectlife-0.0.4/connectlife/api.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 connectlife-0.0.4/connectlife/appliance.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 connectlife-0.0.4/connectlife/dump.py
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_dishwasher.json
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_hood_1.json
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_hood_2.json
--rw-r--r--   0        0        0    14445 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_induction_hob_1.json
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_induction_hob_2.json
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_professional_tumble_dryer.json
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_professional_washing_machine.json
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Gorenje_dishwasher.json
--rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Gorenje_washing_machine.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Heat_pump.json
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Oven_type_1.json
--rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Oven_type_2.json
--rw-r--r--   0        0        0   587306 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/format.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 connectlife-0.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 connectlife-0.0.4/LICENSE
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 connectlife-0.0.4/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 connectlife-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 connectlife-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 connectlife-0.0.5/.github/workflows/python-publish.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 connectlife-0.0.5/connectlife/__init__.py
+-rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 connectlife-0.0.5/connectlife/api.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 connectlife-0.0.5/connectlife/appliance.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 connectlife-0.0.5/connectlife/dump.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Asko_dishwasher.json
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Asko_hood_1.json
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Asko_hood_2.json
+-rw-r--r--   0        0        0    14445 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Asko_induction_hob_1.json
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Asko_induction_hob_2.json
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Asko_professional_tumble_dryer.json
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Asko_professional_washing_machine.json
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Gorenje_dishwasher.json
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Gorenje_washing_machine.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Heat_pump.json
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Oven_type_1.json
+-rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/Oven_type_2.json
+-rw-r--r--   0        0        0   587306 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 connectlife-0.0.5/dumps/format.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 connectlife-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 connectlife-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 connectlife-0.0.5/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 connectlife-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 connectlife-0.0.5/PKG-INFO
```

### Comparing `connectlife-0.0.4/.github/workflows/python-publish.yaml` & `connectlife-0.0.5/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/connectlife/api.py` & `connectlife-0.0.5/connectlife/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -60,26 +60,31 @@
     async def login(self) -> None:
         await self._fetch_access_token()
 
 
     async def get_appliances(self) -> Any:
         """Make a request."""
         appliances = await self.get_appliances_json()
-        self.appliances = [ConnectLifeAppliance(self, a) for a in appliances]
+        self.appliances = [ConnectLifeAppliance(self, a) for a in appliances if "deviceId" in a]
         return self.appliances
 
 
     async def get_appliances_json(self) -> Any:
         """Make a request and return the response as text."""
         await self._fetch_access_token()
         async with aiohttp.ClientSession() as session:
             async with session.get(APPLIANCES_URL, headers={
                 "User-Agent": "connectlife-api-connector 2.1.4",
                 "X-Token": self._access_token
             }) as response:
+                if response.status != 200:
+                    _LOGGER.debug(f"Response status code: {response.status}")
+                    _LOGGER.debug(response.headers)
+                    _LOGGER.debug(await response.text())
+                    raise LifeConnectError(f"Unexpected response: status={response.status}")
                 return await response.json()
 
 
     async def _fetch_access_token(self):
         if self._expires is None:
             await self._initial_access_token()
         elif self._expires < dt.datetime.now():
@@ -89,44 +94,63 @@
     async def _initial_access_token(self):
         async with aiohttp.ClientSession() as session:
             async with session.post(LOGIN_URL, data={
                 "loginID": self._username,
                 "password": self._password,
                 "APIKey": API_KEY,
             }) as response:
-                _LOGGER.debug(response.status)
+                if response.status != 200:
+                    _LOGGER.debug(f"Response status code: {response.status}")
+                    _LOGGER.debug(response.headers)
+                    _LOGGER.debug(await response.text())
+                    raise LifeConnectAuthError(f"Unexpected response from login: status={response.status}")
                 body = await self._json(response)
                 uid = body["UID"]
                 login_token = body["sessionInfo"]["cookieValue"]
 
             async with session.post(JWT_URL, data={
                 "APIKey": API_KEY,
                 "login_token":  login_token
             }) as response:
+                if response.status != 200:
+                    _LOGGER.debug(f"Response status code: {response.status}")
+                    _LOGGER.debug(response.headers)
+                    _LOGGER.debug(await response.text())
+                    raise LifeConnectAuthError(f"Unexpected response from getJWT: status={response.status}")
                 body = await self._json(response)
                 id_token = body["id_token"]
 
             async with session.post(OAUTH2_AUTHORIZE, json={
                 "client_id": CLIENT_ID,
                 "redirect_uri": OAUTH2_REDIRECT,
                 "idToken":  id_token,
                 "response_type": "code",
                 "thirdType":"CDC",
                 "thirdClientId": uid,
             }) as response:
+                if response.status != 200:
+                    _LOGGER.debug(f"Response status code: {response.status}")
+                    _LOGGER.debug(response.headers)
+                    _LOGGER.debug(await response.text())
+                    raise LifeConnectAuthError(f"Unexpected response from authorize: status={response.status}")
                 body = await response.json()
                 code = body["code"]
 
             async with session.post(OAUTH2_TOKEN, data={
                 "client_id": CLIENT_ID,
                 "client_secret": CLIENT_SECRET,
                 "redirect_uri": OAUTH2_REDIRECT,
                 "grant_type": "authorization_code",
                 "code": code,
             }) as response:
+                if response.status != 200:
+                    _LOGGER.debug(f"Response status code: {response.status}")
+                    _LOGGER.debug(response.headers)
+                    _LOGGER.debug(await response.text())
+                    raise LifeConnectAuthError(f"Unexpected response from initial access token: status={response.status}")
                 body = await self._json(response)
                 self._access_token = body["access_token"]
                 # Renew 90 seconds before expiration
                 self._expires = dt.datetime.now() + dt.timedelta(0, body["expires_in"] - 90)
                 self._refresh_token = body["refresh_token"]
 
 
@@ -135,14 +159,19 @@
             async with session.post(OAUTH2_TOKEN, data={
                 "client_id": CLIENT_ID,
                 "client_secret": CLIENT_SECRET,
                 "redirect_uri": OAUTH2_REDIRECT,
                 "grant_type": "refresh_token",
                 "refresh_token": self._refresh_token,
             }) as response:
+                if response.status != 200:
+                    _LOGGER.debug(f"Response status code: {response.status}")
+                    _LOGGER.debug(response.headers)
+                    _LOGGER.debug(await response.text())
+                    raise LifeConnectAuthError(f"Unexpected response from refreshing access token: status={response.status}")
                 body = await response.json()
                 self._access_token = body["access_token"]
                 # Renew 90 seconds before expiration
                 self._expires = dt.datetime.now() + dt.timedelta(0, body["expires_in"] - 90)
 
 
     async def _json(self, response: aiohttp.ClientResponse) -> Any:
```

### Comparing `connectlife-0.0.4/connectlife/appliance.py` & `connectlife-0.0.5/connectlife/appliance.py`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/connectlife/dump.py` & `connectlife-0.0.5/connectlife/dump.py`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Asko_dishwasher.json` & `connectlife-0.0.5/dumps/Asko_dishwasher.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Asko_hood_1.json` & `connectlife-0.0.5/dumps/Asko_hood_1.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Asko_hood_2.json` & `connectlife-0.0.5/dumps/Asko_hood_2.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Asko_induction_hob_1.json` & `connectlife-0.0.5/dumps/Asko_induction_hob_1.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Asko_induction_hob_2.json` & `connectlife-0.0.5/dumps/Asko_induction_hob_2.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Asko_professional_tumble_dryer.json` & `connectlife-0.0.5/dumps/Asko_professional_tumble_dryer.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Asko_professional_washing_machine.json` & `connectlife-0.0.5/dumps/Asko_professional_washing_machine.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Gorenje_dishwasher.json` & `connectlife-0.0.5/dumps/Gorenje_dishwasher.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Gorenje_washing_machine.json` & `connectlife-0.0.5/dumps/Gorenje_washing_machine.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Heat_pump.json` & `connectlife-0.0.5/dumps/Heat_pump.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Oven_type_1.json` & `connectlife-0.0.5/dumps/Oven_type_1.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/Oven_type_2.json` & `connectlife-0.0.5/dumps/Oven_type_2.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/README.md` & `connectlife-0.0.5/dumps/README.md`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/dumps/format.py` & `connectlife-0.0.5/dumps/format.py`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/LICENSE` & `connectlife-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/README.md` & `connectlife-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.4/pyproject.toml` & `connectlife-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "connectlife"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Øyvind Matheson Wergeland", email="oyvind@wergeland.org" },
 ]
 description = "A Python library for communicating with the ConnectLife API"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `connectlife-0.0.4/PKG-INFO` & `connectlife-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: connectlife
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for communicating with the ConnectLife API
 Project-URL: Homepage, https://github.com/oyvindwe/connectlife
 Project-URL: Issues, https://github.com/oyvindwe/connectlife/issues
 Author-email: Øyvind Matheson Wergeland <oyvind@wergeland.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

