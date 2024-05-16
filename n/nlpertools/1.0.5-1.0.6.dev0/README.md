# Comparing `tmp/nlpertools-1.0.5.tar.gz` & `tmp/nlpertools-1.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpertools-1.0.5.tar", last modified: Tue Oct 11 08:49:12 2022, max compression
+gzip compressed data, was "nlpertools-1.0.6.dev0.tar", last modified: Thu May 16 08:59:49 2024, max compression
```

## Comparing `nlpertools-1.0.5.tar` & `nlpertools-1.0.6.dev0.tar`

### file list

```diff
@@ -1,38 +1,61 @@
-drwxrwxrwx   0        0        0        0 2022-10-11 08:49:12.128368 nlpertools-1.0.5/
--rw-rw-rw-   0        0        0    11531 2022-06-22 07:00:46.000000 nlpertools-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2436 2022-10-11 08:49:12.128368 nlpertools-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1898 2022-10-11 08:33:02.000000 nlpertools-1.0.5/README.md
--rw-rw-rw-   0        0        0      108 2022-06-22 07:00:46.000000 nlpertools-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      677 2022-10-11 08:49:12.145120 nlpertools-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-11 08:49:12.070112 nlpertools-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2022-10-11 08:49:12.111712 nlpertools-1.0.5/src/nlpertools/
--rw-rw-rw-   0        0        0      481 2022-10-11 07:28:02.000000 nlpertools-1.0.5/src/nlpertools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-11 08:49:12.127693 nlpertools-1.0.5/src/nlpertools/algo/
--rw-rw-rw-   0        0        0        0 2022-10-11 07:06:10.000000 nlpertools-1.0.5/src/nlpertools/algo/__init__.py
--rw-rw-rw-   0        0        0     1835 2022-10-11 07:49:54.000000 nlpertools-1.0.5/src/nlpertools/algo/kmp.py
--rw-rw-rw-   0        0        0     9481 2022-10-11 07:58:04.000000 nlpertools-1.0.5/src/nlpertools/data_client.py
-drwxrwxrwx   0        0        0        0 2022-10-11 08:49:12.128368 nlpertools-1.0.5/src/nlpertools/data_structure/
--rw-rw-rw-   0        0        0        0 2022-10-11 07:06:10.000000 nlpertools-1.0.5/src/nlpertools/data_structure/__init__.py
--rw-rw-rw-   0        0        0      316 2022-10-10 05:48:01.000000 nlpertools-1.0.5/src/nlpertools/data_structure/base_structure.py
--rw-rw-rw-   0        0        0       71 2022-06-22 07:00:46.000000 nlpertools-1.0.5/src/nlpertools/dataprocess.py
-drwxrwxrwx   0        0        0        0 2022-10-11 08:49:12.128368 nlpertools-1.0.5/src/nlpertools/io/
--rw-rw-rw-   0        0        0       71 2022-06-23 07:18:30.000000 nlpertools-1.0.5/src/nlpertools/io/__init__.py
--rw-rw-rw-   0        0        0      798 2022-06-23 07:27:23.000000 nlpertools-1.0.5/src/nlpertools/io/dir.py
--rw-rw-rw-   0        0        0     5925 2022-10-11 07:58:04.000000 nlpertools-1.0.5/src/nlpertools/io/file.py
--rw-rw-rw-   0        0        0    17578 2022-10-11 07:58:04.000000 nlpertools-1.0.5/src/nlpertools/ml.py
--rw-rw-rw-   0        0        0     1809 2022-10-11 07:58:04.000000 nlpertools-1.0.5/src/nlpertools/openApi.py
--rw-rw-rw-   0        0        0     7865 2022-10-11 08:45:08.000000 nlpertools-1.0.5/src/nlpertools/other.py
--rw-rw-rw-   0        0        0     1211 2022-06-29 03:40:54.000000 nlpertools-1.0.5/src/nlpertools/plugin.py
--rw-rw-rw-   0        0        0     2337 2022-10-11 07:58:04.000000 nlpertools-1.0.5/src/nlpertools/reminder.py
-drwxrwxrwx   0        0        0        0 2022-10-11 08:49:12.128368 nlpertools-1.0.5/src/nlpertools/template/
--rw-rw-rw-   0        0        0        0 2022-10-11 07:06:10.000000 nlpertools-1.0.5/src/nlpertools/template/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-11 08:49:12.128368 nlpertools-1.0.5/src/nlpertools/utils/
--rw-rw-rw-   0        0        0       71 2022-10-11 07:58:04.000000 nlpertools-1.0.5/src/nlpertools/utils/__init__.py
--rw-rw-rw-   0        0        0     2739 2022-10-11 08:40:14.000000 nlpertools-1.0.5/src/nlpertools/utils/package.py
--rw-rw-rw-   0        0        0     3676 2022-10-11 07:50:56.000000 nlpertools-1.0.5/src/nlpertools/utils_for_nlpertools.py
--rw-rw-rw-   0        0        0     2649 2022-09-29 03:56:45.000000 nlpertools-1.0.5/src/nlpertools/wrapper.py
-drwxrwxrwx   0        0        0        0 2022-10-11 08:49:12.111712 nlpertools-1.0.5/src/nlpertools.egg-info/
--rw-rw-rw-   0        0        0     2436 2022-10-11 08:49:12.000000 nlpertools-1.0.5/src/nlpertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      800 2022-10-11 08:49:12.000000 nlpertools-1.0.5/src/nlpertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-11 08:49:12.000000 nlpertools-1.0.5/src/nlpertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-10-11 08:49:12.000000 nlpertools-1.0.5/src/nlpertools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.130754 nlpertools-1.0.6.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-16 08:59:49.130754 nlpertools-1.0.6.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-16 08:59:49.130754 nlpertools-1.0.6.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.122754 nlpertools-1.0.6.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.122754 nlpertools-1.0.6.dev0/src/nlpertools/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.126754 nlpertools-1.0.6.dev0/src/nlpertools/algo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/algo/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/algo/bit_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/algo/kmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/algo/num_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/algo/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/algo/union.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13534 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/data_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.126754 nlpertools-1.0.6.dev0/src/nlpertools/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/data_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/data_structure/base_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22658 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/dataprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/default_db_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.126754 nlpertools-1.0.6.dev0/src/nlpertools/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/io/dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16798 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.126754 nlpertools-1.0.6.dev0/src/nlpertools/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/monitor/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/monitor/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/nlpertools_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/open_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/pic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/reminder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.126754 nlpertools-1.0.6.dev0/src/nlpertools/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.126754 nlpertools-1.0.6.dev0/src/nlpertools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29280 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/utils/log_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/utils/package_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/utils/package_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/utils_for_nlpertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/vector_index_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.130754 nlpertools-1.0.6.dev0/src/nlpertools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-16 08:59:49.000000 nlpertools-1.0.6.dev0/src/nlpertools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-16 08:59:49.000000 nlpertools-1.0.6.dev0/src/nlpertools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:59:49.000000 nlpertools-1.0.6.dev0/src/nlpertools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 08:59:49.000000 nlpertools-1.0.6.dev0/src/nlpertools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.126754 nlpertools-1.0.6.dev0/src/nlpertools_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/src/nlpertools_helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:59:49.130754 nlpertools-1.0.6.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/tests/test_kmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-16 08:59:38.000000 nlpertools-1.0.6.dev0/tests/test_path_exists.py
```

### Comparing `nlpertools-1.0.5/LICENSE` & `nlpertools-1.0.6.dev0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-        Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+        Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `nlpertools-1.0.5/setup.cfg` & `nlpertools-1.0.6.dev0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206e 6c70 6572 746f 6f6c 730d 0a76   = nlpertools..v
-00000020: 6572 7369 6f6e 203d 2031 2e30 2e35 0d0a  ersion = 1.0.5..
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6e6c 7065 7274 6f6f 6c73 0a76 6572  = nlpertools.ver
+00000020: 7369 6f6e 203d 2031 2e30 2e36 6465 760a  sion = 1.0.6dev.
 00000030: 6175 7468 6f72 203d 2079 6f75 7368 754a  author = youshuJ
-00000040: 690d 0a61 7574 686f 725f 656d 6169 6c20  i..author_email 
-00000050: 3d20 7a6a 7332 3030 3031 3230 3540 676d  = zjs20001205@gm
-00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
-00000070: 7469 6f6e 203d 2041 2073 6d61 6c6c 2070  tion = A small p
-00000080: 6163 6b61 6765 2061 626f 7574 2073 6d61  ackage about sma
-00000090: 6c6c 2062 6173 6963 2049 4f20 6f70 6572  ll basic IO oper
-000000a0: 6174 696f 6e20 7768 656e 2063 6f64 696e  ation when codin
-000000b0: 670d 0a6c 6f6e 675f 6465 7363 7269 7074  g..long_descript
-000000c0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000d0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
-000000e0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-000000f0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
-00000100: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
-00000110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00000120: 767a 6969 2f6e 6c70 6572 746f 6f6c 730d  vzii/nlpertools.
-00000130: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-00000140: 0d0a 0942 7567 2054 7261 636b 6572 203d  ...Bug Tracker =
-00000150: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000160: 636f 6d2f 6c76 7a69 692f 6e6c 7065 7274  com/lvzii/nlpert
-00000170: 6f6f 6c73 2f69 7373 7565 730d 0a63 6c61  ools/issues..cla
-00000180: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-00000190: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001b0: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
-000001c0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-000001d0: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-000001e0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-000001f0: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000200: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000210: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000220: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
-00000230: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-00000240: 6571 7569 7265 7320 3d20 3e3d 332e 360d  equires = >=3.6.
-00000250: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000260: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-00000270: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
-00000280: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000290: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000002a0: 300d 0a0d 0a                             0....
+00000040: 690a 6175 7468 6f72 5f65 6d61 696c 203d  i.author_email =
+00000050: 207a 6a73 3230 3030 3132 3035 4067 6d61   zjs20001205@gma
+00000060: 696c 2e63 6f6d 0a64 6573 6372 6970 7469  il.com.descripti
+00000070: 6f6e 203d 2041 2073 6d61 6c6c 2070 6163  on = A small pac
+00000080: 6b61 6765 2061 626f 7574 2073 6d61 6c6c  kage about small
+00000090: 2062 6173 6963 2049 4f20 6f70 6572 6174   basic IO operat
+000000a0: 696f 6e20 7768 656e 2063 6f64 696e 670a  ion when coding.
+000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000c0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000000d0: 6d64 0a6c 6f6e 675f 6465 7363 7269 7074  md.long_descript
+000000e0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+000000f0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+00000100: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+00000110: 6974 6875 622e 636f 6d2f 6c76 7a69 692f  ithub.com/lvzii/
+00000120: 6e6c 7065 7274 6f6f 6c73 0a70 726f 6a65  nlpertools.proje
+00000130: 6374 5f75 726c 7320 3d20 0a09 4275 6720  ct_urls = ..Bug 
+00000140: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+00000150: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 767a  //github.com/lvz
+00000160: 6969 2f6e 6c70 6572 746f 6f6c 732f 6973  ii/nlpertools/is
+00000170: 7375 6573 0a63 6c61 7373 6966 6965 7273  sues.classifiers
+00000180: 203d 200a 0950 726f 6772 616d 6d69 6e67   = ..Programming
+00000190: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001a0: 686f 6e20 3a3a 2033 0a09 4c69 6365 6e73  hon :: 3..Licens
+000001b0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001c0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000001d0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+000001e0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000001f0: 6465 6e74 0a0a 5b6f 7074 696f 6e73 5d0a  dent..[options].
+00000200: 7061 636b 6167 655f 6469 7220 3d20 0a09  package_dir = ..
+00000210: 3d20 7372 630a 7061 636b 6167 6573 203d  = src.packages =
+00000220: 2066 696e 643a 0a70 7974 686f 6e5f 7265   find:.python_re
+00000230: 7175 6972 6573 203d 203e 3d33 2e36 0a0a  quires = >=3.6..
+00000240: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000250: 732e 6669 6e64 5d0a 7768 6572 6520 3d20  s.find].where = 
+00000260: 7372 630a 0a5b 6f70 7469 6f6e 732e 7061  src..[options.pa
+00000270: 636b 6167 655f 6461 7461 5d0a 6e6c 7065  ckage_data].nlpe
+00000280: 7274 6f6f 6c73 203d 202a 2e79 6d6c 0a0a  rtools = *.yml..
+00000290: 5b65 6767 5f69 6e66 6f5d 0a74 6167 5f62  [egg_info].tag_b
+000002a0: 7569 6c64 203d 200a 7461 675f 6461 7465  uild = .tag_date
+000002b0: 203d 2030 0a0a                            = 0..
```

