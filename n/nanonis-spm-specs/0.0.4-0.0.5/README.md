# Comparing `tmp/nanonis_spm_specs-0.0.4.tar.gz` & `tmp/nanonis_spm_specs-0.0.5.tar.gz`

## Comparing `nanonis_spm_specs-0.0.4.tar` & `nanonis_spm_specs-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/.DS_Store
--rw-r--r--   0        0        0  1935487 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/TCPProtocol_SPM.pdf
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/test.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/.idea/SPECS.iml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0     9047 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/.idea/workspace.xml
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0   488397 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/nanonis_spm_specs/NanonisClass.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/nanonis_spm_specs/__init__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/README.md
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0  1935487 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/TCPProtocol_SPM.pdf
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/package-lock.json
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/test.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/.idea/SPECS.iml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0   488350 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/nanonis_spm_specs/NanonisClass.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/nanonis_spm_specs/__init__.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/trash/Spectroscopy0001.fsb
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/trash/Spectroscopy0002.fsb
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/README.md
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 nanonis_spm_specs-0.0.5/PKG-INFO
```

### Comparing `nanonis_spm_specs-0.0.4/TCPProtocol_SPM.pdf` & `nanonis_spm_specs-0.0.5/TCPProtocol_SPM.pdf`

 * *Files identical despite different names*

### Comparing `nanonis_spm_specs-0.0.4/.idea/workspace.xml` & `nanonis_spm_specs-0.0.5/.idea/workspace.xml`

 * *Files 8% similar despite different names*

#### Comparing `nanonis_spm_specs-0.0.4/.idea/workspace.xml` & `nanonis_spm_specs-0.0.5/.idea/workspace.xml`

```diff
@@ -3,19 +3,22 @@
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="15c2ba6c-d2d2-4be3-8734-f6948252bab3" name="Changes" comment="WorkingVersion">
       <change afterPath="$PROJECT_DIR$/LICENSE.txt" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/dist/nanonis_spm_specs-0.0.3-py3-none-any.whl" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/dist/nanonis_spm_specs-0.0.3.tar.gz" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/dist/nanonis_spm_specs-0.0.5-py3-none-any.whl" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/dist/nanonis_spm_specs-0.0.5.tar.gz" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/nanonis_spm_specs/__init__.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/package-lock.json" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/test.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/trash/Spectroscopy0001.fsb" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/trash/Spectroscopy0002.fsb" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/NanonisClass.py" beforeDir="false" afterPath="$PROJECT_DIR$/nanonis_spm_specs/NanonisClass.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/NanonisPython-2.py" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/NanonisPython.py" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/Nanonis_py/Nanonis.py" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/TCPProtocol_SPM.pdf" beforeDir="false" afterPath="$PROJECT_DIR$/TCPProtocol_SPM.pdf" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/TCPProtocol_Tramea.pdf" beforeDir="false"/>
     </list>
@@ -44,44 +47,46 @@
   <component name="ProjectLevelVcsManager" settingsEditedManually="true">
     <ConfirmationsSetting value="2" id="Add"/>
   </component>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "ASKED_ADD_EXTERNAL_FILES": "true",
-    "Python.NanonisClass.executor": "Run",
-    "Python.test.executor": "Run",
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "WebServerToolWindowFactoryState": "false",
-    "git-widget-placeholder": "master",
-    "last_opened_file_path": "/Users/samueloneill/Desktop/SPECS_SPM",
-    "node.js.detected.package.eslint": "true",
-    "node.js.detected.package.tslint": "true",
-    "node.js.selected.package.eslint": "(autodetect)",
-    "node.js.selected.package.tslint": "(autodetect)",
-    "nodejs_package_manager_path": "npm",
-    "settings.editor.selected.configurable": "terminal",
-    "vue.rearranger.settings.migration": "true"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;ASKED_ADD_EXTERNAL_FILES&quot;: &quot;true&quot;,
+    &quot;Python.NanonisClass.executor&quot;: &quot;Run&quot;,
+    &quot;Python.test.executor&quot;: &quot;Run&quot;,
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;WebServerToolWindowFactoryState&quot;: &quot;false&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;master&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/Users/samueloneill/Desktop/SPECS_SPM&quot;,
+    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
+    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
+    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
+    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
+    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;terminal&quot;,
+    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
+      <recent name="$PROJECT_DIR$/trash"/>
       <recent name="$PROJECT_DIR$/nanonis_spm_specs_zurich"/>
       <recent name="$PROJECT_DIR$"/>
       <recent name="$PROJECT_DIR$/app"/>
     </key>
   </component>
   <component name="SharedIndexes">
     <attachedChunks>
       <set>
