# Comparing `tmp/conan-2.3.0.tar.gz` & `tmp/conan-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan-2.3.0.tar", last modified: Mon May  6 16:43:40 2024, max compression
+gzip compressed data, was "dist/conan-2.3.1.tar", last modified: Thu May 16 17:40:58 2024, max compression
```

## Comparing `conan-2.3.0.tar` & `conan-2.3.1.tar`

### file list

```diff
@@ -1,376 +1,376 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.742570 conan-2.3.0/
--rw-r--r--   0 root         (0) root         (0)     1084 2024-05-06 16:43:32.000000 conan-2.3.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-06 16:43:32.000000 conan-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8377 2024-05-06 16:43:40.743570 conan-2.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6118 2024-05-06 16:43:32.000000 conan-2.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.703566 conan-2.3.0/conan/
--rw-r--r--   0 root         (0) root         (0)      165 2024-05-06 16:43:32.000000 conan-2.3.0/conan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.704566 conan-2.3.0/conan/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2455 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/conan_api.py
--rw-r--r--   0 root         (0) root         (0)    13040 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/model.py
--rw-r--r--   0 root         (0) root         (0)     9460 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.706567 conan-2.3.0/conan/api/subapi/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13263 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/cache.py
--rw-r--r--   0 root         (0) root         (0)      756 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/command.py
--rw-r--r--   0 root         (0) root         (0)     9255 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/config.py
--rw-r--r--   0 root         (0) root         (0)     4793 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/download.py
--rw-r--r--   0 root         (0) root         (0)     2714 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/export.py
--rw-r--r--   0 root         (0) root         (0)    11805 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/graph.py
--rw-r--r--   0 root         (0) root         (0)     3961 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/install.py
--rw-r--r--   0 root         (0) root         (0)    17548 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/list.py
--rw-r--r--   0 root         (0) root         (0)     5524 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/local.py
--rw-r--r--   0 root         (0) root         (0)     4808 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/lockfile.py
--rw-r--r--   0 root         (0) root         (0)     5193 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/new.py
--rw-r--r--   0 root         (0) root         (0)     7441 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/profiles.py
--rw-r--r--   0 root         (0) root         (0)    13412 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/remotes.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/remove.py
--rw-r--r--   0 root         (0) root         (0)     1117 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/search.py
--rw-r--r--   0 root         (0) root         (0)     6670 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.707567 conan-2.3.0/conan/cli/
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7430 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/args.py
--rw-r--r--   0 root         (0) root         (0)    12224 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     8279 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.710567 conan-2.3.0/conan/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3994 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/build.py
--rw-r--r--   0 root         (0) root         (0)     7489 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/cache.py
--rw-r--r--   0 root         (0) root         (0)     4609 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)    10989 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/create.py
--rw-r--r--   0 root         (0) root         (0)     3252 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/download.py
--rw-r--r--   0 root         (0) root         (0)     3157 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/editable.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/export.py
--rw-r--r--   0 root         (0) root         (0)     5798 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/export_pkg.py
--rw-r--r--   0 root         (0) root         (0)    21213 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/graph.py
--rw-r--r--   0 root         (0) root         (0)     2495 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/inspect.py
--rw-r--r--   0 root         (0) root         (0)     4704 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)    13371 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/list.py
--rw-r--r--   0 root         (0) root         (0)     7511 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/lock.py
--rw-r--r--   0 root         (0) root         (0)     4260 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/new.py
--rw-r--r--   0 root         (0) root         (0)     3696 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/pkglist.py
--rw-r--r--   0 root         (0) root         (0)     3553 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/profile.py
--rw-r--r--   0 root         (0) root         (0)    12835 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/remote.py
--rw-r--r--   0 root         (0) root         (0)     6487 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/search.py
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/source.py
--rw-r--r--   0 root         (0) root         (0)     4411 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/test.py
--rw-r--r--   0 root         (0) root         (0)     6871 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/upload.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      490 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/exit_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.710567 conan-2.3.0/conan/cli/formatters/
--rw-r--r--   0 root         (0) root         (0)      158 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.710567 conan-2.3.0/conan/cli/formatters/graph/
--rw-r--r--   0 root         (0) root         (0)      110 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5663 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/graph_info_text.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/info_graph_dot.py
--rw-r--r--   0 root         (0) root         (0)    15953 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/info_graph_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.711567 conan-2.3.0/conan/cli/formatters/list/
--rw-r--r--   0 root         (0) root         (0)       37 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4612 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/list/binary_html_table.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/list/list.py
--rw-r--r--   0 root         (0) root         (0)    12834 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/list/search_table_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.711567 conan-2.3.0/conan/cli/printers/
--rw-r--r--   0 root         (0) root         (0)      331 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/printers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6412 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/printers/graph.py
--rw-r--r--   0 root         (0) root         (0)      139 2024-05-06 16:43:32.000000 conan-2.3.0/conan/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.712567 conan-2.3.0/conan/internal/
--rw-r--r--   0 root         (0) root         (0)      419 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.712567 conan-2.3.0/conan/internal/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20992 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/detect_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.714568 conan-2.3.0/conan/internal/api/new/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/alias_new.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/autoools_exe.py
--rw-r--r--   0 root         (0) root         (0)     3850 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/autotools_lib.py
--rw-r--r--   0 root         (0) root         (0)     2916 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/basic.py
--rw-r--r--   0 root         (0) root         (0)     2041 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/bazel_exe.py
--rw-r--r--   0 root         (0) root         (0)     4565 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/bazel_lib.py
--rw-r--r--   0 root         (0) root         (0)     2932 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/cmake_exe.py
--rw-r--r--   0 root         (0) root         (0)     8212 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/cmake_lib.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/local_recipes_index.py
--rw-r--r--   0 root         (0) root         (0)     2334 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/meson_exe.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/meson_lib.py
--rw-r--r--   0 root         (0) root         (0)     2207 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/msbuild_exe.py
--rw-r--r--   0 root         (0) root         (0)    12307 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/msbuild_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.714568 conan-2.3.0/conan/internal/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11189 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     4083 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/conan_reference_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.715567 conan-2.3.0/conan/internal/cache/db/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3949 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/cache_database.py
--rw-r--r--   0 root         (0) root         (0)     9222 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/packages_table.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/recipes_table.py
--rw-r--r--   0 root         (0) root         (0)     2639 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/table.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/home_paths.py
--rw-r--r--   0 root         (0) root         (0)     3114 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/conan_app.py
--rw-r--r--   0 root         (0) root         (0)     5045 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/deploy.py
--rw-r--r--   0 root         (0) root         (0)     3098 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/integrity_check.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/internal_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.715567 conan-2.3.0/conan/internal/runner/
--rw-r--r--   0 root         (0) root         (0)      302 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14530 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/runner/docker.py
--rw-r--r--   0 root         (0) root         (0)    12370 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/runner/ssh.py
--rw-r--r--   0 root         (0) root         (0)     6712 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/runner/wsl.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/upload_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.716568 conan-2.3.0/conan/tools/
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.716568 conan-2.3.0/conan/tools/android/
--rw-r--r--   0 root         (0) root         (0)       50 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/android/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1138 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/android/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.716568 conan-2.3.0/conan/tools/apple/
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12880 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/apple.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/xcodebuild.py
--rw-r--r--   0 root         (0) root         (0)    16239 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/xcodedeps.py
--rw-r--r--   0 root         (0) root         (0)     5754 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/xcodetoolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.717568 conan-2.3.0/conan/tools/build/
--rw-r--r--   0 root         (0) root         (0)     4190 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11121 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/cppstd.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/cpu.py
--rw-r--r--   0 root         (0) root         (0)     2302 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/cross_building.py
--rw-r--r--   0 root         (0) root         (0)    16208 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/flags.py
--rw-r--r--   0 root         (0) root         (0)      563 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/stdcpp_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.718568 conan-2.3.0/conan/tools/cmake/
--rw-r--r--   0 root         (0) root         (0)      217 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14319 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.718568 conan-2.3.0/conan/tools/cmake/cmakedeps/
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11138 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/cmakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.719568 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/
--rw-r--r--   0 root         (0) root         (0)     3944 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4563 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/config.py
--rw-r--r--   0 root         (0) root         (0)     4061 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/config_version.py
--rw-r--r--   0 root         (0) root         (0)     5956 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/macros.py
--rw-r--r--   0 root         (0) root         (0)    14989 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/target_configuration.py
--rw-r--r--   0 root         (0) root         (0)    20350 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/target_data.py
--rw-r--r--   0 root         (0) root         (0)     3656 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/targets.py
--rw-r--r--   0 root         (0) root         (0)     4746 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/layout.py
--rw-r--r--   0 root         (0) root         (0)    16807 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/presets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.719568 conan-2.3.0/conan/tools/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/toolchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45120 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/toolchain/blocks.py
--rw-r--r--   0 root         (0) root         (0)    13776 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/toolchain/toolchain.py
--rw-r--r--   0 root         (0) root         (0)      171 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.720568 conan-2.3.0/conan/tools/env/
--rw-r--r--   0 root         (0) root         (0)      168 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26546 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/env/environment.py
--rw-r--r--   0 root         (0) root         (0)     3601 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/env/virtualbuildenv.py
--rw-r--r--   0 root         (0) root         (0)     3561 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/env/virtualrunenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.721568 conan-2.3.0/conan/tools/files/
--rw-r--r--   0 root         (0) root         (0)      535 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2672 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/conandata.py
--rw-r--r--   0 root         (0) root         (0)     7429 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/copy_pattern.py
--rw-r--r--   0 root         (0) root         (0)    24002 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/files.py
--rw-r--r--   0 root         (0) root         (0)     4177 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/packager.py
--rw-r--r--   0 root         (0) root         (0)     6540 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/patches.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.721568 conan-2.3.0/conan/tools/files/symlinks/
--rw-r--r--   0 root         (0) root         (0)      148 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/symlinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/symlinks/symlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.722568 conan-2.3.0/conan/tools/gnu/
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6173 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/autotools.py
--rw-r--r--   0 root         (0) root         (0)     2962 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/autotoolsdeps.py
--rw-r--r--   0 root         (0) root         (0)    13681 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/autotoolstoolchain.py
--rw-r--r--   0 root         (0) root         (0)     3986 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/get_gnu_triplet.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/gnudeps_flags.py
--rw-r--r--   0 root         (0) root         (0)    13632 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/gnutoolchain.py
--rw-r--r--   0 root         (0) root         (0)    27066 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/makedeps.py
--rw-r--r--   0 root         (0) root         (0)     4290 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/pkgconfig.py
--rw-r--r--   0 root         (0) root         (0)    19100 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/pkgconfigdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.723568 conan-2.3.0/conan/tools/google/
--rw-r--r--   0 root         (0) root         (0)      201 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3387 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/bazel.py
--rw-r--r--   0 root         (0) root         (0)    23672 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/bazeldeps.py
--rw-r--r--   0 root         (0) root         (0)     1188 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/layout.py
--rw-r--r--   0 root         (0) root         (0)     8113 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.723568 conan-2.3.0/conan/tools/intel/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/intel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6498 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/intel/intel_cc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.723568 conan-2.3.0/conan/tools/layout/
--rw-r--r--   0 root         (0) root         (0)      605 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/layout/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.724568 conan-2.3.0/conan/tools/meson/
--rw-r--r--   0 root         (0) root         (0)       98 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4702 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/meson/helpers.py
--rw-r--r--   0 root         (0) root         (0)     5269 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/meson/meson.py
--rw-r--r--   0 root         (0) root         (0)    25007 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/meson/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.725568 conan-2.3.0/conan/tools/microsoft/
--rw-r--r--   0 root         (0) root         (0)      558 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1335 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/layout.py
--rw-r--r--   0 root         (0) root         (0)     3312 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/msbuild.py
--rw-r--r--   0 root         (0) root         (0)    19246 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/msbuilddeps.py
--rw-r--r--   0 root         (0) root         (0)     2967 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/nmakedeps.py
--rw-r--r--   0 root         (0) root         (0)     4984 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/nmaketoolchain.py
--rw-r--r--   0 root         (0) root         (0)      593 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/subsystems.py
--rw-r--r--   0 root         (0) root         (0)    11139 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/toolchain.py
--rw-r--r--   0 root         (0) root         (0)    14962 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.725568 conan-2.3.0/conan/tools/premake/
--rw-r--r--   0 root         (0) root         (0)      103 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/premake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/premake/premake.py
--rw-r--r--   0 root         (0) root         (0)    10534 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/premake/premakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.726569 conan-2.3.0/conan/tools/qbs/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/qbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2901 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/qbs/qbs.py
--rw-r--r--   0 root         (0) root         (0)     9897 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/qbs/qbsprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.726569 conan-2.3.0/conan/tools/scm/
--rw-r--r--   0 root         (0) root         (0)       77 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/scm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13281 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/scm/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.726569 conan-2.3.0/conan/tools/scons/
--rw-r--r--   0 root         (0) root         (0)       50 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/scons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2362 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/scons/sconsdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.726569 conan-2.3.0/conan/tools/system/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17993 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/system/package_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.703566 conan-2.3.0/conan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8377 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9839 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.727569 conan-2.3.0/conans/
--rw-r--r--   0 root         (0) root         (0)      201 2024-05-06 16:43:32.000000 conan-2.3.0/conans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.729569 conan-2.3.0/conans/client/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.729569 conan-2.3.0/conans/client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4924 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     2033 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cache/editable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.730569 conan-2.3.0/conans/client/cmd/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cmd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7883 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cmd/export.py
--rw-r--r--   0 root         (0) root         (0)    12622 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cmd/uploader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.730569 conan-2.3.0/conans/client/conanfile/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/build.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/configure.py
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/implementations.py
--rw-r--r--   0 root         (0) root         (0)     2138 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.731569 conan-2.3.0/conans/client/conf/
--rw-r--r--   0 root         (0) root         (0)     7449 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7919 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/config_installer.py
--rw-r--r--   0 root         (0) root         (0)     1419 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/detect.py
--rw-r--r--   0 root         (0) root         (0)     4582 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/detect_vs.py
--rw-r--r--   0 root         (0) root         (0)     1270 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/required_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.731569 conan-2.3.0/conans/client/downloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/downloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10333 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/downloaders/caching_file_downloader.py
--rw-r--r--   0 root         (0) root         (0)     5595 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/downloaders/download_cache.py
--rw-r--r--   0 root         (0) root         (0)     6731 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/downloaders/file_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.732569 conan-2.3.0/conans/client/generators/
--rw-r--r--   0 root         (0) root         (0)    10455 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/generators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.733569 conan-2.3.0/conans/client/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/build_mode.py
--rw-r--r--   0 root         (0) root         (0)     5532 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     4451 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/compute_pid.py
--rw-r--r--   0 root         (0) root         (0)    15453 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    23117 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/graph_binaries.py
--rw-r--r--   0 root         (0) root         (0)    21937 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/graph_builder.py
--rw-r--r--   0 root         (0) root         (0)     2924 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/graph_error.py
--rw-r--r--   0 root         (0) root         (0)    21344 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/install_graph.py
--rw-r--r--   0 root         (0) root         (0)     5186 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/profile_node_definer.py
--rw-r--r--   0 root         (0) root         (0)     1895 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/provides.py
--rw-r--r--   0 root         (0) root         (0)     7221 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/proxy.py
--rw-r--r--   0 root         (0) root         (0)     6480 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/python_requires.py
--rw-r--r--   0 root         (0) root         (0)     5326 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/range_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2595 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/hook_manager.py
--rw-r--r--   0 root         (0) root         (0)    21840 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/installer.py
--rw-r--r--   0 root         (0) root         (0)    17007 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/loader.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/loader_txt.py
--rw-r--r--   0 root         (0) root         (0)     5413 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/migrations.py
--rw-r--r--   0 root         (0) root         (0)     1971 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/pkg_sign.py
--rw-r--r--   0 root         (0) root         (0)    17816 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/profile_loader.py
--rw-r--r--   0 root         (0) root         (0)    14595 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/remote_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.735570 conan-2.3.0/conans/client/rest/
--rw-r--r--   0 root         (0) root         (0)      838 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5837 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/auth_manager.py
--rw-r--r--   0 root         (0) root         (0)     6132 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/client_routes.py
--rw-r--r--   0 root         (0) root         (0)     6936 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/conan_requester.py
--rw-r--r--   0 root         (0) root         (0)     3945 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/file_uploader.py
--rw-r--r--   0 root         (0) root         (0)     2650 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/remote_credentials.py
--rw-r--r--   0 root         (0) root         (0)     5424 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/rest_client.py
--rw-r--r--   0 root         (0) root         (0)     9776 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/rest_client_common.py
--rw-r--r--   0 root         (0) root         (0)    14934 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/rest_client_v2.py
--rw-r--r--   0 root         (0) root         (0)     9149 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest_client_local_recipe_index.py
--rw-r--r--   0 root         (0) root         (0)     3903 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.735570 conan-2.3.0/conans/client/store/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4205 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/store/localdb.py
--rw-r--r--   0 root         (0) root         (0)     8798 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/subsystems.py
--rw-r--r--   0 root         (0) root         (0)     4223 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/userio.py
--rwxr-xr-x   0 root         (0) root         (0)      118 2024-05-06 16:43:32.000000 conan-2.3.0/conans/conan.py
--rw-r--r--   0 root         (0) root         (0)      699 2024-05-06 16:43:32.000000 conan-2.3.0/conans/conan_server.py
--rw-r--r--   0 root         (0) root         (0)     7419 2024-05-06 16:43:32.000000 conan-2.3.0/conans/errors.py
--rw-r--r--   0 root         (0) root         (0)     3290 2024-05-06 16:43:32.000000 conan-2.3.0/conans/migrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.737570 conan-2.3.0/conans/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20506 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/build_info.py
--rw-r--r--   0 root         (0) root         (0)    12678 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/conan_file.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/conanfile_interface.py
--rw-r--r--   0 root         (0) root         (0)    32656 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/conf.py
--rw-r--r--   0 root         (0) root         (0)     6302 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/dependencies.py
--rw-r--r--   0 root         (0) root         (0)    13116 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/graph_lock.py
--rw-r--r--   0 root         (0) root         (0)    15205 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/info.py
--rw-r--r--   0 root         (0) root         (0)     5423 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/layout.py
--rw-r--r--   0 root         (0) root         (0)     4883 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/manifest.py
--rw-r--r--   0 root         (0) root         (0)    17829 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/options.py
--rw-r--r--   0 root         (0) root         (0)     3861 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/package_ref.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/pkg_type.py
--rw-r--r--   0 root         (0) root         (0)     7155 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/profile.py
--rw-r--r--   0 root         (0) root         (0)     8088 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/recipe_ref.py
--rw-r--r--   0 root         (0) root         (0)    24648 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/requires.py
--rw-r--r--   0 root         (0) root         (0)     2171 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/rest_routes.py
--rw-r--r--   0 root         (0) root         (0)    14049 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/settings.py
--rw-r--r--   0 root         (0) root         (0)     6184 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/version.py
--rw-r--r--   0 root         (0) root         (0)     8643 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/version_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.738570 conan-2.3.0/conans/paths/
--rw-r--r--   0 root         (0) root         (0)     2198 2024-05-06 16:43:32.000000 conan-2.3.0/conans/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      251 2024-05-06 16:43:32.000000 conan-2.3.0/conans/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      191 2024-05-06 16:43:32.000000 conan-2.3.0/conans/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-06 16:43:32.000000 conan-2.3.0/conans/requirements_runner.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-06 16:43:32.000000 conan-2.3.0/conans/requirements_server.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.738570 conan-2.3.0/conans/search/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-05-06 16:43:32.000000 conan-2.3.0/conans/search/query_parse.py
--rw-r--r--   0 root         (0) root         (0)     4474 2024-05-06 16:43:32.000000 conan-2.3.0/conans/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.738570 conan-2.3.0/conans/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.739570 conan-2.3.0/conans/test/assets/
--rw-r--r--   0 root         (0) root         (0)      510 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1651 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/autotools.py
--rw-r--r--   0 root         (0) root         (0)     3753 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/cmake.py
--rw-r--r--   0 root         (0) root         (0)    17307 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/genconanfile.py
--rw-r--r--   0 root         (0) root         (0)     6352 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/pkg_cmake.py
--rw-r--r--   0 root         (0) root         (0)     6008 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/sources.py
--rw-r--r--   0 root         (0) root         (0)    11972 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/visual_project_files.py
--rw-r--r--   0 root         (0) root         (0)    13188 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.741570 conan-2.3.0/conans/test/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4868 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     2806 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/file_server.py
--rw-r--r--   0 root         (0) root         (0)     4155 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/mocks.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     2038 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/scm.py
--rw-r--r--   0 root         (0) root         (0)     3858 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/server_launcher.py
--rw-r--r--   0 root         (0) root         (0)     3187 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/test_files.py
--rw-r--r--   0 root         (0) root         (0)    37579 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.742570 conan-2.3.0/conans/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/config_parser.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/dates.py
--rw-r--r--   0 root         (0) root         (0)     1301 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     1396 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/env.py
--rw-r--r--   0 root         (0) root         (0)    11974 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/files.py
--rw-r--r--   0 root         (0) root         (0)     3657 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/locks.py
--rw-r--r--   0 root         (0) root         (0)     3729 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/runners.py
--rw-r--r--   0 root         (0) root         (0)     1416 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/sha.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/windows.py
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-06 16:43:32.000000 conan-2.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-06 16:43:40.743570 conan-2.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5218 2024-05-06 16:43:32.000000 conan-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.556604 conan-2.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-05-16 17:40:48.000000 conan-2.3.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-16 17:40:48.000000 conan-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8377 2024-05-16 17:40:58.556604 conan-2.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6118 2024-05-16 17:40:48.000000 conan-2.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.512600 conan-2.3.1/conan/
+-rw-r--r--   0 root         (0) root         (0)      165 2024-05-16 17:40:48.000000 conan-2.3.1/conan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.513600 conan-2.3.1/conan/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/conan_api.py
+-rw-r--r--   0 root         (0) root         (0)    13040 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/model.py
+-rw-r--r--   0 root         (0) root         (0)     9460 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.516600 conan-2.3.1/conan/api/subapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13263 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/cache.py
+-rw-r--r--   0 root         (0) root         (0)      756 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/command.py
+-rw-r--r--   0 root         (0) root         (0)     9255 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/config.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/download.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/export.py
+-rw-r--r--   0 root         (0) root         (0)    11805 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3961 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/install.py
+-rw-r--r--   0 root         (0) root         (0)    17548 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/list.py
+-rw-r--r--   0 root         (0) root         (0)     5596 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/local.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/lockfile.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/new.py
+-rw-r--r--   0 root         (0) root         (0)     7441 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    13412 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/remotes.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/search.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2024-05-16 17:40:48.000000 conan-2.3.1/conan/api/subapi/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.516600 conan-2.3.1/conan/cli/
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7430 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)    12224 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8279 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.520601 conan-2.3.1/conan/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/build.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)    10989 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/create.py
+-rw-r--r--   0 root         (0) root         (0)     3252 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/editable.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/export.py
+-rw-r--r--   0 root         (0) root         (0)     5914 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/export_pkg.py
+-rw-r--r--   0 root         (0) root         (0)    21213 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     4704 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)    13371 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/list.py
+-rw-r--r--   0 root         (0) root         (0)     7511 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/lock.py
+-rw-r--r--   0 root         (0) root         (0)     4260 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/new.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/pkglist.py
+-rw-r--r--   0 root         (0) root         (0)     3553 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/profile.py
+-rw-r--r--   0 root         (0) root         (0)    12835 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/remote.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/source.py
+-rw-r--r--   0 root         (0) root         (0)     4411 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     6871 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/upload.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      490 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/exit_codes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.520601 conan-2.3.1/conan/cli/formatters/
+-rw-r--r--   0 root         (0) root         (0)      158 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.521601 conan-2.3.1/conan/cli/formatters/graph/
+-rw-r--r--   0 root         (0) root         (0)      110 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5663 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/graph/graph_info_text.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/graph/info_graph_dot.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/graph/info_graph_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.522601 conan-2.3.1/conan/cli/formatters/list/
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/list/binary_html_table.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/list/list.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/formatters/list/search_table_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.522601 conan-2.3.1/conan/cli/printers/
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/printers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6412 2024-05-16 17:40:48.000000 conan-2.3.1/conan/cli/printers/graph.py
+-rw-r--r--   0 root         (0) root         (0)      139 2024-05-16 17:40:48.000000 conan-2.3.1/conan/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.523601 conan-2.3.1/conan/internal/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.523601 conan-2.3.1/conan/internal/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21295 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/detect_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.525601 conan-2.3.1/conan/internal/api/new/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/alias_new.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/autoools_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3850 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/autotools_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/bazel_exe.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/bazel_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/cmake_exe.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/cmake_lib.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/local_recipes_index.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/meson_exe.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/meson_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/msbuild_exe.py
+-rw-r--r--   0 root         (0) root         (0)    12307 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/api/new/msbuild_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.525601 conan-2.3.1/conan/internal/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11189 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4083 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/cache/conan_reference_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.526601 conan-2.3.1/conan/internal/cache/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/cache/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/cache/db/cache_database.py
+-rw-r--r--   0 root         (0) root         (0)     9222 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/cache/db/packages_table.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/cache/db/recipes_table.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/cache/db/table.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/cache/home_paths.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/conan_app.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/integrity_check.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/internal_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.526601 conan-2.3.1/conan/internal/runner/
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14525 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/runner/docker.py
+-rw-r--r--   0 root         (0) root         (0)    12370 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/runner/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/runner/wsl.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-16 17:40:48.000000 conan-2.3.1/conan/internal/upload_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.526601 conan-2.3.1/conan/tools/
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.527601 conan-2.3.1/conan/tools/android/
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/android/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/android/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.527601 conan-2.3.1/conan/tools/apple/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/apple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12880 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/apple/apple.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/apple/xcodebuild.py
+-rw-r--r--   0 root         (0) root         (0)    16239 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/apple/xcodedeps.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/apple/xcodetoolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.528602 conan-2.3.1/conan/tools/build/
+-rw-r--r--   0 root         (0) root         (0)     4190 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11121 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/build/cppstd.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/build/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/build/cross_building.py
+-rw-r--r--   0 root         (0) root         (0)    16208 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/build/flags.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/build/stdcpp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.529601 conan-2.3.1/conan/tools/cmake/
+-rw-r--r--   0 root         (0) root         (0)      217 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14319 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.529601 conan-2.3.1/conan/tools/cmake/cmakedeps/
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmakedeps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11138 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmakedeps/cmakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.530602 conan-2.3.1/conan/tools/cmake/cmakedeps/templates/
+-rw-r--r--   0 root         (0) root         (0)     3944 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmakedeps/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4563 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmakedeps/templates/config.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmakedeps/templates/config_version.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmakedeps/templates/macros.py
+-rw-r--r--   0 root         (0) root         (0)    14989 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmakedeps/templates/target_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    20350 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmakedeps/templates/target_data.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/cmakedeps/templates/targets.py
+-rw-r--r--   0 root         (0) root         (0)     4746 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/layout.py
+-rw-r--r--   0 root         (0) root         (0)    17034 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/presets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.530602 conan-2.3.1/conan/tools/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/toolchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45120 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/toolchain/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    13891 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/toolchain/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/cmake/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.531602 conan-2.3.1/conan/tools/env/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26546 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/env/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3601 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/env/virtualbuildenv.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/env/virtualrunenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.532602 conan-2.3.1/conan/tools/files/
+-rw-r--r--   0 root         (0) root         (0)      535 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/files/conandata.py
+-rw-r--r--   0 root         (0) root         (0)     7429 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/files/copy_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    24002 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/files/files.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/files/packager.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/files/patches.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.532602 conan-2.3.1/conan/tools/files/symlinks/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/files/symlinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/files/symlinks/symlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.533602 conan-2.3.1/conan/tools/gnu/
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6173 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/autotoolsdeps.py
+-rw-r--r--   0 root         (0) root         (0)    13681 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/autotoolstoolchain.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/get_gnu_triplet.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/gnudeps_flags.py
+-rw-r--r--   0 root         (0) root         (0)    13632 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/gnutoolchain.py
+-rw-r--r--   0 root         (0) root         (0)    27066 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/makedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/pkgconfig.py
+-rw-r--r--   0 root         (0) root         (0)    19100 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/gnu/pkgconfigdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.534602 conan-2.3.1/conan/tools/google/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/google/bazel.py
+-rw-r--r--   0 root         (0) root         (0)    23672 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/google/bazeldeps.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/google/layout.py
+-rw-r--r--   0 root         (0) root         (0)     8113 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/google/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.534602 conan-2.3.1/conan/tools/intel/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/intel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/intel/intel_cc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.534602 conan-2.3.1/conan/tools/layout/
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/layout/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.535602 conan-2.3.1/conan/tools/meson/
+-rw-r--r--   0 root         (0) root         (0)       98 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/meson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/meson/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/meson/meson.py
+-rw-r--r--   0 root         (0) root         (0)    25007 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/meson/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.536602 conan-2.3.1/conan/tools/microsoft/
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/microsoft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/microsoft/layout.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/microsoft/msbuild.py
+-rw-r--r--   0 root         (0) root         (0)    19246 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/microsoft/msbuilddeps.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/microsoft/nmakedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/microsoft/nmaketoolchain.py
+-rw-r--r--   0 root         (0) root         (0)      593 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/microsoft/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)    11139 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/microsoft/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)    15069 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/microsoft/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.536602 conan-2.3.1/conan/tools/premake/
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/premake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/premake/premake.py
+-rw-r--r--   0 root         (0) root         (0)    10534 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/premake/premakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.536602 conan-2.3.1/conan/tools/qbs/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/qbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/qbs/qbs.py
+-rw-r--r--   0 root         (0) root         (0)     9897 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/qbs/qbsprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.537602 conan-2.3.1/conan/tools/scm/
+-rw-r--r--   0 root         (0) root         (0)       77 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/scm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13281 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/scm/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.537602 conan-2.3.1/conan/tools/scons/
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/scons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/scons/sconsdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.537602 conan-2.3.1/conan/tools/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17993 2024-05-16 17:40:48.000000 conan-2.3.1/conan/tools/system/package_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.513600 conan-2.3.1/conan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8377 2024-05-16 17:40:58.000000 conan-2.3.1/conan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9839 2024-05-16 17:40:58.000000 conan-2.3.1/conan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 17:40:58.000000 conan-2.3.1/conan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-16 17:40:58.000000 conan-2.3.1/conan.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-16 17:40:58.000000 conan-2.3.1/conan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-16 17:40:58.000000 conan-2.3.1/conan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.538602 conan-2.3.1/conans/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-05-16 17:40:48.000000 conan-2.3.1/conans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.542603 conan-2.3.1/conans/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.542603 conan-2.3.1/conans/client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/cache/editable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.542603 conan-2.3.1/conans/client/cmd/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/cmd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7883 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/cmd/export.py
+-rw-r--r--   0 root         (0) root         (0)    12622 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/cmd/uploader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.543603 conan-2.3.1/conans/client/conanfile/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conanfile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conanfile/build.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conanfile/configure.py
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conanfile/implementations.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conanfile/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.543603 conan-2.3.1/conans/client/conf/
+-rw-r--r--   0 root         (0) root         (0)     7461 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7919 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conf/config_installer.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conf/detect.py
+-rw-r--r--   0 root         (0) root         (0)     4595 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conf/detect_vs.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/conf/required_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.544603 conan-2.3.1/conans/client/downloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/downloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/downloaders/caching_file_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/downloaders/download_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6731 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/downloaders/file_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.544603 conan-2.3.1/conans/client/generators/
+-rw-r--r--   0 root         (0) root         (0)    10455 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/generators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.546603 conan-2.3.1/conans/client/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/build_mode.py
+-rw-r--r--   0 root         (0) root         (0)     6170 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/compute_pid.py
+-rw-r--r--   0 root         (0) root         (0)    15998 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    23157 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/graph_binaries.py
+-rw-r--r--   0 root         (0) root         (0)    22436 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/graph_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/graph_error.py
+-rw-r--r--   0 root         (0) root         (0)    21376 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/install_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5186 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/profile_node_definer.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/provides.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     6480 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/python_requires.py
+-rw-r--r--   0 root         (0) root         (0)     5326 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/graph/range_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/hook_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21840 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/installer.py
+-rw-r--r--   0 root         (0) root         (0)    17007 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/loader_txt.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/migrations.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/pkg_sign.py
+-rw-r--r--   0 root         (0) root         (0)    17816 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/profile_loader.py
+-rw-r--r--   0 root         (0) root         (0)    14595 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/remote_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.547603 conan-2.3.1/conans/client/rest/
+-rw-r--r--   0 root         (0) root         (0)      838 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5837 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest/auth_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest/client_routes.py
+-rw-r--r--   0 root         (0) root         (0)     6936 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest/conan_requester.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest/file_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest/remote_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     5424 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)     9776 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest/rest_client_common.py
+-rw-r--r--   0 root         (0) root         (0)    14934 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest/rest_client_v2.py
+-rw-r--r--   0 root         (0) root         (0)     9149 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/rest_client_local_recipe_index.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.547603 conan-2.3.1/conans/client/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4205 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/store/localdb.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)     4223 2024-05-16 17:40:48.000000 conan-2.3.1/conans/client/userio.py
+-rwxr-xr-x   0 root         (0) root         (0)      118 2024-05-16 17:40:48.000000 conan-2.3.1/conans/conan.py
+-rw-r--r--   0 root         (0) root         (0)      699 2024-05-16 17:40:48.000000 conan-2.3.1/conans/conan_server.py
+-rw-r--r--   0 root         (0) root         (0)     7419 2024-05-16 17:40:48.000000 conan-2.3.1/conans/errors.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-05-16 17:40:48.000000 conan-2.3.1/conans/migrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.550604 conan-2.3.1/conans/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20506 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/build_info.py
+-rw-r--r--   0 root         (0) root         (0)    12678 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/conan_file.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/conanfile_interface.py
+-rw-r--r--   0 root         (0) root         (0)    32672 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/conf.py
+-rw-r--r--   0 root         (0) root         (0)     6302 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    13316 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/graph_lock.py
+-rw-r--r--   0 root         (0) root         (0)    15205 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/info.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    17829 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/options.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/package_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/pkg_type.py
+-rw-r--r--   0 root         (0) root         (0)     7155 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/profile.py
+-rw-r--r--   0 root         (0) root         (0)     8317 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/recipe_ref.py
+-rw-r--r--   0 root         (0) root         (0)    24616 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/requires.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/rest_routes.py
+-rw-r--r--   0 root         (0) root         (0)    14049 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/version.py
+-rw-r--r--   0 root         (0) root         (0)     8643 2024-05-16 17:40:48.000000 conan-2.3.1/conans/model/version_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.550604 conan-2.3.1/conans/paths/
+-rw-r--r--   0 root         (0) root         (0)     2198 2024-05-16 17:40:48.000000 conan-2.3.1/conans/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      251 2024-05-16 17:40:48.000000 conan-2.3.1/conans/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2024-05-16 17:40:48.000000 conan-2.3.1/conans/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-16 17:40:48.000000 conan-2.3.1/conans/requirements_runner.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-16 17:40:48.000000 conan-2.3.1/conans/requirements_server.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.551604 conan-2.3.1/conans/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-05-16 17:40:48.000000 conan-2.3.1/conans/search/query_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-05-16 17:40:48.000000 conan-2.3.1/conans/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.552604 conan-2.3.1/conans/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.553604 conan-2.3.1/conans/test/assets/
+-rw-r--r--   0 root         (0) root         (0)      510 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/assets/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/assets/cmake.py
+-rw-r--r--   0 root         (0) root         (0)    17307 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/assets/genconanfile.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/assets/pkg_cmake.py
+-rw-r--r--   0 root         (0) root         (0)     6008 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/assets/sources.py
+-rw-r--r--   0 root         (0) root         (0)    11972 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/assets/visual_project_files.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.554604 conan-2.3.1/conans/test/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/utils/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/utils/file_server.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/utils/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/utils/scm.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/utils/server_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/utils/test_files.py
+-rw-r--r--   0 root         (0) root         (0)    37579 2024-05-16 17:40:48.000000 conan-2.3.1/conans/test/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:40:58.556604 conan-2.3.1/conans/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/config_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/dates.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/env.py
+-rw-r--r--   0 root         (0) root         (0)    11974 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/locks.py
+-rw-r--r--   0 root         (0) root         (0)     3729 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/runners.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/sha.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-05-16 17:40:48.000000 conan-2.3.1/conans/util/windows.py
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-16 17:40:48.000000 conan-2.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-16 17:40:58.557604 conan-2.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5218 2024-05-16 17:40:48.000000 conan-2.3.1/setup.py
```

### Comparing `conan-2.3.0/LICENSE.md` & `conan-2.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/PKG-INFO` & `conan-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.3.0
+Version: 2.3.1
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.3.0/README.md` & `conan-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/conan_api.py` & `conan-2.3.1/conan/api/conan_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/model.py` & `conan-2.3.1/conan/api/model.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/output.py` & `conan-2.3.1/conan/api/output.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/cache.py` & `conan-2.3.1/conan/api/subapi/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/command.py` & `conan-2.3.1/conan/api/subapi/command.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/config.py` & `conan-2.3.1/conan/api/subapi/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/download.py` & `conan-2.3.1/conan/api/subapi/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/export.py` & `conan-2.3.1/conan/api/subapi/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/graph.py` & `conan-2.3.1/conan/api/subapi/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/install.py` & `conan-2.3.1/conan/api/subapi/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/list.py` & `conan-2.3.1/conan/api/subapi/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/local.py` & `conan-2.3.1/conan/api/subapi/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,13 +107,14 @@
     def test(conanfile):
         """ calls the 'test()' method of the current (user folder) test_package/conanfile.py
         """
         with conanfile_exception_formatter(conanfile, "test"):
             with chdir(conanfile.build_folder):
                 conanfile.test()
 
