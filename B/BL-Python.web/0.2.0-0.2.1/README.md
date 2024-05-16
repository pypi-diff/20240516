# Comparing `tmp/bl_python_web-0.2.0.tar.gz` & `tmp/bl_python_web-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_python_web-0.2.0.tar", last modified: Tue May 14 21:50:45 2024, max compression
+gzip compressed data, was "bl_python_web-0.2.1.tar", last modified: Thu May 16 21:19:29 2024, max compression
```

## Comparing `bl_python_web-0.2.0.tar` & `bl_python_web-0.2.1.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.967189 bl_python_web-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.931189 bl_python_web-0.2.0/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.939189 bl_python_web-0.2.0/BL_Python/web/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/encryption/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/encryption/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/dependency_injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/middleware/flask/
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/flask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/middleware/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)    19522 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/middleware/sso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24782 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/scaffolder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/
--rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__main__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_app_type.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_version.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.943189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/basic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/__main__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/_app_type.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/application.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__hook__.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__meta__.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/conftest.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test_{{meta.operation.module_name}}.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/BL_Python/web/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/BL_Python/web/testing/create_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/BL_Python.web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 21:50:45.000000 bl_python_web-0.2.0/BL_Python.web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-14 21:50:45.967189 bl_python_web-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:50:45.967189 bl_python_web-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.935189 bl_python_web-0.2.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/test/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.947189 bl_python_web-0.2.0/test/unit/application/
--rw-r--r--   0 runner    (1001) docker     (127)    14313 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/application/test_create_flask_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/application/test_create_openapi_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.951189 bl_python_web-0.2.0/test/unit/encryption/
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.951189 bl_python_web-0.2.0/test/unit/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_api_request_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_api_response_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_flask_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_openapi_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/middleware/test_sso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.951189 bl_python_web-0.2.0/test/unit/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/scaffolding/test_scaffolding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/test/unit/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.939189 bl_python_web-0.2.0/typings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.955189 bl_python_web-0.2.0/typings/connexion/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/__main__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.955189 bl_python_web-0.2.0/typings/connexion/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/apps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/apps/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/apps/asynchronous.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/apps/flask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/datastructures.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.955189 bl_python_web-0.2.0/typings/connexion/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/decorators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/decorators/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/decorators/parameter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/decorators/response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.955189 bl_python_web-0.2.0/typings/connexion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/frameworks/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/frameworks/flask.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/frameworks/starlette.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/http_facts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/json_schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/jsonifier.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/lifecycle.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.959189 bl_python_web-0.2.0/typings/connexion/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/lifespan.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/request_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/response_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/routing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/server_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/middleware/swagger_ui.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/mock.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.959189 bl_python_web-0.2.0/typings/connexion/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/operations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/operations/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/operations/openapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/operations/swagger2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/problem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/spec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/testing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/uri_parsing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.959189 bl_python_web-0.2.0/typings/connexion/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/abstract.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/form_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/json.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/connexion/validators/parameter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.959189 bl_python_web-0.2.0/typings/flask_injector/
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_injector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_injector/tests.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/flask_login/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/__about__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/login_manager.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/test_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/flask_login/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/connexion/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/connexion/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/fastapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/fastapi/implementation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/flask/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/flask/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/quart/
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/quart/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:50:45.963189 bl_python_web-0.2.0/typings/json_logging/framework/sanic/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework/sanic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/framework_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-14 21:50:42.000000 bl_python_web-0.2.0/typings/json_logging/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.945159 bl_python_web-0.2.1/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.953159 bl_python_web-0.2.1/BL_Python/web/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.953159 bl_python_web-0.2.1/BL_Python/web/encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/encryption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.953159 bl_python_web-0.2.1/BL_Python/web/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/middleware/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/middleware/dependency_injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.953159 bl_python_web-0.2.1/BL_Python/web/middleware/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/middleware/flask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.953159 bl_python_web-0.2.1/BL_Python/web/middleware/openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)    19522 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/middleware/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/middleware/sso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.953159 bl_python_web-0.2.1/BL_Python/web/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24782 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/scaffolder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.945159 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.953159 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.953159 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.953159 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__main__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_app_type.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/_version.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.945159 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/basic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.945159 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/__main__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/_app_type.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/endpoints/application.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.945159 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.945159 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.945159 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/templates/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__hook__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/__meta__.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/conftest.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test_{{meta.operation.module_name}}.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/BL_Python/web/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/BL_Python/web/testing/create_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/BL_Python.web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-16 21:19:29.000000 bl_python_web-0.2.1/BL_Python.web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-16 21:19:29.000000 bl_python_web-0.2.1/BL_Python.web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:19:29.000000 bl_python_web-0.2.1/BL_Python.web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 21:19:29.000000 bl_python_web-0.2.1/BL_Python.web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-16 21:19:29.000000 bl_python_web-0.2.1/BL_Python.web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 21:19:29.000000 bl_python_web-0.2.1/BL_Python.web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.949159 bl_python_web-0.2.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/test/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/test/unit/application/
+-rw-r--r--   0 runner    (1001) docker     (127)    14313 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/application/test_create_flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/application/test_create_openapi_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.957160 bl_python_web-0.2.1/test/unit/encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.961160 bl_python_web-0.2.1/test/unit/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/middleware/test_api_request_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/middleware/test_api_response_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/middleware/test_dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/middleware/test_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/middleware/test_flask_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/middleware/test_openapi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/middleware/test_sso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.961160 bl_python_web-0.2.1/test/unit/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/scaffolding/test_scaffolding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/test/unit/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.949159 bl_python_web-0.2.1/typings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.965160 bl_python_web-0.2.1/typings/connexion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.965160 bl_python_web-0.2.1/typings/connexion/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/apps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/apps/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/apps/asynchronous.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/apps/flask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/datastructures.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.965160 bl_python_web-0.2.1/typings/connexion/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/decorators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/decorators/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/decorators/parameter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/decorators/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.965160 bl_python_web-0.2.1/typings/connexion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/frameworks/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/frameworks/flask.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/frameworks/starlette.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/http_facts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/json_schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/jsonifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/lifecycle.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.969160 bl_python_web-0.2.1/typings/connexion/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/lifespan.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/request_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/response_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/routing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/server_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/middleware/swagger_ui.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/mock.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.969160 bl_python_web-0.2.1/typings/connexion/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/operations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/operations/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/operations/openapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/operations/swagger2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/problem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/uri_parsing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.969160 bl_python_web-0.2.1/typings/connexion/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/validators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/validators/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/validators/form_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/validators/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/connexion/validators/parameter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.969160 bl_python_web-0.2.1/typings/flask_injector/
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_injector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_injector/tests.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.969160 bl_python_web-0.2.1/typings/flask_login/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_login/__about__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_login/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_login/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_login/login_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_login/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_login/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_login/test_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/flask_login/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/typings/json_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/typings/json_logging/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/framework/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/typings/json_logging/framework/connexion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/framework/connexion/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/typings/json_logging/framework/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/framework/fastapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/framework/fastapi/implementation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/typings/json_logging/framework/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/framework/flask/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/typings/json_logging/framework/quart/
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/framework/quart/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:19:29.973160 bl_python_web-0.2.1/typings/json_logging/framework/sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/framework/sanic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/framework_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-16 21:19:26.000000 bl_python_web-0.2.1/typings/json_logging/util.pyi
```

### Comparing `bl_python_web-0.2.0/BL_Python/web/application.py` & `bl_python_web-0.2.1/BL_Python/web/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Flask entry point.
 """
 
 import logging
 from dataclasses import dataclass
 from os import environ, path
-from typing import Generic, Optional, TypeVar, cast
+from typing import Generator, Generic, Optional, TypeVar, cast
 
 import json_logging
 from BL_Python.AWS.ssm import SSMParameters
 from BL_Python.programming.config import AbstractConfig, ConfigBuilder, load_config
 from BL_Python.programming.dependency_injection import ConfigModule
 from connexion import FlaskApp
 from flask import Blueprint, Flask
@@ -161,15 +161,18 @@
     # This will allow subpackages to resolve their own config types,
     # allow for type safety against objects of those types.
     # Otherwise, they can resolve `AbstractConfig`, but then type
     # safety is lost.
     # Note that, if any `ConfigModule` is provided in `application_modules`,
     # those will override the automatically generated `ConfigModule`s.
     application_modules = [
-        ConfigModule(config, type(config)) for (_, config) in full_config
+        ConfigModule(config, type(config))
+        for (_, config) in cast(
+            Generator[tuple[str, AbstractConfig], None, None], full_config
+        )
     ] + (application_modules if application_modules else [])
     # The `full_config` module cannot be overridden unless the application
     # IoC container is fiddled with. `full_config` is the instance registered
     # to `AbstractConfig`.
     modules = application_modules + [ConfigModule(full_config, Config)]
     flask_injector = configure_dependencies(app, application_modules=modules)
```

### Comparing `bl_python_web-0.2.0/BL_Python/web/config.py` & `bl_python_web-0.2.1/BL_Python/web/config.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/encryption/__init__.py` & `bl_python_web-0.2.1/BL_Python/web/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/middleware/__init__.py` & `bl_python_web-0.2.1/BL_Python/web/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/middleware/consts.py` & `bl_python_web-0.2.1/BL_Python/web/middleware/consts.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/middleware/dependency_injection.py` & `bl_python_web-0.2.1/BL_Python/web/middleware/dependency_injection.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/middleware/flask/__init__.py` & `bl_python_web-0.2.1/BL_Python/web/middleware/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/middleware/openapi/__init__.py` & `bl_python_web-0.2.1/BL_Python/web/middleware/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/middleware/sso.py` & `bl_python_web-0.2.1/BL_Python/web/middleware/sso.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/__main__.py` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/__main__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/scaffolder.py` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/scaffolder.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/LICENSE.md.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/README.md.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/README.md.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/docs/CONFIGURATION.md.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/base/{{application.module_name}}/endpoints/application.py.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/basic/{{application.module_name}}/config.toml.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/config.toml.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/openapi/{{application.module_name}}/openapi.yaml.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/endpoints/{{operation.module_name}}.py.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/database/__hook__.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test_{{meta.operation.module_name}}.py.j2` & `bl_python_web-0.2.1/BL_Python/web/scaffolding/templates/optional/{{application.module_name}}/modules/test/templates/test_{{meta.operation.module_name}}.py.j2`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/testing/config.py` & `bl_python_web-0.2.1/BL_Python/web/testing/config.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python/web/testing/create_app.py` & `bl_python_web-0.2.1/BL_Python/web/testing/create_app.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/BL_Python.web.egg-info/PKG-INFO` & `bl_python_web-0.2.1/BL_Python.web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.web
-Version: 0.2.0
+Version: 0.2.1
 Summary: Libraries for building web applications in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bl_python_web-0.2.0/BL_Python.web.egg-info/SOURCES.txt` & `bl_python_web-0.2.1/BL_Python.web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/LICENSE.md` & `bl_python_web-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/PKG-INFO` & `bl_python_web-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.web
-Version: 0.2.0
+Version: 0.2.1
 Summary: Libraries for building web applications in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bl_python_web-0.2.0/README.md` & `bl_python_web-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/pyproject.toml` & `bl_python_web-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/application/test_create_flask_app.py` & `bl_python_web-0.2.1/test/unit/application/test_create_flask_app.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/application/test_create_openapi_app.py` & `bl_python_web-0.2.1/test/unit/application/test_create_openapi_app.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/encryption/test_encryption.py` & `bl_python_web-0.2.1/test/unit/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/middleware/test_api_request_handlers.py` & `bl_python_web-0.2.1/test/unit/middleware/test_api_request_handlers.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/middleware/test_api_response_handlers.py` & `bl_python_web-0.2.1/test/unit/middleware/test_api_response_handlers.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/middleware/test_dependency_injection.py` & `bl_python_web-0.2.1/test/unit/middleware/test_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/middleware/test_error_handlers.py` & `bl_python_web-0.2.1/test/unit/middleware/test_error_handlers.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/middleware/test_flask_middleware.py` & `bl_python_web-0.2.1/test/unit/middleware/test_flask_middleware.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/middleware/test_openapi_middleware.py` & `bl_python_web-0.2.1/test/unit/middleware/test_openapi_middleware.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/scaffolding/test_scaffolding.py` & `bl_python_web-0.2.1/test/unit/scaffolding/test_scaffolding.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/test/unit/test_config.py` & `bl_python_web-0.2.1/test/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/__init__.pyi` & `bl_python_web-0.2.1/typings/connexion/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/apps/abstract.pyi` & `bl_python_web-0.2.1/typings/connexion/apps/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/apps/asynchronous.pyi` & `bl_python_web-0.2.1/typings/connexion/apps/asynchronous.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/apps/flask.pyi` & `bl_python_web-0.2.1/typings/connexion/apps/flask.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/cli.pyi` & `bl_python_web-0.2.1/typings/connexion/cli.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/datastructures.pyi` & `bl_python_web-0.2.1/typings/connexion/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/decorators/main.pyi` & `bl_python_web-0.2.1/typings/connexion/decorators/main.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/decorators/parameter.pyi` & `bl_python_web-0.2.1/typings/connexion/decorators/parameter.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/decorators/response.pyi` & `bl_python_web-0.2.1/typings/connexion/decorators/response.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/exceptions.pyi` & `bl_python_web-0.2.1/typings/connexion/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/frameworks/abstract.pyi` & `bl_python_web-0.2.1/typings/connexion/frameworks/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/frameworks/flask.pyi` & `bl_python_web-0.2.1/typings/connexion/frameworks/flask.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/frameworks/starlette.pyi` & `bl_python_web-0.2.1/typings/connexion/frameworks/starlette.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/handlers.pyi` & `bl_python_web-0.2.1/typings/connexion/handlers.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/json_schema.pyi` & `bl_python_web-0.2.1/typings/connexion/json_schema.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/jsonifier.pyi` & `bl_python_web-0.2.1/typings/connexion/jsonifier.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/lifecycle.pyi` & `bl_python_web-0.2.1/typings/connexion/lifecycle.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/abstract.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/context.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/context.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/exceptions.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/lifespan.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/lifespan.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/main.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/main.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/request_validation.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/request_validation.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/response_validation.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/response_validation.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/routing.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/routing.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/security.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/server_error.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/server_error.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/middleware/swagger_ui.pyi` & `bl_python_web-0.2.1/typings/connexion/middleware/swagger_ui.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/mock.pyi` & `bl_python_web-0.2.1/typings/connexion/mock.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/operations/__init__.pyi` & `bl_python_web-0.2.1/typings/connexion/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/operations/abstract.pyi` & `bl_python_web-0.2.1/typings/connexion/operations/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/operations/openapi.pyi` & `bl_python_web-0.2.1/typings/connexion/operations/openapi.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/operations/swagger2.pyi` & `bl_python_web-0.2.1/typings/connexion/operations/swagger2.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/options.pyi` & `bl_python_web-0.2.1/typings/connexion/options.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/problem.pyi` & `bl_python_web-0.2.1/typings/connexion/problem.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/resolver.pyi` & `bl_python_web-0.2.1/typings/connexion/resolver.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/security.pyi` & `bl_python_web-0.2.1/typings/connexion/security.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/spec.pyi` & `bl_python_web-0.2.1/typings/connexion/spec.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/testing.pyi` & `bl_python_web-0.2.1/typings/connexion/testing.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/types.pyi` & `bl_python_web-0.2.1/typings/connexion/types.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/uri_parsing.pyi` & `bl_python_web-0.2.1/typings/connexion/uri_parsing.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/utils.pyi` & `bl_python_web-0.2.1/typings/connexion/utils.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/validators/__init__.pyi` & `bl_python_web-0.2.1/typings/connexion/validators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/validators/abstract.pyi` & `bl_python_web-0.2.1/typings/connexion/validators/abstract.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/validators/form_data.pyi` & `bl_python_web-0.2.1/typings/connexion/validators/form_data.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/validators/json.pyi` & `bl_python_web-0.2.1/typings/connexion/validators/json.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/connexion/validators/parameter.pyi` & `bl_python_web-0.2.1/typings/connexion/validators/parameter.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/flask_injector/__init__.pyi` & `bl_python_web-0.2.1/typings/flask_injector/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/flask_injector/tests.pyi` & `bl_python_web-0.2.1/typings/flask_injector/tests.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/flask_login/__init__.pyi` & `bl_python_web-0.2.1/typings/flask_login/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/flask_login/login_manager.pyi` & `bl_python_web-0.2.1/typings/flask_login/login_manager.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/flask_login/mixins.pyi` & `bl_python_web-0.2.1/typings/flask_login/mixins.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/flask_login/utils.pyi` & `bl_python_web-0.2.1/typings/flask_login/utils.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/json_logging/__init__.pyi` & `bl_python_web-0.2.1/typings/json_logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/json_logging/framework/connexion/__init__.pyi` & `bl_python_web-0.2.1/typings/json_logging/framework/connexion/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/json_logging/framework/fastapi/implementation.pyi` & `bl_python_web-0.2.1/typings/json_logging/framework/fastapi/implementation.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/json_logging/framework/flask/__init__.pyi` & `bl_python_web-0.2.1/typings/json_logging/framework/flask/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/json_logging/framework/quart/__init__.pyi` & `bl_python_web-0.2.1/typings/json_logging/framework/quart/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/json_logging/framework/sanic/__init__.pyi` & `bl_python_web-0.2.1/typings/json_logging/framework/sanic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/json_logging/framework_base.pyi` & `bl_python_web-0.2.1/typings/json_logging/framework_base.pyi`

 * *Files identical despite different names*

### Comparing `bl_python_web-0.2.0/typings/json_logging/util.pyi` & `bl_python_web-0.2.1/typings/json_logging/util.pyi`

 * *Files identical despite different names*

