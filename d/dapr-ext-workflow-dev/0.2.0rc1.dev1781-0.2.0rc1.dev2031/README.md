# Comparing `tmp/dapr-ext-workflow-dev-0.2.0rc1.dev1781.tar.gz` & `tmp/dapr-ext-workflow-dev-0.2.0rc1.dev2031.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapr-ext-workflow-dev-0.2.0rc1.dev1781.tar", last modified: Mon Nov 27 17:25:42 2023, max compression
+gzip compressed data, was "dapr-ext-workflow-dev-0.2.0rc1.dev2031.tar", last modified: Thu May 16 01:44:44 2024, max compression
```

## Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781.tar` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 17:25:42.897680 dapr-ext-workflow-dev-0.2.0rc1.dev1781/
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-11-27 17:25:42.897680 dapr-ext-workflow-dev-0.2.0rc1.dev1781/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 17:25:42.893680 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 17:25:42.893680 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 17:25:42.897680 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/dapr_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/dapr_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/workflow_activity_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/workflow_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/workflow_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 17:25:42.897680 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr_ext_workflow_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-11-27 17:25:42.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr_ext_workflow_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-11-27 17:25:42.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr_ext_workflow_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 17:25:42.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr_ext_workflow_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-27 17:25:42.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr_ext_workflow_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-27 17:25:42.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr_ext_workflow_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      911 2023-11-27 17:25:42.897680 dapr-ext-workflow-dev-0.2.0rc1.dev1781/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-11-27 17:25:26.000000 dapr-ext-workflow-dev-0.2.0rc1.dev1781/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:44.790928 dapr-ext-workflow-dev-0.2.0rc1.dev2031/
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-16 01:44:44.790928 dapr-ext-workflow-dev-0.2.0rc1.dev2031/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:44.786928 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:44.786928 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:44.786928 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/dapr_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/dapr_workflow_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:44.786928 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/logger/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/retry_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/workflow_activity_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/workflow_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/workflow_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:44.790928 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr_ext_workflow_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-16 01:44:44.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr_ext_workflow_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-16 01:44:44.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr_ext_workflow_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:44:44.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr_ext_workflow_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 01:44:44.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr_ext_workflow_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 01:44:44.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr_ext_workflow_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 01:44:44.790928 dapr-ext-workflow-dev-0.2.0rc1.dev2031/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-16 01:44:30.000000 dapr-ext-workflow-dev-0.2.0rc1.dev2031/setup.py
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/LICENSE` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/PKG-INFO` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapr-ext-workflow-dev
-Version: 0.2.0rc1.dev1781
+Version: 0.2.0rc1.dev2031
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # Import your main classes here
-from dapr.ext.workflow.workflow_runtime import WorkflowRuntime
+from dapr.ext.workflow.workflow_runtime import WorkflowRuntime, alternate_name
 from dapr.ext.workflow.dapr_workflow_client import DaprWorkflowClient
 from dapr.ext.workflow.dapr_workflow_context import DaprWorkflowContext, when_all, when_any
 from dapr.ext.workflow.workflow_activity_context import WorkflowActivityContext
 from dapr.ext.workflow.workflow_state import WorkflowState, WorkflowStatus
