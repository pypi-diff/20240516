# Comparing `tmp/gardener_cicd_cli-1.2397.0.tar.gz` & `tmp/gardener_cicd_cli-1.2398.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_cli-1.2397.0.tar", last modified: Wed May 15 08:51:36 2024, max compression
+gzip compressed data, was "gardener_cicd_cli-1.2398.0.tar", last modified: Thu May 16 11:19:16 2024, max compression
```

## Comparing `gardener_cicd_cli-1.2397.0.tar` & `gardener_cicd_cli-1.2398.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:51:36.322403 gardener_cicd_cli-1.2397.0/
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      222 2024-05-15 08:51:36.322403 gardener_cicd_cli-1.2397.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:51:36.318403 gardener_cicd_cli-1.2397.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)    11057 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/bin/component-cli
--rwxr-xr-x   0 root         (0) root         (0)      369 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/bin/helm
--rwxr-xr-x   0 root         (0) root         (0)     5611 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/bin/launch-dockerd.sh
--rwxr-xr-x   0 root         (0) root         (0)     2694 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/bin/purge_history
--rwxr-xr-x   0 root         (0) root         (0)      265 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/bin/yaml2json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:51:36.322403 gardener_cicd_cli-1.2397.0/gardener_ci/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3901 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/_cfg_mgmt.py
--rw-r--r--   0 root         (0) root         (0)     1984 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/_clamav.py
--rw-r--r--   0 root         (0) root         (0)     5856 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/_concourse.py
--rw-r--r--   0 root         (0) root         (0)    14191 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/_oci.py
--rw-r--r--   0 root         (0) root         (0)     2327 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/_release_notes.py
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/_slack.py
--rw-r--r--   0 root         (0) root         (0)    14072 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/bdba.py
--rw-r--r--   0 root         (0) root         (0)     4900 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/cd.py
--rw-r--r--   0 root         (0) root         (0)     1856 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/checkmarx_cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9039 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/cli_gen.py
--rw-r--r--   0 root         (0) root         (0)     8184 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/compliance.py
--rw-r--r--   0 root         (0) root         (0)     2797 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/config.py
--rw-r--r--   0 root         (0) root         (0)      463 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/containerutil.py
--rw-r--r--   0 root         (0) root         (0)      964 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/docker.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/elastic.py
--rw-r--r--   0 root         (0) root         (0)     3512 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/gh.py
--rw-r--r--   0 root         (0) root         (0)     4328 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/githubutil.py
--rw-r--r--   0 root         (0) root         (0)    12193 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/ocm.py
--rw-r--r--   0 root         (0) root         (0)    12771 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     3031 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/productutil_v2.py
--rwxr-xr-x   0 root         (0) root         (0)      265 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/gardener_ci/yaml2json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:51:36.322403 gardener_cicd_cli-1.2397.0/gardener_cicd_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      222 2024-05-15 08:51:36.000000 gardener_cicd_cli-1.2397.0/gardener_cicd_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      944 2024-05-15 08:51:36.000000 gardener_cicd_cli-1.2397.0/gardener_cicd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 08:51:36.000000 gardener_cicd_cli-1.2397.0/gardener_cicd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2024-05-15 08:51:36.000000 gardener_cicd_cli-1.2397.0/gardener_cicd_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-05-15 08:51:36.000000 gardener_cicd_cli-1.2397.0/gardener_cicd_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-15 08:51:36.000000 gardener_cicd_cli-1.2397.0/gardener_cicd_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 08:51:36.322403 gardener_cicd_cli-1.2397.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2024-05-15 08:50:06.000000 gardener_cicd_cli-1.2397.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:19:16.451780 gardener_cicd_cli-1.2398.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      222 2024-05-16 11:19:16.451780 gardener_cicd_cli-1.2398.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:19:16.443780 gardener_cicd_cli-1.2398.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    11057 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/bin/component-cli
+-rwxr-xr-x   0 root         (0) root         (0)      369 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/bin/helm
+-rwxr-xr-x   0 root         (0) root         (0)     5611 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/bin/launch-dockerd.sh
+-rwxr-xr-x   0 root         (0) root         (0)     2694 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/bin/purge_history
+-rwxr-xr-x   0 root         (0) root         (0)      265 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/bin/yaml2json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:19:16.447780 gardener_cicd_cli-1.2398.0/gardener_ci/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/_cfg_mgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/_clamav.py
+-rw-r--r--   0 root         (0) root         (0)     5856 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/_concourse.py
+-rw-r--r--   0 root         (0) root         (0)    14191 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/_oci.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/_slack.py
+-rw-r--r--   0 root         (0) root         (0)    14066 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/bdba.py
+-rw-r--r--   0 root         (0) root         (0)     4900 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/cd.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/checkmarx_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9039 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/cli_gen.py
+-rw-r--r--   0 root         (0) root         (0)     8184 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/compliance.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/config.py
+-rw-r--r--   0 root         (0) root         (0)      463 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/containerutil.py
+-rw-r--r--   0 root         (0) root         (0)      964 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/docker.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/elastic.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/gh.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/githubutil.py
+-rw-r--r--   0 root         (0) root         (0)    12193 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/ocm.py
+-rw-r--r--   0 root         (0) root         (0)    12771 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/productutil_v2.py
+-rwxr-xr-x   0 root         (0) root         (0)      265 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/gardener_ci/yaml2json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:19:16.451780 gardener_cicd_cli-1.2398.0/gardener_cicd_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      222 2024-05-16 11:19:16.000000 gardener_cicd_cli-1.2398.0/gardener_cicd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      944 2024-05-16 11:19:16.000000 gardener_cicd_cli-1.2398.0/gardener_cicd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 11:19:16.000000 gardener_cicd_cli-1.2398.0/gardener_cicd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2024-05-16 11:19:16.000000 gardener_cicd_cli-1.2398.0/gardener_cicd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-16 11:19:16.000000 gardener_cicd_cli-1.2398.0/gardener_cicd_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-16 11:19:16.000000 gardener_cicd_cli-1.2398.0/gardener_cicd_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 11:19:16.451780 gardener_cicd_cli-1.2398.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2024-05-16 11:18:13.000000 gardener_cicd_cli-1.2398.0/setup.py
```

### Comparing `gardener_cicd_cli-1.2397.0/bin/component-cli` & `gardener_cicd_cli-1.2398.0/bin/component-cli`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/bin/launch-dockerd.sh` & `gardener_cicd_cli-1.2398.0/bin/launch-dockerd.sh`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/bin/purge_history` & `gardener_cicd_cli-1.2398.0/bin/purge_history`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/_cfg_mgmt.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/_cfg_mgmt.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/_clamav.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/_clamav.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/_concourse.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/_concourse.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/_oci.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/_oci.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/_release_notes.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/_release_notes.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/bdba.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/bdba.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 
     def _grouped_results(results: list[dso.model.ArtefactMetadata]) -> dict:
         grouped_results = dict()
 
         for r in results:
             c_id = f'{r.artefact.component_name}:{r.artefact.component_version}'
             a_id = f'{r.artefact.artefact.artefact_name}:{r.artefact.artefact.artefact_version}'
-            p_id = f'{r.data.id.package_name}:{r.data.id.package_version}'
+            p_id = f'{r.data.package_name}:{r.data.package_version}'
 
             key = f'{c_id}:{a_id}:{p_id}'
 
             cve = r.data.cve
             cvss_v3_score = r.data.cvss_v3_score
 
             if key in grouped_results:
```

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/cd.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/cd.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/checkmarx_cli.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/checkmarx_cli.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/cli_gen.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/cli_gen.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/compliance.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/compliance.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/config.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/config.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/docker.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/docker.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/elastic.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/elastic.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/gh.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/gh.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/githubutil.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/githubutil.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/ocm.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/ocm.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/pipeline.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_ci/productutil_v2.py` & `gardener_cicd_cli-1.2398.0/gardener_ci/productutil_v2.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/gardener_cicd_cli.egg-info/SOURCES.txt` & `gardener_cicd_cli-1.2398.0/gardener_cicd_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener_cicd_cli-1.2397.0/setup.py` & `gardener_cicd_cli-1.2398.0/setup.py`

 * *Files identical despite different names*

