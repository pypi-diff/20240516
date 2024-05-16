# Comparing `tmp/atils-1.2.0.tar.gz` & `tmp/atils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atils-1.2.0.tar", max compression
+gzip compressed data, was "atils-1.4.1.tar", max compression
```

## Comparing `atils-1.2.0.tar` & `atils-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1656 2024-03-30 01:10:16.829685 atils-1.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-30 01:10:16.829685 atils-1.2.0/atils/__init__.py
--rw-r--r--   0        0        0    25458 2024-03-30 01:10:16.829685 atils-1.2.0/atils/argocd.py
--rw-r--r--   0        0        0    11679 2024-03-30 01:10:16.829685 atils-1.2.0/atils/atils_kubernetes.py
--rw-r--r--   0        0        0    12819 2024-03-30 01:10:16.829685 atils-1.2.0/atils/build.py
--rw-r--r--   0        0        0        7 2024-03-30 01:10:16.829685 atils-1.2.0/atils/common/.secrets.yaml
--rw-r--r--   0        0        0        0 2024-03-30 01:10:16.829685 atils-1.2.0/atils/common/__init__.py
--rw-r--r--   0        0        0      166 2024-03-30 01:10:33.189541 atils-1.2.0/atils/common/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     7770 2024-03-30 01:10:33.189541 atils-1.2.0/atils/common/__pycache__/yaml_utils.cpython-312.pyc
--rw-r--r--   0        0        0     1139 2024-03-30 01:10:16.829685 atils-1.2.0/atils/common/config.py
--rw-r--r--   0        0        0      237 2024-03-30 01:10:16.829685 atils-1.2.0/atils/common/settings.py
--rw-r--r--   0        0        0      395 2024-03-30 01:10:16.829685 atils-1.2.0/atils/common/settings.yaml
--rw-r--r--   0        0        0     2464 2024-03-30 01:10:16.829685 atils-1.2.0/atils/common/template_utils.py
--rw-r--r--   0        0        0     7225 2024-03-30 01:10:16.829685 atils-1.2.0/atils/common/yaml_utils.py
--rw-r--r--   0        0        0     5014 2024-03-30 01:10:16.829685 atils-1.2.0/atils/helm.py
--rw-r--r--   0        0        0    18600 2024-03-30 01:10:16.829685 atils-1.2.0/atils/jobs.py
--rw-r--r--   0        0        0        0 2024-03-30 01:10:16.829685 atils-1.2.0/atils/templates/__init__.py
--rw-r--r--   0        0        0      704 2024-03-30 01:10:16.829685 atils-1.2.0/atils/templates/master-app.yaml
--rw-r--r--   0        0        0     1830 2024-03-30 01:10:16.829685 atils-1.2.0/atils/test.py
--rw-r--r--   0        0        0      819 2024-03-30 01:10:16.829685 atils-1.2.0/atils/vault.py
--rw-r--r--   0        0        0        0 2024-03-30 01:10:16.829685 atils-1.2.0/atils_bin/__init__.py
--rw-r--r--   0        0        0     1402 2024-03-30 01:10:16.829685 atils-1.2.0/atils_bin/atils.py
--rw-r--r--   0        0        0     1621 2024-03-30 01:10:16.829685 atils-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 atils-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1588 2024-05-16 02:55:32.674743 atils-1.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 02:55:32.674743 atils-1.4.1/atils/__init__.py
+-rw-r--r--   0        0        0    25458 2024-05-16 02:55:32.674743 atils-1.4.1/atils/argocd.py
+-rw-r--r--   0        0        0    15725 2024-05-16 02:55:32.674743 atils-1.4.1/atils/atils_kubernetes.py
+-rw-r--r--   0        0        0    12819 2024-05-16 02:55:32.674743 atils-1.4.1/atils/build.py
+-rw-r--r--   0        0        0        7 2024-05-16 02:55:32.674743 atils-1.4.1/atils/common/.secrets.yaml
+-rw-r--r--   0        0        0        0 2024-05-16 02:55:32.674743 atils-1.4.1/atils/common/__init__.py
+-rw-r--r--   0        0        0      166 2024-05-16 02:55:56.342793 atils-1.4.1/atils/common/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7770 2024-05-16 02:55:56.346793 atils-1.4.1/atils/common/__pycache__/yaml_utils.cpython-312.pyc
+-rw-r--r--   0        0        0     1139 2024-05-16 02:55:32.674743 atils-1.4.1/atils/common/config.py
+-rw-r--r--   0        0        0     1851 2024-05-16 02:55:32.674743 atils-1.4.1/atils/common/console_utils.py
+-rw-r--r--   0        0        0      237 2024-05-16 02:55:32.674743 atils-1.4.1/atils/common/settings.py
+-rw-r--r--   0        0        0      395 2024-05-16 02:55:32.674743 atils-1.4.1/atils/common/settings.yaml
+-rw-r--r--   0        0        0     2464 2024-05-16 02:55:32.674743 atils-1.4.1/atils/common/template_utils.py
+-rw-r--r--   0        0        0     7225 2024-05-16 02:55:32.674743 atils-1.4.1/atils/common/yaml_utils.py
+-rw-r--r--   0        0        0     5014 2024-05-16 02:55:32.674743 atils-1.4.1/atils/helm.py
+-rw-r--r--   0        0        0    25947 2024-05-16 02:55:32.674743 atils-1.4.1/atils/jobs.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:55:32.674743 atils-1.4.1/atils/templates/__init__.py
+-rw-r--r--   0        0        0      704 2024-05-16 02:55:32.674743 atils-1.4.1/atils/templates/master-app.yaml
+-rw-r--r--   0        0        0     1828 2024-05-16 02:55:32.674743 atils-1.4.1/atils/test.py
+-rw-r--r--   0        0        0      819 2024-05-16 02:55:32.674743 atils-1.4.1/atils/vault.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:55:32.674743 atils-1.4.1/atils_bin/__init__.py
+-rw-r--r--   0        0        0     1427 2024-05-16 02:55:32.674743 atils-1.4.1/atils_bin/atils.py
+-rw-r--r--   0        0        0     1638 2024-05-16 02:55:32.678743 atils-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2740 1970-01-01 00:00:00.000000 atils-1.4.1/PKG-INFO
```

### Comparing `atils-1.2.0/README.md` & `atils-1.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Atils
 Atils is a set of python scripts that make it easier to work with this monorepo. It's kind of a grab bag.
 
 ## Subcommands and What They Do
 `argocd`: Manages and installs argocd, using the master-stack application located in the templates folder
 `build`: A wrapper around whatever build tools are needed for a project. Configured using a special `.atils_buildconfig.json` file
 `helm`: Tools for managing helm, at this point just includes our auto-deploy script for development
