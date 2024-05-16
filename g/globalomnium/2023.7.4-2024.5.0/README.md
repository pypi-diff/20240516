# Comparing `tmp/globalomnium-2023.7.4.tar.gz` & `tmp/globalomnium-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalomnium-2023.7.4.tar", last modified: Sat Jul 15 00:07:02 2023, max compression
+gzip compressed data, was "globalomnium-2024.5.0.tar", last modified: Thu May 16 13:17:06 2024, max compression
```

## Comparing `globalomnium-2023.7.4.tar` & `globalomnium-2024.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/globalomnium/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/globalomnium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:17:06.707360 globalomnium-2024.5.0/globalomnium/
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/go_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/globalomnium/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/globalomnium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 13:17:06.000000 globalomnium-2024.5.0/globalomnium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:17:06.711360 globalomnium-2024.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-16 13:17:00.000000 globalomnium-2024.5.0/tests/test_client.py
```

### Comparing `globalomnium-2023.7.4/LICENSE` & `globalomnium-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.4/globalomnium/__init__.py` & `globalomnium-2024.5.0/globalomnium/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,28 +29,28 @@
     InvalidContractError,
     InvalidData,
     RequestFailedError,
 )
 
 
 def get_credentials(parsedargs=None, credentials=None, environ_prefix="GLOBALOMNIUM"):
-    if parsedargs and parsedargs.user:
-        return parsedargs.user, parsedargs.passw
+    if parsedargs and parsedargs.username:
+        return parsedargs.username, parsedargs.password
 
     credentials = credentials or getattr(parsedargs, "credentials", None)
     if credentials:
         with open(credentials, mode="r", encoding="utf-8") as fh:
             d = json.loads(fh.read())
-        return d["user"], d["passw"]
+        return d["username"], d["password"]
 
     if environ_prefix:
         environ_prefix = environ_prefix.upper()
         return (
-            os.environ.get(f"{environ_prefix}_USER"),
-            os.environ.get(f"{environ_prefix}_PASSW"),
+            os.environ.get(f"{environ_prefix}_USERNAME"),
+            os.environ.get(f"{environ_prefix}_PASSWORD"),
         )
 
 
 def sanitize_address(address):
     return " ".join([x.strip().capitalize() for x in address.split(" ") if x])
 
 
