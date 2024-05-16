# Comparing `tmp/python3-cyberfusion-cluster-cli-1.9.7.tar.gz` & `tmp/python3-cyberfusion-cluster-cli-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-cyberfusion-cluster-cli-1.9.7.tar", last modified: Wed Oct 25 14:58:51 2023, max compression
+gzip compressed data, was "python3-cyberfusion-cluster-cli-1.9.8.tar", last modified: Mon Oct 30 11:59:06 2023, max compression
```

## Comparing `python3-cyberfusion-cluster-cli-1.9.7.tar` & `python3-cyberfusion-cluster-cli-1.9.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 14:58:51.124689 python3-cyberfusion-cluster-cli-1.9.7/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1485 2023-10-25 14:58:51.124689 python3-cyberfusion-cluster-cli-1.9.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-10-25 14:58:51.124689 python3-cyberfusion-cluster-cli-1.9.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-10-25 13:52:50.000000 python3-cyberfusion-cluster-cli-1.9.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 14:58:51.116689 python3-cyberfusion-cluster-cli-1.9.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 14:58:51.116689 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 14:58:51.124689 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17097 2023-10-24 08:29:32.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     6527 2023-10-25 13:51:42.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/api_users.py
--rw-rw-rw-   0 root         (0) root         (0)     3098 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/basic_authentication_realms.py
--rw-rw-rw-   0 root         (0) root         (0)    26429 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/borg.py
--rw-rw-rw-   0 root         (0) root         (0)     2961 2023-10-24 08:49:20.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/certificate_managers.py
--rw-rw-rw-   0 root         (0) root         (0)     3434 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/certificates.py
--rw-rw-rw-   0 root         (0) root         (0)    20660 2023-10-25 13:51:42.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/clusters.py
--rw-rw-rw-   0 root         (0) root         (0)     9156 2023-10-25 13:51:42.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/cmses.py
--rw-rw-rw-   0 root         (0) root         (0)     4481 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/crons.py
--rw-rw-rw-   0 root         (0) root         (0)     4492 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/custom_config_snippets.py
--rw-rw-rw-   0 root         (0) root         (0)    12684 2023-10-25 13:51:42.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/databases.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2023-10-25 13:51:42.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/domain_routers.py
--rw-rw-rw-   0 root         (0) root         (0)     2737 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/firewall_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     7519 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/fpm_pools.py
--rw-rw-rw-   0 root         (0) root         (0)     4298 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/ftp_users.py
--rw-rw-rw-   0 root         (0) root         (0)     3992 2023-10-24 08:29:32.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/haproxy_listens.py
--rw-rw-rw-   0 root         (0) root         (0)     4064 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/htpasswd.py
--rw-rw-rw-   0 root         (0) root         (0)     8489 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/logs.py
--rw-rw-rw-   0 root         (0) root         (0)    11270 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     7790 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/main.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/malwares.py
--rw-rw-rw-   0 root         (0) root         (0)     4259 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     7532 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/passenger_apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3796 2023-10-25 13:51:42.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/redis_instances.py
--rw-rw-rw-   0 root         (0) root         (0)    12448 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/security_txt_policies.py
--rw-rw-rw-   0 root         (0) root         (0)     5664 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/ssh_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     9756 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/unix_users.py
--rw-rw-rw-   0 root         (0) root         (0)     4979 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/url_redirects.py
--rw-rw-rw-   0 root         (0) root         (0)    14904 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/virtual_hosts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 14:58:51.124689 python3-cyberfusion-cluster-cli-1.9.7/src/python3_cyberfusion_cluster_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1485 2023-10-25 14:58:51.000000 python3-cyberfusion-cluster-cli-1.9.7/src/python3_cyberfusion_cluster_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1665 2023-10-25 14:58:51.000000 python3-cyberfusion-cluster-cli-1.9.7/src/python3_cyberfusion_cluster_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-25 14:58:51.000000 python3-cyberfusion-cluster-cli-1.9.7/src/python3_cyberfusion_cluster_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-10-25 14:58:51.000000 python3-cyberfusion-cluster-cli-1.9.7/src/python3_cyberfusion_cluster_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      211 2023-10-25 14:58:51.000000 python3-cyberfusion-cluster-cli-1.9.7/src/python3_cyberfusion_cluster_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-10-25 14:58:51.000000 python3-cyberfusion-cluster-cli-1.9.7/src/python3_cyberfusion_cluster_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 11:59:06.569172 python3-cyberfusion-cluster-cli-1.9.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-10-30 11:59:06.569172 python3-cyberfusion-cluster-cli-1.9.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-10-30 11:59:06.569172 python3-cyberfusion-cluster-cli-1.9.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-10-30 11:51:46.000000 python3-cyberfusion-cluster-cli-1.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 11:59:06.561172 python3-cyberfusion-cluster-cli-1.9.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 11:59:06.561172 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 11:59:06.569172 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17142 2023-10-30 11:27:25.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/_utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     6527 2023-10-30 11:27:25.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/api_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/basic_authentication_realms.py
+-rw-rw-rw-   0 root         (0) root         (0)    26429 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/borg.py
+-rw-rw-rw-   0 root         (0) root         (0)     3791 2023-10-30 11:27:25.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/certificate_managers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/certificates.py
+-rw-rw-rw-   0 root         (0) root         (0)    20660 2023-10-30 11:27:25.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/clusters.py
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2023-10-30 11:27:25.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/cmses.py
+-rw-rw-rw-   0 root         (0) root         (0)     4481 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/crons.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/custom_config_snippets.py
+-rw-rw-rw-   0 root         (0) root         (0)    12684 2023-10-30 11:27:25.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/databases.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2023-10-30 11:27:25.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/domain_routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2737 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/firewall_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     7519 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/fpm_pools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4298 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/ftp_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     4037 2023-10-30 11:27:25.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/haproxy_listens.py
+-rw-rw-rw-   0 root         (0) root         (0)     4064 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/htpasswd.py
+-rw-rw-rw-   0 root         (0) root         (0)     8489 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/logs.py
+-rw-rw-rw-   0 root         (0) root         (0)    11270 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     7790 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/malwares.py
+-rw-rw-rw-   0 root         (0) root         (0)     4401 2023-10-30 11:57:49.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     7532 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/passenger_apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3796 2023-10-30 11:27:25.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/redis_instances.py
+-rw-rw-rw-   0 root         (0) root         (0)    12448 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/security_txt_policies.py
+-rw-rw-rw-   0 root         (0) root         (0)     5664 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/ssh_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)     9756 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/unix_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     4979 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/url_redirects.py
+-rw-rw-rw-   0 root         (0) root         (0)    14904 2023-10-24 08:20:50.000000 python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/virtual_hosts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 11:59:06.569172 python3-cyberfusion-cluster-cli-1.9.8/src/python3_cyberfusion_cluster_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-10-30 11:59:06.000000 python3-cyberfusion-cluster-cli-1.9.8/src/python3_cyberfusion_cluster_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-10-30 11:59:06.000000 python3-cyberfusion-cluster-cli-1.9.8/src/python3_cyberfusion_cluster_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-30 11:59:06.000000 python3-cyberfusion-cluster-cli-1.9.8/src/python3_cyberfusion_cluster_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-10-30 11:59:06.000000 python3-cyberfusion-cluster-cli-1.9.8/src/python3_cyberfusion_cluster_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2023-10-30 11:59:06.000000 python3-cyberfusion-cluster-cli-1.9.8/src/python3_cyberfusion_cluster_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-10-30 11:59:06.000000 python3-cyberfusion-cluster-cli-1.9.8/src/python3_cyberfusion_cluster_cli.egg-info/top_level.txt
```

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/LICENSE` & `python3-cyberfusion-cluster-cli-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/PKG-INFO` & `python3-cyberfusion-cluster-cli-1.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-cyberfusion-cluster-cli
-Version: 1.9.7
+Version: 1.9.8
 Summary: CLI for Cluster API.
 Home-page: https://vcs.cyberfusion.nl/core/python3-cyberfusion-cluster-cli
 Author: William Edwards
 Author-email: wedwards@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,cluster,cli
 Platform: linux
```

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/README.md` & `python3-cyberfusion-cluster-cli-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/setup.py` & `python3-cyberfusion-cluster-cli-1.9.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="python3-cyberfusion-cluster-cli",
-    version="1.9.7",
+    version="1.9.8",
     description="CLI for Cluster API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.9",
     author="William Edwards",
     author_email="wedwards@cyberfusion.nl",
     url="https://vcs.cyberfusion.nl/core/python3-cyberfusion-cluster-cli",
