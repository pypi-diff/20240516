# Comparing `tmp/dataclasses_ujson-0.0.5.tar.gz` & `tmp/dataclasses_ujson-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_ujson-0.0.5.tar", last modified: Tue Nov 16 19:30:06 2021, max compression
+gzip compressed data, was "dataclasses_ujson-0.0.8.tar", last modified: Wed Nov 17 07:52:38 2021, max compression
```

## Comparing `dataclasses_ujson-0.0.5.tar` & `dataclasses_ujson-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 artem     (1000) artem     (1000)        0 2021-11-16 19:30:06.615340 dataclasses_ujson-0.0.5/
--rw-rw-r--   0 artem     (1000) artem     (1000)     2944 2021-11-16 19:30:06.615340 dataclasses_ujson-0.0.5/PKG-INFO
-drwxrwxr-x   0 artem     (1000) artem     (1000)        0 2021-11-16 19:30:06.611340 dataclasses_ujson-0.0.5/dataclasses_ujson/
--rw-rw-r--   0 artem     (1000) artem     (1000)        0 2021-11-16 17:21:24.000000 dataclasses_ujson-0.0.5/dataclasses_ujson/__init__.py
--rw-rw-r--   0 artem     (1000) artem     (1000)     3307 2021-11-16 19:28:51.000000 dataclasses_ujson-0.0.5/dataclasses_ujson/dataclasses_ujson.py
-drwxrwxr-x   0 artem     (1000) artem     (1000)        0 2021-11-16 19:30:06.611340 dataclasses_ujson-0.0.5/dataclasses_ujson.egg-info/
--rw-rw-r--   0 artem     (1000) artem     (1000)     2944 2021-11-16 19:30:06.000000 dataclasses_ujson-0.0.5/dataclasses_ujson.egg-info/PKG-INFO
--rw-rw-r--   0 artem     (1000) artem     (1000)      291 2021-11-16 19:30:06.000000 dataclasses_ujson-0.0.5/dataclasses_ujson.egg-info/SOURCES.txt
--rw-rw-r--   0 artem     (1000) artem     (1000)        1 2021-11-16 19:30:06.000000 dataclasses_ujson-0.0.5/dataclasses_ujson.egg-info/dependency_links.txt
--rw-rw-r--   0 artem     (1000) artem     (1000)       26 2021-11-16 19:30:06.000000 dataclasses_ujson-0.0.5/dataclasses_ujson.egg-info/requires.txt
--rw-rw-r--   0 artem     (1000) artem     (1000)       18 2021-11-16 19:30:06.000000 dataclasses_ujson-0.0.5/dataclasses_ujson.egg-info/top_level.txt
--rw-rw-r--   0 artem     (1000) artem     (1000)       63 2021-11-16 19:30:06.615340 dataclasses_ujson-0.0.5/setup.cfg
--rw-rw-r--   0 artem     (1000) artem     (1000)      829 2021-11-16 19:29:54.000000 dataclasses_ujson-0.0.5/setup.py
+drwxrwxr-x   0 artem     (1000) artem     (1000)        0 2021-11-17 07:52:38.834467 dataclasses_ujson-0.0.8/
+-rw-rw-r--   0 artem     (1000) artem     (1000)     2944 2021-11-17 07:52:38.834467 dataclasses_ujson-0.0.8/PKG-INFO
+drwxrwxr-x   0 artem     (1000) artem     (1000)        0 2021-11-17 07:52:38.830467 dataclasses_ujson-0.0.8/dataclasses_ujson/
+-rw-rw-r--   0 artem     (1000) artem     (1000)        0 2021-11-16 17:21:24.000000 dataclasses_ujson-0.0.8/dataclasses_ujson/__init__.py
+-rw-rw-r--   0 artem     (1000) artem     (1000)     3317 2021-11-17 07:51:33.000000 dataclasses_ujson-0.0.8/dataclasses_ujson/dataclasses_ujson.py
+drwxrwxr-x   0 artem     (1000) artem     (1000)        0 2021-11-17 07:52:38.834467 dataclasses_ujson-0.0.8/dataclasses_ujson.egg-info/
+-rw-rw-r--   0 artem     (1000) artem     (1000)     2944 2021-11-17 07:52:38.000000 dataclasses_ujson-0.0.8/dataclasses_ujson.egg-info/PKG-INFO
+-rw-rw-r--   0 artem     (1000) artem     (1000)      291 2021-11-17 07:52:38.000000 dataclasses_ujson-0.0.8/dataclasses_ujson.egg-info/SOURCES.txt
+-rw-rw-r--   0 artem     (1000) artem     (1000)        1 2021-11-17 07:52:38.000000 dataclasses_ujson-0.0.8/dataclasses_ujson.egg-info/dependency_links.txt
+-rw-rw-r--   0 artem     (1000) artem     (1000)       26 2021-11-17 07:52:38.000000 dataclasses_ujson-0.0.8/dataclasses_ujson.egg-info/requires.txt
+-rw-rw-r--   0 artem     (1000) artem     (1000)       18 2021-11-17 07:52:38.000000 dataclasses_ujson-0.0.8/dataclasses_ujson.egg-info/top_level.txt
+-rw-rw-r--   0 artem     (1000) artem     (1000)       63 2021-11-17 07:52:38.834467 dataclasses_ujson-0.0.8/setup.cfg
+-rw-rw-r--   0 artem     (1000) artem     (1000)      829 2021-11-17 07:52:16.000000 dataclasses_ujson-0.0.8/setup.py
```

### Comparing `dataclasses_ujson-0.0.5/PKG-INFO` & `dataclasses_ujson-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses_ujson
-Version: 0.0.5
+Version: 0.0.8
 Summary: fast converter your json to dataclass
 Home-page: https://github.com/kislenko-artem/dataclasses-ujson
 Author: Kislenko Artem 
 Author-email: artem@webart-tech.ru
 License: Apache
 Description: # Install