-`jobs`: Tools for managingl, running, and templating Kubernetes jobs. That's also where we threw a special job for managing a PVC
-`vault`: In the future, will have tools for updating and placing secrets from a local directory into Hashi Vault. Or maybe we'll just use Terraform, that's probably easier
+`jobs`: Tools for managing, running, and templating Kubernetes jobs. Also includes commands for launching into debug containers
+`kubernetes`: Tools for performing operations on a kubernetes cluster that don't really fit anywhere else
 
 ## Configuration and Installation
 So... this isn't great right now. Atils relies on certain configurations, and it doesn't have a good way to set defaults right now. I've included an example for some basic default configs, but in the future we'll want to add some kind of install script or setup helper. This can go anywhere, I put it in my `.zshenv` so it applies on every login:
 
 ```
 export ATILS_INSTALL_DIR="@jinja {{env.HOME}}/PersonalMonorepo"
 export ATILS_KUBECONFIG_LOCATION="@jinja {{env.HOME}}/.kube/"
```

### Comparing `atils-1.2.0/atils/argocd.py` & `atils-1.4.1/atils/argocd.py`

 * *Files identical despite different names*

### Comparing `atils-1.2.0/atils/atils_kubernetes.py` & `atils-1.4.1/atils/atils_kubernetes.py`

 * *Files 22% similar despite different names*

