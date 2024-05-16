# Comparing `tmp/gardener_cicd_dso-1.2397.0.tar.gz` & `tmp/gardener_cicd_dso-1.2398.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_dso-1.2397.0.tar", last modified: Wed May 15 08:51:35 2024, max compression
+gzip compressed data, was "gardener_cicd_dso-1.2398.0.tar", last modified: Thu May 16 11:19:15 2024, max compression
```

## Comparing `gardener_cicd_dso-1.2397.0.tar` & `gardener_cicd_dso-1.2398.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:51:35.718402 gardener_cicd_dso-1.2397.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      211 2024-05-15 08:51:35.718402 gardener_cicd_dso-1.2397.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2093 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:51:35.714402 gardener_cicd_dso-1.2397.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7945 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    19358 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:51:35.718402 gardener_cicd_dso-1.2397.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4680 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     8552 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2252 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7469 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     5564 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:51:35.718402 gardener_cicd_dso-1.2397.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2024-05-15 08:51:35.000000 gardener_cicd_dso-1.2397.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2024-05-15 08:51:35.000000 gardener_cicd_dso-1.2397.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 08:51:35.000000 gardener_cicd_dso-1.2397.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-05-15 08:51:35.000000 gardener_cicd_dso-1.2397.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-05-15 08:51:35.000000 gardener_cicd_dso-1.2397.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:51:35.718402 gardener_cicd_dso-1.2397.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7653 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    17319 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    10774 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     3636 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    29384 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-15 08:51:35.718402 gardener_cicd_dso-1.2397.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-05-15 08:50:06.000000 gardener_cicd_dso-1.2397.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:19:15.867779 gardener_cicd_dso-1.2398.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      211 2024-05-16 11:19:15.867779 gardener_cicd_dso-1.2398.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:19:15.863778 gardener_cicd_dso-1.2398.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7945 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    19358 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:19:15.863778 gardener_cicd_dso-1.2398.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:19:15.867779 gardener_cicd_dso-1.2398.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2024-05-16 11:19:15.000000 gardener_cicd_dso-1.2398.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      670 2024-05-16 11:19:15.000000 gardener_cicd_dso-1.2398.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 11:19:15.000000 gardener_cicd_dso-1.2398.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-16 11:19:15.000000 gardener_cicd_dso-1.2398.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-16 11:19:15.000000 gardener_cicd_dso-1.2398.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:19:15.867779 gardener_cicd_dso-1.2398.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    17319 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    10774 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    29384 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)    13605 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-16 11:19:15.867779 gardener_cicd_dso-1.2398.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-05-16 11:18:13.000000 gardener_cicd_dso-1.2398.0/setup.py
```

### Comparing `gardener_cicd_dso-1.2397.0/LICENSE` & `gardener_cicd_dso-1.2398.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/README.md` & `gardener_cicd_dso-1.2398.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/checkmarx/client.py` & `gardener_cicd_dso-1.2398.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/checkmarx/model.py` & `gardener_cicd_dso-1.2398.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/checkmarx/project.py` & `gardener_cicd_dso-1.2398.0/checkmarx/project.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/checkmarx/tablefmt.py` & `gardener_cicd_dso-1.2398.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/checkmarx/util.py` & `gardener_cicd_dso-1.2398.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/clamav/client.py` & `gardener_cicd_dso-1.2398.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/clamav/cnudie.py` & `gardener_cicd_dso-1.2398.0/clamav/cnudie.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/clamav/model.py` & `gardener_cicd_dso-1.2398.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/clamav/report.py` & `gardener_cicd_dso-1.2398.0/clamav/report.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/clamav/routes.py` & `gardener_cicd_dso-1.2398.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/clamav/scan.py` & `gardener_cicd_dso-1.2398.0/clamav/scan.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/clamav/util.py` & `gardener_cicd_dso-1.2398.0/clamav/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener_cicd_dso-1.2398.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/protecode/assessments.py` & `gardener_cicd_dso-1.2398.0/protecode/assessments.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/protecode/client.py` & `gardener_cicd_dso-1.2398.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/protecode/model.py` & `gardener_cicd_dso-1.2398.0/protecode/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/protecode/rescore.py` & `gardener_cicd_dso-1.2398.0/protecode/rescore.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/protecode/scanning.py` & `gardener_cicd_dso-1.2398.0/protecode/scanning.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/protecode/util.py` & `gardener_cicd_dso-1.2398.0/protecode/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,27 +58,23 @@
 
     artefact = gcm.artifact_from_node(node=scanned_element)
     artefact_ref = dso.model.component_artefact_id_from_ocm(
         component=scanned_element.component,
         artefact=artefact,
     )
 
