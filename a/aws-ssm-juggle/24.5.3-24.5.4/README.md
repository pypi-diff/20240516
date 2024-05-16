# Comparing `tmp/aws_ssm_juggle-24.5.3.tar.gz` & `tmp/aws_ssm_juggle-24.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ssm_juggle-24.5.3.tar", max compression
+gzip compressed data, was "aws_ssm_juggle-24.5.4.tar", max compression
```

## Comparing `aws_ssm_juggle-24.5.3.tar` & `aws_ssm_juggle-24.5.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-05-06 19:39:07.643146 aws_ssm_juggle-24.5.3/LICENSE
--rw-r--r--   0        0        0     2003 2024-05-06 19:39:07.643146 aws_ssm_juggle-24.5.3/README.md
--rw-r--r--   0        0        0     2301 2024-05-06 19:39:07.643146 aws_ssm_juggle-24.5.3/aws_ssm_juggle/__init__.py
--rw-r--r--   0        0        0     7349 2024-05-06 19:39:07.644146 aws_ssm_juggle-24.5.3/aws_ssm_juggle/ec2.py
--rw-r--r--   0        0        0    10748 2024-05-06 19:39:07.644146 aws_ssm_juggle-24.5.3/aws_ssm_juggle/ecs.py
--rw-r--r--   0        0        0      744 2024-05-06 19:39:07.644146 aws_ssm_juggle-24.5.3/pyproject.toml
--rw-r--r--   0        0        0     3150 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-05 06:37:08.152499 aws_ssm_juggle-24.5.4/LICENSE
+-rw-r--r--   0        0        0     2003 2024-05-05 06:37:08.152499 aws_ssm_juggle-24.5.4/README.md
+-rw-r--r--   0        0        0     2301 2024-05-05 06:37:08.152499 aws_ssm_juggle-24.5.4/aws_ssm_juggle/__init__.py
+-rw-r--r--   0        0        0     7447 2024-05-16 08:43:34.394674 aws_ssm_juggle-24.5.4/aws_ssm_juggle/ec2.py
+-rw-r--r--   0        0        0    11082 2024-05-16 08:44:13.277873 aws_ssm_juggle-24.5.4/aws_ssm_juggle/ecs.py
+-rw-r--r--   0        0        0      744 2024-05-16 08:44:20.581098 aws_ssm_juggle-24.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3150 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.4/PKG-INFO
```

### Comparing `aws_ssm_juggle-24.5.3/LICENSE` & `aws_ssm_juggle-24.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.5.3/README.md` & `aws_ssm_juggle-24.5.4/README.md`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.5.3/aws_ssm_juggle/__init__.py` & `aws_ssm_juggle-24.5.4/aws_ssm_juggle/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.5.3/aws_ssm_juggle/ec2.py` & `aws_ssm_juggle-24.5.4/aws_ssm_juggle/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,20 +183,15 @@
     filters = [
         {
             "Name": "instance-state-name",
             "Values": ["running"],
         },
     ]
     if instance_name:
-        filters.append(
-            {
-                "Name": "tag:Name",
-                "Values": [f"*{instance_name}*"]
-            }
-        )
+        filters.append({"Name": "tag:Name", "Values": [f"*{instance_name}*"]})
     reservations = ec2_paginator(
         boto3_session=boto3_session,
         paginator="describe_instances",
         leaf="Reservations",
         Filters=filters,
     )
     instances = []
@@ -225,27 +220,31 @@
     ssh_args, remote_port, local_port = None, None, None
     if "ssh_args" in arguments:
         ssh_args = arguments.ssh_args
     if "remote_port" in arguments:
         remote_port = arguments.remote_port
     if "local_port" in arguments:
         local_port = arguments.local_port
-    while not instance_id:
-        instance_id, _ = get_instance_id(
+    try:
+        while not instance_id:
+            instance_id, _ = get_instance_id(
+                boto3_session=boto3_session,
+                instance_id=instance_id,
+                instance_name=instance_name,
+            )
+            instance_id = instance_id.split(" - ")[0]
+        ec2_session = EC2Session(
             boto3_session=boto3_session,
             instance_id=instance_id,
-            instance_name=instance_name,
+            local_port=local_port,
+            remote_port=remote_port,
+            ssh_args=ssh_args,
         )
-        instance_id = instance_id.split(" - ")[0]
-    ec2_session = EC2Session(
-        boto3_session=boto3_session,
-        instance_id=instance_id,
-        local_port=local_port,
-        remote_port=remote_port,
-        ssh_args=ssh_args,
-    )
-    function = {
-        "start": ec2_session.start,
-        "ssh": ec2_session.ssh,
-        "forward": ec2_session.port_forward,
-    }
-    function.get(arguments.action)()
+        function = {
+            "start": ec2_session.start,
+            "ssh": ec2_session.ssh,
+            "forward": ec2_session.port_forward,
+        }
+        function.get(arguments.action)()
+    except exceptions.ClientError as err:
+        print(err)
+        exit(1)
```