```diff
@@ -53,47 +53,159 @@
     rke_parser.add_argument(
         "-f",
         "--force",
         help="force the recreation of a cluster, in cases where it's already running",
     )
     rke_parser.add_argument(
         "-rk",
-        "--replace-kubeconfig",
-        help="Copies a kubeconfig generated by rke to the system-wide kubeconfig",
+        "--replace-kubeconfig-only",
+        help="Only copy the kubeconfig, but do not create a new cluster",
         action="store_true",
         default=False,
     )
     rke_parser.add_argument(
         "cluster_name",
         help="the name of the cluster to set up. This should match an rke file",
     )
 
+    istio_parser = subparsers.add_parser(
+        "istio", help="Commands to manage or interact with istio"
+    )
+    istio_parser.add_argument(
+        "command",
+        choices=["label-namespaces"],
+        help="Which istio-related operator to perform",
+    )
+
     if len(args) == 0:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
     arguments: argparse.Namespace = parser.parse_args(args)
+    args_dict: dict[str, str] = vars(arguments)
 
     if arguments.subparser_name == "rke-setup":
         if vars(arguments).get("replace_kubeconfig"):
             merge_and_replace_kubeconfig(arguments.cluster_name)
         else:
             setup_rke_cluster(
                 arguments.cluster_name,
             )
+            merge_and_replace_kubeconfig(arguments.cluster_name)
 
     elif arguments.subparser_name == "secrets":
-        args_dict: dict[str, str] = vars(arguments)
         if args_dict["command"] == "decode":
             if args_dict["secret_name"] is None:
                 logging.error("Error: A secret name must be provided ")
                 sys.exit(1)
             else:
                 get_and_decode_secret(args_dict["secret_name"], args_dict["namespace"])
 
+    elif arguments.subparser_name == "istio":
+        if args_dict["command"] == "label-namespaces":
+            _label_namespaces_for_istio_injection(
+                [
+                    "ingress-nginx",
+                    "istio-system",
+                    "kube-public",
+                    "kube-system",
+                    "local-path-storage",
+                ]
+            )
+
+            _clear_pods_for_istio_injection(
+                [
+                    "ingress-nginx",
+                    "istio-system",
+                    "kube-public",
+                    "kube-system",
+                    "local-path-storage",
+                ]
+            )
+
+
+def check_namespace_exists(namespace_name: str) -> bool:
+    """
+    Check if a given kubernetes namespace exists
+    Args:
+        namespace_name (str): The name of the namespace to check
+    Returns:
+        bool: True if the namespace exists, False otherwise.
+    """
+    # Create Kubernetes API client
+    v1 = client.CoreV1Api()
+
+    # Use the API client to list all namespaces
+    namespace_list = v1.list_namespace().items
+
+    # Check if the namespace exists
+    if any(namespace.metadata.name == namespace_name for namespace in namespace_list):
+        return True
+    else:
+        return False
+
+
+def get_and_decode_secret(secret_name: str, secret_namespace: str) -> None:
+    """
+    Get a kubernetes secret, and then decode and pretty print it
+    Args:
+        secret_name (str): The name of the secret to decode and print
+        secret_namespace (str): The namespace the given secret is located in
+    """
+    try:
+        # Create a Kubernetes API client
+        api = client.CoreV1Api()
+
+        if secret_namespace is None:
+            current_context = k8s_config.list_kube_config_contexts()[1]
+            # Check if current_context["context"]["namespace"] is None
+            secret_namespace = current_context.get("context").get(
+                "namespace", "default"
+            )
+
+        # Get the Secret from the specified namespace
+        secret = api.read_namespaced_secret(
+            name=secret_name, namespace=secret_namespace
+        )
+
+        terminal_width = shutil.get_terminal_size().columns
+
+        print("=" * int(terminal_width / 2))
+        print(secret.metadata.name.center(int(terminal_width / 2)))
+        print("=" * int(terminal_width / 2))
+
+        # Decode and pretty print the data items
+        for key, value in secret.data.items():
+            decoded_value = base64.b64decode(value).decode("utf-8")
+            # If decoded_value is more than one line, print on a new line
+            if "\n" in decoded_value:
+                print(f"{key}:")
+                print(decoded_value)
+            else:
+                print(f"{key}: {decoded_value}")
+
+            print("=" * int(terminal_width / 2))
+
+    except Exception as e:
+        logging.error(f"An error occurred: {e}")
+
+
+def get_current_namespace() -> str:
+    """
+    Gets the current namespace set in the current context
+    Returns:
+        str: The current namespace set in the current context
+    """
+    contexts, active_context = k8s_config.list_kube_config_contexts()
+
+    if "namespace" in active_context["context"].keys():
+        return active_context["context"]["namespace"]
+    else:
+        return "default"
+
 
 def load_config() -> bool:
     """
     Loads some kind of kubernetes configuration, either in-cluster or in kubeconfig,
     and returns true if it is able to. If it cannot, it will return false, and the main
     function is in charge of failing if it needs to
 
@@ -186,95 +298,14 @@
         else:
             logging.error(
                 f"Could not find an rke file named {cluster_name}.yaml. Aborting"
             )
             exit(1)
 
 
-def check_namespace_exists(namespace_name: str) -> bool:
-    """
-    Check if a given kubernetes namespace exists
-    Args:
-        namespace_name (str): The name of the namespace to check
-    Returns:
-        bool: True if the namespace exists, False otherwise.
-    """
-    # Create Kubernetes API client
-    v1 = client.CoreV1Api()
-
-    # Use the API client to list all namespaces
-    namespace_list = v1.list_namespace().items
-
-    # Check if the namespace exists
-    if any(namespace.metadata.name == namespace_name for namespace in namespace_list):
-        return True
-    else:
-        return False
-
-
-def get_and_decode_secret(secret_name: str, secret_namespace: str) -> None:
-    """
-    Get a kubernetes secret, and then decode and pretty print it
-    Args:
-        secret_name (str): The name of the secret to decode and print
-        secret_namespace (str): The namespace the given secret is located in
-    """
-    try:
-        # Create a Kubernetes API client
-        api = client.CoreV1Api()
-
-        if secret_namespace is None:
-            current_context = k8s_config.list_kube_config_contexts()[1]
-            # Check if current_context["context"]["namespace"] is None
-            secret_namespace = current_context.get("context").get(
-                "namespace", "default"
-            )
-
-        # Get the Secret from the specified namespace
-        secret = api.read_namespaced_secret(
-            name=secret_name, namespace=secret_namespace
-        )
-
-        terminal_width = shutil.get_terminal_size().columns
-
-        print("=" * int(terminal_width / 2))
-        print(secret.metadata.name.center(int(terminal_width / 2)))
-        print("=" * int(terminal_width / 2))
-
-        # Decode and pretty print the data items
-        for key, value in secret.data.items():
-            decoded_value = base64.b64decode(value).decode("utf-8")
-            # If decoded_value is more than one line, print on a new line
-            if "\n" in decoded_value:
-                print(f"{key}:")
-                print(decoded_value)
-            else:
-                print(f"{key}: {decoded_value}")
-
-            print("=" * int(terminal_width / 2))
-
-    except Exception as e:
-        logging.error(f"An error occurred: {e}")
-
-
-def get_current_namespace() -> str:
-    """
-    Gets the current namespace set in the current context
-    Returns:
-        str: The current namespace set in the current context
-    """
-    contexts, active_context = k8s_config.list_kube_config_contexts()
-
-    if "namespace" in active_context["context"].keys():
-        return active_context["context"]["namespace"]
-    else:
-        return "default"
-
-
-# TODO after we've standardized the names for our cluster, we should make this
 def _check_cluster_availability() -> bool:
     """
     Checks if the cluster in the active context is available, by attempting to list nodes on a five second timeout
     Returns:
         true if the operation to list nodes succeeds, and false otherwise
     """
     try:
@@ -308,7 +339,87 @@
             )
             return False
 
         else:
             logging.error("We found a new kind of issue! This is a bug.")
             logging.error(e)
             return False
+
+
+def _clear_pods_for_istio_injection(excluded_namespaces: list[str]) -> None:
+    try:
+        # Create a Kubernetes API client
+        api = client.CoreV1Api()
+
+        # List all namespaces
+        namespaces = api.list_namespace().items
+
+        # Iterate over each namespace
+        for namespace in namespaces:
+            namespace_name = namespace.metadata.name
+
+            # Check if the namespace is in the excluded list
+            if namespace_name not in excluded_namespaces:
+                # List all pods in the namespace
+                pods = api.list_namespaced_pod(namespace_name).items
+
+                # Iterate over each pod
+                for pod in pods:
+                    # Check if the pod already has an Istio sidecar injected
+                    if "istio-proxy" in [
+                        container.name for container in pod.spec.containers
+                    ]:
+                        print(
+                            f"Skipping pod '{pod.metadata.name}' in namespace '{namespace_name}' (Istio sidecar already"
+                            + " injected)."
+                        )
+                        continue
+
+                    # Check if the pod has the annotation sidecar.istio.io/inject: "false"
+                    if (
+                        pod.metadata.annotations
+                        and pod.metadata.annotations.get("sidecar.istio.io/inject")
+                        == "false"
+                    ):
+                        print(
+                            f"Skipping pod '{pod.metadata.name}' in namespace '{namespace_name}' (annotation"
+                            + ' sidecar.istio.io/inject: "false").'
+                        )
+                        continue
+
+                    # Delete the pod
+                    api.delete_namespaced_pod(pod.metadata.name, namespace_name)
+                    print(
+                        f"Deleted pod '{pod.metadata.name}' in namespace '{namespace_name}' for Istio injection."
+                    )
+
+    except Exception as e:
+        print(f"Error: {str(e)}")
+
+
+def _label_namespaces_for_istio_injection(excluded_namespaces: list[str]) -> None:
+    try:
+        # Create a Kubernetes API client
+        api = client.CoreV1Api()
+
+        # List all namespaces
+        namespaces = api.list_namespace().items
+
+        # Iterate over each namespace
+        for namespace in namespaces:
+            namespace_name = namespace.metadata.name
+
+            # Check if the namespace is in the excluded list
+            if namespace_name not in excluded_namespaces:
+                # Add or update the Istio injection label
+                labels = namespace.metadata.labels or {}
+                labels["istio-injection"] = "enabled"
+                namespace.metadata.labels = labels
+
+                # Update the namespace
+                api.patch_namespace(namespace_name, namespace)
+                print(f"Labeled namespace '{namespace_name}' for Istio injection.")
+            else:
+                print(f"Skipping namespace '{namespace_name}' (excluded).")
+
+    except Exception as e:
+        print(f"Error: {str(e)}")
```

