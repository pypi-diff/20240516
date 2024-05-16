# Comparing `tmp/cherry_orm-0.3.0.tar.gz` & `tmp/cherry_orm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherry_orm-0.3.0.tar", max compression
+gzip compressed data, was "cherry_orm-1.0.0.tar", max compression
```

## Comparing `cherry_orm-0.3.0.tar` & `cherry_orm-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1058 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/LICENSE
--rw-r--r--   0        0        0     3393 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/README.md
--rw-r--r--   0        0        0      682 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/__init__.py
--rw-r--r--   0        0        0       41 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/database/__init__.py
--rw-r--r--   0        0        0     3247 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/database/engine.py
--rw-r--r--   0        0        0     1430 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/exception.py
--rw-r--r--   0        0        0      600 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/fields/__init__.py
--rw-r--r--   0        0        0     1010 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/fields/annotated.py
--rw-r--r--   0        0        0    10704 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/fields/fields.py
--rw-r--r--   0        0        0     8884 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/fields/proxy.py
--rw-r--r--   0        0        0     5622 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/fields/types.py
--rw-r--r--   0        0        0     2461 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/fields/utils.py
--rw-r--r--   0        0        0      280 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/helpers.py
--rw-r--r--   0        0        0       95 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/meta/__init__.py
--rw-r--r--   0        0        0      811 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/meta/constraint.py
--rw-r--r--   0        0        0      421 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/meta/index.py
--rw-r--r--   0        0        0     2012 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/meta/meta.py
--rw-r--r--   0        0        0      649 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/meta/pydantic_config.py
--rw-r--r--   0        0        0       35 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/models/__init__.py
--rw-r--r--   0        0        0    47190 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/models/models.py
--rw-r--r--   0        0        0       43 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/queryset/__init__.py
--rw-r--r--   0        0        0      365 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/queryset/protocol.py
--rw-r--r--   0        0        0    26680 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/queryset/queryset.py
--rw-r--r--   0        0        0     1093 2023-12-12 10:12:28.754666 cherry_orm-0.3.0/cherry/typing.py
--rw-r--r--   0        0        0     2268 2023-12-12 10:12:28.758666 cherry_orm-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4706 1970-01-01 00:00:00.000000 cherry_orm-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3407 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/README.md
+-rw-r--r--   0        0        0      686 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/__init__.py
+-rw-r--r--   0        0        0       41 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/database/__init__.py
+-rw-r--r--   0        0        0     3364 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/database/engine.py
+-rw-r--r--   0        0        0     1430 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/exception.py
+-rw-r--r--   0        0        0      600 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/fields/__init__.py
+-rw-r--r--   0        0        0      981 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/fields/annotated.py
+-rw-r--r--   0        0        0    11714 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/fields/fields.py
+-rw-r--r--   0        0        0     8872 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/fields/proxy.py
+-rw-r--r--   0        0        0     6392 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/fields/types.py
+-rw-r--r--   0        0        0     2390 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/fields/utils.py
+-rw-r--r--   0        0        0      280 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/helpers.py
+-rw-r--r--   0        0        0      101 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/meta/__init__.py
+-rw-r--r--   0        0        0     3606 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/meta/config.py
+-rw-r--r--   0        0        0      415 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/meta/index.py
+-rw-r--r--   0        0        0     1971 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/meta/meta.py
+-rw-r--r--   0        0        0       35 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/models/__init__.py
+-rw-r--r--   0        0        0    47303 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/models/models.py
+-rw-r--r--   0        0        0       43 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/queryset/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/queryset/protocol.py
+-rw-r--r--   0        0        0    28729 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/queryset/queryset.py
+-rw-r--r--   0        0        0     1075 2024-05-16 03:17:26.433917 cherry_orm-1.0.0/cherry/typing.py
+-rw-r--r--   0        0        0     2458 2024-05-16 03:17:26.437917 cherry_orm-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4668 1970-01-01 00:00:00.000000 cherry_orm-1.0.0/PKG-INFO
```

### Comparing `cherry_orm-0.3.0/LICENSE` & `cherry_orm-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cherry_orm-0.3.0/README.md` & `cherry_orm-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,39 +6,39 @@
     <a href="./LICENSE">
         <img src="https://img.shields.io/github/license/CMHopeSunshine/cherry-orm.svg" alt="license">
     </a>
     <a href="https://pypi.python.org/pypi/cherry-orm">
         <img src="https://img.shields.io/pypi/v/cherry-orm.svg" alt="pypi">
     </a>
     <a href="https://www.python.org/">
-        <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+        <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     </a>
 </p>
 
 <p align="center">
     <strong>简体中文</strong>
     ·
     <a href="https://github.com/CMHopeSunshine/cherry-orm/blob/master/README_EN.md">English</a>
 </p>
 
 ## 简介
 
