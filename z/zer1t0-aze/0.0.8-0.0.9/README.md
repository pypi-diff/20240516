# Comparing `tmp/zer1t0_aze-0.0.8.tar.gz` & `tmp/zer1t0_aze-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zer1t0_aze-0.0.8.tar", last modified: Wed May  1 19:39:08 2024, max compression
+gzip compressed data, was "zer1t0_aze-0.0.9.tar", last modified: Sun May  5 14:43:00 2024, max compression
```

## Comparing `zer1t0_aze-0.0.8.tar` & `zer1t0_aze-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,53 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-01 19:39:08.661866 zer1t0_aze-0.0.8/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     2816 2024-05-01 19:39:08.657866 zer1t0_aze-0.0.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2396 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-01 19:39:08.657866 zer1t0_aze-0.0.8/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      767 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/arm_api.py
--rw-rw-r--   0 user      (1000) user      (1000)     1741 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_add_app_secret.py
--rw-rw-r--   0 user      (1000) user      (1000)     3167 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_blob_containers.py
--rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_passwords.py
--rw-rw-r--   0 user      (1000) user      (1000)     7007 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_service_subdomains.py
--rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_brute_usernames.py
--rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_get_tenant_domains.py
--rw-rw-r--   0 user      (1000) user      (1000)      982 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_get_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)      787 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_administrative_unit_members.py
--rw-rw-r--   0 user      (1000) user      (1000)      804 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_administrative_unit_role_members.py
--rw-rw-r--   0 user      (1000) user      (1000)     3369 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_blobs.py
--rw-rw-r--   0 user      (1000) user      (1000)     1109 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_role_assignment.py
--rw-rw-r--   0 user      (1000) user      (1000)      800 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_sp_app_role_assignment.py
--rw-rw-r--   0 user      (1000) user      (1000)      813 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_list_user_memberof.py
--rw-rw-r--   0 user      (1000) user      (1000)     9478 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)     2434 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_search_token_in_cache.py
--rw-rw-r--   0 user      (1000) user      (1000)      746 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_show_ad_role.py
--rw-rw-r--   0 user      (1000) user      (1000)      771 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_show_administrative_unit.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)       80 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/error.py
--rw-rw-r--   0 user      (1000) user      (1000)     1814 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/graph_api.py
--rw-rw-r--   0 user      (1000) user      (1000)     1248 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/permutations.py
--rw-rw-r--   0 user      (1000) user      (1000)      817 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/profile.py
--rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      960 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/request_az.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)     2882 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/tokens.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/aze/version.py
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-01 19:39:08.661866 zer1t0_aze-0.0.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1653 2024-05-01 19:38:49.000000 zer1t0_aze-0.0.8/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-01 19:39:08.657866 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2816 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1042 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1205 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-05-01 19:39:08.000000 zer1t0_aze-0.0.8/zer1t0_aze.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-05 14:43:00.418987 zer1t0_aze-0.0.9/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3123 2024-05-05 14:43:00.418987 zer1t0_aze-0.0.9/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2703 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-05 14:43:00.414986 zer1t0_aze-0.0.9/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2111 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/arm_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1781 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_brute_add_app_secret.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3167 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_brute_blob_containers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_brute_passwords.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7007 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_brute_service_subdomains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_brute_usernames.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1561 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_download_blob.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1049 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_download_deployment_template.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_get_tenant_domains.py
+-rw-rw-r--   0 user      (1000) user      (1000)      982 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_get_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)      787 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_list_administrative_unit_members.py
+-rw-rw-r--   0 user      (1000) user      (1000)      804 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_list_administrative_unit_role_members.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1750 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_list_blobs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1109 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_list_role_assignment.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1028 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_list_sp_app_role_assignment.py
+-rw-rw-r--   0 user      (1000) user      (1000)      813 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_list_user_memberof.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1012 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_list_vm_extensions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1014 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_list_vm_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4982 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2434 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_search_token_in_cache.py
+-rw-rw-r--   0 user      (1000) user      (1000)      746 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_show_ad_role.py
+-rw-rw-r--   0 user      (1000) user      (1000)      771 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_show_administrative_unit.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)       80 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/error.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2063 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/graph_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1248 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/permutations.py
+-rw-rw-r--   0 user      (1000) user      (1000)      817 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/profile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      996 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/request_az.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4664 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/storage_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9005 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/tokens.py
+-rw-rw-r--   0 user      (1000) user      (1000)      565 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/aze/version.py
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-05 14:43:00.418987 zer1t0_aze-0.0.9/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1775 2024-05-05 14:22:19.000000 zer1t0_aze-0.0.9/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-05 14:43:00.418987 zer1t0_aze-0.0.9/zer1t0_aze.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3123 2024-05-05 14:43:00.000000 zer1t0_aze-0.0.9/zer1t0_aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1183 2024-05-05 14:43:00.000000 zer1t0_aze-0.0.9/zer1t0_aze.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-05 14:43:00.000000 zer1t0_aze-0.0.9/zer1t0_aze.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1437 2024-05-05 14:43:00.000000 zer1t0_aze-0.0.9/zer1t0_aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-05-05 14:43:00.000000 zer1t0_aze-0.0.9/zer1t0_aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-05-05 14:43:00.000000 zer1t0_aze-0.0.9/zer1t0_aze.egg-info/top_level.txt
```

### Comparing `zer1t0_aze-0.0.8/LICENSE` & `zer1t0_aze-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/PKG-INFO` & `zer1t0_aze-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zer1t0-aze
-Version: 0.0.8
+Version: 0.0.9
 Summary: Enhance azure cli
 Home-page: https://gitlab.com/Zer1t0/aze
 Author: Eloy Pérez González
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,26 +25,30 @@
 AZE includes the following commands, many of them require to be
 authenticated (marked with Auth) in Azure:
 
 - **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
