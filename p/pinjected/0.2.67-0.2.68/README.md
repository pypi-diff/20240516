# Comparing `tmp/pinjected-0.2.67.tar.gz` & `tmp/pinjected-0.2.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.67.tar", max compression
+gzip compressed data, was "pinjected-0.2.68.tar", max compression
```

## Comparing `pinjected-0.2.67.tar` & `pinjected-0.2.68.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.67/LICENSE
--rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.67/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.67/pinjected/__main__.py
--rw-r--r--   0        0        0        0 2024-05-14 16:51:53.980366 pinjected-0.2.67/pinjected/compatibility/__init__.py
--rw-r--r--   0        0        0      753 2024-05-14 16:55:01.337952 pinjected-0.2.67/pinjected/compatibility/task_group.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.67/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.67/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.67/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.67/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5898 2024-05-13 08:52:30.783178 pinjected-0.2.67/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.67/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7866 2024-05-10 03:03:16.666241 pinjected-0.2.67/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.67/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.67/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-05-14 11:27:40.261061 pinjected-0.2.67/pinjected/di/decorators.py
--rw-r--r--   0        0        0    14572 2024-05-14 13:17:02.297068 pinjected-0.2.67/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.67/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.67/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.67/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.67/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.67/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    56046 2024-05-14 11:34:43.296359 pinjected-0.2.67/pinjected/di/injected.py
--rw-r--r--   0        0        0     2988 2024-05-14 06:50:46.840175 pinjected-0.2.67/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.67/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.67/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.67/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.67/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.67/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.67/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.67/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.67/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.67/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.67/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.67/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.67/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.67/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.67/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.67/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.67/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-05-14 10:11:59.767149 pinjected-0.2.67/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.67/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.67/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.67/pinjected/di/util.py
--rw-r--r--   0        0        0     1290 2024-05-10 07:03:44.040855 pinjected-0.2.67/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.67/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.67/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.67/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.67/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.67/pinjected/global_configs.py
--rw-r--r--   0        0        0     3039 2024-05-03 14:38:08.493688 pinjected-0.2.67/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.67/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.67/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.67/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.67/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.67/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.67/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.67/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.67/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.67/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.67/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.67/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.67/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.67/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.67/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.67/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.67/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.67/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.67/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.67/pinjected/providable.py
--rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.67/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.67/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.67/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.67/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.67/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9628 2024-05-14 16:55:01.331049 pinjected-0.2.67/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.67/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.67/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.67/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.67/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.67/pinjected/test_package/child/module_with.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.67/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.67/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.67/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.67/pinjected/v2/di.py
--rw-r--r--   0        0        0      616 2024-05-15 04:08:13.929515 pinjected-0.2.67/pinjected/v2/keys.py
--rw-r--r--   0        0        0      627 2024-05-10 02:30:28.919876 pinjected-0.2.67/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0    24767 2024-05-15 04:11:18.908390 pinjected-0.2.67/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    20026 2024-05-14 08:55:44.478760 pinjected-0.2.67/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.67/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.67/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.67/pinjected/with_context.py
--rw-r--r--   0        0        0      656 2024-05-15 04:11:22.402816 pinjected-0.2.67/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.67/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.68/LICENSE
+-rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.68/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.68/pinjected/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:51:53.980366 pinjected-0.2.68/pinjected/compatibility/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-14 16:55:01.337952 pinjected-0.2.68/pinjected/compatibility/task_group.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.68/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.68/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.68/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.68/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5898 2024-05-13 08:52:30.783178 pinjected-0.2.68/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.68/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7866 2024-05-10 03:03:16.666241 pinjected-0.2.68/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.68/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.68/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-05-14 11:27:40.261061 pinjected-0.2.68/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    14572 2024-05-14 13:17:02.297068 pinjected-0.2.68/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.68/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.68/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.68/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.68/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.68/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    56168 2024-05-15 06:42:25.667673 pinjected-0.2.68/pinjected/di/injected.py
+-rw-r--r--   0        0        0     2988 2024-05-14 06:50:46.840175 pinjected-0.2.68/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.68/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.68/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.68/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.68/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.68/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.68/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.68/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.68/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.68/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.68/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.68/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.68/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.68/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.68/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.68/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.68/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-05-14 10:11:59.767149 pinjected-0.2.68/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.68/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.68/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.68/pinjected/di/util.py
+-rw-r--r--   0        0        0     1290 2024-05-10 07:03:44.040855 pinjected-0.2.68/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.68/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.68/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.68/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.68/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.68/pinjected/global_configs.py
+-rw-r--r--   0        0        0     3039 2024-05-03 14:38:08.493688 pinjected-0.2.68/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.68/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.68/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.68/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.68/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.68/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.68/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.68/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.68/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.68/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.68/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.68/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.68/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.68/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.68/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.68/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.68/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.68/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.68/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.68/pinjected/providable.py
+-rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.68/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.68/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.68/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.68/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.68/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9732 2024-05-15 05:20:27.364514 pinjected-0.2.68/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.68/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.68/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.68/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.68/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.68/pinjected/test_package/child/module_with.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.68/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.68/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.68/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.68/pinjected/v2/di.py
+-rw-r--r--   0        0        0      616 2024-05-15 04:08:13.929515 pinjected-0.2.68/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      627 2024-05-10 02:30:28.919876 pinjected-0.2.68/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0    24800 2024-05-15 05:09:47.881318 pinjected-0.2.68/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    20026 2024-05-14 08:55:44.478760 pinjected-0.2.68/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.68/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.68/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.68/pinjected/with_context.py
+-rw-r--r--   0        0        0      627 2024-05-15 06:42:40.052436 pinjected-0.2.68/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.68/PKG-INFO
```

### Comparing `pinjected-0.2.67/LICENSE` & `pinjected-0.2.68/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/compatibility/task_group.py` & `pinjected-0.2.68/pinjected/compatibility/task_group.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/decoration.py` & `pinjected-0.2.68/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/demo.py` & `pinjected-0.2.68/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/app_designed.py` & `pinjected-0.2.68/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/app_injected.py` & `pinjected-0.2.68/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/applicative.py` & `pinjected-0.2.68/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/ast.py` & `pinjected-0.2.68/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/decorators.py` & `pinjected-0.2.68/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/design.py` & `pinjected-0.2.68/pinjected/di/design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/designed.py` & `pinjected-0.2.68/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.68/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/graph.py` & `pinjected-0.2.68/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/injected.py` & `pinjected-0.2.68/pinjected/di/injected.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from copy import copy
 from dataclasses import dataclass, field
 from inspect import Traceback, iscoroutinefunction
 from pathlib import Path
 from typing import List, Generic, Union, Callable, TypeVar, Tuple, Set, Dict, Any, Awaitable
 
 from frozendict import frozendict
