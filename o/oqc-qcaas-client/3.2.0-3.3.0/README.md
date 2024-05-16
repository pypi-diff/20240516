# Comparing `tmp/oqc_qcaas_client-3.2.0.tar.gz` & `tmp/oqc_qcaas_client-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqc_qcaas_client-3.2.0.tar", max compression
+gzip compressed data, was "oqc_qcaas_client-3.3.0.tar", max compression
```

## Comparing `oqc_qcaas_client-3.2.0.tar` & `oqc_qcaas_client-3.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1453 2024-04-23 10:55:04.228104 oqc_qcaas_client-3.2.0/LICENSE
--rw-r--r--   0        0        0      350 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/README.md
--rw-r--r--   0        0        0       89 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/qcaas_client/__init__.py
--rw-r--r--   0        0        0    36050 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/qcaas_client/client.py
--rw-r--r--   0        0        0     4981 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/qcaas_client/commandline.py
--rw-r--r--   0        0        0      142 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/qcaas_client/config.py
--rw-r--r--   0        0        0    16377 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/client/scc/compiler/config.py
--rw-r--r--   0        0        0        0 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/__init__.py
--rw-r--r--   0        0        0      745 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/config.py
--rw-r--r--   0        0        0     3915 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/enums.py
--rw-r--r--   0        0        0      539 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/json_utils.py
--rw-r--r--   0        0        0      831 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/log_reduct.py
--rw-r--r--   0        0        0     3202 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/logger.py
--rw-r--r--   0        0        0     3368 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/metrics.py
--rw-r--r--   0        0        0     2207 2024-04-23 10:55:04.218103 oqc_qcaas_client-3.2.0/common/qcaas_common/type_conversions.py
--rw-r--r--   0        0        0     1827 2024-04-23 10:55:12.878618 oqc_qcaas_client-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 oqc_qcaas_client-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1453 2024-05-08 09:24:53.782728 oqc_qcaas_client-3.3.0/LICENSE
+-rw-r--r--   0        0        0      350 2024-05-08 09:24:53.722723 oqc_qcaas_client-3.3.0/client/README.md
+-rw-r--r--   0        0        0       89 2024-05-08 09:24:53.722723 oqc_qcaas_client-3.3.0/client/qcaas_client/__init__.py
+-rw-r--r--   0        0        0    36173 2024-05-08 09:24:53.722723 oqc_qcaas_client-3.3.0/client/qcaas_client/client.py
+-rw-r--r--   0        0        0     4981 2024-05-08 09:24:53.722723 oqc_qcaas_client-3.3.0/client/qcaas_client/commandline.py
+-rw-r--r--   0        0        0      142 2024-05-08 09:24:53.722723 oqc_qcaas_client-3.3.0/client/qcaas_client/config.py
+-rw-r--r--   0        0        0    16377 2024-05-08 09:24:53.722723 oqc_qcaas_client-3.3.0/client/scc/compiler/config.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:24:53.772727 oqc_qcaas_client-3.3.0/common/qcaas_common/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-08 09:24:53.772727 oqc_qcaas_client-3.3.0/common/qcaas_common/config.py
+-rw-r--r--   0        0        0     3915 2024-05-08 09:24:53.772727 oqc_qcaas_client-3.3.0/common/qcaas_common/enums.py
+-rw-r--r--   0        0        0      539 2024-05-08 09:24:53.772727 oqc_qcaas_client-3.3.0/common/qcaas_common/json_utils.py
+-rw-r--r--   0        0        0      831 2024-05-08 09:24:53.772727 oqc_qcaas_client-3.3.0/common/qcaas_common/log_reduct.py
+-rw-r--r--   0        0        0     3202 2024-05-08 09:24:53.772727 oqc_qcaas_client-3.3.0/common/qcaas_common/logger.py
+-rw-r--r--   0        0        0     3368 2024-05-08 09:24:53.772727 oqc_qcaas_client-3.3.0/common/qcaas_common/metrics.py
+-rw-r--r--   0        0        0     2207 2024-05-08 09:24:53.772727 oqc_qcaas_client-3.3.0/common/qcaas_common/type_conversions.py
+-rw-r--r--   0        0        0     1827 2024-05-08 09:25:04.133464 oqc_qcaas_client-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 oqc_qcaas_client-3.3.0/PKG-INFO
```

### Comparing `oqc_qcaas_client-3.2.0/LICENSE` & `oqc_qcaas_client-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/client/qcaas_client/client.py` & `oqc_qcaas_client-3.3.0/client/qcaas_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,31 +66,34 @@
         }
         if self.hybrid_marker:
             task["hybrid_marker"] = self.hybrid_marker
         return task
 
 
 class QPUTaskResult:
