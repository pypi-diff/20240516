# Comparing `tmp/gentccode-0.2.8.tar.gz` & `tmp/gentccode-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentccode-0.2.8.tar", max compression
+gzip compressed data, was "gentccode-0.2.9.tar", max compression
```

## Comparing `gentccode-0.2.8.tar` & `gentccode-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.8/LICENSE
--rw-r--r--   0        0        0     1084 2024-04-10 07:58:28.662833 gentccode-0.2.8/README.md
--rw-r--r--   0        0        0      667 2024-04-15 09:00:43.272875 gentccode-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.8/src/gentccode/__init__.py
--rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.8/src/gentccode/cartesian_for_case.py
--rw-r--r--   0        0        0     1198 2024-04-15 09:00:57.371895 gentccode-0.2.8/src/gentccode/check_version.py
--rw-r--r--   0        0        0     3348 2024-04-10 07:48:10.190075 gentccode-0.2.8/src/gentccode/cli.py
--rw-r--r--   0        0        0    21552 2024-04-10 07:57:26.821826 gentccode-0.2.8/src/gentccode/convert_to_jmx.py
--rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.8/src/gentccode/convert_to_locust.py
--rw-r--r--   0        0        0    13594 2024-04-15 08:54:35.123701 gentccode-0.2.8/src/gentccode/generate_case_code.py
--rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.8/src/gentccode/merge_api.py
--rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.8/src/gentccode/produce_search_case.py
--rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.8/src/gentccode/produce_test_case.py
--rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.8/src/gentccode/read_swagger_rule.py
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 gentccode-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1354 2024-04-19 02:27:18.948883 gentccode-0.2.9/README.md
+-rw-r--r--   0        0        0      667 2024-04-19 02:27:46.148232 gentccode-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.9/src/gentccode/__init__.py
+-rw-r--r--   0        0        0     1462 2024-04-18 04:15:09.513036 gentccode-0.2.9/src/gentccode/cartesian.py
+-rw-r--r--   0        0        0     1198 2024-04-15 09:00:57.371895 gentccode-0.2.9/src/gentccode/check_version.py
+-rw-r--r--   0        0        0     3468 2024-04-18 11:10:18.802801 gentccode-0.2.9/src/gentccode/cli.py
+-rw-r--r--   0        0        0    20937 2024-04-18 11:11:45.814211 gentccode-0.2.9/src/gentccode/convert_to_jmx.py
+-rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.9/src/gentccode/convert_to_locust.py
+-rw-r--r--   0        0        0     3845 2024-04-18 11:04:50.937592 gentccode-0.2.9/src/gentccode/filter_cp_result.py
+-rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.9/src/gentccode/merge_api.py
+-rw-r--r--   0        0        0    14275 2024-04-19 01:59:01.444756 gentccode-0.2.9/src/gentccode/produce_case_code.py
+-rw-r--r--   0        0        0     8683 2024-04-19 02:11:21.299978 gentccode-0.2.9/src/gentccode/produce_use_case.py
+-rw-r--r--   0        0        0      532 2024-04-18 11:11:02.804660 gentccode-0.2.9/src/gentccode/read_swagger_rule.py
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 gentccode-0.2.9/PKG-INFO
```

### Comparing `gentccode-0.2.8/LICENSE` & `gentccode-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.8/pyproject.toml` & `gentccode-0.2.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gentccode"
-version = "0.2.8"
+version = "0.2.9"
 description = "generate test case code"
 authors = ["Lei Su <lei.susl@shopee.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `gentccode-0.2.8/src/gentccode/cartesian_for_case.py` & `gentccode-0.2.9/src/gentccode/cartesian.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 
 
 class CP:
     def __init__(self) -> None:
         self.cartesian_product = []
         self.unique_list = []
 
-    def product_param(self, param):
+    def product_cp_params(self, param) -> list:
         param_copy = copy.deepcopy(param)
         if isinstance(param_copy, list):
             self._product_for_param_list(param_copy)
         elif isinstance(param_copy, dict):
             self._product_for_param_dict(param_copy)
         else:
-            print(f"param type ({type(param_copy)}) is not support")
+            print(f"param type ({type(param)}) is not support")
+        self._remove_duplicate()
+        return self.unique_list
 
     ###
     # param like: [{'a':1},{'b':2},{'c':3}]
     ###
     def _product_for_param_list(self, param_list: list):
         param_len = len(param_list)
         for i in range(param_len):
@@ -41,14 +43,10 @@
         self._product_for_param_list(param_list)
 
     def _remove_duplicate(self):
         for cp in self.cartesian_product:
             if cp not in self.unique_list:
                 self.unique_list.append(cp)
 
-    def get_unique_list(self):
-        self._remove_duplicate()
-        return self.unique_list
-
 
 if __name__ == "__main__":
     pass
```

### Comparing `gentccode-0.2.8/src/gentccode/check_version.py` & `gentccode-0.2.9/src/gentccode/check_version.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.8/src/gentccode/cli.py` & `gentccode-0.2.9/src/gentccode/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 import os
 import click
 from gentccode.check_version import check_package_version, get_current_version
 from gentccode.convert_to_jmx import convert_payloads_of_curl_to_jmx_file
 from gentccode.convert_to_locust import product_locust_code
-from gentccode.produce_search_case import gen_cp_test_case
-from gentccode.produce_test_case import ProduceTestCase
+from gentccode.produce_use_case import ProduceUseCase
 
 
-ptc = ProduceTestCase()
+ptc = ProduceUseCase()
 # 生成的接口信息会保存到这个文件中
-api_yaml_file_path = "api.yaml"
+API_YAML_FILE_PATH = "api.yaml"
 # 生成的接口代码会保存到这个文件中
-case_file_path = "test_cases.py"
+CASE_FILE_PATH = "test_cases.py"
 
-package_name = "gentccode"
+PACKAGE_NAME = "gentccode"
 
 
 @click.group()
 def cli1():
     pass
 
 
 # cli1的回调函数
 @cli1.result_callback()
 def check_update(curl):
-    check_package_version(package_name)
+    check_package_version(PACKAGE_NAME)
 
 
 @click.command(help="generate test code by http's payload")
-@click.option("-n", "--node", required=True, help="json node, like: '.','a.','a.b.'")
+@click.option("-n", "--node", required=True, help="json node, like: '.','a.'")
+@click.option("-p", "--paramtype", required=True, help="query,body")
 @click.argument("filename", type=click.Path(exists=True))
-def cp(node, filename):
-    gen_cp_test_case(
+def cp(node, filename, paramtype):
+    ptc.produce_cp_case(
         node=node,
-        curl_file=filename,
+        param_type=paramtype,
+        source_type="curl",
+        curl_file_path=filename,
+        use_case_file_path=CASE_FILE_PATH,
     )
 
 
 @click.command(help="generate test code by curl file")
 @click.argument("filename", type=click.Path(exists=True))
 def curl(filename):
-    ptc.produce_case_by_yaml_for_curl(filename, api_yaml_file_path, case_file_path)
+    ptc.produce_case_by_yaml_for_curl(filename, API_YAML_FILE_PATH, CASE_FILE_PATH)
 
 
 @click.command(help="generate test code by swagger json file")
 @click.argument("filename", type=click.Path(exists=True))
 def swagger2(filename):
-    ptc.produce_case_by_yaml_for_swagger2(filename, api_yaml_file_path, case_file_path)
+    ptc.produce_case_by_yaml_for_swagger2(filename, API_YAML_FILE_PATH, CASE_FILE_PATH)
 
 
 @click.command(help="auto generate openapi document's test code")
 @click.argument("filename", type=click.Path(exists=True))
 def openapi(filename):
     ptc.produce_merged_case_for_openapi_and_curl(curl_file_path=filename)
 
@@ -91,22 +94,22 @@
 @click.argument("filename", type=click.Path(exists=True))
 def swagger_at(filename):
     ptc.produce_merged_case_for_swagger_and_curl(curl_file_path=filename)
 
 
 @click.command()
 def version():
-    current_version = get_current_version(package_name=package_name)
-    click.echo(f"{package_name}: v{current_version}")
+    current_version = get_current_version(package_name=PACKAGE_NAME)
+    click.echo(f"{PACKAGE_NAME}: v{current_version}")
 
 
 def main():
     # clear api yaml content.
-    if os.path.exists(api_yaml_file_path):
-        with open(api_yaml_file_path, "w") as f:
+    if os.path.exists(API_YAML_FILE_PATH):
+        with open(API_YAML_FILE_PATH, "w") as f:
             f.write("")
     cli1.add_command(curl)
     cli1.add_command(swagger2)
     cli1.add_command(openapi)
     cli1.add_command(locust)
     cli1.add_command(cp)
     cli1.add_command(jmeter)
```

### Comparing `gentccode-0.2.8/src/gentccode/convert_to_jmx.py` & `gentccode-0.2.9/src/gentccode/convert_to_jmx.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,27 +567,7 @@
     if isinstance(req.header, str):
         req.header = json.loads(req.header)
     if isinstance(req.body, str):
         req.body = json.loads(req.body)
     if isinstance(req.query_param, str):
         req.query_param = json.loads(req.query_param)
     return req
-
-
-if __name__ == "__main__":
-    p1 = {
-        "host": "www.baidu.com",
-        "port": "443",
-        "path": "/api/v3",
-        "method": "post",
-        "header": '{"h1":2}',
-        "params": "",
-        "http_type": "https",
-        "params_type": "parameters",
-        "sampler_comments": "test-comments",
-        "controller_name": "test-controller",
-    }
-    yaml_file_path = "./script/generated_result/api_template.yaml"
-    curl_file = "/Users/lei.susl/Desktop/test1/risk-control/iac.txt"
-    convert_payloads_of_curl_to_jmx_file(
-        curl_file_path=curl_file, json_path_assert="success=true"
-    )
```

### Comparing `gentccode-0.2.8/src/gentccode/convert_to_locust.py` & `gentccode-0.2.9/src/gentccode/convert_to_locust.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.8/src/gentccode/generate_case_code.py` & `gentccode-0.2.9/src/gentccode/produce_case_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import yaml
 import json
 from gentccode.read_swagger_rule import BaseRule, NoneRule
 from http_content_parser.param_util import ParamUtil
 from http_content_parser.req_data import ReqData
 
 
-class GenerateCaseCode(object):
+class ProduceCaseCode(object):
     def __init__(self) -> None:
         self.CHAR_SPACE_8 = "        "
         self.CHAR_SPACE_4 = "    "
 
     def produce_code_for_api_yaml(
         self,
         yaml_file_path,
@@ -59,14 +59,15 @@
                 # TODO 后缀只支持接从0递增的数字,后续考虑支持任意字符
                 if unique_char:
                     s = "_" + str(n)
                     cases = self.edit_method_content(
                         req_data,
                         has_payload_assgin=True,
                         has_response_assert=True,
+                        edit_query_param=True,
                         split_respone_assert=split_respone_assert,
                         reset_header=True,
                         unique_char=s,
                         **kwargs,
                     )
                     n += 1
                 else:
@@ -92,14 +93,15 @@
         edit_payload_str_middle = ""
         assert_response_str = ""
         send_request_str = ""
         edit_header_str = ""
         preset_data_str = ""
         method_name_suffix = ""
         assert_response_str_after = ""
+        query_param_str = ""
         for k, v in kwargs.items():
             if k == "add_mysql_method":
                 preset_data_str += space_8 + f"self.toc_sql.{v}()\n"
             elif k == "edit_payload_str_before":
                 edit_payload_str_before += f"{space_8}{v}\n"
             elif k == "unique_char":
                 method_name_suffix += v
@@ -130,19 +132,28 @@
                         f'{space_8}assert response.get("error", -99) == 0\n'
                     )
             elif k == "reset_header":
                 if v:
                     edit_header_str += space_8 + "request_model.header = {}\n"
             elif k == "assert_response_str_after":
                 assert_response_str_after += f"{space_8}{v}\n"
+            elif k == "edit_query_param":
+                if v:
+                    kv_fix_list = ["request_model.query_param", "", "", ""]
+                    query_param_str += self.get_payload_with_assigin_value_str(
+                        param_dict=req_data.query_param,
+                        kv_fix_list=kv_fix_list,
+                        middle_char="=",
+                    )
 
         edit_payload_str = edit_payload_str_before + edit_payload_str_middle
         assert_response_str += assert_response_str_after
         return self.get_method_content_str(
             req_data=req_data,
+            edit_query_param=query_param_str,
             method_name_suffix=method_name_suffix,
             preset_data_str=preset_data_str,
             edit_header_str=edit_header_str,
             send_request_str=send_request_str,
             assert_response_str=assert_response_str,
             edit_payload_str=edit_payload_str,
         )
@@ -165,24 +176,28 @@
                 assert_response = arg_value
             elif arg_name == "preset_data_str":
                 preset_data = arg_value
             elif arg_name == "send_request_str":
                 send_request = arg_value
             elif arg_name == "edit_payload_str":
                 edit_payload = arg_value
+            elif arg_name == "edit_query_param":
+                query_param_str = arg_value
             else:
                 print(f"arg: {arg_name} is invalid")
 
         method_str = (
             f"{space_4}@allure.title('{req_data.method}: {req_data.path}{method_name_suffix}')\n"
             + f"{space_4}def test_case_{req_data.temp_api_label.replace('-', '_').replace('{','').replace('}','')}{method_name_suffix}(self):\n"
             + f"{space_8}# 读取yaml中所有api数据,转换为dict\n"
             + f"{space_8}api_info_in_yaml = ParseUtil.parse_api_info_from_yaml(self.api_yaml_path)\n"
             + f"{space_8}# 获取指定api信息\n"
             + f"{space_8}request_model = api_info_in_yaml['{req_data.temp_api_label}']\n"
+            + f"{space_8}# 编辑query_param\n"
+            + query_param_str
             + f"{space_8}# 编辑header\n"
             + edit_header
             + f"{space_8}request_model.header.update(self.header_auth)\n"
             + f"{space_8}# 编辑payload\n"
             + edit_payload
             + f"{space_8}# 预置数据\n"
             + preset_data
```

### Comparing `gentccode-0.2.8/src/gentccode/merge_api.py` & `gentccode-0.2.9/src/gentccode/merge_api.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.8/PKG-INFO` & `gentccode-0.2.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentccode
-Version: 0.2.8
+Version: 0.2.9
 Summary: generate test case code
 Author: Lei Su
 Author-email: lei.susl@shopee.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -15,57 +15,64 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: http-content-parser (>=0.0.17,<0.0.18)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
-## 简介
+# 简介
 
 gtc(generate test case) 是一个把http请求转换为测试代码的cli工具
 
 ## 功能
 
 - [x] 支持解析curl命令
 - [x] 支持解析postman文件
 - [x] 支持解析swagger2文件
+- [x] 支持解析openapi文件
 - [x] 支持生成笛卡尔积测试脚本
 - [x] 支持解析curl文件并生成Jmeter性能脚本
 - [x] 支持解析curl文件并生成Locust性能脚本
-- [ ] 支持解析postman文件并生成Jmeter性能脚本
 - [ ] 一键生成Jmeter性能压测方案脚本
 
 ## 安装
 
 ```bash
 pip3 install gentccode
 gtc version
 ```
 
 ## 使用
 
 1. 执行下面命令,会在当前目录生成api文件(`api.yaml`)和测试代码的脚本文件(`test_case.py`)
 
-```bash
-gtc curl curl.txt
-gtc postman postman.json
-gtc swagger2 swagger.json
-```
-
-2. 根据参数生成笛卡尔积的用例脚本
-
-```bash
-gtc cp -n a. curl.txt
-```
+    ```bash
+    gtc curl curl.txt
+    gtc postman postman.json
+    gtc swagger2 swagger.json
+    ```
+
+2. 根据笛卡尔积算法生成用例脚本
+
+    ```bash
+    # 对请求中的body进行操作
+    gtc cp -n . -p body curl.txt
+    gtc cp -n filter. -p body curl.txt
+
+    # 对请求中的query param进行操作
+    gtc cp -n . -p query curl.txt
+    ```
 
 3. 执行下面命令,会生成对应的压测脚本
 
-```bash
-gtc jmeter curl.txt --jsonassert code=0 --rate 10 --time 5
-gtc locust curl.txt
-```
+    ```bash
+    # jsonassert 是对response的断言, rate 是tps, time 是 5min
+    gtc jmeter curl.txt --jsonassert code=0 --rate 10 --time 5
+    # locust脚本 
+    gtc locust curl.txt
+    ```
 
 ## 已知问题
 
 - 若postman文件中有变量,则不会生成相对应的代码块.
 - url中必须有http或https协议头
```

