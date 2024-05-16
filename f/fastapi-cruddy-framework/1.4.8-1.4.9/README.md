# Comparing `tmp/fastapi_cruddy_framework-1.4.8.tar.gz` & `tmp/fastapi_cruddy_framework-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-1.4.8.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-1.4.9.tar", max compression
```

## Comparing `fastapi_cruddy_framework-1.4.8.tar` & `fastapi_cruddy_framework-1.4.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.8/LICENSE
--rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.8/README.md
--rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    44781 2024-04-12 17:41:34.217544 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/graphql.py
--rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/pubsub.py
--rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    31716 2024-04-10 18:04:33.796733 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/test_helpers.py
--rw-r--r--   0        0        0     8260 2024-04-10 15:33:48.817894 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/websocket_manager.py
--rw-r--r--   0        0        0     2252 2024-04-12 17:42:31.230211 fastapi_cruddy_framework-1.4.8/pyproject.toml
--rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.9/LICENSE
+-rw-r--r--   0        0        0    54833 2024-05-03 12:50:05.846036 fastapi_cruddy_framework-1.4.9/README.md
+-rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     6865 2024-05-15 17:30:32.709889 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    44781 2024-04-12 17:41:34.217544 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/graphql.py
+-rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/pubsub.py
+-rw-r--r--   0        0        0    36269 2024-05-06 18:59:15.284432 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    31716 2024-04-10 18:04:33.796733 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/test_helpers.py
+-rw-r--r--   0        0        0     8260 2024-04-10 15:33:48.817894 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/websocket_manager.py
+-rw-r--r--   0        0        0     2252 2024-05-15 17:34:29.752719 fastapi_cruddy_framework-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0    56461 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.9/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-1.4.8/LICENSE` & `fastapi_cruddy_framework-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/README.md` & `fastapi_cruddy_framework-1.4.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -884,51 +884,46 @@
 def event_loop():
     loop = get_event_loop_policy().new_event_loop()
     yield loop
     loop.close()
 
 
 @fixture(scope="session", autouse=True)
-
 async def app():
     # Don't move this import!
     from your_app.main import app
 
     yield app
 
 
 @fixture(scope="session", autouse=True)
-
 async def client(app: FastAPI):
     # By using "with" the FastAPI app launch hook is run, connecting the application router
     async with TestClient(app, use_cookies=False) as client:
         while (await client.get("/health")).json() != True:
             await sleep(0.5)
         yield client
 
 
 @fixture(scope="session", autouse=True)
-
 async def unauthenticated_client(client: TestClient):
     blank_client = BrowserTestClient(client=client, cookies=None, headers=None)
     yield blank_client
 
 
 @fixture(scope="session", autouse=True)
-
 async def authenticated_client(client: TestClient):
     sessioned_client = BrowserTestClient(
         client=client, cookies=None, headers=FAKE_AUTH_HEADERS
     )
     await sessioned_client.get(f"/users/authorization{FAKE_AUTH_QP}")
     yield sessioned_client
 
 
 @fixture(scope="function")
-
 async def authenticated_websocket(authenticated_client: BrowserTestClient):
     async with authenticated_client.websocket_connect("/ws") as websocket:
         # For example: data = await websocket.receive_json()
         # Or await websocket.send_json(data)
         # If your server sends any kind of "welcome" messages, make
         # sure you purge them here BEFORE yielding the socket back
         # to whatever function needs to run tests