-    def inspect(self, conanfile_path, remotes, lockfile):
+    def inspect(self, conanfile_path, remotes, lockfile, name=None, version=None, user=None,
+                channel=None):
         app = ConanApp(self._conan_api)
-        conanfile = app.loader.load_named(conanfile_path, name=None, version=None,
-                                          user=None, channel=None, remotes=remotes, graph_lock=lockfile)
+        conanfile = app.loader.load_named(conanfile_path, name=name, version=version, user=user,
+                                          channel=channel, remotes=remotes, graph_lock=lockfile)
         return conanfile
```

### Comparing `conan-2.3.0/conan/api/subapi/lockfile.py` & `conan-2.3.1/conan/api/subapi/lockfile.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/new.py` & `conan-2.3.1/conan/api/subapi/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/profiles.py` & `conan-2.3.1/conan/api/subapi/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/remotes.py` & `conan-2.3.1/conan/api/subapi/remotes.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/remove.py` & `conan-2.3.1/conan/api/subapi/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/search.py` & `conan-2.3.1/conan/api/subapi/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/api/subapi/upload.py` & `conan-2.3.1/conan/api/subapi/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/args.py` & `conan-2.3.1/conan/cli/args.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/cli.py` & `conan-2.3.1/conan/cli/cli.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/command.py` & `conan-2.3.1/conan/cli/command.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/build.py` & `conan-2.3.1/conan/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/cache.py` & `conan-2.3.1/conan/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/config.py` & `conan-2.3.1/conan/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/create.py` & `conan-2.3.1/conan/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/download.py` & `conan-2.3.1/conan/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/editable.py` & `conan-2.3.1/conan/cli/commands/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/export.py` & `conan-2.3.1/conan/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/export_pkg.py` & `conan-2.3.1/conan/cli/commands/export_pkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile, conanfile_path=path,
                                                cwd=cwd, partial=args.lockfile_partial,
                                                overrides=overrides)
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
 