-`Cherry ORM` 是一个 Python 的异步对象关系映射（ORM）库，它基于 [SQLAlchemy Core](https://www.sqlalchemy.org/) 和 [Pydantic V1](https://docs.pydantic.dev/1.10/) 构建。
+`Cherry ORM` 是一个 Python 的异步对象关系映射（ORM）库，它基于 [SQLAlchemy Core](https://www.sqlalchemy.org/) 和 [Pydantic V2](https://docs.pydantic.dev/latest/) 构建。
 
 它的一切设计都是为了简单易用，极大地减少开发者的数据库操作成本，提高开发效率，让开发者更专注于业务逻辑的实现。
 
 ## 安装
 
 - 使用 pip: `pip install cherry-orm`
 - 使用 Poetry: `poetry add cherry-orm`
 - 使用 PDM: `pdm add cherry-orm`
 
 ## 文档
 
--> [文档地址](https://cherry.cherishmoon.fun)
+-> [文档地址](https://cherry.cherishmoon.top)
 
 ## 示例
 
 ```python
 from datetime import date
 from typing import List, Optional
 
@@ -50,27 +50,23 @@
 class Student(cherry.Model):
     id: int = cherry.Field(primary_key=True)
     name: str = cherry.Field(unique=True, index=True)
     age: int
     birthday: date = cherry.Field(default_factory=date.today)
     school: cherry.ForeignKey[Optional["School"]] = None
 
-    class Meta:
-        database = db
-        tablename = "student"
+    cherry_config = cherry.CherryConfig(tablename="student", database=db)
 
 
 class School(cherry.Model):
     id: cherry.PrimaryKey[int]
     name: str = cherry.Field(unique=True, index=True)
     students: cherry.ReverseRelation[List[Student]] = []
 
-    class Meta:
-        database = db
-        tablename = "school"
+    cherry_config = cherry.CherryConfig(tablename="school", database=db)
 
 
 async def main():
     await db.init()
 
     # 插入
     school = await School(id=1, name="school 1").insert()
```

### Comparing `cherry_orm-0.3.0/cherry/__init__.py` & `cherry_orm-1.0.0/cherry/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     ManyToMany as ManyToMany,
     PrimaryKey as PrimaryKey,
     Relationship as Relationship,
     ReverseRelation as ReverseRelation,
     Unique as Unique,
 )
 from .meta import (
+    CherryConfig as CherryConfig,
     CompositeIndex as CompositeIndex,
-    MetaConfig as MetaConfig,
 )
 from .models import Model as Model
 from .typing import (
     CASCADE as CASCADE,
     NO_ACTION as NO_ACTION,
     RESTRICT as RESTRICT,
     SET_DEFAULT as SET_DEFAULT,
```

### Comparing `cherry_orm-0.3.0/cherry/database/engine.py` & `cherry_orm-1.0.0/cherry/database/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import Any, Dict, Optional, Type, TYPE_CHECKING, Union
+from typing import Any, Optional, TYPE_CHECKING, Union
 
 from sqlalchemy import Engine, event, make_url, MetaData, URL
 from sqlalchemy.ext.asyncio import (
     AsyncConnection,
     AsyncEngine,
     create_async_engine,
 )
@@ -19,15 +19,15 @@
     "pk": "pk_%(table_name)s",
 }
 
 
 class Database:
     _engine: AsyncEngine
     _metadata: MetaData
-    _models: Dict[str, Type["Model"]] = {}
+    _models: dict[str, type["Model"]] = {}
     _url: URL
     _connect: Optional[AsyncConnection] = None
     _lock: asyncio.Lock = asyncio.Lock()
     _counter: int = 0
 
     def __init__(self, url: Union[str, URL], **kwargs: Any) -> None:
         if isinstance(url, str):
@@ -58,21 +58,24 @@
         if set_sqlite_pragma and self._url.drivername.startswith("sqlite"):
             self._set_sqlite()
 
         await self.create_all()
 
     def init_all_model(self) -> None:
         for model in self._models.values():
-            model._generate_sqlalchemy_column()
+            model.model_rebuild()
+            model._pre_resolve_relationship_field()
+        for model in self._models.values():
+            model._resolve_sqlalchemy_column()
             model._generate_sqlalchemy_table(self._metadata)
 
     async def dispose(self) -> None:
         await self._engine.dispose()
 
-    def add_model(self, model: Type["Model"]) -> None:
+    def add_model(self, model: type["Model"]) -> None:
         self._models[model.__meta__.tablename] = model
         model.__meta__.database = self
 
     async def __aenter__(self) -> AsyncConnection:
         async with self._lock:
             if self._connect is None:
                 self._connect = self._engine.connect()
```

### Comparing `cherry_orm-0.3.0/cherry/exception.py` & `cherry_orm-1.0.0/cherry/exception.py`

 * *Files identical despite different names*

### Comparing `cherry_orm-0.3.0/cherry/fields/__init__.py` & `cherry_orm-1.0.0/cherry/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `cherry_orm-0.3.0/cherry/fields/annotated.py` & `cherry_orm-1.0.0/cherry/fields/annotated.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import Optional
-from typing_extensions import Annotated
+from typing import Annotated, Optional
 
 from cherry.typing import T
 
 from .fields import Field, Relationship
 
 PrimaryKey = Annotated[T, Field(primary_key=True)]
 """Primary Key Field"""
```

### Comparing `cherry_orm-0.3.0/cherry/fields/proxy.py` & `cherry_orm-1.0.0/cherry/fields/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import abc
+from collections.abc import Iterable, Mapping
 import operator
 from typing import (
     Any,
     Callable,
-    Iterable,
-    List,
-    Mapping,
-    Tuple,
-    Type,
     TYPE_CHECKING,
     Union,
 )
 from typing_extensions import Self
 
 from cherry.exception import FieldTypeError
 from cherry.typing import ModelType
@@ -49,15 +45,15 @@
             return self.binary_expression | other.binary_expression
         return self.binary_expression | other
 
 
 class ModelClause(ModelClauseBase):
     def __init__(
         self,
-        model_cls: Type["Model"],
+        model_cls: type["Model"],
         value: Any,
         field_name: str,
         field: Union[ForeignKeyField, ReverseRelationshipField, ManyToManyField],
         op: OperatorFunc = operator.eq,
     ) -> None:
         if isinstance(field, ForeignKeyField) or (
             isinstance(field, ReverseRelationshipField) and not field.is_list
@@ -140,15 +136,15 @@
 
 
 class JsonFieldClause(ModelClauseBase):
     def __init__(
         self,
         ce: ColumnElement[JSON],
         value: Any,
-        path: List[str],
+        path: list[str],
         op: OperatorFunc = operator.eq,
     ) -> None:
         self.ce = ce
         self.value = value
         self.path = path
         self.op = op
 
@@ -164,15 +160,15 @@
     def __repr__(self) -> str:
         return f"{self.ce} {self.op.__name__} {self.value}"
 
 
 def conversion_type(
     ce: ColumnElement[JSON],
     value: Any,
-) -> Tuple[ColumnElement[JSON], Any]:
+) -> tuple[ColumnElement[JSON], Any]:
     if isinstance(value, str):
         return ce.as_string(), value
     if isinstance(value, int):
         return ce.as_integer(), value
     if isinstance(value, float):
         return ce.as_float(), value
     if isinstance(value, bool):
@@ -184,15 +180,15 @@
     return ce, value
 
 
 class JsonFieldPathProxy:
     def __init__(
         self,
         column: Column,
-        path: List[str],
+        path: list[str],
     ) -> None:
         self.column: Column[JSON] = column
         self.path = path
 
     def __getitem__(self, key: str) -> Self:
         self.path.append(key)
         return self
```

### Comparing `cherry_orm-0.3.0/cherry/fields/types.py` & `cherry_orm-1.0.0/cherry/fields/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import datetime
 from decimal import Decimal
 from enum import Enum
 import ipaddress
 from pathlib import Path
-from typing import Any, cast, Tuple, Type, Union
+from typing import Any, cast, Optional, Union
 from uuid import UUID
 
 from cherry.exception import FieldTypeError
-from cherry.meta import MetaConfig
+from cherry.meta.config import CherryMeta
 
+from annotated_types import MaxLen
 from khemia.typing import (
     all_literal_values,
+    check_isinstance,
     check_issubclass,
     get_args,
-    get_type_from_optional,
+    get_args_without_none,
     is_annotated,
     is_dataclass,
     is_iterable_type,
-    is_json_like_type,
     is_literal_type,
     is_mapping_type,
+    is_none_type,
+    is_sequence_type,
 )
-from pydantic.fields import ModelField
+from pydantic.fields import FieldInfo
 from pydantic.main import BaseModel
 from sqlalchemy import types
 from sqlalchemy.dialects.postgresql import (
     ARRAY as pgARRAY,
     JSONB as pgJSONB,
 )
 from sqlalchemy.engine.interfaces import Dialect
@@ -68,15 +71,15 @@
 
     def load_dialect_impl(self, dialect: Dialect) -> TypeEngine:
         if dialect.name == "postgresql" and self.use_jsonb:
             return dialect.type_descriptor(pgJSONB())
         return dialect.type_descriptor(types.JSON())
 
 
-def sa_to_py_type(type_: Type[Any], config: Type[MetaConfig]):
+def sa_to_py_type(type_: type[Any], config: CherryMeta):
     if issubclass(type_, bool):
         return types.Boolean
     elif issubclass(type_, Enum):
         return types.Enum(type_)
     if issubclass(type_, int):
         return types.Integer
     elif issubclass(type_, float):
@@ -108,30 +111,38 @@
         return types.Numeric(
             precision=getattr(type_, "max_digits", None),
             scale=getattr(type_, "decimal_places", None),
         )
     elif (
         is_dataclass(type_)
         or check_issubclass(type_, BaseModel)
-        or is_json_like_type(type_)
+        or is_mapping_type(type_)
+        or is_sequence_type(type_)
     ):
         return Json(config.use_jsonb_in_postgres)
     else:
         return None
 
 
 def get_sqlalchemy_type_from_field(
-    field: ModelField,
-    config: Type[MetaConfig],
-) -> Tuple[bool, Union[Type[TypeEngine], TypeEngine], bool]:
-    if is_annotated(field.annotation):
-        type_ = get_args(field.annotation)[0]
+    field_info: FieldInfo,
+    config: CherryMeta,
+) -> tuple[bool, Union[type[TypeEngine], TypeEngine], bool]:
+    if not field_info.annotation or is_none_type(field_info.annotation):
+        raise FieldTypeError("field type can not be None")
+    if is_annotated(field_info.annotation):
+        type_ = get_args(field_info.annotation)[0]
     else:
-        type_ = field.annotation
-    is_optional, type_ = get_type_from_optional(type_)
+        type_ = field_info.annotation
+    is_optional, types_ = get_args_without_none(type_)
+    if not types_:
+        raise FieldTypeError(
+            f"{type_} has no matching SQLAlchemy type",
+        )
+    type_ = types_[0]
     if is_literal_type(type_):
         values = all_literal_values(type_)
         if all(issubclass(type(v), type(values[0])) for v in values[1:]):
             if (type_ := sa_to_py_type(type(values[0]), config)) is not None:
                 return is_optional, type_, False
             raise FieldTypeError(
                 f"{type_} has no matching SQLAlchemy type",
@@ -147,23 +158,36 @@
         return is_optional, Json(config.use_jsonb_in_postgres), True
     elif is_iterable_type(type_) and not check_issubclass(type_, str):
         if not config.use_array_in_postgres:
             return is_optional, Json(config.use_jsonb_in_postgres), True
         args = get_args(type_)
         if not args:
             return is_optional, Json(config.use_jsonb_in_postgres), True
-        _, arg_python_type = get_type_from_optional(args[0])
-        if arg_type := sa_to_py_type(arg_python_type, config):
+        _, arg_python_types = get_args_without_none(args[0])
+        if not arg_python_types:
+            return is_optional, Json(config.use_jsonb_in_postgres), True
+        if arg_type := sa_to_py_type(arg_python_types[0], config):
             return is_optional, Array(arg_type), True
         return is_optional, Json(config.use_jsonb_in_postgres), True
     if issubclass(type_, str):
-        if getattr(field.field_info, "long_text", False):
+        if getattr(field_info, "long_text", False):
             return is_optional, types.Text, False
         else:
-            return is_optional, AutoString(length=field.field_info.max_length), False
+            return (
+                is_optional,
+                AutoString(length=get_field_max_length(field_info)),
+                False,
+            )
     if (type_ := sa_to_py_type(type_, config)) is not None:
         return is_optional, type_, False
     if is_dataclass(type_):
         return is_optional, Json(config.use_jsonb_in_postgres), True
     raise FieldTypeError(
         f"{type_} has no matching SQLAlchemy type",
     )
+
+
+def get_field_max_length(field_info: FieldInfo) -> Optional[int]:
+    for metadata in field_info.metadata:
+        if check_isinstance(metadata, MaxLen):
+            return metadata.max_length
+    return None
```

### Comparing `cherry_orm-0.3.0/cherry/fields/utils.py` & `cherry_orm-1.0.0/cherry/fields/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,22 +66,18 @@
     return column_elements
 
 
 def validate_fields(
     model: ModelType,
     input_data: DictStrAny,
 ) -> DictStrAny:
-    if miss := set(input_data) - set(model.__fields__):
+    if miss := set(input_data) - set(model.model_fields):
         raise ValueError(f"{model.__name__} has no fields: {miss}")
 
     fields = {
-        k: (v.outer_type_, v.field_info)
-        for k, v in model.__fields__.items()
-        if k in input_data
+        k: (v.annotation, v) for k, v in model.model_fields.items() if k in input_data
     }
-    new_model = pydantic.create_model(model.__name__, **fields)  # type: ignore
-    values, _, validation_error = pydantic.validate_model(new_model, input_data)
-
-    if validation_error:
-        raise validation_error
-
-    return values
+    new_model: type[pydantic.BaseModel] = pydantic.create_model(
+        model.__name__,
+        **fields,  # type: ignore
+    )
+    return new_model.model_validate(input_data).model_dump()
```

### Comparing `cherry_orm-0.3.0/cherry/meta/meta.py` & `cherry_orm-1.0.0/cherry/meta/meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from typing import (
     Any,
     ClassVar,
-    Dict,
-    List,
     Optional,
-    Tuple,
-    Type,
 )
 
 from cherry.database import Database
 from cherry.fields.fields import (
     ForeignKeyField,
     ManyToManyField,
     ReverseRelationshipField,
@@ -22,45 +18,45 @@
 
 
 class MetaConfig:
     tablename: ClassVar[str]
     database: ClassVar[Database]
     table: ClassVar[Table]
     metadata: ClassVar[MetaData]
-    columns: ClassVar[Dict[str, Column]]
-    constraints: ClassVar[List[ColumnCollectionConstraint]]
-    indexes: ClassVar[List[CompositeIndex]]
+    columns: ClassVar[dict[str, Column]]
+    constraints: ClassVar[list[ColumnCollectionConstraint]]
+    indexes: ClassVar[list[CompositeIndex]]
     abstract: ClassVar[bool]
-    primary_key: ClassVar[Tuple[str, ...]]
-    related_fields: ClassVar[Dict[str, ForeignKeyField]]
-    reverse_related_fields: ClassVar[Dict[str, ReverseRelationshipField]]
-    foreign_keys: ClassVar[Tuple[str, ...]]
-    many_to_many_fields: ClassVar[Dict[str, ManyToManyField]]
-    many_to_many_tables: ClassVar[Dict[str, Table]]
+    primary_key: ClassVar[tuple[str, ...]]
+    related_fields: ClassVar[dict[str, ForeignKeyField]]
+    reverse_related_fields: ClassVar[dict[str, ReverseRelationshipField]]
+    foreign_keys: ClassVar[tuple[str, ...]]
+    many_to_many_fields: ClassVar[dict[str, ManyToManyField]]
+    many_to_many_tables: ClassVar[dict[str, Table]]
     use_jsonb_in_postgres: ClassVar[bool]
     use_array_in_postgres: ClassVar[bool]
 
 
 def mix_meta_config(
-    self_config: Optional[Type[MetaConfig]],
-    parent_config: Type[MetaConfig],
+    self_config: Optional[type[MetaConfig]],
+    parent_config: type[MetaConfig],
     **namespace: Any,
-) -> Type[MetaConfig]:
+) -> type[MetaConfig]:
     if not self_config:
         base_classes = (parent_config,)
     elif self_config == parent_config:
         base_classes = (self_config,)
     else:
         base_classes = self_config, parent_config
 
     return type("Meta", base_classes, namespace)
 
 
 def init_meta_config(
-    meta_config: Type[MetaConfig],
+    meta_config: type[MetaConfig],
 ):
     if not hasattr(meta_config, "abstract"):
         meta_config.abstract = False
     meta_config.columns = {}
     meta_config.constraints = []
     meta_config.related_fields = {}
     meta_config.reverse_related_fields = {}
```

### Comparing `cherry_orm-0.3.0/cherry/models/models.py` & `cherry_orm-1.0.0/cherry/models/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import asyncio
 from functools import reduce
 from typing import (
     Any,
     cast,
     ClassVar,
-    ForwardRef,
-    List,
     Optional,
-    Tuple,
-    Type,
     TYPE_CHECKING,
     Union,
 )
 from typing_extensions import dataclass_transform, Self
 
 from cherry.database import Database
 from cherry.exception import *
@@ -23,109 +19,121 @@
     ManyToManyField,
     Relationship,
     RelationshipField,
     ReverseRelationshipField,
 )
 from cherry.fields.proxy import JsonFieldProxy, RelatedModelProxy
 from cherry.fields.types import get_sqlalchemy_type_from_field
-from cherry.meta.meta import init_meta_config, MetaConfig, mix_meta_config
-from cherry.meta.pydantic_config import generate_pydantic_config
+from cherry.meta.config import (
+    CherryConfig,
+    CherryMeta,
+    default_pydantic_config,
+    generate_cherry_config,
+)
 from cherry.queryset.queryset import QuerySet
 from cherry.typing import AnyMapping, DictStrAny
 
+from khemia.typing import (
+    check_issubclass,
+    get_args,
+    get_args_without_none,
+    is_sequence_type,
+)
 from khemia.utils import classproperty
 from pydantic import PrivateAttr
-from pydantic.fields import FieldInfo
-from pydantic.main import BaseModel, ModelMetaclass
+from pydantic._internal._generics import PydanticGenericMetadata
+from pydantic._internal._model_construction import ModelMetaclass
+from pydantic.fields import _Unset, FieldInfo
+from pydantic.main import BaseModel
 from sqlalchemy import Column, ForeignKey, Index, MetaData, Table
 from sqlalchemy.sql.elements import ColumnElement
 from sqlalchemy.sql.operators import and_
 
 
 @dataclass_transform(kw_only_default=True, field_specifiers=(Field, Relationship))
 class ModelMeta(ModelMetaclass):
     def __new__(
-        cls,
-        name: str,
-        bases: Tuple[Type[Any], ...],
-        attrs: DictStrAny,
+        mcs,
+        cls_name: str,
+        bases: tuple[type[Any], ...],
+        namespace: DictStrAny,
+        __pydantic_generic_metadata__: Union[PydanticGenericMetadata, None] = None,
+        __pydantic_reset_parent_namespace__: bool = True,
+        _create_model_module: Union[str, None] = None,
         **kwargs: Any,
     ) -> "ModelMeta":
-        generate_pydantic_config(attrs)
+        generate_cherry_config(bases, namespace, kwargs)
+        cherry_config: CherryConfig = namespace["cherry_config"]
+        if cherry_config.get("abstract"):
+            cherry_config["abstract"] = False
+
+        cls = cast(
+            type["Model"],
+            super().__new__(
+                mcs,
+                cls_name,
+                bases,
+                namespace,
+                __pydantic_generic_metadata__,
+                __pydantic_reset_parent_namespace__,
+                _create_model_module,
+                **kwargs,
+            ),
+        )
 
-        meta = type("Meta", (MetaConfig,), {})
-        for base in reversed(bases):
-            if base != BaseModel and issubclass(base, Model):
-                meta = mix_meta_config(base.__meta__, MetaConfig)
-        init_meta_config(meta)
-        meta.tablename = name
-        if meta.abstract:
-            meta.abstract = False
-
-        allowed_meta_kwargs = {
-            key
-            for key in dir(meta)
-            if not (key.startswith("__") and key.endswith("__"))
-        }
-        meta_kwargs = {
-            key: kwargs.pop(key) for key in kwargs.keys() & allowed_meta_kwargs
-        }
-        attrs["__meta__"] = mix_meta_config(attrs.get("Meta"), meta, **meta_kwargs)
-
-        new_cls = cast(Type["Model"], super().__new__(cls, name, bases, attrs))
-
-        meta_config = new_cls.__meta__
-
-        for model_field in new_cls.__fields__.values():
-            if model_field.field_info.__class__ is FieldInfo:
-                model_field.field_info = BaseField.from_base_field_info(
-                    model_field.field_info,
-                )
-            field_info = model_field.field_info
-            if isinstance(field_info, BaseField):
-                pass
-            elif isinstance(
-                field_info,
-                RelationshipField,
-            ):
-                if field_info.nullable is None:
-                    field_info.nullable = model_field.allow_none
-                field_info.related_model = model_field.type_  # type: ignore
-            else:
-                raise FieldTypeError(
-                    (
-                        'Field type must be "cherry.Field", got unexpected type: '
-                        f" {field_info.__class__}"
-                    ),
+        for field_name, field_info in cls.model_fields.items():
+            if field_info.__class__ is FieldInfo:
+                cls.model_fields[field_name] = BaseField.from_pydantic_field_info(
+                    field_info,
                 )
 
-        if not meta_config.abstract and hasattr(meta_config, "database"):
-            meta_config.database.add_model(new_cls)
-            meta_config.primary_key = tuple(
-                field.name
-                for field in new_cls.__fields__.values()
-                if isinstance(field.field_info, BaseField)
-                and field.field_info.primary_key
-            )
-            if len(meta_config.primary_key) == 0:
-                raise PrimaryKeyMissingError(
-                    f"Model {new_cls} must have at least one primary key",
+        cls.__meta__ = CherryMeta(
+            tablename=cls.cherry_config.get("tablename") or cls_name,
+        )
+        if (abstract := cls.cherry_config.get("abstract")) is not None:
+            cls.__meta__.abstract = abstract
+        if (database := cls.cherry_config.get("database")) is not None:
+            cls.__meta__.database = database
+            if not abstract:
+                database.add_model(cls)
+                cls.__meta__.primary_key = tuple(
+                    field_name
+                    for field_name, field in cls.model_fields.items()
+                    if isinstance(field, BaseField) and field.primary_key
                 )
 
-        return new_cls
+                if len(cls.__meta__.primary_key) == 0:
+                    raise PrimaryKeyMissingError(
+                        f"Model {cls} must have at least one primary key",
+                    )
+
+        return cls
 
 
 class Model(BaseModel, metaclass=ModelMeta):
+    model_config = default_pydantic_config.copy()
+    cherry_config: ClassVar[CherryConfig]
+    __meta__: ClassVar[CherryMeta]
     if TYPE_CHECKING:
-        __meta__: ClassVar[Type[MetaConfig]]
+        model_fields: ClassVar[
+            dict[
+                str,
+                Union[
+                    BaseField,
+                    ForeignKeyField,
+                    ReverseRelationshipField,
+                    ManyToManyField,
+                ],
+            ]
+        ]
 
     if TYPE_CHECKING:
-        __cherry_foreign_key_values__: DictStrAny = Field(init=False)
+        _cherry_foreign_key_values_: DictStrAny = Field(init=False)
     else:
-        __cherry_foreign_key_values__: DictStrAny = PrivateAttr(default_factory=dict)
+        _cherry_foreign_key_values_: DictStrAny = PrivateAttr(default_factory=dict)
 
     @classproperty
     def tablename(cls) -> str:
         """models's tablename in database"""
         return cls.__meta__.tablename
 
     @classproperty
@@ -157,19 +165,18 @@
                 ),
             )
             if result.inserted_primary_key:
                 self.update_from_dict(result.inserted_primary_key._asdict())
             if not exclude_related:
                 for name, rfield in self.__meta__.reverse_related_fields.items():
                     if related_values := getattr(self, name, None):
-                        related_values = cast(List[Model], related_values)
                         await asyncio.gather(
                             *[
                                 value.update(**{rfield.related_field_name: self})
-                                for value in related_values
+                                for value in cast(list[Model], related_values)
                             ],
                         )
         return self
 
     async def insert_with_related(self, *args: Any) -> Self:
         await self.insert(exclude_related=True)
         table_names = self._get_related_tables(*args)
@@ -303,28 +310,25 @@
             table_names = self._get_related_tables(*args)
             for name, rfield in self.__meta__.related_fields.items():
                 if (
                     table_names is not None
                     and rfield.related_model.tablename not in table_names
                 ):
                     continue
-                if (
-                    rfield.foreign_key_self_name
-                    not in self.__cherry_foreign_key_values__
-                ):
+                if rfield.foreign_key_self_name not in self._cherry_foreign_key_values_:
                     raise RelatedFieldMissingError(
                         (
                             "Can not fetch related model if not been inserted into or"
                             " fetched from database"
                         ),
                     )
                 related_data = await conn.execute(
                     rfield.related_model.table.select().where(
                         getattr(rfield.related_model, rfield.foreign_key)
-                        == self.__cherry_foreign_key_values__[
+                        == self._cherry_foreign_key_values_[
                             rfield.foreign_key_self_name
                         ],
                     ),
                 )
                 if related_one := related_data.fetchone():
                     setattr(
                         self,
@@ -485,15 +489,15 @@
     @classmethod
     async def delete_many(cls, *models: Self) -> int:
         """delete many models from database"""
         if models:
             async with cls.database as conn:
                 result = await conn.execute(
                     cls.table.delete(),
-                    [model.dict(by_alias=True) for model in models],
+                    [model.model_dump(by_alias=True) for model in models],
                 )
                 return result.rowcount
         raise ModelMissingError("You must give at least one model to delete")
 
     @classmethod
     def select(cls) -> QuerySet[Self]:
         """query without any filter condition"""
@@ -506,25 +510,25 @@
 
     @classmethod
     def select_related(cls, *args: Any) -> QuerySet[Self]:
         """select and select related model at the same time"""
         return QuerySet(cls).prefetch_related(*args)
 
     @classmethod
-    async def paginate(cls, page: int, page_size: int) -> List[Self]:
+    async def paginate(cls, page: int, page_size: int) -> list[Self]:
         """select with pagination"""
         return await QuerySet(cls).paginate(page, page_size)
 
     @classmethod
     async def first(cls) -> Optional[Self]:
         """select first model"""
         return await QuerySet(cls).first()
 
     @classmethod
-    async def all(cls) -> List[Self]:
+    async def all(cls) -> list[Self]:
         """select all models"""
         return await QuerySet(cls).all()
 
     @classmethod
     async def random_one(cls) -> Optional[Self]:
         """select one model randomly"""
         return await QuerySet(cls).random_one()
@@ -543,17 +547,17 @@
             return None
 
     @classmethod
     async def get_or_create(
         cls,
         *args: Any,
         defaults: Optional[DictStrAny] = None,
-        fetch_related: Union[bool, Tuple[Any, ...]] = False,
+        fetch_related: Union[bool, tuple[Any, ...]] = False,
         **kwargs: Any,
-    ) -> Tuple[Self, bool]:
+    ) -> tuple[Self, bool]:
         """select one model with filter condition, if not exist, create one"""
         queryset = cls.filter(*args, **kwargs)
         if fetch_related is True or isinstance(fetch_related, tuple):
             queryset = queryset.prefetch_related(
                 () if fetch_related is True else fetch_related,
             )
         try:
@@ -569,17 +573,17 @@
             return await cls(**create_values).insert(), False
 
     @classmethod
     async def update_or_create(
         cls,
         *args: Any,
         defaults: Optional[DictStrAny] = None,
-        fetch_related: Union[bool, Tuple[Any, ...]] = False,
+        fetch_related: Union[bool, tuple[Any, ...]] = False,
         **kwargs: Any,
-    ) -> Tuple[Self, bool]:
+    ) -> tuple[Self, bool]:
         """update one model with filter condition,
         if not exist, create one with filter and defaults values"""
         queryset = cls.filter(*args, **kwargs)
         if fetch_related is True or isinstance(fetch_related, tuple):
             queryset = queryset.prefetch_related(
                 () if fetch_related is True else fetch_related,
             )
@@ -667,71 +671,74 @@
             (
                 getattr(self.__class__, pk) == getattr(self, pk)
                 for pk in self.__meta__.primary_key
             ),
         )
 
     @classmethod
-    def get_pk_columns(cls) -> Tuple[Column, ...]:
+    def get_pk_columns(cls) -> tuple[Column, ...]:
         """get primary key columns"""
         return tuple(getattr(cls, pk) for pk in cls.__meta__.primary_key)
 
     @classmethod
     def parse_from_db_dict(cls, data: DictStrAny) -> Self:
         """parse model from database result dict"""
-        model = cls.parse_obj(data)
+        model = cls.model_validate(data)
         for foreign_key in cls.__meta__.foreign_keys:
-            model.__cherry_foreign_key_values__[foreign_key] = data.pop(
+            model._cherry_foreign_key_values_[foreign_key] = data.pop(
                 foreign_key,
                 None,
             )
         return model
 
     def update_from_dict(self, update_data: AnyMapping):
         """update model from dict"""
         for k, v in update_data.items():
-            if k in self.__fields__:
+            if k in self.model_fields:
                 setattr(self, k, v)
             elif k in self.__meta__.foreign_keys:
-                self.__cherry_foreign_key_values__[k] = v
+                self._cherry_foreign_key_values_[k] = v
 
     def update_from_kwargs(self, **kwargs: Any):
         """update model from kwargs"""
         for k, v in kwargs.items():
-            setattr(self, k, v)
+            if k in self.model_fields:
+                setattr(self, k, v)
+            elif k in self.__meta__.foreign_keys:
+                self._cherry_foreign_key_values_[k] = v
 
     def _extract_db_fields(
         self,
         exclude_pk: bool = False,
         exclude_related: bool = False,
     ) -> DictStrAny:
         """extract database fields from model"""
         exclude = (
             self.__meta__.related_fields.keys()
             | self.__meta__.reverse_related_fields.keys()
             | self.__meta__.many_to_many_fields.keys()
         )
         if exclude_pk:
             exclude |= set(self.__meta__.primary_key)
-        data = self.dict(by_alias=True, exclude=exclude)
+        data = self.model_dump(by_alias=True, exclude=exclude)
         data = {k: list(v) if isinstance(v, set) else v for k, v in data.items()}
         if exclude_related:
             return data
         for field_name, field in self.__meta__.related_fields.items():
             self_value = getattr(self, field_name)
             if self_value is None:
                 data[field.foreign_key_self_name] = None
-                self.__cherry_foreign_key_values__[field.foreign_key_self_name] = None
+                self._cherry_foreign_key_values_[field.foreign_key_self_name] = None
                 continue
             value = getattr(
                 self_value,
                 field.foreign_key,
             )
             data[field.foreign_key_self_name] = value
-            self.__cherry_foreign_key_values__[field.foreign_key_self_name] = value
+            self._cherry_foreign_key_values_[field.foreign_key_self_name] = value
             if not field.nullable and not data[field.foreign_key_self_name]:
                 raise ForeignKeyMissingError(
                     (
                         "Foreign key field"
                         f' "{self.__class__}.{field.foreign_key_self_name}" cannot be'
                         " None when insert or update"
                     ),
@@ -739,44 +746,15 @@
         return data
 
     def _check_pk_null(self) -> bool:
         """check if primary key is null"""
         return all(getattr(self, pk) is None for pk in self.__meta__.primary_key)
 
     @classmethod
-    def update_forward_refs(cls, **localns: Any):
-        """update forward refs and check model type"""
-        super().update_forward_refs(**localns)
-        model_type = []
-        for _, field in cls.__fields__.items():
-            field_info = field.field_info
-            if isinstance(
-                field_info,
-                RelationshipField,
-            ):
-                if isinstance(field_info.related_model, ForwardRef):
-                    field_info.related_model = field.type_
-                if not issubclass(field_info.related_model, Model):
-                    raise RelationSolveError(
-                        (
-                            'Related model must be a "cherry.Model", but got unexpected'
-                            f" type {field_info.related_model}"
-                        ),
-                    )
-                if field_info.related_model in model_type:
-                    raise RelationSolveError(
-                        (
-                            f"Related model {field_info.related_model} can appear only"
-                            f" once in {cls}"
-                        ),
-                    )
-                model_type.append(field_info.related_model)
-
-    @classmethod
-    def _get_related_tables(cls, *args: Any) -> Optional[List[str]]:
+    def _get_related_tables(cls, *args: Any) -> Optional[list[str]]:
         if args:
             table_names = []
             for arg in args:
                 if isinstance(arg, Table):
                     table_names.append(arg.name)
                 elif isinstance(arg, str):
                     table_names.append(arg)
@@ -794,91 +772,136 @@
                         ),
                     )
         else:
             table_names = None
         return table_names
 
     @classmethod
-    def _get_field_type_by_model(cls, model: "Model") -> Tuple[str, RelationshipField]:
-        for field_name, field in cls.__fields__.items():
+    def _get_field_type_by_model(cls, model: "Model") -> tuple[str, RelationshipField]:
+        for field_name, field_info in cls.model_fields.items():
             if isinstance(
-                field.field_info,
+                field_info,
                 RelationshipField,
-            ) and isinstance(model, field.field_info.related_model):
-                return field_name, field.field_info
+            ) and isinstance(model, field_info.related_model):
+                return field_name, field_info
         raise FieldTypeError(
             f"There are no related fields associated with {cls}.{model}",
         )
 
     @classmethod
