# Comparing `tmp/coll-filter-1.2.7.tar.gz` & `tmp/coll-filter-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coll-filter-1.2.7.tar", last modified: Tue May  7 06:16:36 2024, max compression
+gzip compressed data, was "coll-filter-1.2.8.tar", last modified: Thu May 16 00:37:39 2024, max compression
```

## Comparing `coll-filter-1.2.7.tar` & `coll-filter-1.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-07 06:16:36.753139 coll-filter-1.2.7/
--rw-r--r--   0 summy      (501) staff       (20)      960 2024-05-07 06:16:36.752159 coll-filter-1.2.7/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      605 2024-04-29 01:47:24.000000 coll-filter-1.2.7/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-07 06:16:36.744669 coll-filter-1.2.7/cf/
--rw-r--r--   0 summy      (501) staff       (20)     6587 2024-05-07 01:40:56.000000 coll-filter-1.2.7/cf/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     9618 2024-05-07 06:13:06.000000 coll-filter-1.2.7/cf/base.py
--rw-r--r--   0 summy      (501) staff       (20)     4532 2024-05-07 01:32:27.000000 coll-filter-1.2.7/cf/pooling.py
--rw-r--r--   0 summy      (501) staff       (20)     2840 2024-05-07 01:21:41.000000 coll-filter-1.2.7/cf/utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-07 06:16:36.749851 coll-filter-1.2.7/coll_filter.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      960 2024-05-07 06:16:36.000000 coll-filter-1.2.7/coll_filter.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-07 06:16:36.000000 coll-filter-1.2.7/coll_filter.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-07 06:16:36.000000 coll-filter-1.2.7/coll_filter.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-07 06:16:36.000000 coll-filter-1.2.7/coll_filter.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        3 2024-05-07 06:16:36.000000 coll-filter-1.2.7/coll_filter.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-07 06:16:36.753564 coll-filter-1.2.7/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      846 2024-05-07 06:16:19.000000 coll-filter-1.2.7/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-07 06:16:36.750734 coll-filter-1.2.7/test/
--rw-r--r--   0 summy      (501) staff       (20)      277 2024-01-05 03:59:08.000000 coll-filter-1.2.7/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-16 00:37:39.478166 coll-filter-1.2.8/
+-rw-r--r--   0 summy      (501) staff       (20)      960 2024-05-16 00:37:39.477432 coll-filter-1.2.8/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      605 2024-04-29 01:47:24.000000 coll-filter-1.2.8/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-16 00:37:39.469546 coll-filter-1.2.8/cf/
+-rw-r--r--   0 summy      (501) staff       (20)     7310 2024-05-16 00:23:21.000000 coll-filter-1.2.8/cf/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     9560 2024-05-16 00:33:23.000000 coll-filter-1.2.8/cf/base.py
+-rw-r--r--   0 summy      (501) staff       (20)     4696 2024-05-16 00:33:23.000000 coll-filter-1.2.8/cf/pooling.py
+-rw-r--r--   0 summy      (501) staff       (20)     2840 2024-05-07 01:21:41.000000 coll-filter-1.2.8/cf/utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-16 00:37:39.475255 coll-filter-1.2.8/coll_filter.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      960 2024-05-16 00:37:39.000000 coll-filter-1.2.8/coll_filter.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-16 00:37:39.000000 coll-filter-1.2.8/coll_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-16 00:37:39.000000 coll-filter-1.2.8/coll_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-16 00:37:39.000000 coll-filter-1.2.8/coll_filter.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        3 2024-05-16 00:37:39.000000 coll-filter-1.2.8/coll_filter.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-16 00:37:39.478794 coll-filter-1.2.8/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      846 2024-05-16 00:37:05.000000 coll-filter-1.2.8/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-16 00:37:39.476066 coll-filter-1.2.8/test/
+-rw-r--r--   0 summy      (501) staff       (20)      277 2024-01-05 03:59:08.000000 coll-filter-1.2.8/test/test.py
```

### Comparing `coll-filter-1.2.7/PKG-INFO` & `coll-filter-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coll-filter
-Version: 1.2.7
+Version: 1.2.8
 Summary: Collaborative Filtering with multi-process parallelism.
 Home-page: https://gitee.com/summry/myai
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: Collaborative Filtering,recommend
 Platform: UNKNOWN
