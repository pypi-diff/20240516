# Comparing `tmp/cstructs-0.2.1.tar.gz` & `tmp/cstructs-0.2.2.tar.gz`

## Comparing `cstructs-0.2.1.tar` & `cstructs-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 cstructs-0.2.1/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/.gitignore
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/cstructs.iml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/discord.xml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/misc.xml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/modules.xml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/vcs.xml
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/workspace.xml
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/copyright/gplv3.xml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/copyright/profiles_settings.xml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM__Changes_.xml
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 cstructs-0.2.1/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM_[Changes]/shelved.patch
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 cstructs-0.2.1/docs/nativetypes
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/__about__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/__init__.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/exc.py
--rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/nativetypes.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/util.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/datastruct/__init__.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/datastruct/metadata.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 cstructs-0.2.1/src/cstructs/datastruct/reader.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_decorator.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_inheritance.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_metaclass.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_metadata.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_read.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 cstructs-0.2.1/tests/test_write.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cstructs-0.2.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 cstructs-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 cstructs-0.2.1/README.md
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 cstructs-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 cstructs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    23005 2020-02-02 00:00:00.000000 cstructs-0.2.2/cstructs-0.2.1-py3-none-any.whl
+-rw-r--r--   0        0        0    86072 2020-02-02 00:00:00.000000 cstructs-0.2.2/cstructs-0.2.1.tar.gz
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 cstructs-0.2.2/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/.gitignore
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/cstructs.iml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/discord.xml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/misc.xml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/modules.xml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/copyright/gplv3.xml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/copyright/profiles_settings.xml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM__Changes_.xml
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 cstructs-0.2.2/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM_[Changes]/shelved.patch
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 cstructs-0.2.2/docs/nativetypes
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cstructs-0.2.2/src/cstructs/__about__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 cstructs-0.2.2/src/cstructs/__init__.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 cstructs-0.2.2/src/cstructs/exc.py
+-rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 cstructs-0.2.2/src/cstructs/nativetypes.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cstructs-0.2.2/src/cstructs/util.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 cstructs-0.2.2/src/cstructs/datastruct/__init__.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 cstructs-0.2.2/src/cstructs/datastruct/metadata.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 cstructs-0.2.2/src/cstructs/datastruct/reader.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 cstructs-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 cstructs-0.2.2/tests/test_decorator.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 cstructs-0.2.2/tests/test_inheritance.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 cstructs-0.2.2/tests/test_metaclass.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 cstructs-0.2.2/tests/test_metadata.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 cstructs-0.2.2/tests/test_read.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 cstructs-0.2.2/tests/test_write.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cstructs-0.2.2/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 cstructs-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 cstructs-0.2.2/README.md
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 cstructs-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 cstructs-0.2.2/PKG-INFO
```

### Comparing `cstructs-0.2.1/.github/workflows/run-tests.yml` & `cstructs-0.2.2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/.idea/cstructs.iml` & `cstructs-0.2.2/.idea/cstructs.iml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/.idea/workspace.xml` & `cstructs-0.2.2/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `cstructs-0.2.1/.idea/workspace.xml` & `cstructs-0.2.2/.idea/workspace.xml`

```diff
@@ -115,15 +115,15 @@
       <workItem from="1701985877259" duration="3367000"/>
       <workItem from="1710988496657" duration="646000"/>
       <workItem from="1711200100969" duration="6000"/>
       <workItem from="1713623099607" duration="4160000"/>
       <workItem from="1715727875622" duration="40917000"/>
       <workItem from="1715880880748" duration="2518000"/>
       <workItem from="1715884342597" duration="50000"/>
-      <workItem from="1715884716793" duration="1992000"/>
+      <workItem from="1715884716793" duration="3411000"/>
     </task>
     <task id="LOCAL-00017" summary="Minor changes to `nativetypes.py`
 * Raise `InvalidTypeDef` if a `NativeType` is called with a `repeat_length` of 0.
 * Convert `NativeTypes` into a regular class.">
       <option name="closed" value="true"/>
       <created>1701537202276</created>
       <option name="number" value="00017"/>
```

