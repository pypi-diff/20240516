# Comparing `tmp/spark_congruity-0.0.1rc0.tar.gz` & `tmp/spark_congruity-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_congruity-0.0.1rc0.tar", max compression
+gzip compressed data, was "spark_congruity-0.0.1rc1.tar", max compression
```

## Comparing `spark_congruity-0.0.1rc0.tar` & `spark_congruity-0.0.1rc1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-05-16 05:53:44.907450 spark_congruity-0.0.1rc0/LICENSE
--rw-r--r--   0        0        0     1150 2024-05-16 05:53:44.907450 spark_congruity-0.0.1rc0/NOTICE
--rw-r--r--   0        0        0     1667 2024-05-16 05:53:44.907450 spark_congruity-0.0.1rc0/README.md
--rw-r--r--   0        0        0     1311 2024-05-16 05:53:44.907450 spark_congruity-0.0.1rc0/congruity/__init__.py
--rw-r--r--   0        0        0     1594 2024-05-16 05:53:44.907450 spark_congruity-0.0.1rc0/congruity/json_conversion.py
--rw-r--r--   0        0        0     3329 2024-05-16 05:53:44.907450 spark_congruity-0.0.1rc0/congruity/rdd_adapter.py
--rw-r--r--   0        0        0     2150 2024-05-16 05:53:44.907450 spark_congruity-0.0.1rc0/pyproject.toml
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 spark_congruity-0.0.1rc0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 15:30:11.346106 spark_congruity-0.0.1rc1/LICENSE
+-rw-r--r--   0        0        0     1150 2024-05-16 15:30:11.346106 spark_congruity-0.0.1rc1/NOTICE
+-rw-r--r--   0        0        0    14765 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/README.md
+-rw-r--r--   0        0        0     2146 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/congruity/__init__.py
+-rw-r--r--   0        0        0     1594 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/congruity/json_conversion.py
+-rw-r--r--   0        0        0     8890 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/congruity/rdd_adapter.py
+-rw-r--r--   0        0        0     1544 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/congruity/spark_context_adapter.py
+-rw-r--r--   0        0        0     2206 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    15699 1970-01-01 00:00:00.000000 spark_congruity-0.0.1rc1/PKG-INFO
```

### Comparing `spark_congruity-0.0.1rc0/LICENSE` & `spark_congruity-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc0/NOTICE` & `spark_congruity-0.0.1rc1/NOTICE`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc0/congruity/json_conversion.py` & `spark_congruity-0.0.1rc1/congruity/json_conversion.py`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc0/pyproject.toml` & `spark_congruity-0.0.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "spark-congruity"
-version = "0.0.1rc0"
+version = "0.0.1rc1"
 description = ""
 authors = ["Matthew Powers <matthewkevinpowers@gmail.com>", "Martin Grund <martin@databricks.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/databricks/congruity"
 repository = "https://github.com/databricks/congruity"
 classifiers = [
@@ -43,19 +43,23 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7"
 chispa = "0.9.4"
 pytest-describe = "^2"
 pyspark = {extras = ["connect"], version = "3.5.0"}
 
+
+[tool.poetry.group.dev.dependencies]
+black = "24.3.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 # When changing the version, we have to update
 # GitHub workflow version and dev/reformat-python
-required-version = "23.9.1"
+required-version = "24.3.0"
 line-length = 100
 target-version = ['py38']
 include = '\.pyi?$'
 extend-exclude = 'cloudpickle|error_classes.py'
```