```

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 # -------------------------------------------------------------------------------------------
 # BASE ADAPTER
 # -------------------------------------------------------------------------------------------
 class BaseAdapter:
     engine: AsyncEngine
 
-    def __init__(self, **kwargs):
+    def __init__(self, echo=True, **kwargs):
         self.engine = create_async_engine(
             "sqlite+aiosqlite:///file:temp.db?mode=memory&cache=shared&uri=true",
-            echo=True,
+            echo=echo,
             future=True,
             **kwargs,
         )
 
     async def __call__(self) -> AsyncIterator[AsyncSession]:
         # Used by FastAPI Depends
         async with self.getSession() as session:
@@ -53,14 +53,15 @@
     @asynccontextmanager
     async def getSession(self):
         asyncSession = self.asyncSessionGenerator()
         async with asyncSession() as session:
             try:
                 yield session
                 await session.commit()
+                await session.close()
             except:
                 try:
                     await session.rollback()
                 except:
                     pass
                 await session.close()
                 raise
@@ -77,19 +78,21 @@
 # -------------------------------------------------------------------------------------------
 # MYSQL ADAPTER
 # -------------------------------------------------------------------------------------------
 class MysqlAdapter(BaseAdapter):
     connection_uri: str
     engine: AsyncEngine
 
-    def __init__(self, connection_uri="", pool_size=4, max_overflow=64, **kwargs):
+    def __init__(
+        self, connection_uri="", pool_size=4, max_overflow=64, echo=True, **kwargs
+    ):
         self.connection_uri = connection_uri
         self.engine = create_async_engine(
             self.connection_uri,
-            echo=True,
+            echo=echo,
             future=True,
             pool_size=pool_size,
             max_overflow=max_overflow,
             **kwargs,
         )
 
 
@@ -111,25 +114,29 @@
     SQLITE_ASYNC_URL_PREFIX = "sqlite+aiosqlite:///"
     MEMORY_LOCATION_START = "file:"
     MEMORY_LOCATION_END = "?mode=memory&cache=shared&uri=true"
     connection_uri: str
     engine: AsyncEngine
 
     def __init__(
-        self, db_path="temp.db", mode: Literal["memory", "file"] = "memory", **kwargs
+        self,
+        db_path="temp.db",
+        mode: Literal["memory", "file"] = "memory",
+        echo=True,
+        **kwargs,
     ):
         if mode == "memory":
             self.connection_uri = f"{self.SQLITE_ASYNC_URL_PREFIX}{self.MEMORY_LOCATION_START}{db_path}{self.MEMORY_LOCATION_END}"
         else:
             self.connection_uri = f"{self.SQLITE_ASYNC_URL_PREFIX}{db_path}"
         self.engine = create_async_engine(
             self.connection_uri,
             connect_args={"check_same_thread": False},
             poolclass=StaticPool,
-            echo=True,
+            echo=echo,
             future=True,
             **kwargs,
         )
 
 
 # -------------------------------------------------------------------------------------------
 # REDIS ADAPTER
```

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/graphql.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/graphql.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/pubsub.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/pubsub.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/test_helpers.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/util.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/util.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/websocket_manager.py` & `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.8/pyproject.toml` & `fastapi_cruddy_framework-1.4.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "1.4.8"
+version = "1.4.9"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
```

### Comparing `fastapi_cruddy_framework-1.4.8/PKG-INFO` & `fastapi_cruddy_framework-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 1.4.8
+Version: 1.4.9
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: SQLAlchemy-Utils (>=0.41.1,<0.42.0)
 Requires-Dist: SQLAlchemy[asyncio] (>=2.0.0)
 Requires-Dist: async-asgi-testclient (>=1.4.11,<2.0.0)
 Requires-Dist: async-timeout (>=4.0.0,<5.0.0)
@@ -919,51 +920,46 @@
 def event_loop():
     loop = get_event_loop_policy().new_event_loop()
     yield loop
     loop.close()
 
 
 @fixture(scope="session", autouse=True)
-
 async def app():
     # Don't move this import!
     from your_app.main import app
 
     yield app
 
 
 @fixture(scope="session", autouse=True)
-
 async def client(app: FastAPI):
     # By using "with" the FastAPI app launch hook is run, connecting the application router
     async with TestClient(app, use_cookies=False) as client:
         while (await client.get("/health")).json() != True:
             await sleep(0.5)
         yield client
 
 
 @fixture(scope="session", autouse=True)
