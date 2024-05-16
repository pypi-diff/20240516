# Comparing `tmp/latex2pydata-0.1.0.tar.gz` & `tmp/latex2pydata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex2pydata-0.1.0.tar", last modified: Mon Nov 20 19:00:51 2023, max compression
+gzip compressed data, was "latex2pydata-0.2.0.tar", last modified: Thu May 16 20:48:45 2024, max compression
```

## Comparing `latex2pydata-0.1.0.tar` & `latex2pydata-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-11-20 19:00:51.282957 latex2pydata-0.1.0/
--rw-rw-rw-   0        0        0       62 2023-11-20 12:29:22.000000 latex2pydata-0.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1517 2023-11-20 03:50:05.000000 latex2pydata-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5709 2023-11-20 19:00:51.280957 latex2pydata-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2859 2023-11-20 18:52:37.000000 latex2pydata-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-11-20 19:00:51.263962 latex2pydata-0.1.0/latex2pydata/
--rw-rw-rw-   0        0        0      280 2023-11-20 15:01:28.000000 latex2pydata-0.1.0/latex2pydata/__init__.py
--rw-rw-rw-   0        0        0      459 2023-11-20 15:00:18.000000 latex2pydata-0.1.0/latex2pydata/err.py
--rw-rw-rw-   0        0        0     9062 2022-06-22 23:23:51.000000 latex2pydata-0.1.0/latex2pydata/fmtversion.py
--rw-rw-rw-   0        0        0     6251 2023-11-20 17:43:01.000000 latex2pydata-0.1.0/latex2pydata/loading.py
--rw-rw-rw-   0        0        0     3773 2023-11-20 18:55:40.000000 latex2pydata-0.1.0/latex2pydata/schema.py
--rw-rw-rw-   0        0        0      778 2023-11-20 15:08:44.000000 latex2pydata-0.1.0/latex2pydata/util.py
--rw-rw-rw-   0        0        0      150 2023-11-20 04:30:48.000000 latex2pydata-0.1.0/latex2pydata/version.py
-drwxrwxrwx   0        0        0        0 2023-11-20 19:00:51.279958 latex2pydata-0.1.0/latex2pydata.egg-info/
--rw-rw-rw-   0        0        0     5709 2023-11-20 19:00:51.000000 latex2pydata-0.1.0/latex2pydata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-11-20 19:00:51.000000 latex2pydata-0.1.0/latex2pydata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-20 19:00:51.000000 latex2pydata-0.1.0/latex2pydata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-20 19:00:51.000000 latex2pydata-0.1.0/latex2pydata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1332 2023-11-20 16:54:01.000000 latex2pydata-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-20 19:00:51.282957 latex2pydata-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-20 19:00:51.276959 latex2pydata-0.1.0/test/
--rw-rw-rw-   0        0        0     2799 2023-11-20 18:56:44.000000 latex2pydata-0.1.0/test/test_loads.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:48:45.292788 latex2pydata-0.2.0/
+-rw-rw-rw-   0        0        0      281 2024-05-16 20:41:28.000000 latex2pydata-0.2.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1517 2023-11-20 03:50:05.000000 latex2pydata-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5986 2024-05-16 20:48:45.289788 latex2pydata-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3117 2024-05-14 15:11:58.000000 latex2pydata-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 20:48:45.271794 latex2pydata-0.2.0/latex2pydata/
+-rw-rw-rw-   0        0        0      280 2023-11-20 15:01:28.000000 latex2pydata-0.2.0/latex2pydata/__init__.py
+-rw-rw-rw-   0        0        0      459 2023-11-20 15:00:18.000000 latex2pydata-0.2.0/latex2pydata/err.py
+-rw-rw-rw-   0        0        0     9062 2022-06-22 23:23:51.000000 latex2pydata-0.2.0/latex2pydata/fmtversion.py
+-rw-rw-rw-   0        0        0     6503 2024-05-14 14:26:23.000000 latex2pydata-0.2.0/latex2pydata/loading.py
+-rw-rw-rw-   0        0        0     3773 2023-11-20 18:55:40.000000 latex2pydata-0.2.0/latex2pydata/schema.py
+-rw-rw-rw-   0        0        0      778 2023-11-20 15:08:44.000000 latex2pydata-0.2.0/latex2pydata/util.py
+-rw-rw-rw-   0        0        0      150 2024-05-16 20:38:55.000000 latex2pydata-0.2.0/latex2pydata/version.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:48:45.288788 latex2pydata-0.2.0/latex2pydata.egg-info/
+-rw-rw-rw-   0        0        0     5986 2024-05-16 20:48:45.000000 latex2pydata-0.2.0/latex2pydata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-16 20:48:45.000000 latex2pydata-0.2.0/latex2pydata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 20:48:45.000000 latex2pydata-0.2.0/latex2pydata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 20:48:45.000000 latex2pydata-0.2.0/latex2pydata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1345 2024-05-11 15:16:50.000000 latex2pydata-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 20:48:45.292788 latex2pydata-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 20:48:45.286789 latex2pydata-0.2.0/test/
+-rw-rw-rw-   0        0        0     3428 2024-05-14 15:23:36.000000 latex2pydata-0.2.0/test/test_loads.py
```

### Comparing `latex2pydata-0.1.0/LICENSE.txt` & `latex2pydata-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `latex2pydata-0.1.0/PKG-INFO` & `latex2pydata-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex2pydata
-Version: 0.1.0
+Version: 0.2.0
 Summary: Load data from LaTeX in Python literal format
 Author-email: "Geoffrey M. Poore" <gpoore@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Geoffrey M. Poore
         All rights reserved.
         
@@ -29,17 +29,17 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: homepage, https://github.com/gpoore/latex2pydata_py
-Project-URL: repository, https://github.com/gpoore/latex2pydata_py
-Project-URL: changelog, https://github.com/gpoore/latex2pydata_py/blob/master/CHANGELOG.md
+Project-URL: homepage, https://github.com/gpoore/latex2pydata/tree/main/python
+Project-URL: repository, https://github.com/gpoore/latex2pydata
+Project-URL: changelog, https://github.com/gpoore/latex2pydata/blob/main/python/CHANGELOG.md
 Keywords: deserialization,LaTeX,Python literal format
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -52,15 +52,15 @@
 License-File: CHANGELOG.md
 
 # latex2pydata - load data from LaTeX in Python literal format
 
 The latex2pydata Python package is designed to load data in
 [Python literal format](https://docs.python.org/3/reference/lexical_analysis.html#literals)
 that was saved to file by the
-[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata_tex).
+[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata/tree/main/latex).
 This allows data to be passed from [LaTeX](https://www.latex-project.org/) to
 Python.
 
 Raw data is loaded with
 [`ast.literal_eval()`](https://docs.python.org/3/library/ast.html#ast.literal_eval).  This always yields either `dict[str,str]` or
 `list[dict[str,str]]`.  Then data is postprocessed to apply any schemas and to unpack key paths.
 
@@ -93,31 +93,37 @@
 
 Currently, if a key path is used in defining a schema value or setting a
 data value, then the same key path must be used in both the schema and the
 data.  That is, schema validation is currently performed before key path
 unpacking.
 
 See the source code and the
-[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata_tex)
+[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata/tree/main/latex)
 documentation for additional details about schema support.
 
 
 ## Keys and key paths
 
 Data is interpreted as Python literals.  Thus, there is no checking for
 duplicate keys.  If a key is defined multiple times, later values replace
 earlier values.  Similarly, there is no checking for duplicate keys during
 key path unpacking.
 
 
 ## Usage
 
 The package provides two functions for loading data:
-* `load(<filehandle or pathlib.Path>, encoding='utf-8-sig')`
-* `loads(<string>)`
+
+ *  `load(<filehandle or pathlib.Path>, encoding='utf-8-sig')`
+
+ *  `loads(<string>)`
+
+Both of these functions takes optional arguments `schema: dict[str, str]` and
+`schema_missing: 'error' | 'rawstr' | 'evalany'`.  If these are provided, they
+override any schema settings in the file/string metadata.
 
 
 ## Tests
 
 The latex2pydata Python package includes tests.  Additional tests are part
 of the
-[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata_tex).
+[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata/tree/main/latex).
```

