# Comparing `tmp/wp_enhanced-0.8.8.tar.gz` & `tmp/wp_enhanced-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wp_enhanced-0.8.8.tar", max compression
+gzip compressed data, was "wp_enhanced-0.8.9.tar", max compression
```

## Comparing `wp_enhanced-0.8.8.tar` & `wp_enhanced-0.8.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      593 2024-03-19 10:43:13.681546 wp_enhanced-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     1975 2024-03-05 10:44:56.655179 wp_enhanced-0.8.8/README.md
--rw-r--r--   0        0        0     4711 2024-03-14 08:22:26.062624 wp_enhanced-0.8.8/src/wpe/cli.py
--rw-r--r--   0        0        0     6947 2024-03-19 10:42:30.989172 wp_enhanced-0.8.8/src/wpe/core.py
--rw-r--r--   0        0        0     1778 2024-03-19 10:33:46.953081 wp_enhanced-0.8.8/src/wpe/hook_processor.py
--rw-r--r--   0        0        0    17482 2024-03-14 07:44:27.317521 wp_enhanced-0.8.8/src/wpe/parameter.py
--rw-r--r--   0        0        0     2287 2024-03-14 03:45:45.269746 wp_enhanced-0.8.8/src/wpe/pathman.py
--rw-r--r--   0        0        0     3683 2024-03-14 10:03:45.209189 wp_enhanced-0.8.8/src/wpe/project_config.py
--rw-r--r--   0        0        0     1298 2023-11-16 06:38:22.015600 wp_enhanced-0.8.8/src/wpe/templates/.wpe/hooks/post_build.py
--rw-r--r--   0        0        0     1988 2024-03-19 07:55:45.477030 wp_enhanced-0.8.8/src/wpe/templates/.wpe/wpe_project.toml
--rw-r--r--   0        0        0     3525 2024-01-18 03:32:51.913897 wp_enhanced-0.8.8/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp
--rw-r--r--   0        0        0     3456 2024-01-18 03:31:38.067723 wp_enhanced-0.8.8/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h
--rw-r--r--   0        0        0     2591 2023-11-09 12:01:43.217512 wp_enhanced-0.8.8/src/wpe/templates/WwisePlugin/ProjectName.xml
--rw-r--r--   0        0        0     2619 2023-11-09 12:01:43.210512 wp_enhanced-0.8.8/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp
--rw-r--r--   0        0        0     2212 2023-11-09 12:01:43.213515 wp_enhanced-0.8.8/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h
--rw-r--r--   0        0        0      781 2023-08-31 03:15:55.810608 wp_enhanced-0.8.8/src/wpe/util.py
--rw-r--r--   0        0        0     5720 2024-03-19 10:12:32.590345 wp_enhanced-0.8.8/src/wpe/wp_patch/build.py
--rw-r--r--   0        0        0     2847 2024-03-19 03:42:12.795265 wp_enhanced-0.8.8/src/wpe/wp_patch/common/command/android.py
--rw-r--r--   0        0        0     1409 2024-03-19 03:38:23.562202 wp_enhanced-0.8.8/src/wpe/wp_patch/common/platform/android.py
--rw-r--r--   0        0        0    11282 2023-12-20 09:52:04.364880 wp_enhanced-0.8.8/src/wpe/wp_patch/package.py
--rw-r--r--   0        0        0     2560 2024-03-14 08:02:19.221827 wp_enhanced-0.8.8/src/wpe/wp_patch/premake.py
--rw-r--r--   0        0        0    12877 2024-03-15 09:30:41.524075 wp_enhanced-0.8.8/src/wpe/wp_patch/premakePlugins.lua
--rw-r--r--   0        0        0     4024 2024-03-19 10:35:24.029781 wp_enhanced-0.8.8/src/wpe/wp_wrapper.py
--rw-r--r--   0        0        0     2688 1970-01-01 00:00:00.000000 wp_enhanced-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      593 2024-03-19 11:00:28.048604 wp_enhanced-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     1975 2024-03-05 10:44:56.655179 wp_enhanced-0.8.9/README.md
+-rw-r--r--   0        0        0     4711 2024-03-14 08:22:26.062624 wp_enhanced-0.8.9/src/wpe/cli.py
+-rw-r--r--   0        0        0     6947 2024-03-19 10:42:30.989172 wp_enhanced-0.8.9/src/wpe/core.py
+-rw-r--r--   0        0        0     1778 2024-03-19 10:33:46.953081 wp_enhanced-0.8.9/src/wpe/hook_processor.py
+-rw-r--r--   0        0        0    17482 2024-03-14 07:44:27.317521 wp_enhanced-0.8.9/src/wpe/parameter.py
+-rw-r--r--   0        0        0     2287 2024-03-14 03:45:45.269746 wp_enhanced-0.8.9/src/wpe/pathman.py
+-rw-r--r--   0        0        0     3810 2024-03-19 10:53:13.200056 wp_enhanced-0.8.9/src/wpe/project_config.py
+-rw-r--r--   0        0        0     1298 2023-11-16 06:38:22.015600 wp_enhanced-0.8.9/src/wpe/templates/.wpe/hooks/post_build.py
+-rw-r--r--   0        0        0     1988 2024-03-19 07:55:45.477030 wp_enhanced-0.8.9/src/wpe/templates/.wpe/wpe_project.toml
+-rw-r--r--   0        0        0     3525 2024-01-18 03:32:51.913897 wp_enhanced-0.8.9/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp
+-rw-r--r--   0        0        0     3456 2024-01-18 03:31:38.067723 wp_enhanced-0.8.9/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h
+-rw-r--r--   0        0        0     2591 2023-11-09 12:01:43.217512 wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectName.xml
+-rw-r--r--   0        0        0     2619 2023-11-09 12:01:43.210512 wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp
+-rw-r--r--   0        0        0     2212 2023-11-09 12:01:43.213515 wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h
+-rw-r--r--   0        0        0      781 2023-08-31 03:15:55.810608 wp_enhanced-0.8.9/src/wpe/util.py
+-rw-r--r--   0        0        0     5618 2024-03-19 10:51:33.313938 wp_enhanced-0.8.9/src/wpe/wp_patch/build.py
+-rw-r--r--   0        0        0     2847 2024-03-19 03:42:12.795265 wp_enhanced-0.8.9/src/wpe/wp_patch/common/command/android.py
+-rw-r--r--   0        0        0     1409 2024-03-19 03:38:23.562202 wp_enhanced-0.8.9/src/wpe/wp_patch/common/platform/android.py
+-rw-r--r--   0        0        0    11282 2023-12-20 09:52:04.364880 wp_enhanced-0.8.9/src/wpe/wp_patch/package.py
+-rw-r--r--   0        0        0     2560 2024-03-14 08:02:19.221827 wp_enhanced-0.8.9/src/wpe/wp_patch/premake.py
+-rw-r--r--   0        0        0    12877 2024-03-15 09:30:41.524075 wp_enhanced-0.8.9/src/wpe/wp_patch/premakePlugins.lua
+-rw-r--r--   0        0        0     3846 2024-03-19 10:51:33.314938 wp_enhanced-0.8.9/src/wpe/wp_wrapper.py
+-rw-r--r--   0        0        0     2688 1970-01-01 00:00:00.000000 wp_enhanced-0.8.9/PKG-INFO
```

### Comparing `wp_enhanced-0.8.8/pyproject.toml` & `wp_enhanced-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wp-enhanced"
-version = "0.8.8"
+version = "0.8.9"
 description = "Wrapper of `wp.py`. Easy to premake, build, and deploy wwise plugins."
 authors = ["tgalpha <tanalpha.zhy@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "wpe", from = "src" }
 ]