### Comparing `cstructs-0.2.1/.idea/copyright/gplv3.xml` & `cstructs-0.2.2/.idea/copyright/gplv3.xml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/.idea/copyright/profiles_settings.xml` & `cstructs-0.2.2/.idea/copyright/profiles_settings.xml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/.idea/inspectionProfiles/Project_Default.xml` & `cstructs-0.2.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM_[Changes]/shelved.patch` & `cstructs-0.2.2/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM_[Changes]/shelved.patch`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/docs/nativetypes` & `cstructs-0.2.2/docs/nativetypes`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/src/cstructs/__about__.py` & `cstructs-0.2.2/src/cstructs/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A     -
 #  PARTICULAR PURPOSE. See the GNU General Public License for more details.            -
 #                                                                                      -
 #  You should have received a copy of the GNU General Public License along with        -
 #  this program. If not, see <http://www.gnu.org/licenses/>.                           -
 # --------------------------------------------------------------------------------------
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `cstructs-0.2.1/src/cstructs/__init__.py` & `cstructs-0.2.2/src/cstructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/src/cstructs/exc.py` & `cstructs-0.2.2/src/cstructs/exc.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/src/cstructs/nativetypes.py` & `cstructs-0.2.2/src/cstructs/nativetypes.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/src/cstructs/util.py` & `cstructs-0.2.2/src/cstructs/util.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/src/cstructs/datastruct/__init__.py` & `cstructs-0.2.2/src/cstructs/datastruct/__init__.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/src/cstructs/datastruct/metadata.py` & `cstructs-0.2.2/src/cstructs/datastruct/metadata.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/src/cstructs/datastruct/reader.py` & `cstructs-0.2.2/src/cstructs/datastruct/reader.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/tests/__init__.py` & `cstructs-0.2.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/tests/test_decorator.py` & `cstructs-0.2.2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/tests/test_inheritance.py` & `cstructs-0.2.2/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/tests/test_metaclass.py` & `cstructs-0.2.2/tests/test_metaclass.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/tests/test_metadata.py` & `cstructs-0.2.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/tests/test_read.py` & `cstructs-0.2.2/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/tests/test_write.py` & `cstructs-0.2.2/tests/test_write.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/.gitignore` & `cstructs-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/LICENSE.txt` & `cstructs-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/README.md` & `cstructs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.1/pyproject.toml` & `cstructs-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cstructs"
 dynamic = ["version"]
-description = ''
+description = 'Powerful decorator allowing the parsing of binary data into a dataclass and serializing back into raw data.'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "GPL-3.0-or-later"
 keywords = []
 authors = [
   { name = "yntha", email = "bguznvjk@gmail.com" },
 ]
@@ -20,17 +20,17 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = []
 
 [project.urls]
-Documentation = "https://github.com/unknown/cstructs#readme"
-Issues = "https://github.com/unknown/cstructs/issues"
-Source = "https://github.com/unknown/cstructs"
+Documentation = "https://github.com/yntha/cstructs#readme"
+Issues = "https://github.com/yntha/cstructs/issues"
+Source = "https://github.com/yntha/cstructs"
 
 [tool.hatch.version]
 path = "src/cstructs/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
```

### Comparing `cstructs-0.2.1/PKG-INFO` & `cstructs-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: cstructs
-Version: 0.2.1
-Project-URL: Documentation, https://github.com/unknown/cstructs#readme
-Project-URL: Issues, https://github.com/unknown/cstructs/issues
-Project-URL: Source, https://github.com/unknown/cstructs
+Version: 0.2.2
+Summary: Powerful decorator allowing the parsing of binary data into a dataclass and serializing back into raw data.
+Project-URL: Documentation, https://github.com/yntha/cstructs#readme
+Project-URL: Issues, https://github.com/yntha/cstructs/issues
+Project-URL: Source, https://github.com/yntha/cstructs
 Author-email: yntha <bguznvjk@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

