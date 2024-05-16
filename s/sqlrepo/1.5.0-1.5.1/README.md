# Comparing `tmp/sqlrepo-1.5.0.tar.gz` & `tmp/sqlrepo-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlrepo-1.5.0.tar", last modified: Thu May 16 07:26:31 2024, max compression
+gzip compressed data, was "sqlrepo-1.5.1.tar", last modified: Thu May 16 08:11:39 2024, max compression
```

## Comparing `sqlrepo-1.5.0.tar` & `sqlrepo-1.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    12676 2024-05-16 07:23:01.665324 sqlrepo-1.5.0/README.md
--rw-r--r--   0        0        0     3124 2024-05-16 07:26:31.549223 sqlrepo-1.5.0/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/README.md
--rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.5.0/sqlrepo/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.5.0/sqlrepo/__init__.py
--rw-r--r--   0        0        0      828 2024-04-22 06:04:46.395911 sqlrepo-1.5.0/sqlrepo/exc.py
--rw-r--r--   0        0        0        0 2024-05-15 07:58:11.149780 sqlrepo-1.5.0/sqlrepo/ext/__init__.py
--rw-r--r--   0        0        0      368 2024-05-16 07:19:23.476470 sqlrepo-1.5.0/sqlrepo/ext/fastapi/__init__.py
--rw-r--r--   0        0        0     1706 2024-05-16 07:17:37.081028 sqlrepo-1.5.0/sqlrepo/ext/fastapi/containers.py
--rw-r--r--   0        0        0      186 2024-05-16 07:10:05.345399 sqlrepo-1.5.0/sqlrepo/ext/fastapi/helpers.py
--rw-r--r--   0        0        0     7935 2024-05-16 07:04:51.952120 sqlrepo-1.5.0/sqlrepo/ext/fastapi/services.py
--rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.5.0/sqlrepo/logging.py
--rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.5.0/sqlrepo/py.typed
--rw-r--r--   0        0        0    32880 2024-04-22 06:04:46.396911 sqlrepo-1.5.0/sqlrepo/queries.py
--rw-r--r--   0        0        0    23853 2024-04-22 06:04:46.396911 sqlrepo-1.5.0/sqlrepo/repositories.py
--rw-r--r--   0        0        0     4696 2024-04-22 06:04:46.396911 sqlrepo-1.5.0/sqlrepo/uow.py
--rw-r--r--   0        0        0     1202 2024-05-15 13:59:23.791626 sqlrepo-1.5.0/sqlrepo/wrappers.py
--rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-1.5.0/tests/test_async_queries.py
--rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-1.5.0/tests/test_async_repositories.py
--rw-r--r--   0        0        0     1771 2024-04-22 06:04:46.396911 sqlrepo-1.5.0/tests/test_async_uow.py
--rw-r--r--   0        0        0    17037 2024-04-22 06:04:46.397911 sqlrepo-1.5.0/tests/test_base_queries.py
--rw-r--r--   0        0        0     2983 2024-04-22 06:04:46.397911 sqlrepo-1.5.0/tests/test_base_repositories.py
--rw-r--r--   0        0        0    10769 2024-05-16 07:09:22.500629 sqlrepo-1.5.0/tests/test_fastapi_ext.py
--rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-1.5.0/tests/test_sync_queries.py
--rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-1.5.0/tests/test_sync_repositories.py
--rw-r--r--   0        0        0     1540 2024-04-22 06:04:46.397911 sqlrepo-1.5.0/tests/test_sync_uow.py
--rw-r--r--   0        0        0     1061 2024-04-22 06:04:46.397911 sqlrepo-1.5.0/tests/test_wrappers.py
--rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.5.0/tests/types.py
--rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-1.5.0/tests/utils.py
--rw-r--r--   0        0        0    13104 1970-01-01 00:00:00.000000 sqlrepo-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    12676 2024-05-16 07:23:01.665324 sqlrepo-1.5.1/README.md
+-rw-r--r--   0        0        0     3124 2024-05-16 08:11:39.433962 sqlrepo-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.5.1/sqlrepo/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.5.1/sqlrepo/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.5.1/sqlrepo/.pytest_cache/README.md
+-rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.5.1/sqlrepo/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.5.1/sqlrepo/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.5.1/sqlrepo/__init__.py
+-rw-r--r--   0        0        0      828 2024-04-22 06:04:46.395911 sqlrepo-1.5.1/sqlrepo/exc.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:58:11.149780 sqlrepo-1.5.1/sqlrepo/ext/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-16 07:19:23.476470 sqlrepo-1.5.1/sqlrepo/ext/fastapi/__init__.py
+-rw-r--r--   0        0        0     1835 2024-05-16 08:10:46.838226 sqlrepo-1.5.1/sqlrepo/ext/fastapi/containers.py
+-rw-r--r--   0        0        0      186 2024-05-16 07:10:05.345399 sqlrepo-1.5.1/sqlrepo/ext/fastapi/helpers.py
+-rw-r--r--   0        0        0     7935 2024-05-16 07:04:51.952120 sqlrepo-1.5.1/sqlrepo/ext/fastapi/services.py
+-rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.5.1/sqlrepo/logging.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.5.1/sqlrepo/py.typed
+-rw-r--r--   0        0        0    32880 2024-04-22 06:04:46.396911 sqlrepo-1.5.1/sqlrepo/queries.py
+-rw-r--r--   0        0        0    23853 2024-04-22 06:04:46.396911 sqlrepo-1.5.1/sqlrepo/repositories.py
+-rw-r--r--   0        0        0     4696 2024-04-22 06:04:46.396911 sqlrepo-1.5.1/sqlrepo/uow.py
+-rw-r--r--   0        0        0     1202 2024-05-15 13:59:23.791626 sqlrepo-1.5.1/sqlrepo/wrappers.py
+-rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.5.1/tests/conftest.py
+-rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-1.5.1/tests/test_async_queries.py
+-rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-1.5.1/tests/test_async_repositories.py
+-rw-r--r--   0        0        0     1771 2024-04-22 06:04:46.396911 sqlrepo-1.5.1/tests/test_async_uow.py
+-rw-r--r--   0        0        0    17037 2024-04-22 06:04:46.397911 sqlrepo-1.5.1/tests/test_base_queries.py
+-rw-r--r--   0        0        0     2983 2024-04-22 06:04:46.397911 sqlrepo-1.5.1/tests/test_base_repositories.py
+-rw-r--r--   0        0        0    10769 2024-05-16 07:09:22.500629 sqlrepo-1.5.1/tests/test_fastapi_ext.py
+-rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-1.5.1/tests/test_sync_queries.py
+-rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-1.5.1/tests/test_sync_repositories.py
+-rw-r--r--   0        0        0     1540 2024-04-22 06:04:46.397911 sqlrepo-1.5.1/tests/test_sync_uow.py
+-rw-r--r--   0        0        0     1061 2024-04-22 06:04:46.397911 sqlrepo-1.5.1/tests/test_wrappers.py
+-rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.5.1/tests/types.py
+-rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-1.5.1/tests/utils.py
+-rw-r--r--   0        0        0    13104 1970-01-01 00:00:00.000000 sqlrepo-1.5.1/PKG-INFO
```

### Comparing `sqlrepo-1.5.0/README.md` & `sqlrepo-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/pyproject.toml` & `sqlrepo-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     "httpx>=0.27.0",
     "pyment>=0.3.3",
     "ipython>=8.19.0",
 ]
 
 [project]
 name = "sqlrepo"