-from loguru import logger
 from makefun import create_function
 from returns.result import safe
 
 from pinjected.di.injected_analysis import get_instance_origin
 from pinjected.di.proxiable import DelegatedVar
 
 T, U = TypeVar("T"), TypeVar("U")
@@ -506,14 +505,15 @@
             frame = sys._getframe().f_back.f_back
             mod = frame.f_globals["__name__"]
             name = frame.f_code.co_filename
             # return f"{mod.replace('.', '_')}_L_{name}".replace("<", "__").replace(">", "__")
             return mod, name
         except Exception as e:
             # from loguru import logger
+            from loguru import logger
             logger.warning(f"failed to get name of the injected location, due to {e}")
             return f"__unknown_module__maybe_due_to_pickling__", "unknown_location"
 
     @staticmethod
     def pure(value):
         res = InjectedPure(value)
         # I need to set the file that called this function.
@@ -756,14 +756,15 @@
     program: Injected[T]
     program_dependencies: List[Injected]
 
     def __post_init__(self):
         self.program = Injected.ensure_injected(self.program)
 
         async def impl(t):
+            from loguru import logger
             resolver, cache, *deps = t
             logger.info(f"Checking for cache with deps:{deps}")
             sha256_key = hashlib.sha256(str(deps).encode()).hexdigest()
             hash_key = sha256_key
             if hash_key not in cache:
                 logger.info(f"Cache miss for {deps}")
                 data = await resolver[self.program]
@@ -1061,14 +1062,15 @@
 
     def __init__(self,
                  original_function,
                  target_function: Callable,
                  kwargs_mapping: Dict[str, Union[str, type, Callable, Injected, DelegatedVar]]
                  ):
         # I think we need to know where this class is instantiated outside of pinjected_package
+        from loguru import logger
         self.origin_frame = get_instance_origin("pinjected")
         self.original_function = original_function
         super().__init__()
         assert not isinstance(target_function, (Injected, DelegatedVar))
         assert callable(target_function)
         self.target_function = target_function
         assert inspect.iscoroutinefunction(self.target_function), f"{self.target_function} is not a coroutine function"
@@ -1092,14 +1094,15 @@
     def override_mapping(self, **kwargs: Union[str, type, Callable, Injected]):
         return InjectedFunction(self.target_function, {**self.kwargs_mapping, **kwargs})
 
     def get_provider(self):
         signature = self.get_signature()
 
         async def impl(**kwargs):
+            from loguru import logger
             deps = dict()
 
             async def update(key):
                 if key not in deps:
                     if key in self.kwargs_mapping:
                         mapped = self.kwargs_mapping[key]
                     else:
```

### Comparing `pinjected-0.2.67/pinjected/di/injected_analysis.py` & `pinjected-0.2.68/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/modular_injected.py` & `pinjected-0.2.68/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/overload_experimental.py` & `pinjected-0.2.68/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/proxiable.py` & `pinjected-0.2.68/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/session.py` & `pinjected-0.2.68/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/sessioned.py` & `pinjected-0.2.68/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/static_proxy.py` & `pinjected-0.2.68/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.68/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/test_graph.py` & `pinjected-0.2.68/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/test_injected.py` & `pinjected-0.2.68/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/tools/add_overload.py` & `pinjected-0.2.68/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/di/util.py` & `pinjected-0.2.68/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/exceptions.py` & `pinjected-0.2.68/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.68/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.68/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/graph_inspection.py` & `pinjected-0.2.68/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/helper_structure.py` & `pinjected-0.2.68/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/helpers.py` & `pinjected-0.2.68/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.68/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.68/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/ide_supports/default_design.py` & `pinjected-0.2.68/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.68/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.68/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/main_impl.py` & `pinjected-0.2.68/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/maybe_patch.py` & `pinjected-0.2.68/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/module_helper.py` & `pinjected-0.2.68/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/module_inspector.py` & `pinjected-0.2.68/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/module_var_path.py` & `pinjected-0.2.68/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/notification.py` & `pinjected-0.2.68/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/nx_graph_util.py` & `pinjected-0.2.68/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/run_config_utils.py` & `pinjected-0.2.68/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/run_config_utils_v2.py` & `pinjected-0.2.68/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/run_helpers/config.py` & `pinjected-0.2.68/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.68/pinjected/run_helpers/run_injected.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,17 @@
         # trace = traceback.format_exc()
         # Path(f"run_failed_{var_path}.err.log").write_text(str(e) + "\n" + trace)
         # from rich.console import Console
         # console = Console()
         # console.print_exception(show_locals=False)
         raise e
     notify(f"Run result:\n{str(res)[:100]}")
+    logger.info(f"run_injected result:\n{res}")
     if return_result:
+        logger.info(f"delegating the result to fire..")
         return res
 
 
 def find_dot_pinjected():
     # 1. load the .pinjected.py at home directory
     # 2. load the .pinjected.py at current directory
     # hmm, we are currently only looking at the home and current directory.
```

### Comparing `pinjected-0.2.67/pinjected/runnables.py` & `pinjected-0.2.68/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/test_package/__init__.py` & `pinjected-0.2.68/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/test_package/child/module1.py` & `pinjected-0.2.68/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/v2/ainjected.py` & `pinjected-0.2.68/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/v2/binds.py` & `pinjected-0.2.68/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/v2/di.py` & `pinjected-0.2.68/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/v2/keys.py` & `pinjected-0.2.68/pinjected/v2/keys.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/v2/provide_context.py` & `pinjected-0.2.68/pinjected/v2/provide_context.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pinjected/v2/resolver.py` & `pinjected-0.2.68/pinjected/v2/resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
         self.total_status[event.key] = ResolveStatus(event.key, "provide", "waiting", datetime.datetime.now(), None)
 
     def on_provide(self, event: ProvideEvent):
         self.total_status[event.key].status = "provided"
         self.request_status[event.key] = "provided"
         data_str = str(event.data)[:50]
         data_str = self.clean_msg(data_str)
-        self.logger.info(f"{event.cxt.trace_str} := {data_str}")
+        self.logger.info(f"{self.clean_msg(event.cxt.trace_str)} := {data_str}")
         # self.logger.info(f"{self.provider_status_string()}")
 
     def on_deps_ready(self, event: DepsReadyEvent):
         self.total_status[event.key].status = "running"
         self.request_status[event.key] = "running"
         self.logger.info(f"{self.clean_msg(event.cxt.trace_str)}")
         # self.logger.info(f"{self.provider_status_string()}")
@@ -577,20 +577,20 @@
                 # self.logger.debug(f"eval\t-> <magenta>{expr}</magenta>")
         # self.logger.info(f"\n{self.eval_status_string()}")
 
     def expr_repr(self,e):
         msg = show_expr(e)
         msg = self.clean_msg(msg)
         if len(msg) >= 50:
-            msg = msg[:50] + "..."
+            msg = msg[:25] + "..." + msg[-25:]
         return msg
 
     def on_eval_result(self, event):
         expr = self.expr_repr(event.expr)
-        res_msg = self.clean_msg(str(event.result))
+        res_msg = self.clean_msg(str(event.result)[:50])
         match event.expr:
             case Cache(_):
                 return
             case Call():
 
                 self.logger.success(f"call\t<- <magenta>{expr}</magenta>\t:= {res_msg}")
             case UnaryOp('await', _):
```

### Comparing `pinjected-0.2.67/pinjected/visualize_di.py` & `pinjected-0.2.68/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.67/pyproject.toml` & `pinjected-0.2.68/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-[project]
-dependencies = []
-
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.67"
+version = "0.2.68"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "*"
```

### Comparing `pinjected-0.2.67/PKG-INFO` & `pinjected-0.2.68/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.67
+Version: 0.2.68
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