-  subdomains (No auth).
-- **az-brute-blob-containers**: Discover public containers in Azure blobs (No auth).
+  subdomains. (No auth)
+- **az-brute-blob-containers**: Discover public containers in Azure blobs. (No auth)
+- **az-download-blob**: Download blob from URL. (Auth with -a parameter)
+- **az-download-deployment-template**: Download a deployment template. (Auth)
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
-- **az-list-blobs**: List blobs of container from URL (No auth).
+- **az-list-blobs**: List blobs or containers from URL. (Auth with -a parameter)
 - **az-list-administrative-unit-members**: List Administrative Unit members (Auth).
 - **az-list-administrative-unit-role-members**: List Administrative Unit scoped role members (Auth).
 - **az-list-role-assignment**: List roles without requiring a graph access token. (Auth)
 - **az-list-sp-app-role-assignment**: List App roles for a service principal. (Auth)
 - **az-list-user-memberof**: List membership of user, both groups and administrative units. (Auth)
+- **az-list-vm-extensions**: List virtual machine extensions. (Auth)
+- **az-list-vm-permissions**: List virtual machine permissions. (Auth)
 - **az-login-with-token**: Injects tokens directly into Azure Cli token cache.
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-show-ad-role**: Show Entra ID role. (Auth)
 - **az-show-administrative-unit**: Show Administrative Unit. (Auth)
 - **az-whoami**: Shorcut for "az ad signed-in-user show". (Auth)
 
 ## Installation
```

### Comparing `zer1t0_aze-0.0.8/README.md` & `zer1t0_aze-0.0.9/zer1t0_aze.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: zer1t0-aze
+Version: 0.0.9
+Summary: Enhance azure cli
+Home-page: https://gitlab.com/Zer1t0/aze
+Author: Eloy Pérez González
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: msal_extensions
+Requires-Dist: dnspython
+
 # AZE (Azure Cli Enhacement)
 
 Extended utilities for azure management.
 
 A python package intended to be used along with Azure Cli to expand its
 capabilities, even if many commands are completely independent from Azure Cli.
 
@@ -11,26 +25,30 @@
 AZE includes the following commands, many of them require to be
 authenticated (marked with Auth) in Azure:
 
 - **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
