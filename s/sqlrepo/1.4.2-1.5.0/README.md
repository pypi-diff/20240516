# Comparing `tmp/sqlrepo-1.4.2.tar.gz` & `tmp/sqlrepo-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlrepo-1.4.2.tar", last modified: Mon May  6 09:19:40 2024, max compression
+gzip compressed data, was "sqlrepo-1.5.0.tar", last modified: Thu May 16 07:26:31 2024, max compression
```

## Comparing `sqlrepo-1.4.2.tar` & `sqlrepo-1.5.0.tar`

### file list

```diff
@@ -1,29 +1,35 @@
--rw-r--r--   0        0        0    10244 2024-04-22 06:04:46.394911 sqlrepo-1.4.2/README.md
--rw-r--r--   0        0        0     3054 2024-05-06 09:19:40.069292 sqlrepo-1.4.2/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/README.md
--rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.4.2/sqlrepo/__init__.py
--rw-r--r--   0        0        0      828 2024-04-22 06:04:46.395911 sqlrepo-1.4.2/sqlrepo/exc.py
--rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.4.2/sqlrepo/logging.py
--rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.4.2/sqlrepo/py.typed
--rw-r--r--   0        0        0    32880 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/sqlrepo/queries.py
--rw-r--r--   0        0        0    23853 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/sqlrepo/repositories.py
--rw-r--r--   0        0        0     4696 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/sqlrepo/uow.py
--rw-r--r--   0        0        0     1057 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/sqlrepo/wrappers.py
--rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.4.2/tests/__init__.py
--rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.4.2/tests/conftest.py
--rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-1.4.2/tests/test_async_queries.py
--rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-1.4.2/tests/test_async_repositories.py
--rw-r--r--   0        0        0     1771 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/tests/test_async_uow.py
--rw-r--r--   0        0        0    17037 2024-04-22 06:04:46.397911 sqlrepo-1.4.2/tests/test_base_queries.py
--rw-r--r--   0        0        0     2983 2024-04-22 06:04:46.397911 sqlrepo-1.4.2/tests/test_base_repositories.py
--rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-1.4.2/tests/test_sync_queries.py
--rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-1.4.2/tests/test_sync_repositories.py
--rw-r--r--   0        0        0     1540 2024-04-22 06:04:46.397911 sqlrepo-1.4.2/tests/test_sync_uow.py
--rw-r--r--   0        0        0     1061 2024-04-22 06:04:46.397911 sqlrepo-1.4.2/tests/test_wrappers.py
--rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.4.2/tests/types.py
--rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-1.4.2/tests/utils.py
--rw-r--r--   0        0        0    10597 1970-01-01 00:00:00.000000 sqlrepo-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0    12676 2024-05-16 07:23:01.665324 sqlrepo-1.5.0/README.md
+-rw-r--r--   0        0        0     3124 2024-05-16 07:26:31.549223 sqlrepo-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/README.md
+-rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.5.0/sqlrepo/__init__.py
+-rw-r--r--   0        0        0      828 2024-04-22 06:04:46.395911 sqlrepo-1.5.0/sqlrepo/exc.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:58:11.149780 sqlrepo-1.5.0/sqlrepo/ext/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-16 07:19:23.476470 sqlrepo-1.5.0/sqlrepo/ext/fastapi/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-16 07:17:37.081028 sqlrepo-1.5.0/sqlrepo/ext/fastapi/containers.py
+-rw-r--r--   0        0        0      186 2024-05-16 07:10:05.345399 sqlrepo-1.5.0/sqlrepo/ext/fastapi/helpers.py
+-rw-r--r--   0        0        0     7935 2024-05-16 07:04:51.952120 sqlrepo-1.5.0/sqlrepo/ext/fastapi/services.py
+-rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.5.0/sqlrepo/logging.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.5.0/sqlrepo/py.typed
+-rw-r--r--   0        0        0    32880 2024-04-22 06:04:46.396911 sqlrepo-1.5.0/sqlrepo/queries.py
+-rw-r--r--   0        0        0    23853 2024-04-22 06:04:46.396911 sqlrepo-1.5.0/sqlrepo/repositories.py
+-rw-r--r--   0        0        0     4696 2024-04-22 06:04:46.396911 sqlrepo-1.5.0/sqlrepo/uow.py
+-rw-r--r--   0        0        0     1202 2024-05-15 13:59:23.791626 sqlrepo-1.5.0/sqlrepo/wrappers.py
+-rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-1.5.0/tests/test_async_queries.py
+-rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-1.5.0/tests/test_async_repositories.py
+-rw-r--r--   0        0        0     1771 2024-04-22 06:04:46.396911 sqlrepo-1.5.0/tests/test_async_uow.py
+-rw-r--r--   0        0        0    17037 2024-04-22 06:04:46.397911 sqlrepo-1.5.0/tests/test_base_queries.py
+-rw-r--r--   0        0        0     2983 2024-04-22 06:04:46.397911 sqlrepo-1.5.0/tests/test_base_repositories.py
+-rw-r--r--   0        0        0    10769 2024-05-16 07:09:22.500629 sqlrepo-1.5.0/tests/test_fastapi_ext.py
+-rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-1.5.0/tests/test_sync_queries.py
+-rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-1.5.0/tests/test_sync_repositories.py
+-rw-r--r--   0        0        0     1540 2024-04-22 06:04:46.397911 sqlrepo-1.5.0/tests/test_sync_uow.py
+-rw-r--r--   0        0        0     1061 2024-04-22 06:04:46.397911 sqlrepo-1.5.0/tests/test_wrappers.py
+-rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.5.0/tests/types.py
+-rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-1.5.0/tests/utils.py
+-rw-r--r--   0        0        0    13104 1970-01-01 00:00:00.000000 sqlrepo-1.5.0/PKG-INFO
```

### Comparing `sqlrepo-1.4.2/README.md` & `sqlrepo-1.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -298,7 +298,111 @@
     __skip_session_use__ = True
 
 ...
 ```
 
 and this will cause no commit or other session manipulation (except session create for repositories
 work).
+
+## Extensions
+
+v1.5.0 now provided extensions for other technologies like web-frameworks. Now only FastAPI is
+supported.
+
+### FastAPI
+
+FastAPI extensions implements base classes for services and container, so you can work with your
+code easier.
+
+First of all You need to prepare all to work with plugin:
+
+```python
+from functools import cached_property
+
+from fastapi import FastAPI
+from sqlalchemy import create_engine
+from sqlalchemy.orm import DeclarativeBase, sessionmaker
+
+from sqlrepo import BaseSyncRepository
+
+engine = create_engine("<your-db-url-here>")
+Session = sessionmaker(engine)
+
+
+class Base(DeclarativeBase): ...
+
+
+class YourModel(Base):
+    # Your model definition
+    ...
+
+
+def get_session():
+    with Session() as session:
+        yield session
+
+
+app = FastAPI()
+```
+
+then you should use plugin like this:
+
+```python
+# your prepared code below
+
+from sqlrepo.ext.fastapi import add_container_overrides
+add_container_overrides(app, get_session)
+```
+
+then you can implements containers and services like this:
+
+```python
+# your prepared code below
+
+from pydantic import BaseModel, ConfigDict
+
+from sqlrepo.ext.fastapi import BaseSyncContainer, BaseSyncService
+
+
+class YourModelDetail(BaseModel):
+    model_config = ConfigDict(from_attributes=True)
+    ...
+
+
+class YourModelList(BaseModel):
+    model_config = ConfigDict(from_attributes=True)
+    ...
+
+
+class YourModelRepository(BaseSyncRepository[YourModel]):
+    def your_custom_repo_method(self) -> YourModel: ...
+
+
+class YourModelService(BaseSyncService[YourModel, YourModelDetail, YourModelList]):
+    detail_schema = YourModelDetail
+    list_schema = YourModelList
+    not_found_message = "YourModel entity not found in database"
+    not_found_exception = HTTPException
+
+    def init_repositories(self, session: "Session") -> None:
+        self.your_model_repo = YourModelRepository(session)
+
+    def your_custom_service_method(self) -> YourModelDetail:
+        return self.resolve(self.your_model_repo.your_custom_repo_method())
+
+
+class Container(BaseSyncContainer):
+
+    @cached_property
+    def your_model_service(self):
+        return YourModelService(self.session, self.request)
+```
+
+and finally you can use Container in your routes like this:
+
+```python
+# your prepared code below
+
+@app.get("/", response_model=YourModelDetail)
+def get_your_model(container: Container = Depends()):
+    return container.your_model_service.your_custom_service_method()
+```
```