### Comparing `atils-1.2.0/atils/build.py` & `atils-1.4.1/atils/build.py`

 * *Files identical despite different names*

### Comparing `atils-1.2.0/atils/common/__pycache__/yaml_utils.cpython-312.pyc` & `atils-1.4.1/atils/common/__pycache__/yaml_utils.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sat Mar 30 01:10:16 2024 UTC, .py size: 7225 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 7866 0766 391c 0000  ........xf.f9...
+00000000: cb0d 0d0a 0000 0000 a475 4566 391c 0000  .........uEf9...
 00000010: e300 0000 0000 0000 0000 0000 0012 0000  ................
 00000020: 0000 0000 00f3 fa00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6402  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 0200 6500 6a08 0000  l.m.Z.....e.j...
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 6500 6a0a 0000 0000 0000 0000 0000 0000  e.j.............
 00000070: 0000 0000 0000 ac03 ab01 0000 0000 0000  ................
```

### Comparing `atils-1.2.0/atils/common/config.py` & `atils-1.4.1/atils/common/config.py`

 * *Files identical despite different names*

### Comparing `atils-1.2.0/atils/common/template_utils.py` & `atils-1.4.1/atils/common/template_utils.py`

 * *Files identical despite different names*

### Comparing `atils-1.2.0/atils/common/yaml_utils.py` & `atils-1.4.1/atils/common/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `atils-1.2.0/atils/helm.py` & `atils-1.4.1/atils/helm.py`

 * *Files identical despite different names*