```

### Comparing `wp_enhanced-0.8.8/README.md` & `wp_enhanced-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/cli.py` & `wp_enhanced-0.8.9/src/wpe/cli.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/core.py` & `wp_enhanced-0.8.9/src/wpe/core.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/hook_processor.py` & `wp_enhanced-0.8.9/src/wpe/hook_processor.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/parameter.py` & `wp_enhanced-0.8.9/src/wpe/parameter.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/pathman.py` & `wp_enhanced-0.8.9/src/wpe/pathman.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/project_config.py` & `wp_enhanced-0.8.9/src/wpe/project_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os.path as osp
+import platform
 
 import kkpyutil as util
 
 # project
 from wpe.util import *
 from wpe.pathman import PathMan
 
@@ -75,15 +76,16 @@
             if line.startswith('version = '):
                 config_lines[i] = f'version = {new_version}\n'
                 break
         util.save_lines(self.pathMan.projConfig, config_lines)
         self.load()
 
     def target_platforms(self) -> list[PlatformTarget]:
-        return [PlatformTarget(target) for target in self.config['project']['targets']]
+        platform_targets_key = 'win_targets' if platform.system() == 'Windows' else 'mac_targets'
+        return [PlatformTarget(target) for target in self.config['project'][platform_targets_key]]
 
     def plugin_info(self) -> PluginInfo:
         return PluginInfo(self.config['plugin_info'])
 
     def has_parameters(self) -> bool:
         return 'parameters' in self.config