-version = "1.5.0"
+version = "1.5.1"
 description = "sqlalchemy repositories with crud operations and other utils for it."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
```

### Comparing `sqlrepo-1.5.0/sqlrepo/exc.py` & `sqlrepo-1.5.1/sqlrepo/exc.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/sqlrepo/ext/fastapi/containers.py` & `sqlrepo-1.5.1/sqlrepo/ext/fastapi/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from typing import TYPE_CHECKING, Protocol
 
 from fastapi import Depends, Request
 
 if TYPE_CHECKING:
+    from collections.abc import AsyncGenerator, Generator
+
     from fastapi import FastAPI
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm.session import Session
 
     class SyncSessionDependsProtocol(Protocol):
         """Sync session depends protocol for FastAPI framework."""
 
         @staticmethod
-        def __call__() -> Session: ...  # noqa: D102
+        def __call__() -> Session | Generator[Session, None, None]: ...  # noqa: D102
 
     class AsyncSessionDependsProtocol(Protocol):
         """Async session depends protocol for FastAPI framework."""
 
         @staticmethod
-        async def __call__() -> AsyncSession: ...  # noqa: D102
+        async def __call__() -> AsyncSession | AsyncGenerator[AsyncSession, None]: ...  # noqa: D102
 
 
 def _get_session_stub() -> None:
     """Stub function, that will be overridden by main plug functions."""
 
 
 def add_container_overrides(
```

### Comparing `sqlrepo-1.5.0/sqlrepo/ext/fastapi/services.py` & `sqlrepo-1.5.1/sqlrepo/ext/fastapi/services.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/sqlrepo/logging.py` & `sqlrepo-1.5.1/sqlrepo/logging.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/sqlrepo/queries.py` & `sqlrepo-1.5.1/sqlrepo/queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/sqlrepo/repositories.py` & `sqlrepo-1.5.1/sqlrepo/repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/sqlrepo/uow.py` & `sqlrepo-1.5.1/sqlrepo/uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/sqlrepo/wrappers.py` & `sqlrepo-1.5.1/sqlrepo/wrappers.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/conftest.py` & `sqlrepo-1.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_async_queries.py` & `sqlrepo-1.5.1/tests/test_async_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_async_repositories.py` & `sqlrepo-1.5.1/tests/test_async_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_async_uow.py` & `sqlrepo-1.5.1/tests/test_async_uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_base_queries.py` & `sqlrepo-1.5.1/tests/test_base_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_base_repositories.py` & `sqlrepo-1.5.1/tests/test_base_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_fastapi_ext.py` & `sqlrepo-1.5.1/tests/test_fastapi_ext.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_sync_queries.py` & `sqlrepo-1.5.1/tests/test_sync_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_sync_repositories.py` & `sqlrepo-1.5.1/tests/test_sync_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_sync_uow.py` & `sqlrepo-1.5.1/tests/test_sync_uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/test_wrappers.py` & `sqlrepo-1.5.1/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/types.py` & `sqlrepo-1.5.1/tests/types.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/tests/utils.py` & `sqlrepo-1.5.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.0/PKG-INFO` & `sqlrepo-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlrepo
-Version: 1.5.0
+Version: 1.5.1
 Summary: sqlalchemy repositories with crud operations and other utils for it.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: sqlalchemy>=2.0.29
 Requires-Dist: python-dev-utils[sqlalchemy_filters]>=1.11.0
 Requires-Dist: fastapi>=0.100; extra == "fastapi"
```