+from dapr.ext.workflow.retry_policy import RetryPolicy
 
 __all__ = [
     'WorkflowRuntime',
     'DaprWorkflowClient',
     'DaprWorkflowContext',
     'WorkflowActivityContext',
     'WorkflowState',
     'WorkflowStatus',
     'when_all',
-    'when_any'
+    'when_any',
+    'alternate_name',
+    'RetryPolicy',
 ]
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/dapr_workflow_client.py` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/dapr_workflow_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,47 +23,66 @@
 from dapr.ext.workflow.workflow_context import Workflow
 from dapr.ext.workflow.util import getAddress
 
 from dapr.clients import DaprInternalError
 from dapr.clients.http.client import DAPR_API_TOKEN_HEADER
 from dapr.conf import settings
 from dapr.conf.helpers import GrpcEndpoint
+from dapr.ext.workflow.logger import LoggerOptions, Logger
 
 T = TypeVar('T')
 TInput = TypeVar('TInput')
 TOutput = TypeVar('TOutput')
 
 
 class DaprWorkflowClient:
     """Defines client operations for managing Dapr Workflow instances.
 
-       This is an alternative to the general purpose Dapr client. It uses a gRPC connection to send
-       commands directly to the workflow engine, bypassing the Dapr API layer.
+    This is an alternative to the general purpose Dapr client. It uses a gRPC connection to send
+    commands directly to the workflow engine, bypassing the Dapr API layer.
 
-       This client is intended to be used by workflow application, not by general purpose
-       application.
+    This client is intended to be used by workflow application, not by general purpose
+    application.
     """
 
-    def __init__(self, host: Optional[str] = None, port: Optional[str] = None):
+    def __init__(
+        self,
+        host: Optional[str] = None,
+        port: Optional[str] = None,
+        logger_options: Optional[LoggerOptions] = None,
+    ):
         address = getAddress(host, port)
 
         try:
             uri = GrpcEndpoint(address)
         except ValueError as error:
             raise DaprInternalError(f'{error}') from error
 
+        self._logger = Logger('DaprWorkflowClient', logger_options)
+
         metadata = tuple()
         if settings.DAPR_API_TOKEN:
             metadata = ((DAPR_API_TOKEN_HEADER, settings.DAPR_API_TOKEN),)
-        self.__obj = client.TaskHubGrpcClient(host_address=uri.endpoint, metadata=metadata,
-                                              secure_channel=uri.tls)
-
-    def schedule_new_workflow(self, workflow: Workflow, *, input: Optional[TInput] = None,
-                              instance_id: Optional[str] = None,
-                              start_at: Optional[datetime] = None) -> str:
+        options = self._logger.get_options()
+        self.__obj = client.TaskHubGrpcClient(
+            host_address=uri.endpoint,
+            metadata=metadata,
+            secure_channel=uri.tls,
+            log_handler=options.log_handler,
+            log_formatter=options.log_formatter,
+        )
+
+    def schedule_new_workflow(
+        self,
+        workflow: Workflow,
+        *,
+        input: Optional[TInput] = None,
+        instance_id: Optional[str] = None,
+        start_at: Optional[datetime] = None,
+    ) -> str:
         """Schedules a new workflow instance for execution.
 
         Args:
             workflow: The workflow to schedule.
             input: The optional input to pass to the scheduled workflow instance. This must be a
             serializable value.
             instance_id: The unique ID of the workflow instance to schedule. If not specified, a
@@ -71,19 +90,28 @@
             start_at: The time when the workflow instance should start executing.
             If not specified or if a date-time in the past is specified, the workflow instance will
             be scheduled immediately.
 
         Returns:
             The ID of the scheduled workflow instance.
         """
-        return self.__obj.schedule_new_orchestration(workflow.__name__, input=input,
-                                                     instance_id=instance_id, start_at=start_at)
-
-    def get_workflow_state(self, instance_id: str, *,
-                           fetch_payloads: bool = True) -> Optional[WorkflowState]:
+        if hasattr(workflow, '_dapr_alternate_name'):
+            return self.__obj.schedule_new_orchestration(
+                workflow.__dict__['_dapr_alternate_name'],
+                input=input,
+                instance_id=instance_id,
+                start_at=start_at,
+            )
+        return self.__obj.schedule_new_orchestration(
+            workflow.__name__, input=input, instance_id=instance_id, start_at=start_at
+        )
+
+    def get_workflow_state(
+        self, instance_id: str, *, fetch_payloads: bool = True
+    ) -> Optional[WorkflowState]:
         """Fetches runtime state for the specified workflow instance.
 
         Args:
             instanceId: The unique ID of the workflow instance to fetch.
             fetch_payloads: If true, fetches the input, output payloads and custom status
             for the workflow instance. Defaults to false.
 
@@ -91,16 +119,17 @@
             The current state of the workflow instance, or None if the workflow instance does not
             exist.
 
         """
         state = self.__obj.get_orchestration_state(instance_id, fetch_payloads=fetch_payloads)
         return WorkflowState(state) if state else None
 
-    def wait_for_workflow_start(self, instance_id: str, *, fetch_payloads: bool = False,
-                                timeout_in_seconds: int = 60) -> Optional[WorkflowState]:
+    def wait_for_workflow_start(
+        self, instance_id: str, *, fetch_payloads: bool = False, timeout_in_seconds: int = 60
+    ) -> Optional[WorkflowState]:
         """Waits for a workflow to start running and returns a WorkflowState object that contains
            metadata about the started workflow.
 
            A "started" workflow instance is any instance not in the WorkflowRuntimeStatus.Pending
            state. This method will return a completed task if the workflow has already started
            running or has already completed.
 
@@ -111,20 +140,22 @@
             timeout_in_seconds: The maximum time to wait for the workflow instance to start running.
             Defaults to 60 seconds.
 
         Returns:
             WorkflowState record that describes the workflow instance and its execution status.
             If the specified workflow isn't found, the WorkflowState.Exists value will be false.
         """
-        state = self.__obj.wait_for_orchestration_start(instance_id, fetch_payloads=fetch_payloads,
-                                                        timeout=timeout_in_seconds)
+        state = self.__obj.wait_for_orchestration_start(
+            instance_id, fetch_payloads=fetch_payloads, timeout=timeout_in_seconds
+        )
         return WorkflowState(state) if state else None
 
-    def wait_for_workflow_completion(self, instance_id: str, *, fetch_payloads: bool = True,
-                                     timeout_in_seconds: int = 60) -> Optional[WorkflowState]:
+    def wait_for_workflow_completion(
+        self, instance_id: str, *, fetch_payloads: bool = True, timeout_in_seconds: int = 60
+    ) -> Optional[WorkflowState]:
         """Waits for a workflow to complete and returns a WorkflowState object that contains
            metadata about the started instance.
 
            A "completed" workflow instance is any instance in one of the terminal states. For
            example, the WorkflowRuntimeStatus.Completed, WorkflowRuntimeStatus.Failed or
            WorkflowRuntimeStatus.Terminated states.
 
@@ -142,21 +173,22 @@
             for the workflow instance. Defaults to true.
             timeout_in_seconds: The maximum time in seconds to wait for the workflow instance to
             complete. Defaults to 60 seconds.
 
         Returns:
             WorkflowState record that describes the workflow instance and its execution status.
         """
-        state = self.__obj.wait_for_orchestration_completion(instance_id,
-                                                             fetch_payloads=fetch_payloads,
-                                                             timeout=timeout_in_seconds)
+        state = self.__obj.wait_for_orchestration_completion(
+            instance_id, fetch_payloads=fetch_payloads, timeout=timeout_in_seconds
+        )
         return WorkflowState(state) if state else None
 
-    def raise_workflow_event(self, instance_id: str, event_name: str, *,
-                             data: Optional[Any] = None):
+    def raise_workflow_event(
+        self, instance_id: str, event_name: str, *, data: Optional[Any] = None
+    ):
         """Sends an event notification message to a waiting workflow instance.
            In order to handle the event, the target workflow instance must be waiting for an
            event named value of "eventName" param using the wait_for_external_event API.
            If the target workflow instance is not yet waiting for an event named param "eventName"
            value, then the event will be saved in the workflow instance state and dispatched
            immediately when the workflow calls wait_for_external_event.
            This event saving occurs even if the workflow has canceled its wait operation before
@@ -179,26 +211,27 @@
     def terminate_workflow(self, instance_id: str, *, output: Optional[Any] = None):
         """Terminates a running workflow instance and updates its runtime status to
            WorkflowRuntimeStatus.Terminated This method internally enqueues a "terminate" message in
            the task hub. When the task hub worker processes this message, it will update the runtime
            status of the target instance to WorkflowRuntimeStatus.Terminated. You can use
            wait_for_workflow_completion to wait for the instance to reach the terminated state.
 
-           Terminating a workflow instance has no effect on any in-flight activity function
-           executions or child workflows that were started by the terminated instance. Those
-           actions will continue to run without interruption. However, their results will be
-           discarded. If you want to terminate child-workflows, you must issue separate terminate
-           commands for each child workflow instance individually.
+           Terminating a workflow will terminate all child workflows that were started by
+           the workflow instance.
+
+           However, terminating a workflow has no effect on any in-flight activity function
+           executions that were started by the terminated workflow instance.
 
            At the time of writing, there is no way to terminate an in-flight activity execution.
 
         Args:
             instance_id: The ID of the workflow instance to terminate.
             output: The optional output to set for the terminated workflow instance.
-       """
+
+        """
         return self.__obj.terminate_orchestration(instance_id, output=output)
 
     def pause_workflow(self, instance_id: str):
         """Suspends a workflow instance, halting processing of it until resume_workflow is used to
            resume the workflow.
 
         Args:
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/util.py` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from typing import Optional
 
 from dapr.conf import settings
 
 
 def getAddress(host: Optional[str] = None, port: Optional[str] = None) -> str:
     if not host and not port:
