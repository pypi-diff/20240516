# Comparing `tmp/solar_registry-0.2.7.tar.gz` & `tmp/solar_registry-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.2.7.tar", last modified: Wed May 15 07:08:54 2024, max compression
+gzip compressed data, was "solar_registry-0.2.8.tar", last modified: Wed May 15 07:31:32 2024, max compression
```

## Comparing `solar_registry-0.2.7.tar` & `solar_registry-0.2.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-05-15 07:08:31.581664 solar_registry-0.2.7/LICENSE
--rw-r--r--   0        0        0      682 2024-05-15 07:08:31.581664 solar_registry-0.2.7/README.md
--rw-r--r--   0        0        0     1240 2024-05-15 07:08:54.149713 solar_registry-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     2158 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     4959 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0     2120 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     3942 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/cos_sync.py
--rw-r--r--   0        0        0     2517 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2628 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      505 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     2068 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-15 07:08:31.581664 solar_registry-0.2.7/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0      364 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_cos_sync.py
--rw-r--r--   0        0        0      680 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_merger.py
--rw-r--r--   0        0        0      495 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_pr_generator.py
--rw-r--r--   0        0        0      928 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_testtool.py
--rw-r--r--   0        0        0      291 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/test_validator.py
--rw-r--r--   0        0        0      731 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/testdata/error_meta_file/pytest/testtool.yaml
--rw-r--r--   0        0        0      736 2024-05-15 07:08:31.581664 solar_registry-0.2.7/tests/testdata/error_version_file/pytest/testtool.yaml
--rw-r--r--   0        0        0     2778 2024-05-15 07:08:31.585665 solar_registry-0.2.7/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-15 07:08:31.585665 solar_registry-0.2.7/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     2942 2024-05-15 07:08:31.585665 solar_registry-0.2.7/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 07:31:06.782474 solar_registry-0.2.8/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-15 07:31:06.782474 solar_registry-0.2.8/README.md
+-rw-r--r--   0        0        0     1240 2024-05-15 07:31:32.686683 solar_registry-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     4959 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     3993 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/cos_sync.py
+-rw-r--r--   0        0        0     2517 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2628 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      505 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     2068 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/__init__.py
+-rw-r--r--   0        0        0      364 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_cos_sync.py
+-rw-r--r--   0        0        0      680 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_merger.py
+-rw-r--r--   0        0        0      495 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_pr_generator.py
+-rw-r--r--   0        0        0      928 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_testtool.py
+-rw-r--r--   0        0        0      291 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_validator.py
+-rw-r--r--   0        0        0      731 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/error_meta_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0      736 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/error_version_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0     2778 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     2942 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.2.8/PKG-INFO
```

### Comparing `solar_registry-0.2.7/LICENSE` & `solar_registry-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/README.md` & `solar_registry-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/pyproject.toml` & `solar_registry-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.2.7"
+version = "0.2.8"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.2.7/src/solar_registry/cli.py` & `solar_registry-0.2.8/src/solar_registry/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     testtool = get_testtool(tool_name, working_dir)
     merger = MetaMerger(testtool)
     merger.merge_index_and_history(Path(output))
 
 
 @app.command()
 def pull_request(
-        tool_name: Annotated[str, typer.Argument(help="工具名称")],
-        working_dir: Annotated[Optional[str], typer.Argument(help="可选工作目录")] = None,
+    tool_name: Annotated[str, typer.Argument(help="工具名称")],
+    working_dir: Annotated[Optional[str], typer.Argument(help="可选工作目录")] = None,
 ) -> None:
     """
     合并元数据之后，向项目提PR进行合并操作
     """
     testtool = get_testtool(tool_name, working_dir)
     pr_gen = PullRequestGenerator(testtool)
     pr_gen.merge_and_create_pull_request()
```

### Comparing `solar_registry-0.2.7/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.2.8/src/solar_registry/commands/meta_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/src/solar_registry/model/test_tool.py` & `solar_registry-0.2.8/src/solar_registry/model/test_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     name: str
     value: str
     default: str
     choices: list[ParamChoice] | None = None
 
 
 class TestTool(BaseModel):
