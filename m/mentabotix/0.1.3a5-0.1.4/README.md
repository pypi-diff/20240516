# Comparing `tmp/mentabotix-0.1.3a5.tar.gz` & `tmp/mentabotix-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.3a5.tar", last modified: Tue May 14 11:03:26 2024, max compression
+gzip compressed data, was "mentabotix-0.1.4.tar", last modified: Thu May 16 06:04:50 2024, max compression
```

## Comparing `mentabotix-0.1.3a5.tar` & `mentabotix-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1066 2024-05-14 11:03:00.168787 mentabotix-0.1.3a5/LICENSE
--rw-r--r--   0        0        0    23777 2024-05-14 11:03:00.168787 mentabotix-0.1.3a5/README.md
--rw-r--r--   0        0        0      678 2024-05-14 11:03:26.613098 mentabotix-0.1.3a5/pyproject.toml
--rw-r--r--   0        0        0     1158 2024-05-14 11:03:00.168787 mentabotix-0.1.3a5/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    68552 2024-05-14 11:03:00.168787 mentabotix-0.1.3a5/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-14 11:03:00.168787 mentabotix-0.1.3a5/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-14 11:03:00.168787 mentabotix-0.1.3a5/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    19965 2024-05-14 11:03:00.168787 mentabotix-0.1.3a5/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     7841 2024-05-14 11:03:00.172787 mentabotix-0.1.3a5/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-14 11:03:00.172787 mentabotix-0.1.3a5/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     9429 2024-05-14 11:03:00.172787 mentabotix-0.1.3a5/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-14 11:03:00.172787 mentabotix-0.1.3a5/tests/__init__.py
--rw-r--r--   0        0        0    15471 2024-05-14 11:03:00.172787 mentabotix-0.1.3a5/tests/test_botix.py
--rw-r--r--   0        0        0     8534 2024-05-14 11:03:00.172787 mentabotix-0.1.3a5/tests/test_composer.py
--rw-r--r--   0        0        0     8042 2024-05-14 11:03:00.172787 mentabotix-0.1.3a5/tests/test_menta.py
--rw-r--r--   0        0        0     6488 2024-05-14 11:03:00.172787 mentabotix-0.1.3a5/tests/test_moving_state.py
--rw-r--r--   0        0        0     5578 2024-05-14 11:03:00.172787 mentabotix-0.1.3a5/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24211 1970-01-01 00:00:00.000000 mentabotix-0.1.3a5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-16 06:04:25.185276 mentabotix-0.1.4/LICENSE
+-rw-r--r--   0        0        0    23781 2024-05-16 06:04:25.185276 mentabotix-0.1.4/README.md
+-rw-r--r--   0        0        0      678 2024-05-16 06:04:50.953431 mentabotix-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1158 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    68552 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    20144 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     7841 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     9429 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-16 06:04:25.185276 mentabotix-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0    15471 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_botix.py
+-rw-r--r--   0        0        0     8534 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_menta.py
+-rw-r--r--   0        0        0     6488 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5578 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24215 1970-01-01 00:00:00.000000 mentabotix-0.1.4/PKG-INFO
```

### Comparing `mentabotix-0.1.3a5/LICENSE` & `mentabotix-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/README.md` & `mentabotix-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -168,16 +168,16 @@
 
 # Extra context for the judge function, here only contains the "baseline"
 extra_context = {"baseline": 47}
 
 from typing import Callable
 
 # Construct the judge function object
-updater_function: Callable[[], bool] = menta_instance.construct_judge_function(usages, judging_source=judging_source,
-                                                                               extra_context=extra_context)
+updater_function: Callable[[], bool] = menta_instance.construct_inlined_function(usages, judging_source=judging_source,
+                                                                                 extra_context=extra_context)
 
 # Use the judge function to update the system
 updater_function()
 
 
 # Below is the equivalent implementation of the judge function, but is defined manually. 
 # It acts exactly the same as the `updater_function` above.
```

### Comparing `mentabotix-0.1.3a5/pyproject.toml` & `mentabotix-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "mentabotix"
-version = "0.1.3a5"
+version = "0.1.4"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
     "pyapriltags>=3.3.0.3",
     "terminaltables>=3.1.10",