### Comparing `nlpertools-1.0.5/src/nlpertools/algo/kmp.py` & `nlpertools-1.0.6.dev0/src/nlpertools/algo/kmp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,94 @@
-#!/usr/bin/python3.8
-# -*- coding: utf-8 -*-
-# @Author  : youshu.Ji
-
-def build(pattern_string):
-    """
-    构建模式串的PMT
-    [zhihu](https://www.zhihu.com/question/21923021/answer/281346746)
-
-    """
-    # 构建pattern需要回溯的位置，
-    backtrace_points = [0] * len(pattern_string)
-    main_pointer, pattern_pointer = 0, -1
-    backtrace_points[0] = -1
-    while main_pointer < len(pattern_string) - 1:
-        if pattern_pointer == -1 or pattern_string[pattern_pointer] == pattern_string[main_pointer]:
-            main_pointer += 1
-            pattern_pointer += 1
-            backtrace_points[main_pointer] = pattern_pointer
-        else:
-            pattern_pointer = backtrace_points[pattern_pointer]
-    return backtrace_points
-
-
-def find(main_string, pattern_string):
-    """
-    模式匹配
-    一边构建字串的回溯点，一边判断模式是否匹配
-    """
-    if len(main_string) < len(pattern_string):
-        return False
-    main_string = " " + main_string
-    backtrace_points = [0] * (len(main_string) + 1)
-    main_pointer, pattern_pointer = 0, -1
-    backtrace_points[0] = -1
-    while main_pointer < len(main_string):
-        if pattern_pointer == -1 or pattern_string[pattern_pointer] == main_string[main_pointer]:
-            if pattern_pointer == len(pattern_string) - 1:
-                return True
-            main_pointer += 1
-            pattern_pointer += 1
-            backtrace_points[main_pointer] = pattern_pointer
-        else:
-            pattern_pointer = backtrace_points[pattern_pointer]
-    return False
-
-
-if __name__ == '__main__':
-    test_main_string = "aa"
-    test_pattern_string = "aa"
-
-    res = build(test_pattern_string)
-    print(res)
-    res = find(test_main_string, test_pattern_string)
-    print(res)
+#!/usr/bin/python3.8
+# -*- coding: utf-8 -*-
+# @Author  : youshu.Ji
+
+def build(pattern_string):
+    """
+    构建模式串的PMT
+    [zhihu](https://www.zhihu.com/question/21923021/answer/281346746)
+
+    """
+    # 构建pattern需要回溯的位置，
+    backtrace_points = [0] * len(pattern_string)
+    main_pointer, pattern_pointer = 0, -1
+    backtrace_points[0] = -1
+    while main_pointer < len(pattern_string) - 1:
+        if pattern_pointer == -1 or pattern_string[pattern_pointer] == pattern_string[main_pointer]:
+            main_pointer += 1
+            pattern_pointer += 1
+            backtrace_points[main_pointer] = pattern_pointer
+        else:
+            pattern_pointer = backtrace_points[pattern_pointer]
+    return backtrace_points
+
+
+def build_2(needle: str):
+    # 这写的比第一种简洁
+    # 查找方法也是自己，唯一就是判断结束条件，不是用-1了
+    m = len(needle)
+    if m == 0:
+        return 0
+
+    pmt = [0] * m
+    pattern_pointer = 0
+    for main_pointer in range(1, m):
+        while pattern_pointer > 0 and needle[main_pointer] != needle[pattern_pointer]:
+            pattern_pointer = pmt[pattern_pointer - 1]
+        if needle[main_pointer] == needle[pattern_pointer]:
+            pattern_pointer += 1
+        pmt[main_pointer] = pattern_pointer
+    return pmt
+
+
+def find_after_build(main_string, pattern_string):
+    backtracker = build(pattern_string)
+    # print(backtracker)
+    main_pointer, pattern_pointer = -1, -1
+    while main_pointer <= len(main_string) - 1:
+        if pattern_pointer == -1 or pattern_string[pattern_pointer] == main_string[main_pointer]:
+            # 这是返回首次匹配时main的位置
+            if pattern_pointer == len(pattern_string) - 1:
+                return main_pointer - len(pattern_string) + 1
+            pattern_pointer += 1
+            main_pointer += 1
+        else:
+            pattern_pointer = backtracker[pattern_pointer]
+    return -1
+
+
+def find(main_string, pattern_string):
+    """
+    模式匹配
+    一边构建字串的回溯点，一边判断模式是否匹配
+    """
+    if len(main_string) < len(pattern_string):
+        return False
+    main_string = " " + main_string
+    backtrace_points = [0] * (len(main_string) + 1)
+    main_pointer, pattern_pointer = 0, -1
+    backtrace_points[0] = -1
+    while main_pointer < len(main_string):
+        if pattern_pointer == -1 or pattern_string[pattern_pointer] == main_string[main_pointer]:
+            if pattern_pointer == len(pattern_string) - 1:
+                return True
+            main_pointer += 1
+            pattern_pointer += 1
+            backtrace_points[main_pointer] = pattern_pointer
+        else:
+            pattern_pointer = backtrace_points[pattern_pointer]
+    return False
+
+
+if __name__ == '__main__':
+    test_main_string = "abababc"
+    test_pattern_string = "abababc"
+
+    res = build(test_pattern_string)
+    print(res)
+    res = build_2(test_pattern_string)
+    print(res)
+    # res = find(test_main_string, test_pattern_string)
+    # print(res)
+    #
+    # res = find_after_build(test_main_string, test_pattern_string)
+    # print(res)
```

### Comparing `nlpertools-1.0.5/src/nlpertools/openApi.py` & `nlpertools-1.0.6.dev0/src/nlpertools/open_api.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-#!/usr/bin/python3.8
-# -*- coding: utf-8 -*-
-# @Author  : youshu.Ji
-import hashlib
-import json
-import time
-import uuid
-
-# import requests
-from .utils.package import *
-
-
-def translate_by_youdao(text):
-    YOUDAO_URL = 'https://openapi.youdao.com/api'
-    APP_KEY = 'xx'
-    APP_SECRET = 'xx'
-
-    def _truncate(q):
-        if q is None:
-            return None
-        size = len(q)
-        return q if size <= 20 else q[0:10] + str(size) + q[size - 10:size]
-
-    def _do_request(data):
-        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
-        return requests.post(YOUDAO_URL, data=data, headers=headers)
-
-    def _encrypt(signStr):
-        hash_algorithm = hashlib.sha256()
-        hash_algorithm.update(signStr.encode('utf-8'))
-        return hash_algorithm.hexdigest()
-
-    q = text
-
-    data = {}
-    data['from'] = '源语言'
-    data['to'] = '目标语言'
-    data['signType'] = 'v3'
-    curtime = str(int(time.time()))
-    data['curtime'] = curtime
-    salt = str(uuid.uuid1())
-    signStr = APP_KEY + _truncate(q) + salt + curtime + APP_SECRET
-    sign = _encrypt(signStr)
-    data['appKey'] = APP_KEY
-    data['q'] = q
-    data['salt'] = salt
-    data['sign'] = sign
-    data['vocabId'] = "您的用户词表ID"
-    youdao_res = _do_request(data)
-    res = youdao_res.json()['translation'][0]
-    return res
-
-
-def get_TexSmart(text):
-    # text 可以是list， 也可以是str
-    # 如果是分类结果 total['cat_list']['name']
-    obj = {"str": text, "options": {"text_cat": {"enable": True}}}
-    req_str = json.dumps(obj).encode()
-
-    url = "https://texsmart.qq.com/api"
-    r = requests.post(url, data=req_str)
-    r.encoding = "utf-8"
-    print(r.text)
-    total = json.loads(r.text)
-    return total
+#!/usr/bin/python3.8
+# -*- coding: utf-8 -*-
+# @Author  : youshu.Ji
+import hashlib
+import json
+import time
+import uuid
+
+# import requests
+from .utils.package import *
+
+
+def translate_by_youdao(text):
+    YOUDAO_URL = 'https://openapi.youdao.com/api'
+    APP_KEY = 'xx'
+    APP_SECRET = 'xx'
+
+    def _truncate(q):
+        if q is None:
+            return None
+        size = len(q)
+        return q if size <= 20 else q[0:10] + str(size) + q[size - 10:size]
+
+    def _do_request(data):
+        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+        return requests.post(YOUDAO_URL, data=data, headers=headers)
+
+    def _encrypt(signStr):
+        hash_algorithm = hashlib.sha256()
+        hash_algorithm.update(signStr.encode('utf-8'))
+        return hash_algorithm.hexdigest()
+
+    q = text
+
+    data = {}
+    data['from'] = '源语言'
+    data['to'] = '目标语言'
+    data['signType'] = 'v3'
+    curtime = str(int(time.time()))
+    data['curtime'] = curtime
+    salt = str(uuid.uuid1())
+    signStr = APP_KEY + _truncate(q) + salt + curtime + APP_SECRET
+    sign = _encrypt(signStr)
+    data['appKey'] = APP_KEY
+    data['q'] = q
+    data['salt'] = salt
+    data['sign'] = sign
+    data['vocabId'] = "您的用户词表ID"
+    youdao_res = _do_request(data)
+    res = youdao_res.json()['translation'][0]
+    return res
+
+
+def get_TexSmart(text):
+    # text 可以是list， 也可以是str
+    # 如果是分类结果 total['cat_list']['name']
+    obj = {"str": text, "options": {"text_cat": {"enable": True}}}
+    req_str = json.dumps(obj).encode()
+
+    url = "https://texsmart.qq.com/api"
+    r = requests.post(url, data=req_str)
+    r.encoding = "utf-8"
+    print(r.text)
+    total = json.loads(r.text)
+    return total
```

### Comparing `nlpertools-1.0.5/src/nlpertools/utils_for_nlpertools.py` & `nlpertools-1.0.6.dev0/src/nlpertools/utils_for_nlpertools.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import os
-import shutil
-from importlib import import_module
-
-from .io.dir import j_mkdir
-from .io.file import readtxt_list_all_strip, writetxt_w_list
-
-
-def try_import(name, package):
-    try:
-        return import_module(name, package=package)
-    except:
-        print("import {} failed".format(name))
-    finally:
-        pass
-
-
-def convert_import_to_try_import(from_path, to_path):
-    j_mkdir(to_path)
-    for root, dirs, files in os.walk(from_path):
-        for sub_dir in dirs:
-            j_mkdir(os.path.join(root.replace(from_path, to_path), sub_dir))
-        for file in files:
-            src = os.path.join(root, file)
-            dst = os.path.join(root.replace(from_path, to_path), file)
-            excluded_file = ["wrapper.py", "kmp.py", "__init__.py"]
-            if file.endswith(".py") and file != "utils_for_nlpertools.py" and file not in excluded_file:
-                raw_code = readtxt_list_all_strip(src)
-                start_idx, end_idx = 0, 0
-
-                for idx, each_line in enumerate(raw_code[:30]):
-                    each_line = each_line.lstrip("# ")
-                    if start_idx == 0 and (each_line.startswith("from") or each_line.startswith("import")):
-                        try:
-                            exec(each_line)
-                        except:
-                            start_idx = idx
-                    if start_idx != 0 and not each_line:
-                        end_idx = idx
-                        break
-                # print(file, start_idx, end_idx)
-                if start_idx != 0 and end_idx != 0:
-                    new_code = raw_code[:start_idx] + convert_import_string_to_import_list(
-                        "\n".join(raw_code[start_idx:end_idx])) + raw_code[end_idx:]
-                else:
-                    new_code = raw_code
-                writetxt_w_list(new_code, dst)
-            else:
-                shutil.copy(src=src, dst=dst)
-    print("convert over")
-
-
-def get_import_info(text):
-    pass
-
-
-def convert_import_string_to_import_list(text):
-    """
-    该方法将 import 转变为 try import
-    """
-    models_to_import = []
-    import_list = text.split("\n")
-    for each in import_list:
-        print(each)
-        name, package, as_name = None, None, None
-        elements = each.split(" ")
-        for pre, cur in zip(elements, elements[1:]):
-            if cur.endswith(","):
-                cur = cur.rstrip(",")
-            # 为了实现from import 和 import统一，首先把package和name的含义反过来，后面再掉换
-            if pre == "import":
-                package = cur
-            if pre == "from":
-                name = cur
-            if pre == "as":
-                as_name = cur
-            if pre[-1] == ",":
-                # 针对 from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer
-                # 将将前面部分和当前的组成新字段
-                prefix = each.split("import")[0]
-                import_list.append("{}import {}".format(prefix, cur))
-        if not as_name:
-            as_name = package.split(".")[-1]
-        if not name:
-            name, package = package, name
-        models_to_import.append((name, package, as_name))
-    # 打印
-    all_import_info = ["", "from utils_for_nlpertools import try_import", ""]
-    for name, package, as_name in models_to_import:
-        import_info = '{} = try_import("{}", {})'.format(as_name, name, '"{}"'.format(package) if package else package)
-        all_import_info.append(import_info)
-        print(import_info)
-    return all_import_info
+import os
+import shutil
+from importlib import import_module
+
+from .io.dir import j_mkdir
+from .io.file import readtxt_list_all_strip, writetxt_w_list
+
+
+def try_import(name, package):
+    try:
+        return import_module(name, package=package)
+    except:
+        print("import {} failed".format(name))
+    finally:
+        pass
+
+
+def convert_import_to_try_import(from_path, to_path):
+    j_mkdir(to_path)
+    for root, dirs, files in os.walk(from_path):
+        for sub_dir in dirs:
+            j_mkdir(os.path.join(root.replace(from_path, to_path), sub_dir))
+        for file in files:
+            src = os.path.join(root, file)
+            dst = os.path.join(root.replace(from_path, to_path), file)
+            excluded_file = ["wrapper.py", "kmp.py", "__init__.py"]
+            if file.endswith(".py") and file != "utils_for_nlpertools.py" and file not in excluded_file:
+                raw_code = readtxt_list_all_strip(src)
+                start_idx, end_idx = 0, 0
+
+                for idx, each_line in enumerate(raw_code[:30]):
+                    each_line = each_line.lstrip("# ")
+                    if start_idx == 0 and (each_line.startswith("from") or each_line.startswith("import")):
+                        try:
+                            exec(each_line)
+                        except:
+                            start_idx = idx
+                    if start_idx != 0 and not each_line:
+                        end_idx = idx
+                        break
+                # print(file, start_idx, end_idx)
+                if start_idx != 0 and end_idx != 0:
+                    new_code = raw_code[:start_idx] + convert_import_string_to_import_list(
+                        "\n".join(raw_code[start_idx:end_idx])) + raw_code[end_idx:]
+                else:
+                    new_code = raw_code
+                writetxt_w_list(new_code, dst)
+            else:
+                shutil.copy(src=src, dst=dst)
+    print("convert over")
+
+
+def get_import_info(text):
+    pass
+
+
+def convert_import_string_to_import_list(text):
+    """
+    该方法将 import 转变为 try import
+    """
+    models_to_import = []
+    import_list = text.split("\n")
+    for each in import_list:
+        print(each)
+        name, package, as_name = None, None, None
+        elements = each.split(" ")
+        for pre, cur in zip(elements, elements[1:]):
+            if cur.endswith(","):
+                cur = cur.rstrip(",")
+            # 为了实现from import 和 import统一，首先把package和name的含义反过来，后面再掉换
+            if pre == "import":
+                package = cur
+            if pre == "from":
+                name = cur
+            if pre == "as":
+                as_name = cur
+            if pre[-1] == ",":
+                # 针对 from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer
+                # 将将前面部分和当前的组成新字段
+                prefix = each.split("import")[0]
+                import_list.append("{}import {}".format(prefix, cur))
+        if not as_name:
+            as_name = package.split(".")[-1]
+        if not name:
+            name, package = package, name
+        models_to_import.append((name, package, as_name))
+    # 打印
+    all_import_info = ["", "from utils_for_nlpertools import try_import", ""]
+    for name, package, as_name in models_to_import:
+        import_info = '{} = try_import("{}", {})'.format(as_name, name, '"{}"'.format(package) if package else package)
+        all_import_info.append(import_info)
+        print(import_info)
+    return all_import_info
```

### Comparing `nlpertools-1.0.5/src/nlpertools.egg-info/SOURCES.txt` & `nlpertools-1.0.6.dev0/src/nlpertools.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/nlpertools/__init__.py
 src/nlpertools/data_client.py
 src/nlpertools/dataprocess.py
