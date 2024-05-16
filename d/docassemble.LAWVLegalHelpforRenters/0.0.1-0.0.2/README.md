# Comparing `tmp/docassemble.LAWVLegalHelpforRenters-0.0.1.tar.gz` & `tmp/docassemble.LAWVLegalHelpforRenters-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.LAWVLegalHelpforRenters-0.0.1.tar", last modified: Mon May 13 14:31:20 2024, max compression
+gzip compressed data, was "docassemble.LAWVLegalHelpforRenters-0.0.2.tar", last modified: Thu May 16 14:11:38 2024, max compression
```

## Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1.tar` & `docassemble.LAWVLegalHelpforRenters-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-13 14:31:20.277358 docassemble.LAWVLegalHelpforRenters-0.0.1/
--rw-r--r--   0 www-data    (33) www-data    (33)     1087 2024-05-13 14:31:06.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/LICENSE
--rw-r--r--   0 www-data    (33) www-data    (33)       18 2024-05-13 14:31:06.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/MANIFEST.in
--rw-r--r--   0 www-data    (33) www-data    (33)      638 2024-05-13 14:31:20.277358 docassemble.LAWVLegalHelpforRenters-0.0.1/PKG-INFO
--rw-r--r--   0 www-data    (33) www-data    (33)      317 2024-05-13 14:31:06.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/README.md
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-13 14:31:20.273358 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-13 14:31:20.273358 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/
--rw-r--r--   0 www-data    (33) www-data    (33)       22 2024-05-13 14:31:06.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/__init__.py
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-13 14:31:20.273358 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-13 14:31:20.273358 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/
--rw-r--r--   0 www-data    (33) www-data    (33)     3807 2024-05-13 14:20:37.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/informal_hearing_request.yml
--rw-r--r--   0 www-data    (33) www-data    (33)     8743 2024-05-13 14:20:10.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/petition_for_appeal.yml
--rw-r--r--   0 www-data    (33) www-data    (33)     5070 2024-05-13 14:20:30.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/return_of_security_deposit.yml
--rw-r--r--   0 www-data    (33) www-data    (33)     4747 2024-05-13 14:20:18.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/warranty_of_habitability.yml
--rw-r--r--   0 www-data    (33) www-data    (33)     9661 2024-05-13 14:20:50.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/wrongful_occ_answer.yml
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-13 14:31:20.273358 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/sources/
--rw-r--r--   0 www-data    (33) www-data    (33)      134 2024-05-13 14:31:06.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/sources/README.md
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-13 14:31:20.277358 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/static/
--rw-r--r--   0 www-data    (33) www-data    (33)      105 2024-05-13 14:31:06.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/static/README.md
--rw-r--r--   0 www-data    (33) www-data    (33)   352046 2023-12-12 18:28:39.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/static/civil_judgment_order_rental.png
--rw-r--r--   0 www-data    (33) www-data    (33)   905259 2023-12-11 15:27:40.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/static/wrongful_occupation_petition.png
--rw-r--r--   0 www-data    (33) www-data    (33)  1176014 2023-12-11 15:27:40.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/static/wrongful_occupation_summons.png
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-13 14:31:20.277358 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/
--rw-r--r--   0 www-data    (33) www-data    (33)      102 2024-05-13 14:31:06.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/README.md
--rw-r--r--   0 www-data    (33) www-data    (33)    28179 2024-04-09 14:28:00.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/informal_hearing_eviction.docx
--rw-r--r--   0 www-data    (33) www-data    (33)    28440 2024-04-09 14:28:00.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/informal_hearing_termination.docx
--rw-r--r--   0 www-data    (33) www-data    (33)    18201 2024-01-30 15:34:46.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/notice_of_warranty_of_habitability.docx
--rw-r--r--   0 www-data    (33) www-data    (33)    20403 2024-05-02 17:45:32.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/notice_to_acknowledge_stay.docx
--rw-r--r--   0 www-data    (33) www-data    (33)    64943 2024-05-02 17:45:32.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/petition_for_appeal.pdf
--rw-r--r--   0 www-data    (33) www-data    (33)    14125 2024-01-30 16:13:57.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/return_of_security_deposit.docx
--rw-r--r--   0 www-data    (33) www-data    (33)   199223 2023-12-12 14:10:27.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/wrongful_occupation_answer.pdf
--rw-r--r--   0 www-data    (33) www-data    (33)       57 2024-05-13 14:31:06.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/__init__.py
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-13 14:31:20.273358 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/
--rw-r--r--   0 www-data    (33) www-data    (33)      638 2024-05-13 14:31:20.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/PKG-INFO
--rw-r--r--   0 www-data    (33) www-data    (33)     1932 2024-05-13 14:31:20.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/SOURCES.txt
--rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-05-13 14:31:20.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/dependency_links.txt
--rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-05-13 14:31:20.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/namespace_packages.txt
--rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-05-13 14:31:20.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/not-zip-safe
--rw-r--r--   0 www-data    (33) www-data    (33)       30 2024-05-13 14:31:20.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/requires.txt
--rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-05-13 14:31:20.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/top_level.txt
--rw-r--r--   0 www-data    (33) www-data    (33)       79 2024-05-13 14:31:20.277358 docassemble.LAWVLegalHelpforRenters-0.0.1/setup.cfg
--rw-r--r--   0 www-data    (33) www-data    (33)     2749 2024-05-13 14:31:06.000000 docassemble.LAWVLegalHelpforRenters-0.0.1/setup.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-16 14:11:37.999577 docassemble.LAWVLegalHelpforRenters-0.0.2/
+-rw-r--r--   0 www-data    (33) www-data    (33)     1087 2024-05-16 14:11:25.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/LICENSE
+-rw-r--r--   0 www-data    (33) www-data    (33)       18 2024-05-16 14:11:25.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/MANIFEST.in
+-rw-r--r--   0 www-data    (33) www-data    (33)      638 2024-05-16 14:11:37.999577 docassemble.LAWVLegalHelpforRenters-0.0.2/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)      317 2024-05-16 14:11:25.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-16 14:11:37.995577 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-16 14:11:37.995577 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/
+-rw-r--r--   0 www-data    (33) www-data    (33)       22 2024-05-16 14:11:25.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-16 14:11:37.995577 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-16 14:11:37.995577 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/
+-rw-r--r--   0 www-data    (33) www-data    (33)     3807 2024-05-13 14:20:37.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/informal_hearing_request.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     8743 2024-05-13 14:20:10.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/petition_for_appeal.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     5070 2024-05-13 14:20:30.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/return_of_security_deposit.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     4747 2024-05-13 14:20:18.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/warranty_of_habitability.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     9591 2024-05-16 14:07:07.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/wrongful_occ_answer.yml
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-16 14:11:37.995577 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/sources/
+-rw-r--r--   0 www-data    (33) www-data    (33)      134 2024-05-16 14:11:25.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/sources/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-16 14:11:37.999577 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/static/
+-rw-r--r--   0 www-data    (33) www-data    (33)      105 2024-05-16 14:11:25.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/static/README.md
+-rw-r--r--   0 www-data    (33) www-data    (33)   352046 2023-12-12 18:28:39.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/static/civil_judgment_order_rental.png
+-rw-r--r--   0 www-data    (33) www-data    (33)   905259 2023-12-11 15:27:40.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/static/wrongful_occupation_petition.png
+-rw-r--r--   0 www-data    (33) www-data    (33)  1176014 2023-12-11 15:27:40.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/static/wrongful_occupation_summons.png
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-16 14:11:37.999577 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/
+-rw-r--r--   0 www-data    (33) www-data    (33)      102 2024-05-16 14:11:25.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/README.md
+-rw-r--r--   0 www-data    (33) www-data    (33)    28179 2024-04-09 14:28:00.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/informal_hearing_eviction.docx
+-rw-r--r--   0 www-data    (33) www-data    (33)    28440 2024-04-09 14:28:00.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/informal_hearing_termination.docx
+-rw-r--r--   0 www-data    (33) www-data    (33)    18201 2024-01-30 15:34:46.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/notice_of_warranty_of_habitability.docx
+-rw-r--r--   0 www-data    (33) www-data    (33)    20403 2024-05-02 17:45:32.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/notice_to_acknowledge_stay.docx
+-rw-r--r--   0 www-data    (33) www-data    (33)    64943 2024-05-02 17:45:32.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/petition_for_appeal.pdf
+-rw-r--r--   0 www-data    (33) www-data    (33)    14125 2024-01-30 16:13:57.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/return_of_security_deposit.docx
+-rw-r--r--   0 www-data    (33) www-data    (33)   199223 2023-12-12 14:10:27.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/wrongful_occupation_answer.pdf
+-rw-r--r--   0 www-data    (33) www-data    (33)       57 2024-05-16 14:11:25.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-05-16 14:11:37.995577 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/
+-rw-r--r--   0 www-data    (33) www-data    (33)      638 2024-05-16 14:11:37.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)     1932 2024-05-16 14:11:37.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/SOURCES.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-05-16 14:11:37.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/dependency_links.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-05-16 14:11:37.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/namespace_packages.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-05-16 14:11:37.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/not-zip-safe
+-rw-r--r--   0 www-data    (33) www-data    (33)       30 2024-05-16 14:11:37.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/requires.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-05-16 14:11:37.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/top_level.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       79 2024-05-16 14:11:37.999577 docassemble.LAWVLegalHelpforRenters-0.0.2/setup.cfg
+-rw-r--r--   0 www-data    (33) www-data    (33)     2749 2024-05-16 14:11:25.000000 docassemble.LAWVLegalHelpforRenters-0.0.2/setup.py
```

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/LICENSE` & `docassemble.LAWVLegalHelpforRenters-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/PKG-INFO` & `docassemble.LAWVLegalHelpforRenters-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.LAWVLegalHelpforRenters
-Version: 0.0.1
+Version: 0.0.2
 Summary: A docassemble extension.
 Home-page: https://docassemble.org
 Author: System Administrator
 Author-email: dhenry@lawv.net
 License: The MIT License (MIT)
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/informal_hearing_request.yml` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/informal_hearing_request.yml`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/petition_for_appeal.yml` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/petition_for_appeal.yml`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/return_of_security_deposit.yml` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/return_of_security_deposit.yml`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/warranty_of_habitability.yml` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/warranty_of_habitability.yml`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/questions/wrongful_occ_answer.yml` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/questions/wrongful_occ_answer.yml`

 * *Files 4% similar despite different names*