### Comparing `sqlrepo-1.4.2/pyproject.toml` & `sqlrepo-1.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -172,27 +172,32 @@
     "httpx>=0.27.0",
     "pyment>=0.3.3",
     "ipython>=8.19.0",
 ]
 
 [project]
 name = "sqlrepo"
-version = "1.4.2"
+version = "1.5.0"
 description = "sqlalchemy repositories with crud operations and other utils for it."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
     "sqlalchemy>=2.0.29",
-    "python-dev-utils[sqlalchemy_filters]>=1.8.3",
+    "python-dev-utils[sqlalchemy_filters]>=1.11.0",
 ]
 
 [project.license]
 text = "MIT"
 
+[project.optional-dependencies]
+fastapi = [
+    "fastapi>=0.100",
+]
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `sqlrepo-1.4.2/sqlrepo/exc.py` & `sqlrepo-1.5.0/sqlrepo/exc.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/sqlrepo/logging.py` & `sqlrepo-1.5.0/sqlrepo/logging.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/sqlrepo/queries.py` & `sqlrepo-1.5.0/sqlrepo/queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/sqlrepo/repositories.py` & `sqlrepo-1.5.0/sqlrepo/repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/sqlrepo/uow.py` & `sqlrepo-1.5.0/sqlrepo/uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/sqlrepo/wrappers.py` & `sqlrepo-1.5.0/sqlrepo/wrappers.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,20 @@
 
     replace with such pattern:
 
         1) if there is SQLAlchemyError, throw QueryError, because its error in query executing.
 
         2) if there is error from python-dev-utils (BaseDevError), throw RepositoryError.
 
-        3) if there is possible python errors (no all. Only specific), throw BaseSQLRepoError.
+        3) if there is possible python errors (not all. Only specific), throw BaseSQLRepoError.
     """
     try:
         yield
     except SQLAlchemyError as exc:
-        raise QueryError from exc
+        msg = "error on SQLAlchemy level."
+        raise QueryError(msg) from exc
     except BaseDevError as exc:
+        msg = "error on python-dev-utils package level."
         raise RepositoryError from exc
     except (AttributeError, TypeError, ValueError) as exc:
+        msg = "error on python level."
         raise BaseSQLRepoError from exc
```

