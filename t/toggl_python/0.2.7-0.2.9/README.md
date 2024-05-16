# Comparing `tmp/toggl_python-0.2.7.tar.gz` & `tmp/toggl_python-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toggl_python-0.2.7.tar", last modified: Wed Dec 23 08:16:59 2020, max compression
+gzip compressed data, was "toggl_python-0.2.9.tar", max compression
```

## Comparing `toggl_python-0.2.7.tar` & `toggl_python-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1070 2020-12-23 08:12:19.720000 toggl_python-0.2.7/LICENSE
--rw-r--r--   0        0        0     1374 2020-12-23 08:12:19.720000 toggl_python-0.2.7/README.md
--rw-r--r--   0        0        0     1414 2020-12-23 08:12:19.720000 toggl_python-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1093 2020-12-23 08:12:19.720000 toggl_python-0.2.7/toggl_python/__init__.py
--rw-r--r--   0        0        0     1891 2020-12-23 08:12:19.720000 toggl_python-0.2.7/toggl_python/api.py
--rw-r--r--   0        0        0      244 2020-12-23 08:12:19.720000 toggl_python-0.2.7/toggl_python/auth.py
--rw-r--r--   0        0        0     3531 2020-12-23 08:12:19.720000 toggl_python-0.2.7/toggl_python/entities.py
--rw-r--r--   0        0        0      456 2020-12-23 08:12:19.720000 toggl_python-0.2.7/toggl_python/exceptions.py
--rw-r--r--   0        0        0     8283 2020-12-23 08:12:19.720000 toggl_python-0.2.7/toggl_python/repository.py
--rw-r--r--   0        0        0      583 2020-12-23 08:12:19.720000 toggl_python-0.2.7/toggl_python/response.py
--rw-r--r--   0        0        0     2102 2020-12-23 08:16:59.770000 toggl_python-0.2.7/setup.py
--rw-r--r--   0        0        0     2190 2020-12-23 08:16:59.770000 toggl_python-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-14 13:54:47.928217 toggl_python-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1811 2024-05-14 13:54:47.928217 toggl_python-0.2.9/README.md
+-rw-r--r--   0        0        0     1527 2024-05-16 07:18:29.442678 toggl_python-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1007 2024-05-14 13:54:47.930216 toggl_python-0.2.9/toggl_python/__init__.py
+-rw-r--r--   0        0        0     2300 2024-05-14 13:54:47.930216 toggl_python-0.2.9/toggl_python/api.py
+-rw-r--r--   0        0        0      335 2024-05-14 13:54:47.930216 toggl_python-0.2.9/toggl_python/auth.py
+-rw-r--r--   0        0        0     3773 2024-05-14 13:54:47.930216 toggl_python-0.2.9/toggl_python/entities.py
+-rw-r--r--   0        0        0      840 2024-05-14 13:54:47.930216 toggl_python-0.2.9/toggl_python/exceptions.py
+-rw-r--r--   0        0        0     8868 2024-05-14 13:54:47.931217 toggl_python-0.2.9/toggl_python/repository.py
+-rw-r--r--   0        0        0      779 2024-05-14 13:54:47.931217 toggl_python-0.2.9/toggl_python/response.py
+-rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 toggl_python-0.2.9/PKG-INFO
```

### Comparing `toggl_python-0.2.7/LICENSE` & `toggl_python-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `toggl_python-0.2.7/README.md` & `toggl_python-0.2.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,26 +12,44 @@
 * Documentation: https://toggl-python.readthedocs.io.  
 
 
 Installation
 ------------
 `pip install toggl-python` or use [poetry](https://python-poetry.org) `poetry add toggl-python`
 
-Features
---------
+Usage example
+-------------
 
-- Get TimeEntries.
+Get authenticated user time entries:
 
 ```python
 from toggl_python import TokenAuth, TimeEntries
 
 if __name__ == "__main__":
     auth = TokenAuth('AUTH_TOKEN')
     print(TimeEntries(auth=auth).list())
 ```
 
-* *TODO*
+Get information about the authenticated user:
+
+```python
+from toggl_python import TokenAuth, Users
+
+if __name__ == "__main__":
+    auth = TokenAuth('AUTH_TOKEN')
+    print(Users(auth=auth).me())
+```
+
+Get information about authenticated user workspaces:
+
+```python
+from toggl_python import TokenAuth, Workspaces
+
+if __name__ == "__main__":
+    auth = TokenAuth('AUTH_TOKEN')
+    print(Workspaces(auth=auth).list())
+```
 
 Credits
 -------
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
```