-    def _generate_sqlalchemy_column(cls):
-        if any(f for f in cls.__fields__.values() if isinstance(f.type_, ForwardRef)):
-            cls.update_forward_refs()
-        for model_field in cls.__fields__.values():
-            field_info = model_field.field_info
+    def _pre_resolve_relationship_field(cls):
+        for field_name, field_info in cls.model_fields.items():
+            if not isinstance(field_info, RelationshipField):
+                continue
+            is_nullable, type_ = get_args_without_none(field_info.annotation)  # type: ignore
+            if len(type_) != 1:
+                raise FieldTypeError(
+                    f"wrong type for model {cls}'s field {field_name}",
+                )
+            type_ = type_[0]
+            if is_sequence_type(type_):
+                type_ = get_args(type_)
+                if len(type_) != 1:
+                    raise FieldTypeError(
+                        f"wrong type for Model {cls}'s field {field_name}",
+                    )
+                type_ = type_[0]
+                if isinstance(field_info, ReverseRelationshipField):
+                    field_info.is_list = True
+                elif isinstance(field_info, ForeignKeyField):
+                    raise FieldTypeError(
+                        f"Model {cls}'s ForeignKeyField {field_name} "
+                        f"types must be a subclass of Cherry.Model, not {type_}",
+                    )
+            elif isinstance(field_info, ManyToManyField):
+                raise FieldTypeError(
+                    f"Model {cls}'s ManyToManyField {field_name} types"
+                    f" must be a sequence type of Cherry.Model, not {type_}",
+                )
+            if not check_issubclass(type_, Model):
+                raise FieldTypeError(
+                    f"Model {cls}'s RelationshipField {field_name} types"
+                    f" must be a subclass of Cherry.Model, not {type_}",
+                )
+            field_info.nullable = is_nullable
+            field_info.related_model = type_
+
+    @classmethod
+    def _resolve_sqlalchemy_column(cls):
+        for field_name, field_info in cls.model_fields.items():
             if isinstance(field_info, BaseField):
                 nullable, type_, is_json = get_sqlalchemy_type_from_field(
-                    model_field,
+                    field_info,
                     cls.__meta__,
                 )
                 if field_info.nullable is None:
                     field_info.nullable = nullable