-    "bdmc>=0.1.5",
+    "bdmc>=0.1.5.6",
     "opencv-python-headless>=4.9.0.80",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `mentabotix-0.1.3a5/src/mentabotix/__init__.py` & `mentabotix-0.1.4/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/src/mentabotix/modules/botix.py` & `mentabotix-0.1.4/src/mentabotix/modules/botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/src/mentabotix/modules/logger.py` & `mentabotix-0.1.4/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/src/mentabotix/modules/menta.py` & `mentabotix-0.1.4/src/mentabotix/modules/menta.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,30 +146,34 @@
             return update_funcs[0]
         eval_kwargs = {f"func_{i}": update_funcs[i] for i in range(len(update_funcs))}
         func_call_strings = [f"{func}()" for func in eval_kwargs]
         eval_string = "lambda:" + "(" + f",".join(func_call_strings) + ")"
         eval_obj = eval(eval_string, eval_kwargs)
         return eval_obj
 
-    def construct_judge_function(
+    def construct_inlined_function(
         self,
         usages: List[SamplerUsage],
         judging_source: List[SourceCode] | SourceCode,
         extra_context: Dict[str, Any] = None,
-    ) -> Callable[[], bool]:
+        return_raw: bool = False,
+    ) -> Callable[[], Any] | Tuple[str, Dict[str, Any]]:
         """
         构造一个判断函数。该函数根据提供的采样器使用情况、判断源和额外的上下文信息，动态生成一个判断逻辑的函数。
 
         参数:
         - usages: 一个SamplerUsage对象的列表，描述了每个采样器是如何被使用的。
         - judging_source: 判断源，可以是字符串或字符串列表。定义了判断逻辑的代码。
         - extra_context: 可选的字典，提供了额外的上下文信息，这些信息在执行判断函数时会包含在执行环境中。
 
         返回值:
-        - 一个无参数的布尔型函数，执行时根据判断逻辑返回True或False。
+        - 一个无参数的布尔型函数，执行时根据判断逻辑返回Any类型的结果。
+
+        Args:
+            return_raw:
         """
 
         # 将judging_source统一处理为字符串格式
         judging_source: str = judging_source if isinstance(judging_source, str) else "\n ".join(judging_source)
 
         # 定义返回标识符，检查判断源中是否包含该标识符
         RET_IDENTIFIER: str = "ret"
@@ -232,15 +236,18 @@
 
         # 构建完整的函数源码并编译执行
         func_source = f"def _func():\n" f" {temp_var_source}\n" f" {judging_source}\n" f" return {RET_IDENTIFIER}"
         _logger.debug(f"Created func_source: {func_source}")
         _logger.debug("Compiling func_source")
 
         # 更新执行环境中的采样器和额外上下文信息
+
         used_samplers.update(extra_context) if extra_context else None
+        if return_raw:
+            return func_source, used_samplers
         exec(func_source, used_samplers)  # exec the source with the context
         func_obj: Callable[[], bool] = used_samplers.get("_func")
         _logger.debug(f"Succeed, compiled func_obj: {func_obj}")
         return func_obj
 
     @staticmethod
     def _index_for_seq_sampler_data(data_var_name: str, required: List[int] | int) -> List[str]:
```

### Comparing `mentabotix-0.1.3a5/src/mentabotix/tools/composers.py` & `mentabotix-0.1.4/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/src/mentabotix/tools/generators.py` & `mentabotix-0.1.4/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.4/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/tests/test_botix.py` & `mentabotix-0.1.4/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/tests/test_composer.py` & `mentabotix-0.1.4/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/tests/test_menta.py` & `mentabotix-0.1.4/tests/test_menta.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,33 +115,35 @@
     def test_construct_judge(self):
         # Test with multiple usages
         sages = [
             SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
             SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
             SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2]),
         ]
-        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0 or s1 or s2 or s3 or s4 or s5")
+        func = self.menta.construct_inlined_function(
+            usages=sages, judging_source="ret=s0 or s1 or s2 or s3 or s4 or s5"
+        )
         self.assertIsInstance(func, Callable)
         self.assertEqual(func(), 1.2)
-        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0+s1+s2+s3+s4+s5")
+        func = self.menta.construct_inlined_function(usages=sages, judging_source="ret=s0+s1+s2+s3+s4+s5")
         self.assertIsInstance(func, Callable)
         self.assertEqual(func(), 53.5)
 
         # Test with 1 usage