### Comparing `toggl_python-0.2.7/toggl_python/__init__.py` & `toggl_python-0.2.9/toggl_python/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,50 +14,47 @@
     Tag,
     Task,
     TimeEntry,
     User,
     Workspace,
     WorkspaceUser,
 )
-from .repository import Projects  # noqa: F401
 from .repository import (
     Clients,
     Dashboards,
     Groups,
     ProjectUsers,
     ReportTimeEntries,
     Tags,
-    Tasks,
     TimeEntries,
     Users,
     Workspaces,
     WorkspaceUsers,
 )
 
+
 __all__ = [
     "Activity",
     "BasicAuth",
     "BaseEntity",
     "Client",
     "Clients",
     "Dashboard",
     "Dashboards",
     "Group",
     "Groups",
     "MostActiveUser",
     "Project",
-    "Projects",
     "ProjectUser",
     "ProjectUsers",
     "ReportTimeEntry",
     "ReportTimeEntries",
     "Tag",
     "Tags",
     "Task",
-    "Tasks",
     "TimeEntries",
     "TimeEntry",
     "TokenAuth",
     "User",
     "Users",
     "Workspace",
     "Workspaces",
```

### Comparing `toggl_python-0.2.7/toggl_python/api.py` & `toggl_python-0.2.9/toggl_python/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 import typing
 from functools import partial
 from typing import Any, Dict, Optional
 
 import httpx
 
 from .auth import BasicAuth, TokenAuth
-from .exceptions import STATUS_2_EXCEPTION
+from .exceptions import raise_from_response
 
 
 class Api:
-    """Simple api wraper."""
+    """
+    Simple api wrapper.
+    Allow to interact with official Toggl API via httpx.
+    """
 
-    BASE_URL: httpx.URL = httpx.URL("https://www.toggl.com/api/v8/")
+    BASE_URL: httpx.URL = httpx.URL("https://api.track.toggl.com/api/v9/")
     HEADERS = {
         "content-type": "application/json",
         "user_agent": "toggl-python",
     }
 
     def __init__(
         self,
@@ -25,14 +28,21 @@
         auth: Optional[typing.Union[BasicAuth, TokenAuth]] = None,
     ):
         if base_url:
             self.BASE_URL = httpx.URL(base_url)
         self.client = httpx.Client(base_url=self.BASE_URL, auth=auth)
 
     def __getattr__(self, httpmethod: str) -> Any:
+        """
+        Checking existence of `httpmethod` method in httpx-client
+        and `partial` it to our client `api_method`
+
+        :param httpmethod: method name we trying to serve
+        :return:
+        """
         try:
             method = getattr(self.client, httpmethod)
         except AttributeError:
             raise AttributeError(f"No such http method ({httpmethod})!")
 
         return partial(self.api_method, method)
 
@@ -41,15 +51,22 @@
         method: Any,
         url: str,
         params: Optional[Dict[str, Any]] = None,
         data: Optional[Dict[str, Any]] = None,
         files: Optional[Dict[str, Any]] = None,
     ) -> Any:
         """
-        Call http method with specified url and params
+        Call httpx method with specified url and params
+
+        :param method: method we throwed from httpx-client via `__getattr__`
+        :param url: target url we nesting on `BASE_URL`
+        :param params: params to pass
+        :param data: json-data to pass
+        :param files: files to pass
+        :return:
         """
 
         _url = self.BASE_URL.join(url)
 
         response = (
             method(_url, params=params, headers=self.HEADERS)
             if method.__name__ == "get"
@@ -57,12 +74,11 @@
                 _url,
                 params=params,
                 json=data,
                 files=files,
                 headers=self.HEADERS,
             )
         )
-        if response.status_code == httpx.codes.OK:
-            return response
-        else:
-            exception_class = STATUS_2_EXCEPTION[response.status_code]
-            raise exception_class(response.text)
+
+        raise_from_response(response)
+
+        return response
```

### Comparing `toggl_python-0.2.7/toggl_python/entities.py` & `toggl_python-0.2.9/toggl_python/entities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Callable, List, Optional, Union
 