-
     __test__ = False
 
     """
     测试工具模型定义
     """
 
     schema_version: float = Field(alias="schemaVersion")
@@ -56,15 +55,14 @@
 
 class ArchType(str, Enum):
     Amd64 = "amd64"
     Arm64 = "arm64"
 
 
 class TestToolTarget(BaseModel):
-
     __test__ = False
 
     """
     发布包模型定义
     """
 
     os: OsType
@@ -79,15 +77,14 @@
     """
 
     meta_version: str = Field("1", alias="metaVersion")
     tools: list[TestTool]
 
 
 class TestToolMetadata(BaseModel):
-
     __test__ = False
 
     """
     通过solar-registry生成的最新版本发布元数据
 
     包含元数据信息和target信息
     """
```

### Comparing `solar_registry-0.2.7/src/solar_registry/service/cos_sync.py` & `solar_registry-0.2.8/src/solar_registry/service/cos_sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,43 +50,45 @@
                 output_path = Path(temp) / relative_file
                 output_path.parent.mkdir(parents=True, exist_ok=True)
 
                 logger.info(f"Download {relative_file} to {output_path}...")
                 self.cos_client.download_file(
                     Bucket=self.cos_bucket,
                     Key=relative_file,
-                    DestFilePath=str(output_path)
+                    DestFilePath=str(output_path),
                 )
 
                 logger.info("Compare MD5...")
                 if calculate_md5(full_path) == calculate_md5(output_path):
                     logger.info(
-                        f"relative_file {relative_file} not changed, skip upload"
+                        f"✨ relative_file {relative_file} not changed, skip upload"
                     )
                 else:
                     response = self.cos_client.upload_file(
                         Bucket=self.cos_bucket,
                         Key=relative_file,
                         LocalFilePath=str(full_path),
                         EnableMD5=True,
-                        ACL='public-read',  # 必须设置为公有读取
+                        ACL="public-read",  # 必须设置为公有读取
                         progress_callback=None,
                     )
                     logger.info(
-                        f"relative_file {relative_file} uploaded, ETag: {response['ETag']}"
+                        f"✅ relative_file {relative_file} uploaded, ETag: {response['ETag']}"
                     )
 
         else:
             logger.info(f"File {relative_file} does not exist on cos, start upload...")
             # 文件不存在直接上传
             with open(Path(self.workdir, relative_file), "rb") as fp:
                 response = self.cos_client.put_object(
                     Bucket=self.cos_bucket, Key=relative_file, Body=fp
                 )
-                logger.info(f'File {relative_file} uploaded, ETag: {response["ETag"]}!')
+                logger.info(
+                    f'✅ File {relative_file} uploaded, ETag: {response["ETag"]}!'
+                )
 
 
 def calculate_md5(file_path: Path) -> str:
     """
     计算文件的 MD5 码。
 
     Args:
```

### Comparing `solar_registry-0.2.7/src/solar_registry/service/generator.py` & `solar_registry-0.2.8/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/src/solar_registry/service/pr_generator.py` & `solar_registry-0.2.8/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/src/solar_registry/service/validator.py` & `solar_registry-0.2.8/src/solar_registry/service/validator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/src/solar_registry/util/file.py` & `solar_registry-0.2.8/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/tests/test_merger.py` & `solar_registry-0.2.8/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/tests/test_testtool.py` & `solar_registry-0.2.8/tests/test_testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/tests/testdata/error_meta_file/pytest/testtool.yaml` & `solar_registry-0.2.8/tests/testdata/error_meta_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/tests/testdata/error_version_file/pytest/testtool.yaml` & `solar_registry-0.2.8/tests/testdata/error_version_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.2.8/tests/testdata/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.2.8/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.2.8/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.7/PKG-INFO` & `solar_registry-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.2.7
+Version: 0.2.8
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