-        <option value="bundled-python-sdk-50da183f06c8-2887949eec09-com.jetbrains.pycharm.pro.sharedIndexes.bundled-PY-233.13135.95"/>
+        <option value="bundled-js-predefined-1d06a55b98c1-91d5c284f522-JavaScript-PY-241.15989.155"/>
+        <option value="bundled-python-sdk-babbdf50b680-7c6932dee5e4-com.jetbrains.pycharm.pro.sharedIndexes.bundled-PY-241.15989.155"/>
       </set>
     </attachedChunks>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="15c2ba6c-d2d2-4be3-8734-f6948252bab3" name="Changes" comment=""/>
@@ -118,15 +123,27 @@
       <workItem from="1702973757285" duration="17964000"/>
       <workItem from="1703148934423" duration="1290000"/>
       <workItem from="1703153800702" duration="9000"/>
       <workItem from="1704384069612" duration="7573000"/>
       <workItem from="1704971905061" duration="1256000"/>
       <workItem from="1705997429716" duration="1280000"/>
       <workItem from="1705999323816" duration="1900000"/>
-      <workItem from="1706716194950" duration="9921000"/>
+      <workItem from="1706716194950" duration="14401000"/>
+      <workItem from="1708674725554" duration="5588000"/>
+      <workItem from="1709127166659" duration="1214000"/>
+      <workItem from="1709709684945" duration="3093000"/>
+      <workItem from="1709809504510" duration="649000"/>
+      <workItem from="1710316516352" duration="1310000"/>
+      <workItem from="1710419613244" duration="3918000"/>
+      <workItem from="1710770784504" duration="1377000"/>
+      <workItem from="1715599843941" duration="2491000"/>
+      <workItem from="1715711021543" duration="10000"/>
+      <workItem from="1715844057773" duration="4904000"/>
+      <workItem from="1715854434663" duration="1952000"/>
+      <workItem from="1715860683155" duration="761000"/>
     </task>
     <task id="LOCAL-00001" summary="WorkingVersion">
       <option name="closed" value="true"/>
       <created>1699450207857</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -157,13 +174,13 @@
   </component>
   <component name="VcsManagerConfiguration">
     <option name="ADD_EXTERNAL_FILES_SILENTLY" value="true"/>
     <MESSAGE value="WorkingVersion"/>
     <option name="LAST_COMMIT_MESSAGE" value="WorkingVersion"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
+    <SUITE FILE_PATH="coverage/SPECS_SPM$test.coverage" NAME="test Coverage Results" MODIFIED="1715851483142" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="false" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/SPECS$NanonisClass.coverage" NAME="NanonisClass Coverage Results" MODIFIED="1700750127555" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/app"/>
     <SUITE FILE_PATH="coverage/SPECS$test.coverage" NAME="test Coverage Results" MODIFIED="1700823742419" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
-    <SUITE FILE_PATH="coverage/SPECS_SPM$test.coverage" NAME="test Coverage Results" MODIFIED="1707819121417" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/SPECS_SPM$NanonisClass.coverage" NAME="NanonisClass Coverage Results" MODIFIED="1702997230550" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/nanonis_spm_specs_zurich"/>
-    <SUITE FILE_PATH="coverage/SPECS$NanonisClass.coverage" NAME="NanonisClass Coverage Results" MODIFIED="1700750127555" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/app"/>
   </component>
 </project>
```

### Comparing `nanonis_spm_specs-0.0.4/nanonis_spm_specs/NanonisClass.py` & `nanonis_spm_specs-0.0.5/nanonis_spm_specs/NanonisClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import numpy as np
 
 
 class Nanonis:
     displayInfo = 0
 
     def __init__(self, connection):
-        # enter IP and Port of Nanonis server
         self.connection = connection
     def close(self):
         self.connection.close()
 
     def returnDebugInfo(self, displayInfo):
         self.displayInfo = displayInfo
```

### Comparing `nanonis_spm_specs-0.0.4/README.md` & `nanonis_spm_specs-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nanonis_spm_specs-0.0.4/PKG-INFO` & `nanonis_spm_specs-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nanonis_spm_specs
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for controlling Nanonis SPM software through python
 Author-email: Samuel O'Neill <samuel.oneill@specs-zurich.com>
 License-File: LICENSE.txt
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