-    scan_id = dso.model.BDBAScanId(
-        base_url=scan_result.base_url(),
-        report_url=scan_result.report_url(),
-        product_id=scan_result.product_id(),
-        group_id=scan_result.group_id(),
-    )
+    base_url = scan_result.base_url()
+    report_url = scan_result.report_url()
+    product_id = scan_result.product_id()
+    group_id = scan_result.group_id()
 
     findings: list[dso.model.ArtefactMetadata] = []
     for package in scan_result.components():
-        package_id = dso.model.BDBAPackageId(
-            package_name=package.name(),
-            package_version=package.version(),
-        )
+        package_name = package.name()
+        package_version = package.version()
 
         filesystem_paths = list(iter_filesystem_paths(component=package))
 
         licenses = list({
             dso.model.License(
                 name=license.name,
             ) for license in package.licenses
@@ -87,16 +83,20 @@
         meta = dso.model.Metadata(
             datasource=dso.model.Datasource.BDBA,
             type=dso.model.Datatype.STRUCTURE_INFO,
             creation_date=now,
         )
 
         structure_info = dso.model.StructureInfo(
-            id=package_id,
-            scan_id=scan_id,
+            package_name=package_name,
+            package_version=package_version,
+            base_url=base_url,
+            report_url=report_url,
+            product_id=product_id,
+            group_id=group_id,
             licenses=licenses,
             filesystem_paths=filesystem_paths,
         )
 
         yield dso.model.ArtefactMetadata(
             artefact=artefact_ref,
             meta=meta,
@@ -111,16 +111,20 @@
         )
 
         for license in licenses:
             if not license_cfg or license_cfg.is_allowed(license=license.name):
                 continue
 
             license_finding = dso.model.LicenseFinding(
-                id=package_id,
-                scan_id=scan_id,
+                package_name=package_name,
+                package_version=package_version,
+                base_url=base_url,
+                report_url=report_url,
+                product_id=product_id,
+                group_id=group_id,
                 severity=gcm.Severity.BLOCKER.name,
                 license=license,
             )
 
             artefact_metadata = dso.model.ArtefactMetadata(
                 artefact=artefact_ref,
                 meta=meta,
@@ -150,19 +154,15 @@
                 # convert it in our scoping, so there would always be some edge cases where it does
                 # not fit properly. However, by translating all triages for each scan result, we
                 # implicitly use the BDBA scopes since they are already applied by BDBA to each scan
                 # result. So, we can correctly mimic the BDBA scopes with the acceptable price of
                 # redundant (rescoring) data.
                 vulnerability_rescoring = dso.model.CustomRescoring(
                     finding=dso.model.RescoringVulnerabilityFinding(
-                        id=dso.model.BDBAPackageId(
-                            package_name=package_id.package_name,
-                            # don't specify version to store only one rescoring per package name
-                            package_version=None,
-                        ),
+                        package_name=package_name,
                         cve=vulnerability.cve(),
                     ),
                     referenced_type=dso.model.Datatype.VULNERABILITY,
                     severity=gcm.Severity.NONE.name, # bdba only allows triaging to NONE
                     user=dso.model.BDBAUser(
                         username=triage.user().get('username'),
                         email=triage.user().get('email'),
@@ -182,16 +182,20 @@
             meta = dso.model.Metadata(
                 datasource=dso.model.Datasource.BDBA,
                 type=dso.model.Datatype.VULNERABILITY,
                 creation_date=now,
             )
 
             vulnerability_finding = dso.model.VulnerabilityFinding(
-                id=package_id,
-                scan_id=scan_id,
+                package_name=package_name,
+                package_version=package_version,
+                base_url=base_url,
+                report_url=report_url,
+                product_id=product_id,
+                group_id=group_id,
                 severity=gcr._criticality_classification(
                     cve_score=vulnerability.cve_severity(),
                 ).name,
                 cve=vulnerability.cve(),
                 cvss_v3_score=vulnerability.cve_severity(),
                 cvss=vulnerability.cvss,
                 summary=vulnerability.summary(),
```

### Comparing `gardener_cicd_dso-1.2397.0/setup.dso.py` & `gardener_cicd_dso-1.2398.0/setup.dso.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2397.0/setup.py` & `gardener_cicd_dso-1.2398.0/setup.py`

 * *Files identical despite different names*

