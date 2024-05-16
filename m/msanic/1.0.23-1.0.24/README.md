# Comparing `tmp/msanic-1.0.23-py3-none-any.whl.zip` & `tmp/msanic-1.0.24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 59350 bytes, number of entries: 42
+Zip file size: 59377 bytes, number of entries: 42
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 msanic/__init__.py
 -rw-rw-rw-  2.0 fat     3462 b- defN 24-Apr-15 07:17 msanic/base_blue.py
 -rw-rw-rw-  2.0 fat     8536 b- defN 24-May-05 02:44 msanic/base_conf.py
 -rw-rw-rw-  2.0 fat     3241 b- defN 24-Mar-25 14:10 msanic/base_server.py
 -rw-rw-rw-  2.0 fat     9666 b- defN 24-May-10 03:10 msanic/base_ws.py
 -rw-rw-rw-  2.0 fat     2908 b- defN 24-Apr-28 08:44 msanic/exception.py
 -rw-rw-rw-  2.0 fat     7677 b- defN 24-Apr-15 07:12 msanic/handler_http.py
@@ -21,24 +21,24 @@
 -rw-rw-rw-  2.0 fat     2495 b- defN 24-Mar-21 14:40 msanic/libs/mult_log.py
 -rw-rw-rw-  2.0 fat     5263 b- defN 24-Mar-21 14:40 msanic/libs/random_maker.py
 -rw-rw-rw-  2.0 fat     8705 b- defN 24-May-10 09:56 msanic/libs/rds_client.py
 -rw-rw-rw-  2.0 fat     1116 b- defN 24-Apr-03 08:13 msanic/libs/rds_locker.py
 -rw-rw-rw-  2.0 fat     6985 b- defN 24-Apr-28 09:19 msanic/libs/tool.py
 -rw-rw-rw-  2.0 fat     5014 b- defN 24-Mar-25 15:32 msanic/libs/tool_dt.py
 -rw-rw-rw-  2.0 fat     3070 b- defN 24-Mar-21 14:40 msanic/libs/tool_jwt.py
--rw-rw-rw-  2.0 fat     2031 b- defN 24-May-04 15:37 msanic/libs/tool_ws.py
+-rw-rw-rw-  2.0 fat     1956 b- defN 24-May-16 08:01 msanic/libs/tool_ws.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-20 12:48 msanic/orm/__init__.py
 -rw-rw-rw-  2.0 fat      730 b- defN 24-Mar-19 13:56 msanic/orm/db_index.py
 -rw-rw-rw-  2.0 fat    18726 b- defN 24-Apr-28 08:44 msanic/orm/db_model.py
 -rw-rw-rw-  2.0 fat    11698 b- defN 24-Apr-03 07:45 msanic/orm/mssql_generator.py
 -rw-rw-rw-  2.0 fat    11743 b- defN 24-Apr-28 08:44 msanic/orm/mysql_generator.py
 -rw-rw-rw-  2.0 fat    11720 b- defN 24-Apr-03 07:45 msanic/orm/pgsql_generator.py
 -rw-rw-rw-  2.0 fat     5098 b- defN 24-Apr-12 02:19 msanic/orm/rc_model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 test/__init__.py
 -rw-rw-rw-  2.0 fat      701 b- defN 24-May-04 15:15 test/test_unit.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-10 09:56 msanic-1.0.23.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4801 b- defN 24-May-10 09:56 msanic-1.0.23.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 09:56 msanic-1.0.23.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       52 b- defN 24-May-10 09:56 msanic-1.0.23.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 24-May-10 09:56 msanic-1.0.23.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3314 b- defN 24-May-10 09:56 msanic-1.0.23.dist-info/RECORD
-42 files, 182817 bytes uncompressed, 54156 bytes compressed:  70.4%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-16 08:01 msanic-1.0.24.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4918 b- defN 24-May-16 08:01 msanic-1.0.24.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:01 msanic-1.0.24.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       52 b- defN 24-May-16 08:01 msanic-1.0.24.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-16 08:01 msanic-1.0.24.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3314 b- defN 24-May-16 08:01 msanic-1.0.24.dist-info/RECORD
+42 files, 182859 bytes uncompressed, 54183 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -102,26 +102,26 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_unit.py
 Comment: 
 
-Filename: msanic-1.0.23.dist-info/LICENSE
+Filename: msanic-1.0.24.dist-info/LICENSE
 Comment: 
 
-Filename: msanic-1.0.23.dist-info/METADATA
+Filename: msanic-1.0.24.dist-info/METADATA
 Comment: 
 
-Filename: msanic-1.0.23.dist-info/WHEEL
+Filename: msanic-1.0.24.dist-info/WHEEL
 Comment: 
 
-Filename: msanic-1.0.23.dist-info/entry_points.txt
+Filename: msanic-1.0.24.dist-info/entry_points.txt
 Comment: 
 
-Filename: msanic-1.0.23.dist-info/top_level.txt
+Filename: msanic-1.0.24.dist-info/top_level.txt
 Comment: 
 
-Filename: msanic-1.0.23.dist-info/RECORD
+Filename: msanic-1.0.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## msanic/libs/tool_ws.py

```diff
@@ -1,11 +1,9 @@
 from typing import Union
 
-from sanic.server.protocols.websocket_protocol import WebSocketProtocol
-
 from msanic.libs.consts import Code, StaCode
 from msanic.libs.tool import json_encode, json_parse
 
 
 def pack_msg(
         cmd_type: Union[int, str],
         cmd_code: Union[int, str],
```