-from pydantic import BaseModel, EmailStr, HttpUrl
+from pydantic import BaseModel, EmailStr, Field, HttpUrl
 
 
 class BaseEntity(BaseModel):
     id: Optional[int] = None
     at: Optional[datetime] = None
 
 
@@ -13,26 +13,26 @@
     name: str
     wid: int
     notes: Optional[str] = None
 
 
 class Group(BaseEntity):
     name: str
-    wid: int
+    wid: int = Field(alias="workspace_id")
 
 
 class Project(BaseEntity):
     name: str
     wid: int
     cid: Optional[int] = None
     active: bool = True
     is_private: bool = True
     template: Optional[bool] = None
     template_id: Optional[int] = None
-    billable: bool = True
+    billable: Optional[bool] = True
     auto_estimates: Optional[bool] = False
     estimated_hours: Optional[int] = None
     color: Union[str, int] = 0
     rate: Optional[float] = None
     created_at: Optional[datetime] = None
 
 
@@ -44,36 +44,37 @@
     manage: Optional[bool] = False
     rate: Optional[float] = None
     full_name: Optional[float] = None
 
 
 class Tag(BaseEntity):
     name: str
-    wid: int
+    wid: int = Field(alias="workspace_id")
 
 
 class Task(BaseEntity):
     name: str
-    pid: int
-    wid: int
-    uid: Optional[int] = None
+    pid: int = Field(alias="project_id")
+    wid: int = Field(alias="workspace_id")
+    uid: Optional[int] = Field(alias="user_id", default=None)
     estimated_seconds: Optional[int] = None
+    tracked_seconds: Optional[int] = None
     active: Optional[bool] = True
 
 
 class TimeEntry(BaseEntity):
     wid: int
     pid: Optional[int] = None
     tid: Optional[int] = None
     description: Optional[str] = None
     billable: Optional[bool] = False
     start: Union[datetime, Callable[[], datetime]] = datetime.now
     stop: Optional[Union[datetime, Callable[[], datetime]]] = None
     duration: int
-    created_with: Optional[str]
+    created_with: Optional[str] = None
     tags: List[str] = []
     duronly: Optional[bool] = None
 
 
 class ReportTimeEntry(BaseEntity):
     wid: Optional[int] = None
     pid: Optional[int] = None
@@ -85,49 +86,45 @@
     cur: Optional[Union[str, bool]] = False
     start: Union[datetime, Callable[[], datetime]] = datetime.now
     end: Optional[Union[datetime, Callable[[], datetime]]] = None
     dur: int
     tags: List[str] = []
 
 
-class User(BaseEntity):
-    api_token: Optional[str] = None
-    default_wid: Optional[int] = None
-    email: EmailStr
-    fullname: str
-    jquery_timeofday_format: str
-    jquery_date_format: str
-    timeofday_format: str
-    date_format: str
-    store_start_and_stop_time: bool
-    beginning_of_week: int = 0
-    language: str
-    image_url: HttpUrl
-    sidebar_piechart: bool
-    new_blog_post: Dict[str, Any] = None
-    send_product_emails: bool
-    send_weekly_report: bool
-    send_timer_notifications: bool
-    openid_enabled: bool
-    timezone: str
-
-
 class Workspace(BaseEntity):
     name: str
     premium: bool
     admin: bool
-    default_hourly_rate: float
+    default_hourly_rate: Optional[float] = None
     default_currency: str
     only_admins_may_create_projects: bool
     only_admins_see_billable_rates: bool
     rounding: int
     rounding_minutes: int
     logo_url: Optional[HttpUrl] = None
 
 
+class User(BaseEntity):
+    api_token: Optional[str] = None
+    default_wid: Optional[int] = Field(alias="default_workspace_id", default=None)
+    email: EmailStr
+    fullname: str
+    beginning_of_week: int = 0
+    image_url: Optional[HttpUrl] = None
+    openid_enabled: Optional[bool] = None
+    timezone: Optional[str] = None
+    country_id: Optional[int] = None
+    projects: Optional[Project] = None
+    tags: Optional[Tag] = None
+    tasks: Optional[Task] = None
+    time_entries: Optional[TimeEntry] = None
+    updated_at: str
+    workspaces: Optional[Workspace] = None
+
+
 class WorkspaceUser(BaseEntity):
     uid: int
     wid: int
     admin: bool
     active: bool
     name: Optional[str] = None
     email: Optional[EmailStr] = None