```diff
@@ -298,16 +298,15 @@
           admitting = "No"
           denying = "Yes"
 
         generate_wrongful_occupation_answer
         success_exit
     else:
       # Should go to appeal once written
-      failure_reason = "Your hearing has already been held and you have been ordered to leave your property.  You need to file an appeal."
-      ineligible
+      command('leave', url="https://iolaw.net/start/LAWV%20Petition%20for%20Appeal/")
   else:
     failure_reason = "If you have not received a summons and complaint, there is no need to file an answer at this time."
     ineligible
 ---
 code: |
   detail = ""
   if warranty["electricity"]:
```

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/static/civil_judgment_order_rental.png` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/static/civil_judgment_order_rental.png`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/static/wrongful_occupation_petition.png` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/static/wrongful_occupation_petition.png`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/static/wrongful_occupation_summons.png` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/static/wrongful_occupation_summons.png`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/informal_hearing_eviction.docx` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/informal_hearing_eviction.docx`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/informal_hearing_termination.docx` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/informal_hearing_termination.docx`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/notice_of_warranty_of_habitability.docx` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/notice_of_warranty_of_habitability.docx`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/notice_to_acknowledge_stay.docx` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/notice_to_acknowledge_stay.docx`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/petition_for_appeal.pdf` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/petition_for_appeal.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/return_of_security_deposit.docx` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/return_of_security_deposit.docx`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble/LAWVLegalHelpforRenters/data/templates/wrongful_occupation_answer.pdf` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble/LAWVLegalHelpforRenters/data/templates/wrongful_occupation_answer.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/PKG-INFO` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.LAWVLegalHelpforRenters
-Version: 0.0.1
+Version: 0.0.2
 Summary: A docassemble extension.
 Home-page: https://docassemble.org
 Author: System Administrator
 Author-email: dhenry@lawv.net
 License: The MIT License (MIT)
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/docassemble.LAWVLegalHelpforRenters.egg-info/SOURCES.txt` & `docassemble.LAWVLegalHelpforRenters-0.0.2/docassemble.LAWVLegalHelpforRenters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVLegalHelpforRenters-0.0.1/setup.py` & `docassemble.LAWVLegalHelpforRenters-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.LAWVLegalHelpforRenters',
-      version='0.0.1',
+      version='0.0.2',
       description=('A docassemble extension.'),
       long_description='Source package for the LAWV Legal Help for Renters project that will allow users to create documents for: 1) Answer to Wrongful Occupation\r\n2) Breach of Warranty of Habitability Letter\r\n3) Petition for Appeal from Bench Trial\r\n4) Public Housing Authority Informal Hearing Request\r\n5) Return of Security Deposit Letter',
       long_description_content_type='text/markdown',
       author='System Administrator',
       author_email='dhenry@lawv.net',
       license='The MIT License (MIT)',
       url='https://docassemble.org',
```