## Comparing `msanic-1.0.23.dist-info/LICENSE` & `msanic-1.0.24.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `msanic-1.0.23.dist-info/METADATA` & `msanic-1.0.24.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msanic
-Version: 1.0.23
+Version: 1.0.24
 Summary: A web framework who is use sanic + tortoise-orm + redis to quick create http&websocket server.
 Author: DHDONG
 Author-email: zscych@qq.com
 License: MIT
 Keywords: WebServer,Sanic,WebSite Develop,Web Framework
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,21 +16,21 @@
 Requires-Dist: redis[hiredis] >=4.4.0
 Requires-Dist: pyjwt >=0.2.6
 Requires-Dist: httpx >=0.23.0
 Requires-Dist: orjson >=3.9.15
 Requires-Dist: tzdata >=2023.1
 Requires-Dist: pycryptodome >=3.16.0
 
-# Sanic Server
+# Sanic Server 后续该项目将迁移至nsanic（nice sanic），后续更新都将在新项目上进行，该项目不再维护  
   
 ## 设计与依赖说明  
 1. 服务体系 -- 基于sanic 22.3.x 以上版本的http/websocket服务框架  
 2. python环境 -- 基于3.9的async/await原生异步模型  
 3. ORM -- 采用tortoise-orm -- 0.19.1 以上的异步ORM数据模型  
-4. 数据库连接驱动 -- 建议MySQL/mariaDB采用aiomysql, postgresql采用asyncpg  
+4. 数据库连接驱动 -- 默认MySQL/mariaDB采用asyncmy, postgresql采用asyncpg  
 5. 数据迁移工具 -- 使用aerich作为基本的数据迁移工具  
 6. 缓存 -- 采用redis作为公有化基础缓存，版本建议 6.x以上  
 7. 缓存驱动 -- 官方redis驱动支持，采用连接池模式  
   
 ## 项目说明  
 参照项目目录
 logs        -- 运行日志存放目录，按服务区分，服务停止情况下，删除后会自动生成
```

## Comparing `msanic-1.0.23.dist-info/RECORD` & `msanic-1.0.24.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 msanic/libs/mult_log.py,sha256=wN-Wu2Q8byarCyu34mBmeBJUPIvmYZy6BVauifRoZDQ,2495
 msanic/libs/random_maker.py,sha256=-7ybIY0LrQ4eqvrCYc9kHBgnzqaEyRAYo57KOXKtRCA,5263
 msanic/libs/rds_client.py,sha256=MM06CYV_kHmDm954kPK_h0c-4MDpXlcoZ6c7O01p3oM,8705
 msanic/libs/rds_locker.py,sha256=Q8UkKAyHz4xdoG_oL0j5BfsBpTeKbW8sy7yDXwO62_E,1116
 msanic/libs/tool.py,sha256=7Bp0KkNMiuLnSATXccaBdW5Qz3FWaPykVNemfGu-Xb0,6985
 msanic/libs/tool_dt.py,sha256=ymTQBwxoUHigSX_L06LHDjzGBNmKjKXTLLAQBv_ssA8,5014
 msanic/libs/tool_jwt.py,sha256=cCdHNB16fp3MZfDT77ocUtHFtOrQjKu1qZL9x2iCI0A,3070
-msanic/libs/tool_ws.py,sha256=17HCilJU6_DC9BUnSxWzySVlcqa5h3KYAnIXR1UDFNo,2031
+msanic/libs/tool_ws.py,sha256=HjrnlSHbEJ14COgBoS4iQ34auwGDxgJ6ScPGWbO_jnE,1956
 msanic/orm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 msanic/orm/db_index.py,sha256=LmqneAZnHPfWsWNS4wH6F8iyZ56xtXtczglRFOZtgHA,730
 msanic/orm/db_model.py,sha256=Gd9Zm7DjiEH4xGEqM19Iar-2tTMY5lziRfaBlWOBLZ0,18726
 msanic/orm/mssql_generator.py,sha256=c9q71hljWqBxoNriG0OefwD48w3gVTb62HnFKjreom4,11698
 msanic/orm/mysql_generator.py,sha256=6AMVa9twa7GRCuTlEga5g2zHJvkCD9YocUwGGcvLQ4Q,11743
 msanic/orm/pgsql_generator.py,sha256=BMNDAZ-2X9dPbUOBlhR5UJBfqXWpl23KRgTozleKCCQ,11720
 msanic/orm/rc_model.py,sha256=NcgSVW34eSx_TiMYE9DYrA6Bt_qitTRH5pX3UYqa6ok,5098
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_unit.py,sha256=zIZWr20nXYmLsKZpGZv-dmRuwQTJXyTcAcUDbx3FdF0,701
-msanic-1.0.23.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
-msanic-1.0.23.dist-info/METADATA,sha256=7bss3xgpQDK4OZza02bn0GoOYgOTyBznx_foqvqjM6Q,4801
-msanic-1.0.23.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-msanic-1.0.23.dist-info/entry_points.txt,sha256=CAoZ_qtmP0HhzVmX9w0oN-KSxoCpdqxjDC4pljoU-l4,52
-msanic-1.0.23.dist-info/top_level.txt,sha256=lT96LXfr87NYrx1PR9GraMGNX9KQ6ImvR88MTHEhBkM,12
-msanic-1.0.23.dist-info/RECORD,,
+msanic-1.0.24.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
+msanic-1.0.24.dist-info/METADATA,sha256=KgBvxz-tIqS9I4_IkY7deVJdVtxIPL18I92EU7EkYO0,4918
+msanic-1.0.24.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+msanic-1.0.24.dist-info/entry_points.txt,sha256=CAoZ_qtmP0HhzVmX9w0oN-KSxoCpdqxjDC4pljoU-l4,52
+msanic-1.0.24.dist-info/top_level.txt,sha256=lT96LXfr87NYrx1PR9GraMGNX9KQ6ImvR88MTHEhBkM,12
+msanic-1.0.24.dist-info/RECORD,,
```

