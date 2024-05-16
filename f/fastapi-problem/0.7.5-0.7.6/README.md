# Comparing `tmp/fastapi_problem-0.7.5.tar.gz` & `tmp/fastapi_problem-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_problem-0.7.5.tar", max compression
+gzip compressed data, was "fastapi_problem-0.7.6.tar", max compression
```

## Comparing `fastapi_problem-0.7.5.tar` & `fastapi_problem-0.7.6.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11307 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/LICENSE
--rw-r--r--   0        0        0     1905 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/README.md
--rw-r--r--   0        0        0     2228 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/src/fastapi_problem/__init__.py
--rw-r--r--   0        0        0      220 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/src/fastapi_problem/cors.py
--rw-r--r--   0        0        0     3407 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/src/fastapi_problem/error.py
--rw-r--r--   0        0        0        0 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/src/fastapi_problem/handler/__init__.py
--rw-r--r--   0        0        0     5955 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/src/fastapi_problem/handler/base.py
--rw-r--r--   0        0        0     2976 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/src/fastapi_problem/handler/fastapi.py
--rw-r--r--   0        0        0     2225 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/src/fastapi_problem/handler/starlette.py
--rw-r--r--   0        0        0      297 2024-05-13 10:40:24.979704 fastapi_problem-0.7.5/src/fastapi_problem/handler/util.py
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 fastapi_problem-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/LICENSE
+-rw-r--r--   0        0        0     1888 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/README.md
+-rw-r--r--   0        0        0     2177 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/src/fastapi_problem/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/src/fastapi_problem/cors.py
+-rw-r--r--   0        0        0     3444 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/src/fastapi_problem/error.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/src/fastapi_problem/handler/__init__.py
+-rw-r--r--   0        0        0     5959 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/src/fastapi_problem/handler/base.py
+-rw-r--r--   0        0        0     2977 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/src/fastapi_problem/handler/fastapi.py
+-rw-r--r--   0        0        0      299 2024-05-15 09:45:31.099707 fastapi_problem-0.7.6/src/fastapi_problem/handler/util.py
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 fastapi_problem-0.7.6/PKG-INFO
```

### Comparing `fastapi_problem-0.7.5/LICENSE` & `fastapi_problem-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_problem-0.7.5/README.md` & `fastapi_problem-0.7.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# FastAPI Problems v0.7.5
+# FastAPI Problems
 [![image](https://img.shields.io/pypi/v/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/l/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/pyversions/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 ![style](https://github.com/NRWLDev/fastapi-problem/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/fastapi-problem/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/fastapi-problem/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/fastapi-problem)
 
-`fastapi_problem` is a set of exceptions and handlers for use in starlette/fastapi
+`fastapi_problem` is a set of exceptions and handlers for use in fastapi
 applications to support easy error management and responses
 
 Each exception easily marshals to JSON based on the
 [RFC9457](https://www.rfc-editor.org/rfc/rfc9457.html) spec for use in api
 errors.
 
 Check the [docs](https://nrwldev.github.io/fastapi-problem) for more details.
```

### Comparing `fastapi_problem-0.7.5/pyproject.toml` & `fastapi_problem-0.7.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-problem"
-version = "0.7.5"
+version = "0.7.6"
 description = "FastAPI support for RFC9457 problems."
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/NRWLDev/fastapi-problem/"
 homepage="https://github.com/NRWLDev/fastapi-problem/"
 readme = "README.md"
 
@@ -23,22 +23,19 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3.0"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.7.5"
+current_version = "0.7.6"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
-filename = "README.md"
-
-[[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
 
 [tool.changelog_gen]
 release = true
 commit = true
```

### Comparing `fastapi_problem-0.7.5/src/fastapi_problem/error.py` & `fastapi_problem-0.7.6/src/fastapi_problem/error.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,31 +18,31 @@
     All exceptions should inherit from this or a subclass of it (depending on the usage),
     this will allow all apps and libraries to maintain a common exception chain
     """
 
     def __init__(
         self: t.Self,
         title: str,
-        code: str | None = None,
+        type_: str | None = None,
         details: str | None = None,
         status: int = 500,
         **kwargs,
     ) -> None:
         super().__init__(title)
-        self._code = code
+        self._type = type_
         self.title = title
         self.details = details
         self.status = status
         self.extras = kwargs
 
     @property
     def type(self: t.Self) -> str:
         type_ = "".join(self.__class__.__name__.rsplit("Error", 1))
         type_ = CONVERT_RE.sub("-", type_).lower()
-        return self._code if self._code else type_
+        return self._type if self._type else type_
 
     def marshal(self: t.Self, *, strip_debug: bool = False) -> dict[str, t.Any]:
         """Generate a JSON compatible representation.
 
         Args:
         ----
             strip_debug: If true, remove anything that is not title/type.
@@ -65,34 +65,35 @@
         return ret
 
 
 class HttpException(Problem):
     def __init__(
         self: t.Self,
         title: str,
-        code: str | None = None,
+        type_: str | None = None,
         details: str | None = None,
         status: int = 500,
         **kwargs,
     ) -> None:
         warn(
             "HttpException use is deprecated, use `Problem` subclasses instead.",
             FutureWarning,
             stacklevel=2,
         )
-        super().__init__(title, code=code, details=details, status=status, **kwargs)
+        super().__init__(title, type_=type_, details=details, status=status, **kwargs)
 
 
 class StatusProblem(Problem):
     code = None
+    type_ = None
     title = "Base http exception."
     status = 500
 
     def __init__(self: t.Self, details: str | None = None, **kwargs) -> None:
-        super().__init__(self.title, code=self.code, details=details, status=self.status, **kwargs)
+        super().__init__(self.title, type_=self.type_ or self.code, details=details, status=self.status, **kwargs)
 
 
 class HttpCodeException(StatusProblem):
     def __init__(self: t.Self, details: str | None = None, **kwargs) -> None:
         warn(
             "HttpCodeException use is deprecated, use `StatusProblem` subclasses instead.",
             FutureWarning,
```

### Comparing `fastapi_problem-0.7.5/src/fastapi_problem/handler/base.py` & `fastapi_problem-0.7.6/src/fastapi_problem/handler/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 Handler = t.Callable[["ExceptionHandler", Request, Exception], tuple[dict, Problem]]
 PreHook = t.Callable[[Request, JSONResponse], JSONResponse]
 PostHook = t.Callable[[Request, Exception], None]
 
 
 def http_exception_handler(eh: ExceptionHandler, _request: Request, exc: HTTPException) -> tuple[dict, Problem]:
     wrapper = eh.unhandled_wrappers.get(str(exc.status_code))
-    title, code = convert_status_code(exc.status_code)
+    title, type_ = convert_status_code(exc.status_code)
     details = exc.detail
     ret = (
         wrapper(details)
         if wrapper
         else Problem(
             title=title,
-            code=code,
+            type_=type_,
             details=details,
             status=exc.status_code,
         )
     )
     headers = exc.headers or {}
 
     return headers, ret
@@ -70,15 +70,15 @@
         wrapper = self.unhandled_wrappers.get("default", self.unhandled_wrappers.get("500"))
         ret = (
             wrapper(str(exc))
             if wrapper
             else Problem(
                 title="Unhandled exception occurred.",
                 details=str(exc),
-                code="unhandled-exception",
+                type_="unhandled-exception",
             )
         )
         headers = {}
 
         for exc_type, handler in self.handlers.items():
             if isinstance(exc, exc_type):
                 headers_, ret = handler(self, request, exc)
```

### Comparing `fastapi_problem-0.7.5/src/fastapi_problem/handler/fastapi.py` & `fastapi_problem-0.7.6/src/fastapi_problem/handler/fastapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     errors = json.loads(json.dumps(exc.errors(), default=str))
     kwargs = {"errors": errors}
     ret = (
         wrapper(**kwargs)
         if wrapper
         else Problem(
             title="Request validation error.",
-            code="request-validation-failed",
+            type_="request-validation-failed",
             status=422,
             **kwargs,
         )
     )
 
     return {}, ret
```

### Comparing `fastapi_problem-0.7.5/PKG-INFO` & `fastapi_problem-0.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-problem
-Version: 0.7.5
+Version: 0.7.6
 Summary: FastAPI support for RFC9457 problems.
 Home-page: https://github.com/NRWLDev/fastapi-problem/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: edgy.edgemond@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,23 +12,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/NRWLDev/fastapi-problem/
 Description-Content-Type: text/markdown
 
-# FastAPI Problems v0.7.5
+# FastAPI Problems
 [![image](https://img.shields.io/pypi/v/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/l/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/pyversions/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 ![style](https://github.com/NRWLDev/fastapi-problem/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/fastapi-problem/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/fastapi-problem/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/fastapi-problem)
 
-`fastapi_problem` is a set of exceptions and handlers for use in starlette/fastapi
+`fastapi_problem` is a set of exceptions and handlers for use in fastapi
 applications to support easy error management and responses
 
 Each exception easily marshals to JSON based on the
 [RFC9457](https://www.rfc-editor.org/rfc/rfc9457.html) spec for use in api
 errors.
 
 Check the [docs](https://nrwldev.github.io/fastapi-problem) for more details.
```