-        address = settings.DAPR_GRPC_ENDPOINT or (f"{settings.DAPR_RUNTIME_HOST}:"
-                                                  f"{settings.DAPR_GRPC_PORT}")
+        address = settings.DAPR_GRPC_ENDPOINT or (
+            f'{settings.DAPR_RUNTIME_HOST}:' f'{settings.DAPR_GRPC_PORT}'
+        )
     else:
         host = host or settings.DAPR_RUNTIME_HOST
         port = port or settings.DAPR_GRPC_PORT
-        address = f"{host}:{port}"
+        address = f'{host}:{port}'
 
     return address
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/version.py` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/version.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__version__ = "0.2.0rc1.dev"
+__version__ = '0.2.0rc1.dev'
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/workflow_activity_context.py` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/workflow_activity_context.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from durabletask import task
 
 T = TypeVar('T')
 TInput = TypeVar('TInput')
 TOutput = TypeVar('TOutput')
 
 
-class WorkflowActivityContext():
+class WorkflowActivityContext:
     """Defines properties and methods for task activity context objects."""
 
     def __init__(self, ctx: task.ActivityContext):
         self.__obj = ctx
 
     @property
     def workflow_id(self) -> str:
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/workflow_context.py` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/workflow_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 T = TypeVar('T')
 TInput = TypeVar('TInput')
 TOutput = TypeVar('TOutput')
 
 
 class WorkflowContext(ABC):
     """Context object used by workflow implementations to perform actions such as scheduling
-       activities, durable timers, waiting for external events, and for getting basic information
-       about the current workflow instance.
+    activities, durable timers, waiting for external events, and for getting basic information
+    about the current workflow instance.
     """
 
     @property
     @abstractmethod
     def instance_id(self) -> str:
         """Get the ID of the current workflow instance.
 
@@ -97,16 +97,17 @@
         -------
         Task
             A Durable Timer Task that schedules the timer to wake up the orchestrator
         """
         pass
 
     @abstractmethod
-    def call_activity(self, activity: Activity[TOutput], *,
-                      input: Optional[TInput] = None) -> task.Task[TOutput]:
+    def call_activity(
+        self, activity: Activity[TOutput], *, input: Optional[TInput] = None
+    ) -> task.Task[TOutput]:
         """Schedule an activity for execution.
 
         Parameters
         ----------
         activity: Activity[TInput, TOutput]
             A reference to the activity function to call.
         input: TInput | None
@@ -118,17 +119,21 @@
         -------
         Task
             A Durable Task that completes when the called activity function completes or fails.
         """
         pass
 
     @abstractmethod
-    def call_child_workflow(self, orchestrator: Workflow[TOutput], *,
-                            input: Optional[TInput] = None,
-                            instance_id: Optional[str] = None) -> task.Task[TOutput]:
+    def call_child_workflow(
+        self,
+        orchestrator: Workflow[TOutput],
+        *,
+        input: Optional[TInput] = None,
+        instance_id: Optional[str] = None,
+    ) -> task.Task[TOutput]:
         """Schedule child-workflow function for execution.
 
         Parameters
         ----------
         orchestrator: Orchestrator[TInput, TOutput]
             A reference to the orchestrator function to call.
         input: TInput
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr/ext/workflow/workflow_state.py` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr/ext/workflow/workflow_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,10 +68,10 @@
             'last_updated_at': self.__obj.last_updated_at,
             'serialized_input': self.__obj.serialized_input,
             'serialized_output': self.__obj.serialized_output,
             'serialized_custom_status': self.__obj.serialized_custom_status,
             'failure_details': {
                 'message': self.__obj.failure_details.message,
                 'error_type': self.__obj.failure_details.error_type,
-                'stack_trace': self.__obj.failure_details.stack_trace
-            }
+                'stack_trace': self.__obj.failure_details.stack_trace,
+            },
         }
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr_ext_workflow_dev.egg-info/PKG-INFO` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr_ext_workflow_dev.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapr-ext-workflow-dev
-Version: 0.2.0rc1.dev1781
+Version: 0.2.0rc1.dev2031
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/dapr_ext_workflow_dev.egg-info/SOURCES.txt` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/dapr_ext_workflow_dev.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 dapr/ext/workflow/__init__.py
 dapr/ext/workflow/dapr_workflow_client.py
 dapr/ext/workflow/dapr_workflow_context.py