```

### Comparing `toggl_python-0.2.7/toggl_python/repository.py` & `toggl_python-0.2.9/toggl_python/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import partial
 from typing import Any, Dict, Optional, Tuple, Type, Union
 
 import httpx
 
 from .api import Api
+from .auth import BasicAuth, TokenAuth
 from .entities import (
     BaseEntity,
     Client,
     Dashboard,
     Group,
     Project,
     ProjectUser,
@@ -17,18 +18,22 @@
     TimeEntry,
     User,
     Workspace,
     WorkspaceUser,
 )
 from .exceptions import MethodNotAllowed, NotSupported
 from .response import ListResponse, ReportTimeEntriesList
-from .auth import BasicAuth, TokenAuth
 
 
 class BaseRepository(Api):
+    """
+    Base API-class for managing entities on Toggl side:
+    list, detail them and etc.
+    """
+
     LIST_URL = ""
     DETAIL_URL: Optional[str] = None
     ENTITY_CLASS: Type[BaseEntity] = BaseEntity
     ADDITIONAL_METHODS: Dict[str, Dict[str, Any]] = {}
     EXCLUDED_METHODS: Optional[Tuple[str, ...]] = None
     ADDITIONAL_PARAMS: Dict[str, Dict[str, Any]] = {}
     DATA_CONTAINER: Dict[str, Optional[str]] = {}
@@ -40,23 +45,28 @@
         auth: Optional[Union[BasicAuth, TokenAuth]] = None,
     ) -> None:
         super().__init__(base_url=base_url, auth=auth)
         if not self.DETAIL_URL:
             self.DETAIL_URL = self.LIST_URL + "/{id}"
 
     def __getattr__(self, attr: str) -> Any:
+        """
+        Trying to get `partial`ed method `attr` from httpx-client.
+        In case of fail -> try to get own method from `ADDITIONAL_METHODS`
+        and `partial`ing it as well from payload of `ADDITIONAL_METHODS` item.
+        :param attr:
+        :return:
+        """
         if self.EXCLUDED_METHODS and attr in self.EXCLUDED_METHODS:
             raise MethodNotAllowed
         try:
             method = super().__getattr__(attr)
         except AttributeError:
             if attr in self.ADDITIONAL_METHODS.keys():
-                method = partial(
-                    self.additionat_method, **self.ADDITIONAL_METHODS[attr]
-                )
+                method = partial(self.additionat_method, **self.ADDITIONAL_METHODS[attr])
             else:
                 raise AttributeError(f"No such method ({attr})!")
         return method
 
     def additionat_method(
         self,
         url: str,
@@ -67,48 +77,56 @@
         single_item: bool = False,
         data_key: Optional[str] = None,
         params: Optional[Dict[str, Any]] = None,
         data: Optional[Dict[str, Any]] = None,
         files: Optional[Dict[str, Any]] = None,
     ) -> Any:
         """
-        Call additional method with specified url and params
-        """
+        Call additional method with specified url and params.
 