-    conanfile = conan_api.local.inspect(path, remotes, lockfile)
+    conanfile = conan_api.local.inspect(path, remotes, lockfile, name=args.name,
+                                        version=args.version, user=args.user, channel=args.channel)
     # The package_type is not fully processed at export
     if conanfile.package_type == "python-require":
         raise ConanException("export-pkg can only be used for binaries, not for 'python-require'")
     ref, conanfile = conan_api.export.export(path=path, name=args.name, version=args.version,
                                              user=args.user, channel=args.channel, lockfile=lockfile,
                                              remotes=remotes)
     lockfile = conan_api.lockfile.update_lockfile_export(lockfile, conanfile, ref,
```

### Comparing `conan-2.3.0/conan/cli/commands/graph.py` & `conan-2.3.1/conan/cli/commands/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/inspect.py` & `conan-2.3.1/conan/cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/install.py` & `conan-2.3.1/conan/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/list.py` & `conan-2.3.1/conan/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/lock.py` & `conan-2.3.1/conan/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/new.py` & `conan-2.3.1/conan/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/pkglist.py` & `conan-2.3.1/conan/cli/commands/pkglist.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/profile.py` & `conan-2.3.1/conan/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/remote.py` & `conan-2.3.1/conan/cli/commands/remote.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/remove.py` & `conan-2.3.1/conan/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/search.py` & `conan-2.3.1/conan/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/source.py` & `conan-2.3.1/conan/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/test.py` & `conan-2.3.1/conan/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/upload.py` & `conan-2.3.1/conan/cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/commands/version.py` & `conan-2.3.1/conan/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/formatters/graph/graph.py` & `conan-2.3.1/conan/cli/formatters/graph/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/formatters/graph/graph_info_text.py` & `conan-2.3.1/conan/cli/formatters/graph/graph_info_text.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/formatters/graph/info_graph_html.py` & `conan-2.3.1/conan/cli/formatters/graph/info_graph_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/formatters/list/binary_html_table.py` & `conan-2.3.1/conan/cli/formatters/list/binary_html_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/formatters/list/list.py` & `conan-2.3.1/conan/cli/formatters/list/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/formatters/list/search_table_html.py` & `conan-2.3.1/conan/cli/formatters/list/search_table_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/cli/printers/graph.py` & `conan-2.3.1/conan/cli/printers/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/detect_api.py` & `conan-2.3.1/conan/internal/api/detect_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -380,17 +380,22 @@
             return detect_cl_compiler(command)
 
         # I am not able to find its version
         output.error("Not able to automatically detect '%s' version" % command)
         return None, None, None
 
     if platform.system() == "Windows":
-        compiler, version, compiler_exe = detect_msvc_compiler()
-        if compiler:
-            return compiler, version, compiler_exe
+        ide_version = _detect_vs_ide_version()
+        version = {"17": "193", "16": "192", "15": "191"}.get(str(ide_version))  # Map to compiler
+        if ide_version == "17":
+            update = detect_msvc_update(version)  # FIXME weird passing here the 193 compiler version
+            if update and int(update) >= 10:
+                version = "194"
+        if version:
+            return 'msvc', Version(version), None
 
     if platform.system() == "SunOS":
         sun_cc, sun_cc_version, compiler_exe = detect_suncc_compiler()
         if sun_cc:
             return sun_cc, sun_cc_version, compiler_exe
 
     if platform.system() in ["Darwin", "FreeBSD"]:
@@ -405,15 +410,15 @@
         gcc, gcc_version, compiler_exe = detect_gcc_compiler()
         if gcc:
             return gcc, gcc_version, compiler_exe
         return detect_clang_compiler()
 
 
 def default_msvc_ide_version(version):
-    version = {"193": "17", "192": "16", "191": "15"}.get(str(version))
+    version = {"194": "17", "193": "17", "192": "16", "191": "15"}.get(str(version))
     if version:
         return Version(version)
 
 
 def _detect_vs_ide_version():
     from conans.client.conf.detect_vs import vs_installation_path
     msvc_versions = "17", "16", "15"
```

### Comparing `conan-2.3.0/conan/internal/api/new/autoools_exe.py` & `conan-2.3.1/conan/internal/api/new/autoools_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/autotools_lib.py` & `conan-2.3.1/conan/internal/api/new/autotools_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/basic.py` & `conan-2.3.1/conan/internal/api/new/basic.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/bazel_exe.py` & `conan-2.3.1/conan/internal/api/new/bazel_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/bazel_lib.py` & `conan-2.3.1/conan/internal/api/new/bazel_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/cmake_exe.py` & `conan-2.3.1/conan/internal/api/new/cmake_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/cmake_lib.py` & `conan-2.3.1/conan/internal/api/new/cmake_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/local_recipes_index.py` & `conan-2.3.1/conan/internal/api/new/local_recipes_index.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/meson_exe.py` & `conan-2.3.1/conan/internal/api/new/meson_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/meson_lib.py` & `conan-2.3.1/conan/internal/api/new/meson_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/msbuild_exe.py` & `conan-2.3.1/conan/internal/api/new/msbuild_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/api/new/msbuild_lib.py` & `conan-2.3.1/conan/internal/api/new/msbuild_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/cache/cache.py` & `conan-2.3.1/conan/internal/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/cache/conan_reference_layout.py` & `conan-2.3.1/conan/internal/cache/conan_reference_layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/cache/db/cache_database.py` & `conan-2.3.1/conan/internal/cache/db/cache_database.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/cache/db/packages_table.py` & `conan-2.3.1/conan/internal/cache/db/packages_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/cache/db/recipes_table.py` & `conan-2.3.1/conan/internal/cache/db/recipes_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/cache/db/table.py` & `conan-2.3.1/conan/internal/cache/db/table.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/cache/home_paths.py` & `conan-2.3.1/conan/internal/cache/home_paths.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/conan_app.py` & `conan-2.3.1/conan/internal/conan_app.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/deploy.py` & `conan-2.3.1/conan/internal/deploy.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/integrity_check.py` & `conan-2.3.1/conan/internal/integrity_check.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/internal_tools.py` & `conan-2.3.1/conan/internal/internal_tools.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/runner/docker.py` & `conan-2.3.1/conan/internal/runner/docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         # Update conan command and some paths to run inside the container
         raw_args[raw_args.index(args.path)] = self.abs_docker_path
         self.profiles = []
         if self.args.profile_build and self.args.profile_host:
             profile_list = set(self.args.profile_build + self.args.profile_host)
         else:
             profile_list = self.args.profile_host or self.args.profile_build
-        
+
         # Update the profile paths
         for i, raw_arg in enumerate(raw_args):
             for i, raw_profile in enumerate(profile_list):
                 _profile = ProfileLoader.get_profile_path(os.path.join(ConfigAPI(self.conan_api).home(), 'profiles'), raw_profile, os.getcwd())
                 _name = f'{os.path.basename(_profile)}_{i}'
                 if raw_profile in raw_arg:
                     raw_args[raw_args.index(raw_arg)] = raw_arg.replace(raw_profile, os.path.join(self.abs_docker_path, '.conanrunner/profiles', _name))
@@ -107,15 +107,15 @@
         self.configfile = config_parser(host_profile.runner.get('configfile'))
         self.dockerfile = host_profile.runner.get('dockerfile') or self.configfile.build.dockerfile
         self.docker_build_context = host_profile.runner.get('build_context') or self.configfile.build.build_context
         self.image = host_profile.runner.get('image') or self.configfile.image
         if not (self.dockerfile or self.image):
             raise ConanException("'dockerfile' or docker image name is needed")
         self.image = self.image or 'conan-runner-default'
-        self.name = self.configfile.image or f'conan-runner-{host_profile.runner.get("suffix", "docker")}'
+        self.name = self.configfile.run.name or f'conan-runner-{host_profile.runner.get("suffix", "docker")}'
         self.remove = str(host_profile.runner.get('remove', 'false')).lower() == 'true'
         self.cache = str(host_profile.runner.get('cache', 'clean'))
         self.container = None
 
     def run(self):
         """
         run conan inside a Docker continer
```

### Comparing `conan-2.3.0/conan/internal/runner/ssh.py` & `conan-2.3.1/conan/internal/runner/ssh.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/runner/wsl.py` & `conan-2.3.1/conan/internal/runner/wsl.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/internal/upload_metadata.py` & `conan-2.3.1/conan/internal/upload_metadata.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/android/utils.py` & `conan-2.3.1/conan/tools/android/utils.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/apple/__init__.py` & `conan-2.3.1/conan/tools/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/apple/apple.py` & `conan-2.3.1/conan/tools/apple/apple.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/apple/xcodebuild.py` & `conan-2.3.1/conan/tools/apple/xcodebuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/apple/xcodedeps.py` & `conan-2.3.1/conan/tools/apple/xcodedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/apple/xcodetoolchain.py` & `conan-2.3.1/conan/tools/apple/xcodetoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/build/__init__.py` & `conan-2.3.1/conan/tools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/build/cppstd.py` & `conan-2.3.1/conan/tools/build/cppstd.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/build/cpu.py` & `conan-2.3.1/conan/tools/build/cpu.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/build/cross_building.py` & `conan-2.3.1/conan/tools/build/cross_building.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/build/flags.py` & `conan-2.3.1/conan/tools/build/flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/build/stdcpp_library.py` & `conan-2.3.1/conan/tools/build/stdcpp_library.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/cmake.py` & `conan-2.3.1/conan/tools/cmake/cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/cmakedeps/cmakedeps.py` & `conan-2.3.1/conan/tools/cmake/cmakedeps/cmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/__init__.py` & `conan-2.3.1/conan/tools/cmake/cmakedeps/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/config.py` & `conan-2.3.1/conan/tools/cmake/cmakedeps/templates/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/config_version.py` & `conan-2.3.1/conan/tools/cmake/cmakedeps/templates/config_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/macros.py` & `conan-2.3.1/conan/tools/cmake/cmakedeps/templates/macros.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/target_configuration.py` & `conan-2.3.1/conan/tools/cmake/cmakedeps/templates/target_configuration.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/target_data.py` & `conan-2.3.1/conan/tools/cmake/cmakedeps/templates/target_data.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/targets.py` & `conan-2.3.1/conan/tools/cmake/cmakedeps/templates/targets.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/layout.py` & `conan-2.3.1/conan/tools/cmake/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/presets.py` & `conan-2.3.1/conan/tools/cmake/presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,32 +12,34 @@
 from conans.client.graph.graph import RECIPE_CONSUMER
 from conan.errors import ConanException
 from conans.util.files import save, load
 
 
 def write_cmake_presets(conanfile, toolchain_file, generator, cache_variables,
                         user_presets_path=None, preset_prefix=None, buildenv=None, runenv=None,
-                        cmake_executable=None):
+                        cmake_executable=None, absolute_paths=None):
     preset_path, preset_data = _CMakePresets.generate(conanfile, toolchain_file, generator,
                                                       cache_variables, preset_prefix, buildenv, runenv,
-                                                      cmake_executable)
-    _IncludingPresets.generate(conanfile, preset_path, user_presets_path, preset_prefix, preset_data)
+                                                      cmake_executable, absolute_paths)
+    _IncludingPresets.generate(conanfile, preset_path, user_presets_path, preset_prefix, preset_data,
+                               absolute_paths)
 
 
 class _CMakePresets:
     """ Conan generated main CMakePresets.json inside the generators_folder
     """
     @staticmethod
     def generate(conanfile, toolchain_file, generator, cache_variables, preset_prefix, buildenv, runenv,
-                 cmake_executable):
+                 cmake_executable, absolute_paths):
         toolchain_file = os.path.abspath(os.path.join(conanfile.generators_folder, toolchain_file))
-        try:  # Make it relative to the build dir if possible
-            toolchain_file = os.path.relpath(toolchain_file, conanfile.build_folder)
-        except ValueError:
-            pass
+        if not absolute_paths:
+            try:  # Make it relative to the build dir if possible
+                toolchain_file = os.path.relpath(toolchain_file, conanfile.build_folder)
+            except ValueError:
+                pass
         cache_variables = cache_variables or {}
         if platform.system() == "Windows" and generator == "MinGW Makefiles":
             if "CMAKE_SH" not in cache_variables:
                 cache_variables["CMAKE_SH"] = "CMAKE_SH-NOTFOUND"
 
         cmake_make_program = conanfile.conf.get("tools.gnu:make_program",
                                                 default=cache_variables.get("CMAKE_MAKE_PROGRAM"))
@@ -245,15 +247,16 @@
 
 class _IncludingPresets:
     """
     CMakeUserPresets or ConanPresets.json that include the main generated CMakePresets
     """
 
     @staticmethod
-    def generate(conanfile, preset_path, user_presets_path, preset_prefix, preset_data):
+    def generate(conanfile, preset_path, user_presets_path, preset_prefix, preset_data,
+                 absolute_paths):
         if not user_presets_path:
             return
 
         # If generators folder is the same as source folder, do not create the user presets
         # we already have the CMakePresets.json right there
         if not (conanfile.source_folder and conanfile.source_folder != conanfile.generators_folder):
             return
@@ -284,18 +287,19 @@
             if "conan" not in data.get("vendor", {}):
                 # The file is not ours, we cannot overwrite it
                 return
 
         if inherited_user:
             _IncludingPresets._clean_user_inherits(data, preset_data)
 
-        try:  # Make it relative to the CMakeUserPresets.json if possible
-            preset_path = os.path.relpath(preset_path, output_dir)
-        except ValueError:
-            pass
+        if not absolute_paths:
+            try:  # Make it relative to the CMakeUserPresets.json if possible
+                preset_path = os.path.relpath(preset_path, output_dir)
+            except ValueError:
+                pass
         data = _IncludingPresets._append_user_preset_path(data, preset_path, output_dir)
 
         data = json.dumps(data, indent=4)
         ConanOutput(str(conanfile)).info(f"CMakeToolchain generated: {user_presets_path}")
         save(user_presets_path, data)
 
     @staticmethod
```

### Comparing `conan-2.3.0/conan/tools/cmake/toolchain/blocks.py` & `conan-2.3.1/conan/tools/cmake/toolchain/blocks.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/cmake/toolchain/toolchain.py` & `conan-2.3.1/conan/tools/cmake/toolchain/toolchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,15 @@
 
         # Set the CMAKE_MODULE_PATH and CMAKE_PREFIX_PATH to the deps .builddirs
         self.find_builddirs = True
         self.user_presets_path = "CMakeUserPresets.json"
         self.presets_prefix = "conan"
         self.presets_build_environment = None
         self.presets_run_environment = None
+        self.absolute_paths = False  # By default use relative paths to toolchain and presets
 
     def _context(self):
         """ Returns dict, the context for the template
         """
         self.preprocessor_definitions.quote_preprocessor_strings()
 
         blocks = self.blocks.process_blocks()
@@ -264,15 +265,15 @@
             runenv = {name: value for name, value in
                       run_env.items(variable_reference="$penv{{{name}}}")}
 
             cmake_executable = self._conanfile.conf.get("tools.cmake:cmake_program", None) or self._find_cmake_exe()
 
         write_cmake_presets(self._conanfile, toolchain_file, self.generator, cache_variables,
                             self.user_presets_path, self.presets_prefix, buildenv, runenv,
-                            cmake_executable)
+                            cmake_executable, self.absolute_paths)
 
     def _get_generator(self, recipe_generator):
         # Returns the name of the generator to be used by CMake
         conanfile = self._conanfile
 
         # Downstream consumer always higher priority
         generator_conf = conanfile.conf.get("tools.cmake.cmaketoolchain:generator")
```

### Comparing `conan-2.3.0/conan/tools/env/environment.py` & `conan-2.3.1/conan/tools/env/environment.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/env/virtualbuildenv.py` & `conan-2.3.1/conan/tools/env/virtualbuildenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/env/virtualrunenv.py` & `conan-2.3.1/conan/tools/env/virtualrunenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/files/__init__.py` & `conan-2.3.1/conan/tools/files/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/files/conandata.py` & `conan-2.3.1/conan/tools/files/conandata.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/files/copy_pattern.py` & `conan-2.3.1/conan/tools/files/copy_pattern.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/files/files.py` & `conan-2.3.1/conan/tools/files/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/files/packager.py` & `conan-2.3.1/conan/tools/files/packager.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/files/patches.py` & `conan-2.3.1/conan/tools/files/patches.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/files/symlinks/symlinks.py` & `conan-2.3.1/conan/tools/files/symlinks/symlinks.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/gnu/autotools.py` & `conan-2.3.1/conan/tools/gnu/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/gnu/autotoolsdeps.py` & `conan-2.3.1/conan/tools/gnu/autotoolsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/gnu/autotoolstoolchain.py` & `conan-2.3.1/conan/tools/gnu/autotoolstoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/gnu/get_gnu_triplet.py` & `conan-2.3.1/conan/tools/gnu/get_gnu_triplet.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/gnu/gnudeps_flags.py` & `conan-2.3.1/conan/tools/gnu/gnudeps_flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/gnu/gnutoolchain.py` & `conan-2.3.1/conan/tools/gnu/gnutoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/gnu/makedeps.py` & `conan-2.3.1/conan/tools/gnu/makedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/gnu/pkgconfig.py` & `conan-2.3.1/conan/tools/gnu/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/gnu/pkgconfigdeps.py` & `conan-2.3.1/conan/tools/gnu/pkgconfigdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/google/bazel.py` & `conan-2.3.1/conan/tools/google/bazel.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/google/bazeldeps.py` & `conan-2.3.1/conan/tools/google/bazeldeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/google/layout.py` & `conan-2.3.1/conan/tools/google/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/google/toolchain.py` & `conan-2.3.1/conan/tools/google/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/intel/intel_cc.py` & `conan-2.3.1/conan/tools/intel/intel_cc.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/layout/__init__.py` & `conan-2.3.1/conan/tools/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/meson/helpers.py` & `conan-2.3.1/conan/tools/meson/helpers.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/meson/meson.py` & `conan-2.3.1/conan/tools/meson/meson.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/meson/toolchain.py` & `conan-2.3.1/conan/tools/meson/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/microsoft/__init__.py` & `conan-2.3.1/conan/tools/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/microsoft/layout.py` & `conan-2.3.1/conan/tools/microsoft/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/microsoft/msbuild.py` & `conan-2.3.1/conan/tools/microsoft/msbuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/microsoft/msbuilddeps.py` & `conan-2.3.1/conan/tools/microsoft/msbuilddeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/microsoft/nmakedeps.py` & `conan-2.3.1/conan/tools/microsoft/nmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/microsoft/nmaketoolchain.py` & `conan-2.3.1/conan/tools/microsoft/nmaketoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/microsoft/subsystems.py` & `conan-2.3.1/conan/tools/microsoft/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/microsoft/toolchain.py` & `conan-2.3.1/conan/tools/microsoft/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/microsoft/visual.py` & `conan-2.3.1/conan/tools/microsoft/visual.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,16 @@
     :return: VS IDE version
     """
     _visuals = {'170': '11',
                 '180': '12',
                 '190': '14',
                 '191': '15',
                 '192': '16',
-                '193': '17'}
+                '193': '17',
+                '194': '17'}  # Note both 193 and 194 belong to VS 17 2022
     return _visuals[str(version)]
 
 
 def msvc_version_to_toolset_version(version):
     """
     Gets the Visual Studio IDE toolset version given the ``msvc`` compiler one.
 
@@ -71,15 +72,16 @@
     :return: VS IDE toolset version
     """
     toolsets = {'170': 'v110',
                 '180': 'v120',
                 '190': 'v140',
                 '191': 'v141',
                 '192': 'v142',
-                "193": 'v143'}
+                "193": 'v143',
+                "194": 'v143'}
     return toolsets.get(str(version))
 
 
 class VCVars:
     """
     VCVars class generator
     """
