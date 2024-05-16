# Comparing `tmp/bstk_notitia-0.3.0.tar.gz` & `tmp/bstk_notitia-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_notitia-0.3.0.tar", max compression
+gzip compressed data, was "bstk_notitia-0.4.0.tar", max compression
```

## Comparing `bstk_notitia-0.3.0.tar` & `bstk_notitia-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1705 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/README.md
--rw-r--r--   0        0        0     1080 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/__init__.py
--rw-r--r--   0        0        0      903 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/error.py
--rw-r--r--   0        0        0     1430 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/driver.py
--rw-r--r--   0        0        0     1086 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/informant.py
--rw-r--r--   0        0        0     5381 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/investigator.py
--rw-r--r--   0        0        0     2037 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/observer.py
--rw-r--r--   0        0        0     1309 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/lib/abc/reporter.py
--rw-r--r--   0        0        0     9185 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/loader.py
--rw-r--r--   0        0        0     5974 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/driver/mongodb.py
--rw-r--r--   0        0        0      565 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/driver/null.py
--rw-r--r--   0        0        0     2463 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/driver/passthrough.py
--rw-r--r--   0        0        0      745 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/informant/internal/datetime.py
--rw-r--r--   0        0        0      400 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/informant/internal/http.py
--rw-r--r--   0        0        0     1466 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/investigator/internal/clock.py
--rw-r--r--   0        0        0     2205 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py
--rw-r--r--   0        0        0     1605 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/mongo_collection_change.py
--rw-r--r--   0        0        0     1434 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/mongo_record.py
--rw-r--r--   0        0        0     1460 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/tick.py
--rw-r--r--   0        0        0      697 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/echo.py
--rw-r--r--   0        0        0     3018 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/mongo_record.py
--rw-r--r--   0        0        0     4025 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/notitia_case.py
--rw-r--r--   0        0        0    10357 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/notitia.py
--rw-r--r--   0        0        0    15705 2024-05-14 01:30:06.253910 bstk_notitia-0.3.0/bstk_notitia/roster.py
--rw-r--r--   0        0        0      815 2024-05-14 01:30:21.481951 bstk_notitia-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2307 1970-01-01 00:00:00.000000 bstk_notitia-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1705 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/README.md
+-rw-r--r--   0        0        0     1080 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/__init__.py
+-rw-r--r--   0        0        0      903 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/error.py
+-rw-r--r--   0        0        0     1430 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/driver.py
+-rw-r--r--   0        0        0     1086 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/informant.py
+-rw-r--r--   0        0        0     5381 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/investigator.py
+-rw-r--r--   0        0        0     2037 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/observer.py
+-rw-r--r--   0        0        0     1309 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/reporter.py
+-rw-r--r--   0        0        0     9185 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/loader.py
+-rw-r--r--   0        0        0     8904 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/driver/mongodb.py
+-rw-r--r--   0        0        0      565 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/driver/null.py
+-rw-r--r--   0        0        0     2463 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/driver/passthrough.py
+-rw-r--r--   0        0        0      745 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/informant/internal/datetime.py
+-rw-r--r--   0        0        0      400 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/informant/internal/http.py
+-rw-r--r--   0        0        0     1466 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/clock.py
+-rw-r--r--   0        0        0     1895 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py
+-rw-r--r--   0        0        0     3313 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/notitia_casereporter.py
+-rw-r--r--   0        0        0     1648 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_changestream.py
+-rw-r--r--   0        0        0     3532 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_collectionstream.py
+-rw-r--r--   0        0        0     1434 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_record.py
+-rw-r--r--   0        0        0     1460 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/tick.py
+-rw-r--r--   0        0        0      697 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/echo.py
+-rw-r--r--   0        0        0     3018 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/mongo_record.py
+-rw-r--r--   0        0        0     4025 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/notitia_case.py
+-rw-r--r--   0        0        0    10357 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/notitia.py
+-rw-r--r--   0        0        0    15705 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/roster.py
+-rw-r--r--   0        0        0      815 2024-05-16 01:18:06.456922 bstk_notitia-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2307 1970-01-01 00:00:00.000000 bstk_notitia-0.4.0/PKG-INFO
```

### Comparing `bstk_notitia-0.3.0/README.md` & `bstk_notitia-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/__init__.py` & `bstk_notitia-0.4.0/bstk_notitia/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/error.py` & `bstk_notitia-0.4.0/bstk_notitia/error.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/lib/abc/driver.py` & `bstk_notitia-0.4.0/bstk_notitia/lib/abc/driver.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/lib/abc/informant.py` & `bstk_notitia-0.4.0/bstk_notitia/lib/abc/informant.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/lib/abc/investigator.py` & `bstk_notitia-0.4.0/bstk_notitia/lib/abc/investigator.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/lib/abc/observer.py` & `bstk_notitia-0.4.0/bstk_notitia/lib/abc/observer.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/lib/abc/reporter.py` & `bstk_notitia-0.4.0/bstk_notitia/lib/abc/reporter.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/loader.py` & `bstk_notitia-0.4.0/bstk_notitia/loader.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/driver/null.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/driver/null.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/driver/passthrough.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/driver/passthrough.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/informant/internal/datetime.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/informant/internal/datetime.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/investigator/internal/clock.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/clock.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 import typing
-from uuid import uuid4
 from bstk_notitia.lib.abc.investigator import InvestigatorABC
 
 if typing.TYPE_CHECKING:
     import datetime
     from modules.driver.mongodb import NotitiaModule as MongoDBDriver, DriverABC
 
 """
@@ -50,23 +49,14 @@
 
 class NotitiaModule(InvestigatorABC):
     name = "Internal MongoDB Record Collector"
     key = "internal/mongo_record_processor"
     driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
 
     async def start(self, **kwargs):
-        res = await self.reporter["internal/mongo_record"].receive(
-            action="insert",
-            record=None,
-            data={
-                "uuid": str(uuid4()),
-                "collected": False,
-                "department": self.department,
-            },
-        )
 
         async for document in self.observer["internal/mongo_record"].monitor():
             data: datetime.datetime = await self.informant[
                 "internal/datetime"
             ].enquire()
             res = await self.reporter["internal/mongo_record"].receive(
                 action="update",
```

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/mongo_collection_change.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_changestream.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,41 +15,40 @@
     }
 }
 
 
 @dataclass
 class NotitiaModule(ObserverABC):
     name = "Internal MongoDB Changestream"
-    key = "internal/mongodb_collection_change"
+    key = "internal/mongodb_changestream"
     resume_token: typing.AnyStr = field(init=False, default=None)
 
     if typing.TYPE_CHECKING:
         driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
 
     async def glance(self, document: typing.Dict) -> typing.Union[None, typing.Dict]:
-        if "fullDocument" not in document:
-            return None
-        return document["fullDocument"]
+        return document.get("fullDocument", None)
 
     async def monitor(
         self,
         collection: typing.AnyStr,
-        options: typing.Optional[typing.Dict] = None,
         lookup: typing.Optional[typing.Dict] = None,
+        options: typing.Optional[typing.Dict] = None,
     ) -> typing.AsyncGenerator[bson.RawBSONDocument, None]:
         _pipeline = []
         if lookup:
             _pipeline.append(lookup)
 
-        async for token, change in self.driver["mongodb"].watch(
-            collection=collection,
+        _collection = self.driver["mongodb"].get_collection(collection)
+        change_stream = self.driver["mongodb"].change_stream(
+            collection=_collection,
             pipeline=_pipeline,
-            resume_token=self.resume_token,
             **options,
-        ):
+        )
+        async for token, change in self.driver["mongodb"].watch(change_stream):
             self.resume_token = token
             if not change:
                 return
 
             doc = await self.glance(change[1])
             if not doc:
                 continue
```

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/mongo_record.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_record.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/observer/internal/tick.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/tick.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/echo.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/echo.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/mongo_record.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/mongo_record.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/modules/reporter/internal/notitia_case.py` & `bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/notitia_case.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/notitia.py` & `bstk_notitia-0.4.0/bstk_notitia/notitia.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/bstk_notitia/roster.py` & `bstk_notitia-0.4.0/bstk_notitia/roster.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.3.0/pyproject.toml` & `bstk_notitia-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk_notitia"
-version = "0.3.0"
+version = "0.4.0"
 description = "notitia core runtime & modules"
 authors = ["colin <colin@broadstack.com.au>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = { extras = ["cli"], version = "^1.0.0" }
```

### Comparing `bstk_notitia-0.3.0/PKG-INFO` & `bstk_notitia-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk_notitia
-Version: 0.3.0
+Version: 0.4.0
 Summary: notitia core runtime & modules
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

