# Comparing `tmp/neptune_fetcher-0.2.0.tar.gz` & `tmp/neptune_fetcher-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_fetcher-0.2.0.tar", max compression
+gzip compressed data, was "neptune_fetcher-0.3.0.tar", max compression
```

## Comparing `neptune_fetcher-0.2.0.tar` & `neptune_fetcher-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      678 2024-04-19 12:25:59.982524 neptune_fetcher-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-04-19 12:25:59.982524 neptune_fetcher-0.2.0/LICENSE
--rw-r--r--   0        0        0    10266 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/README.md
--rw-r--r--   0        0        0     2352 2024-04-19 12:26:12.678558 neptune_fetcher-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      739 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/__init__.py
--rw-r--r--   0        0        0     1597 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/cache.py
--rw-r--r--   0        0        0     5219 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/fetchable.py
--rw-r--r--   0        0        0     3990 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/fields.py
--rw-r--r--   0        0        0     8471 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/read_only_project.py
--rw-r--r--   0        0        0     3054 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/read_only_run.py
--rw-r--r--   0        0        0    11886 1970-01-01 00:00:00.000000 neptune_fetcher-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      859 2024-04-23 11:35:45.902395 neptune_fetcher-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-23 11:35:45.902395 neptune_fetcher-0.3.0/LICENSE
+-rw-r--r--   0        0        0    14581 2024-04-23 11:35:45.902395 neptune_fetcher-0.3.0/README.md
+-rw-r--r--   0        0        0     2352 2024-04-23 11:35:56.622494 neptune_fetcher-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      739 2024-04-23 11:35:45.902395 neptune_fetcher-0.3.0/src/neptune_fetcher/__init__.py
+-rw-r--r--   0        0        0     1597 2024-04-23 11:35:45.902395 neptune_fetcher-0.3.0/src/neptune_fetcher/cache.py
+-rw-r--r--   0        0        0     5219 2024-04-23 11:35:45.902395 neptune_fetcher-0.3.0/src/neptune_fetcher/fetchable.py
+-rw-r--r--   0        0        0     3990 2024-04-23 11:35:45.902395 neptune_fetcher-0.3.0/src/neptune_fetcher/fields.py
+-rw-r--r--   0        0        0    11025 2024-04-23 11:35:45.902395 neptune_fetcher-0.3.0/src/neptune_fetcher/read_only_project.py
+-rw-r--r--   0        0        0     3054 2024-04-23 11:35:45.902395 neptune_fetcher-0.3.0/src/neptune_fetcher/read_only_run.py
+-rw-r--r--   0        0        0    16201 1970-01-01 00:00:00.000000 neptune_fetcher-0.3.0/PKG-INFO
```

### Comparing `neptune_fetcher-0.2.0/CHANGELOG.md` & `neptune_fetcher-0.3.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## neptune-fetcher 0.3.0
+
+### Features
+- Regex support with `columns_regex` and `names_regex` for `fetch_runs_df()` ([#20](https://github.com/neptune-ai/neptune-fetcher/pull/20))
+
+
 ## neptune-fetcher 0.2.0
 
 ### Features
 - Added support for bool, state, datetime and float series ([#19](https://github.com/neptune-ai/neptune-fetcher/pull/19))
 - Added support for fetching float series values ([#19](https://github.com/neptune-ai/neptune-fetcher/pull/19))
 
 ### Changes
```

### Comparing `neptune_fetcher-0.2.0/LICENSE` & `neptune_fetcher-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_fetcher-0.2.0/pyproject.toml` & `neptune_fetcher-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 style = "semver"
 pattern = "default-unprefixed"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 # Base neptune package
-neptune = "2.0.0a2"
+neptune = "2.0.0a3"
 
 # Optional for default progress update handling
 tqdm = { version = ">=4.66.0", optional = true }
 
 
 [tool.poetry]
 authors = ["neptune.ai <contact@neptune.ai>"]
@@ -24,15 +24,15 @@
 repository = "https://github.com/neptune-ai/neptune-fetcher"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-fetcher"
 readme = "README.md"
-version = "0.2.0"
+version = "0.3.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_fetcher-0.2.0/src/neptune_fetcher/__init__.py` & `neptune_fetcher-0.3.0/src/neptune_fetcher/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_fetcher-0.2.0/src/neptune_fetcher/cache.py` & `neptune_fetcher-0.3.0/src/neptune_fetcher/cache.py`

 * *Files identical despite different names*

### Comparing `neptune_fetcher-0.2.0/src/neptune_fetcher/fetchable.py` & `neptune_fetcher-0.3.0/src/neptune_fetcher/fetchable.py`

 * *Files identical despite different names*

### Comparing `neptune_fetcher-0.2.0/src/neptune_fetcher/fields.py` & `neptune_fetcher-0.3.0/src/neptune_fetcher/fields.py`

 * *Files identical despite different names*

### Comparing `neptune_fetcher-0.2.0/src/neptune_fetcher/read_only_project.py` & `neptune_fetcher-0.3.0/src/neptune_fetcher/read_only_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 # limitations under the License.
 #
 __all__ = [
     "ReadOnlyProject",
 ]
 
 import os
+import re
 from typing import (
     TYPE_CHECKING,
     Dict,
     Generator,
     Iterable,
     List,
     Optional,
     Union,
 )
 
+from neptune.api.pagination import paginate_over
 from neptune.envs import (
     NEPTUNE_FETCH_TABLE_STEP_SIZE,
     PROJECT_ENV_NAME,
 )
 from neptune.internal.backends.api_model import Project
 from neptune.internal.backends.hosted_neptune_backend import HostedNeptuneBackend
 from neptune.internal.backends.nql import (
@@ -57,14 +59,18 @@
     get_attribute_value_from_entry,
 )
 
 if TYPE_CHECKING:
     from pandas import DataFrame
 
 
+MAX_COLUMNS_ALLOWED = 10_000
+MAX_REGEXABLE_RUNS = 100
+
+
 class ReadOnlyProject:
     """Class for retrieving metadata from a neptune.ai project in a limited read-only mode."""
 
     def __init__(
         self,
         project: Optional[str] = None,
         api_token: Optional[str] = None,
@@ -88,14 +94,15 @@
         self._backend: HostedNeptuneBackend = HostedNeptuneBackend(
             credentials=Credentials.from_token(api_token=api_token), proxies=proxies
         )
         self._project_qualified_name: Optional[str] = conform_optional(self._project, QualifiedName)
         self._project_api_object: Project = project_name_lookup(
             backend=self._backend, name=self._project_qualified_name
         )
+        self._project_key: str = self._project_api_object.sys_id
         self._project_id: UniqueId = self._project_api_object.id
         self.project_identifier = normalize_project_name(
             name=self._project, workspace=self._project_api_object.workspace
         )
 
     def list_runs(self) -> Generator[Dict[str, Optional[str]], None, None]:
         """Lists IDs and names of the runs in the project.
@@ -141,14 +148,16 @@
         Returns `pandas.DataFrame` with two columns ('sys/id' and 'sys/name') and rows corresponding to project runs.
         """
         return self.fetch_runs_df(columns=["sys/id", "sys/name"])
 
     def fetch_runs_df(
         self,
         columns: Optional[Iterable[str]] = None,
+        columns_regex: Optional[str] = None,
+        names_regex: Optional[str] = None,
         with_ids: Optional[Iterable[str]] = None,
         states: Optional[Iterable[str]] = None,
         owners: Optional[Iterable[str]] = None,
         tags: Optional[Iterable[str]] = None,
         trashed: Optional[bool] = False,
         limit: Optional[int] = None,
         sort_by: str = "sys/creation_time",
@@ -156,14 +165,18 @@
         progress_bar: Union[bool, Optional[ProgressBarType]] = None,
     ) -> "DataFrame":
         """Fetches the runs' metadata and returns them as a pandas DataFrame.
 
         Args:
             columns: None or a list of column names to include in the result.
                 Defaults to None, which includes all available columns up to 10k.
+            columns_regex: A regex pattern to filter columns by name.
+                Use this parameter to include columns in addition to the ones specified by the `columns` parameter.
+            names_regex: A regex pattern to filter the runs by name.
+                When applied, it needs to limit the number of runs to 100 or fewer.
             with_ids: A list of run IDs to filter the results.
             states: A list of run states to filter the results.
             owners: A list of owner names to filter the results.
             tags: A list of tags to filter the results.
             trashed: Whether to return trashed runs as the result.
                 If True: return only trashed runs.
                 If False (default): return only non-trashed runs.
@@ -187,21 +200,64 @@
             # Fetch runs by specific IDs
             specific_run_ids = ["RUN-123", "RUN-456"]
             specific_runs_df = my_project.fetch_runs_df(with_ids=specific_run_ids)
             ```
         """
         step_size = int(os.getenv(NEPTUNE_FETCH_TABLE_STEP_SIZE, "200"))
 
-        query = prepare_nql_query(with_ids, states, owners, tags, trashed)
-
         if columns is not None:
             # always return entries with `sys/id` column when filter applied
             columns = set(columns)
             columns.add("sys/id")
 
+            if columns_regex is not None:
+                field_definitions = list(
+                    paginate_over(
+                        getter=self._backend.query_fields_definitions_within_project,
+                        extract_entries=lambda data: data.entries,
+                        project_id=self._project_qualified_name,
+                        field_name_regex=columns_regex,
+                        experiment_ids_filter=with_ids,
+                    )
+                )
+                for field_definition in field_definitions:
+                    columns.add(field_definition.path)
+
+            if len(columns) > MAX_COLUMNS_ALLOWED:
+                raise ValueError(
+                    f"Too many columns requested ({len(columns)}). "
+                    "Please limit the number of columns to 10 000 or fewer."
+                )
+
+        if names_regex is not None:
+            objects = paginate_over(
+                getter=self._backend.query_fields_within_project,
+                extract_entries=lambda data: data.entries,
+                project_id=self._project_qualified_name,
+                field_names_filter=["sys/name"],
+                experiment_ids_filter=with_ids,
+            )
+            regex = re.compile(names_regex)
+            filtered_with_ids = []
+
+            for experiment in objects:
+                for field in experiment.fields:
+                    if field.path == "sys/name" and regex.match(field.value) is not None:
+                        filtered_with_ids.append(experiment.object_key)
+
+                        if len(filtered_with_ids) > MAX_REGEXABLE_RUNS:
+                            raise ValueError(
+                                "Too many runs matched the names regex. "
+                                f"Please limit the number of runs to {MAX_REGEXABLE_RUNS} or fewer."
+                            )
+
+            with_ids = filtered_with_ids
+
+        query = prepare_nql_query(ids=with_ids, states=states, owners=owners, tags=tags, trashed=trashed)
+
         leaderboard_entries = self._backend.search_leaderboard_entries(
             project_id=self._project_id,
             types=[ContainerType.RUN],
             query=query,
             columns=columns,
             limit=limit,
             sort_by=sort_by,
```

### Comparing `neptune_fetcher-0.2.0/src/neptune_fetcher/read_only_run.py` & `neptune_fetcher-0.3.0/src/neptune_fetcher/read_only_run.py`

 * *Files identical despite different names*