@@ -136,14 +138,15 @@
             if int(vs_version) <= 14:
                 vcvars_ver = None
             else:
                 compiler_version = str(conanfile.settings.compiler.version)
                 compiler_update = conanfile.settings.get_safe("compiler.update", "")
                 # The equivalent of compiler 19.26 is toolset 14.26
                 vcvars_ver = "14.{}{}".format(compiler_version[-1], compiler_update)
+
         vcvarsarch = _vcvars_arch(conanfile)
 
         winsdk_version = conanfile.conf.get("tools.microsoft:winsdk_version", check_type=str)
         winsdk_version = winsdk_version or conanfile.settings.get_safe("os.version")
         # The vs_install_path is like
         # C:\Program Files (x86)\Microsoft Visual Studio\2019\Community
         # C:\Program Files (x86)\Microsoft Visual Studio\2017\Community
```

### Comparing `conan-2.3.0/conan/tools/premake/premake.py` & `conan-2.3.1/conan/tools/premake/premake.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/premake/premakedeps.py` & `conan-2.3.1/conan/tools/premake/premakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/qbs/qbs.py` & `conan-2.3.1/conan/tools/qbs/qbs.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/qbs/qbsprofile.py` & `conan-2.3.1/conan/tools/qbs/qbsprofile.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/scm/git.py` & `conan-2.3.1/conan/tools/scm/git.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/scons/sconsdeps.py` & `conan-2.3.1/conan/tools/scons/sconsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan/tools/system/package_manager.py` & `conan-2.3.1/conan/tools/system/package_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan.egg-info/PKG-INFO` & `conan-2.3.1/conan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.3.0
+Version: 2.3.1
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.3.0/conan.egg-info/SOURCES.txt` & `conan-2.3.1/conan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conan.egg-info/requires.txt` & `conan-2.3.1/conan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/cache/cache.py` & `conan-2.3.1/conans/client/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/cache/editable.py` & `conan-2.3.1/conans/client/cache/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/cmd/export.py` & `conan-2.3.1/conans/client/cmd/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/cmd/uploader.py` & `conan-2.3.1/conans/client/cmd/uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/conanfile/build.py` & `conan-2.3.1/conans/client/conanfile/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/conanfile/configure.py` & `conan-2.3.1/conans/client/conanfile/configure.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/conanfile/implementations.py` & `conan-2.3.1/conans/client/conanfile/implementations.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/conanfile/package.py` & `conan-2.3.1/conans/client/conanfile/package.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/conf/__init__.py` & `conan-2.3.1/conans/client/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,22 +90,22 @@
                     "6", "6.1", "6.2", "6.3", "6.4", "6.5",
                     "7", "7.1", "7.2", "7.3", "7.4", "7.5",
                     "8", "8.1", "8.2", "8.3", "8.4", "8.5",
                     "9", "9.1", "9.2", "9.3", "9.4", "9.5",
                     "10", "10.1", "10.2", "10.3", "10.4", "10.5",
                     "11", "11.1", "11.2", "11.3", "11.4",
                     "12", "12.1", "12.2", "12.3",
