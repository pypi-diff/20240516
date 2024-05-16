# Comparing `tmp/qtmodel-0.3.1.tar.gz` & `tmp/qtmodel-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.3.1.tar", last modified: Wed May 15 05:49:13 2024, max compression
+gzip compressed data, was "qtmodel-0.3.2.tar", last modified: Wed May 15 09:06:05 2024, max compression
```

## Comparing `qtmodel-0.3.1.tar` & `qtmodel-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 05:49:13.271619 qtmodel-0.3.1/
--rw-rw-rw-   0        0        0    37701 2024-05-15 05:49:13.270553 qtmodel-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 05:49:13.248896 qtmodel-0.3.1/qtmodel/
--rw-rw-rw-   0        0        0       93 2024-05-15 02:13:58.000000 qtmodel-0.3.1/qtmodel/__init__.py
--rw-rw-rw-   0        0        0    82085 2024-05-15 02:46:03.000000 qtmodel-0.3.1/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     3834 2024-05-15 02:13:47.000000 qtmodel-0.3.1/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.3.1/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-05-15 05:49:13.268158 qtmodel-0.3.1/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    37701 2024-05-15 05:49:12.000000 qtmodel-0.3.1/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-15 05:49:13.000000 qtmodel-0.3.1/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 05:49:12.000000 qtmodel-0.3.1/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 05:49:12.000000 qtmodel-0.3.1/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 05:49:13.271619 qtmodel-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-15 05:49:09.000000 qtmodel-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:05.482772 qtmodel-0.3.2/
+-rw-rw-rw-   0        0        0    37701 2024-05-15 09:06:05.481772 qtmodel-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:05.463049 qtmodel-0.3.2/qtmodel/
+-rw-rw-rw-   0        0        0       93 2024-05-15 02:13:58.000000 qtmodel-0.3.2/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0    82411 2024-05-15 09:02:31.000000 qtmodel-0.3.2/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     4574 2024-05-15 07:19:18.000000 qtmodel-0.3.2/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0     3884 2024-05-15 09:01:13.000000 qtmodel-0.3.2/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:05.479767 qtmodel-0.3.2/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    37701 2024-05-15 09:06:04.000000 qtmodel-0.3.2/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-05-15 09:06:05.000000 qtmodel-0.3.2/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:06:04.000000 qtmodel-0.3.2/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 09:06:05.000000 qtmodel-0.3.2/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:06:05.482772 qtmodel-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-15 09:05:44.000000 qtmodel-0.3.2/setup.py
```

### Comparing `qtmodel-0.3.1/PKG-INFO` & `qtmodel-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.1
+Version: 0.3.2
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.3.1/README.md` & `qtmodel-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.1/qtmodel/qt_mdb.py` & `qtmodel-0.3.2/qtmodel/qt_mdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,26 @@
             example:
                 qt_model.ExportFile("a.mct")
             Returns: 无
         """
         qt_model.ExportFile(file_path)
 
     @staticmethod
+    def import_file(file_path: str):
+        """
+            导入命令
+            Args:
+                file_path:导入文件(.mct/.qdat/.dxf/.3dx)
+            example:
+                qt_model.ImportFile("a.mct")
+            Returns: 无
+        """
+        qt_model.ImportFile(file_path)
+
+    @staticmethod
     def do_solve():
         """
             运行分析
             example:
                     mdb.do_solve()
             Returns: 无
         """
```

### Comparing `qtmodel-0.3.1/qtmodel/qt_odb.py` & `qtmodel-0.3.2/qtmodel/qt_odb.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     @staticmethod
     def __get_force_j(force_info):
         return [force_info.INodeForce.Fx, force_info.INodeForce.Fy, force_info.INodeForce.Fz,
                 force_info.INodeForce.Mx, force_info.INodeForce.My, force_info.INodeForce.Mz]
 
     @staticmethod
-    def get_beam_force(beam_id=1, stage_id=1, result_kind=1, increment_type=1):
+    def get_beam_force(beam_id, stage_id: int, result_kind: int = 1, increment_type: int = 1):
         """
         获取梁单元内力,支持单个节点和节点列表
         Args:
             beam_id: 梁单元号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
@@ -37,15 +37,15 @@
             bf_list = qt_model.GetBeamForce(beam_id, stage_id, result_kind, increment_type)
             list_res = []
             for item in bf_list:
                 list_res.append(FrameElementForce(item.ElementId, Odb.__get_force_i(item), Odb.__get_force_j(item)))
             return list_res
 
     @staticmethod
-    def get_cable_force(cable_id=1, stage_id=1, result_kind=1, increment_type=1):
+    def get_cable_force(cable_id, stage_id, result_kind=1, increment_type=1):
         """
         获取索单元内力,支持单个节点和节点列表
         Args:
             cable_id: 索单元号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type:  1-全量    2-增量
@@ -60,15 +60,15 @@
             bf_list = qt_model.GetCableForce(cable_id, stage_id, result_kind, increment_type)
             list_res = []
             for item in bf_list:
                 list_res.append(FrameElementForce(item.ElementId, Odb.__get_force_i(item), Odb.__get_force_j(item)))
             return list_res
 
     @staticmethod
-    def get_link_force(cable_id=1, stage_id=1, result_kind=1, increment_type=1):
+    def get_link_force(cable_id, stage_id: int, result_kind: int = 1, increment_type: int = 1):
         """
         获取桁架单元内力,支持单个节点和节点列表
         Args:
             cable_id: 桁架单元号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
@@ -81,7 +81,19 @@
             return FrameElementForce(cable_id, Odb.__get_force_i(bf_list[0]), Odb.__get_force_j(bf_list[0]))
         elif type(cable_id) == list:
             bf_list = qt_model.GetLinkForce(cable_id, stage_id, result_kind, increment_type)
             list_res = []
             for item in bf_list:
                 list_res.append(FrameElementForce(item.ElementId, Odb.__get_force_i(item), Odb.__get_force_j(item)))
             return list_res
+
+    @staticmethod
+    def get_node_displacement(node_id, stage_id: int, result_kind: int = 1, increment_type: int = 1):
+        if type(node_id) == int:
+            bf_list = qt_model.GetNodeDisplacement([node_id], stage_id, result_kind, increment_type)
+            return FrameElementForce(node_id, Odb.__get_force_i(bf_list[0]), Odb.__get_force_j(bf_list[0]))
+        elif type(node_id) == list:
+            bf_list = qt_model.GetNodeDisplacement(node_id, stage_id, result_kind, increment_type)
+            list_res = []
+            for item in bf_list:
+                list_res.append(FrameElementForce(item.ElementId, Odb.__get_force_i(item), Odb.__get_force_j(item)))
+            return list_res
```

### Comparing `qtmodel-0.3.1/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.3.2/qtmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.1
+Version: 0.3.2
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.3.1/setup.py` & `qtmodel-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.3.1",
+    version="0.3.2",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
     description="python modeling for qt  24/05/06 ",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
```