### Comparing `sqlrepo-1.4.2/tests/conftest.py` & `sqlrepo-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/test_async_queries.py` & `sqlrepo-1.5.0/tests/test_async_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/test_async_repositories.py` & `sqlrepo-1.5.0/tests/test_async_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/test_async_uow.py` & `sqlrepo-1.5.0/tests/test_async_uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/test_base_queries.py` & `sqlrepo-1.5.0/tests/test_base_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/test_base_repositories.py` & `sqlrepo-1.5.0/tests/test_base_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/test_sync_queries.py` & `sqlrepo-1.5.0/tests/test_sync_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/test_sync_repositories.py` & `sqlrepo-1.5.0/tests/test_sync_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/test_sync_uow.py` & `sqlrepo-1.5.0/tests/test_sync_uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/test_wrappers.py` & `sqlrepo-1.5.0/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/types.py` & `sqlrepo-1.5.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/tests/utils.py` & `sqlrepo-1.5.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.2/PKG-INFO` & `sqlrepo-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlrepo
-Version: 1.4.2
+Version: 1.5.0
 Summary: sqlalchemy repositories with crud operations and other utils for it.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: sqlalchemy>=2.0.29
-Requires-Dist: python-dev-utils[sqlalchemy_filters]>=1.8.3
+Requires-Dist: python-dev-utils[sqlalchemy_filters]>=1.11.0
+Requires-Dist: fastapi>=0.100; extra == "fastapi"
+Provides-Extra: fastapi
 Description-Content-Type: text/markdown
 
 # sqlrepo
 
 ![coverage](./coverage.svg)
 
 > Repository pattern implementation for SQLAlchemy models.
@@ -309,7 +311,111 @@
     __skip_session_use__ = True
 
 ...
 ```
 
 and this will cause no commit or other session manipulation (except session create for repositories
 work).
+
+## Extensions
+
+v1.5.0 now provided extensions for other technologies like web-frameworks. Now only FastAPI is
+supported.
+
+### FastAPI
+
+FastAPI extensions implements base classes for services and container, so you can work with your
+code easier.
+
+First of all You need to prepare all to work with plugin:
+
+```python
+from functools import cached_property
+
+from fastapi import FastAPI
+from sqlalchemy import create_engine
+from sqlalchemy.orm import DeclarativeBase, sessionmaker
+
+from sqlrepo import BaseSyncRepository
+
+engine = create_engine("<your-db-url-here>")
+Session = sessionmaker(engine)
+
+
+class Base(DeclarativeBase): ...
+
+
+class YourModel(Base):
+    # Your model definition
+    ...
+
+
+def get_session():
+    with Session() as session:
+        yield session
+
+
+app = FastAPI()
+```
+
+then you should use plugin like this:
+
+```python
+# your prepared code below
+
+from sqlrepo.ext.fastapi import add_container_overrides
+add_container_overrides(app, get_session)
+```
+
+then you can implements containers and services like this:
+
+```python
+# your prepared code below
+
+from pydantic import BaseModel, ConfigDict
+
+from sqlrepo.ext.fastapi import BaseSyncContainer, BaseSyncService
+
+
+class YourModelDetail(BaseModel):
+    model_config = ConfigDict(from_attributes=True)
+    ...
+
+
+class YourModelList(BaseModel):
+    model_config = ConfigDict(from_attributes=True)
+    ...
+
+
+class YourModelRepository(BaseSyncRepository[YourModel]):
+    def your_custom_repo_method(self) -> YourModel: ...
+
+
+class YourModelService(BaseSyncService[YourModel, YourModelDetail, YourModelList]):
+    detail_schema = YourModelDetail
+    list_schema = YourModelList
+    not_found_message = "YourModel entity not found in database"
+    not_found_exception = HTTPException
+
+    def init_repositories(self, session: "Session") -> None:
+        self.your_model_repo = YourModelRepository(session)
+
+    def your_custom_service_method(self) -> YourModelDetail:
+        return self.resolve(self.your_model_repo.your_custom_repo_method())
+
+
+class Container(BaseSyncContainer):
+
+    @cached_property
+    def your_model_service(self):
+        return YourModelService(self.session, self.request)
+```
+
+and finally you can use Container in your routes like this:
+
+```python
+# your prepared code below
+
+@app.get("/", response_model=YourModelDetail)
+def get_your_model(container: Container = Depends()):
+    return container.your_model_service.your_custom_service_method()
+```
```