### Comparing `latex2pydata-0.1.0/README.md` & `latex2pydata-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # latex2pydata - load data from LaTeX in Python literal format
 
 The latex2pydata Python package is designed to load data in
 [Python literal format](https://docs.python.org/3/reference/lexical_analysis.html#literals)
 that was saved to file by the
-[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata_tex).
+[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata/tree/main/latex).
 This allows data to be passed from [LaTeX](https://www.latex-project.org/) to
 Python.
 
 Raw data is loaded with
 [`ast.literal_eval()`](https://docs.python.org/3/library/ast.html#ast.literal_eval).  This always yields either `dict[str,str]` or
 `list[dict[str,str]]`.  Then data is postprocessed to apply any schemas and to unpack key paths.
 
@@ -40,31 +40,37 @@
 
 Currently, if a key path is used in defining a schema value or setting a
 data value, then the same key path must be used in both the schema and the
 data.  That is, schema validation is currently performed before key path
 unpacking.
 
 See the source code and the
-[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata_tex)
+[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata/tree/main/latex)
 documentation for additional details about schema support.
 
 
 ## Keys and key paths
 
 Data is interpreted as Python literals.  Thus, there is no checking for
 duplicate keys.  If a key is defined multiple times, later values replace
 earlier values.  Similarly, there is no checking for duplicate keys during
 key path unpacking.
 
 
 ## Usage
 
 The package provides two functions for loading data:
-* `load(<filehandle or pathlib.Path>, encoding='utf-8-sig')`
-* `loads(<string>)`
+
+ *  `load(<filehandle or pathlib.Path>, encoding='utf-8-sig')`
+
+ *  `loads(<string>)`
+
+Both of these functions takes optional arguments `schema: dict[str, str]` and
+`schema_missing: 'error' | 'rawstr' | 'evalany'`.  If these are provided, they
+override any schema settings in the file/string metadata.
 
 
 ## Tests
 
 The latex2pydata Python package includes tests.  Additional tests are part
 of the
-[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata_tex).
+[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata/tree/main/latex).
```

### Comparing `latex2pydata-0.1.0/latex2pydata/fmtversion.py` & `latex2pydata-0.2.0/latex2pydata/fmtversion.py`

 * *Files identical despite different names*

### Comparing `latex2pydata-0.1.0/latex2pydata/loading.py` & `latex2pydata-0.2.0/latex2pydata/loading.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2023, Geoffrey M. Poore
+# Copyright (c) 2023-2024, Geoffrey M. Poore
 # All rights reserved.
 #
 # Licensed under the BSD 3-Clause License:
 # http://opensource.org/licenses/BSD-3-Clause
 #
 
 
@@ -29,59 +29,65 @@
 
 RawLoadedDataType = dict[str, str] | list[dict[str, str]]
 LoadedDataType = dict[str, Any] | list[dict[str, Any]]
 
 
 
 
-def load(readable: pathlib.Path | io.BytesIO | io.TextIOBase, encoding: str|None=None) -> LoadedDataType:
+def load(readable: pathlib.Path | io.BytesIO | io.TextIOBase,
+         encoding: str | None = None,
+         schema: dict[str, str] | None = None,
+         schema_missing: Literal['error'] | Literal['rawstr'] | Literal['evalany'] | None = None) -> LoadedDataType:
     if isinstance(readable, pathlib.Path):
         encoding = encoding or 'utf-8-sig'
-        return loads(readable.read_text(encoding=encoding))
+        return loads(readable.read_text(encoding=encoding), schema, schema_missing)
     raw_read: bytes | str = readable.read()
     if isinstance(raw_read, bytes):
         encoding = encoding or 'utf-8-sig'
-        return loads(raw_read.decode(encoding))
+        return loads(raw_read.decode(encoding), schema, schema_missing)
     if isinstance(raw_read, str):
         if encoding is not None:
             raise TypeError(f'Cannot specify encoding "{encoding}" for a readable that returns a string')
-        return loads(raw_read)
+        return loads(raw_read, schema, schema_missing)
     raise TypeError
 
 
-def loads(string: str) -> LoadedDataType:
-    schema: None | dict[str, str] = None
-    schema_missing: Literal['error'] | Literal['rawstr'] | Literal['evalany'] = 'error'
+def loads(string: str,
+          schema: dict[str, str] | None = None,
+          schema_missing: Literal['error'] | Literal['rawstr'] | Literal['evalany'] | None = None) -> LoadedDataType:
+
     if string.startswith(metadata_comment_pattern):
         metadata_str = string[len(metadata_comment_pattern):string.find('\n')].strip()
         try:
             metadata = ast.literal_eval(metadata_str)
         except Exception as e:
             raise Latex2PydataInvalidMetadataError(f'Loading metadata failed:\n{e}')
         if not isinstance(metadata, dict):
             raise Latex2PydataInvalidMetadataError('Invalid metadata (must be a dict)')
-        if 'schema' in metadata:
+        if schema is None and 'schema' in metadata:
             schema = metadata['schema']
-            if schema is not None:
-                if not isinstance(schema, dict):
-                    raise Latex2PydataSchemaError('Invalid schema (must be dict[str, str])')
-                if not all(isinstance(k, str) and isinstance(v, str) for k, v in schema.items()):
-                    raise Latex2PydataSchemaError('Invalid schema (must be dict[str, str])')
-                schema = {k: v.replace(' ', '') for k, v in schema.items()}
-                for k, v in schema.items():
-                    if not keypath_re.fullmatch(k):
-                        raise Latex2PydataSchemaError(f'Invalid or unsupported schema key "{k}"')
-                    if not annot_re.fullmatch(v):
-                        raise Latex2PydataSchemaError(
-                            f'Invalid or unsupported schema value (type annotation) "{v}"'
-                        )
-        if 'schema_missing' in metadata:
+        if schema_missing is None and 'schema_missing' in metadata:
             schema_missing = metadata['schema_missing']
-            if schema_missing not in ('error', 'rawstr', 'evalany'):
-                raise Latex2PydataInvalidMetadataError(f'Invalid "schema_missing" value "{schema_missing}"')
+    if schema is not None:
+        if not isinstance(schema, dict):
+            raise Latex2PydataSchemaError('Invalid schema (must be dict[str, str])')
+        if not all(isinstance(k, str) and isinstance(v, str) for k, v in schema.items()):
+            raise Latex2PydataSchemaError('Invalid schema (must be dict[str, str])')
+        schema = {k: v.replace(' ', '') for k, v in schema.items()}
+        for k, v in schema.items():
+            if not keypath_re.fullmatch(k):
+                raise Latex2PydataSchemaError(f'Invalid or unsupported schema key "{k}"')
+            if not annot_re.fullmatch(v):
+                raise Latex2PydataSchemaError(
+                    f'Invalid or unsupported schema value (type annotation) "{v}"'
+                )
+    if schema_missing is None:
+        schema_missing = 'error'
+    elif schema_missing not in ('error', 'rawstr', 'evalany'):
+        raise Latex2PydataInvalidMetadataError(f'Invalid "schema_missing" value "{schema_missing}"')
 
     try:
         raw_data: RawLoadedDataType = ast.literal_eval(string)
     except Exception as e:
         raise Latex2PydataInvalidDataError(f'Loading data with ast.literal_eval() failed:\n{e}')
     top_is_list: bool
     if isinstance(raw_data, list):
```

### Comparing `latex2pydata-0.1.0/latex2pydata/schema.py` & `latex2pydata-0.2.0/latex2pydata/schema.py`

 * *Files identical despite different names*

### Comparing `latex2pydata-0.1.0/latex2pydata/util.py` & `latex2pydata-0.2.0/latex2pydata/util.py`

 * *Files identical despite different names*

### Comparing `latex2pydata-0.1.0/latex2pydata.egg-info/PKG-INFO` & `latex2pydata-0.2.0/latex2pydata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex2pydata
-Version: 0.1.0
+Version: 0.2.0
 Summary: Load data from LaTeX in Python literal format
 Author-email: "Geoffrey M. Poore" <gpoore@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Geoffrey M. Poore
         All rights reserved.
         
@@ -29,17 +29,17 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: homepage, https://github.com/gpoore/latex2pydata_py
-Project-URL: repository, https://github.com/gpoore/latex2pydata_py
-Project-URL: changelog, https://github.com/gpoore/latex2pydata_py/blob/master/CHANGELOG.md
+Project-URL: homepage, https://github.com/gpoore/latex2pydata/tree/main/python
+Project-URL: repository, https://github.com/gpoore/latex2pydata
+Project-URL: changelog, https://github.com/gpoore/latex2pydata/blob/main/python/CHANGELOG.md
 Keywords: deserialization,LaTeX,Python literal format
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -52,15 +52,15 @@
 License-File: CHANGELOG.md
 
 # latex2pydata - load data from LaTeX in Python literal format
 
 The latex2pydata Python package is designed to load data in
 [Python literal format](https://docs.python.org/3/reference/lexical_analysis.html#literals)
 that was saved to file by the
-[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata_tex).
+[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata/tree/main/latex).
 This allows data to be passed from [LaTeX](https://www.latex-project.org/) to
 Python.
 
 Raw data is loaded with
 [`ast.literal_eval()`](https://docs.python.org/3/library/ast.html#ast.literal_eval).  This always yields either `dict[str,str]` or
 `list[dict[str,str]]`.  Then data is postprocessed to apply any schemas and to unpack key paths.
 
@@ -93,31 +93,37 @@
 
 Currently, if a key path is used in defining a schema value or setting a
 data value, then the same key path must be used in both the schema and the
 data.  That is, schema validation is currently performed before key path
 unpacking.
 
 See the source code and the
-[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata_tex)
+[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata/tree/main/latex)
 documentation for additional details about schema support.
 
 
 ## Keys and key paths
 
 Data is interpreted as Python literals.  Thus, there is no checking for
 duplicate keys.  If a key is defined multiple times, later values replace
 earlier values.  Similarly, there is no checking for duplicate keys during
 key path unpacking.
 
 
 ## Usage
 
 The package provides two functions for loading data:
-* `load(<filehandle or pathlib.Path>, encoding='utf-8-sig')`
-* `loads(<string>)`
+
+ *  `load(<filehandle or pathlib.Path>, encoding='utf-8-sig')`
+
+ *  `loads(<string>)`
+
+Both of these functions takes optional arguments `schema: dict[str, str]` and
+`schema_missing: 'error' | 'rawstr' | 'evalany'`.  If these are provided, they
+override any schema settings in the file/string metadata.
 
 
 ## Tests
 
 The latex2pydata Python package includes tests.  Additional tests are part
 of the
-[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata_tex).
+[latex2pydata LaTeX package](https://github.com/gpoore/latex2pydata/tree/main/latex).
```

### Comparing `latex2pydata-0.1.0/pyproject.toml` & `latex2pydata-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     'Operating System :: OS Independent',
     'Topic :: File Formats',
     'Topic :: Software Development :: Libraries',
 ]
 
 
 [project.urls]
-homepage = 'https://github.com/gpoore/latex2pydata_py'
-repository = 'https://github.com/gpoore/latex2pydata_py'
-changelog = 'https://github.com/gpoore/latex2pydata_py/blob/master/CHANGELOG.md'
+homepage = 'https://github.com/gpoore/latex2pydata/tree/main/python'
+repository = 'https://github.com/gpoore/latex2pydata'
+changelog = 'https://github.com/gpoore/latex2pydata/blob/main/python/CHANGELOG.md'
 
 
 [tool.setuptools]
 license-files = ['LICENSE*', 'CHANGELOG*']
 
 [tool.setuptools.dynamic]
 version = {attr = 'latex2pydata.__version__'}
```

### Comparing `latex2pydata-0.1.0/test/test_loads.py` & `latex2pydata-0.2.0/test/test_loads.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,25 @@
         "key3": "'abc'",
         "key4": "None",
         }
         ''')
     assert latex2pydata.loads(data_str) == {"key1": 123, "key2": True, "key3": 'abc', "key4": None}
 
 
+def test_loads_scalar_schema_opt_arg():
+    data_str = textwrap.dedent('''\
+        # latex2pydata metadata: {"schema": {"key1": "int"}, "schema_missing": "rawstr"}
+        {"key1": "123", "key2": "456",}
+        ''')
+    assert latex2pydata.loads(data_str) == {"key1": 123, "key2": "456"}
+    assert latex2pydata.loads(data_str, schema_missing='evalany') == {"key1": 123, "key2": 456}
+    assert latex2pydata.loads(data_str, schema={"key2": "int"}, schema_missing='rawstr') == {"key1": "123", "key2": 456}
+    assert latex2pydata.loads(data_str, schema={"key1": "int", "key2": "int"}) == {"key1": 123, "key2": 456}
+
+
 def test_loads_collection_schema():
     data_str = textwrap.dedent('''\
         # latex2pydata metadata: {"schema": {"key1": "list[set[int|float]]"}}
         {
         "key1": "[{1, 2.3}, {4, 5}, {6.0, 7.1}]"
         }
         ''')
```

