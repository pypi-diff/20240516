# Comparing `tmp/SqliteCloud-0.0.30.tar.gz` & `tmp/sqlitecloud-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SqliteCloud-0.0.30.tar", last modified: Mon Jan 15 11:18:31 2024, max compression
+gzip compressed data, was "sqlitecloud-0.0.74.tar", last modified: Thu May 16 16:04:41 2024, max compression
```

## Comparing `SqliteCloud-0.0.30.tar` & `sqlitecloud-0.0.74.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 11:18:31.837093 SqliteCloud-0.0.30/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-01-15 11:18:31.837093 SqliteCloud-0.0.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/README-PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 11:18:31.837093 SqliteCloud-0.0.30/SqliteCloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-01-15 11:18:31.000000 SqliteCloud-0.0.30/SqliteCloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-15 11:18:31.000000 SqliteCloud-0.0.30/SqliteCloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 11:18:31.000000 SqliteCloud-0.0.30/SqliteCloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-15 11:18:31.000000 SqliteCloud-0.0.30/SqliteCloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-15 11:18:31.000000 SqliteCloud-0.0.30/SqliteCloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 11:18:31.837093 SqliteCloud-0.0.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-15 11:18:24.000000 SqliteCloud-0.0.30/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 11:18:31.837093 SqliteCloud-0.0.30/sqlitecloud/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/sqlitecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/sqlitecloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/sqlitecloud/conn_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14714 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/sqlitecloud/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/sqlitecloud/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/sqlitecloud/resultset.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/sqlitecloud/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/sqlitecloud/vm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/sqlitecloud/wrapper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 11:18:31.837093 SqliteCloud-0.0.30/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-01-15 11:18:21.000000 SqliteCloud-0.0.30/tests/test_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/README-PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/SqliteCloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-16 16:04:38.000000 sqlitecloud-0.0.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/sqlitecloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/conn_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22420 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/resultset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22271 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/integration/test_driver.py
```

### Comparing `SqliteCloud-0.0.30/PKG-INFO` & `sqlitecloud-0.0.74/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqliteCloud
-Version: 0.0.30
+Version: 0.0.74
 Summary: A Python package for working with SQLite databases in the cloud.
 Home-page: https://github.com/sqlitecloud/python
 Author: Sam Reghenzi & Matteo Fredi
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SqliteCloud-0.0.30/README-PYPI.md` & `sqlitecloud-0.0.74/README-PYPI.md`

 * *Files identical despite different names*

### Comparing `SqliteCloud-0.0.30/SqliteCloud.egg-info/PKG-INFO` & `sqlitecloud-0.0.74/SqliteCloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqliteCloud
-Version: 0.0.30
+Version: 0.0.74
 Summary: A Python package for working with SQLite databases in the cloud.
 Home-page: https://github.com/sqlitecloud/python
 Author: Sam Reghenzi & Matteo Fredi
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SqliteCloud-0.0.30/setup.py` & `sqlitecloud-0.0.74/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         full_path = os.path.join(base_path, f'../{filename}')
         with io.open(full_path, encoding='utf-8') as file:
             return file.read()
 
 
 setup(
     name='SqliteCloud',
-    version='0.0.30',
+    version='0.0.74',
     author='Sam Reghenzi & Matteo Fredi',
     description='A Python package for working with SQLite databases in the cloud.',
     long_description=read_file('README-PYPI.md'),
     long_description_content_type='text/markdown',
     url="https://github.com/sqlitecloud/python",
     packages=find_packages(),
     install_requires=[
```

### Comparing `SqliteCloud-0.0.30/sqlitecloud/client.py` & `sqlitecloud-0.0.74/sqlitecloud/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,157 +1,150 @@
 """ Module to interact with remote SqliteCloud database
 
 """
-import ctypes
-from dataclasses import dataclass
-from typing import Any, List, Optional, Tuple
+from typing import Optional
+from urllib import parse
 
-from sqlitecloud.driver import (
+from sqlitecloud.driver import Driver
+from sqlitecloud.resultset import SqliteCloudResultSet
+from sqlitecloud.types import (
+    SQCloudConfig,
     SQCloudConnect,
-    SQCloudErrorMsg,
-    SQCloudIsError,
-    SQCloudExec,
-    SQCloudExecArray,
-    SQCloudConnectWithString,
-    SQCloudDisconnect,
-    SQCloudPubSubCB,
-    SQCloudResultDump,
-    SQCloudResultIsError,
-    SqlParameter,
+    SQCloudException,
+    SqliteCloudAccount,
 )
-from sqlitecloud.pubsub import SQCloudPubSubCallback, subscribe_pub_sub
-from sqlitecloud.resultset import SqliteCloudResultSet
-from sqlitecloud.wrapper_types import SQCloudConfig, SQCloudResult
-
-
-@dataclass
-class SqliteCloudAccount:
-    username: str
-    password: str
-    hostname: str
-    dbname: str
-    port: int
 
 
 class SqliteCloudClient:
     """
-    Client to connect to SqliteCloud
+    Client to interact with Sqlite Cloud
     """
 
-    _config: Optional[SQCloudConfig] = None
-    connection_str: Optional[str] = None
-    hostname: str
-    dbname: str
-    port: int
-    _pub_sub_cbs: List[Tuple[str, SQCloudPubSubCB]] = []
+    SQLITE_DEFAULT_PORT = 8860
 
     def __init__(
         self,
         cloud_account: Optional[SqliteCloudAccount] = None,
         connection_str: Optional[str] = None,
-        pub_subs: SQCloudPubSubCallback = [],
+        # pub_subs: SQCloudPubSubCallback = [],
     ) -> None:
-        """Initializes a new instance of the class.
+        """Initializes a new instance of the class with connection information.
 
         Args:
             connection_str (str): The connection string for the database.
-            uuid (UUID, optional): The UUID for the instance. Defaults to a new UUID generated using uuid4().
-
-        Raises:
-            ValueError: If the connection string is invalid.
 
         """
-        for pb in pub_subs:
-            self._pub_sub_cbs.append(("channel1", SQCloudPubSubCB(pb)))
+        self.driver = Driver()
+
+        self.config = SQCloudConfig()
+
         if connection_str:
-            self.connection_str = connection_str
+            self.config = self._parse_connection_string(connection_str)
         elif cloud_account:
-            self.config = SQCloudConfig()
-            self.config.username = self._encode_str_to_c(cloud_account.username)
-            self.config.password = self._encode_str_to_c(cloud_account.password)
-            self.hostname = cloud_account.hostname
-            self.dbname = cloud_account.dbname
-            self.port = cloud_account.port
-
+            self.config.account = cloud_account
         else:
-            raise Exception("Missing connection parameters")
-
-    def _encode_str_to_c(self, text):
-        return ctypes.c_char_p(text.encode("utf-8"))
+            raise SQCloudException("Missing connection parameters")
 
     def open_connection(self) -> SQCloudConnect:
         """Opens a connection to the SQCloud server.
 
         Returns:
             SQCloudConnect: An instance of the SQCloudConnect class representing the connection to the SQCloud server.
 
         Raises:
-            Exception: If an error occurs while opening the connection.
+            SQCloudException: If an error occurs while opening the connection.
         """
-
-        # Set other config properties...
-        connection = None
-        if self.connection_str:
-            connection = SQCloudConnectWithString(self.connection_str, None)
-        else:
-            connection = SQCloudConnect(
-                self._encode_str_to_c(self.hostname), self.port, self.config
-            )
-        self._check_connection(connection)
-        SQCloudExec(connection, self._encode_str_to_c(f"USE DATABASE {self.dbname};"))
-        self._check_connection(connection)
-        for cb in self._pub_sub_cbs:
-            subscribe_pub_sub(connection, cb[0], cb[1])
+        connection = self.driver.connect(
+            self.config.account.hostname, self.config.account.port, self.config
+        )
 
         return connection
 
-    def _check_connection(self, connection) -> None:
-        is_error = SQCloudIsError(connection)
-        if is_error:
-            error_message = SQCloudErrorMsg(connection)
-            print("An error occurred.", error_message.decode("utf-8"))
-            raise Exception(error_message)
-
     def disconnect(self, conn: SQCloudConnect) -> None:
-        """Closes the connection to the database.
-
-        This method is used to close the connection to the database. It does not take any arguments and does not return any value.
-
-        Returns:
-            None: This method does not return any value.
-        """
-        SQCloudDisconnect(conn)
+        """Close the connection to the database."""
+        self.driver.disconnect(conn)
 
     def exec_query(
         self, query: str, conn: SQCloudConnect = None
     ) -> SqliteCloudResultSet:
-        """Executes a SQL query on the SQLite database.
+        """Executes a SQL query on the SQLite Cloud database.
 
         Args:
             query (str): The SQL query to be executed.
 
         Returns:
             SqliteCloudResultSet: The result set of the executed query.
         """
-        print(query)
-        # pylint: disable=unused-variable
-        local_conn, close_at_end = (
-            (conn, False) if conn else (self.open_connection(), True)
-        )
-        result: SQCloudResult = SQCloudExec(local_conn, self._encode_str_to_c(query))
-        self._check_connection(local_conn)
+        provided_connection = conn is not None
+        if not provided_connection:
+            conn = self.open_connection()
+
+        result = self.driver.execute(query, conn)
+
+        if not provided_connection:
+            self.disconnect(conn)
+
         return SqliteCloudResultSet(result)
 
-    def exec_statement(
-        self, query: str, values: List[Any], conn: SQCloudConnect = None
-    ) -> SqliteCloudResultSet:
-        local_conn = conn if conn else self.open_connection()
-        result: SQCloudResult = SQCloudExecArray(
-            local_conn,
-            self._encode_str_to_c(query),
-            [SqlParameter(self._encode_str_to_c(str(v)), v) for v in values],
-        )
-        if SQCloudResultIsError(result):
-            raise Exception(
-                "Query error: " + str(SQCloudResultDump(local_conn, result))
+    def sendblob(self, blob: bytes, conn: SQCloudConnect) -> SqliteCloudResultSet:
+        """Sends a blob to the SQLite database.
+
+        Args:
+            blob (bytes): The blob to be sent to the database.
+            conn (SQCloudConnect): The connection to the database.
+        """
+        return self.driver.sendblob(blob, conn)
+
+    def _parse_connection_string(self, connection_string) -> SQCloudConfig:
+        # URL STRING FORMAT
+        # sqlitecloud://user:pass@host.com:port/dbname?timeout=10&key2=value2&key3=value3
+        # or sqlitecloud://host.sqlite.cloud:8860/dbname?apikey=zIiAARzKm9XBVllbAzkB1wqrgijJ3Gx0X5z1A4m4xBA
+
+        config = SQCloudConfig()
+        config.account = SqliteCloudAccount()
+
+        try:
+            params = parse.urlparse(connection_string)
+
+            options = {}
+            query = params.query
+            options = parse.parse_qs(query)
+            for option, values in options.items():
+                opt = option.lower()
+                value = values.pop()
+
+                if value.lower() in ["true", "false"]:
+                    value = bool(value)
+                elif value.isdigit():
+                    value = int(value)
+                else:
+                    value = value
+
+                if hasattr(config, opt):
+                    setattr(config, opt, value)
+                elif hasattr(config.account, opt):
+                    setattr(config.account, opt, value)
+
+            # apikey or username/password is accepted
+            if not config.account.apikey:
+                config.account.username = (
+                    parse.unquote(params.username) if params.username else ""
+                )
+                config.account.password = (
+                    parse.unquote(params.password) if params.password else ""
+                )
+
+            path = params.path
+            database = path.strip("/")
+            if database:
+                config.account.dbname = database
+
+            config.account.hostname = params.hostname
+            config.account.port = (
+                int(params.port) if params.port else self.SQLITE_DEFAULT_PORT
             )
-        return SqliteCloudResultSet(result)
+
+            return config
+        except Exception as e:
+            raise SQCloudException(
+                f"Invalid connection string {connection_string}"
+            ) from e
```