```

### Comparing `coll-filter-1.2.7/README.rst` & `coll-filter-1.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `coll-filter-1.2.7/cf/__init__.py` & `coll-filter-1.2.8/cf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,15 +100,30 @@
         @param item_similar  物品相似矩阵
         @param similar_fn  相似度计算函数
         @return {user_id: [(item_id, score),],}
         """
         assert recall_num > 0, "'recall_num' should be a positive number."
         return self._coll_filter.item_cf(recall_num, similar_num, user_ids, item_similar, similar_fn)
 
-    def recommend(self, user_id: U, recall_num=64, similar_num=8, similar_fn=None, ratio=0.5) -> List[Tuple[T, float]]:
+    def recommend(self, user_id: U, recall_num=64, similar_num=8, similar_fn=None, ratio=0.5, return_score=False) \
+            -> List[Tuple[T, float]]:
+        """
+        给一个用户推荐
+        @param user_id  要推荐的用户
+        @param recall_num  每个用户最大召回个数
+        @param similar_num  每个物品最大相似物品个数
+        @param similar_fn  相似度计算函数
+        @param ratio  推荐结果中item_cf所占比例
+        @param return_score 是否返回分数
+        @return [item_id,] or [(item_id, score),]
+        """
+        result = self._recommend(user_id, recall_num, similar_num, similar_fn, ratio)
+        return result if return_score else [item[0] for item in result]
+
+    def _recommend(self, user_id: U, recall_num, similar_num, similar_fn, ratio) -> List[Tuple[T, float]]:
         """
         给一个用户推荐
         @param user_id  要推荐的用户
         @param recall_num  每个用户最大召回个数
         @param similar_num  每个物品最大相似物品个数
         @param similar_fn  相似度计算函数
         @param ratio  推荐结果中item_cf所占比例
```

### Comparing `coll-filter-1.2.7/cf/base.py` & `coll-filter-1.2.8/cf/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,31 +86,29 @@
         @param recall_num  每个用户推荐结果数目
         @param similar_num  用户相似矩阵最大个数
         @param user_ids  要推荐的用户列表
         @param user_similar  用户相似矩阵
         @param similar_fn  相似度计算函数
         @return {user_id: [(item, score),],}
         """
-        if user_similar is None:
-            user_similar = self.cal_similar(CFType.UCF, similar_num, similar_fn)
+        user_similar = user_similar or self.cal_similar(CFType.UCF, similar_num, similar_fn)
         return self._cf(user_ids, user_similar, recall_num, CFType.UCF)
 
     def item_cf(self, recall_num=10, similar_num=256, user_ids=None, item_similar=None, similar_fn=None):
         """
         物品协同过滤
 
         @param recall_num  每个用户推荐结果数目
         @param similar_num  物品相似矩阵最大个数
         @param user_ids  要推荐的用户列表
         @param item_similar  物品相似矩阵
         @param similar_fn  相似度计算函数
         @return {user_id: [(item, score),],}
         """
-        if item_similar is None:
-            item_similar = self.cal_similar(CFType.ICF, similar_num, similar_fn)
+        item_similar = item_similar or self.cal_similar(CFType.ICF, similar_num, similar_fn)
         return self._cf(user_ids, item_similar, recall_num, CFType.ICF)
 
     def cal_similar(self, cf_type: CFType, similar_num=256, similar_fn=None):
         """
         计算相似度
 
         @return dict{:List()}    {user1: {user2: similar}}