-                cls.__meta__.columns[model_field.name] = Column(
-                    model_field.name,
+                default = (
+                    field_info.default
+                    if field_info.default is not _Unset
+                    else field_info.default_factory
+                    if field_info.default_factory is not _Unset
+                    else None
+                )
+                cls.__meta__.columns[field_name] = Column(
+                    field_name,
                     type_=type_,
                     primary_key=field_info.primary_key,
                     nullable=field_info.nullable,
                     index=field_info.index,
                     unique=field_info.unique,
                     autoincrement=field_info.autoincrement,
-                    default=field_info.default or field_info.default_factory or None,
+                    default=default,
                     **field_info.sa_column_extra,
                 )
                 if is_json:
                     setattr(
                         cls,
-                        model_field.name,
-                        JsonFieldProxy(cls.__meta__.columns[model_field.name]),
+                        field_name,
+                        JsonFieldProxy(cls.__meta__.columns[field_name]),
                     )
                 else:
                     setattr(
                         cls,
-                        model_field.name,
-                        cls.__meta__.columns[model_field.name],
+                        field_name,
+                        cls.__meta__.columns[field_name],
                     )
             elif isinstance(field_info, ForeignKeyField):
                 if not hasattr(field_info, "related_field_name"):
-                    for rname, rfield in field_info.related_model.__fields__.items():
+                    for (
+                        rname,
+                        rfield_info,
+                    ) in field_info.related_model.model_fields.items():  # noqa: E501
                         has_flag = False
                         if (
-                            isinstance(rfield.field_info, ReverseRelationshipField)
-                            and rfield.field_info.related_model is cls
+                            isinstance(rfield_info, ReverseRelationshipField)
+                            and rfield_info.related_model is cls
                             and (
-                                rfield.field_info.related_field_name == model_field.name
-                                or rfield.field_info.related_field_name is None
+                                rfield_info.related_field_name == field_name
+                                or rfield_info.related_field_name is None
                             )
                         ):
                             has_flag = True
                             field_info.related_field_name = rname
-                            field_info.related_field = rfield.field_info
-                            rfield.field_info.related_field_name = model_field.name
-                            rfield.field_info.related_field = field_info
+                            field_info.related_field = rfield_info
+                            rfield_info.related_field_name = field_name
+                            rfield_info.related_field = field_info
                             break
                         if not has_flag:
                             field_info.related_field_name = None
                             field_info.related_field = None
                 if (
                     not hasattr(field_info, "related_field")
                     and field_info.related_field_name is not None
                 ):
                     field_info.related_field = cast(
                         ReverseRelationshipField,
-                        field_info.related_model.__fields__[
+                        field_info.related_model.model_fields[
                             field_info.related_field_name
-                        ].field_info,
+                        ],
                     )
                 if not hasattr(field_info, "foreign_key"):
                     if len(field_info.related_model.__meta__.primary_key) != 1:
                         raise PrimaryKeyMultipleError(
                             (
                                 f"{cls} has multiple primary keys, you must"
                                 " explicitly give out foreign key through"
@@ -887,15 +910,15 @@
                         )
                     field_info.foreign_key = (
                         field_info.related_model.__meta__.primary_key[0]
                     )
                 field_info.foreign_key_self_name = (
                     f"{field_info.related_model.tablename}_{field_info.foreign_key}"  # noqa: E501
                 )
-                cls.__meta__.columns[model_field.name] = Column(
+                cls.__meta__.columns[field_name] = Column(
                     f"{field_info.related_model.tablename}_{field_info.foreign_key}",
                     ForeignKey(
                         f"{field_info.related_model.tablename}.{field_info.foreign_key}",
                         onupdate=field_info.on_update
                         or (
                             field_info.related_field
                             and field_info.related_field.on_update
@@ -908,141 +931,133 @@
                         )
                         or "NO ACTION",
                         **field_info.foreign_key_extra,
                     ),
                     nullable=field_info.nullable,
                     **field_info.sa_column_extra,
                 )
-                cls.__meta__.related_fields[model_field.name] = field_info
+                cls.__meta__.related_fields[field_name] = field_info
                 setattr(
                     cls,
-                    model_field.name,
+                    field_name,
                     RelatedModelProxy(
                         cls,
                         field_info.related_model,
-                        model_field.name,
+                        field_name,
                         field_info,
                     ),
                 )
                 setattr(
                     cls,
                     field_info.foreign_key_self_name,
-                    cls.__meta__.columns[model_field.name],
+                    cls.__meta__.columns[field_name],
                 )
             elif isinstance(field_info, ReverseRelationshipField):
-                # from pydantic.fields.py, 2 is list
-                if model_field.shape == 2:
-                    field_info.is_list = True
-                elif model_field.shape != 1:
-                    raise FieldTypeError(
-                        (
-                            'ReverseRelationshipField must be a "cherry.Model" type or'
-                            " alist of it"
-                        ),
-                    )
                 if not hasattr(field_info, "related_field_name"):
-                    for rname, rfield in field_info.related_model.__fields__.items():
+                    for (
+                        rname,
+                        rfield_info,
+                    ) in field_info.related_model.model_fields.items():  # noqa: E501
                         if (
-                            isinstance(rfield.field_info, ForeignKeyField)
-                            and rfield.field_info.related_model is cls
+                            isinstance(rfield_info, ForeignKeyField)
+                            and rfield_info.related_model is cls
                             and (
-                                rfield.field_info.related_field_name == model_field.name
-                                or rfield.field_info.related_field_name is None
+                                rfield_info.related_field_name == field_name
+                                or rfield_info.related_field_name is None
                             )
                         ):
                             field_info.related_field_name = rname
-                            field_info.related_field = rfield.field_info
-                            rfield.field_info.related_field_name = model_field.name
-                            rfield.field_info.related_field = field_info
+                            field_info.related_field = rfield_info
+                            rfield_info.related_field_name = field_name
+                            rfield_info.related_field = field_info
                             break
                 if hasattr(field_info, "related_field_name"):
-                    cls.__meta__.reverse_related_fields[model_field.name] = field_info
+                    cls.__meta__.reverse_related_fields[field_name] = field_info
                     setattr(
                         cls,
-                        model_field.name,
+                        field_name,
                         RelatedModelProxy(
                             cls,
                             field_info.related_model,
-                            model_field.name,
+                            field_name,
                             field_info,
                         ),
                     )
                     if not hasattr(field_info, "related_field"):
                         field_info.related_field = cast(
                             ForeignKeyField,
-                            field_info.related_model.__fields__[
+                            field_info.related_model.model_fields[
                                 field_info.related_field_name
-                            ].field_info,
+                            ],
                         )
                 else:
                     raise RelationSolveError(
                         (
                             "There are no related fields associated with"
-                            f" {cls}.{model_field.name}"
+                            f" {cls}.{field_name}"
                         ),
                     )
             elif isinstance(field_info, ManyToManyField):
-                if model_field.shape != 2:
-                    raise FieldTypeError(
-                        'ManyToManyField must be a list of "cherry.Model" type',
-                    )
                 if not hasattr(field_info, "m2m_field_name"):
                     if len(cls.__meta__.primary_key) != 1:
                         raise PrimaryKeyMultipleError(
                             (
                                 f"{cls} has multiple primary keys, you must"
                                 " explicitly give out foreign key through"
                                 ' Relationship(many_to_many="some field")'
                             ),
                         )
                     field_info.m2m_field_name = cls.__meta__.primary_key[0]
                 if not hasattr(field_info, "related_field_name"):
-                    for rname, rfield in field_info.related_model.__fields__.items():
+                    for (
+                        rname,
+                        rfield_info,
+                    ) in field_info.related_model.model_fields.items():  # noqa: E501
                         if (
-                            isinstance(rfield.field_info, ManyToManyField)
-                            and rfield.field_info.related_model is cls
+                            isinstance(rfield_info, ManyToManyField)
+                            and rfield_info.related_model is cls
                             and (
                                 (
                                     rfn := getattr(
-                                        rfield.field_info,
+                                        rfield_info,
                                         "related_field_name",
                                         None,
                                     )
                                 )
                                 is None
-                                or rfn == model_field.name
+                                or rfn == field_name
                             )
                         ):
                             field_info.related_field_name = rname
-                            field_info.related_field = rfield.field_info
-                            rfield.field_info.related_field_name = model_field.name
-                            rfield.field_info.related_field = field_info
+                            field_info.related_field = rfield_info
+                            rfield_info.related_field_name = field_name
+                            rfield_info.related_field = field_info
                             break
                 if not hasattr(field_info, "related_field_name"):
                     raise RelationSolveError(
                         (
                             "There are no related fields associated with"
-                            f" {cls}.{model_field.name}"
+                            f" {cls}.{field_name}"
                         ),
                     )
                 if not hasattr(field_info, "related_field"):
                     field_info.related_field = cast(
                         ManyToManyField,
-                        field_info.related_model.__fields__[
+                        field_info.related_model.model_fields[
                             field_info.related_field_name
-                        ].field_info,
+                        ],
                     )
-                cls.__meta__.many_to_many_fields[model_field.name] = field_info
+                cls.__meta__.many_to_many_fields[field_name] = field_info
                 setattr(
                     cls,
-                    model_field.name,
+                    field_name,
                     RelatedModelProxy(
                         cls,
                         field_info.related_model,
-                        model_field.name,
+                        field_name,
                         field_info,
                     ),
                 )
         cls.__meta__.foreign_keys = tuple(
             f.foreign_key_self_name for f in cls.__meta__.related_fields.values()
         )
         return cls.__meta__.columns
@@ -1110,15 +1125,15 @@
                 field.related_field.table = table
                 cls.__meta__.many_to_many_tables[field_name] = table
                 field.related_model.__meta__.many_to_many_tables[
                     field.related_field_name
                 ] = table
 
         for index in cls.__meta__.indexes:
-            columns: List[Column] = [
+            columns: list[Column] = [
                 (
                     f.get_column()
                     if isinstance((f := getattr(cls, column_name)), RelatedModelProxy)
                     else f
                 )
                 for column_name in index.columns
             ]
```

### Comparing `cherry_orm-0.3.0/cherry/queryset/queryset.py` & `cherry_orm-1.0.0/cherry/queryset/queryset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from dataclasses import dataclass, field
 from functools import reduce
 from typing import (
     Any,
     cast,
-    Dict,
     Generic,
-    List,
     Literal,
     Optional,
     overload,
-    Tuple,
-    Type,
     Union,
 )
 from typing_extensions import Self, Unpack
 
 from cherry.exception import MultipleDataError, NoMatchDataError, PaginateArgError
 from cherry.fields.fields import (
     ForeignKeyField,
@@ -39,25 +35,30 @@
 from sqlalchemy.ext.asyncio import AsyncConnection
 from sqlalchemy.sql.operators import and_
 
 
 @dataclass
 class QueryOptions:
     clause: OptionalClause = None
-    order_by: List[Any] = field(default_factory=list)
-    limit: Optional[int] = None
-    offset: Optional[int] = None
-    related: List[Any] = field(default_factory=list)
-    related_fields: Dict[str, ForeignKeyField] = field(default_factory=dict)
-    reverse_related_fields: Dict[str, ReverseRelationshipField] = field(
+    funcs: list[
+        tuple[Literal["order_by", "group_by", "limit", "offset", "distinct"], bool, Any]
+    ] = field(default_factory=list)
+    # order_by: list[Any] = field(default_factory=list)
+    # group_by: list[Any] = field(default_factory=list)
+    # limit: Optional[int] = None
+    # offset: Optional[int] = None
+    # distinct: Optional[int] = None
+    related: list[Any] = field(default_factory=list)
+    related_fields: dict[str, ForeignKeyField] = field(default_factory=dict)
+    reverse_related_fields: dict[str, ReverseRelationshipField] = field(
         default_factory=dict,
     )
-    many_to_many_fields: Dict[str, ManyToManyField] = field(default_factory=dict)
+    many_to_many_fields: dict[str, ManyToManyField] = field(default_factory=dict)
 
-    def get_join(self, select_stat: Select) -> List[Any]:
+    def get_join(self, select_stat: Select) -> list[Any]:
         tables = select_stat.columns_clause_froms
         join_ = []
         if isinstance(self.clause, BooleanClauseList):
             for f in self.clause:
                 if isinstance(f.left, Column) and f.left.table not in tables:
                     join_.append(f.left.table)
                 if isinstance(f.right, Column) and f.right.table not in tables:
@@ -74,29 +75,40 @@
             ):
                 join_.append(self.clause.right.table)
         return [j for j in join_ if j is not None]
 
     def as_select_option(self, select_stat: Select):
         if self.clause is not None:
             select_stat = select_stat.where(self.clause)
-        if self.order_by:
-            select_stat = select_stat.order_by(*self.order_by)
-        if self.limit:
-            select_stat = select_stat.limit(self.limit)
-        if self.offset:
-            select_stat = select_stat.offset(self.offset)
+        for func_ in self.funcs:
+            if func_[0] == "distinct":
+                select_stat = select_stat.distinct()
+            elif func_[1]:
+                select_stat = getattr(select_stat, func_[0])(*func_[2])
+            else:
+                select_stat = getattr(select_stat, func_[0])(func_[2])
+        # if self.group_by:
+        #     select_stat = select_stat.group_by(*self.group_by)
+        # if self.order_by:
+        #     select_stat = select_stat.order_by(*self.order_by)
+        # if self.limit:
+        #     select_stat = select_stat.limit(self.limit)
+        # if self.offset:
+        #     select_stat = select_stat.offset(self.offset)
+        # if self.distinct:
+        #     select_stat = select_stat.distinct()
         if join_ := self.get_join(select_stat):
             select_stat = select_stat.join(*join_)
         return select_stat
 
 
 class QuerySet(QuerySetProtocol, Generic[T_MODEL]):
     def __init__(
         self,
-        model_cls: Type[T_MODEL],
+        model_cls: type[T_MODEL],
         *args: Any,
         **kwargs: Any,
     ) -> None:
         self.model_cls = model_cls
         self.raw_claust_list: ClauseListType = []
         final_clause = self._parse_clause(*args, **kwargs)
         self.options = QueryOptions(
@@ -107,24 +119,37 @@
         clause = self._parse_clause(*args, **kwargs)
         if self.options.clause is None:
             self.options.clause = clause
         elif clause is not None:
             self.options.clause &= clause
         return self
 
+    def group_by(self, *args: Any) -> Self:
+        # self.options.group_by.extend(args)
+        self.options.funcs.append(("group_by", True, args))
+        return self
+
     def order_by(self, *args: Any) -> Self:
-        self.options.order_by.extend(args)
+        # self.options.order_by.extend(args)
+        self.options.funcs.append(("order_by", True, args))
         return self
 
     def limit(self, num: int) -> Self:
-        self.options.limit = num
+        # self.options.limit = num
+        self.options.funcs.append(("limit", False, num))
+        return self
+
+    def distinct(self, is_: bool = True) -> Self:
+        # self.options.distinct = is_
+        self.options.funcs.append(("distinct", False, is_))
         return self
 
     def offset(self, num: int) -> Self:
-        self.options.offset = num
+        # self.options.offset = num
+        self.options.funcs.append(("offset", False, num))
         return self
 
     def prefetch_related(self, *args: Any) -> Self:
         table_names = self.model_cls._get_related_tables(*args)
 
         self.options.related_fields = (
             self.model_cls.__meta__.related_fields
@@ -155,30 +180,30 @@
             }
         )
         return self
 
     @overload
     def values(
         self,
-        *args: Unpack[Tuple[T, ...]],
+        *args: Unpack[tuple[T, ...]],
         flatten: Literal[True],
     ) -> "ValueQuerySet[T]":
         ...
 
     @overload
     def values(
         self,
-        *args: Unpack[Tuple[T, Unpack[Ts]]],
+        *args: Unpack[tuple[T, Unpack[Ts]]],
         flatten: Literal[False] = False,
     ) -> "ValuesQuerySet[T, Unpack[Ts]]":
         ...
 
     def values(
         self,
-        *args: Unpack[Tuple[T, Unpack[Ts]]],
+        *args: Unpack[tuple[T, Unpack[Ts]]],
         flatten: bool = False,
     ) -> Union["ValuesQuerySet[T, Unpack[Ts]]", "ValueQuerySet[T]"]:
         if flatten:
             if len(args) > 1:
                 raise ValueError("Only one argument is allowed")
             return ValueQuerySet(
                 args[0],
@@ -225,15 +250,15 @@
                 )
             if len(results) == 1:
                 data = results[0]._asdict()
                 await self._fetch_one_related(conn, data)
                 return self.model_cls.parse_from_db_dict(data)
             raise NoMatchDataError(f"No match data for {self.model_cls}")
 
-    async def all(self) -> List[T_MODEL]:
+    async def all(self) -> list[T_MODEL]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
                 self.options.as_select_option(self.model_cls.table.select()),
             )
             data = [data._asdict() for data in result.fetchall()]
             await self._fetch_many_related(conn, data)
 
@@ -241,26 +266,28 @@
 
     async def random_one(self) -> Optional[T_MODEL]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
                 self.options.as_select_option(
                     self.model_cls.table.select().order_by(func.random()),
                 ),
-            )
+            )  # type: ignore
             if result_one := result.fetchone():
                 data = result_one._asdict()
                 await self._fetch_one_related(conn, data)
                 return self.model_cls.parse_from_db_dict(data)
             return None
 
-    async def paginate(self, page: int, page_size: int) -> List[T_MODEL]:
+    async def paginate(self, page: int, page_size: int) -> list[T_MODEL]:
         if page < 1 or page_size < 1:
             raise PaginateArgError("page and page_size must be positive")
-        self.options.limit = page_size
-        self.options.offset = (page - 1) * page_size
+        # self.options.limit = page_size
+        self.options.funcs.append(("limit", False, page_size))
+        # self.options.offset = (page - 1) * page_size
+        self.options.funcs.append(("offset", False, (page - 1) * page_size))
         return await self.all()
 
     async def delete(self) -> int:
         async with self.model_cls.database as conn:
             stat = self.model_cls.table.delete()
             if self.options.clause is not None:
                 stat = stat.where(self.options.clause)
@@ -325,15 +352,15 @@
             result = await conn.execute(
                 self.options.as_select_option(
                     select(func.sum(column)).select_from(self.model_cls.table),
                 ),
             )
             return result.scalar()
 
-    async def _fetch_one_related(self, conn: AsyncConnection, now_data: Dict[str, Any]):
+    async def _fetch_one_related(self, conn: AsyncConnection, now_data: dict[str, Any]):
         for name, rfield in self.options.related_fields.items():
             related_data = await conn.execute(
                 rfield.related_model.__meta__.table.select().where(
                     getattr(rfield.related_model, rfield.foreign_key)
                     == now_data[rfield.foreign_key_self_name],
                 ),
             )
@@ -370,15 +397,15 @@
             now_data[name] = [
                 related_one._asdict() for related_one in related_data.fetchall()
             ]
 
     async def _fetch_many_related(
         self,
         conn: AsyncConnection,
-        now_datas: List[Dict[str, Any]],
+        now_datas: list[dict[str, Any]],
     ):
         for name, rfield in self.options.related_fields.items():
             related_values = [data[rfield.foreign_key_self_name] for data in now_datas]
             related_data = await conn.execute(
                 rfield.related_model.__meta__.table.select().where(
                     getattr(rfield.related_model, rfield.foreign_key).in_(
                         related_values,
@@ -476,83 +503,85 @@
 
 
 class ValuesQuerySet(QuerySetProtocol, Generic[T, Unpack[Ts]]):
     def __init__(
         self,
         query1: T,
         *querys: Unpack[Ts],
-        model_cls: Type[T_MODEL],
+        model_cls: type[T_MODEL],
         options: QueryOptions,
     ) -> None:
         self.query1 = query1
         self.querys = querys
         self.model_cls = model_cls
         self.options = options
 
-    async def first(self) -> Optional[Tuple[T, Unpack[Ts]]]:
+    async def first(self) -> Optional[tuple[T, Unpack[Ts]]]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
-                self.options.as_select_option(select(self.query1, *self.querys)),
+                self.options.as_select_option(select(self.query1, *self.querys)),  # type: ignore
             )
             if result_one := result.fetchone():
                 return result_one._tuple()
             return None
 
-    async def get(self) -> Tuple[T, Unpack[Ts]]:
+    async def get(self) -> tuple[T, Unpack[Ts]]:
         async with self.model_cls.database as conn:
             results = await self.all()
             if len(results) > 1:
                 raise MultipleDataError(
                     f"{self.model_cls} expect one data, but got {len(results)} datas",
                 )
             if len(results) == 1:
                 return results[0]
             raise NoMatchDataError(f"No match data for {self.model_cls}")
 
-    async def all(self) -> List[Tuple[T, Unpack[Ts]]]:
+    async def all(self) -> list[tuple[T, Unpack[Ts]]]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
-                self.options.as_select_option(select(self.query1, *self.querys)),
+                self.options.as_select_option(select(self.query1, *self.querys)),  # type: ignore
             )
             return [result_one._tuple() for result_one in result.fetchall()]
 
-    async def random_one(self) -> Optional[Tuple[T, Unpack[Ts]]]:
+    async def random_one(self) -> Optional[tuple[T, Unpack[Ts]]]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
                 self.options.as_select_option(
-                    select(self.query1, *self.querys).order_by(func.random()),
+                    select(self.query1, *self.querys).order_by(func.random()),  # type: ignore
                 ),
             )
             if result_one := result.fetchone():
                 return result_one._tuple()
             return None
 
-    async def paginate(self, page: int, page_size: int) -> List[Tuple[T, Unpack[Ts]]]:
+    async def paginate(self, page: int, page_size: int) -> list[tuple[T, Unpack[Ts]]]:
         if page < 1 or page_size < 1:
             raise PaginateArgError("page and page_size must be positive")
-        self.options.limit = page_size
-        self.options.offset = (page - 1) * page_size
+        # self.options.limit = page_size
+        self.options.funcs.append(("limit", False, page_size))
+        # self.options.offset = (page - 1) * page_size
+        self.options.funcs.append(("offset", False, (page - 1) * page_size))
         return await self.all()
 
 
 class ValueQuerySet(QuerySetProtocol, Generic[T]):
     def __init__(
         self,
         query: T,
-        model_cls: Type[T_MODEL],
+        model_cls: type[T_MODEL],
         options: QueryOptions,
     ) -> None:
         self.query = query
         self.model_cls = model_cls
         self.options = options
 
     async def first(self) -> Optional[T]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
-                self.options.as_select_option(select(self.query)),
+                self.options.as_select_option(select(self.query)),  # type: ignore
             )
             if result_one := result.fetchone():
                 return result_one._tuple()[0]
             return None
 
     async def get(self) -> T:
         results = await self.all()
@@ -560,101 +589,105 @@
             raise MultipleDataError(
                 f"{self.model_cls} expect one data, but got {len(results)} datas",
             )
         if len(results) == 1:
             return results[0]
         raise NoMatchDataError(f"No match data for {self.model_cls}")
 
-    async def all(self) -> List[T]:
+    async def all(self) -> list[T]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
-                self.options.as_select_option(select(self.query)),
+                self.options.as_select_option(select(self.query)),  # type: ignore
             )
             return [result_one._tuple()[0] for result_one in result.fetchall()]
 
     async def random_one(self) -> Optional[T]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