-
 async def unauthenticated_client(client: TestClient):
     blank_client = BrowserTestClient(client=client, cookies=None, headers=None)
     yield blank_client
 
 
 @fixture(scope="session", autouse=True)
-
 async def authenticated_client(client: TestClient):
     sessioned_client = BrowserTestClient(
         client=client, cookies=None, headers=FAKE_AUTH_HEADERS
     )
     await sessioned_client.get(f"/users/authorization{FAKE_AUTH_QP}")
     yield sessioned_client
 
 
 @fixture(scope="function")
-
 async def authenticated_websocket(authenticated_client: BrowserTestClient):
     async with authenticated_client.websocket_connect("/ws") as websocket:
         # For example: data = await websocket.receive_json()
         # Or await websocket.send_json(data)
         # If your server sends any kind of "welcome" messages, make
         # sure you purge them here BEFORE yielding the socket back
         # to whatever function needs to run tests
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.8 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.9 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries :: Application Frameworks Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Requires-Dist: SQLAlchemy-
-Utils (>=0.41.1,<0.42.0) Requires-Dist: SQLAlchemy[asyncio] (>=2.0.0) Requires-
-Dist: async-asgi-testclient (>=1.4.11,<2.0.0) Requires-Dist: async-timeout
-(>=4.0.0,<5.0.0) Requires-Dist: fakeredis (>=2.21.3) Requires-Dist: fastapi
-[all] (>=0.100.0) Requires-Dist: inflect (>=7.0.0,<8.0.0) Requires-Dist:
-pymitter (>=0.5.0) Requires-Dist: redis (>=5.0.1,<6.0.0) Requires-Dist:
-sqlmodel (>=0.0.16,<0.0.17) Requires-Dist: strawberry-graphql[fastapi]
-(>=0.223.0) Requires-Dist: uuid7 (>=0.1.0,<0.2.0) Requires-Dist: validator-
-collection (>=1.5.0,<2.0.0) Project-URL: Repository, https://github.com/
-mdconaway/fastapi-cruddy-framework Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Software Development Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Requires-Dist: SQLAlchemy-Utils (>=0.41.1,<0.42.0) Requires-
+Dist: SQLAlchemy[asyncio] (>=2.0.0) Requires-Dist: async-asgi-testclient
+(>=1.4.11,<2.0.0) Requires-Dist: async-timeout (>=4.0.0,<5.0.0) Requires-Dist:
+fakeredis (>=2.21.3) Requires-Dist: fastapi[all] (>=0.100.0) Requires-Dist:
+inflect (>=7.0.0,<8.0.0) Requires-Dist: pymitter (>=0.5.0) Requires-Dist: redis
+(>=5.0.1,<6.0.0) Requires-Dist: sqlmodel (>=0.0.16,<0.0.17) Requires-Dist:
+strawberry-graphql[fastapi] (>=0.223.0) Requires-Dist: uuid7 (>=0.1.0,<0.2.0)
+Requires-Dist: validator-collection (>=1.5.0,<2.0.0) Project-URL: Repository,
+https://github.com/mdconaway/fastapi-cruddy-framework Description-Content-Type:
+text/markdown
                     ********** FFaassttAAPPII -- CCrruuddddyy FFrraammeewwoorrkk **********
                                     _[_L_o_g_o_]
 ## About Cruddy Framework [![Product Name Screen Shot][product-screenshot]]
 (https://github.com/mdconaway/fastapi-cruddy-framework) CCrruuddddyy FFrraammeewwoorrkk nnooww
 ssuuppppoorrttss GGrraapphhQQLL!! FFoorr eexxaammpplleess,, sseeee tthhee [[eexxaammppllee sseerrvveerr]]((eexxaammpplleess//
 ffaassttaappii__ccrruuddddyy__ssqqlliittee))!! `fastapi-cruddy-framework` is a companion library to
 [FastAPI](https://fastapi.tiangolo.com/) designed to bring the development
```