### Comparing `atils-1.2.0/atils/jobs.py` & `atils-1.4.1/atils/jobs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import argparse
 import itertools
+import json
 import logging
 import os
 import sys
 import termios
 import time
 import tty
 from threading import Thread
 from typing import List
 
 import yaml
 from kubernetes.client.rest import ApiException
 from kubernetes.stream import stream
 
 from atils import atils_kubernetes
-from atils.common import config, template_utils
+from atils.common import config, console_utils, template_utils
 from kubernetes import client
 from kubernetes import config as k8s_config
 from kubernetes import utils
 
 client.rest.logger.setLevel(logging.ERROR)
 
 logging.basicConfig(level=config.get_logging_level())  # type: ignore
@@ -37,60 +38,123 @@
         help="Commands to manage kubernetes jobs", dest="subparser_name"
     )
 
     run_parser = subparsers.add_parser("run")
     run_parser.add_argument("job_name", help="Name of the job to run")
     # TODO Add some values for jobs, if needed, so we can set them with this argument
     run_parser.add_argument(
-        "--set", help="Set values to fill in job template. WIP, not currently working"
+        "--set",
+        help="Set values to fill in job template. WIP, not currently working",
+        nargs=2,
+        action="append",
+        dest="values",
     )
-    run_parser.add_argument("--tag", help="Image tag to use for the job")
 
     pvc_parser = subparsers.add_parser("manage-pvc")
     pvc_parser.add_argument(
         "--pvc-name", "-pn", help="The name of the PVC to launch a management pod for"
     )
     pvc_parser.add_argument(
         "--namespace",
         "-n",
         help="The namespace the PVC is located in. Defaults to current namespace",
     )
 
+    postgres_parser = subparsers.add_parser("postgres-manager")
+
     list_parser = subparsers.add_parser("list")
 
+    describe_parser = subparsers.add_parser("describe")
+    describe_parser.add_argument("job_name", help="Then name of the job to describe")
+
     arguments: argparse.Namespace = parser.parse_args(args)
 
     if arguments.subparser_name == "run":
+        args_dict = vars(arguments)
         job_args = {}
 
-        args_dict = vars(args)
-        if "image" in args_dict and args_dict["tag"] is not None:
-            job_args["image_tag"] = args_dict["tag"]
+        if args_dict["values"] is not None:
+            for arg in args_dict["values"]:
+                job_args[arg[0]] = arg[1]
+
+        jobconfig_args = _get_arguments_from_jobconfig(args_dict["job_name"])
+
+        args_filled_from_command_lines = _fill_out_jobconfig_args_from_command_line(
+            jobconfig_args, job_args
+        )
+
+        if "" in args_filled_from_command_lines.values():
+            final_job_args = _get_missing_arguments_interactive(
+                args_filled_from_command_lines
+            )
         else:
-            job_args["image_tag"] = "latest"
+            final_job_args = args_filled_from_command_lines
 
-        run_job(arguments.job_name, job_args)
+        run_job(arguments.job_name, final_job_args)
     elif arguments.subparser_name == "manage-pvc":
         args_dict = vars(arguments)
         current_namespace = atils_kubernetes.get_current_namespace()
 
         if "namespace" in args_dict.keys():
             if args_dict.get("namespace") is not None:
                 launch_pvc_manager(args_dict["pvc_name"], args_dict["namespace"])
             else:
                 launch_pvc_manager(args_dict["pvc_name"], current_namespace)
         else:
             launch_pvc_manager(args_dict["pvc_name"], current_namespace)
+    elif arguments.subparser_name == "postgres-manager":
+        launch_postgres_manager()
     elif arguments.subparser_name == "list":
         list_available_jobs()
+    elif arguments.subparser_name == "describe":
+        args_dict = vars(arguments)
+        describe_job(args_dict["job_name"])
     else:
         logging.error(f"Unrecognized command {arguments.subparser_name}")
         exit(1)
 
 