+src/nlpertools/default_db_config.yml
 src/nlpertools/ml.py
-src/nlpertools/openApi.py
+src/nlpertools/movie.py
+src/nlpertools/nlpertools_config.yml
+src/nlpertools/open_api.py
 src/nlpertools/other.py
+src/nlpertools/pic.py
 src/nlpertools/plugin.py
 src/nlpertools/reminder.py
 src/nlpertools/utils_for_nlpertools.py
+src/nlpertools/vector_index_demo.py
 src/nlpertools/wrapper.py
 src/nlpertools.egg-info/PKG-INFO
 src/nlpertools.egg-info/SOURCES.txt
 src/nlpertools.egg-info/dependency_links.txt
 src/nlpertools.egg-info/top_level.txt
 src/nlpertools/algo/__init__.py
+src/nlpertools/algo/ac.py
+src/nlpertools/algo/bit_ops.py
 src/nlpertools/algo/kmp.py
+src/nlpertools/algo/num_ops.py
+src/nlpertools/algo/template.py
+src/nlpertools/algo/union.py
 src/nlpertools/data_structure/__init__.py
 src/nlpertools/data_structure/base_structure.py
 src/nlpertools/io/__init__.py
 src/nlpertools/io/dir.py
 src/nlpertools/io/file.py
+src/nlpertools/monitor/__init__.py
+src/nlpertools/monitor/gpu.py
+src/nlpertools/monitor/memory.py
 src/nlpertools/template/__init__.py
 src/nlpertools/utils/__init__.py
-src/nlpertools/utils/package.py
+src/nlpertools/utils/lazy.py
+src/nlpertools/utils/log_util.py
+src/nlpertools/utils/package.py
+src/nlpertools/utils/package_v1.py
+src/nlpertools/utils/package_v2.py
+src/nlpertools_helper/__init__.py
+tests/test_kmp.py
+tests/test_path_exists.py
```