```

### Comparing `dataclasses_ujson-0.0.5/dataclasses_ujson/dataclasses_ujson.py` & `dataclasses_ujson-0.0.8/dataclasses_ujson/dataclasses_ujson.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from dataclasses import is_dataclass, dataclass
+from dataclasses import is_dataclass
 import sys
-from typing import Any, Generator, List, Union
+from typing import Any, Generator, TypeVar, Type, Union
 
 NEW_TYPING = sys.version_info[:3] >= (3, 7, 0)  # PEP 560
 if NEW_TYPING:
     from typing import _GenericAlias as GenericMeta
 else:
     from typing import GenericMeta
 
 import ujson as json
 
-DC = dataclass
-DC_GENERATOR = Generator[List[DC], List[DC], None]
+DC = TypeVar('DC')
+DC_GENERATOR = Generator[Type[DC], None, None]
 
 
 class UJsonMixin:
 
     @classmethod
     def loads(cls: DC, json_string: str, many: bool = False,
-              **kwargs) -> Union[DC, DC_GENERATOR]:
+              **kwargs) -> Union[Type[DC], DC_GENERATOR]:
         """
 
         :param json_string: string of json, what should be encoded
         :param many: true if it is list. For example: [{"x": 1}, {"x": 2}]
         :param kwargs: other arguments to json.loads
         :return: Union[DC, DC_GENERATOR]
         """
@@ -31,15 +31,15 @@
             return UJsonMixin.from_dict_many(cls, data)
         return UJsonMixin.from_dict(cls, data)
 
     def dumps(self):
         raise NotImplemented()
 
     @staticmethod
-    def from_dict(cls: DC, data: dict, _kwargs: dict = None) -> DC:
+    def from_dict(cls: DC, data: dict, _kwargs: dict = None) -> Type[DC]:
         if _kwargs is None:
             _kwargs = {}
         try:
             for field in getattr(cls, '__dataclass_fields__').values():
                 field_value = data.get(field.name)
                 if field_value is None:
                     _kwargs[field.name] = None
```

### Comparing `dataclasses_ujson-0.0.5/dataclasses_ujson.egg-info/PKG-INFO` & `dataclasses_ujson-0.0.8/dataclasses_ujson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-ujson
-Version: 0.0.5
+Version: 0.0.8
 Summary: fast converter your json to dataclass
 Home-page: https://github.com/kislenko-artem/dataclasses-ujson
 Author: Kislenko Artem 
 Author-email: artem@webart-tech.ru
 License: Apache
 Description: # Install
```

### Comparing `dataclasses_ujson-0.0.5/setup.py` & `dataclasses_ujson-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "ReadMe.md").read_text()
 
 setup(
     name="dataclasses_ujson",
-    version="0.0.5",
+    version="0.0.8",
     packages=find_packages(exclude=("tests*","bench_marks.py")),
     author="Kislenko Artem ",
     author_email="artem@webart-tech.ru",
     description="fast converter your json to dataclass",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/kislenko-artem/dataclasses-ujson",
```