-                    "13", "13.1", "13.2", 
+                    "13", "13.1", "13.2", "13.3",
                     "14", "14.1"]
         libcxx: [libstdc++, libstdc++11]
         threads: [null, posix, win32]  # Windows MinGW
         exception: [null, dwarf2, sjlj, seh]  # Windows MinGW
         cppstd: [null, 98, gnu98, 11, gnu11, 14, gnu14, 17, gnu17, 20, gnu20, 23, gnu23]
     msvc:
-        version: [170, 180, 190, 191, 192, 193]
+        version: [170, 180, 190, 191, 192, 193, 194]
         update: [null, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
         runtime: [static, dynamic]
         runtime_type: [Debug, Release]
         cppstd: [null, 14, 17, 20, 23]
         toolset: [null, v110_xp, v120_xp, v140_xp, v141_xp]
     clang:
         version: ["3.3", "3.4", "3.5", "3.6", "3.7", "3.8", "3.9", "4.0",
```

### Comparing `conan-2.3.0/conans/client/conf/config_installer.py` & `conan-2.3.1/conans/client/conf/config_installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/conf/detect.py` & `conan-2.3.1/conans/client/conf/detect.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/conf/detect_vs.py` & `conan-2.3.1/conans/client/conf/detect_vs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def vs_installation_path(version):
     return _vs_installation_path(version)[0]
 
 
 def vs_detect_update(version):
-    version = {"193": "17", "192": "16", "191": "15"}.get(str(version))
+    version = {"194": "17", "193": "17", "192": "16", "191": "15"}.get(str(version))
     full_version = _vs_installation_path(version)[1]
     components = full_version.split(".")
     if len(components) > 1:
         return components[1]
 
 
 def _vs_installation_path(version):
```

### Comparing `conan-2.3.0/conans/client/conf/required_version.py` & `conan-2.3.1/conans/client/conf/required_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/downloaders/caching_file_downloader.py` & `conan-2.3.1/conans/client/downloaders/caching_file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/downloaders/download_cache.py` & `conan-2.3.1/conans/client/downloaders/download_cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/downloaders/file_downloader.py` & `conan-2.3.1/conans/client/downloaders/file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/generators/__init__.py` & `conan-2.3.1/conans/client/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/graph/build_mode.py` & `conan-2.3.1/conans/client/graph/build_mode.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/graph/compatibility.py` & `conan-2.3.1/conans/client/graph/compatibility.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,34 +26,51 @@
 from conan.tools.build import supported_cppstd
 from conan.errors import ConanException
 
 
 def cppstd_compat(conanfile):
     # It will try to find packages with all the cppstd versions
     extension_properties = getattr(conanfile, "extension_properties", {})
-    if extension_properties.get("compatibility_cppstd") is False:
-        return []
     compiler = conanfile.settings.get_safe("compiler")
     compiler_version = conanfile.settings.get_safe("compiler.version")
     cppstd = conanfile.settings.get_safe("compiler.cppstd")
-    if not compiler or not compiler_version or not cppstd:
+    if not compiler or not compiler_version:
         return []
     base = dict(conanfile.settings.values_list)
-    cppstd_possible_values = supported_cppstd(conanfile)
-    if cppstd_possible_values is None:
-        conanfile.output.warning(f'No cppstd compatibility defined for compiler "{compiler}"')
-        return []
-    ret = []
-    for _cppstd in cppstd_possible_values:
-        if _cppstd is None or _cppstd == cppstd:
+    factors = []  # List of list, each sublist is a potential combination
+    if cppstd is not None and extension_properties.get("compatibility_cppstd") is not False:
+        cppstd_possible_values = supported_cppstd(conanfile)
+        if cppstd_possible_values is None:
+            conanfile.output.warning(f'No cppstd compatibility defined for compiler "{compiler}"')
+        else:
+            factors.append([{"compiler.cppstd": v} for v in cppstd_possible_values if v != cppstd])
+
+    if compiler == "msvc":
+        msvc_fallback = {"194": "193"}.get(compiler_version)
+        if msvc_fallback:
+            factors.append([{"compiler.version": msvc_fallback}])
+
+    combinations = []
+    for factor in factors:
+        if not combinations:
+            combinations = factor
             continue
+        new_combinations = []
+        for comb in combinations:
+            for f in factor:
+                comb = comb.copy()
+                comb.update(f)
+                new_combinations.append(comb)
+        combinations = new_combinations
+
+    ret = []
+    for comb in combinations:
         configuration = base.copy()
-        configuration["compiler.cppstd"] = _cppstd
+        configuration.update(comb)
         ret.append({"settings": [(k, v) for k, v in configuration.items()]})
-
     return ret
 """
 
 
 def migrate_compatibility_files(cache_folder):
     from conans.client.migrations import update_file
     compatible_folder = HomePaths(cache_folder).compatibility_plugin_path
```

### Comparing `conan-2.3.0/conans/client/graph/compute_pid.py` & `conan-2.3.1/conans/client/graph/compute_pid.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/graph/graph.py` & `conan-2.3.1/conans/client/graph/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,19 @@
         # didn't find at check_downstream_exist, because we didn't know the shared/static
         existing = self.transitive_deps.get(require)
         if existing is not None and existing.require is not require:
             if existing.node is not None and existing.node.ref != node.ref:
                 # print("  +++++Runtime conflict!", require, "with", node.ref)
                 return True
             require.aggregate(existing.require)
+            # An override can be overriden by a downstream force/override
+            if existing.require.override and existing.require.ref != require.ref:
+                # If it is an override, but other value, it has been overriden too
+                existing.require.overriden_ref = existing.require.ref
+                existing.require.override_ref = require.ref
 
         assert not require.version_range  # No ranges slip into transitive_deps definitions
         # TODO: Might need to move to an update() for performance
         self.transitive_deps.pop(require, None)
         self.transitive_deps[require] = TransitiveRequirement(require, node)
 
         # Check if need to propagate downstream
@@ -114,14 +119,15 @@
             d = self.dependants[0]
 
         down_require = d.require.transform_downstream(self.conanfile.package_type, require,
                                                       node.conanfile.package_type)
         if down_require is None:
             return
 
+        down_require.defining_require = require.defining_require
         return d.src.propagate_downstream(down_require, node)
 
     def check_downstream_exists(self, require):
         # First, a check against self, could be a loop-conflict
         # This is equivalent as the Requirement hash and eq methods
         # TODO: Make self.ref always exist, but with name=None if name not defined
         if self.ref is not None and require.ref.name == self.ref.name:
@@ -157,14 +163,15 @@
         down_require = dependant.require.transform_downstream(self.conanfile.package_type,
                                                               require, None)
 
         if down_require is None:
             # print("    No need to check downstream more")
             return result
 
+        down_require.defining_require = require.defining_require
         source_node = dependant.src
         return source_node.check_downstream_exists(down_require) or result
 
     def check_loops(self, new_node):
         if self.ref == new_node.ref and self.context == new_node.context:
             return self
         if not self.dependants:
@@ -271,17 +278,17 @@
         return repr(self.serialize())
 
     @staticmethod
     def create(nodes):
         overrides = {}
         for n in nodes:
             for r in n.conanfile.requires.values():
-                if r.override:
+                if r.override and not r.overriden_ref:  # overrides are not real graph edges
                     continue
-                if r.overriden_ref and not r.force:
+                if r.overriden_ref:
                     overrides.setdefault(r.overriden_ref, set()).add(r.override_ref)
                 else:
                     overrides.setdefault(r.ref, set()).add(None)
 
         # reduce, eliminate those overrides definitions that only override to None, that is, not
         # really an override
         result = Overrides()
```

### Comparing `conan-2.3.0/conans/client/graph/graph_binaries.py` & `conan-2.3.1/conans/client/graph/graph_binaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                                       f"{conanfile.info.dump_diff(compatible_package)}")
             node._package_id = package_id  # Modifying package id under the hood, FIXME
             node.binary = None  # Invalidate it
             self._process_compatible_node(node, remotes, update)  # TODO: what if BINARY_BUILD
             if node.binary in (BINARY_CACHE, BINARY_UPDATE, BINARY_DOWNLOAD):
                 _compatible_found(package_id, compatible_package)
                 return
-        if not update:
+        if not should_update_reference(conanfile.ref, update):
             conanfile.output.info(f"Compatible configurations not found in cache, checking servers")
             for package_id, compatible_package in compatibles.items():
                 conanfile.output.info(f"'{package_id}': "
                                       f"{conanfile.info.dump_diff(compatible_package)}")
                 node._package_id = package_id  # Modifying package id under the hood, FIXME
                 node.binary = None  # Invalidate it
                 self._evaluate_download(node, remotes, update)
```

### Comparing `conan-2.3.0/conans/client/graph/graph_builder.py` & `conan-2.3.1/conans/client/graph/graph_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,21 @@
             # print("  Existing previous requirements from ", base_previous, "=>", prev_require)
 
             if prev_require is None:
                 raise GraphLoopError(node, require, prev_node)
 
             prev_ref = prev_node.ref if prev_node else prev_require.ref
             if prev_require.force or prev_require.override:  # override
-                require.overriden_ref = require.ref  # Store that the require has been overriden
-                require.override_ref = prev_ref
-                require.ref = prev_ref
+                if prev_require.defining_require is not require:
+                    require.overriden_ref = require.overriden_ref or require.ref.copy()  # Old one
+                    # require.override_ref can be !=None if lockfile-overrides defined
+                    require.override_ref = (require.override_ref or prev_require.override_ref
+                                            or prev_require.ref.copy())  # New one
+                    require.defining_require = prev_require.defining_require  # The overrider
+                require.ref = prev_ref  # New one, maybe resolved with revision
             else:
                 self._conflicting_version(require, node, prev_require, prev_node,
                                           prev_ref, base_previous, self._resolve_prereleases)
 
         if prev_node is None:
             # new node, must be added and expanded (node -> new_node)
             new_node = self._create_new_node(node, require, graph, profile_host, profile_build,
@@ -191,14 +195,16 @@
                 resolved = False
                 if graph_lock is not None:
                     resolved = graph_lock.replace_alias(require, alias)
                 # if partial, we might still need to resolve the alias
                 if not resolved:
                     self._resolve_alias(node, require, alias, graph)
             self._resolve_replace_requires(node, require, profile_build, profile_host, graph)
+            if graph_lock:
+                graph_lock.resolve_overrides(require)
             node.transitive_deps[require] = TransitiveRequirement(require, node=None)
 
     def _resolve_alias(self, node, require, alias, graph):
         # First try cached
         cached = graph.aliased.get(alias)
         if cached is not None:
             while True:
```

### Comparing `conan-2.3.0/conans/client/graph/graph_error.py` & `conan-2.3.1/conans/client/graph/graph_error.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/graph/install_graph.py` & `conan-2.3.1/conans/client/graph/install_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             install_pkg_ref = _InstallPackageReference.create(node)
             self.packages[node.package_id] = install_pkg_ref
 
         for dep in node.dependencies:
             if dep.dst.binary != BINARY_SKIP:
                 if dep.dst.ref == node.ref:  # If the node is itself, then it is internal dep
                     install_pkg_ref.depends.append(dep.dst.pref.package_id)
-                else:
+                elif dep.dst.ref not in self.depends:
                     self.depends.append(dep.dst.ref)
 
     def _install_order(self):
         # TODO: Repeated, refactor
         # a topological order by levels, returns a list of list, in order of processing
         levels = []
         opened = self.packages
```

### Comparing `conan-2.3.0/conans/client/graph/profile_node_definer.py` & `conan-2.3.1/conans/client/graph/profile_node_definer.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/graph/provides.py` & `conan-2.3.1/conans/client/graph/provides.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/graph/proxy.py` & `conan-2.3.1/conans/client/graph/proxy.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/graph/python_requires.py` & `conan-2.3.1/conans/client/graph/python_requires.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/graph/range_resolver.py` & `conan-2.3.1/conans/client/graph/range_resolver.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/hook_manager.py` & `conan-2.3.1/conans/client/hook_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/installer.py` & `conan-2.3.1/conans/client/installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/loader.py` & `conan-2.3.1/conans/client/loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/loader_txt.py` & `conan-2.3.1/conans/client/loader_txt.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/migrations.py` & `conan-2.3.1/conans/client/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/pkg_sign.py` & `conan-2.3.1/conans/client/pkg_sign.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/profile_loader.py` & `conan-2.3.1/conans/client/profile_loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/remote_manager.py` & `conan-2.3.1/conans/client/remote_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest/__init__.py` & `conan-2.3.1/conans/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest/auth_manager.py` & `conan-2.3.1/conans/client/rest/auth_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest/client_routes.py` & `conan-2.3.1/conans/client/rest/client_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest/conan_requester.py` & `conan-2.3.1/conans/client/rest/conan_requester.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest/file_uploader.py` & `conan-2.3.1/conans/client/rest/file_uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest/remote_credentials.py` & `conan-2.3.1/conans/client/rest/remote_credentials.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest/rest_client.py` & `conan-2.3.1/conans/client/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest/rest_client_common.py` & `conan-2.3.1/conans/client/rest/rest_client_common.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest/rest_client_v2.py` & `conan-2.3.1/conans/client/rest/rest_client_v2.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/rest_client_local_recipe_index.py` & `conan-2.3.1/conans/client/rest_client_local_recipe_index.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/source.py` & `conan-2.3.1/conans/client/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/store/localdb.py` & `conan-2.3.1/conans/client/store/localdb.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/subsystems.py` & `conan-2.3.1/conans/client/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/client/userio.py` & `conan-2.3.1/conans/client/userio.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/conan_server.py` & `conan-2.3.1/conans/conan_server.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/errors.py` & `conan-2.3.1/conans/errors.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/migrations.py` & `conan-2.3.1/conans/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/build_info.py` & `conan-2.3.1/conans/model/build_info.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/conan_file.py` & `conan-2.3.1/conans/model/conan_file.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/conanfile_interface.py` & `conan-2.3.1/conans/model/conanfile_interface.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/conf.py` & `conan-2.3.1/conans/model/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     "tools.apple:enable_arc": "(boolean) Enable/Disable ARC Apple Clang flags",
     "tools.apple:enable_visibility": "(boolean) Enable/Disable Visibility Apple Clang flags",
     "tools.env.virtualenv:powershell": "If it is set to True it will generate powershell launchers if os=Windows",
     # Compilers/Flags configurations
     "tools.build:compiler_executables": "Defines a Python dict-like with the compilers path to be used. Allowed keys {'c', 'cpp', 'cuda', 'objc', 'objcxx', 'rc', 'fortran', 'asm', 'hip', 'ispc', 'ld', 'ar'}",
     "tools.build:cxxflags": "List of extra CXX flags used by different toolchains like CMakeToolchain, AutotoolsToolchain and MesonToolchain",
     "tools.build:cflags": "List of extra C flags used by different toolchains like CMakeToolchain, AutotoolsToolchain and MesonToolchain",
-    "tools.build:defines": "List of extra definition flags used by different toolchains like CMakeToolchain and AutotoolsToolchain",
+    "tools.build:defines": "List of extra definition flags used by different toolchains like CMakeToolchain, AutotoolsToolchain and MesonToolchain",
     "tools.build:sharedlinkflags": "List of extra flags used by CMakeToolchain for CMAKE_SHARED_LINKER_FLAGS_INIT variable",
     "tools.build:exelinkflags": "List of extra flags used by CMakeToolchain for CMAKE_EXE_LINKER_FLAGS_INIT variable",
     "tools.build:linker_scripts": "List of linker script files to pass to the linker used by different toolchains like CMakeToolchain, AutotoolsToolchain, and MesonToolchain",
     # Package ID composition
     "tools.info.package_id:confs": "List of existing configuration to be part of the package ID",
 }
```

### Comparing `conan-2.3.0/conans/model/dependencies.py` & `conan-2.3.1/conans/model/dependencies.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/graph_lock.py` & `conan-2.3.1/conans/model/graph_lock.py`

 * *Files 3% similar despite different names*

```diff
@@ -257,33 +257,38 @@
     def resolve_locked(self, node, require, resolve_prereleases):
         if require.build or node.context == CONTEXT_BUILD:
             locked_refs = self._build_requires.refs()
         elif node.is_conf:
             locked_refs = self._conf_requires.refs()
         else:
             locked_refs = self._requires.refs()
-        self._resolve_overrides(require)
         try:
             self._resolve(require, locked_refs, resolve_prereleases)
         except ConanException:
             overrides = self._overrides.get(require.ref)
             if overrides is not None and len(overrides) > 1:
                 msg = f"Override defined for {require.ref}, but multiple possible overrides" \
                       f" {overrides}. You might need to apply the 'conan graph build-order'" \
                       f" overrides for correctly building this package with this lockfile"
                 ConanOutput().error(msg, error_type="exception")
             raise
 
-    def _resolve_overrides(self, require):
-        existing = self._overrides.get(require.ref)
-        if existing is not None and len(existing) == 1:
-            require.overriden_ref = require.ref  # Store that the require has been overriden
-            ref = next(iter(existing))
-            require.ref = ref
-            require.override_ref = ref
+    def resolve_overrides(self, require):
+        """ The lockfile contains the overrides to be able to inject them when the lockfile is
+        applied to upstream dependencies, that have the overrides downstream
+        """
+        if not self._overrides:
+            return
+
+        overriden = self._overrides.get(require.ref)
+        if overriden and len(overriden) == 1:
+            override_ref = next(iter(overriden))
+            require.overriden_ref = require.overriden_ref or require.ref.copy()
+            require.override_ref = override_ref
+            require.ref = override_ref
 
     def resolve_prev(self, node):
         if node.context == CONTEXT_BUILD:
             prevs = self._build_requires.get(node.ref)
         else:
             prevs = self._requires.get(node.ref)
         if prevs:
```

### Comparing `conan-2.3.0/conans/model/info.py` & `conan-2.3.1/conans/model/info.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/layout.py` & `conan-2.3.1/conans/model/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/manifest.py` & `conan-2.3.1/conans/model/manifest.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/options.py` & `conan-2.3.1/conans/model/options.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/package_ref.py` & `conan-2.3.1/conans/model/package_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/pkg_type.py` & `conan-2.3.1/conans/model/pkg_type.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/profile.py` & `conan-2.3.1/conans/model/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/recipe_ref.py` & `conan-2.3.1/conans/model/recipe_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,19 @@
             version = Version(version)
         self.version = version  # This MUST be a version if we want to be able to order
         self.user = user
         self.channel = channel
         self.revision = revision
         self.timestamp = timestamp
 
+    def copy(self):
+        # Used for creating copy in lockfile-overrides mechanism
+        return RecipeReference(self.name, self.version, self.user, self.channel, self.revision,
+                               self.timestamp)
+
     def __repr__(self):
         """ long repr like pkg/0.1@user/channel#rrev%timestamp """
         result = self.repr_notime()
         if self.timestamp is not None:
             result += "%{}".format(self.timestamp)
         return result
```

### Comparing `conan-2.3.0/conans/model/requires.py` & `conan-2.3.1/conans/model/requires.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
         self._test = test
         self._package_id_mode = package_id_mode
         self._force = force
         self._override = override
         self._direct = direct
         self.options = options
         # Meta and auxiliary information
+        # The "defining_require" is the require that defines the current value. If this require is
+        # overriden/forced, this attribute will point to the overriding/forcing requirement.
+        self.defining_require = self  # if not overriden, it points to itself
         self.overriden_ref = None  # to store if the requirement has been overriden (store old ref)
         self.override_ref = None  # to store if the requirement has been overriden (store new ref)
         self.is_test = test  # to store that it was a test, even if used as regular requires too
         self.skip = False
 
     @property
     def files(self):  # require needs some files in dependency package
@@ -514,24 +517,14 @@
         req = Requirement(ref, headers=False, libs=False, build=True, run=run, visible=visible,
                           package_id_mode=package_id_mode, options=options, override=override)
 
         if raise_if_duplicated and self._requires.get(req):
             raise ConanException("Duplicated requirement: {}".format(ref))
         self._requires[req] = req
 
-    def override(self, ref):
-        req = Requirement(ref)
-        old_requirement = self._requires.get(req)
-        if old_requirement is not None:
-            req.force = True
-            self._requires[req] = req
-        else:
-            req.override = True
-            self._requires[req] = req
-
     def test_require(self, ref, run=None, options=None, force=None):
         """
              Represent a testing framework like gtest
 
              visible = False => Only the direct consumer can see it, won't conflict
              build = False => The test are linked in the host context to run in the host machine
              libs = True => We need to link with gtest
```

### Comparing `conan-2.3.0/conans/model/rest_routes.py` & `conan-2.3.1/conans/model/rest_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/settings.py` & `conan-2.3.1/conans/model/settings.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/version.py` & `conan-2.3.1/conans/model/version.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/model/version_range.py` & `conan-2.3.1/conans/model/version_range.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/paths/__init__.py` & `conan-2.3.1/conans/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/search/query_parse.py` & `conan-2.3.1/conans/search/query_parse.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/search/search.py` & `conan-2.3.1/conans/search/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/assets/autotools.py` & `conan-2.3.1/conans/test/assets/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/assets/cmake.py` & `conan-2.3.1/conans/test/assets/cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/assets/genconanfile.py` & `conan-2.3.1/conans/test/assets/genconanfile.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/assets/pkg_cmake.py` & `conan-2.3.1/conans/test/assets/pkg_cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/assets/sources.py` & `conan-2.3.1/conans/test/assets/sources.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/assets/visual_project_files.py` & `conan-2.3.1/conans/test/assets/visual_project_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/conftest.py` & `conan-2.3.1/conans/test/conftest.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/utils/artifactory.py` & `conan-2.3.1/conans/test/utils/artifactory.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/utils/file_server.py` & `conan-2.3.1/conans/test/utils/file_server.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/utils/mocks.py` & `conan-2.3.1/conans/test/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/utils/profiles.py` & `conan-2.3.1/conans/test/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/utils/scm.py` & `conan-2.3.1/conans/test/utils/scm.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/utils/server_launcher.py` & `conan-2.3.1/conans/test/utils/server_launcher.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/utils/test_files.py` & `conan-2.3.1/conans/test/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/test/utils/tools.py` & `conan-2.3.1/conans/test/utils/tools.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/util/config_parser.py` & `conan-2.3.1/conans/util/config_parser.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/util/dates.py` & `conan-2.3.1/conans/util/dates.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/util/encrypt.py` & `conan-2.3.1/conans/util/encrypt.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/util/env.py` & `conan-2.3.1/conans/util/env.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/util/files.py` & `conan-2.3.1/conans/util/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/util/locks.py` & `conan-2.3.1/conans/util/locks.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/util/runners.py` & `conan-2.3.1/conans/util/runners.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/util/sha.py` & `conan-2.3.1/conans/util/sha.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/conans/util/windows.py` & `conan-2.3.1/conans/util/windows.py`

 * *Files identical despite different names*

### Comparing `conan-2.3.0/setup.py` & `conan-2.3.1/setup.py`

 * *Files identical despite different names*