@@ -69,36 +69,34 @@
 __doc__ = """
     # Returned JSON payloads for login phase:
 
     scenario: Valid credentials.
     response code: 200
     response json:
     {
-        "redirect": "informacion-del-contrato",
-        "zona": "B",
-        "success": "true",
-        "idioma": "ES",
-        "uCcr": "",
+    "result": true,
+    "error": "",
+    "redirectURL": "/VirtualOffice/Secure/action_login"
     }
 
     scenario: Invalid credentials.
     response code: 200
     response json:
     {
-        "success": "false",
-        "message": "El usuario o la contraseña que has introducido son incorrectos. Por favor, inténtalo de nuevo.",
+        "result": false,
+        "error": "Error de inicio de sesión, comprueba que las credencias son válidas."
     }
 
 
     scenario: Several login retries with invalid credentials.
     response code: 200
     response json:
     {
-      "success": "false",
-      "message": "Número de intentos de acceso excedido. Usuario bloqueado temporalmente. Vuelva a intentarlo dentro de 5 minutos."
+        "result": false,
+        "error": "Detectados varios intentos de acceso consecutivos. Por favor, vuélvalo a intentar más tarde."
     }
 
     # Retuned JSON payloads for measures (exposed keys: "valLecturaContador", "valMagnitud", "valEstado")
 
     scenario: valid measure
     response code: 200
     response json:
```

### Comparing `globalomnium-2023.7.4/globalomnium/__main__.py` & `globalomnium-2024.5.0/globalomnium/__main__.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.4/globalomnium/cli.py` & `globalomnium-2024.5.0/globalomnium/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 from datetime import datetime, timedelta
 
 from . import Client, RequestFailedError, get_credentials, get_session
 
 
 def build_arg_parser():
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", required=False)
-    parser.add_argument("-p", "--passw", required=False)
+    parser.add_argument("-u", "--username", required=False)
+    parser.add_argument("-p", "--password", required=False)
     parser.add_argument("--credentials", required=False)
     parser.add_argument("--retries", type=int, default=1)
     parser.add_argument("--contract")
 
     parser.add_argument("--list-contracts", action="store_true")
     parser.add_argument("--get-measure", action="store_true")
     parser.add_argument("--get-historical-consumption", action="store_true")
@@ -76,23 +76,23 @@
         datefmt="%Y-%m-%d %H:%M:%S",
     )
     logger = logging.getLogger("globalomnium")
     logger.setLevel(logging.DEBUG)
 
     parser = build_arg_parser()
     args = parser.parse_args()
-    user, passw = get_credentials(args)
+    username, password = get_credentials(args)
 
-    if not user or not passw:
+    if not username or not password:
         print("Missing username or password", file=sys.stderr)
         sys.exit(1)
 
     session = await get_session()
     client = Client(
-        user=user, passw=passw, session=session, logger=logger
+        username=username, password=password, session=session, logger=logger
     )
 
     try:
         if data := await _main():
             print(pprint.pformat(data))
 
     except RequestFailedError as e:
```

### Comparing `globalomnium-2023.7.4/globalomnium/mqtt.py` & `globalomnium-2024.5.0/globalomnium/mqtt.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
     parser = cli.build_arg_parser()
     parser.add_argument("--host", required=True)
     parser.add_argument("--topic", default="globalomnium")
 
     args = parser.parse_args()
 
-    user, passw = get_credentials(args)
-    measure = cli.get_measure(user, passw)
+    username, password = get_credentials(args)
+    measure = cli.get_measure(username, password)
     if not measure:
         sys.exit(1)
 
     msgs = [
         {"topic": f"{args.topic}/{k}", "payload": v, "retain": True}
         for (k, v) in measure.asdict().items()
     ]
```

### Comparing `globalomnium-2023.7.4/globalomnium/parsers.py` & `globalomnium-2024.5.0/globalomnium/parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301,
 # USA.
 
 
-import itertools
+# import itertools
+import re
 from datetime import datetime, timedelta
 from typing import Dict, List, Optional
 
-from .types import ConsumptionForPeriod, HistoricalConsumption
+from .go_types import ConsumptionForPeriod, HistoricalConsumption
 
 
 def parser_generic_historical_data(data, base_dt: datetime) -> Dict:
     def _normalize_historical_item(idx: int, item: Optional[Dict]) -> Optional[Dict]:
         if item is None:
             return None
 
@@ -52,30 +53,31 @@
         "accumulated": float(data["acumulado"]),
         # "accumulated-co2": float(data["acumuladoCO2"]),
         "historical": historical,
     }
 
 
 def parse_historical_consumption(data) -> HistoricalConsumption:
-    def list_to_dict(values, keys):
-        return {keys[idx]: values[idx] for idx in range(len(values))}
+    # def list_to_dict(values, keys):
+    #    return {keys[idx]: values[idx] for idx in range(len(values))}
 
     # CORREGIR, YA QUE EN GO EXISTE EL CAMPO FECHA DESDE PERO ESTA EN BLANCO, ESTA LA FEHA EN UN CAMPO STRING QUE HAY QUE DECODIFICAR
-    start = datetime.strptime(table[0]["FechaDesde"], "%d-%m-%Y").replace(
-        hour=0, minute=0, second=0
-    )
+    timestamp_matches = re.findall(r'\d+', data["table"][0]["Fecha"])
+    timestamp = int(timestamp_matches[0]) // 1000
+    start = datetime.fromtimestamp(timestamp)
+  
 
-    period_names = table[0]["Periodo"]
+    # period_names = table[0]["Periodo"]
 
     ret = HistoricalConsumption(
-        total=table[0]["Lectura"],
+        total=data["table"][0]["Lectura"],
         # desglosed=list_to_dict(data[0]["totalesPeriodosTarifarios"], period_names),
     )
 
-    for idx, value in enumerate(tabla[0]["Lectura"]):
+    for idx, value in enumerate(data["table"][0]["Lectura"]):
         ret.consumptions.append(
             ConsumptionForPeriod(
                 start=start + timedelta(hours=idx),
                 end=start + timedelta(hours=idx + 1),
                 value=value,
                 # desglosed=list_to_dict(
                 #     data[0]["valoresPeriodosTarifarios"][idx], period_names
```

### Comparing `globalomnium-2023.7.4/setup.cfg` & `globalomnium-2024.5.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = globalomnium
-version = 2023.07.4
-author = carlos-48 (forked from Luis López)
+version = 2024.05.0
+author = carlos-48
 author_email = karloselmaster@gmail.com
 description = Interface to globalomnium.com water data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/carlos-48/globalomnium
 project_urls = 
 	Bug Tracker = https://github.com/carlos-48/globalomnium/issues
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `globalomnium-2023.7.4/tests/test_client.py` & `globalomnium-2024.5.0/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,17 @@
             "globalomnium.Client.request_bytes",
             new_class=AsyncMock,
             return_value=read_fixture("historical-consumption"),
         ):
             ret = await self.client.get_historical_consumption(self.start, self.end)
 
             self.assertEqual(ret["accumulated"], 97871.0)
-            self.assertEqual(ret["accumulated-co2"], 23586.91)
+            #self.assertEqual(ret["accumulated-co2"], 23586.91)
 
-    @patch("globalomnium.Client.is_logged", return_value=True)
+#    @patch("globalomnium.Client.is_logged", return_value=True)
 #     async def test_historical_power_demand(self, _):
 #        with patch(
 #            "globalomnium.Client.request_bytes",
 #            new_class=AsyncMock,
 #            side_effect=[
 #                read_fixture("historical-power-demand-limits"),
 #                read_fixture("historical-power-demand"),
```