-                self.options.as_select_option(select(self.query)).order_by(
+                self.options.as_select_option(select(self.query)).order_by(  # type: ignore
                     func.random(),
                 ),
             )
             if result_one := result.fetchone():
                 return result_one._tuple()[0]
             return None
 
-    async def paginate(self, page: int, page_size: int) -> List[T]:
+    async def paginate(self, page: int, page_size: int) -> list[T]:
         if page < 1 or page_size < 1:
             raise PaginateArgError("page and page_size must be positive")
-        self.options.limit = page_size
-        self.options.offset = (page - 1) * page_size
+        # self.options.limit = page_size
+        self.options.funcs.append(("limit", False, page_size))
+        # self.options.offset = (page - 1) * page_size
+        self.options.funcs.append(("offset", False, (page - 1) * page_size))
         return await self.all()
 
 
 class ValueDictQuerySet(QuerySetProtocol):
     def __init__(
         self,
         *querys: Any,
-        model_cls: Type[T_MODEL],
+        model_cls: type[T_MODEL],
         options: QueryOptions,
     ) -> None:
         self.querys = querys or (model_cls.table,)
         self.model_cls = model_cls
         self.options = options
 
-    async def first(self) -> Optional[Dict[str, Any]]:
+    async def first(self) -> Optional[dict[str, Any]]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
                 self.options.as_select_option(select(*self.querys)),
             )
             if result_one := result.fetchone():
                 return result_one._asdict()
             return None
 