-  subdomains (No auth).
-- **az-brute-blob-containers**: Discover public containers in Azure blobs (No auth).
+  subdomains. (No auth)
+- **az-brute-blob-containers**: Discover public containers in Azure blobs. (No auth)
+- **az-download-blob**: Download blob from URL. (Auth with -a parameter)
+- **az-download-deployment-template**: Download a deployment template. (Auth)
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
-- **az-list-blobs**: List blobs of container from URL (No auth).
+- **az-list-blobs**: List blobs or containers from URL. (Auth with -a parameter)
 - **az-list-administrative-unit-members**: List Administrative Unit members (Auth).
 - **az-list-administrative-unit-role-members**: List Administrative Unit scoped role members (Auth).
 - **az-list-role-assignment**: List roles without requiring a graph access token. (Auth)
 - **az-list-sp-app-role-assignment**: List App roles for a service principal. (Auth)
 - **az-list-user-memberof**: List membership of user, both groups and administrative units. (Auth)
+- **az-list-vm-extensions**: List virtual machine extensions. (Auth)
+- **az-list-vm-permissions**: List virtual machine permissions. (Auth)
 - **az-login-with-token**: Injects tokens directly into Azure Cli token cache.
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-show-ad-role**: Show Entra ID role. (Auth)
 - **az-show-administrative-unit**: Show Administrative Unit. (Auth)
 - **az-whoami**: Shorcut for "az ad signed-in-user show". (Auth)
 
 ## Installation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zer1t0_aze-0.0.8/aze/az_brute_add_app_secret.py` & `zer1t0_aze-0.0.9/aze/az_brute_add_app_secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
     for app in applications:
         try:
             logging.info("Try to add secret to app {} ({})".format(
                 app["id"], app["displayName"]
             ))
             resp = graph_api.add_secret_to_application(access_token_raw, app["id"])
             resp["app"] = {
-                "id": app["id"],
+                "oid": app["id"],
+                "appId": app["appId"],
                 "displayName": app["displayName"]
             }
             print(json.dumps(resp, indent=4))
         except AzeRequestError as e:
             logging.debug("Error {}".format(e))
```

### Comparing `zer1t0_aze-0.0.8/aze/az_brute_blob_containers.py` & `zer1t0_aze-0.0.9/aze/az_brute_blob_containers.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_brute_passwords.py` & `zer1t0_aze-0.0.9/aze/az_brute_passwords.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_brute_service_subdomains.py` & `zer1t0_aze-0.0.9/aze/az_brute_service_subdomains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_brute_usernames.py` & `zer1t0_aze-0.0.9/aze/az_brute_usernames.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_get_login_info.py` & `zer1t0_aze-0.0.9/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_get_tenant_domains.py` & `zer1t0_aze-0.0.9/aze/az_get_tenant_domains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_get_tenant_id.py` & `zer1t0_aze-0.0.9/aze/az_get_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_inspect_token.py` & `zer1t0_aze-0.0.9/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_list_administrative_unit_members.py` & `zer1t0_aze-0.0.9/aze/az_list_administrative_unit_members.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_list_administrative_unit_role_members.py` & `zer1t0_aze-0.0.9/aze/az_list_administrative_unit_role_members.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_list_role_assignment.py` & `zer1t0_aze-0.0.9/aze/az_list_role_assignment.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_list_sp_app_role_assignment.py` & `zer1t0_aze-0.0.9/aze/az_list_vm_permissions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 import argparse
 from . import arm_api
-import json
 from . import profile
 from .tokens import search_token_for_subscription
-from . import arm_api, graph_api
+import json
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        "List App roles for a service principal."
+        "List virtual machine permissions."
+    )
+
+    parser.add_argument(
+        "-g","--resource-group",
+        help="VM Resource group name",
     )
 
-    parser.add_argument("id", help="Service Principal ID")
+    parser.add_argument(
+        "--vm-name",
+        help="VM name",
+    )
 
     args = parser.parse_args()
     return args
 
 def main():
     args = parse_args()
 
-    sp_id = args.id
+    resource_group_name = args.resource_group
+    vm_name = args.vm_name
 
     default_sub = profile.get_profile_default_subscription()
     access_token_obj = search_token_for_subscription(
         default_sub,
-        scopes=["https://graph.microsoft.com//.default"]
+        scopes=["https://management.core.windows.net//.default"]
     )
+
     access_token_raw = access_token_obj["secret"]
-    roles = graph_api.list_sp_app_role_asignments(access_token_raw, sp_id)
 