```

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/_utilities.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,18 +287,20 @@
 
 
 def get_haproxy_listen_to_node_by_multiple(
     haproxy_listen_name: str,
     node_hostname: str,
 ) -> HAProxyListenToNode:
     """Get HAProxy listen to node by HAProxy listen name and node hostname."""
+    node = get_object(get_support().nodes, hostname=node_hostname)
     haproxy_listen = get_object(
-        get_support().haproxy_listens, name=haproxy_listen_name
+        get_support().haproxy_listens,
+        name=haproxy_listen_name,
+        cluster_id=node.cluster.id,
     )
-    node = get_object(get_support().nodes, hostname=node_hostname)
 
     return get_object(
         get_support().haproxy_listens_to_nodes,
         haproxy_listen_id=haproxy_listen.id,
         node_id=node.id,
     )
```

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/api_users.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/api_users.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/basic_authentication_realms.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/basic_authentication_realms.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/borg.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/borg.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/certificates.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/certificates.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/clusters.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/clusters.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/cmses.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/cmses.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/crons.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/crons.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/custom_config_snippets.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/custom_config_snippets.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/databases.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/databases.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/domain_routers.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/domain_routers.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/firewall_groups.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/firewall_groups.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/fpm_pools.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/fpm_pools.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/ftp_users.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/ftp_users.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/haproxy_listens.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/haproxy_listens.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,18 +127,20 @@
 def create_node(
     haproxy_listen_name: str,
     node_hostname: str,
 ) -> None:
     """Create HAProxy listen to node."""
     haproxy_listen_to_node = HAProxyListenToNode(get_support())
 