-    async def get(self) -> Dict[str, Any]:
+    async def get(self) -> dict[str, Any]:
         results = await self.all()
         if len(results) > 1:
             raise MultipleDataError(
                 f"{self.model_cls} expect one data, but got {len(results)} datas",
             )
         if len(results) == 1:
             return results[0]
         raise NoMatchDataError(f"No match data for {self.model_cls}")
 
-    async def all(self) -> List[Dict[str, Any]]:
+    async def all(self) -> list[dict[str, Any]]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
                 self.options.as_select_option(select(*self.querys)),
             )
             return [result_one._asdict() for result_one in result.fetchall()]
 
-    async def random_one(self) -> Optional[Dict[str, Any]]:
+    async def random_one(self) -> Optional[dict[str, Any]]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
                 self.options.as_select_option(select(*self.querys)).order_by(
                     func.random(),
                 ),
             )
             if result_one := result.fetchone():
                 return result_one._asdict()
             return None
 
-    async def paginate(self, page: int, page_size: int) -> List[Dict[str, Any]]:
+    async def paginate(self, page: int, page_size: int) -> list[dict[str, Any]]:
         if page < 1 or page_size < 1:
             raise PaginateArgError("page and page_size must be positive")
-        self.options.limit = page_size
-        self.options.offset = (page - 1) * page_size
+        # self.options.limit = page_size
+        self.options.funcs.append(("limit", False, page_size))
+        # self.options.offset = (page - 1) * page_size
+        self.options.funcs.append(("offset", False, (page - 1) * page_size))
         return await self.all()
 
 
 class CoalesceQuerySet(QuerySetProtocol, Generic[Unpack[Ts]]):
     def __init__(
         self,
         *columns: Unpack[Ts],
-        model_cls: Type[T_MODEL],
+        model_cls: type[T_MODEL],
         options: QueryOptions,
     ) -> None:
         self.columns = columns
         self.model_cls = model_cls
         self.options = options
 
     async def first(self) -> Union[Unpack[Ts], None]:
@@ -676,15 +709,15 @@
             raise MultipleDataError(
                 f"{self.model_cls} expect one data, but got {len(results)} datas",
             )
         if len(results) == 1:
             return results[0]
         raise NoMatchDataError(f"No match data for {self.model_cls}")
 
-    async def all(self) -> List[Union[Unpack[Ts], None]]:
+    async def all(self) -> list[Union[Unpack[Ts], None]]:
         async with self.model_cls.database as conn:
             result = await conn.execute(
                 self.options.as_select_option(
                     select(func.coalesce(*self.columns)).select_from(
                         self.model_cls.table,
                     ),
                 ),
@@ -706,13 +739,15 @@
                 return result_one[0]
             return None
 
     async def paginate(
         self,
         page: int,
         page_size: int,
-    ) -> List[Union[Unpack[Ts], None]]:
+    ) -> list[Union[Unpack[Ts], None]]:
         if page < 1 or page_size < 1:
             raise PaginateArgError("page and page_size must be positive")
-        self.options.limit = page_size
-        self.options.offset = (page - 1) * page_size
+        # self.options.limit = page_size
+        self.options.funcs.append(("limit", False, page_size))
+        # self.options.offset = (page - 1) * page_size
+        self.options.funcs.append(("offset", False, (page - 1) * page_size))
         return await self.all()
