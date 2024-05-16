# Comparing `tmp/matter_persistence-1.0.0-py3-none-any.whl.zip` & `tmp/matter_persistence-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 14747 bytes, number of entries: 20
+Zip file size: 15062 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_persistence/__about__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 matter_persistence/__init__.py
 -rw-r--r--  2.0 unx     3778 b- defN 20-Feb-02 00:00 matter_persistence/decorators.py
 -rw-r--r--  2.0 unx     1062 b- defN 20-Feb-02 00:00 matter_persistence/foundation_model.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 matter_persistence/redis/__init__.py
 -rw-r--r--  2.0 unx     4910 b- defN 20-Feb-02 00:00 matter_persistence/redis/async_redis_client.py
 -rw-r--r--  2.0 unx      404 b- defN 20-Feb-02 00:00 matter_persistence/redis/base.py
 -rw-r--r--  2.0 unx     1956 b- defN 20-Feb-02 00:00 matter_persistence/redis/cache_helper.py
 -rw-r--r--  2.0 unx      337 b- defN 20-Feb-02 00:00 matter_persistence/redis/exceptions.py
--rw-r--r--  2.0 unx     6117 b- defN 20-Feb-02 00:00 matter_persistence/redis/manager.py
+-rw-r--r--  2.0 unx     9145 b- defN 20-Feb-02 00:00 matter_persistence/redis/manager.py
 -rw-r--r--  2.0 unx     1326 b- defN 20-Feb-02 00:00 matter_persistence/redis/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 matter_persistence/sql/__init__.py
 -rw-r--r--  2.0 unx     2532 b- defN 20-Feb-02 00:00 matter_persistence/sql/base.py
 -rw-r--r--  2.0 unx      513 b- defN 20-Feb-02 00:00 matter_persistence/sql/exceptions.py
 -rw-r--r--  2.0 unx     3607 b- defN 20-Feb-02 00:00 matter_persistence/sql/manager.py
 -rw-r--r--  2.0 unx     3971 b- defN 20-Feb-02 00:00 matter_persistence/sql/utils.py
-?rw-r--r--  2.0 unx     2900 b- defN 20-Feb-02 00:00 matter_persistence-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_persistence-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_persistence-1.0.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1801 b- defN 20-Feb-02 00:00 matter_persistence-1.0.0.dist-info/RECORD
-20 files, 36503 bytes uncompressed, 11745 bytes compressed:  67.8%
+?rw-r--r--  2.0 unx     2901 b- defN 20-Feb-02 00:00 matter_persistence-1.1.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_persistence-1.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_persistence-1.1.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1801 b- defN 20-Feb-02 00:00 matter_persistence-1.1.0.dist-info/RECORD
+20 files, 39532 bytes uncompressed, 12060 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: matter_persistence/sql/manager.py
 Comment: 
 
 Filename: matter_persistence/sql/utils.py
 Comment: 
 
-Filename: matter_persistence-1.0.0.dist-info/METADATA
+Filename: matter_persistence-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: matter_persistence-1.0.0.dist-info/WHEEL
+Filename: matter_persistence-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: matter_persistence-1.0.0.dist-info/licenses/LICENSE
+Filename: matter_persistence-1.1.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_persistence-1.0.0.dist-info/RECORD
+Filename: matter_persistence-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_persistence/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.0.0"
+__version__ = "1.1.0"
```

## matter_persistence/redis/manager.py

```diff
@@ -20,14 +20,17 @@
 
     Methods:
     - __get_cache_client: Private method to get the cache client.
     - save_value: Saves a value to the cache with an optional expiration time.
     - get_value: Retrieves a value from the cache.
     - delete_value: Deletes a value from the cache.
     - cache_record_exists: Checks if a cache record exists.