-        func = self.menta.construct_judge_function(
+        func = self.menta.construct_inlined_function(
             usages=[
                 SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
             ],
             judging_source="ret=s0 + s1",
         )
         self.assertIsInstance(func, Callable)
         self.assertEqual(func(), 2.5)
 
         # Test with  multiline judging source
-        func = self.menta.construct_judge_function(
+        func = self.menta.construct_inlined_function(
             usages=sages,
             judging_source=["a=s0+s1", "print(f'this is {a}')", "b=s3+s4+s5", "print(f'this is {b}')", "ret=s2"],
         )
         self.assertIsInstance(func, Callable)
         self.assertEqual(func(), 50)
 
     def test_indexer_seq(self):
@@ -173,15 +175,15 @@
 
     def test_constructed_judge_function_performance(self):
         sages = [
             SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
             SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
             SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2]),
         ]
-        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0+s1+s2+s3+s4+s5")
+        func = self.menta.construct_inlined_function(usages=sages, judging_source="ret=s0+s1+s2+s3+s4+s5")
 
         def _manual_seq_func():
             seq_temp = mock_sequence_sampler()
 
             return seq_temp[0], seq_temp[2]
 
         def _manual_drc_func():
@@ -192,14 +194,15 @@
             return *_manual_seq_func(), mock_indexed_sampler(5), *_manual_drc_func()
 
         def _manual_judge_func():
             return sum(_manual_asm_func())
 
         self.assertEqual(func(), _manual_judge_func())
 
+        print(_manual_drc_func())
         import timeit
 
         # 假设这两个函数已经在你的代码中定义好了
 
         # 设置测试次数（例如：1000次）
         number_of_runs = 1000
 
@@ -211,14 +214,38 @@
         # 对_manual_judge_func()进行计时测试
         manual_judge_func_time = timeit.timeit(lambda: _manual_judge_func(), number=number_of_runs)
 
         print(f"_manual_judge_func() execution time for {number_of_runs} runs: {manual_judge_func_time:.6f} seconds")
 
         print(f"func() is {manual_judge_func_time / func_time:.2f} times faster than _manual_judge_func()")
 
+    def test_construct_ret_raw(self):
+        sages = [
+            SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+            SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
+            SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2]),
+        ]
+        func, _ = self.menta.construct_inlined_function(
+            usages=sages, judging_source="ret=s0,s1,s2,s3,s4+s5", return_raw=True
+        )
+
+        self.assertEqual(
+            func,
+            """def _func():
+ func_0_temp,func_2_temp=func_0(),func_2()
+ ret=func_0_temp[0],func_0_temp[2],func_1(5),((func_2_temp>>0)&1),((func_2_temp>>1)&1)+((func_2_temp>>2)&1)
+ return ret""",
+        )
+
+        print(func)
+        func = self.menta.construct_inlined_function(
+            usages=sages, judging_source="ret=s0,s1,s2,s3,s4+s5", return_raw=False
+        )
+        print(func())
+
     def tearDown(self):
         # 清理可能的副作用
         pass
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.3a5/tests/test_moving_state.py` & `mentabotix-0.1.4/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/tests/test_moving_transition.py` & `mentabotix-0.1.4/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.3a5/PKG-INFO` & `mentabotix-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.3a5
+Version: 0.1.4
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pyapriltags>=3.3.0.3
 Requires-Dist: terminaltables>=3.1.10
-Requires-Dist: bdmc>=0.1.5
+Requires-Dist: bdmc>=0.1.5.6
 Requires-Dist: opencv-python-headless>=4.9.0.80
 Description-Content-Type: text/markdown
 
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
@@ -183,16 +183,16 @@
 
 # Extra context for the judge function, here only contains the "baseline"
 extra_context = {"baseline": 47}
 
 from typing import Callable
 
 # Construct the judge function object
-updater_function: Callable[[], bool] = menta_instance.construct_judge_function(usages, judging_source=judging_source,
-                                                                               extra_context=extra_context)
+updater_function: Callable[[], bool] = menta_instance.construct_inlined_function(usages, judging_source=judging_source,
+                                                                                 extra_context=extra_context)
 
 # Use the judge function to update the system
 updater_function()
 
 
 # Below is the equivalent implementation of the judge function, but is defined manually. 
 # It acts exactly the same as the `updater_function` above.
```