```

### Comparing `cherry_orm-0.3.0/cherry/typing.py` & `cherry_orm-1.0.0/cherry/typing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,11 @@
+from collections.abc import Mapping
 from typing import (
     Any,
-    Dict,
-    List,
     Literal,
-    Mapping,
-    Tuple,
-    Type,
     TYPE_CHECKING,
     TypeVar,
     Union,
 )
 from typing_extensions import TypeAlias, TypeVarTuple
 
 from sqlalchemy import BinaryExpression, BooleanClauseList
@@ -32,13 +28,13 @@
 NO_ACTION: Literal["NO ACTION"] = "NO ACTION"
 SET_DEFAULT: Literal["SET DEFAULT"] = "SET DEFAULT"
 
 T = TypeVar("T")
 Ts = TypeVarTuple("Ts")
 T_MODEL = TypeVar("T_MODEL", bound="Model")
 
-ModelType = Type["Model"]
-DictStrAny: TypeAlias = Dict[str, Any]
-TupleAny: TypeAlias = Tuple[Any, ...]
+ModelType = type["Model"]
+DictStrAny: TypeAlias = dict[str, Any]
+TupleAny: TypeAlias = tuple[Any, ...]
 AnyMapping: TypeAlias = Mapping[Any, Any]
-ClauseListType: TypeAlias = List[Union[BinaryExpression[bool], "ModelClause"]]
+ClauseListType: TypeAlias = list[Union[BinaryExpression[bool], "ModelClause"]]
 OptionalClause: TypeAlias = Union[BooleanClauseList, BinaryExpression, None]
```

### Comparing `cherry_orm-0.3.0/pyproject.toml` & `cherry_orm-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "cherry-orm"
-version = "0.3.0"
+version = "1.0.0"
 description = "Python asynchronous ORM based on SQLAlchemy and Pydantic."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["database", "orm", "sqlalchemy", "pydantic", "asyncio"]
 packages = [{ include = "cherry" }]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pydantic = "^1.10.10"
+python = "^3.9"
+pydantic = "^2.7.0"
 SQLAlchemy = "^2.0.22"
-khemia = "^0.1.0"
+khemia = "^0.1.1"
 aiosqlite = { version = "^0.19.0", optional = true }
 asyncmy = { version = "^0.2.8", optional = true }
 asyncpg = { version = "^0.28.0", optional = true }
 
 [tool.poetry.extras]
 sqlite = ["aiosqlite"]
 aiosqlite = ["aiosqlite"]
@@ -26,16 +26,16 @@
 postgresql = ["asyncpg"]
 asyncpg = ["asyncpg"]
 psycopg = ["psycopg"]
 all = ["aiosqlite", "asyncmy", "asyncpg"]
 
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.1.2"
-pre-commit = "^3.1.0"
+ruff = "^0.1.15"
+pre-commit = "^3.7.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.2.7"
@@ -62,15 +62,15 @@
     "C4",    # flake8-comprehensions
     "COM",   # flake8-commas
     "B",     # flake8-bugbear
     "ASYNC", # flake8-async
 ]
 ignore = ["E402", "B008", "F403", "F405", "B005", "B905", "F841"]
 line-length = 88
-target-version = "py38"
+target-version = "py39"
 ignore-init-module-imports = true
 
 
 [tool.ruff.isort]
 force-sort-within-sections = true
 extra-standard-library = ["typing_extensions"]
 force-wrap-aliases = true
@@ -85,11 +85,18 @@
     "third-party",
 ]
 
 [tool.ruff.pycodestyle]
 ignore-overlong-task-comments = true
 max-doc-length = 120
 
+[tool.pyright]
+pythonVersion = "3.9"
+pythonPlatform = "All"
+defineConstant = { PYDANTIC_V2 = true }
+typeCheckingMode = "basic"
+reportShadowedImports = false
+disableBytesTypePromotions = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cherry_orm-0.3.0/PKG-INFO` & `cherry_orm-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: cherry-orm
-Version: 0.3.0
+Version: 1.0.0
 Summary: Python asynchronous ORM based on SQLAlchemy and Pydantic.
 License: MIT
 Keywords: database,orm,sqlalchemy,pydantic,asyncio
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: aiomysql
 Provides-Extra: aiosqlite
 Provides-Extra: all
@@ -23,55 +22,55 @@
 Provides-Extra: postgresql
 Provides-Extra: psycopg
 Provides-Extra: sqlite
 Requires-Dist: SQLAlchemy (>=2.0.22,<3.0.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0) ; extra == "sqlite" or extra == "aiosqlite" or extra == "all"
 Requires-Dist: asyncmy (>=0.2.8,<0.3.0) ; extra == "mysql" or extra == "asyncmy" or extra == "all"
 Requires-Dist: asyncpg (>=0.28.0,<0.29.0) ; extra == "postgresql" or extra == "asyncpg" or extra == "all"
-Requires-Dist: khemia (>=0.1.0,<0.2.0)
-Requires-Dist: pydantic (>=1.10.10,<2.0.0)
+Requires-Dist: khemia (>=0.1.1,<0.2.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
     <h1 align="center">Cherry ORM</h1>
     <p align="center">Python 异步 ORM</p>
 </p>
 <p align="center">
     <a href="./LICENSE">
         <img src="https://img.shields.io/github/license/CMHopeSunshine/cherry-orm.svg" alt="license">
     </a>
     <a href="https://pypi.python.org/pypi/cherry-orm">
         <img src="https://img.shields.io/pypi/v/cherry-orm.svg" alt="pypi">
     </a>
     <a href="https://www.python.org/">
-        <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+        <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     </a>
 </p>
 
 <p align="center">
     <strong>简体中文</strong>
     ·
     <a href="https://github.com/CMHopeSunshine/cherry-orm/blob/master/README_EN.md">English</a>
 </p>
 
 ## 简介
 
-`Cherry ORM` 是一个 Python 的异步对象关系映射（ORM）库，它基于 [SQLAlchemy Core](https://www.sqlalchemy.org/) 和 [Pydantic V1](https://docs.pydantic.dev/1.10/) 构建。
+`Cherry ORM` 是一个 Python 的异步对象关系映射（ORM）库，它基于 [SQLAlchemy Core](https://www.sqlalchemy.org/) 和 [Pydantic V2](https://docs.pydantic.dev/latest/) 构建。
 
 它的一切设计都是为了简单易用，极大地减少开发者的数据库操作成本，提高开发效率，让开发者更专注于业务逻辑的实现。
 
 ## 安装
 
 - 使用 pip: `pip install cherry-orm`
 - 使用 Poetry: `poetry add cherry-orm`
 - 使用 PDM: `pdm add cherry-orm`
 
 ## 文档
 
--> [文档地址](https://cherry.cherishmoon.fun)
+-> [文档地址](https://cherry.cherishmoon.top)
 
 ## 示例
 
 ```python
 from datetime import date
 from typing import List, Optional
 
@@ -83,27 +82,23 @@
 class Student(cherry.Model):
     id: int = cherry.Field(primary_key=True)
     name: str = cherry.Field(unique=True, index=True)
     age: int
     birthday: date = cherry.Field(default_factory=date.today)
     school: cherry.ForeignKey[Optional["School"]] = None
 
-    class Meta:
-        database = db
-        tablename = "student"
+    cherry_config = cherry.CherryConfig(tablename="student", database=db)
 
 
 class School(cherry.Model):
     id: cherry.PrimaryKey[int]
     name: str = cherry.Field(unique=True, index=True)
     students: cherry.ReverseRelation[List[Student]] = []
 
-    class Meta:
-        database = db
-        tablename = "school"
+    cherry_config = cherry.CherryConfig(tablename="school", database=db)
 
 
 async def main():
     await db.init()
 
     # 插入
     school = await School(id=1, name="school 1").insert()
```