+def describe_job(job_name: str) -> None:
+    """
+    Using the .atils_jobconfig.json file, describe a job's purpose, as well as any arguments it takes.
+
+    Args:
+        job_name (str): The name of the job to describe
+    """
+    jobs_dir = config.get_full_atils_dir("JOBS_DIR")
+    dir_for_job = os.path.join(jobs_dir, job_name)
+
+    if os.path.exists(dir_for_job):
+        jobconfig_path = os.path.join(dir_for_job, ".atils_jobconfig.json")
+
+        if os.path.exists(jobconfig_path):
+            with open(jobconfig_path) as file:
+                jobconfig_data = json.load(file)
+                console_utils.print_jobconfig(jobconfig_data)
+        else:
+            logging.error(
+                f"Job {job_name} does not have a jobconfig. It probably will not run successfully"
+            )
+            exit(1)
+    else:
+        logging.error(f"Job {job_name} does not exist")
+        exit(1)
+
+    return
+
+
+def launch_postgres_manager() -> None:
+    """
+    Launch a postgres client pod, connected to the master user
+    """
+    _create_postgres_manager_pod()
+    time.sleep(5)
+    _exec_shell_in_pod("postgres-manager", "postgres", "postgres-manager", ["psql"])
+
+
 def launch_pvc_manager(pvc_name: str, namespace: str) -> None:
     """
     Given the name of a PVC, and the namespace it lives in, launch some kind of container that mounts it
 
     Args:
         pvc_name (str): The name of the PVC to launch a management container for
         namespace (str): The namespace the PVC is located in
@@ -108,35 +172,34 @@
         _create_pvc_manager_pod(pvc_name, namespace)
 
         pod_name = "pvc-manager"
         volume_name = pvc_name
 
     time.sleep(5)
 
-    _exec_shell_in_pod(pod_name, "videos", "pvc-manager")
+    _exec_shell_in_pod(pod_name, namespace, "pvc-manager")
 
 
 def list_available_jobs() -> None:
     # TODO exclude the docs directory, include a list of valid arguments
     """
     Print all the jobs available to run in the jobs directory to the console
     """
     jobs_dir = config.get_full_atils_dir("JOBS_DIR")
 
     root, dirs, files = next(os.walk(jobs_dir))
     for job in dirs:
-        description = "No description provided"
-        description_location = os.path.join(jobs_dir, job, "description.txt")
-        if os.path.exists(description_location):
-            with open(description_location) as file:
-                description = file.read()
-                if len(description) > 250:
-                    description = description[0:251] + "..."
+        if job != "docs":
+            jobconfig_path = os.path.join(jobs_dir, job, ".atils_jobconfig.json")
+            if os.path.exists(jobconfig_path):
+                with open(jobconfig_path) as file:
+                    jobconfig_data = json.load(file)
+                    description = jobconfig_data["short_description"]
 
-        print(f"{job}:      {description}")
+                print(f"{job}:      {description}")
 
 
 def run_job(job_name: str, args=None) -> None:
     """
     Given a job name and list of args, render the job template, then run the job
     Args:
         job_name (str): The name of the job to run. Must be a directory in the JOBS_DIR directory
@@ -183,14 +246,85 @@
                         raise e
             print("\n")
             logging.info(f"Job {job_name} deleted")
             return
     logging.info(f"No job named {job_name} found in namespace {namespace}")
 
 
+def _create_postgres_manager_pod() -> None:
+    # TODO we can make this generic with a ton of arguments
+    """
+    Create a postgres client pod, connected to the master user
+    """
+    try:
+        api_instance = client.CoreV1Api()
+
+        try:
+            existing_pod = api_instance.read_namespaced_pod(
+                name="postgres-manager", namespace="postgres"
+            )
+
+            # TODO right now, we might get kicked out of our pod if it's close to expiring. That's probably
+            # not a big deal, but if so, fix it here
+            if existing_pod:
+                logging.info(
+                    "There's already a postgres-manager pod! We're just gonna leave it"
+                )
+                return
+        except ApiException as e:
+            if e.status != 404:
+                logging.error(
+                    f"Error checking for existing pod 'postgres-manager': {str(e)}"
+                )
+                exit(1)
+
+        pod_manifest = {
+            "apiVersion": "v1",
+            "kind": "Pod",
+            "metadata": {"name": "postgres-manager"},
+            "spec": {
+                "containers": [
+                    {
+                        "name": "postgres-manager",
+                        "image": "aidanhilt/atils-postgres-client",
+                        "command": ["sh", "-c", "sleep 1800"],
+                        "env": [
+                            {
+                                "name": "PGHOST",
+                                "value": "postgres-postgresql.postgres.svc.cluster.local",
+                            },
+                            {"name": "PGUSER", "value": "postgres"},
+                            {
+                                "name": "PGPASSWORD",
+                                "valueFrom": {
+                                    "secretKeyRef": {
+                                        "name": "postgres-config",
+                                        "key": "postgres-password",
+                                    }
+                                },
+                            },
+                            {"name": "PGDATABASE", "value": "postgres"},
+                        ],
+                    }
+                ],
+                "restartPolicy": "Never",
+            },
+        }
+
+        try:
+            # Create the pod
+            api_instance.create_namespaced_pod(namespace="postgres", body=pod_manifest)
+            logging.info("Created pod 'postgres-manager' in postgres namespace")
+        except client.rest.ApiException as e:
+            logging.error(f"Error creating pod 'postgres-manager': {str(e)}")
+
+    except Exception as e:
+        logging.error(f"Error occurred while creating pod 'postgres-manager': {str(e)}")
+
+
 def _create_pvc_manager_pod(pvc_name: str, namespace: str) -> None:
     try:
         api_instance = client.CoreV1Api()
 
         # Check if a pod named "pvc-manager" already exists in the namespace
         try:
             existing_pod = api_instance.read_namespaced_pod(
@@ -300,29 +434,32 @@
                     f"Error deleting ephemeral container from pod '{pod_name}': {str(e)}"
                 )
 
     except Exception as e:
         logging.error(f"Error occurred while deleting ephemeral container: {str(e)}")
 
 