-    print(json.dumps(roles, indent=4))
+    resp = arm_api.list_vm_permissions(
+        access_token_raw,
+        default_sub["id"],
+        resource_group_name,
+        vm_name,
+    )
+
+    print(json.dumps(resp, indent=4))
```

### Comparing `zer1t0_aze-0.0.8/aze/az_list_user_memberof.py` & `zer1t0_aze-0.0.9/aze/az_list_user_memberof.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_login_with_token.py` & `zer1t0_aze-0.0.9/aze/tokens.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,178 +1,163 @@
-import argparse
+
+from msal_extensions import FilePersistenceWithDataProtection,\
+    KeychainPersistence, LibsecretPersistence, FilePersistence,\
+    PersistedTokenCache
+import os
+from .error import AzeError
+from . import utils
 import requests
-import base64
 import json
+import base64
 import time
-import configparser
-import os
-from . import utils
-from .tenant import resolve_tenant_id
-from .error import AzeError
-from .tokens import load_token_cache
-from . import arm_api
-from . import profile
-
-def parse_args():
-    parser = argparse.ArgumentParser(description="Login with Azure Tokens")
-    main_token_group = parser.add_mutually_exclusive_group(required=True)
-    main_token_group.add_argument(
-        "-a", "--access-token",
-        help="Access token for any Azure service.",
-        action='append',
-    )
-    main_token_group.add_argument(
-        "-r", "--refresh-token",
-        help="Refresh token",
-    )
 