+dapr/ext/workflow/retry_policy.py
 dapr/ext/workflow/util.py
 dapr/ext/workflow/version.py
 dapr/ext/workflow/workflow_activity_context.py
 dapr/ext/workflow/workflow_context.py
 dapr/ext/workflow/workflow_runtime.py
 dapr/ext/workflow/workflow_state.py
+dapr/ext/workflow/logger/__init__.py
+dapr/ext/workflow/logger/logger.py
+dapr/ext/workflow/logger/options.py
 dapr_ext_workflow_dev.egg-info/PKG-INFO
 dapr_ext_workflow_dev.egg-info/SOURCES.txt
 dapr_ext_workflow_dev.egg-info/dependency_links.txt
 dapr_ext_workflow_dev.egg-info/requires.txt
 dapr_ext_workflow_dev.egg-info/top_level.txt
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/setup.cfg` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 	Source = https://github.com/dapr/python-sdk
 
 [options]
 python_requires = >=3.8
 packages = find_namespace:
 include_package_data = True
 install_requires = 
-	dapr-dev >= 1.11.0rc1.dev
-	durabletask >= 0.1.0
+	dapr >= 1.13.0
+	durabletask >= 0.1.1a1
 
 [options.packages.find]
 include = 
 	dapr.*
 exclude = 
 	tests
```

### Comparing `dapr-ext-workflow-dev-0.2.0rc1.dev1781/setup.py` & `dapr-ext-workflow-dev-0.2.0rc1.dev2031/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 def is_release():
     return '.dev' not in __version__
 
 
 name = 'dapr-ext-workflow'
 version = __version__
 description = 'The official release of Dapr Python SDK Workflow Authoring Extension.'
-long_description = '''
+long_description = """
 This is the Workflow authoring extension for Dapr.
 
 Dapr is a portable, serverless, event-driven runtime that makes it easy for developers to
 build resilient, stateless and stateful microservices that run on the cloud and edge and
 embraces the diversity of languages and developer frameworks.
 
 Dapr codifies the best practices for building microservice applications into open,
 independent, building blocks that enable you to build portable applications with the language
 and framework of your choice. Each building block is independent and you can use one, some,
 or all of them in your application.
-'''.lstrip()
+""".lstrip()
 
 # Get build number from GITHUB_RUN_NUMBER environment variable
 build_number = os.environ.get('GITHUB_RUN_NUMBER', '0')
 
 if not is_release():
     name += '-dev'
     version = f'{__version__}{build_number}'
```