### Comparing `aws_ssm_juggle-24.5.3/aws_ssm_juggle/ecs.py` & `aws_ssm_juggle-24.5.4/aws_ssm_juggle/ecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,69 +310,73 @@
         arguments.cluster,
         arguments.service,
         arguments.task,
         arguments.container,
         remote_port,
         None,
     )
-    while not menu_loop_condition(
-        cluster=cluster,
-        service=service,
-        task=task,
-        container=container,
-        remote_port=remote_port,
-        action=arguments.action,
-    ):
-        cluster, _ = get_cluster(ecs=ecs, cluster=cluster)
-        cluster, service, _ = get_service(ecs=ecs, cluster=cluster, service=service)
-        cluster, service, task, _ = get_task(ecs=ecs, cluster=cluster, service=service, task=task)
-        if cluster and task:
-            task_details = ecs.describe_tasks(cluster=cluster, tasks=[task])
-            containers = [container.get("name") for container in task_details.get("tasks")[0].get("containers")]
-            ret = get_container(
-                cluster=cluster,
-                service=service,
-                task=task,
-                containers=containers,
-                container=container,
-            )
-            task, container, container_index = ret
-        if (arguments.action == "forward" and container) and not remote_port:
-            task_definition_arn = task_details.get("tasks")[0].get("taskDefinitionArn")
-            task_definition = task_definition or ecs.describe_task_definition(taskDefinition=task_definition_arn).get(
-                "taskDefinition"
-            )
-            ports = [
-                str(container.get("containerPort"))
-                for container in task_definition.get("containerDefinitions")[container_index].get("portMappings")
-            ]
-            container, remote_port, _ = get_port(
-                cluster=cluster,
-                service=service,
-                task=task,
-                container=container,
-                containers=containers,
-                ports=ports,
-                port=remote_port,
-            )
-    ecs_session = ECSSession(
-        cluster=cluster,
-        boto3_session=boto3_session,
-        command=command,
-        container=container,
-        container_index=container_index,
-        local_port=local_port,
-        remote_port=remote_port,
-        task=task,
-        task_details=task_details,
-    )
-    function = {
-        "forward": ecs_session.port_forward,
-        "command": ecs_session.execute_command,
-    }
-    print("---")
-    print(f"cluster: {cluster}")
-    print(f"service: {service}")
-    print(f"task: {task}")
-    print(f"container: {container}")
-    print("---")
-    function.get(arguments.action)()
+    try:
+        while not menu_loop_condition(
+            cluster=cluster,
+            service=service,
+            task=task,
+            container=container,
+            remote_port=remote_port,
+            action=arguments.action,
+        ):
+            cluster, _ = get_cluster(ecs=ecs, cluster=cluster)
+            cluster, service, _ = get_service(ecs=ecs, cluster=cluster, service=service)
+            cluster, service, task, _ = get_task(ecs=ecs, cluster=cluster, service=service, task=task)
+            if cluster and task:
+                task_details = ecs.describe_tasks(cluster=cluster, tasks=[task])
+                containers = [container.get("name") for container in task_details.get("tasks")[0].get("containers")]
+                ret = get_container(
+                    cluster=cluster,
+                    service=service,
+                    task=task,
+                    containers=containers,
+                    container=container,
+                )
+                task, container, container_index = ret
+            if (arguments.action == "forward" and container) and not remote_port:
+                task_definition_arn = task_details.get("tasks")[0].get("taskDefinitionArn")
+                task_definition = task_definition or ecs.describe_task_definition(taskDefinition=task_definition_arn).get(
+                    "taskDefinition"
+                )
+                ports = [
+                    str(container.get("containerPort"))
+                    for container in task_definition.get("containerDefinitions")[container_index].get("portMappings")
+                ]
+                container, remote_port, _ = get_port(
+                    cluster=cluster,
+                    service=service,
+                    task=task,
+                    container=container,
+                    containers=containers,
+                    ports=ports,
+                    port=remote_port,
+                )
+        ecs_session = ECSSession(
+            cluster=cluster,
+            boto3_session=boto3_session,
+            command=command,
+            container=container,
+            container_index=container_index,
+            local_port=local_port,
+            remote_port=remote_port,
+            task=task,
+            task_details=task_details,
+        )
+        function = {
+            "forward": ecs_session.port_forward,
+            "command": ecs_session.execute_command,
+        }
+        print("---")
+        print(f"cluster: {cluster}")
+        print(f"service: {service}")
+        print(f"task: {task}")
+        print(f"container: {container}")
+        print("---")
+        function.get(arguments.action)()
+    except exceptions.ClientError as err:
+        print(err)
+        exit(1)
```

### Comparing `aws_ssm_juggle-24.5.3/pyproject.toml` & `aws_ssm_juggle-24.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-ssm-juggle"
-version = "24.5.3"
+version = "24.5.4"
 description = "AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)"
 authors = ["Stefan Heitmüller <stefan.heitmueller@gmx.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/morph027/aws-ssm-juggle"
 
 [tool.poetry.dependencies]
```

### Comparing `aws_ssm_juggle-24.5.3/PKG-INFO` & `aws_ssm_juggle-24.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-juggle
-Version: 24.5.3
+Version: 24.5.4
 Summary: AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)
 Home-page: https://github.com/morph027/aws-ssm-juggle
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```