+        :param url: url we use to build a target url
+        :param _id:
+        :param additional_id:
+        :param entity:
+        :param detail:
+        :param single_item:
+        :param data_key:
+        :param params: params to pass
+        :param data: json-data to pass
+        :param files: files to pass
+        :return:
+        """
         if detail:
             if not self.DETAIL_URL:
                 raise AttributeError("Not defined DETAIL_URL")
             _url = (self.DETAIL_URL + "/" + url + "/{additional_id}").format(
                 id=_id, additional_id=additional_id
             )
-            return self._retrieve(
-                _url, entity, headers=self.HEADERS, params=params
-            )
+            return self._retrieve(_url, entity, headers=self.HEADERS, params=params)
         elif _id:
             if not self.DETAIL_URL:
                 raise AttributeError("Not defined DETAIL_URL")
             _url = (self.DETAIL_URL + "/" + url).format(id=_id)
-            return self._list(_url, entity, headers=self.HEADERS, param=params)
+            return self._list(_url, entity, headers=self.HEADERS, param=params, data_key=data_key)
         elif single_item:
-            _url = str(self.BASE_URL) + "/" + url
+            _url = str(self.BASE_URL) + f"{url}"
             return self._retrieve(
                 _url,
                 entity,
                 headers=self.HEADERS,
                 params=params,
-                data_key="data",
             )
         else:
             raise NotSupported
 
     def _retrieve(
         self,
         _url: Union[str, httpx.URL],
         entity_class: Any,
-        data_key: Optional[str] = "data",
+        data_key: Optional[str] = None,
         **kwargs: Any,
     ) -> Any:
         params = kwargs
         params.update(self.ADDITIONAL_PARAMS.get("retrieve", {}))
 
         response = self.get(_url, params=params)
         data = response.json()
@@ -185,41 +203,31 @@
 
 
 class Groups(BaseRepository):
     LIST_URL = "groups"
     ENTITY_CLASS = Group
 
 
-class Projects(BaseRepository):
-    LIST_URL = "projects"
-    ENTITY_CLASS = Project
-
-
 class ProjectUsers(BaseRepository):
     LIST_URL = "project_users"
     ENTITY_CLASS = ProjectUser
 
 
 class Tags(BaseRepository):
     LIST_URL = "tags"
     ENTITY_CLASS = Tag
 
 
-class Tasks(BaseRepository):
-    LIST_URL = "tasks"
-    ENTITY_CLASS = Task
-
-
 class TimeEntries(BaseRepository):
-    LIST_URL = "time_entries"
+    LIST_URL = "me/time_entries"
     ENTITY_CLASS = TimeEntry
 
 
 class ReportTimeEntries(BaseRepository):
-    BASE_URL: httpx.URL = httpx.URL("https://toggl.com/reports/api/v2/")
+    BASE_URL: httpx.URL = httpx.URL("https://api.track.toggl.com/reports/api/v2/")
     ADDITIONAL_PARAMS = {"list": {"user_agent": "toggl_python"}}
     DATA_CONTAINER = {"list": "data"}
     LIST_URL = "details"
     ENTITY_CLASS = ReportTimeEntry
     LIST_RESPONSE = ReportTimeEntriesList
 
 
@@ -233,18 +241,19 @@
 
 
 class Workspaces(BaseRepository):
     LIST_URL = "workspaces"
     ENTITY_CLASS = Workspace
     ADDITIONAL_METHODS = {
         "projects": {"url": "projects", "entity": Project, "detail": False},
+        "detail_project": {"url": "projects", "entity": Project, "detail": True},
         "users": {"url": "users", "entity": User, "detail": False},
         "clients": {"url": "clients", "entity": Client, "detail": False},
         "groups": {"url": "groups", "entity": Group, "detail": False},
-        "tasks": {"url": "tasks", "entity": Task, "detail": False},
+        "tasks": {"url": "tasks", "entity": Task, "data_key": "data", "detail": False},
         "tags": {"url": "tags", "entity": Tag, "detail": False},
         "workspace_users": {
             "url": "workspace_users",
             "entity": WorkspaceUser,
             "detail": False,
         },
     }
```

### Comparing `toggl_python-0.2.7/toggl_python/response.py` & `toggl_python-0.2.9/toggl_python/response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from typing import Any, List, Tuple
 
 
 class ListResponse(List[Any]):
+    """
+    Base class for list response based from mutable sequence
+    """
+
     response_parameters: Tuple[str, ...] = ()
 
     def __init__(self, value: Any, response_body: Any):
         super(ListResponse, self).__init__(value)
 
         for parameter in self.response_parameters:
             if parameter in response_body:
                 setattr(self, parameter, response_body[parameter])
 
 
 class ReportTimeEntriesList(ListResponse):
+    """
+    Simple ListResponse, extended with params `response_parameters`
+    from `response_body` on init
+    """
+
     response_parameters = (
         "total_count",
         "per_page",
         "total_grand",
         "total_billable",
         "total_currencies",
     )
```

### Comparing `toggl_python-0.2.7/setup.py` & `toggl_python-0.2.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,78 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: toggl_python
+Version: 0.2.9
+Summary: Python wrapper for Toggl API.
+Home-page: https://github.com/evrone/toggl_python
+Author: Ivlev Denis
+Author-email: me@dierz.pro
+Requires-Python: >=3.12,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: httpx[http2] (>=0.25.1,<0.26.0)
+Requires-Dist: pydantic[email] (>=2.5.1,<3.0.0)
+Project-URL: Documentation, https://toggl-python.readthedocs.io
+Project-URL: Repository, https://github.com/evrone/toggl_python
+Description-Content-Type: text/markdown
+
+Toggl Python API
+================
+
+![https://pypi.python.org/pypi/toggl_python](https://img.shields.io/pypi/v/toggl_python.svg) ![https://travis-ci.com/evrone/toggl_python](https://img.shields.io/travis/evrone/toggl_python.svg) ![https://toggl-python.readthedocs.io/en/latest/?badge=latest](https://readthedocs.org/projects/toggl-python/badge/?version=latest) ![https://pyup.io/repos/github/evrone/toggl_python/](https://pyup.io/repos/github/evrone/toggl_python/shield.svg)
+
+
+Toggl Python API
+----------------
+[<img src="https://evrone.com/logo/evrone-sponsored-logo.png" width=231>](https://evrone.com/?utm_source=github.com)  
+* Based on open Toggl API documentation: https://github.com/toggl/toggl_api_docs/blob/master/toggl_api.md
+* Free software: MIT license
+* Documentation: https://toggl-python.readthedocs.io.  
+
+
+Installation
+------------
+`pip install toggl-python` or use [poetry](https://python-poetry.org) `poetry add toggl-python`
+
+Usage example
+-------------
+
+Get authenticated user time entries:
+
+```python
+from toggl_python import TokenAuth, TimeEntries
+
+if __name__ == "__main__":
+    auth = TokenAuth('AUTH_TOKEN')
+    print(TimeEntries(auth=auth).list())
+```
+
+Get information about the authenticated user:
+
+```python
+from toggl_python import TokenAuth, Users
+
+if __name__ == "__main__":
+    auth = TokenAuth('AUTH_TOKEN')
+    print(Users(auth=auth).me())
+```
+
+Get information about authenticated user workspaces:
+
+```python
+from toggl_python import TokenAuth, Workspaces
+
+if __name__ == "__main__":
+    auth = TokenAuth('AUTH_TOKEN')
+    print(Workspaces(auth=auth).list())
+```
 
-packages = \
-['toggl_python']
+Credits
+-------
 
-package_data = \
-{'': ['*']}
+This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
 
-install_requires = \
-['httpx[http2]>=0.16.1,<0.17.0', 'pydantic[email]>=1.7.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'toggl-python',
-    'version': '0.2.7',
-    'description': 'Python wrapper for Toggl API.',
-    'long_description': 'Toggl Python API\n================\n\n![https://pypi.python.org/pypi/toggl_python](https://img.shields.io/pypi/v/toggl_python.svg) ![https://travis-ci.com/evrone/toggl_python](https://img.shields.io/travis/evrone/toggl_python.svg) ![https://toggl-python.readthedocs.io/en/latest/?badge=latest](https://readthedocs.org/projects/toggl-python/badge/?version=latest) ![https://pyup.io/repos/github/evrone/toggl_python/](https://pyup.io/repos/github/evrone/toggl_python/shield.svg)\n\n\nToggl Python API\n----------------\n[<img src="https://evrone.com/logo/evrone-sponsored-logo.png" width=231>](https://evrone.com/?utm_source=github.com)  \n* Based on open Toggl API documentation: https://github.com/toggl/toggl_api_docs/blob/master/toggl_api.md\n* Free software: MIT license\n* Documentation: https://toggl-python.readthedocs.io.  \n\n\nInstallation\n------------\n`pip install toggl-python` or use [poetry](https://python-poetry.org) `poetry add toggl-python`\n\nFeatures\n--------\n\n- Get TimeEntries.\n\n```python\nfrom toggl_python import TokenAuth, TimeEntries\n\nif __name__ == "__main__":\n    auth = TokenAuth(\'AUTH_TOKEN\')\n    print(TimeEntries(auth=auth).list())\n```\n\n* *TODO*\n\nCredits\n-------\n\nThis package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.\n',
-    'author': 'Ivlev Denis',
-    'author_email': 'me@dierz.pro',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/evrone/toggl_python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