```

### Comparing `wp_enhanced-0.8.8/src/wpe/templates/.wpe/hooks/post_build.py` & `wp_enhanced-0.8.9/src/wpe/templates/.wpe/hooks/post_build.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/templates/.wpe/wpe_project.toml` & `wp_enhanced-0.8.9/src/wpe/templates/.wpe/wpe_project.toml`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp` & `wp_enhanced-0.8.9/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.cpp`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h` & `wp_enhanced-0.8.9/src/wpe/templates/SoundEnginePlugin/ProjectNameFXParams.h`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/templates/WwisePlugin/ProjectName.xml` & `wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectName.xml`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp` & `wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectNamePlugin.cpp`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h` & `wp_enhanced-0.8.9/src/wpe/templates/WwisePlugin/ProjectNamePlugin.h`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/util.py` & `wp_enhanced-0.8.9/src/wpe/util.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/wp_patch/build.py` & `wp_enhanced-0.8.9/src/wpe/wp_patch/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,17 @@
             exit_with_error("Invalid build hooks file {} at {}\n{}".format(args.build_hooks_file, PROJECT_ROOT, str(e)))
 
     # handle platform-specific command line specificites
     platform_info = platform_registry.get(args.platform)
 
     invalid_archs = set(args.archs) - set(platform_info.build.archs)
     if invalid_archs:
-        print("warning: Skipped invalid architecture(s) '{}' for target {}.".format(invalid_archs, platform_info.name))
+        print("error: Invalid architecture(s) '{}' for target {}.".format(invalid_archs, platform_info.name))
         print("supported architectures: {}".format(', '.join(platform_info.build.archs)))
-        args.archs = list(set(args.archs) - invalid_archs)
-        if not args.archs:
-            return 0
+        return 1
 
     if not args.toolset:
         if platform_info.build.require_toolset:
             print("error: 'Toolset' argument for target {} needs to be specified using -t or --toolset, -h for more details.".format(platform_info.name))
             print("supported toolsets: {}".format(', '.join(platform_info.build.toolsets)))
             return 1
     elif args.toolset not in platform_info.build.toolsets:
```

### Comparing `wp_enhanced-0.8.8/src/wpe/wp_patch/common/command/android.py` & `wp_enhanced-0.8.9/src/wpe/wp_patch/common/command/android.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/wp_patch/common/platform/android.py` & `wp_enhanced-0.8.9/src/wpe/wp_patch/common/platform/android.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/wp_patch/package.py` & `wp_enhanced-0.8.9/src/wpe/wp_patch/package.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/wp_patch/premake.py` & `wp_enhanced-0.8.9/src/wpe/wp_patch/premake.py`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/wp_patch/premakePlugins.lua` & `wp_enhanced-0.8.9/src/wpe/wp_patch/premakePlugins.lua`

 * *Files identical despite different names*

### Comparing `wp_enhanced-0.8.8/src/wpe/wp_wrapper.py` & `wp_enhanced-0.8.9/src/wpe/wp_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os
 import os.path as osp
 import platform
 
 import kkpyutil as util
 
 
@@ -76,17 +75,14 @@
             raise ValueError(f'Unknown subcommand: {subcommand}')
         return self.run(subcommand, *args[1:])
 
     @staticmethod
     @inject_wwise_sdk_for_android
     def build(*args):
         import wpe.wp_patch.build as wpe_build
-        if (plt := args[0]) not in wpe_build.SUPPORTED_PLATFORMS:
-            logging.info(f'Skip build for unsupported platform: {plt}')
-            return 0
         res = wpe_build.run(args)
         if res != 0:
             raise RuntimeError(f'Build failed. Exit code: {res}')
         return res
 
     def generate_bundle(self, *args):
         return self.run('generate_bundle', *args)
```

### Comparing `wp_enhanced-0.8.8/PKG-INFO` & `wp_enhanced-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wp-enhanced
-Version: 0.8.8
+Version: 0.8.9
 Summary: Wrapper of `wp.py`. Easy to premake, build, and deploy wwise plugins.
 Home-page: https://github.com/tgalpha/wp-enhanced
 License: MIT
 Author: tgalpha
 Author-email: tanalpha.zhy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