+    node = get_object(get_support().nodes, hostname=node_hostname)
     haproxy_listen = get_object(
-        get_support().haproxy_listens, name=haproxy_listen_name
+        get_support().haproxy_listens,
+        name=haproxy_listen_name,
+        cluster_id=node.cluster.id,
     )
-    node = get_object(get_support().nodes, hostname=node_hostname)
 
     haproxy_listen_to_node.create(
         haproxy_listen_id=haproxy_listen.id, node_id=node.id
     )
 
 
 @app.command()
```

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/htpasswd.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/htpasswd.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/logs.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/logs.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/mail.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/mail.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/main.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/main.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/malwares.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/malwares.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/nodes.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     DETAILED_MESSAGE,
     EMTPY_TO_CLEAR_MESSAGE,
     catch_api_exception,
     console,
     delete_api_object,
     get_object,
     get_support,
+    wait_for_task,
 )
 from cyberfusion.ClusterSupport.nodes import Node, NodeGroup
 
 app = typer.Typer()
 
 
 @app.command("list")
@@ -45,14 +46,15 @@
     )
 
 
 @app.command()
 @catch_api_exception
 def create(
     cluster_name: str,
+    product: str,
     groups: List[NodeGroup] = typer.Option(..., "--group", show_default=False),
     comment: Optional[str] = typer.Option(default=None),
 ) -> None:
     """Create node."""
     node = Node(get_support())
 
     cluster = get_object(get_support().clusters, name=cluster_name)
@@ -65,22 +67,25 @@
                 cluster_id=cluster.id, groups=group
             )
 
             groups_properties[group] = {"is_master": len(existing_nodes) == 0}
         else:
             groups_properties[group] = None
 
-    node.create(
+    task_collection = node.create(
         groups=groups,
         comment=comment,
         load_balancer_health_checks_groups_pairs={},
         groups_properties=groups_properties,
         cluster_id=cluster.id,
+        product=product,
     )
 
+    wait_for_task(task_collection_uuid=task_collection.uuid)
+
 
 @app.command()
 @catch_api_exception
 def add_groups(hostname: str, groups: List[NodeGroup]) -> None:
     """Add groups."""
     node = get_object(get_support().nodes, hostname=hostname)
```

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/passenger_apps.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/passenger_apps.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/redis_instances.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/redis_instances.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/security_txt_policies.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/security_txt_policies.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/ssh_keys.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/unix_users.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/unix_users.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/url_redirects.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/url_redirects.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/cyberfusion/ClusterCli/virtual_hosts.py` & `python3-cyberfusion-cluster-cli-1.9.8/src/cyberfusion/ClusterCli/virtual_hosts.py`

 * *Files identical despite different names*

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/python3_cyberfusion_cluster_cli.egg-info/PKG-INFO` & `python3-cyberfusion-cluster-cli-1.9.8/src/python3_cyberfusion_cluster_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-cyberfusion-cluster-cli
-Version: 1.9.7
+Version: 1.9.8
 Summary: CLI for Cluster API.
 Home-page: https://vcs.cyberfusion.nl/core/python3-cyberfusion-cluster-cli
 Author: William Edwards
 Author-email: wedwards@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,cluster,cli
 Platform: linux
```

### Comparing `python3-cyberfusion-cluster-cli-1.9.7/src/python3_cyberfusion_cluster_cli.egg-info/SOURCES.txt` & `python3-cyberfusion-cluster-cli-1.9.8/src/python3_cyberfusion_cluster_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