+    - save_with_key: Saves a value to the cache with an optional expiration time using a key.
+    - get_with_key: Retrieves a value from the cache using a key.
+    - delete_with_key: Deletes a value from the cache using a key.
     - is_cache_alive: Checks if the cache client is alive.
 
     Usage example:
         Check examples/redis.ipynb for usage examples.
     """
 
     def __init__(
@@ -152,13 +155,83 @@
             organization_id=organization_id,
             internal_id=str(internal_id),
             object_class=object_class,
         )
         async with self.__get_cache_client() as cache_client:
             return bool(await cache_client.exists(key))  # cache_client.exists() returns 0 or 1
 
+    async def save_with_key(
+        self,
+        key: str,
+        value: Any,
+        object_class: type[Model] | None = None,
+        expiration_in_seconds: int | None = None,
+    ):
+        object_name = object_class.__name__ if object_class else None
+        hash_key = CacheHelper.create_basic_hash_key(key, object_name)
+        if object_class:
+            value = value.model_dump_json()
+
+        async with self.__get_cache_client() as cache_client:
+            if expiration_in_seconds:
+                result = await cache_client.set_value(hash_key, value, ttl=expiration_in_seconds)
+            else:
+                result = await cache_client.set_value(hash_key, value)
+
+        if not result:
+            raise CacheRecordNotSavedError(
+                description=f"Unable to store value in cache. Key: {key}",
+                detail={"key": key, "hash_key": hash_key},
+            )
+
+        return result
+
+    async def get_with_key(self, key: str, object_class: type[Model] | None = None) -> Any:
+        object_name = object_class.__name__ if object_class else None
+        hash_key = CacheHelper.create_basic_hash_key(key, object_name)
+        async with self.__get_cache_client() as cache_client:
+            value = await cache_client.get_value(hash_key)
+        if not value:
+            raise CacheRecordNotFoundError(
+                description=f"Unable to retrieve value from cache. Key: {key}",
+                detail={"key": key, "hash_key": hash_key},
+            )
+
+        if object_class:
+            if isinstance(value, list):
+                value = [object_class.model_validate_json(item) for item in value]
+            else:
+                value = object_class.model_validate_json(value)
+
+        return value
+
+    async def delete_with_key(
+        self,
+        key: str,
+        object_class: type[Model] | None = None,
+    ) -> Any:
+        object_name = object_class.__name__ if object_class else None
+        hash_key = CacheHelper.create_basic_hash_key(key, object_name)
+
+        async with self.__get_cache_client() as cache_client:
+            if not await cache_client.delete_key(hash_key):
+                raise CacheRecordNotFoundError(
+                    description=f"Unable to retrieve value from cache. Key: {key}",
+                    detail={"key": key, "hash_key": hash_key},
+                )
+
+    async def cache_record_with_key_exists(
+        self,
+        key: str,
+        object_class: type[Model] | None = None,
+    ) -> bool:
+        object_name = object_class.__name__ if object_class else None
+        hash_key = CacheHelper.create_basic_hash_key(key, object_name)
+        async with self.__get_cache_client() as cache_client:
+            return bool(await cache_client.exists(hash_key))  # cache_client.exists() returns 0 or 1
+
     async def is_cache_alive(self):
         """
         Checks if the cache client is alive.
         """
         async with self.__get_cache_client() as cache_client:
             return await cache_client.is_alive()
```

## Comparing `matter_persistence-1.0.0.dist-info/METADATA` & `matter_persistence-1.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: matter-persistence
-Version: 1.0.0
+Version: 1.1.0
 Summary: Matter persistance library.
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-persistence#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-persistence/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-persistence
 Author-email: Rômulo Jales <romulo@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -63,7 +63,8 @@
 assume a deleted field!
 
 *Check usage example for* **DatabaseManager** *and some of the utility functions in [examples/sql](./examples/sql.ipynb).*
 
 ## Contributing
 
 for contributions, check the [CONTRIBUTING.md](CONTRIBUTING.md) file
+
```

## Comparing `matter_persistence-1.0.0.dist-info/licenses/LICENSE` & `matter_persistence-1.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_persistence-1.0.0.dist-info/RECORD` & `matter_persistence-1.1.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-matter_persistence/__about__.py,sha256=dmRc9IvjUx73VWAI-p5tuBWiZMJz5_SUSYLP769tv9M,134
+matter_persistence/__about__.py,sha256=bY_nM7erfu6ZowAj4rj9sUxHb6UwLAepqSYI0RRu0ck,134
 matter_persistence/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 matter_persistence/decorators.py,sha256=ztVSkwrNmwWlJyrY4jjVL8ZWSgQbqhknXjASTJ_S2KY,3778
 matter_persistence/foundation_model.py,sha256=uSLJR5hh7qNFKEdKLvLPrR2yCc433PBHL5CuSi-4y7I,1062
 matter_persistence/redis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 matter_persistence/redis/async_redis_client.py,sha256=xDSQjCit9eA4AW6HLss9W-l8iVaAZBB48Ofg37CWo30,4910
 matter_persistence/redis/base.py,sha256=CL1ktGe2bu919VP6E41Y9VhOTDBK7EANPZSG--D4TPA,404
 matter_persistence/redis/cache_helper.py,sha256=bUXi_gyPCbhHYOwKvKAOwD8Mu3j4CFVzJaATuoshs9o,1956
 matter_persistence/redis/exceptions.py,sha256=0-FTL359fGBRK-uo4a5k2dZgkat6meF8hyhrIDjlaFo,337
-matter_persistence/redis/manager.py,sha256=dUx656IaMdaTvtD-ROWEO05LsvCNtE5gN8pUCuHCQRo,6117
+matter_persistence/redis/manager.py,sha256=Xk9SY27tHo8PZg8xJx0krC_KY_qzHgBX03z7vQiAb1A,9145
 matter_persistence/redis/utils.py,sha256=GgDFPqiJzBbcqTlFl4A1ENhLUlnhefybc5i04Sz9cSQ,1326
 matter_persistence/sql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 matter_persistence/sql/base.py,sha256=DSgJDT_jbdG0bnV35A_Wbi3zdVcpL7_oqeynTCsg-vU,2532
 matter_persistence/sql/exceptions.py,sha256=v4ZJk3krK0nt0Xdtmjiy0eOuj5N1QZyVH1i94jw17DM,513
 matter_persistence/sql/manager.py,sha256=78xpqQP8GRP1SErgzpvFoIM61XuK_ihCJJA_z8OVlSg,3607
 matter_persistence/sql/utils.py,sha256=rLF9Ym7bHuJmN2WCkc4yJmJW6WLR-OKy9hLM2HBxs7g,3971
-matter_persistence-1.0.0.dist-info/METADATA,sha256=bcaLpT8ClKdK_tab2h_Iu_D_1O5Cu5NTfVi_lQddi1g,2900
-matter_persistence-1.0.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-matter_persistence-1.0.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_persistence-1.0.0.dist-info/RECORD,,
+matter_persistence-1.1.0.dist-info/METADATA,sha256=SQCTyu0xo31RbMu0g9cKU9J77sIwhEPNM3qysdGd2Po,2901
+matter_persistence-1.1.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+matter_persistence-1.1.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_persistence-1.1.0.dist-info/RECORD,,
```