+
     def __init__(self, id_, result=None, metrics=None, error_details=None):
         self.id = id_
         self.result = result
         self.metrics = metrics or dict()
         self.error_details: QPUTaskErrors = error_details
 
     def has_errored(self):
         return self.error_details is not None
 
 
 class QPUTaskErrors:
+
     def __init__(self, error_message, error_code=None):
         self.error_code = error_code or -1
         self.error_message = error_message
 
 
 def retry_on_expired_token(func):
+
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         try:
             return func(self, *args, **kwargs)
         except ExpiredTokenException:
             self._authentication_token = None
             return func(self, *args, **kwargs)
@@ -102,23 +105,22 @@
     results = []
     unscheduled_tasks = [task for task in tasks if task not in scheduled_tasks]
     for task in unscheduled_tasks:
         results.append(
             QPUTaskResult(
                 id_=task.task_id,
                 error_details=QPUTaskErrors("Failed to schedule task."),
-            )
-        )
+            ))
     return results
 
 
 class OQCClient:
-    def __init__(
-        self, url, email=None, password=None, timeout=(5, 25), authentication_token=None
-    ):
+
+    def __init__(self, url, email=None, password=None, timeout=(5, 25),
+                 authentication_token=None):
         self.server_version = None
         self._authentication_token = authentication_token
         self._qpus = None
         self.timeout = timeout
         self.default_qpu_id = "qpu:uk:2:0eb3cf2363"
         if email:
             self._email = _validated_email(email)
@@ -130,16 +132,15 @@
             self._password = None
 
         if url is None:
             raise ValueError("Need a URL to connect too.")
 
         if (email and not password) or (password and not email):
             raise ValueError(
-                "If one of email and password are provided, both must be provided"
-            )
+                "If one of email and password are provided, both must be provided")
 
         if authentication_token and (email or password):
             raise ValueError(
                 "If one authentication_token is specified, email and password must not be specified"
             )
 
         # build the user agent
@@ -156,16 +157,15 @@
         self.url = _validated_url(url)
         server_version = self._get("/admin/version", authenticate=False).json()
         self.server_version = server_version["version"]
         if self.server_version >= 3:
             self.get_qpus()
         if self.server_version == 2 and authentication_token:
             raise ValueError(
-                "You can't provide an authentication_token for this server"
-            )
+                "You can't provide an authentication_token for this server")
 
     @property
     def email(self):
         return self._email
 
     @email.setter
     def email(self, value):
@@ -179,33 +179,27 @@
     @password.setter
     def password(self, value):
         self._password = _validated_password(value)
         self._authentication_token = None  # Clear existing token to force re-auth.
 
     def _handle_response_error(self, response):
         if not self.server_version and response.status_code != 200:
-            raise ServerException(
-                response.content.decode("utf-8"), response.status_code
-            )
-        if (
-            self.server_version
-            and self.server_version >= 3
-            and response.status_code == 401
-        ):
+            raise ServerException(response.content.decode("utf-8"),
+                                  response.status_code)
+        if (self.server_version and self.server_version >= 3
+                and response.status_code == 401):
             raise ServerException("Authentication Error", response.status_code, {})
 
         if response.status_code != 200:
             # Right now we can, occasionally, return HTML blobs. Looks ugly,
             # but better than parsing exception.
-            if not response.headers.get("content-type", "").startswith(
-                "application/json"
-            ):
-                raise ServerException(
-                    response.content.decode("utf-8"), response.status_code
-                )
+            if not response.headers.get("content-type",
+                                        "").startswith("application/json"):
+                raise ServerException(response.content.decode("utf-8"),
+                                      response.status_code)
             else:
                 exception_info = response.json()
                 exception_keys = exception_info.keys()
                 if self.server_version >= 3 and "response" in exception_info:
                     raise ServerException(
                         exception_info["response"]["errors"][0],
                         response.status_code,
@@ -226,17 +220,16 @@
                             exception_info,
                         )
                     # FEATURE REQUEST: Replace string match;
                     # requires configuring JWT expired error
                     if "Token has expired" in message:
                         raise ExpiredTokenException(message, exception_info)
                     else:
-                        raise ServerException(
-                            message, response.status_code, exception_info
-                        )
+                        raise ServerException(message, response.status_code,
+                                              exception_info)
 
     def _handle_response_messages(self, response):
         try:
             response = response.json()
             if isinstance(response, dict):
                 messages = [response.get("message", "")]
                 messages.extend(response.get("messages", []))
@@ -267,17 +260,16 @@
         )
         self._handle_response_error(response)
         self._handle_response_messages(response)
 
         return response
 
     @retry_on_expired_token
-    def _get(
-        self, endpoint, params=None, data=None, json=None, authenticate=True, **kwargs
-    ):
+    def _get(self, endpoint, params=None, data=None, json=None, authenticate=True,
+             **kwargs):
         """Helper for get requests. Applies common info such as headers etc."""
         if authenticate:
             self.authenticate()
         headers = kwargs.get("headers", self._build_headers())
         if not endpoint.startswith("http"):
             endpoint = self.url + endpoint
         response = requests.get(
@@ -337,32 +329,27 @@
         self._handle_response_messages(response)
 
         return response
 
     def authenticate(self):
         if self._authentication_token is not None:
             return True
-        if (
-            self._email is None
-            and self._password is None
-            and self._authentication_token is None
-        ):
+        if (self._email is None and self._password is None
+                and self._authentication_token is None):
             return False
 
         payload = {"email": self._email or "", "password": self._password or ""}
         if self.server_version == 3:
             self._post("/admin/logout", {}, authenticate=False)
-            auth = self._post(
-                "/admin/login?include_auth_token=true", payload, authenticate=False
-            )
+            auth = self._post("/admin/login?include_auth_token=true", payload,
+                              authenticate=False)
             self._handle_response_messages(auth)
             response = auth.json()
             self._authentication_token = response["response"]["user"][
-                "authentication_token"
-            ]
+                "authentication_token"]
         else:
             auth = self._post("/auth", payload, authenticate=False)
             self._handle_response_messages(auth)
             response = auth.json()
             self._authentication_token = response["access_token"]
 
         return self._authentication_token is not None
@@ -407,16 +394,15 @@
         return headers
 
     def get_token_expiry_time(self) -> Optional[str]:
         if self._authentication_token is None:
             return None
         if self.server_version == 3:
             auth_token = self._get(
-                f"/admin/auth_tokens/{self._authentication_token}"
-            ).json()
+                f"/admin/auth_tokens/{self._authentication_token}").json()
             expires_at = auth_token["expires_at"]
             expires_time = datetime.strptime(expires_at, "%Y-%m-%dT%H:%M:%S")
             base_date = datetime(1970, 1, 1)
             expires_timestamp = (expires_time - base_date).total_seconds()
             return int(expires_timestamp)
         else:
             return self._get("/admin/token_expiry").json()