@@ -139,15 +137,15 @@
         计算相似度
 
         @return dict{:List()}    {user1: {user2: similar}}
         """
         logger.info(f'开始{cf_type.value}相似度计算, similar_num = {similar_num}')
         func_start_time = time.perf_counter()
         dict1, items_list, cal_similar_func = self._get_cal_similar_inputs(cf_type)
-        similar_fn = similar_fn if similar_fn else self.similar_fn
+        similar_fn = similar_fn or self.similar_fn
         similar = cal_similar_func(dict1, items_list, similar_fn)
         similar = sort_similar(similar, similar_num)
         print_cost_time(f"完成{cf_type.value}相似度计算, 当前进程<{os.getpid()}> 总生成 {len(similar)} 条记录, 总耗时", func_start_time)
         return similar
 
     def _get_cal_similar_inputs(self, cf_type: CFType):
         if cf_type == CFType.UCF:
```

### Comparing `coll-filter-1.2.7/cf/pooling.py` & `coll-filter-1.2.8/cf/pooling.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from multiprocessing import Pool
 from typing import Iterable, Tuple
 from .base import BaseCollFilter
 from . import default_similar_func, CFType, U, T
 from .utils import print_cost_time, sort_similar, logger
 
 
+PARALLEL_THRESHOLD = 4096
+
+
 class PoolMultiProcessor:
 
     def __init__(self, parallel_num):
         cpu_count = os.cpu_count()
         self.parallel_num = cpu_count if parallel_num <= 1 else parallel_num
         self.pool = Pool(cpu_count - 1) if self.parallel_num >= cpu_count else Pool(self.parallel_num - 1)
 
@@ -77,16 +80,19 @@
 
         @return dict{:dict}    {user1: {user2: similar}}
         """
         logger.info(f'开始{cf_type.value}相似度计算, similar_num: {similar_num}')
         func_start_time = time.perf_counter()
         dict1, items_list, cal_similar_func = self._get_cal_similar_inputs(cf_type)
         items_list = list(items_list)
-        similar_fn = similar_fn if similar_fn else self.similar_fn
-        similar = self.processor.cal_similar(dict1, items_list, cal_similar_func, similar_fn)
+        similar_fn = similar_fn or self.similar_fn
+        if len(items_list) <= PARALLEL_THRESHOLD:
+            similar = cal_similar_func(dict1, items_list, similar_fn)
+        else:
+            similar = self.processor.cal_similar(dict1, items_list, cal_similar_func, similar_fn)
         similar = sort_similar(similar, similar_num)
         print_cost_time(f"完成{cf_type.value}相似度计算, 当前进程<{os.getpid()}>, 总生成 {len(similar)} 条记录, 总耗时", func_start_time)
         return similar
         self.processor.release()
 
     def _cf(self, user_ids, similar_dict, recall_num, cf_type: CFType):
         logger.info(f'开始{cf_type.value}推理, recall_num: {recall_num}')
@@ -96,14 +102,14 @@
                 return {user_id: [] for user_id in user_ids}
 
             user_items_list = list(map(lambda x: (x, self.user_item_ratings.get(x, [])), user_ids))
         else:
             user_items_list = self.user_item_ratings.items()
 
         cf_func = self._rating_user_cf if cf_type == CFType.UCF else self._rating_item_cf
-        if len(user_items_list) > 4096:
+        if len(user_items_list) > PARALLEL_THRESHOLD:
             cf_result = self.processor.cf(self.user_item_ratings, user_items_list, similar_dict, recall_num, cf_func)
         else:
             cf_result = cf_func(self.user_item_ratings, similar_dict, user_items_list, recall_num)
         print_cost_time(f"完成{cf_type.value}推理, 当前进程<{os.getpid()}>, 生成{len(cf_result)}条记录, 总耗时", func_start_time)
         return cf_result
```

### Comparing `coll-filter-1.2.7/cf/utils.py` & `coll-filter-1.2.8/cf/utils.py`

 * *Files identical despite different names*

### Comparing `coll-filter-1.2.7/coll_filter.egg-info/PKG-INFO` & `coll-filter-1.2.8/coll_filter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coll-filter
-Version: 1.2.7
+Version: 1.2.8
 Summary: Collaborative Filtering with multi-process parallelism.
 Home-page: https://gitee.com/summry/myai
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: Collaborative Filtering,recommend
 Platform: UNKNOWN
```

### Comparing `coll-filter-1.2.7/setup.py` & `coll-filter-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='coll-filter',
     packages=['cf'],
     description="Collaborative Filtering with multi-process parallelism.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.7',
+    version='1.2.8',
     url='https://gitee.com/summry/myai',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['Collaborative Filtering', 'recommend'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