-def _exec_shell_in_pod(pod_name: str, namespace: str, container_name: str) -> None:
+def _exec_shell_in_pod(
+    pod_name: str,
+    namespace: str,
+    container_name: str,
+    exec_command: list[str] = ["/bin/zsh"],
+) -> None:
     """
     Exec into a given container in a given pod, in a given namespace. This will assume
     that the container has zsh installed
 
     Args:
         pod_name (str): The name of the pod to exec into
         namespace (str): The namespace the pod is located in
         container_name (str): The name of the container to exec into
     """
     api_client = client.ApiClient()
     api_instance = client.CoreV1Api(api_client)
 
-    exec_command = ["/bin/zsh"]
-
     resp = stream(
         api_instance.connect_get_namespaced_pod_exec,
         pod_name,
         namespace,
         command=exec_command,
         container=container_name,
         stderr=True,
@@ -349,14 +486,32 @@
     finally:
         # reset tty
         print("\033c")
         termios.tcsetattr(stdin_fd, termios.TCSADRAIN, old_settings)
         print("press enter")
 
 
+def _fill_out_jobconfig_args_from_command_line(
+    jobconfig_args: dict, command_line_args: dict
+) -> dict[str, str]:
+    """
+    Fill out the jobconfig_args dictionary with the c.
+
+    Args:
+        jobconfig_args (dict): The dictionary to fill out
+        command_line_args (dict): The dictionary containing the command line arguments
+
+    Returns:
+        dict: The updated jobconfig_args dictionary
+    """
+    for key, value in command_line_args.items():
+        jobconfig_args[key] = value
+    return jobconfig_args
+
+
 def _find_pod_by_pvc(pvc_name: str) -> str:
     """
     Given the name of a PVC, find the name of a pod it is attached to. If no pod is attached, return an empty string
 
     Args:
         pvc_name (str): The name of the PVC to search for
 
@@ -416,14 +571,79 @@
         sys.exit(1)
 
     except Exception as e:
         logging.error(f"Error occurred while searching for volume: {str(e)}")
         sys.exit(1)
 
 
+def _get_arguments_from_jobconfig(job_name: str) -> dict[str, str]:
+    """
+    Get the arguments from the jobconfig file.
+
+    Args:
+        job_name (str): The name of the job to get the arguments for
+
+    Returns:
+        dict[str, str]: A dictionary containing the arguments
+    """
+    try:
+        jobs_dir = config.get_full_atils_dir("JOBS_DIR")
+        if os.path.exists(os.path.join(jobs_dir, job_name, ".atils_jobconfig.json")):
+            jobconfig_file = os.path.join(jobs_dir, job_name, ".atils_jobconfig.json")
+        else:
+            logging.error(f"No jobconfig found for job {job_name}, exiting")
+            sys.exit(1)
+
+        jobconfig_args = {}
+
+        # Read the jobconfig file
+        with open(jobconfig_file, "r") as file:
+            jobconfig = json.load(file)
+
+            if "args" in jobconfig.keys():
+                for arg in jobconfig["args"]:
+                    if "default" in arg.keys():
+                        jobconfig_args[arg["name"]] = arg["default"]
+                    else:
+                        jobconfig_args[arg["name"]] = ""
+
+        return jobconfig_args
+
+    except Exception as e:
+        logging.error(
+            f"Error occurred while getting arguments from jobconfig: {str(e)}"
+        )
+        sys.exit(1)
+
+
+def _get_missing_arguments_interactive(
+    missing_args_dict: dict[str, str]
+) -> dict[str, str]:
+    """
+    Get missing job arguments from the user.
+
+    Args:
+        missing_args_dict (dict[str, str]): A dictionary containing the missing arguments
+
+    Returns:
+        dict[str, str]: A dictionary containing the updated missing arguments
+    """
+    try:
+        for arg_name, arg_value in missing_args_dict.items():
+            if arg_value == "":
+                arg_value = input(f"Enter value for {arg_name}: ")
+                missing_args_dict[arg_name] = arg_value
+
+        return missing_args_dict
+
+    except Exception as e:
+        logging.error(f"Error occurred while getting missing arguments: {str(e)}")
+        sys.exit(1)
+
+
 def _launch_job(job_dict):
     job_name = job_dict["metadata"]["name"]
 
     if "namespace" in job_dict["metadata"]:
         namespace = job_dict["metadata"]["namespace"]
     else:
         _, active_context = k8s_config.list_kube_config_contexts()
```

### Comparing `atils-1.2.0/atils/templates/master-app.yaml` & `atils-1.4.1/atils/templates/master-app.yaml`

 * *Files identical despite different names*

### Comparing `atils-1.2.0/atils/test.py` & `atils-1.4.1/atils/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Stuff for actually running test functions
 # ==========================================
 def main(args: str):
     parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
     parser.add_argument(
         "action",
-        help="Select which action to perform. Defaults to build",
+        help="Select which action to perform. Defaults to run",
         default="run",
         nargs="?",
     )
 
     parser.add_argument("--function-name", type=str)
 
     arguments: argparse.Namespace = parser.parse_args(args)
```

### Comparing `atils-1.2.0/atils/vault.py` & `atils-1.4.1/atils/vault.py`

 * *Files identical despite different names*

### Comparing `atils-1.2.0/atils_bin/atils.py` & `atils-1.4.1/atils_bin/atils.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     if script_name == "kubernetes":
         kubernetes.main(sys.argv[2:])
     elif script_name == "argocd":
         argocd.main(sys.argv[2:])
     elif script_name == "build":
         build.main(sys.argv[2:])
-    elif script_name == "job":
+    elif script_name == "job" or script_name == "jobs":
         jobs.main(sys.argv[2:])
     elif script_name == "helm":
         helm.main(sys.argv[2:])
     elif script_name == "test":
         test.main(sys.argv[2:])
     elif script_name == "help" or script_name == "--help":
         print(
```

### Comparing `atils-1.2.0/pyproject.toml` & `atils-1.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atils"
-version = "1.2.0"
+version = "1.4.1"
 description = "A series of scripts used to interact and work with this repository."
 authors = ["Aidan Hilt <aidanhilt2@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "atils" },
     { include = "atils_bin" }
 ]
@@ -23,14 +23,15 @@
 dynaconf = "^3.1.12"
 jinja2 = "^3.1.2"
 termcolor = "^2.3.0"
 watchfiles = "^0.21.0"
 asyncio = "^3.4.3"
 setuptools = "^69.0.3"
 colored = "^2.2.4"
+rich = "^13.7.1"
 
 [tool.poetry.group.dev.dependencies]
 MonkeyType = "22.2.0"
 black = "22.12.0"
 pytest = "7.2.0"
 flake8 = "^7.0.0"
 check-jsonschema = "^0.28.0"
```

### Comparing `atils-1.2.0/PKG-INFO` & `atils-1.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atils
-Version: 1.2.0
+Version: 1.4.1
 Summary: A series of scripts used to interact and work with this repository.
 Author: Aidan Hilt
 Author-email: aidanhilt2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,30 +16,31 @@
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: hvac (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: kubernetes (>=28.1.0,<29.0.0)
 Requires-Dist: mypy (>=1.1.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Requires-Dist: shutils (>=0.1.0,<0.2.0)
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.9,<7.0.0.0)
 Requires-Dist: watchfiles (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Atils
 Atils is a set of python scripts that make it easier to work with this monorepo. It's kind of a grab bag.
 
 ## Subcommands and What They Do
 `argocd`: Manages and installs argocd, using the master-stack application located in the templates folder
 `build`: A wrapper around whatever build tools are needed for a project. Configured using a special `.atils_buildconfig.json` file
 `helm`: Tools for managing helm, at this point just includes our auto-deploy script for development
-`jobs`: Tools for managingl, running, and templating Kubernetes jobs. That's also where we threw a special job for managing a PVC
-`vault`: In the future, will have tools for updating and placing secrets from a local directory into Hashi Vault. Or maybe we'll just use Terraform, that's probably easier
+`jobs`: Tools for managing, running, and templating Kubernetes jobs. Also includes commands for launching into debug containers
+`kubernetes`: Tools for performing operations on a kubernetes cluster that don't really fit anywhere else
 
 ## Configuration and Installation
 So... this isn't great right now. Atils relies on certain configurations, and it doesn't have a good way to set defaults right now. I've included an example for some basic default configs, but in the future we'll want to add some kind of install script or setup helper. This can go anywhere, I put it in my `.zshenv` so it applies on every login:
 
 ```
 export ATILS_INSTALL_DIR="@jinja {{env.HOME}}/PersonalMonorepo"
 export ATILS_KUBECONFIG_LOCATION="@jinja {{env.HOME}}/.kube/"
```