@@ -425,20 +411,18 @@
         """Change the users password"""
         if self.server_version == 3:
             user = self.get_user_info(email, validate)
             if user:
                 response = self._post(
                     f"/admin/users/{user['id']}/update_password",
                     json={
-                        "password": (
-                            _validated_password(password) if validate else password
-                        ),
-                        "password_confirm": (
-                            _validated_password(password) if validate else password
-                        ),
+                        "password":
+                        (_validated_password(password) if validate else password),
+                        "password_confirm":
+                        (_validated_password(password) if validate else password),
                     },
                 )
             else:
                 return None
         else:
             response = self._put(
                 "/admin/users/passwords",
@@ -459,15 +443,17 @@
             if user:
                 results = self._get(f"/admin/users/{user['id']}").json()
             else:
                 return None
         else:
             results = self._get(
                 "/admin/users/password_expiry",
-                {"email": _validated_email(email) if validate else email},
+                {
+                    "email": _validated_email(email) if validate else email
+                },
             ).json()
         return results.get("password_expires_at", None)
 
     def get_user_info(self, email, validate=True):
         if self.server_version == 3:
             results = self._get(
                 f"/admin/users?q={quote(_validated_email(email) if validate else email)}"
@@ -476,15 +462,17 @@
             if results["total"] > 0:
                 return results["items"][0]
             else:
                 return None
         else:
             results = self._get(
                 "/admin/users",
-                {"email": _validated_email(email) if validate else email},
+                {
+                    "email": _validated_email(email) if validate else email
+                },
             ).json()
             return results
 
     def get_next_window(self, qpu_id=None):
         """
         Fetches the next active window.
 
@@ -494,16 +482,15 @@
         endpoint = self._get_qpu_endpoint(qpu_id)
         next_window_dict = self._get(endpoint + "/windows/next").json()
 
         if next_window_dict == {} or "next_window" not in next_window_dict:
             return None
 
         return _validate_datetime_format(
-            next_window_dict.get("next_window").get("starting")
-        )
+            next_window_dict.get("next_window").get("starting"))
 
     def create_one_off_window_(
         self,
         qpu_id,
         start_datetime,
         end_datetime,
         lease_type,
@@ -646,27 +633,27 @@
         # FEATURE REQUEST: Add processing timeout.
         results = []
         scheduled_count = len(scheduled_tasks)
         current_task_index = 0
         retry_attempt = 0
         while current_task_index < scheduled_count:
             scheduled_task = scheduled_tasks[current_task_index]
-            task_info = self.get_task(scheduled_task.task_id)
+            task_info = self.get_task(scheduled_task.task_id, scheduled_task.qpu_id)
             status = self._get_task_status(task_info)
             if status == TaskStatus.FAILED.value:
                 logging.info(f"{scheduled_task.task_id} failed execution.")
                 error_details = self._get_task_errors(task_info)
                 results.append(
-                    QPUTaskResult(scheduled_task.task_id, error_details=error_details)
-                )
+                    QPUTaskResult(scheduled_task.task_id, error_details=error_details))
             elif status == TaskStatus.COMPLETED.value:
                 logging.info(f"{scheduled_task.task_id} completed execution.")
                 qpu_result = self._get_task_results(scheduled_task.task_id, task_info)
                 if include_metrics:
-                    qpu_result.metrics = self.get_task_metrics(scheduled_task.task_id)
+                    qpu_result.metrics = self.get_task_metrics(
+                        scheduled_task.task_id, scheduled_task.qpu_id)
                 results.append(qpu_result)
 
             # If we have a new result, process the next block, otherwise
             # retry with increasing delay.
             if current_task_index != len(results):
                 current_task_index = len(results)
                 retry_attempt = 0
@@ -678,46 +665,46 @@
         if not isinstance(tasks, list):
             tasks = [tasks]
 
         results.extend(_get_unscheduled_tasks_results(tasks, scheduled_tasks))
 
         return results
 
-    def create_task_ids(
-        self, ntasks: int, qpu_id: str = None, tag: str = None
-    ) -> List[str]:
+    def create_task_ids(self, ntasks: int, qpu_id: str = None,
+                        tag: str = None) -> List[str]:
         if self.server_version >= 3:
             server = self._get_qpu_endpoint(qpu_id)
             return self._post(
                 f"{server}/tasks",
-                json={"qpu_id": qpu_id, "task_count": ntasks, "tag": tag},
+                json={
+                    "qpu_id": qpu_id,
+                    "task_count": ntasks,
+                    "tag": tag
+                },
             ).json()
         else:
             return self._post(f"/tasks?n={ntasks}").json()
 
-    def schedule_tasks(
-        self, tasks: Union[QPUTask, List[QPUTask]], qpu_id: str = None, tag: str = None
-    ) -> List[QPUTask]:
+    def schedule_tasks(self, tasks: Union[QPUTask, List[QPUTask]], qpu_id: str = None,
+                       tag: str = None) -> List[QPUTask]:
         """
         Schedules all tasks to run on the QPU and updates the task objects with the
         associated run ID's. Automatically disconnects socket unless
         auto_disconnect=False. If wait for acknowledgement the set of tasks returned
         will contain only those that are confirmed to have been schedueled, otherwise
         will just return all tasks.
         """
 
         if not isinstance(tasks, List):
             tasks = [tasks]
 
         invalid_tasks = [task for task in tasks if not isinstance(task, QPUTask)]
         if any(invalid_tasks):
-            raise ValueError(
-                f"{', '.join([str(task) for task in invalid_tasks])}"
-                f" are invalid types to try and schedule."
-            )
+            raise ValueError(f"{', '.join([str(task) for task in invalid_tasks])}"
+                             f" are invalid types to try and schedule.")
 
         if self.server_version >= 3:
             # if qpu_id is provided, set it on all tasks
             if qpu_id:
                 for task in tasks:
                     task.qpu_id = qpu_id
             else:
@@ -862,26 +849,27 @@
         endpoint = f"/tasks/{str(task_id)}/timings"
         if self.server_version >= 3:
             server = self._get_qpu_endpoint(qpu_id)
             endpoint = server + endpoint
         metadata = self._get(endpoint).json()
         return metadata.get("timings", None)
 
-    def get_task_execution_estimates(
-        self, task_ids: Union[uuid4, list[uuid4]], qpu_id: str = None
-    ):
+    def get_task_execution_estimates(self, task_ids: Union[uuid4, list[uuid4]],
+                                     qpu_id: str = None):
         if not isinstance(task_ids, list):
             task_ids = [task_ids]
         endpoint = "/monitoring/task_wait_time"
         if self.server_version >= 3:
             server = self._get_qpu_endpoint(qpu_id)
             endpoint = server + endpoint
         return self._post(
             endpoint,
-            json={"task_ids": [str(id) for id in task_ids]},
+            json={
+                "task_ids": [str(id) for id in task_ids]
+            },
         ).json()
 
     def get_qpu_execution_estimates(self, qpu_ids: Union[str, list[str]] = None):
         if qpu_ids is None:
             qpu_ids = self.default_qpu_id
         if not isinstance(qpu_ids, list):
             qpu_ids = [qpu_ids]
@@ -908,15 +896,17 @@
                     for wait_time in resp1["qpu_wait_times"]:
                         response["qpu_wait_times"].append(wait_time)
 
             return response
         else:
             return self._post(
                 "/monitoring/qpu_wait_time",
-                json={"targets": [str(id) for id in qpu_ids]},
+                json={
+                    "targets": [str(id) for id in qpu_ids]
+                },
             ).json()
 
     def cancel_task(self, task_ids: Union[uuid4, list[uuid4]], qpu_id: str = None):
         if not isinstance(task_ids, list):
             task_ids = [task_ids]
 
         endpoint = "/tasks/cancel_many"
```

### Comparing `oqc_qcaas_client-3.2.0/client/qcaas_client/commandline.py` & `oqc_qcaas_client-3.3.0/client/qcaas_client/commandline.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/client/scc/compiler/config.py` & `oqc_qcaas_client-3.3.0/client/scc/compiler/config.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/common/qcaas_common/config.py` & `oqc_qcaas_client-3.3.0/common/qcaas_common/config.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/common/qcaas_common/enums.py` & `oqc_qcaas_client-3.3.0/common/qcaas_common/enums.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/common/qcaas_common/json_utils.py` & `oqc_qcaas_client-3.3.0/common/qcaas_common/json_utils.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/common/qcaas_common/log_reduct.py` & `oqc_qcaas_client-3.3.0/common/qcaas_common/log_reduct.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/common/qcaas_common/logger.py` & `oqc_qcaas_client-3.3.0/common/qcaas_common/logger.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/common/qcaas_common/metrics.py` & `oqc_qcaas_client-3.3.0/common/qcaas_common/metrics.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/common/qcaas_common/type_conversions.py` & `oqc_qcaas_client-3.3.0/common/qcaas_common/type_conversions.py`

 * *Files identical despite different names*

### Comparing `oqc_qcaas_client-3.2.0/pyproject.toml` & `oqc_qcaas_client-3.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "oqc_qcaas_client"
-version = "3.2.0"
+version = "3.3.0"
 description = "OQC Quantum Computing as a Service (QCaaS)"
 authors = [ "OQC <oqc_qcaas_support@oxfordquantumcircuits.com>",]
 readme = "client/README.md"
 exclude = [ ".env",]
 license = "BSD-3-Clause"
 source = []
 [[tool.poetry.packages]]
```

### Comparing `oqc_qcaas_client-3.2.0/PKG-INFO` & `oqc_qcaas_client-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oqc_qcaas_client
-Version: 3.2.0
+Version: 3.3.0
 Summary: OQC Quantum Computing as a Service (QCaaS)
 License: BSD-3-Clause
 Author: OQC
 Author-email: oqc_qcaas_support@oxfordquantumcircuits.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