-    parser.add_argument(
-        "--tenant",
-        help="Tenant domain or ID. Required when refresh token is used."
+CredentialType = PersistedTokenCache.CredentialType
+
+# class CredentialType:
+#         ACCESS_TOKEN = "AccessToken"
+#         REFRESH_TOKEN = "RefreshToken"
+#         ACCOUNT = "Account"  # Not exactly a credential type, but we put it here
+#         ID_TOKEN = "IdToken"
+#         APP_METADATA = "AppMetadata"
+
+def search_token_for_subscription(subscription, scopes, token_cache=None):
+    token_cache = token_cache or load_token_cache()
+
+    query = {
+        "username": subscription["user"]["name"],
+        "realm": subscription["tenantId"],
+    }
+
+    accounts = search_token_in_cache(
+        CredentialType.ACCOUNT,
+        query=query,
+        token_cache=token_cache,
     )
+    if not accounts and subscription["id"] != subscription["tenantId"]:
+        query["realm"] = "organizations"
+        accounts = search_token_in_cache(
+            CredentialType.ACCOUNT,
+            query=query,
+            token_cache=token_cache,
+        )
 
-    return parser.parse_args()
+    if not accounts:
+        raise AzeError("Unable to find account for subscription")
 
-def main():
-    args = parse_args()
-    access_tokens = args.access_token
-    refresh_token = args.refresh_token
-    tenant = args.tenant
-
-
-    resp_subscriptions = []
-    if access_tokens:
-        t_infos = [TokenInformation(at) for at in access_tokens]
-    elif refresh_token:
-        if not tenant:
-            utils.eprint("--tenant required when using refresh token")
-            return -1
-        tenant_id = resolve_tenant_id(tenant)
-        tokens = request_tokens_from_refresh(tenant_id, refresh_token)
+    account = accounts[0]
+
+    access_tokens = search_token_in_cache(
+        CredentialType.ACCESS_TOKEN,
+        query={"home_account_id": account["home_account_id"]},
+        scopes=scopes,
+        token_cache=token_cache,
+    )
+
+    if not access_tokens:
+        refresh_token_obj = search_token_in_cache(
+            CredentialType.REFRESH_TOKEN,
+            query={"home_account_id": account["home_account_id"]},
+            token_cache=token_cache,
+        )
+        if not refresh_token_obj:
+            raise AzeError(
+                "Unable to find Access Token (or Refresh Token) for account '{}' with scope '{}'".format(
+                    account["home_account_id"],
+                    ", ".join(scopes),
+                ))
+
+        tokens = request_tokens_from_refresh(
+            subscription["tenantId"],
+            refresh_token_obj[0]["secret"],
+            " ".join(scopes),
+        )
 
         at_info = TokenInformation(
             tokens["access_token"],
             refresh_token=tokens["refresh_token"],
             id_token=tokens["id_token"],
             scope=tokens["scope"],
             client_info=tokens["client_info"],
             expires_in=tokens["expires_in"],
             ext_expires_in=tokens["ext_expires_in"],
         )
-        t_infos = [at_info]
-
-    for t_info in t_infos:
-        if t_info.endpoint == "https://management.core.windows.net/"\
-           or t_info["aud"] == "https://management.azure.com/":
-            resp_subscriptions = arm_api.list_subscriptions(
-                t_info.access_token
-            )
-            break
 
-    token_cache = load_token_cache()
-    store_tokens(t_infos, token_cache)
-    set_subscriptions(t_infos[0], resp_subscriptions)
+        store_tokens([at_info], token_cache)
 
+        access_tokens = search_token_in_cache(
+            CredentialType.ACCESS_TOKEN,
+            query={"home_account_id": account["home_account_id"]},
+            scopes=scopes,
+            token_cache=token_cache,
+        )
 
+    if not access_tokens:
+        raise AzeError(
+                "Unable to find Access Token for account '{}' with scope '{}'".format(
+                    account["home_account_id"],
+                    ", ".join(scopes),
+                ))
+
+
+    return access_tokens[0]
+
+def search_token_in_cache(
+        token_type,
+        query=None,
+        scopes=None,
+        token_cache=None
+):
+    token_cache = token_cache or load_token_cache()
+    return token_cache.find(token_type, query=query, target=scopes)
+
+
+def load_token_cache(encrypted=False):
+    azure_dir = os.path.join(os.environ["HOME"], ".azure")
+    extension = "json" if not encrypted else "bin"
+    return load_persisted_token_cache(
+        os.path.join(azure_dir, "msal_token_cache.{}".format(extension)),
+        encrypted
+    )
 
 
-# A simple implementation of Profile._set_subscriptions
-# https://github.com/Azure/azure-cli/blob/6771b2b1ef04ed2f8e71b636eccce5cf68a7d76d/src/azure-cli-core/azure/cli/core/_profile.py#L454
-def set_subscriptions(at_info, resp_subscriptions):
-    default_subscription_id = store_profiles(at_info, resp_subscriptions)
-    set_default_subscription_id(default_subscription_id)
-
-AZURE_CLOUD = "AzureCloud"
-
-def store_profiles(at_info, resp_subscriptions):
-    tenant_id = at_info["tid"]
-    username = at_info.username
-
-    # To use tokens user type must be "user" since "servicePrincipal"
-    # is reserved to use the secrets store
-    user_type = "user"
-
-    profile_data = profile.load_profile()
-
-    cached_subscriptions = {}
-    for sub in profile_data["subscriptions"]:
-        sub["isDefault"] = False
-        cached_subscriptions[sub["id"]] = sub
-
-
-    can_be_default = True
-    new_subscriptions = {}
-    if resp_subscriptions:
-        for rsub in resp_subscriptions:
-            sub_id = rsub["subscriptionId"]
-            state = rsub["state"]
-            is_default = state == "Enabled" and can_be_default
-            if is_default:
-                can_be_default = False
-
-            new_subscriptions[sub_id] = {
-                "id": sub_id,
-                "name": rsub["displayName"],
-                "state": state,
-                "isDefault": is_default,
-                "tenantId": tenant_id,
-                "environmentName": AZURE_CLOUD,
-                "user": {
-                    "name": username,
-                    "type": user_type,
-                }
-            }
+def load_persisted_token_cache(location, encrypt):
+    persistence = build_persistence(location, encrypt)
+    return PersistedTokenCache(persistence)
+
+def build_persistence(location, encrypt):
+    if encrypt:
+        if sys.platform.startswith('win'):
+            return FilePersistenceWithDataProtection(location)
+        if sys.platform.startswith('darwin'):
+            return KeychainPersistence(
+                location,
+                "my_service_name",
+                "my_account_name"
+            )
+        if sys.platform.startswith('linux'):
+            return LibsecretPersistence(
+                location,
+                schema_name="my_schema_name",
+                attributes={"my_attr1": "foo", "my_attr2": "bar"}
+            )
     else:
-        new_subscriptions[tenant_id] = {
-            "id": tenant_id,
-            "name": "N/A(tenant level account)",
-            "state": "Enabled",
-            "isDefault": True,
-            "tenantId": tenant_id,
-            "environmentName": AZURE_CLOUD,
-            "user": {
-                "name": username,
-                "type": user_type,
-            }
-        }
-
-    cached_subscriptions.update(new_subscriptions)
-    default_subscription_id = [
-        s["id"]
-        for s in cached_subscriptions.values()
-        if s["isDefault"]
-    ][0]
-    profile_data["subscriptions"] = list(cached_subscriptions.values())
-
-    profile.store_profile(profile_data)
-    return default_subscription_id
-
-def set_default_subscription_id(default_subscription_id):
-    config_file = "{}/.azure/clouds.config".format(os.environ["HOME"])
-    config = configparser.ConfigParser()
-    config.read(config_file)
-    config.set(AZURE_CLOUD, "subscription", default_subscription_id)
+        return FilePersistence(location)
 
-    with open(config_file, 'w') as fo:
-        config.write(fo)
 
-
-AZCLI_ID = "04b07795-8ddb-461a-bbee-02f9e1bf7b46"
-
-def request_tokens_from_refresh(tenant_id, refresh_token):
+def request_tokens_from_refresh(tenant_id, refresh_token, scope):
     url = "https://login.microsoftonline.com/{}/oauth2/v2.0/token".format(
         tenant_id
     )
     data = {
-        "client_id": AZCLI_ID,
+        "client_id": utils.AZCLI_ID,
         "grant_type": "refresh_token",
         "client_info": 1,
         "claims": '{"access_token": {"xms_cc": {"values": ["CP1"]}}}',
         "refresh_token": refresh_token,
-        "scope": "https://management.core.windows.net//.default offline_access openid profile",
+        "scope": scope
     }
 
     resp = requests.post(url, data)
     if resp.status_code != 200:
         raise AzeError(
             "Unable to get access token, error {}: {} - {}".format(
                 resp.status_code,
@@ -180,14 +165,15 @@
                 resp.json().get("error_description", "")
             )
         )
 
     return resp.json()
 
 
+
 def store_tokens(tokens_info, token_cache):
     if not tokens_info:
         return
 
     tokens_events = [create_event_from_token_info(t_info) for t_info in tokens_info]
     for t_event in tokens_events:
         token_cache.add(t_event)
@@ -292,15 +278,15 @@
     if t_info.refresh_token:
         resp["refresh_token"] = t_info.refresh_token
     if t_info.id_token:
         resp["id_token"] = t_info.id_token
 
     # No matter what is t_info["appid"] since we tell the Azure Cli
     # to use the token as it belongs to it
-    client_id = AZCLI_ID
+    client_id = utils.AZCLI_ID
     username = t_info.username
     tenant_id = t_info.tenant_id
     return {
         "username": username,
         "environment": "login.microsoftonline.com",
         "client_id": client_id,
         "scope": scopes,
```

### Comparing `zer1t0_aze-0.0.8/aze/az_search_token_in_cache.py` & `zer1t0_aze-0.0.9/aze/az_search_token_in_cache.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_show_ad_role.py` & `zer1t0_aze-0.0.9/aze/az_show_ad_role.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/az_show_administrative_unit.py` & `zer1t0_aze-0.0.9/aze/az_show_administrative_unit.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/graph_api.py` & `zer1t0_aze-0.0.9/aze/graph_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,17 +15,25 @@
 
 def list_applications(access_token):
     return request_az_api(
         "https://graph.microsoft.com/v1.0/applications",
         access_token,
     )["value"]
 
-def list_sp_app_role_asignments(access_token, sp_id):
+def list_sp_app_role_asignments(access_token, sp_id=None, app_id=None):
+    if sp_id:
+        url = "https://graph.microsoft.com/v1.0/servicePrincipals/{}/appRoleAssignments".format(sp_id)
+    elif app_id:
+        url = "https://graph.microsoft.com/v1.0/servicePrincipals(appId='{}')/appRoleAssignments".format(app_id)
+
+    else:
+        raise ValueError("Must provide sp_id or app_id")
+
     return request_az_api(
-        "https://graph.microsoft.com/v1.0/servicePrincipals/{}/appRoleAssignments".format(sp_id),
+        url,
         access_token,
     )["value"]
 
 def list_user_memberof(access_token, user):
     return request_az_api(
         "https://graph.microsoft.com/v1.0/users/{}/memberOf".format(user),
         access_token,
```

### Comparing `zer1t0_aze-0.0.8/aze/permutations.py` & `zer1t0_aze-0.0.9/aze/permutations.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/profile.py` & `zer1t0_aze-0.0.9/aze/profile.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/read_in.py` & `zer1t0_aze-0.0.9/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.8/aze/request_az.py` & `zer1t0_aze-0.0.9/aze/request_az.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,28 +7,29 @@
     while next_link:
         resp = request_az_api(next_link, access_token)
         values.extend(resp["value"])
         next_link = resp.get("@odata.nextLink", "")
 
     return values
 
-def request_az_api(url, access_token, method="GET", json=None):
+def request_az_api(url, access_token, method="GET", json=None, params=None):
     headers = {
         "Authorization": "Bearer {}".format(access_token)
     }
 
     if method.upper() == "POST":
         req = requests.post
     else:
         req = requests.get
 
     resp = req(
         url,
         headers=headers,
         json=json,
+        params=params,
         # verify=False,
     )
 
     if resp.status_code != 200:
         raise AzeRequestError(
             "Error {} in response: {} ({})".format(
                 resp.status_code,
```

### Comparing `zer1t0_aze-0.0.8/aze/utils.py` & `zer1t0_aze-0.0.9/aze/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import sys
 from uuid import UUID
 
+AZCLI_ID = "04b07795-8ddb-461a-bbee-02f9e1bf7b46"
+
 def add_b64_padding(data):
     padding_len = (4 - (len(data) % 4)) % 4
     return data + "=" * padding_len
 
 def eprint(*args, **kwargs):
     print(*args, file=sys.stderr, **kwargs)
```

### Comparing `zer1t0_aze-0.0.8/setup.py` & `zer1t0_aze-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,25 +17,29 @@
 
 scripts = [
     "az-brute-add-app-secret",
     "az-brute-passwords",
     "az-brute-usernames",
     "az-brute-service-subdomains",
     "az-brute-blob-containers",
+    "az-download-blob",
+    "az-download-deployment-template",
     "az-get-login-info",
     "az-get-tenant-domains",
     "az-get-tenant-id",
     "az-inspect-token",
     "az-list-administrative-unit-members",
     "az-list-administrative-unit-role-members",
     "az-list-blobs",
     "az-list-subscriptions",
     "az-list-role-assignment",
     "az-list-sp-app-role-assignment",
     "az-list-user-memberof",
+    "az-list-vm-extensions",
+    "az-list-vm-permissions",
     "az-login-with-token",
     "az-search-token-in-cache",
     "az-show-ad-role",
     "az-show-administrative-unit",
     "az-whoami",
 ]
```

### Comparing `zer1t0_aze-0.0.8/zer1t0_aze.egg-info/PKG-INFO` & `zer1t0_aze-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: zer1t0-aze
-Version: 0.0.8
-Summary: Enhance azure cli
-Home-page: https://gitlab.com/Zer1t0/aze
-Author: Eloy Pérez González
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: msal_extensions
-Requires-Dist: dnspython
-
 # AZE (Azure Cli Enhacement)
 
 Extended utilities for azure management.
 
 A python package intended to be used along with Azure Cli to expand its
 capabilities, even if many commands are completely independent from Azure Cli.
 
@@ -25,26 +11,30 @@
 AZE includes the following commands, many of them require to be
 authenticated (marked with Auth) in Azure:
 
 - **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
-  subdomains (No auth).
-- **az-brute-blob-containers**: Discover public containers in Azure blobs (No auth).
+  subdomains. (No auth)
+- **az-brute-blob-containers**: Discover public containers in Azure blobs. (No auth)
+- **az-download-blob**: Download blob from URL. (Auth with -a parameter)
+- **az-download-deployment-template**: Download a deployment template. (Auth)
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
-- **az-list-blobs**: List blobs of container from URL (No auth).
+- **az-list-blobs**: List blobs or containers from URL. (Auth with -a parameter)
 - **az-list-administrative-unit-members**: List Administrative Unit members (Auth).
 - **az-list-administrative-unit-role-members**: List Administrative Unit scoped role members (Auth).
 - **az-list-role-assignment**: List roles without requiring a graph access token. (Auth)
 - **az-list-sp-app-role-assignment**: List App roles for a service principal. (Auth)
 - **az-list-user-memberof**: List membership of user, both groups and administrative units. (Auth)
+- **az-list-vm-extensions**: List virtual machine extensions. (Auth)
+- **az-list-vm-permissions**: List virtual machine permissions. (Auth)
 - **az-login-with-token**: Injects tokens directly into Azure Cli token cache.
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-show-ad-role**: Show Entra ID role. (Auth)
 - **az-show-administrative-unit**: Show Administrative Unit. (Auth)
 - **az-whoami**: Shorcut for "az ad signed-in-user show". (Auth)
 
 ## Installation
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zer1t0_aze-0.0.8/zer1t0_aze.egg-info/SOURCES.txt` & `zer1t0_aze-0.0.9/zer1t0_aze.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,35 +6,40 @@
 aze/__init__.py
 aze/arm_api.py
 aze/az_brute_add_app_secret.py
 aze/az_brute_blob_containers.py
 aze/az_brute_passwords.py
 aze/az_brute_service_subdomains.py
 aze/az_brute_usernames.py
+aze/az_download_blob.py
+aze/az_download_deployment_template.py
 aze/az_get_login_info.py
 aze/az_get_tenant_domains.py
 aze/az_get_tenant_id.py
 aze/az_inspect_token.py
 aze/az_list_administrative_unit_members.py
 aze/az_list_administrative_unit_role_members.py
 aze/az_list_blobs.py
 aze/az_list_role_assignment.py
 aze/az_list_sp_app_role_assignment.py
 aze/az_list_user_memberof.py
+aze/az_list_vm_extensions.py
+aze/az_list_vm_permissions.py
 aze/az_login_with_token.py
 aze/az_search_token_in_cache.py
 aze/az_show_ad_role.py
 aze/az_show_administrative_unit.py
 aze/az_whoami.py
 aze/error.py
 aze/graph_api.py
 aze/permutations.py
 aze/profile.py
 aze/read_in.py
 aze/request_az.py
+aze/storage_api.py
 aze/tenant.py
 aze/tokens.py
 aze/utils.py
 aze/version.py
 zer1t0_aze.egg-info/PKG-INFO
 zer1t0_aze.egg-info/SOURCES.txt
 zer1t0_aze.egg-info/dependency_links.txt
```

### Comparing `zer1t0_aze-0.0.8/zer1t0_aze.egg-info/entry_points.txt` & `zer1t0_aze-0.0.9/zer1t0_aze.egg-info/entry_points.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [console_scripts]
 az-brute-add-app-secret = aze.az_brute_add_app_secret:main
 az-brute-blob-containers = aze.az_brute_blob_containers:main
 az-brute-passwords = aze.az_brute_passwords:main
 az-brute-service-subdomains = aze.az_brute_service_subdomains:main
 az-brute-usernames = aze.az_brute_usernames:main
+az-download-blob = aze.az_download_blob:main
+az-download-deployment-template = aze.az_download_deployment_template:main
 az-get-login-info = aze.az_get_login_info:main
 az-get-tenant-domains = aze.az_get_tenant_domains:main
 az-get-tenant-id = aze.az_get_tenant_id:main
 az-inspect-token = aze.az_inspect_token:main
 az-list-administrative-unit-members = aze.az_list_administrative_unit_members:main
 az-list-administrative-unit-role-members = aze.az_list_administrative_unit_role_members:main
 az-list-blobs = aze.az_list_blobs:main
 az-list-role-assignment = aze.az_list_role_assignment:main
 az-list-sp-app-role-assignment = aze.az_list_sp_app_role_assignment:main
 az-list-subscriptions = aze.az_list_subscriptions:main
 az-list-user-memberof = aze.az_list_user_memberof:main
+az-list-vm-extensions = aze.az_list_vm_extensions:main
+az-list-vm-permissions = aze.az_list_vm_permissions:main
 az-login-with-token = aze.az_login_with_token:main
 az-search-token-in-cache = aze.az_search_token_in_cache:main
 az-show-ad-role = aze.az_show_ad_role:main
 az-show-administrative-unit = aze.az_show_administrative_unit:main
 az-whoami = aze.az_whoami:main
```

