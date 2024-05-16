# Comparing `tmp/prefect-client-2.18.3.tar.gz` & `tmp/prefect-client-2.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-client-2.18.3.tar", last modified: Thu May  2 22:50:01 2024, max compression
+gzip compressed data, was "prefect-client-2.19.0.tar", last modified: Mon May 13 20:33:58 2024, max compression
```

## Comparing `prefect-client-2.18.3.tar` & `prefect-client-2.19.0.tar`

### file list

```diff
@@ -1,348 +1,349 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.090017 prefect-client-2.18.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 22:49:59.000000 prefect-client-2.18.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-02 22:49:59.000000 prefect-client-2.18.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-02 22:50:01.090017 prefect-client-2.18.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-02 22:49:59.000000 prefect-client-2.18.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-02 22:49:59.000000 prefect-client-2.18.3/requirements-client.txt
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-02 22:49:59.000000 prefect-client-2.18.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-02 22:49:59.000000 prefect-client-2.18.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-02 22:50:01.090017 prefect-client-2.18.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-02 22:49:59.000000 prefect-client-2.18.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.050017 prefect-client-2.18.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.054017 prefect-client-2.18.3/src/prefect/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/.prefectignore
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.054017 prefect-client-2.18.3/src/prefect/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.054017 prefect-client-2.18.3/src/prefect/_internal/compatibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/compatibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/compatibility/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/compatibility/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.058017 prefect-client-2.18.3/src/prefect/_internal/concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    18201 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/cancellation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/concurrency/waiters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.058017 prefect-client-2.18.3/src/prefect/_internal/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.058017 prefect-client-2.18.3/src/prefect/_internal/pydantic/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/annotations/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.058017 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/config_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/field_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_construct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_dump_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_fields_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_validate_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/type_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/v1_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/v2_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pydantic/v2_validated_func.py
--rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/pytz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.062017 prefect-client-2.18.3/src/prefect/_internal/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/schemas/bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/schemas/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/schemas/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    32417 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_internal/schemas/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.062017 prefect-client-2.18.3/src/prefect/_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.062017 prefect-client-2.18.3/src/prefect/_vendor/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40983 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/datastructures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.062017 prefect-client-2.18.3/src/prefect/_vendor/fastapi/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/dependencies/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    31968 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/dependencies/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.066017 prefect-client-2.18.3/src/prefect/_vendor/fastapi/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/middleware/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/middleware/gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/middleware/httpsredirect.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/middleware/trustedhost.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/middleware/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.066017 prefect-client-2.18.3/src/prefect/_vendor/fastapi/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/openapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/openapi/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/openapi/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/openapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/param_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/params.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    57083 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.066017 prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/open_id_connect_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/staticfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/testclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/fastapi/websockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.070017 prefect-client-2.18.3/src/prefect/_vendor/starlette/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/convertors.py
--rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/formparsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.070017 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/httpsredirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/trustedhost.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/staticfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)    29902 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/testclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_vendor/starlette/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24597 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    27789 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/automations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.074017 prefect-client-2.18.3/src/prefect/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16311 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/blocks/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    43496 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/blocks/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/blocks/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/blocks/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    27247 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/blocks/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/blocks/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/blocks/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.074017 prefect-client-2.18.3/src/prefect/client/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   124402 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/orchestration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.074017 prefect-client-2.18.3/src/prefect/client/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/schemas/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/schemas/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    52389 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/schemas/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/schemas/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/schemas/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/schemas/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/client/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.074017 prefect-client-2.18.3/src/prefect/concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/concurrency/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/concurrency/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/concurrency/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/concurrency/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.074017 prefect-client-2.18.3/src/prefect/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deployments/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41656 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deployments/deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    44772 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deployments/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deployments/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.078017 prefect-client-2.18.3/src/prefect/deployments/steps/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deployments/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deployments/steps/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deployments/steps/pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deployments/steps/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.078017 prefect-client-2.18.3/src/prefect/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deprecated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deprecated/data_documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.078017 prefect-client-2.18.3/src/prefect/deprecated/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deprecated/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deprecated/packaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deprecated/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deprecated/packaging/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deprecated/packaging/orion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/deprecated/packaging/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    90406 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.078017 prefect-client-2.18.3/src/prefect/events/
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.078017 prefect-client-2.18.3/src/prefect/events/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/cli/automations.py
--rw-r--r--   0 runner    (1001) docker     (127)    20391 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/related.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.078017 prefect-client-2.18.3/src/prefect/events/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14171 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/schemas/automations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/schemas/deployment_triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9394 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/schemas/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/schemas/labelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/events/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    35260 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/filesystems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/flow_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)    71253 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/futures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.082017 prefect-client-2.18.3/src/prefect/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.082017 prefect-client-2.18.3/src/prefect/infrastructure/provisioners/
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/provisioners/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    41231 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/provisioners/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    47674 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/provisioners/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/infrastructure/provisioners/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.082017 prefect-client-2.18.3/src/prefect/input/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/input/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18697 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/input/run_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.082017 prefect-client-2.18.3/src/prefect/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/logging/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/logging/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/logging/highlighters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/logging/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/logging/logging.yml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/manifests.py
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/new_flow_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/new_task_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/profiles.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.082017 prefect-client-2.18.3/src/prefect/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/pydantic/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    25502 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.082017 prefect-client-2.18.3/src/prefect/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48115 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runner/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runner/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runner/submit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.086017 prefect-client-2.18.3/src/prefect/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runtime/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runtime/flow_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/runtime/task_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.046017 prefect-client-2.18.3/src/prefect/server/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.050017 prefect-client-2.18.3/src/prefect/server/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.050017 prefect-client-2.18.3/src/prefect/server/api/collections_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.086017 prefect-client-2.18.3/src/prefect/server/api/collections_data/views/
--rw-r--r--   0 runner    (1001) docker     (127)    80259 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.086017 prefect-client-2.18.3/src/prefect/server/api/static/
--rw-r--r--   0 runner    (1001) docker     (127)    73430 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/server/api/static/prefect-logo-mark-gradient.png
--rw-r--r--   0 runner    (1001) docker     (127)    74410 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.086017 prefect-client-2.18.3/src/prefect/software/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/software/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/software/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/software/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/software/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    21036 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/task_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/task_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    55077 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.086017 prefect-client-2.18.3/src/prefect/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.090017 prefect-client-2.18.3/src/prefect/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/asyncutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/callables.py
--rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    20180 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/dockerutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/importtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/names.py
--rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/processutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/render_swagger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.090017 prefect-client-2.18.3/src/prefect/utilities/schema_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/schema_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/schema_tools/hydration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/schema_tools/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/slugify.py
--rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/utilities/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.090017 prefect-client-2.18.3/src/prefect/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44977 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/workers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/workers/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/workers/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/workers/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-02 22:49:59.000000 prefect-client-2.18.3/src/prefect/workers/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:50:01.090017 prefect-client-2.18.3/src/prefect_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-02 22:50:00.000000 prefect-client-2.18.3/src/prefect_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-05-02 22:50:01.000000 prefect-client-2.18.3/src/prefect_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:50:00.000000 prefect-client-2.18.3/src/prefect_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 22:50:00.000000 prefect-client-2.18.3/src/prefect_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 22:50:00.000000 prefect-client-2.18.3/src/prefect_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86829 2024-05-02 22:49:59.000000 prefect-client-2.18.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.437620 prefect-client-2.19.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 20:33:54.000000 prefect-client-2.19.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 20:33:54.000000 prefect-client-2.19.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-13 20:33:58.437620 prefect-client-2.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-13 20:33:54.000000 prefect-client-2.19.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 20:33:54.000000 prefect-client-2.19.0/requirements-client.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-13 20:33:54.000000 prefect-client-2.19.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-13 20:33:54.000000 prefect-client-2.19.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-13 20:33:58.441620 prefect-client-2.19.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-13 20:33:54.000000 prefect-client-2.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.389620 prefect-client-2.19.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.397620 prefect-client-2.19.0/src/prefect/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/.prefectignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.397620 prefect-client-2.19.0/src/prefect/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.397620 prefect-client-2.19.0/src/prefect/_internal/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/compatibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/compatibility/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/compatibility/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.397620 prefect-client-2.19.0/src/prefect/_internal/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18277 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/concurrency/waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.401620 prefect-client-2.19.0/src/prefect/_internal/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.401620 prefect-client-2.19.0/src/prefect/_internal/pydantic/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/annotations/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.401620 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/config_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_construct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_dump_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_fields_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_validate_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/type_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/v1_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/v2_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pydantic/v2_validated_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/pytz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.405620 prefect-client-2.19.0/src/prefect/_internal/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/schemas/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/schemas/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/schemas/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32835 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_internal/schemas/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.405620 prefect-client-2.19.0/src/prefect/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.405620 prefect-client-2.19.0/src/prefect/_vendor/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40983 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/datastructures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.409620 prefect-client-2.19.0/src/prefect/_vendor/fastapi/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/dependencies/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31968 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/dependencies/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.409620 prefect-client-2.19.0/src/prefect/_vendor/fastapi/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/middleware/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/middleware/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/middleware/httpsredirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/middleware/trustedhost.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/middleware/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.409620 prefect-client-2.19.0/src/prefect/_vendor/fastapi/openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/openapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/openapi/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/openapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/openapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/param_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57083 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.409620 prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/open_id_connect_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/staticfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/testclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/fastapi/websockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.413620 prefect-client-2.19.0/src/prefect/_vendor/starlette/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/convertors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/formparsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.417620 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/httpsredirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/trustedhost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/staticfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29899 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/testclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_vendor/starlette/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24597 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27789 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.417620 prefect-client-2.19.0/src/prefect/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16311 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/blocks/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43496 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/blocks/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/blocks/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/blocks/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27211 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/blocks/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/blocks/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/blocks/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.417620 prefect-client-2.19.0/src/prefect/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139211 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/orchestration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.421620 prefect-client-2.19.0/src/prefect/client/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27957 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/schemas/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/schemas/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53031 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/schemas/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15325 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/schemas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/schemas/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/schemas/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/client/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.421620 prefect-client-2.19.0/src/prefect/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/concurrency/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/concurrency/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/concurrency/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/concurrency/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18189 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.421620 prefect-client-2.19.0/src/prefect/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deployments/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41656 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deployments/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44772 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deployments/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deployments/schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.421620 prefect-client-2.19.0/src/prefect/deployments/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deployments/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deployments/steps/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deployments/steps/pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deployments/steps/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.421620 prefect-client-2.19.0/src/prefect/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deprecated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deprecated/data_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.425620 prefect-client-2.19.0/src/prefect/deprecated/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deprecated/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deprecated/packaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deprecated/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deprecated/packaging/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deprecated/packaging/orion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/deprecated/packaging/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90418 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.425620 prefect-client-2.19.0/src/prefect/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.425620 prefect-client-2.19.0/src/prefect/events/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/cli/automations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/related.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.425620 prefect-client-2.19.0/src/prefect/events/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14171 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/schemas/automations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/schemas/deployment_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9394 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/schemas/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/schemas/labelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/events/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35260 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/flow_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73247 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/futures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.425620 prefect-client-2.19.0/src/prefect/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.429620 prefect-client-2.19.0/src/prefect/infrastructure/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/provisioners/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41231 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/provisioners/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47674 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/provisioners/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/infrastructure/provisioners/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.429620 prefect-client-2.19.0/src/prefect/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/input/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18697 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/input/run_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.429620 prefect-client-2.19.0/src/prefect/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/logging/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/logging/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/logging/highlighters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/logging/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/logging/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/manifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/new_flow_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/new_task_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/profiles.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.429620 prefect-client-2.19.0/src/prefect/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/pydantic/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25502 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.429620 prefect-client-2.19.0/src/prefect/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44838 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runner/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runner/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runner/submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.433620 prefect-client-2.19.0/src/prefect/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runtime/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runtime/flow_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/runtime/task_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.389620 prefect-client-2.19.0/src/prefect/server/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.389620 prefect-client-2.19.0/src/prefect/server/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.389620 prefect-client-2.19.0/src/prefect/server/api/collections_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.433620 prefect-client-2.19.0/src/prefect/server/api/collections_data/views/
+-rw-r--r--   0 runner    (1001) docker     (127)    80259 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.433620 prefect-client-2.19.0/src/prefect/server/api/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    73430 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/server/api/static/prefect-logo-mark-gradient.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74705 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.433620 prefect-client-2.19.0/src/prefect/software/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/software/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/software/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/software/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/software/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21036 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/task_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/task_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55567 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.433620 prefect-client-2.19.0/src/prefect/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.437620 prefect-client-2.19.0/src/prefect/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/asyncutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/callables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20180 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/dockerutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25669 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/importtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/processutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/render_swagger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.437620 prefect-client-2.19.0/src/prefect/utilities/schema_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/schema_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/schema_tools/hydration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/schema_tools/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/slugify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/utilities/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.437620 prefect-client-2.19.0/src/prefect/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45125 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/workers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/workers/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/workers/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/workers/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-13 20:33:54.000000 prefect-client-2.19.0/src/prefect/workers/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:58.437620 prefect-client-2.19.0/src/prefect_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-13 20:33:58.000000 prefect-client-2.19.0/src/prefect_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-13 20:33:58.000000 prefect-client-2.19.0/src/prefect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:33:58.000000 prefect-client-2.19.0/src/prefect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 20:33:58.000000 prefect-client-2.19.0/src/prefect_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 20:33:58.000000 prefect-client-2.19.0/src/prefect_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86829 2024-05-13 20:33:54.000000 prefect-client-2.19.0/versioneer.py
```

### Comparing `prefect-client-2.18.3/LICENSE` & `prefect-client-2.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/MANIFEST.in` & `prefect-client-2.19.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/PKG-INFO` & `prefect-client-2.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-client
-Version: 2.18.3
+Version: 2.19.0
 Summary: Workflow orchestration and management.
 Home-page: https://www.prefect.io
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/PrefectHQ/prefect/blob/main/RELEASE-NOTES.md
 Project-URL: Documentation, https://docs.prefect.io
```

### Comparing `prefect-client-2.18.3/README.md` & `prefect-client-2.19.0/README.md`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/requirements-client.txt` & `prefect-client-2.19.0/requirements-client.txt`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/requirements-dev.txt` & `prefect-client-2.19.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/setup.cfg` & `prefect-client-2.19.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/setup.py` & `prefect-client-2.19.0/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/__init__.py` & `prefect-client-2.19.0/src/prefect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,33 +21,20 @@
 __ui_static_subpath__ = __module_path__ / "server" / "ui_build"
 
 # The absolute path to the built UI within the Python module
 __ui_static_path__ = __module_path__ / "server" / "ui"
 
 del _version, pathlib
 
-if sys.version_info < (3, 8):
-    warnings.warn(
-        (
-            "Prefect dropped support for Python 3.7 when it reached end-of-life"
-            " . To use new versions of Prefect, you will need"
-            " to upgrade to Python 3.8+. See https://devguide.python.org/versions/ for "
-            " more details."
-        ),
-        FutureWarning,
-        stacklevel=2,
-    )
-
 
 # Import user-facing API
-from prefect.runner import Runner, serve
 from prefect.deployments import deploy
 from prefect.states import State
 from prefect.logging import get_run_logger
-from prefect.flows import flow, Flow
+from prefect.flows import flow, Flow, serve
 from prefect.tasks import task, Task
 from prefect.context import tags
 from prefect.manifests import Manifest
 from prefect.utilities.annotations import unmapped, allow_failure
 from prefect.results import BaseResult
 from prefect.engine import pause_flow_run, resume_flow_run, suspend_flow_run
 from prefect.client.orchestration import get_client, PrefectClient
@@ -155,14 +142,13 @@
     "get_run_logger",
     "Manifest",
     "State",
     "tags",
     "task",
     "Task",
     "unmapped",
-    "Runner",
     "serve",
     "deploy",
     "pause_flow_run",
     "resume_flow_run",
     "suspend_flow_run",
 ]
```

### Comparing `prefect-client-2.18.3/src/prefect/_internal/_logging.py` & `prefect-client-2.19.0/src/prefect/_internal/_logging.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/compatibility/deprecated.py` & `prefect-client-2.19.0/src/prefect/_internal/compatibility/deprecated.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/compatibility/experimental.py` & `prefect-client-2.19.0/src/prefect/_internal/compatibility/experimental.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/__init__.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/api.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/api.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/calls.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/calls.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/cancellation.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/cancellation.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,12 +577,14 @@
 
 def _send_exception_to_thread(thread: threading.Thread, exc_type: Type[BaseException]):
     """
     Raise an exception in a thread.
 
     This will not interrupt long-running system calls like `sleep` or `wait`.
     """
+    if not thread.ident:
+        raise ValueError("Thread is not started.")
     ret = ctypes.pythonapi.PyThreadState_SetAsyncExc(
         ctypes.c_long(thread.ident), ctypes.py_object(exc_type)
     )
     if ret == 0:
         raise ValueError("Thread not found.")
```

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/event_loop.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/event_loop.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/inspection.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/inspection.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/primitives.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/primitives.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/services.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/services.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/threads.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/threads.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/concurrency/waiters.py` & `prefect-client-2.19.0/src/prefect/_internal/concurrency/waiters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/__init__.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/_base_model.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/_base_model.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/_compat.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/_compat.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/_flags.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/_flags.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/annotations/pendulum.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/annotations/pendulum.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/config_dict.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/config_dict.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/field_validator.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/field_validator.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_construct.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_construct.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_copy.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_copy.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_dump.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_dump.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_dump_json.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_dump_json.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_fields.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_fields.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_fields_set.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_fields_set.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_json_schema.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_json_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_rebuild.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_rebuild.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_validate.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_validate.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_validate_json.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_validate_json.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/model_validator.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/model_validator.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/utilities/type_adapter.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/utilities/type_adapter.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/v1_schema.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/v1_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/v2_schema.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/v2_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pydantic/v2_validated_func.py` & `prefect-client-2.19.0/src/prefect/_internal/pydantic/v2_validated_func.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/pytz.py` & `prefect-client-2.19.0/src/prefect/_internal/pytz.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/schemas/bases.py` & `prefect-client-2.19.0/src/prefect/_internal/schemas/bases.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/schemas/fields.py` & `prefect-client-2.19.0/src/prefect/_internal/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/schemas/serializers.py` & `prefect-client-2.19.0/src/prefect/_internal/schemas/serializers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_internal/schemas/validators.py` & `prefect-client-2.19.0/src/prefect/_internal/schemas/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,18 @@
 
 def validate_values_conform_to_schema(
     values: dict, schema: dict, ignore_required: bool = False
 ):
     """
     Validate that the provided values conform to the provided json schema.
 
+    TODO: This schema validation is outdated. The latest version is
+    prefect.utilities.schema_tools.validate, which handles fixes to Pydantic v1
+    schemas for null values and tuples.
+
     Args:
         values: The values to validate.
         schema: The schema to validate against.
         ignore_required: Whether to ignore the required fields in the schema. Should be
             used when a partial set of values is acceptable.
 
     Raises:
@@ -318,14 +322,20 @@
                 active=values["is_schedule_active"],
             )
         ]
 
     return values
 
 
+def validate_schedule_max_scheduled_runs(v: Optional[int], limit: int) -> Optional[int]:
+    if v is not None and v > limit:
+        raise ValueError(f"`max_scheduled_runs` must be less than or equal to {limit}.")
+    return v
+
+
 def remove_old_deployment_fields(values: dict) -> dict:
     # 2.7.7 removed worker_pool_queue_id in lieu of worker_pool_name and
     # worker_pool_queue_name. Those fields were later renamed to work_pool_name
     # and work_queue_name. This validator removes old fields provided
     # by older clients to avoid 422 errors.
     values_copy = copy(values)
     worker_pool_queue_id = values_copy.pop("worker_pool_queue_id", None)
```

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/__init__.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/applications.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/applications.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/concurrency.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/concurrency.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/datastructures.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/dependencies/models.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/dependencies/models.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/dependencies/utils.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/encoders.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/encoders.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/exception_handlers.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/exceptions.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/openapi/docs.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/openapi/models.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/openapi/models.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/openapi/utils.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/param_functions.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/param_functions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/params.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/params.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/responses.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/responses.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/routing.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/routing.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/__init__.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/api_key.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/api_key.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/http.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/http.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/oauth2.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/security/open_id_connect_url.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/fastapi/utils.py` & `prefect-client-2.19.0/src/prefect/_vendor/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/_compat.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/_compat.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/_exception_handler.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/_utils.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/_utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/applications.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/applications.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/authentication.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/authentication.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/background.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/background.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/concurrency.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/concurrency.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/config.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/config.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/convertors.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/convertors.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/datastructures.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/datastructures.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/endpoints.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/endpoints.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/exceptions.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/formparsers.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/formparsers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/__init__.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/authentication.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/base.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/cors.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/errors.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/exceptions.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/gzip.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/gzip.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/httpsredirect.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/httpsredirect.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/sessions.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/sessions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/trustedhost.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/trustedhost.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/middleware/wsgi.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/requests.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/requests.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/responses.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/responses.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/routing.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/routing.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/schemas.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/schemas.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/staticfiles.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/staticfiles.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/status.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/status.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/templating.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/templating.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/testclient.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/testclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,15 +457,15 @@
         follow_redirects: typing.Optional[bool] = None,
         allow_redirects: typing.Optional[bool] = None,
         timeout: typing.Union[
             httpx._types.TimeoutTypes, httpx._client.UseClientDefault
         ] = httpx._client.USE_CLIENT_DEFAULT,
         extensions: typing.Optional[typing.Dict[str, typing.Any]] = None,
     ) -> httpx.Response:
-        url = self.base_url.join(url)
+        url = self._merge_url(url)
         redirect = self._choose_redirect_arg(follow_redirects, allow_redirects)
         return super().request(
             method,
             url,
             content=content,
             data=data,
             files=files,
```

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/types.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/types.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_vendor/starlette/websockets.py` & `prefect-client-2.19.0/src/prefect/_vendor/starlette/websockets.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/_version.py` & `prefect-client-2.19.0/src/prefect/_version.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/agent.py` & `prefect-client-2.19.0/src/prefect/agent.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/artifacts.py` & `prefect-client-2.19.0/src/prefect/artifacts.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/automations.py` & `prefect-client-2.19.0/src/prefect/automations.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/blocks/abstract.py` & `prefect-client-2.19.0/src/prefect/blocks/abstract.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/blocks/core.py` & `prefect-client-2.19.0/src/prefect/blocks/core.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/blocks/fields.py` & `prefect-client-2.19.0/src/prefect/blocks/fields.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/blocks/kubernetes.py` & `prefect-client-2.19.0/src/prefect/blocks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/blocks/notifications.py` & `prefect-client-2.19.0/src/prefect/blocks/notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     custom_details: Optional[Dict[str, str]] = Field(
         default=None,
         description="Additional details to include as part of the payload.",
         examples=['{"disk_space_left": "145GB"}'],
     )
 
     def block_initialization(self) -> None:
-        from apprise.plugins.NotifyPagerDuty import NotifyPagerDuty
+        from apprise.plugins.pagerduty import NotifyPagerDuty
 
         url = SecretStr(
             NotifyPagerDuty(
                 apikey=self.api_key.get_secret_value(),
                 integrationkey=self.integration_key.get_secret_value(),
                 source=self.source,
                 component=self.component,
@@ -299,15 +299,15 @@
         default=...,
         description="A list of valid Twilio phone number(s) to send the message to.",
         # not wrapped in brackets because of the way UI displays examples; in code should be ["18004242424"]
         examples=["18004242424"],
     )
 
     def block_initialization(self) -> None:
-        from apprise.plugins.NotifyTwilio import NotifyTwilio
+        from apprise.plugins.twilio import NotifyTwilio
 
         url = SecretStr(
             NotifyTwilio(
                 account_sid=self.account_sid,
                 auth_token=self.auth_token.get_secret_value(),
                 source=self.from_phone_number,
                 targets=self.to_phone_numbers,
@@ -397,15 +397,15 @@
     details: Optional[Dict[str, str]] = Field(
         default=None,
         description="Additional details composed of key/values pairs.",
         examples=['{"key1": "value1", "key2": "value2"}'],
     )
 
     def block_initialization(self) -> None:
-        from apprise.plugins.NotifyOpsgenie import NotifyOpsgenie
+        from apprise.plugins.opsgenie import NotifyOpsgenie
 
         targets = []
         if self.target_user:
             [targets.append(f"@{x}") for x in self.target_user]
         if self.target_team:
             [targets.append(f"#{x}") for x in self.target_team]
         if self.target_schedule:
@@ -485,15 +485,15 @@
 
     port: int = Field(
         default=8065,
         description="The port of your Mattermost server.",
     )
 
     def block_initialization(self) -> None:
-        from apprise.plugins.NotifyMattermost import NotifyMattermost
+        from apprise.plugins.mattermost import NotifyMattermost
 
         url = SecretStr(
             NotifyMattermost(
                 token=self.token.get_secret_value(),
                 fullpath=self.path,
                 host=self.hostname,
                 botname=self.botname,
@@ -578,15 +578,15 @@
             "Over-ride the default discord avatar icon URL. By default this is not set"
             " and Apprise chooses the URL dynamically based on the type of message"
             " (info, success, warning, or error)."
         ),
     )
 
     def block_initialization(self) -> None:
-        from apprise.plugins.NotifyDiscord import NotifyDiscord
+        from apprise.plugins.discord import NotifyDiscord
 
         url = SecretStr(
             NotifyDiscord(
                 webhook_id=self.webhook_id.get_secret_value(),
                 webhook_token=self.webhook_token.get_secret_value(),
                 botname=self.botname,
                 tts=self.tts,
@@ -769,15 +769,15 @@
         default=...,
         title="Recipient emails",
         description="Email ids of all recipients.",
         examples=['"recipient1@gmail.com"'],
     )
 
     def block_initialization(self) -> None:
-        from apprise.plugins.NotifySendGrid import NotifySendGrid
+        from apprise.plugins.sendgrid import NotifySendGrid
 
         url = SecretStr(
             NotifySendGrid(
                 apikey=self.api_key.get_secret_value(),
                 from_email=self.sender_email,
                 targets=self.to_emails,
             ).url()
```

### Comparing `prefect-client-2.18.3/src/prefect/blocks/system.py` & `prefect-client-2.19.0/src/prefect/blocks/system.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/blocks/webhook.py` & `prefect-client-2.19.0/src/prefect/blocks/webhook.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/client/base.py` & `prefect-client-2.19.0/src/prefect/client/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import sys
 import threading
+import time
 import uuid
 from collections import defaultdict
 from contextlib import asynccontextmanager
 from datetime import datetime, timezone
 from typing import (
     Any,
     AsyncGenerator,
@@ -21,14 +22,15 @@
 )
 
 import anyio
 import httpx
 from asgi_lifespan import LifespanManager
 from httpx import HTTPStatusError, Request, Response
 from prefect._vendor.starlette import status
+from prefect._vendor.starlette.testclient import TestClient
 from typing_extensions import Self
 
 import prefect
 from prefect.client import constants
 from prefect.client.schemas.objects import CsrfToken
 from prefect.exceptions import PrefectHTTPStatusError
 from prefect.logging import get_logger
@@ -178,15 +180,15 @@
         everything else about the original Response instance intact.
         """
         new_response = copy.copy(response)
         new_response.__class__ = cls
         return new_response
 
 
-class PrefectHttpxClient(httpx.AsyncClient):
+class PrefectHttpxAsyncClient(httpx.AsyncClient):
     """
     A Prefect wrapper for the async httpx client with support for retry-after headers
     for the provided status codes (typically 429, 502 and 503).
 
     Additionally, this client will always call `raise_for_status` on responses.
 
     For more details on rate limit headers, see:
@@ -390,7 +392,248 @@
 
             token: CsrfToken = CsrfToken.parse_obj(token_response.json())
             self.csrf_token = token.token
             self.csrf_token_expiration = token.expiration
 
         request.headers["Prefect-Csrf-Token"] = self.csrf_token
         request.headers["Prefect-Csrf-Client"] = str(self.csrf_client_id)
+
+
+class PrefectHttpxSyncClient(httpx.Client):
+    """
+    A Prefect wrapper for the async httpx client with support for retry-after headers
+    for the provided status codes (typically 429, 502 and 503).
+
+    Additionally, this client will always call `raise_for_status` on responses.
+
+    For more details on rate limit headers, see:
+    [Configuring Cloudflare Rate Limiting](https://support.cloudflare.com/hc/en-us/articles/115001635128-Configuring-Rate-Limiting-from-UI)
+    """
+
+    def __init__(
+        self,
+        *args,
+        enable_csrf_support: bool = False,
+        raise_on_all_errors: bool = True,
+        **kwargs,
+    ):
+        self.enable_csrf_support: bool = enable_csrf_support
+        self.csrf_token: Optional[str] = None
+        self.csrf_token_expiration: Optional[datetime] = None
+        self.csrf_client_id: uuid.UUID = uuid.uuid4()
+        self.raise_on_all_errors: bool = raise_on_all_errors
+
+        super().__init__(*args, **kwargs)
+
+        user_agent = (
+            f"prefect/{prefect.__version__} (API {constants.SERVER_API_VERSION})"
+        )
+        self.headers["User-Agent"] = user_agent
+
+    def _send_with_retry(
+        self,
+        request: Request,
+        send: Callable[[Request], Response],
+        send_args: Tuple,
+        send_kwargs: Dict,
+        retry_codes: Set[int] = set(),
+        retry_exceptions: Tuple[Exception, ...] = tuple(),
+    ):
+        """
+        Send a request and retry it if it fails.
+
+        Sends the provided request and retries it up to PREFECT_CLIENT_MAX_RETRIES times
+        if the request either raises an exception listed in `retry_exceptions` or
+        receives a response with a status code listed in `retry_codes`.
+
+        Retries will be delayed based on either the retry header (preferred) or
+        exponential backoff if a retry header is not provided.
+        """
+        try_count = 0
+        response = None
+
+        is_change_request = request.method.lower() in {"post", "put", "patch", "delete"}
+
+        if self.enable_csrf_support and is_change_request:
+            self._add_csrf_headers(request=request)
+
+        while try_count <= PREFECT_CLIENT_MAX_RETRIES.value():
+            try_count += 1
+            retry_seconds = None
+            exc_info = None
+
+            try:
+                response = send(request, *send_args, **send_kwargs)
+            except retry_exceptions:  # type: ignore
+                if try_count > PREFECT_CLIENT_MAX_RETRIES.value():
+                    raise
+                # Otherwise, we will ignore this error but capture the info for logging
+                exc_info = sys.exc_info()
+            else:
+                # We got a response; check if it's a CSRF error, otherwise
+                # return immediately if it is not retryable
+                if (
+                    response.status_code == status.HTTP_403_FORBIDDEN
+                    and "Invalid CSRF token" in response.text
+                ):
+                    # We got a CSRF error, clear the token and try again
+                    self.csrf_token = None
+                    self._add_csrf_headers(request)
+                elif response.status_code not in retry_codes:
+                    return response
+
+                if "Retry-After" in response.headers:
+                    retry_seconds = float(response.headers["Retry-After"])
+
+            # Use an exponential back-off if not set in a header
+            if retry_seconds is None:
+                retry_seconds = 2**try_count
+
+            # Add jitter
+            jitter_factor = PREFECT_CLIENT_RETRY_JITTER_FACTOR.value()
+            if retry_seconds > 0 and jitter_factor > 0:
+                if response is not None and "Retry-After" in response.headers:
+                    # Always wait for _at least_ retry seconds if requested by the API
+                    retry_seconds = bounded_poisson_interval(
+                        retry_seconds, retry_seconds * (1 + jitter_factor)
+                    )
+                else:
+                    # Otherwise, use a symmetrical jitter
+                    retry_seconds = clamped_poisson_interval(
+                        retry_seconds, jitter_factor
+                    )
+
+            logger.debug(
+                (
+                    "Encountered retryable exception during request. "
+                    if exc_info
+                    else (
+                        "Received response with retryable status code"
+                        f" {response.status_code}. "
+                    )
+                )
+                + f"Another attempt will be made in {retry_seconds}s. "
+                "This is attempt"
+                f" {try_count}/{PREFECT_CLIENT_MAX_RETRIES.value() + 1}.",
+                exc_info=exc_info,
+            )
+            time.sleep(retry_seconds)
+
+        assert (
+            response is not None
+        ), "Retry handling ended without response or exception"
+
+        # We ran out of retries, return the failed response
+        return response
+
+    def send(self, request: Request, *args, **kwargs) -> Response:
+        """
+        Send a request with automatic retry behavior for the following status codes:
+
+        - 403 Forbidden, if the request failed due to CSRF protection
+        - 408 Request Timeout
+        - 429 CloudFlare-style rate limiting
+        - 502 Bad Gateway
+        - 503 Service unavailable
+        - Any additional status codes provided in `PREFECT_CLIENT_RETRY_EXTRA_CODES`
+        """
+
+        super_send = super().send
+        response = self._send_with_retry(
+            request=request,
+            send=super_send,
+            send_args=args,
+            send_kwargs=kwargs,
+            retry_codes={
+                status.HTTP_429_TOO_MANY_REQUESTS,
+                status.HTTP_503_SERVICE_UNAVAILABLE,
+                status.HTTP_502_BAD_GATEWAY,
+                status.HTTP_408_REQUEST_TIMEOUT,
+                *PREFECT_CLIENT_RETRY_EXTRA_CODES.value(),
+            },
+            retry_exceptions=(
+                httpx.ReadTimeout,
+                httpx.PoolTimeout,
+                httpx.ConnectTimeout,
+                # `ConnectionResetError` when reading socket raises as a `ReadError`
+                httpx.ReadError,
+                # Sockets can be closed during writes resulting in a `WriteError`
+                httpx.WriteError,
+                # Uvicorn bug, see https://github.com/PrefectHQ/prefect/issues/7512
+                httpx.RemoteProtocolError,
+                # HTTP2 bug, see https://github.com/PrefectHQ/prefect/issues/7442
+                httpx.LocalProtocolError,
+            ),
+        )
+
+        # Convert to a Prefect response to add nicer errors messages
+        response = PrefectResponse.from_httpx_response(response)
+
+        if self.raise_on_all_errors:
+            response.raise_for_status()
+
+        return response
+
+    def _add_csrf_headers(self, request: Request):
+        now = datetime.now(timezone.utc)
+
+        if not self.enable_csrf_support:
+            return
+
+        if not self.csrf_token or (
+            self.csrf_token_expiration and now > self.csrf_token_expiration
+        ):
+            token_request = self.build_request(
+                "GET", f"/csrf-token?client={self.csrf_client_id}"
+            )
+
+            try:
+                token_response = self.send(token_request)
+            except PrefectHTTPStatusError as exc:
+                old_server = exc.response.status_code == status.HTTP_404_NOT_FOUND
+                unconfigured_server = (
+                    exc.response.status_code == status.HTTP_422_UNPROCESSABLE_ENTITY
+                    and "CSRF protection is disabled." in exc.response.text
+                )
+
+                if old_server or unconfigured_server:
+                    # The token endpoint is either unavailable, suggesting an
+                    # older server, or CSRF protection is disabled. In either
+                    # case we should disable CSRF support.
+                    self.enable_csrf_support = False
+                    return
+
+                raise
+
+            token: CsrfToken = CsrfToken.parse_obj(token_response.json())
+            self.csrf_token = token.token
+            self.csrf_token_expiration = token.expiration
+
+        request.headers["Prefect-Csrf-Token"] = self.csrf_token
+        request.headers["Prefect-Csrf-Client"] = str(self.csrf_client_id)
+
+
+class PrefectHttpxSyncEphemeralClient(TestClient, PrefectHttpxSyncClient):
+    """
+    This client is a synchronous httpx client that can be used to talk directly
+    to an ASGI app, such as an ephemeral Prefect API.
+
+    It is a subclass of both Starlette's `TestClient` and Prefect's
+    `PrefectHttpxSyncClient`, so it combines the synchronous testing
+    capabilities of `TestClient` with the Prefect-specific behaviors of
+    `PrefectHttpxSyncClient`.
+    """
+
+    def __init__(
+        self,
+        *args,
+        # override TestClient default
+        raise_server_exceptions=False,
+        **kwargs,
+    ):
+        super().__init__(
+            *args,
+            raise_server_exceptions=raise_server_exceptions,
+            **kwargs,
+        )
+
+    pass
```

### Comparing `prefect-client-2.18.3/src/prefect/client/cloud.py` & `prefect-client-2.19.0/src/prefect/client/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 else:
     import pydantic
 
 from prefect._vendor.starlette import status
 
 import prefect.context
 import prefect.settings
-from prefect.client.base import PrefectHttpxClient
+from prefect.client.base import PrefectHttpxAsyncClient
 from prefect.client.schemas import Workspace
 from prefect.exceptions import PrefectException
 from prefect.settings import (
     PREFECT_API_KEY,
     PREFECT_CLOUD_API_URL,
     PREFECT_UNIT_TEST_MODE,
 )
@@ -68,15 +68,17 @@
         httpx_settings = httpx_settings or dict()
         httpx_settings.setdefault("headers", dict())
         httpx_settings["headers"].setdefault("Authorization", f"Bearer {api_key}")
 
         httpx_settings.setdefault("base_url", host)
         if not PREFECT_UNIT_TEST_MODE.value():
             httpx_settings.setdefault("follow_redirects", True)
-        self._client = PrefectHttpxClient(**httpx_settings, enable_csrf_support=False)
+        self._client = PrefectHttpxAsyncClient(
+            **httpx_settings, enable_csrf_support=False
+        )
 
     async def api_healthcheck(self):
         """
         Attempts to connect to the Cloud API and raises the encountered exception if not
         successful.
 
         If successful, returns `None`.
```

### Comparing `prefect-client-2.18.3/src/prefect/client/collections.py` & `prefect-client-2.19.0/src/prefect/client/collections.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/client/orchestration.py` & `prefect-client-2.19.0/src/prefect/client/orchestration.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 from prefect.client.schemas import sorting
 from prefect.events import filters
 from prefect.settings import (
     PREFECT_API_SERVICES_TRIGGERS_ENABLED,
     PREFECT_EXPERIMENTAL_EVENTS,
 )
-from prefect.utilities.asyncutils import run_sync
 
 if HAS_PYDANTIC_V2:
     import pydantic.v1 as pydantic
 else:
     import pydantic
 
 from asgi_lifespan import LifespanManager
@@ -117,14 +116,15 @@
     WorkPool,
     WorkQueue,
     WorkQueueStatusDetail,
 )
 from prefect.client.schemas.responses import (
     DeploymentResponse,
     FlowRunResponse,
+    GlobalConcurrencyLimitResponse,
     WorkerFlowRunResponse,
 )
 from prefect.client.schemas.schedules import SCHEDULE_TYPES
 from prefect.client.schemas.sorting import (
     ArtifactCollectionSort,
     ArtifactSort,
     DeploymentSort,
@@ -150,15 +150,21 @@
 )
 from prefect.utilities.collections import AutoEnum
 
 if TYPE_CHECKING:
     from prefect.flows import Flow as FlowObject
     from prefect.tasks import Task as TaskObject
 
-from prefect.client.base import ASGIApp, PrefectHttpxClient, app_lifespan_context
+from prefect.client.base import (
+    ASGIApp,
+    PrefectHttpxAsyncClient,
+    PrefectHttpxSyncClient,
+    PrefectHttpxSyncEphemeralClient,
+    app_lifespan_context,
+)
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
 class ServerType(AutoEnum):
     EPHEMERAL = AutoEnum.auto()
@@ -170,15 +176,15 @@
             return True
 
         return PREFECT_EXPERIMENTAL_EVENTS and PREFECT_API_SERVICES_TRIGGERS_ENABLED
 
 
 def get_client(
     httpx_settings: Optional[Dict[str, Any]] = None, sync_client: bool = False
-) -> "PrefectClient":
+) -> Union["PrefectClient", "SyncPrefectClient"]:
     """
     Retrieve a HTTP client for communicating with the Prefect REST API.
 
     The client must be context managed; for example:
 
     ```python
     async with get_client() as client:
@@ -357,15 +363,15 @@
             httpx_settings.setdefault("follow_redirects", True)
 
         enable_csrf_support = (
             self.server_type != ServerType.CLOUD
             and PREFECT_CLIENT_CSRF_SUPPORT_ENABLED.value()
         )
 
-        self._client = PrefectHttpxClient(
+        self._client = PrefectHttpxAsyncClient(
             **httpx_settings, enable_csrf_support=enable_csrf_support
         )
         self._loop = None
 
         # See https://www.python-httpx.org/advanced/#custom-transports
         #
         # If we're using an HTTP/S client (not the ephemeral client), adjust the
@@ -1948,15 +1954,15 @@
             schedule_id: the deployment schedule ID of interest
             active: whether or not the schedule should be active
             schedule: the cron, rrule, or interval schedule this deployment schedule should use
         """
         kwargs = {}
         if active is not None:
             kwargs["active"] = active
-        elif schedule is not None:
+        if schedule is not None:
             kwargs["schedule"] = schedule
 
         deployment_schedule_update = DeploymentScheduleUpdate(**kwargs)
         json = deployment_schedule_update.dict(json_compatible=True, exclude_unset=True)
 
         try:
             await self._client.patch(
@@ -3050,35 +3056,37 @@
             if e.response.status_code == status.HTTP_404_NOT_FOUND:
                 raise prefect.exceptions.ObjectNotFound(http_exc=e) from e
             else:
                 raise
 
     async def read_global_concurrency_limit_by_name(
         self, name: str
-    ) -> Dict[str, object]:
+    ) -> GlobalConcurrencyLimitResponse:
         try:
             response = await self._client.get(f"/v2/concurrency_limits/{name}")
-            return response.json()
+            return GlobalConcurrencyLimitResponse.parse_obj(response.json())
         except httpx.HTTPStatusError as e:
             if e.response.status_code == status.HTTP_404_NOT_FOUND:
                 raise prefect.exceptions.ObjectNotFound(http_exc=e) from e
             else:
                 raise
 
     async def read_global_concurrency_limits(
         self, limit: int = 10, offset: int = 0
-    ) -> List[Dict[str, object]]:
+    ) -> List[GlobalConcurrencyLimitResponse]:
         response = await self._client.post(
             "/v2/concurrency_limits/filter",
             json={
                 "limit": limit,
                 "offset": offset,
             },
         )
-        return response.json()
+        return pydantic.parse_obj_as(
+            List[GlobalConcurrencyLimitResponse], response.json()
+        )
 
     async def create_flow_run_input(
         self, flow_run_id: UUID, key: str, value: str, sender: Optional[str] = None
     ):
         """
         Creates a flow run input.
 
@@ -3361,15 +3369,15 @@
     A synchronous client for interacting with the [Prefect REST API](/api-ref/rest-api/).
 
     Args:
         api: the REST API URL or FastAPI application to connect to
         api_key: An optional API key for authentication.
         api_version: The API version this client is compatible with.
         httpx_settings: An optional dictionary of settings to pass to the underlying
-            `httpx.AsyncClient`
+            `httpx.Client`
 
     Examples:
 
         Say hello to a Prefect REST API
 
         <div class="terminal">
         ```
@@ -3382,46 +3390,424 @@
         </div>
     """
 
     def __init__(
         self,
         api: Union[str, ASGIApp],
         *,
-        api_key: Optional[str] = None,
-        api_version: Optional[str] = None,
+        api_key: str = None,
+        api_version: str = None,
         httpx_settings: Optional[Dict[str, Any]] = None,
     ) -> None:
-        self._prefect_client = PrefectClient(
-            api=api,
-            api_key=api_key,
-            api_version=api_version,
-            httpx_settings=httpx_settings,
+        httpx_settings = httpx_settings.copy() if httpx_settings else {}
+        httpx_settings.setdefault("headers", {})
+
+        if PREFECT_API_TLS_INSECURE_SKIP_VERIFY:
+            httpx_settings.setdefault("verify", False)
+        else:
+            cert_file = PREFECT_API_SSL_CERT_FILE.value()
+            if not cert_file:
+                cert_file = certifi.where()
+            httpx_settings.setdefault("verify", cert_file)
+
+        if api_version is None:
+            api_version = SERVER_API_VERSION
+        httpx_settings["headers"].setdefault("X-PREFECT-API-VERSION", api_version)
+        if api_key:
+            httpx_settings["headers"].setdefault("Authorization", f"Bearer {api_key}")
+
+        # Context management
+        self._ephemeral_app: Optional[ASGIApp] = None
+        self.manage_lifespan = True
+        self.server_type: ServerType
+
+        self._closed = False
+        self._started = False
+
+        # Connect to an external application
+        if isinstance(api, str):
+            if httpx_settings.get("app"):
+                raise ValueError(
+                    "Invalid httpx settings: `app` cannot be set when providing an "
+                    "api url. `app` is only for use with ephemeral instances. Provide "
+                    "it as the `api` parameter instead."
+                )
+            httpx_settings.setdefault("base_url", api)
+
+            # See https://www.python-httpx.org/advanced/#pool-limit-configuration
+            httpx_settings.setdefault(
+                "limits",
+                httpx.Limits(
+                    # We see instability when allowing the client to open many connections at once.
+                    # Limiting concurrency results in more stable performance.
+                    max_connections=16,
+                    max_keepalive_connections=8,
+                    # The Prefect Cloud LB will keep connections alive for 30s.
+                    # Only allow the client to keep connections alive for 25s.
+                    keepalive_expiry=25,
+                ),
+            )
+
+            # See https://www.python-httpx.org/http2/
+            # Enabling HTTP/2 support on the client does not necessarily mean that your requests
+            # and responses will be transported over HTTP/2, since both the client and the server
+            # need to support HTTP/2. If you connect to a server that only supports HTTP/1.1 the
+            # client will use a standard HTTP/1.1 connection instead.
+            httpx_settings.setdefault("http2", PREFECT_API_ENABLE_HTTP2.value())
+
+            self.server_type = (
+                ServerType.CLOUD
+                if api.startswith(PREFECT_CLOUD_API_URL.value())
+                else ServerType.SERVER
+            )
+
+        # Connect to an in-process application
+        elif isinstance(api, ASGIApp):
+            self._ephemeral_app = api
+            self.server_type = ServerType.EPHEMERAL
+
+        else:
+            raise TypeError(
+                f"Unexpected type {type(api).__name__!r} for argument `api`. Expected"
+                " 'str' or 'ASGIApp/FastAPI'"
+            )
+
+        # See https://www.python-httpx.org/advanced/#timeout-configuration
+        httpx_settings.setdefault(
+            "timeout",
+            httpx.Timeout(
+                connect=PREFECT_API_REQUEST_TIMEOUT.value(),
+                read=PREFECT_API_REQUEST_TIMEOUT.value(),
+                write=PREFECT_API_REQUEST_TIMEOUT.value(),
+                pool=PREFECT_API_REQUEST_TIMEOUT.value(),
+            ),
         )
 
-    def __enter__(self):
-        run_sync(self._prefect_client.__aenter__())
+        if not PREFECT_UNIT_TEST_MODE:
+            httpx_settings.setdefault("follow_redirects", True)
+
+        enable_csrf_support = (
+            self.server_type != ServerType.CLOUD
+            and PREFECT_CLIENT_CSRF_SUPPORT_ENABLED.value()
+        )
+
+        if self.server_type == ServerType.EPHEMERAL:
+            self._client = PrefectHttpxSyncEphemeralClient(
+                api, base_url="http://ephemeral-prefect/api"
+            )
+        else:
+            self._client = PrefectHttpxSyncClient(
+                **httpx_settings, enable_csrf_support=enable_csrf_support
+            )
+
+        # See https://www.python-httpx.org/advanced/#custom-transports
+        #
+        # If we're using an HTTP/S client (not the ephemeral client), adjust the
+        # transport to add retries _after_ it is instantiated. If we alter the transport
+        # before instantiation, the transport will not be aware of proxies unless we
+        # reproduce all of the logic to make it so.
+        #
+        # Only alter the transport to set our default of 3 retries, don't modify any
+        # transport a user may have provided via httpx_settings.
+        #
+        # Making liberal use of getattr and isinstance checks here to avoid any
+        # surprises if the internals of httpx or httpcore change on us
+        if isinstance(api, str) and not httpx_settings.get("transport"):
+            transport_for_url = getattr(self._client, "_transport_for_url", None)
+            if callable(transport_for_url):
+                server_transport = transport_for_url(httpx.URL(api))
+                if isinstance(server_transport, httpx.HTTPTransport):
+                    pool = getattr(server_transport, "_pool", None)
+                    if isinstance(pool, httpcore.ConnectionPool):
+                        pool._retries = 3
+
+        self.logger = get_logger("client")
+
+    @property
+    def api_url(self) -> httpx.URL:
+        """
+        Get the base URL for the API.
+        """
+        return self._client.base_url
+
+    # Context management ----------------------------------------------------------------
+
+    def __enter__(self) -> "SyncPrefectClient":
+        """
+        Start the client.
+
+        If the client is already started, this will raise an exception.
+
+        If the client is already closed, this will raise an exception. Use a new client
+        instance instead.
+        """
+        if self._closed:
+            # httpx.Client does not allow reuse so we will not either.
+            raise RuntimeError(
+                "The client cannot be started again after closing. "
+                "Retrieve a new client with `get_client()` instead."
+            )
+
+        if self._started:
+            # httpx.Client does not allow reentrancy so we will not either.
+            raise RuntimeError("The client cannot be started more than once.")
+        self._client.__enter__()
+        self._started = True
+
         return self
 
-    def __exit__(self, *exc_info):
-        return run_sync(self._prefect_client.__aexit__(*exc_info))
+    def __exit__(self, *exc_info) -> None:
+        """
+        Shutdown the client.
+        """
+        self._closed = True
+        self._client.__exit__(*exc_info)
 
-    async def __aenter__(self):
-        raise RuntimeError(
-            "The `SyncPrefectClient` must be entered with a sync context. Use '"
-            "with SyncPrefectClient(...)' not 'async with SyncPrefectClient(...)'"
-        )
+    # API methods ----------------------------------------------------------------------
+
+    def api_healthcheck(self) -> Optional[Exception]:
+        """
+        Attempts to connect to the API and returns the encountered exception if not
+        successful.
 
-    async def __aexit__(self, *_):
-        assert False, "This should never be called but must be defined for __aenter__"
+        If successful, returns `None`.
+        """
+        try:
+            self._client.get("/health")
+            return None
+        except Exception as exc:
+            return exc
 
     def hello(self) -> httpx.Response:
         """
         Send a GET request to /hello for testing purposes.
         """
-        return run_sync(self._prefect_client.hello())
+        return self._client.get("/hello")
+
+    def create_flow(self, flow: "FlowObject") -> UUID:
+        """
+        Create a flow in the Prefect API.
+
+        Args:
+            flow: a [Flow][prefect.flows.Flow] object
+
+        Raises:
+            httpx.RequestError: if a flow was not created for any reason
+
+        Returns:
+            the ID of the flow in the backend
+        """
+        return self.create_flow_from_name(flow.name)
+
+    def create_flow_from_name(self, flow_name: str) -> UUID:
+        """
+        Create a flow in the Prefect API.
+
+        Args:
+            flow_name: the name of the new flow
+
+        Raises:
+            httpx.RequestError: if a flow was not created for any reason
+
+        Returns:
+            the ID of the flow in the backend
+        """
+        flow_data = FlowCreate(name=flow_name)
+        response = self._client.post(
+            "/flows/", json=flow_data.dict(json_compatible=True)
+        )
+
+        flow_id = response.json().get("id")
+        if not flow_id:
+            raise httpx.RequestError(f"Malformed response: {response}")
+
+        # Return the id of the created flow
+        return UUID(flow_id)
+
+    def create_flow_run(
+        self,
+        flow: "FlowObject",
+        name: Optional[str] = None,
+        parameters: Optional[Dict[str, Any]] = None,
+        context: Optional[Dict[str, Any]] = None,
+        tags: Optional[Iterable[str]] = None,
+        parent_task_run_id: Optional[UUID] = None,
+        state: Optional["prefect.states.State"] = None,
+    ) -> FlowRun:
+        """
+        Create a flow run for a flow.
+
+        Args:
+            flow: The flow model to create the flow run for
+            name: An optional name for the flow run
+            parameters: Parameter overrides for this flow run.
+            context: Optional run context data
+            tags: a list of tags to apply to this flow run
+            parent_task_run_id: if a subflow run is being created, the placeholder task
+                run identifier in the parent flow
+            state: The initial state for the run. If not provided, defaults to
+                `Scheduled` for now. Should always be a `Scheduled` type.
+
+        Raises:
+            httpx.RequestError: if the Prefect API does not successfully create a run for any reason
+
+        Returns:
+            The flow run model
+        """
+        parameters = parameters or {}
+        context = context or {}
+
+        if state is None:
+            state = prefect.states.Pending()
+
+        # Retrieve the flow id
+        flow_id = self.create_flow(flow)
+
+        flow_run_create = FlowRunCreate(
+            flow_id=flow_id,
+            flow_version=flow.version,
+            name=name,
+            parameters=parameters,
+            context=context,
+            tags=list(tags or []),
+            parent_task_run_id=parent_task_run_id,
+            state=state.to_state_create(),
+            empirical_policy=FlowRunPolicy(
+                retries=flow.retries,
+                retry_delay=flow.retry_delay_seconds,
+            ),
+        )
+
+        flow_run_create_json = flow_run_create.dict(json_compatible=True)
+        response = self._client.post("/flow_runs/", json=flow_run_create_json)
+        flow_run = FlowRun.parse_obj(response.json())
+
+        # Restore the parameters to the local objects to retain expectations about
+        # Python objects
+        flow_run.parameters = parameters
+
+        return flow_run
+
+    def read_flow_run(self, flow_run_id: UUID) -> FlowRun:
+        """
+        Query the Prefect API for a flow run by id.
+
+        Args:
+            flow_run_id: the flow run ID of interest
+
+        Returns:
+            a Flow Run model representation of the flow run
+        """
+        try:
+            response = self._client.get(f"/flow_runs/{flow_run_id}")
+        except httpx.HTTPStatusError as e:
+            if e.response.status_code == 404:
+                raise prefect.exceptions.ObjectNotFound(http_exc=e) from e
+            else:
+                raise
+        return FlowRun.parse_obj(response.json())
+
+    def read_flow_runs(
+        self,
+        *,
+        flow_filter: FlowFilter = None,
+        flow_run_filter: FlowRunFilter = None,
+        task_run_filter: TaskRunFilter = None,
+        deployment_filter: DeploymentFilter = None,
+        work_pool_filter: WorkPoolFilter = None,
+        work_queue_filter: WorkQueueFilter = None,
+        sort: FlowRunSort = None,
+        limit: int = None,
+        offset: int = 0,
+    ) -> List[FlowRun]:
+        """
+        Query the Prefect API for flow runs. Only flow runs matching all criteria will
+        be returned.
+
+        Args:
+            flow_filter: filter criteria for flows
+            flow_run_filter: filter criteria for flow runs
+            task_run_filter: filter criteria for task runs
+            deployment_filter: filter criteria for deployments
+            work_pool_filter: filter criteria for work pools
+            work_queue_filter: filter criteria for work pool queues
+            sort: sort criteria for the flow runs
+            limit: limit for the flow run query
+            offset: offset for the flow run query
+
+        Returns:
+            a list of Flow Run model representations
+                of the flow runs
+        """
+        body = {
+            "flows": flow_filter.dict(json_compatible=True) if flow_filter else None,
+            "flow_runs": (
+                flow_run_filter.dict(json_compatible=True, exclude_unset=True)
+                if flow_run_filter
+                else None
+            ),
+            "task_runs": (
+                task_run_filter.dict(json_compatible=True) if task_run_filter else None
+            ),
+            "deployments": (
+                deployment_filter.dict(json_compatible=True)
+                if deployment_filter
+                else None
+            ),
+            "work_pools": (
+                work_pool_filter.dict(json_compatible=True)
+                if work_pool_filter
+                else None
+            ),
+            "work_pool_queues": (
+                work_queue_filter.dict(json_compatible=True)
+                if work_queue_filter
+                else None
+            ),
+            "sort": sort,
+            "limit": limit,
+            "offset": offset,
+        }
+
+        response = self._client.post("/flow_runs/filter", json=body)
+        return pydantic.parse_obj_as(List[FlowRun], response.json())
+
+    def set_flow_run_state(
+        self,
+        flow_run_id: UUID,
+        state: "prefect.states.State",
+        force: bool = False,
+    ) -> OrchestrationResult:
+        """
+        Set the state of a flow run.
+
+        Args:
+            flow_run_id: the id of the flow run
+            state: the state to set
+            force: if True, disregard orchestration logic when setting the state,
+                forcing the Prefect API to accept the state
+
+        Returns:
+            an OrchestrationResult model representation of state orchestration output
+        """
+        state_create = state.to_state_create()
+        state_create.state_details.flow_run_id = flow_run_id
+        state_create.state_details.transition_id = uuid4()
+        try:
+            response = self._client.post(
+                f"/flow_runs/{flow_run_id}/set_state",
+                json=dict(state=state_create.dict(json_compatible=True), force=force),
+            )
+        except httpx.HTTPStatusError as e:
+            if e.response.status_code == status.HTTP_404_NOT_FOUND:
+                raise prefect.exceptions.ObjectNotFound(http_exc=e) from e
+            else:
+                raise
+
+        return OrchestrationResult.parse_obj(response.json())
 
     def create_task_run(
         self,
         task: "TaskObject[P, R]",
         flow_run_id: Optional[UUID],
         dynamic_key: str,
         name: Optional[str] = None,
@@ -3453,25 +3839,102 @@
             state: The initial state for the run. If not provided, defaults to
                 `Pending` for now. Should always be a `Scheduled` type.
             task_inputs: the set of inputs passed to the task
 
         Returns:
             The created task run.
         """
-        return run_sync(
-            self._prefect_client.create_task_run(
-                task=task,
-                flow_run_id=flow_run_id,
-                dynamic_key=dynamic_key,
-                name=name,
-                extra_tags=extra_tags,
-                state=state,
-                task_inputs=task_inputs,
-            )
+        tags = set(task.tags).union(extra_tags or [])
+
+        if state is None:
+            state = prefect.states.Pending()
+
+        task_run_data = TaskRunCreate(
+            name=name,
+            flow_run_id=flow_run_id,
+            task_key=task.task_key,
+            dynamic_key=dynamic_key,
+            tags=list(tags),
+            task_version=task.version,
+            empirical_policy=TaskRunPolicy(
+                retries=task.retries,
+                retry_delay=task.retry_delay_seconds,
+                retry_jitter_factor=task.retry_jitter_factor,
+            ),
+            state=state.to_state_create(),
+            task_inputs=task_inputs or {},
+        )
+
+        response = self._client.post(
+            "/task_runs/", json=task_run_data.dict(json_compatible=True)
         )
+        return TaskRun.parse_obj(response.json())
+
+    def read_task_run(self, task_run_id: UUID) -> TaskRun:
+        """
+        Query the Prefect API for a task run by id.
+
+        Args:
+            task_run_id: the task run ID of interest
+
+        Returns:
+            a Task Run model representation of the task run
+        """
+        response = self._client.get(f"/task_runs/{task_run_id}")
+        return TaskRun.parse_obj(response.json())
+
+    def read_task_runs(
+        self,
+        *,
+        flow_filter: FlowFilter = None,
+        flow_run_filter: FlowRunFilter = None,
+        task_run_filter: TaskRunFilter = None,
+        deployment_filter: DeploymentFilter = None,
+        sort: TaskRunSort = None,
+        limit: int = None,
+        offset: int = 0,
+    ) -> List[TaskRun]:
+        """
+        Query the Prefect API for task runs. Only task runs matching all criteria will
+        be returned.
+
+        Args:
+            flow_filter: filter criteria for flows
+            flow_run_filter: filter criteria for flow runs
+            task_run_filter: filter criteria for task runs
+            deployment_filter: filter criteria for deployments
+            sort: sort criteria for the task runs
+            limit: a limit for the task run query
+            offset: an offset for the task run query
+
+        Returns:
+            a list of Task Run model representations
+                of the task runs
+        """
+        body = {
+            "flows": flow_filter.dict(json_compatible=True) if flow_filter else None,
+            "flow_runs": (
+                flow_run_filter.dict(json_compatible=True, exclude_unset=True)
+                if flow_run_filter
+                else None
+            ),
+            "task_runs": (
+                task_run_filter.dict(json_compatible=True) if task_run_filter else None
+            ),
+            "deployments": (
+                deployment_filter.dict(json_compatible=True)
+                if deployment_filter
+                else None
+            ),
+            "sort": sort,
+            "limit": limit,
+            "offset": offset,
+        }
+        response = self._client.post("/task_runs/filter", json=body)
+        return pydantic.parse_obj_as(List[TaskRun], response.json())
 
     def set_task_run_state(
         self,
         task_run_id: UUID,
         state: prefect.states.State,
         force: bool = False,
     ) -> OrchestrationResult:
@@ -3483,83 +3946,29 @@
             state: the state to set
             force: if True, disregard orchestration logic when setting the state,
                 forcing the Prefect API to accept the state
 
         Returns:
             an OrchestrationResult model representation of state orchestration output
         """
-        return run_sync(
-            self._prefect_client.set_task_run_state(
-                task_run_id=task_run_id,
-                state=state,
-                force=force,
-            )
-        )
-
-    def create_flow_run(
-        self,
-        flow_id: UUID,
-        parameters: Optional[Dict[str, Any]] = None,
-        context: Optional[Dict[str, Any]] = None,
-        scheduled_start_time: Optional[datetime.datetime] = None,
-        run_name: Optional[str] = None,
-        labels: Optional[List[str]] = None,
-        parameters_json: Optional[str] = None,
-        run_config: Optional[Dict[str, Any]] = None,
-        idempotency_key: Optional[str] = None,
-    ) -> FlowRunResponse:
-        """
-        Create a new flow run.
-
-        Args:
-            - flow_id (UUID): the ID of the flow to create a run for
-            - parameters (Optional[Dict[str, Any]]): a dictionary of parameter values to pass to the flow
-            - context (Optional[Dict[str, Any]]): a dictionary of context values to pass to the flow
-            - scheduled_start_time (Optional[datetime.datetime]): the scheduled start time for the flow run
-            - run_name (Optional[str]): a name to assign to the flow run
-            - labels (Optional[List[str]]): a list of labels to assign to the flow run
-            - parameters_json (Optional[str]): a JSON string of parameter values to pass to the flow
-            - run_config (Optional[Dict[str, Any]]): a dictionary of run configuration options
-            - idempotency_key (Optional[str]): a key to ensure idempotency when creating the flow run
-
-        Returns:
-            - FlowRunResponse: the created flow run
-        """
-        return run_sync(
-            self._prefect_client.create_flow_run(
-                flow_id=flow_id,
-                parameters=parameters,
-                context=context,
-                scheduled_start_time=scheduled_start_time,
-                run_name=run_name,
-                labels=labels,
-                parameters_json=parameters_json,
-                run_config=run_config,
-                idempotency_key=idempotency_key,
-            )
+        state_create = state.to_state_create()
+        state_create.state_details.task_run_id = task_run_id
+        response = self._client.post(
+            f"/task_runs/{task_run_id}/set_state",
+            json=dict(state=state_create.dict(json_compatible=True), force=force),
         )
+        return OrchestrationResult.parse_obj(response.json())
 
-    async def set_flow_run_state(
-        self,
-        flow_run_id: UUID,
-        state: "prefect.states.State",
-        force: bool = False,
-    ) -> OrchestrationResult:
+    def read_task_run_states(self, task_run_id: UUID) -> List[prefect.states.State]:
         """
-        Set the state of a flow run.
+        Query for the states of a task run
 
         Args:
-            flow_run_id: the id of the flow run
-            state: the state to set
-            force: if True, disregard orchestration logic when setting the state,
-                forcing the Prefect API to accept the state
+            task_run_id: the id of the task run
 
         Returns:
-            an OrchestrationResult model representation of state orchestration output
+            a list of State model representations of the task run states
         """
-        return run_sync(
-            self._prefect_client.set_flow_run_state(
-                flow_run_id=flow_run_id,
-                state=state,
-                force=force,
-            )
+        response = self._client.get(
+            "/task_run_states/", params=dict(task_run_id=str(task_run_id))
         )
+        return pydantic.parse_obj_as(List[prefect.states.State], response.json())
```

### Comparing `prefect-client-2.18.3/src/prefect/client/schemas/__init__.py` & `prefect-client-2.19.0/src/prefect/client/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/client/schemas/actions.py` & `prefect-client-2.19.0/src/prefect/client/schemas/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 import prefect.client.schemas.objects as objects
 from prefect._internal.schemas.bases import ActionBaseModel
 from prefect._internal.schemas.fields import DateTimeTZ
 from prefect._internal.schemas.serializers import orjson_dumps_extra_compatible
 from prefect._internal.schemas.validators import (
     raise_on_name_alphanumeric_dashes_only,
     raise_on_name_alphanumeric_underscores_only,
+    raise_on_name_with_banned_characters,
     remove_old_deployment_fields,
     return_none_schedule,
     validate_message_template_variables,
     validate_name_present_on_nonanonymous_blocks,
+    validate_schedule_max_scheduled_runs,
 )
 from prefect.client.schemas.objects import StateDetails, StateType
 from prefect.client.schemas.schedules import SCHEDULE_TYPES
-from prefect.types import NonNegativeInteger
+from prefect.settings import PREFECT_DEPLOYMENT_SCHEDULE_MAX_SCHEDULED_RUNS
+from prefect.types import NonNegativeFloat, NonNegativeInteger, PositiveInteger
 from prefect.utilities.collections import listrepr
 from prefect.utilities.pydantic import get_class_fields_only
 
 if TYPE_CHECKING:
     from prefect.deprecated.data_documents import DataDocument
     from prefect.results import BaseResult
 
@@ -97,24 +100,63 @@
 class DeploymentScheduleCreate(ActionBaseModel):
     schedule: SCHEDULE_TYPES = Field(
         default=..., description="The schedule for the deployment."
     )
     active: bool = Field(
         default=True, description="Whether or not the schedule is active."
     )
+    max_active_runs: Optional[PositiveInteger] = Field(
+        default=None,
+        description="The maximum number of active runs for the schedule.",
+    )
+    max_scheduled_runs: Optional[PositiveInteger] = Field(
+        default=None,
+        description="The maximum number of scheduled runs for the schedule.",
+    )
+    catchup: bool = Field(
+        default=False,
+        description="Whether or not a worker should catch up on Late runs for the schedule.",
+    )
+
+    @validator("max_scheduled_runs")
+    def validate_max_scheduled_runs(cls, v):
+        return validate_schedule_max_scheduled_runs(
+            v, PREFECT_DEPLOYMENT_SCHEDULE_MAX_SCHEDULED_RUNS.value()
+        )
 
 
 class DeploymentScheduleUpdate(ActionBaseModel):
     schedule: Optional[SCHEDULE_TYPES] = Field(
         default=None, description="The schedule for the deployment."
     )
     active: bool = Field(
         default=True, description="Whether or not the schedule is active."
     )
 
+    max_active_runs: Optional[PositiveInteger] = Field(
+        default=None,
+        description="The maximum number of active runs for the schedule.",
+    )
+
+    max_scheduled_runs: Optional[PositiveInteger] = Field(
+        default=None,
+        description="The maximum number of scheduled runs for the schedule.",
+    )
+
+    catchup: Optional[bool] = Field(
+        default=None,
+        description="Whether or not a worker should catch up on Late runs for the schedule.",
+    )
+
+    @validator("max_scheduled_runs")
+    def validate_max_scheduled_runs(cls, v):
+        return validate_schedule_max_scheduled_runs(
+            v, PREFECT_DEPLOYMENT_SCHEDULE_MAX_SCHEDULED_RUNS.value()
+        )
+
 
 class DeploymentCreate(DeprecatedInfraOverridesField, ActionBaseModel):
     """Data used by the Prefect REST API to create a deployment."""
 
     @root_validator(pre=True)
     def remove_old_fields(cls, values):
         return remove_old_deployment_fields(values)
@@ -700,38 +742,46 @@
     _validate_name_format = validator("name", allow_reuse=True)(validate_variable_name)
 
 
 class GlobalConcurrencyLimitCreate(ActionBaseModel):
     """Data used by the Prefect REST API to create a global concurrency limit."""
 
     name: str = Field(description="The name of the global concurrency limit.")
-    limit: int = Field(
+    limit: NonNegativeInteger = Field(
         description=(
             "The maximum number of slots that can be occupied on this concurrency"
             " limit."
         )
     )
     active: Optional[bool] = Field(
         default=True,
         description="Whether or not the concurrency limit is in an active state.",
     )
-    active_slots: Optional[int] = Field(
+    active_slots: Optional[NonNegativeInteger] = Field(
         default=0,
         description="Number of tasks currently using a concurrency slot.",
     )
-    slot_decay_per_second: Optional[float] = Field(
+    slot_decay_per_second: Optional[NonNegativeFloat] = Field(
         default=0.0,
         description=(
             "Controls the rate at which slots are released when the concurrency limit"
             " is used as a rate limit."
         ),
     )
 
+    @validator("name", check_fields=False)
+    def validate_name_characters(cls, v):
+        return raise_on_name_with_banned_characters(v)
+
 
 class GlobalConcurrencyLimitUpdate(ActionBaseModel):
     """Data used by the Prefect REST API to update a global concurrency limit."""
 
     name: Optional[str] = Field(None)
-    limit: Optional[int] = Field(None)
-    active: Optional[bool] = Field(None)
-    active_slots: Optional[int] = Field(None)
-    slot_decay_per_second: Optional[float] = Field(None)
+    limit: Optional[NonNegativeInteger] = Field(None)
+    active: Optional[NonNegativeInteger] = Field(None)
+    active_slots: Optional[NonNegativeInteger] = Field(None)
+    slot_decay_per_second: Optional[NonNegativeFloat] = Field(None)
+
+    @validator("name", check_fields=False)
+    def validate_name_characters(cls, v):
+        return raise_on_name_with_banned_characters(v)
```

### Comparing `prefect-client-2.18.3/src/prefect/client/schemas/filters.py` & `prefect-client-2.19.0/src/prefect/client/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/client/schemas/objects.py` & `prefect-client-2.19.0/src/prefect/client/schemas/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,15 +686,17 @@
     )
     state_id: Optional[UUID] = Field(
         default=None, description="The id of the current task run state."
     )
     task_inputs: Dict[str, List[Union[TaskRunResult, Parameter, Constant]]] = Field(
         default_factory=dict,
         description=(
-            "Tracks the source of inputs to a task run. Used for internal bookkeeping."
+            "Tracks the source of inputs to a task run. Used for internal bookkeeping. "
+            "Note the special __parents__ key, used to indicate a parent/child "
+            "relationship that may or may not include an input or wait_for semantic."
         ),
     )
     state_type: Optional[StateType] = Field(
         default=None, description="The type of the current task run state."
     )
     state_name: Optional[str] = Field(
         default=None, description="The name of the current task run state."
@@ -927,14 +929,26 @@
     )
     schedule: SCHEDULE_TYPES = Field(
         default=..., description="The schedule for the deployment."
     )
     active: bool = Field(
         default=True, description="Whether or not the schedule is active."
     )
+    max_active_runs: Optional[PositiveInteger] = Field(
+        default=None,
+        description="The maximum number of active runs for the schedule.",
+    )
+    max_scheduled_runs: Optional[PositiveInteger] = Field(
+        default=None,
+        description="The maximum number of scheduled runs for the schedule.",
+    )
+    catchup: bool = Field(
+        default=False,
+        description="Whether or not a worker should catch up on Late runs for the schedule.",
+    )
 
 
 class Deployment(DeprecatedInfraOverridesField, ObjectBaseModel):
     """An ORM representation of deployment data."""
 
     name: str = Field(default=..., description="The name of the deployment.")
     version: Optional[str] = Field(
```

### Comparing `prefect-client-2.18.3/src/prefect/client/schemas/responses.py` & `prefect-client-2.19.0/src/prefect/client/schemas/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,7 +425,26 @@
 class MinimalConcurrencyLimitResponse(PrefectBaseModel):
     class Config:
         extra = "ignore"  # 2024/4/1
 
     id: UUID
     name: str
     limit: int
+
+
+class GlobalConcurrencyLimitResponse(ObjectBaseModel):
+    """
+    A response object for global concurrency limits.
+    """
+
+    active: bool = Field(
+        default=True, description="Whether the global concurrency limit is active."
+    )
+    name: str = Field(
+        default=..., description="The name of the global concurrency limit."
+    )
+    limit: int = Field(default=..., description="The concurrency limit.")
+    active_slots: int = Field(default=..., description="The number of active slots.")
+    slot_decay_per_second: float = Field(
+        default=2.0,
+        description="The decay rate for active slots when used as a rate limit.",
+    )
```

### Comparing `prefect-client-2.18.3/src/prefect/client/schemas/schedules.py` & `prefect-client-2.19.0/src/prefect/client/schemas/schedules.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
 
     class Config:
         extra = "forbid"
         exclude_none = True
 
     interval: PositiveDuration
-    anchor_date: DateTimeTZ = None
+    anchor_date: Optional[DateTimeTZ] = None
     timezone: Optional[str] = Field(default=None, examples=["America/New_York"])
 
     @validator("anchor_date", always=True)
     def validate_anchor_date(cls, v):
         return default_anchor_date(v)
 
     @validator("timezone", always=True)
```

### Comparing `prefect-client-2.18.3/src/prefect/client/schemas/sorting.py` & `prefect-client-2.19.0/src/prefect/client/schemas/sorting.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/client/subscriptions.py` & `prefect-client-2.19.0/src/prefect/client/subscriptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/client/utilities.py` & `prefect-client-2.19.0/src/prefect/client/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,20 @@
     from prefect.context import FlowRunContext, TaskRunContext
 
     flow_run_context = FlowRunContext.get()
     task_run_context = TaskRunContext.get()
 
     if (
         flow_run_context
-        and getattr(flow_run_context.client, "_loop") == get_running_loop()
+        and getattr(flow_run_context.client, "_loop", None) == get_running_loop()
     ):
         return flow_run_context.client, True
     elif (
         task_run_context
-        and getattr(task_run_context.client, "_loop") == get_running_loop()
+        and getattr(task_run_context.client, "_loop", None) == get_running_loop()
     ):
         return task_run_context.client, True
     else:
         from prefect.client.orchestration import get_client as get_httpx_client
 
         return get_httpx_client(), False
```

### Comparing `prefect-client-2.18.3/src/prefect/concurrency/asyncio.py` & `prefect-client-2.19.0/src/prefect/concurrency/asyncio.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,69 @@
 import asyncio
 from contextlib import asynccontextmanager
-from typing import List, Literal, Union, cast
+from typing import List, Literal, Optional, Union, cast
 
 import httpx
 import pendulum
 
 try:
     from pendulum import Interval
 except ImportError:
     # pendulum < 3
     from pendulum.period import Period as Interval  # type: ignore
 
 from prefect import get_client
 from prefect.client.schemas.responses import MinimalConcurrencyLimitResponse
+from prefect.utilities.timeout import timeout_async
 
 from .events import (
     _emit_concurrency_acquisition_events,
     _emit_concurrency_release_events,
 )
 from .services import ConcurrencySlotAcquisitionService
 
 
 class ConcurrencySlotAcquisitionError(Exception):
     """Raised when an unhandlable occurs while acquiring concurrency slots."""
 
 
 @asynccontextmanager
-async def concurrency(names: Union[str, List[str]], occupy: int = 1):
+async def concurrency(
+    names: Union[str, List[str]],
+    occupy: int = 1,
+    timeout_seconds: Optional[float] = None,
+):
+    """A context manager that acquires and releases concurrency slots from the
+    given concurrency limits.
+
+    Args:
+        names: The names of the concurrency limits to acquire slots from.
+        occupy: The number of slots to acquire and hold from each limit.
+        timeout_seconds: The number of seconds to wait for the slots to be acquired before
+            raising a `TimeoutError`. A timeout of `None` will wait indefinitely.
+
+    Raises:
+        TimeoutError: If the slots are not acquired within the given timeout.
+
+    Example:
+    A simple example of using the async `concurrency` context manager:
+    ```python
+    from prefect.concurrency.asyncio import concurrency
+
+    async def resource_heavy():
+        async with concurrency("test", occupy=1):
+            print("Resource heavy task")
+
+    async def main():
+        await resource_heavy()
+    ```
+    """
     names = names if isinstance(names, list) else [names]
-
-    limits = await _acquire_concurrency_slots(names, occupy)
+    with timeout_async(seconds=timeout_seconds):
+        limits = await _acquire_concurrency_slots(names, occupy)
     acquisition_time = pendulum.now("UTC")
     emitted_events = _emit_concurrency_acquisition_events(limits, occupy)
 
     try:
         yield
     finally:
         occupancy_period = cast(Interval, (pendulum.now("UTC") - acquisition_time))
```

### Comparing `prefect-client-2.18.3/src/prefect/concurrency/events.py` & `prefect-client-2.19.0/src/prefect/concurrency/events.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/concurrency/services.py` & `prefect-client-2.19.0/src/prefect/concurrency/services.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/concurrency/sync.py` & `prefect-client-2.19.0/src/prefect/concurrency/sync.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,82 @@
 from contextlib import contextmanager
-from typing import List, Union, cast
+from typing import List, Optional, Union, cast
 
 import pendulum
 
 try:
     from pendulum import Interval
 except ImportError:
     # pendulum < 3
     from pendulum.period import Period as Interval  # type: ignore
 
 from prefect._internal.concurrency.api import create_call, from_sync
 from prefect._internal.concurrency.event_loop import get_running_loop
 from prefect.client.schemas.responses import MinimalConcurrencyLimitResponse
+from prefect.utilities.timeout import timeout
 
 from .asyncio import (
     _acquire_concurrency_slots,
     _release_concurrency_slots,
 )
 from .events import (
     _emit_concurrency_acquisition_events,
     _emit_concurrency_release_events,
 )
 
 
 @contextmanager
-def concurrency(names: Union[str, List[str]], occupy: int = 1):
+def concurrency(
+    names: Union[str, List[str]],
+    occupy: int = 1,
+    timeout_seconds: Optional[float] = None,
+):
+    """A context manager that acquires and releases concurrency slots from the
+    given concurrency limits.
+
+    Args:
+        names: The names of the concurrency limits to acquire slots from.
+        occupy: The number of slots to acquire and hold from each limit.
+        timeout_seconds: The number of seconds to wait for the slots to be acquired before
+            raising a `TimeoutError`. A timeout of `None` will wait indefinitely.
+
+    Raises:
+        TimeoutError: If the slots are not acquired within the given timeout.
+
+    Example:
+    A simple example of using the sync `concurrency` context manager:
+    ```python
+    from prefect.concurrency.sync import concurrency
+
+    def resource_heavy():
+        with concurrency("test", occupy=1):
+            print("Resource heavy task")
+
+    def main():
+        resource_heavy()
+    ```
+    """
     names = names if isinstance(names, list) else [names]
 
-    limits: List[MinimalConcurrencyLimitResponse] = _call_async_function_from_sync(
-        _acquire_concurrency_slots, names, occupy
-    )
+    with timeout(seconds=timeout_seconds):
+        limits: List[MinimalConcurrencyLimitResponse] = _call_async_function_from_sync(
+            _acquire_concurrency_slots, names, occupy
+        )
     acquisition_time = pendulum.now("UTC")
     emitted_events = _emit_concurrency_acquisition_events(limits, occupy)
 
     try:
         yield
     finally:
         occupancy_period = cast(Interval, pendulum.now("UTC") - acquisition_time)
         _call_async_function_from_sync(
-            _release_concurrency_slots, names, occupy, occupancy_period.total_seconds()
+            _release_concurrency_slots,
+            names,
+            occupy,
+            occupancy_period.total_seconds(),
         )
         _emit_concurrency_release_events(limits, occupy, emitted_events)
 
 
 def rate_limit(names: Union[str, List[str]], occupy: int = 1):
     """Block execution until an `occupy` number of slots of the concurrency
     limits given in `names` are acquired. Requires that all given concurrency
```

### Comparing `prefect-client-2.18.3/src/prefect/context.py` & `prefect-client-2.19.0/src/prefect/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 else:
     from pydantic import BaseModel, Field, PrivateAttr
 
 import prefect.logging
 import prefect.logging.configuration
 import prefect.settings
 from prefect._internal.schemas.fields import DateTimeTZ
-from prefect.client.orchestration import PrefectClient
+from prefect.client.orchestration import PrefectClient, SyncPrefectClient
 from prefect.client.schemas import FlowRun, TaskRun
 from prefect.events.worker import EventsWorker
 from prefect.exceptions import MissingContextError
 from prefect.futures import PrefectFuture
 from prefect.results import ResultFactory
 from prefect.settings import PREFECT_HOME, Profile, Settings
 from prefect.states import State
@@ -209,15 +209,15 @@
     Attributes:
         start_time: The time the run context was entered
         client: The Prefect client instance being used for API communication
     """
 
     start_time: DateTimeTZ = Field(default_factory=lambda: pendulum.now("UTC"))
     input_keyset: Optional[Dict[str, Dict[str, str]]] = None
-    client: PrefectClient
+    client: Union[PrefectClient, SyncPrefectClient]
 
 
 class EngineContext(RunContext):
     """
     The context for a flow run. Data in this context is only available from within a
     flow run function.
```

### Comparing `prefect-client-2.18.3/src/prefect/deployments/base.py` & `prefect-client-2.19.0/src/prefect/deployments/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deployments/deployments.py` & `prefect-client-2.19.0/src/prefect/deployments/deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deployments/runner.py` & `prefect-client-2.19.0/src/prefect/deployments/runner.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deployments/schedules.py` & `prefect-client-2.19.0/src/prefect/deployments/schedules.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deployments/steps/core.py` & `prefect-client-2.19.0/src/prefect/deployments/steps/core.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deployments/steps/pull.py` & `prefect-client-2.19.0/src/prefect/deployments/steps/pull.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deployments/steps/utility.py` & `prefect-client-2.19.0/src/prefect/deployments/steps/utility.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deprecated/data_documents.py` & `prefect-client-2.19.0/src/prefect/deprecated/data_documents.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deprecated/packaging/base.py` & `prefect-client-2.19.0/src/prefect/deprecated/packaging/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deprecated/packaging/docker.py` & `prefect-client-2.19.0/src/prefect/deprecated/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deprecated/packaging/file.py` & `prefect-client-2.19.0/src/prefect/deprecated/packaging/file.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deprecated/packaging/orion.py` & `prefect-client-2.19.0/src/prefect/deprecated/packaging/orion.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/deprecated/packaging/serializers.py` & `prefect-client-2.19.0/src/prefect/deprecated/packaging/serializers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/engine.py` & `prefect-client-2.19.0/src/prefect/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -2434,22 +2434,22 @@
         )
         exit(1)
 
     try:
         if PREFECT_EXPERIMENTAL_ENABLE_NEW_ENGINE.value():
             from prefect.new_flow_engine import (
                 load_flow_and_flow_run,
-                run_flow,
+                run_flow_async,
                 run_flow_sync,
             )
 
             flow_run, flow = run_sync(load_flow_and_flow_run)
             # run the flow
             if flow.isasync:
-                run_sync(run_flow(flow, flow_run=flow_run))
+                run_sync(run_flow_async(flow, flow_run=flow_run))
             else:
                 run_flow_sync(flow, flow_run=flow_run)
         else:
             enter_flow_run_engine_from_subprocess(flow_run_id)
     except Abort as exc:
         engine_logger.info(
             f"Engine execution of flow run '{flow_run_id}' aborted by orchestrator:"
```

### Comparing `prefect-client-2.18.3/src/prefect/events/__init__.py` & `prefect-client-2.19.0/src/prefect/events/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/actions.py` & `prefect-client-2.19.0/src/prefect/events/actions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/cli/automations.py` & `prefect-client-2.19.0/src/prefect/events/cli/automations.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/clients.py` & `prefect-client-2.19.0/src/prefect/events/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from websockets.client import WebSocketClientProtocol, connect
 from websockets.exceptions import (
     ConnectionClosed,
     ConnectionClosedError,
     ConnectionClosedOK,
 )
 
-from prefect.client.base import PrefectHttpxClient
+from prefect.client.base import PrefectHttpxAsyncClient
 from prefect.events import Event
 from prefect.logging import get_logger
 from prefect.settings import (
     PREFECT_API_KEY,
     PREFECT_API_URL,
     PREFECT_CLOUD_API_URL,
     PREFECT_EXPERIMENTAL_EVENTS,
@@ -189,15 +189,15 @@
                 "PrefectEphemeralEventsClient cannot be used when PREFECT_API_KEY is set."
                 " Please use PrefectEventsClient or PrefectCloudEventsClient instead."
             )
         from prefect.server.api.server import create_app
 
         app = create_app()
 
-        self._http_client = PrefectHttpxClient(
+        self._http_client = PrefectHttpxAsyncClient(
             transport=httpx.ASGITransport(app=app, raise_app_exceptions=False),
             base_url="http://ephemeral-prefect/api",
             enable_csrf_support=False,
         )
 
     async def __aenter__(self) -> Self:
         await super().__aenter__()
```

### Comparing `prefect-client-2.18.3/src/prefect/events/filters.py` & `prefect-client-2.19.0/src/prefect/events/filters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/instrument.py` & `prefect-client-2.19.0/src/prefect/events/instrument.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/related.py` & `prefect-client-2.19.0/src/prefect/events/related.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/schemas/automations.py` & `prefect-client-2.19.0/src/prefect/events/schemas/automations.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/schemas/deployment_triggers.py` & `prefect-client-2.19.0/src/prefect/events/schemas/deployment_triggers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/schemas/events.py` & `prefect-client-2.19.0/src/prefect/events/schemas/events.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/schemas/labelling.py` & `prefect-client-2.19.0/src/prefect/events/schemas/labelling.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/utilities.py` & `prefect-client-2.19.0/src/prefect/events/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/events/worker.py` & `prefect-client-2.19.0/src/prefect/events/worker.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/exceptions.py` & `prefect-client-2.19.0/src/prefect/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/filesystems.py` & `prefect-client-2.19.0/src/prefect/filesystems.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/flow_runs.py` & `prefect-client-2.19.0/src/prefect/flow_runs.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/flows.py` & `prefect-client-2.19.0/src/prefect/flows.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,31 +339,14 @@
                     "Disable validation or change the argument names."
                 ) from exc
 
         self.persist_result = persist_result
         self.result_storage = result_storage
         self.result_serializer = result_serializer
         self.cache_result_in_memory = cache_result_in_memory
-
-        # Check for collision in the registry
-        registry = PrefectObjectRegistry.get()
-
-        if registry and any(
-            other
-            for other in registry.get_instances(Flow)
-            if other.name == self.name and id(other.fn) != id(self.fn)
-        ):
-            file = inspect.getsourcefile(self.fn)
-            line_number = inspect.getsourcelines(self.fn)[1]
-            warnings.warn(
-                f"A flow named {self.name!r} and defined at '{file}:{line_number}' "
-                "conflicts with another flow. Consider specifying a unique `name` "
-                "parameter in the flow definition:\n\n "
-                "`@flow(name='my_unique_name', ...)`"
-            )
         self.on_completion = on_completion
         self.on_failure = on_failure
         self.on_cancellation = on_cancellation
         self.on_crashed = on_crashed
         self.on_running = on_running
 
         # Used for flows loaded from remote storage
@@ -1715,7 +1698,98 @@
     try:
         flow = load_flow_from_script(tmpfile.name, flow_name=flow_name)
     finally:
         # windows compat
         tmpfile.close()
         os.remove(tmpfile.name)
     return flow
+
+
+@sync_compatible
+async def serve(
+    *args: "RunnerDeployment",
+    pause_on_shutdown: bool = True,
+    print_starting_message: bool = True,
+    limit: Optional[int] = None,
+    **kwargs,
+):
+    """
+    Serve the provided list of deployments.
+
+    Args:
+        *args: A list of deployments to serve.
+        pause_on_shutdown: A boolean for whether or not to automatically pause
+            deployment schedules on shutdown.
+        print_starting_message: Whether or not to print message to the console
+            on startup.
+        limit: The maximum number of runs that can be executed concurrently.
+        **kwargs: Additional keyword arguments to pass to the runner.
+
+    Examples:
+        Prepare two deployments and serve them:
+
+        ```python
+        import datetime
+
+        from prefect import flow, serve
+
+        @flow
+        def my_flow(name):
+            print(f"hello {name}")
+
+        @flow
+        def my_other_flow(name):
+            print(f"goodbye {name}")
+
+        if __name__ == "__main__":
+            # Run once a day
+            hello_deploy = my_flow.to_deployment(
+                "hello", tags=["dev"], interval=datetime.timedelta(days=1)
+            )
+
+            # Run every Sunday at 4:00 AM
+            bye_deploy = my_other_flow.to_deployment(
+                "goodbye", tags=["dev"], cron="0 4 * * sun"
+            )
+
+            serve(hello_deploy, bye_deploy)
+        ```
+    """
+    from rich.console import Console, Group
+    from rich.table import Table
+
+    from prefect.runner import Runner
+
+    runner = Runner(pause_on_shutdown=pause_on_shutdown, limit=limit, **kwargs)
+    for deployment in args:
+        await runner.add_deployment(deployment)
+
+    if print_starting_message:
+        help_message_top = (
+            "[green]Your deployments are being served and polling for"
+            " scheduled runs!\n[/]"
+        )
+
+        table = Table(title="Deployments", show_header=False)
+
+        table.add_column(style="blue", no_wrap=True)
+
+        for deployment in args:
+            table.add_row(f"{deployment.flow_name}/{deployment.name}")
+
+        help_message_bottom = (
+            "\nTo trigger any of these deployments, use the"
+            " following command:\n[blue]\n\t$ prefect deployment run"
+            " [DEPLOYMENT_NAME]\n[/]"
+        )
+        if PREFECT_UI_URL:
+            help_message_bottom += (
+                "\nYou can also trigger your deployments via the Prefect UI:"
+                f" [blue]{PREFECT_UI_URL.value()}/deployments[/]\n"
+            )
+
+        console = Console()
+        console.print(
+            Group(help_message_top, table, help_message_bottom), soft_wrap=True
+        )
+
+    await runner.start()
```

### Comparing `prefect-client-2.18.3/src/prefect/futures.py` & `prefect-client-2.19.0/src/prefect/futures.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/__init__.py` & `prefect-client-2.19.0/src/prefect/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/base.py` & `prefect-client-2.19.0/src/prefect/infrastructure/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/container.py` & `prefect-client-2.19.0/src/prefect/infrastructure/container.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/kubernetes.py` & `prefect-client-2.19.0/src/prefect/infrastructure/kubernetes.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/process.py` & `prefect-client-2.19.0/src/prefect/infrastructure/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,27 @@
 
 This module is deprecated as of March 2024 and will not be available after September 2024.
 It has been replaced by the process worker from the `prefect.workers` module, which offers enhanced functionality and better performance.
 
 For upgrade instructions, see https://docs.prefect.io/latest/guides/upgrade-guide-agents-to-workers/.
 """
 
-import asyncio
 import contextlib
 import os
 import shlex
 import signal
 import socket
 import subprocess
 import sys
 import tempfile
 from pathlib import Path
 from typing import Dict, Tuple, Union
 
 import anyio
 import anyio.abc
-import sniffio
 
 from prefect._internal.compatibility.deprecated import deprecated_class
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import Field
 else:
@@ -39,28 +37,14 @@
 from prefect.utilities.processutils import get_sys_executable, run_process
 
 if sys.platform == "win32":
     # exit code indicating that the process was terminated by Ctrl+C or Ctrl+Break
     STATUS_CONTROL_C_EXIT = 0xC000013A
 
 
-def _use_threaded_child_watcher():
-    if (
-        sys.version_info < (3, 8)
-        and sniffio.current_async_library() == "asyncio"
-        and sys.platform != "win32"
-    ):
-        from prefect.utilities.compat import ThreadedChildWatcher
-
-        # Python < 3.8 does not use a `ThreadedChildWatcher` by default which can
-        # lead to errors in tests on unix as the previous default `SafeChildWatcher`
-        # is not compatible with threaded event loops.
-        asyncio.get_event_loop_policy().set_child_watcher(ThreadedChildWatcher())
-
-
 def _infrastructure_pid_from_process(process: anyio.abc.Process) -> str:
     hostname = socket.gethostname()
     return f"{hostname}:{process.pid}"
 
 
 def _parse_infrastructure_pid(infrastructure_pid: str) -> Tuple[str, int]:
     hostname, pid = infrastructure_pid.split(":")
@@ -117,15 +101,14 @@
     async def run(
         self,
         task_status: anyio.abc.TaskStatus = None,
     ) -> "ProcessResult":
         if not self.command:
             raise ValueError("Process cannot be run with empty command.")
 
-        _use_threaded_child_watcher()
         display_name = f" {self.name!r}" if self.name else ""
 
         # Open a subprocess to execute the flow run
         self.logger.info(f"Opening process{display_name}...")
         working_dir_ctx = (
             tempfile.TemporaryDirectory(suffix="prefect")
             if not self.working_dir
```

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/provisioners/__init__.py` & `prefect-client-2.19.0/src/prefect/infrastructure/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/provisioners/cloud_run.py` & `prefect-client-2.19.0/src/prefect/infrastructure/provisioners/cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/provisioners/container_instance.py` & `prefect-client-2.19.0/src/prefect/infrastructure/provisioners/container_instance.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/provisioners/ecs.py` & `prefect-client-2.19.0/src/prefect/infrastructure/provisioners/ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/infrastructure/provisioners/modal.py` & `prefect-client-2.19.0/src/prefect/infrastructure/provisioners/modal.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/input/__init__.py` & `prefect-client-2.19.0/src/prefect/input/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/input/actions.py` & `prefect-client-2.19.0/src/prefect/input/actions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/input/run_input.py` & `prefect-client-2.19.0/src/prefect/input/run_input.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/logging/configuration.py` & `prefect-client-2.19.0/src/prefect/logging/configuration.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/logging/filters.py` & `prefect-client-2.19.0/src/prefect/logging/filters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/logging/formatters.py` & `prefect-client-2.19.0/src/prefect/logging/formatters.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,18 +95,15 @@
 
         # defaults added in 3.10
         if sys.version_info >= (3, 10):
             init_kwargs["defaults"] = defaults
             style_kwargs["defaults"] = defaults
 
         # validate added in 3.8
-        if sys.version_info >= (3, 8):
-            init_kwargs["validate"] = validate
-        else:
-            validate = False
+        init_kwargs["validate"] = validate
 
         super().__init__(format, datefmt, style, **init_kwargs)
 
         self.flow_run_fmt = flow_run_fmt
         self.task_run_fmt = task_run_fmt
 
         # Retrieve the style class from the base class to avoid importing private
```

### Comparing `prefect-client-2.18.3/src/prefect/logging/handlers.py` & `prefect-client-2.19.0/src/prefect/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/logging/highlighters.py` & `prefect-client-2.19.0/src/prefect/logging/highlighters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/logging/loggers.py` & `prefect-client-2.19.0/src/prefect/logging/loggers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/logging/logging.yml` & `prefect-client-2.19.0/src/prefect/logging/logging.yml`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/manifests.py` & `prefect-client-2.19.0/src/prefect/manifests.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/new_flow_engine.py` & `prefect-client-2.19.0/src/prefect/new_flow_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import asyncio
 import inspect
+import logging
 import os
-from contextlib import AsyncExitStack, asynccontextmanager, contextmanager
-from dataclasses import dataclass
+import time
+from contextlib import contextmanager
+from dataclasses import dataclass, field
 from typing import (
     Any,
     Coroutine,
     Dict,
     Generic,
     Iterable,
     Literal,
@@ -20,143 +21,161 @@
 
 import anyio
 import anyio._backends._asyncio
 from sniffio import AsyncLibraryNotFoundError
 from typing_extensions import ParamSpec
 
 from prefect import Task, get_client
-from prefect.client.orchestration import PrefectClient
+from prefect.client.orchestration import SyncPrefectClient
 from prefect.client.schemas import FlowRun, TaskRun
 from prefect.client.schemas.filters import FlowRunFilter
 from prefect.client.schemas.sorting import FlowRunSort
 from prefect.context import FlowRunContext
 from prefect.deployments import load_flow_from_flow_run
+from prefect.exceptions import Abort, Pause
 from prefect.flows import Flow, load_flow_from_entrypoint
 from prefect.futures import PrefectFuture, resolve_futures_to_states
-from prefect.logging.loggers import flow_run_logger
+from prefect.logging.loggers import flow_run_logger, get_logger
 from prefect.results import ResultFactory
 from prefect.states import (
     Pending,
     Running,
     State,
+    exception_to_crashed_state,
     exception_to_failed_state,
     return_value_to_state,
 )
 from prefect.utilities.asyncutils import A, Async, run_sync
 from prefect.utilities.callables import parameters_to_args_kwargs
 from prefect.utilities.engine import (
-    _dynamic_key_for_task_run,
     _resolve_custom_flow_run_name,
-    collect_task_run_inputs,
-    propose_state,
+    propose_state_sync,
 )
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
-async def load_flow_and_flow_run(flow_run_id: UUID) -> Tuple[FlowRun, Flow]:
+def load_flow_and_flow_run(flow_run_id: UUID) -> Tuple[FlowRun, Flow]:
     ## TODO: add error handling to update state and log tracebacks
     entrypoint = os.environ.get("PREFECT__FLOW_ENTRYPOINT")
 
-    async with get_client() as client:
-        flow_run = await client.read_flow_run(flow_run_id)
-        flow = (
-            load_flow_from_entrypoint(entrypoint)
-            if entrypoint
-            else await load_flow_from_flow_run(flow_run, client=client)
-        )
+    client = get_client(sync_client=True)
+    flow_run = client.read_flow_run(flow_run_id)
+    flow = (
+        load_flow_from_entrypoint(entrypoint)
+        if entrypoint
+        else run_sync(load_flow_from_flow_run(flow_run, client=client))
+    )
+
     return flow_run, flow
 
 
 @dataclass
 class FlowRunEngine(Generic[P, R]):
     flow: Optional[Union[Flow[P, R], Flow[P, Coroutine[Any, Any, R]]]] = None
     parameters: Optional[Dict[str, Any]] = None
     flow_run: Optional[FlowRun] = None
     flow_run_id: Optional[UUID] = None
+    logger: logging.Logger = field(default_factory=lambda: get_logger("engine"))
     _is_started: bool = False
-    _client: Optional[PrefectClient] = None
+    _client: Optional[SyncPrefectClient] = None
     short_circuit: bool = False
 
     def __post_init__(self):
         if self.flow is None and self.flow_run_id is None:
             raise ValueError("Either a flow or a flow_run_id must be provided.")
 
         if self.parameters is None:
             self.parameters = {}
 
     @property
-    def client(self) -> PrefectClient:
+    def client(self) -> SyncPrefectClient:
         if not self._is_started or self._client is None:
             raise RuntimeError("Engine has not started.")
         return self._client
 
     @property
     def state(self) -> State:
         return self.flow_run.state  # type: ignore
 
-    async def begin_run(self) -> State:
+    def begin_run(self) -> State:
         new_state = Running()
-        state = await self.set_state(new_state)
+        state = self.set_state(new_state)
         while state.is_pending():
-            await asyncio.sleep(1)
-            state = await self.set_state(new_state)
+            time.sleep(0.2)
+            state = self.set_state(new_state)
         return state
 
-    async def set_state(self, state: State) -> State:
+    def set_state(self, state: State, force: bool = False) -> State:
         """ """
         # prevents any state-setting activity
         if self.short_circuit:
             return self.state
 
-        state = await propose_state(self.client, state, flow_run_id=self.flow_run.id)  # type: ignore
+        state = propose_state_sync(
+            self.client, state, flow_run_id=self.flow_run.id, force=force
+        )  # type: ignore
         self.flow_run.state = state  # type: ignore
         self.flow_run.state_name = state.name  # type: ignore
         self.flow_run.state_type = state.type  # type: ignore
         return state
 
-    async def result(self, raise_on_failure: bool = True) -> "Union[R, State, None]":
+    def result(self, raise_on_failure: bool = True) -> "Union[R, State, None]":
         _result = self.state.result(raise_on_failure=raise_on_failure, fetch=True)  # type: ignore
         # state.result is a `sync_compatible` function that may or may not return an awaitable
         # depending on whether the parent frame is sync or not
         if inspect.isawaitable(_result):
-            _result = await _result
+            _result = run_sync(_result)
         return _result
 
-    async def handle_success(self, result: R) -> R:
+    def handle_success(self, result: R) -> R:
         result_factory = getattr(FlowRunContext.get(), "result_factory", None)
         if result_factory is None:
             raise ValueError("Result factory is not set")
-        terminal_state = await return_value_to_state(
-            await resolve_futures_to_states(result),
-            result_factory=result_factory,
+        terminal_state = run_sync(
+            return_value_to_state(
+                run_sync(resolve_futures_to_states(result)),
+                result_factory=result_factory,
+            )
         )
-        await self.set_state(terminal_state)
+        self.set_state(terminal_state)
         return result
 
-    async def handle_exception(
+    def handle_exception(
         self,
         exc: Exception,
         msg: Optional[str] = None,
         result_factory: Optional[ResultFactory] = None,
     ) -> State:
         context = FlowRunContext.get()
-        state = await exception_to_failed_state(
-            exc,
-            message=msg or "Flow run encountered an exception:",
-            result_factory=result_factory or getattr(context, "result_factory", None),
+        state = run_sync(
+            exception_to_failed_state(
+                exc,
+                message=msg or "Flow run encountered an exception:",
+                result_factory=result_factory
+                or getattr(context, "result_factory", None),
+            )
         )
-        state = await self.set_state(state)
+        state = self.set_state(state)
         if self.state.is_scheduled():
-            state = await self.set_state(Running())
+            state = self.set_state(Running())
         return state
 
-    async def load_subflow_run(
-        self, parent_task_run: TaskRun, client: PrefectClient, context: FlowRunContext
+    def handle_crash(self, exc: BaseException) -> None:
+        state = run_sync(exception_to_crashed_state(exc))
+        self.logger.error(f"Crash detected! {state.message}")
+        self.logger.debug("Crash details:", exc_info=exc)
+        self.set_state(state, force=True)
+
+    def load_subflow_run(
+        self,
+        parent_task_run: TaskRun,
+        client: SyncPrefectClient,
+        context: FlowRunContext,
     ) -> Union[FlowRun, None]:
         """
         This method attempts to load an existing flow run for a subflow task
         run, if appropriate.
 
         If the parent task run is in a final but not COMPLETED state, and not
         being rerun, then we attempt to load an existing flow run instead of
@@ -181,126 +200,75 @@
         # situations where we are confident the flow should not be run
         # again.
         assert isinstance(parent_task_run.state, State)
         if parent_task_run.state.is_final() and not (
             rerunning and not parent_task_run.state.is_completed()
         ):
             # return the most recent flow run, if it exists
-            flow_runs = await client.read_flow_runs(
+            flow_runs = client.read_flow_runs(
                 flow_run_filter=FlowRunFilter(
                     parent_task_run_id={"any_": [parent_task_run.id]}
                 ),
                 sort=FlowRunSort.EXPECTED_START_TIME_ASC,
                 limit=1,
             )
             if flow_runs:
                 return flow_runs[-1]
 
-    async def create_subflow_task_run(
-        self, client: PrefectClient, context: FlowRunContext
-    ) -> TaskRun:
-        """
-        Adds a task to a parent flow run that represents the execution of a subflow run.
-
-        The task run is referred to as the "parent task run" of the subflow and will be kept
-        in sync with the subflow run's state by the orchestration engine.
-        """
-        dummy_task = Task(
-            name=self.flow.name, fn=self.flow.fn, version=self.flow.version
-        )
-        task_inputs = {
-            k: await collect_task_run_inputs(v)
-            for k, v in (self.parameters or {}).items()
-        }
-        parent_task_run = await client.create_task_run(
-            task=dummy_task,
-            flow_run_id=(
-                context.flow_run.id
-                if getattr(context, "flow_run", None)
-                and isinstance(context.flow_run, FlowRun)
-                else None
-            ),
-            dynamic_key=_dynamic_key_for_task_run(context, dummy_task),  # type: ignore
-            task_inputs=task_inputs,  # type: ignore
-            state=Pending(),
-        )
-        return parent_task_run
-
-    async def create_flow_run(self, client: PrefectClient) -> FlowRun:
+    def create_flow_run(self, client: SyncPrefectClient) -> FlowRun:
         flow_run_ctx = FlowRunContext.get()
         parameters = self.parameters or {}
 
         parent_task_run = None
 
         # this is a subflow run
         if flow_run_ctx:
-            # get the parent task run
-            parent_task_run = await self.create_subflow_task_run(
-                client=client, context=flow_run_ctx
+            # add a task to a parent flow run that represents the execution of a subflow run
+            # reuse the logic from the TaskRunEngine to ensure parents are created correctly
+            parent_task = Task(
+                name=self.flow.name, fn=self.flow.fn, version=self.flow.version
+            )
+            parent_task_run = run_sync(
+                parent_task.create_run(
+                    client=self.client,
+                    flow_run_context=flow_run_ctx,
+                    parameters=self.parameters,
+                )
             )
 
             # check if there is already a flow run for this subflow
-            if subflow_run := await self.load_subflow_run(
+            if subflow_run := self.load_subflow_run(
                 parent_task_run=parent_task_run, client=client, context=flow_run_ctx
             ):
                 return subflow_run
 
         try:
             flow_run_name = _resolve_custom_flow_run_name(
                 flow=self.flow, parameters=parameters
             )
         except TypeError:
             flow_run_name = None
 
-        flow_run = await client.create_flow_run(
+        flow_run = client.create_flow_run(
             flow=self.flow,
             name=flow_run_name,
             parameters=self.flow.serialize_parameters(parameters),
             state=Pending(),
             parent_task_run_id=getattr(parent_task_run, "id", None),
         )
         return flow_run
 
-    @asynccontextmanager
-    async def enter_run_context(self, client: Optional[PrefectClient] = None):
-        if client is None:
-            client = self.client
-        if not self.flow_run:
-            raise ValueError("Flow run not set")
-
-        self.flow_run = await client.read_flow_run(self.flow_run.id)
-        task_runner = self.flow.task_runner.duplicate()
-
-        async with AsyncExitStack() as stack:
-            task_runner = await stack.enter_async_context(
-                self.flow.task_runner.duplicate().start()
-            )
-            stack.enter_context(
-                FlowRunContext(
-                    flow=self.flow,
-                    log_prints=self.flow.log_prints or False,
-                    flow_run=self.flow_run,
-                    parameters=self.parameters,
-                    client=client,
-                    background_tasks=anyio.create_task_group(),
-                    result_factory=await ResultFactory.from_flow(self.flow),
-                    task_runner=task_runner,
-                )
-            )
-            self.logger = flow_run_logger(flow_run=self.flow_run, flow=self.flow)
-            yield
-
     @contextmanager
-    def enter_run_context_sync(self, client: Optional[PrefectClient] = None):
+    def enter_run_context(self, client: Optional[SyncPrefectClient] = None):
         if client is None:
             client = self.client
         if not self.flow_run:
             raise ValueError("Flow run not set")
 
-        self.flow_run = run_sync(client.read_flow_run(self.flow_run.id))
+        self.flow_run = client.read_flow_run(self.flow_run.id)
 
         # if running in a completely synchronous frame, anyio will not detect the
         # backend to use for the task group
         try:
             task_group = anyio.create_task_group()
         except AsyncLibraryNotFoundError:
             task_group = anyio._backends._asyncio.TaskGroup()
@@ -309,109 +277,90 @@
             flow=self.flow,
             log_prints=self.flow.log_prints or False,
             flow_run=self.flow_run,
             parameters=self.parameters,
             client=client,
             background_tasks=task_group,
             result_factory=run_sync(ResultFactory.from_flow(self.flow)),
-            task_runner=self.flow.task_runner,
+            task_runner=self.flow.task_runner.duplicate(),
         ):
-            self.logger = flow_run_logger(flow_run=self.flow_run, flow=self.flow)
-            yield
+            # set the logger to the flow run logger
+            current_logger = self.logger
+            try:
+                self.logger = flow_run_logger(flow_run=self.flow_run, flow=self.flow)
+                yield
+            finally:
+                self.logger = current_logger
 
-    @asynccontextmanager
-    async def start(self):
+    @contextmanager
+    def start(self):
         """
         Enters a client context and creates a flow run if needed.
         """
-        async with get_client() as client:
+
+        with get_client(sync_client=True) as client:
             self._client = client
             self._is_started = True
 
             # this conditional is engaged whenever a run is triggered via deployment
             if self.flow_run_id and not self.flow:
-                self.flow_run = await client.read_flow_run(self.flow_run_id)
+                self.flow_run = client.read_flow_run(self.flow_run_id)
                 try:
-                    self.flow = await self.load_flow(client)
+                    self.flow = self.load_flow(client)
                 except Exception as exc:
-                    await self.handle_exception(
+                    self.handle_exception(
                         exc,
                         msg="Failed to load flow from entrypoint.",
                     )
                     self.short_circuit = True
 
             if not self.flow_run:
-                self.flow_run = await self.create_flow_run(client)
+                self.flow_run = self.create_flow_run(client)
+                self.logger.debug(f'Created flow run "{self.flow_run.id}"')
 
             # validate prior to context so that context receives validated params
             if self.flow.should_validate_parameters:
                 try:
                     self.parameters = self.flow.validate_parameters(
                         self.parameters or {}
                     )
                 except Exception as exc:
-                    await self.handle_exception(
+                    self.handle_exception(
                         exc,
                         msg="Validation of flow parameters failed with error",
-                        result_factory=await ResultFactory.from_flow(self.flow),
+                        result_factory=run_sync(ResultFactory.from_flow(self.flow)),
                     )
                     self.short_circuit = True
             try:
                 yield self
+            except Exception:
+                # regular exceptions are caught and re-raised to the user
+                raise
+            except (Abort, Pause):
+                raise
+            except BaseException as exc:
+                # BaseExceptions are caught and handled as crashes
+                self.handle_crash(exc)
+                raise
             finally:
                 self._is_started = False
                 self._client = None
 
-    @contextmanager
-    def start_sync(self):
-        """
-        Enters a client context and creates a flow run if needed.
-        """
-
-        client = get_client()
-        run_sync(client.__aenter__())
-        self._client = client
-        self._is_started = True
-
-        if not self.flow_run:
-            self.flow_run = run_sync(self.create_flow_run(client))
-
-        # validate prior to context so that context receives validated params
-        if self.flow.should_validate_parameters:
-            try:
-                self.parameters = self.flow.validate_parameters(self.parameters or {})
-            except Exception as exc:
-                run_sync(
-                    self.handle_exception(
-                        exc,
-                        msg="Validation of flow parameters failed with error",
-                        result_factory=run_sync(ResultFactory.from_flow(self.flow)),
-                    )
-                )
-                self.short_circuit = True
-        try:
-            yield self
-        finally:
-            # quickly close client
-            run_sync(client.__aexit__(None, None, None))
-            self._is_started = False
-            self._client = None
-
     def is_running(self) -> bool:
         if getattr(self, "flow_run", None) is None:
             return False
         return getattr(self, "flow_run").state.is_running()
 
     def is_pending(self) -> bool:
         if getattr(self, "flow_run", None) is None:
             return False  # TODO: handle this differently?
         return getattr(self, "flow_run").state.is_pending()
 
 
-async def run_flow(
+async def run_flow_async(
     flow: Optional[Flow[P, Coroutine[Any, Any, R]]] = None,
     flow_run: Optional[FlowRun] = None,
     flow_run_id: Optional[UUID] = None,
     parameters: Optional[Dict[str, Any]] = None,
     wait_for: Optional[Iterable[PrefectFuture[A, Async]]] = None,
     return_type: Literal["state", "result"] = "result",
 ) -> Union[R, None]:
@@ -420,61 +369,81 @@
 
     We will most likely want to use this logic as a wrapper and return a coroutine for type inference.
     """
 
     engine = FlowRunEngine[P, R](flow, parameters, flow_run, flow_run_id)
 
     # This is a context manager that keeps track of the state of the flow run.
-    async with engine.start() as run:
-        await run.begin_run()
+    with engine.start() as run:
+        run.begin_run()
 
         while run.is_running():
-            async with run.enter_run_context():
+            with run.enter_run_context():
                 try:
                     # This is where the flow is actually run.
                     call_args, call_kwargs = parameters_to_args_kwargs(
                         flow.fn, run.parameters or {}
                     )
                     result = cast(R, await flow.fn(*call_args, **call_kwargs))  # type: ignore
                     # If the flow run is successful, finalize it.
-                    await run.handle_success(result)
+                    run.handle_success(result)
 
                 except Exception as exc:
                     # If the flow fails, and we have retries left, set the flow to retrying.
-                    await run.handle_exception(exc)
+                    run.handle_exception(exc)
 
         if return_type == "state":
             return run.state
-        return await run.result()
+        return run.result()
 
 
 def run_flow_sync(
     flow: Flow[P, R],
     flow_run: Optional[FlowRun] = None,
     parameters: Optional[Dict[str, Any]] = None,
     wait_for: Optional[Iterable[PrefectFuture[A, Async]]] = None,
     return_type: Literal["state", "result"] = "result",
 ) -> Union[R, State, None]:
     engine = FlowRunEngine[P, R](flow, parameters, flow_run)
 
     # This is a context manager that keeps track of the state of the flow run.
-    with engine.start_sync() as run:
-        run_sync(run.begin_run())
+    with engine.start() as run:
+        run.begin_run()
 
         while run.is_running():
-            with run.enter_run_context_sync():
+            with run.enter_run_context():
                 try:
                     # This is where the flow is actually run.
                     call_args, call_kwargs = parameters_to_args_kwargs(
                         flow.fn, run.parameters or {}
                     )
                     result = cast(R, flow.fn(*call_args, **call_kwargs))  # type: ignore
                     # If the flow run is successful, finalize it.
-                    run_sync(run.handle_success(result))
+                    run.handle_success(result)
 
                 except Exception as exc:
                     # If the flow fails, and we have retries left, set the flow to retrying.
-                    run_sync(run.handle_exception(exc))
+                    run.handle_exception(exc)
 
         if return_type == "state":
             return run.state
-        return run_sync(run.result())
+        return run.result()
+
+
+def run_flow(
+    flow: Flow[P, R],
+    flow_run: Optional[FlowRun] = None,
+    parameters: Optional[Dict[str, Any]] = None,
+    wait_for: Optional[Iterable[PrefectFuture[A, Async]]] = None,
+    return_type: Literal["state", "result"] = "result",
+) -> Union[R, State, None]:
+    kwargs = dict(
+        flow=flow,
+        flow_run=flow_run,
+        parameters=parameters,
+        wait_for=wait_for,
+        return_type=return_type,
+    )
+    if flow.isasync:
+        return run_flow_async(**kwargs)
+    else:
+        return run_flow_sync(**kwargs)
```

### Comparing `prefect-client-2.18.3/src/prefect/new_task_engine.py` & `prefect-client-2.19.0/src/prefect/new_task_engine.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,75 @@
-import asyncio
 import inspect
 import logging
-from contextlib import asynccontextmanager, contextmanager
+import time
+from contextlib import contextmanager
 from dataclasses import dataclass, field
 from typing import (
     Any,
     Callable,
     Coroutine,
     Dict,
+    Generator,
     Generic,
     Iterable,
     Literal,
     Optional,
     TypeVar,
     Union,
     cast,
 )
-from uuid import uuid4
 
 import pendulum
 from typing_extensions import ParamSpec
 
 from prefect import Task, get_client
-from prefect._internal.concurrency.cancellation import (
-    AlarmCancelScope,
-    AsyncCancelScope,
-    CancelledError,
-)
-from prefect.client.orchestration import PrefectClient
+from prefect.client.orchestration import SyncPrefectClient
 from prefect.client.schemas import TaskRun
-from prefect.client.schemas.objects import TaskRunResult
 from prefect.context import FlowRunContext, TaskRunContext
 from prefect.futures import PrefectFuture, resolve_futures_to_states
 from prefect.logging.loggers import get_logger, task_run_logger
 from prefect.results import ResultFactory
 from prefect.server.schemas.states import State
 from prefect.settings import PREFECT_TASKS_REFRESH_CACHE
 from prefect.states import (
-    Pending,
     Retrying,
     Running,
     StateDetails,
     exception_to_crashed_state,
     exception_to_failed_state,
     return_value_to_state,
 )
-from prefect.utilities.asyncutils import A, Async, is_async_fn, run_sync
+from prefect.utilities.asyncutils import A, Async, run_sync
 from prefect.utilities.callables import parameters_to_args_kwargs
 from prefect.utilities.engine import (
-    _dynamic_key_for_task_run,
     _get_hook_name,
-    _resolve_custom_task_run_name,
-    collect_task_run_inputs,
-    propose_state,
+    propose_state_sync,
 )
+from prefect.utilities.timeout import timeout, timeout_async
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
-@asynccontextmanager
-async def timeout(seconds: Optional[float] = None):
-    try:
-        with AsyncCancelScope(timeout=seconds):
-            yield
-    except CancelledError:
-        raise TimeoutError(f"Task timed out after {seconds} second(s).")
-
-
-@contextmanager
-def timeout_sync(seconds: Optional[float] = None):
-    try:
-        with AlarmCancelScope(timeout=seconds):
-            yield
-    except CancelledError:
-        raise TimeoutError(f"Task timed out after {seconds} second(s).")
-
-
 @dataclass
 class TaskRunEngine(Generic[P, R]):
     task: Union[Task[P, R], Task[P, Coroutine[Any, Any, R]]]
     logger: logging.Logger = field(default_factory=lambda: get_logger("engine"))
     parameters: Optional[Dict[str, Any]] = None
     task_run: Optional[TaskRun] = None
     retries: int = 0
     _is_started: bool = False
-    _client: Optional[PrefectClient] = None
+    _client: Optional[SyncPrefectClient] = None
 
     def __post_init__(self):
         if self.parameters is None:
             self.parameters = {}
 
     @property
-    def client(self) -> PrefectClient:
+    def client(self) -> SyncPrefectClient:
         if not self._is_started or self._client is None:
             raise RuntimeError("Engine has not started.")
         return self._client
 
     @property
     def state(self) -> State:
         if not self.task_run:
@@ -110,52 +83,63 @@
         ] = self.task.retry_condition_fn
         if not self.task_run:
             raise ValueError("Task run is not set")
         return not retry_condition or retry_condition(
             self.task, self.task_run, self.state
         )
 
-    async def _run_hooks(self, state: State) -> None:
-        """Run the on_failure and on_completion hooks for a task, making sure to
-        catch and log any errors that occur.
-        """
+    def get_hooks(self, state: State, as_async: bool = False) -> Iterable[Callable]:
         task = self.task
         task_run = self.task_run
 
         if not task_run:
             raise ValueError("Task run is not set")
 
         hooks = None
         if state.is_failed() and task.on_failure:
             hooks = task.on_failure
         elif state.is_completed() and task.on_completion:
             hooks = task.on_completion
 
-        if hooks:
-            for hook in hooks:
-                hook_name = _get_hook_name(hook)
+        for hook in hooks or []:
+            hook_name = _get_hook_name(hook)
+
+            @contextmanager
+            def hook_context():
                 try:
                     self.logger.info(
                         f"Running hook {hook_name!r} in response to entering state"
                         f" {state.name!r}"
                     )
-                    if is_async_fn(hook):
-                        await hook(task, task_run, state)
-                    else:
-                        hook(task, task_run, state)
+                    yield
                 except Exception:
                     self.logger.error(
                         f"An error was encountered while running hook {hook_name!r}",
                         exc_info=True,
                     )
                 else:
                     self.logger.info(
                         f"Hook {hook_name!r} finished running successfully"
                     )
 
+            if as_async:
+
+                async def _hook_fn():
+                    with hook_context():
+                        result = hook(task, task_run, state)
+                        if inspect.isawaitable(result):
+                            await result
+            else:
+
+                def _hook_fn():
+                    with hook_context():
+                        hook(task, task_run, state)
+
+            yield _hook_fn
+
     def _compute_state_details(
         self, include_cache_expiration: bool = False
     ) -> StateDetails:
         ## setup cache metadata
         task_run_context = TaskRunContext.get()
         cache_key = (
             self.task.cache_key_fn(
@@ -183,221 +167,148 @@
             cache_expiration = None
         return StateDetails(
             cache_key=cache_key,
             refresh_cache=refresh_cache,
             cache_expiration=cache_expiration,
         )
 
-    async def begin_run(self):
+    def begin_run(self):
         state_details = self._compute_state_details()
         new_state = Running(state_details=state_details)
-        state = await self.set_state(new_state)
+        state = self.set_state(new_state)
         while state.is_pending():
-            await asyncio.sleep(1)
-            state = await self.set_state(new_state)
+            time.sleep(0.2)
+            state = self.set_state(new_state)
 
-    async def set_state(self, state: State, force: bool = False) -> State:
+    def set_state(self, state: State, force: bool = False) -> State:
         if not self.task_run:
             raise ValueError("Task run is not set")
-        new_state = await propose_state(
+        new_state = propose_state_sync(
             self.client, state, task_run_id=self.task_run.id, force=force
-        )  # type: ignore
+        )
+        # type: ignore
 
         # currently this is a hack to keep a reference to the state object
         # that has an in-memory result attached to it; using the API state
         # could result in losing that reference
         self.task_run.state = new_state
-        if new_state.is_final():
-            await self._run_hooks(new_state)
         return new_state
 
-    async def result(self, raise_on_failure: bool = True) -> "Union[R, State, None]":
+    def result(self, raise_on_failure: bool = True) -> "Union[R, State, None]":
         _result = self.state.result(raise_on_failure=raise_on_failure, fetch=True)
         # state.result is a `sync_compatible` function that may or may not return an awaitable
         # depending on whether the parent frame is sync or not
         if inspect.isawaitable(_result):
-            _result = await _result
+            _result = run_sync(_result)
         return _result
 
-    async def handle_success(self, result: R) -> R:
+    def handle_success(self, result: R) -> R:
         result_factory = getattr(TaskRunContext.get(), "result_factory", None)
         if result_factory is None:
             raise ValueError("Result factory is not set")
-        terminal_state = await return_value_to_state(
-            await resolve_futures_to_states(result),
-            result_factory=result_factory,
+        terminal_state = run_sync(
+            return_value_to_state(
+                run_sync(resolve_futures_to_states(result)),
+                result_factory=result_factory,
+            )
         )
         terminal_state.state_details = self._compute_state_details(
             include_cache_expiration=True
         )
-        await self.set_state(terminal_state)
+        self.set_state(terminal_state)
         return result
 
-    async def handle_retry(self, exc: Exception) -> bool:
+    def handle_retry(self, exc: Exception) -> bool:
         """
         If the task has retries left, and the retry condition is met, set the task to retrying.
         - If the task has no retries left, or the retry condition is not met, return False.
         - If the task has retries left, and the retry condition is met, return True.
         """
         if self.retries < self.task.retries and self.can_retry:
-            await self.set_state(Retrying(), force=True)
+            self.set_state(Retrying(), force=True)
             self.retries = self.retries + 1
             return True
         return False
 
-    async def handle_exception(self, exc: Exception) -> None:
+    def handle_exception(self, exc: Exception) -> None:
         # If the task fails, and we have retries left, set the task to retrying.
-        if not await self.handle_retry(exc):
+        if not self.handle_retry(exc):
             # If the task has no retries left, or the retry condition is not met, set the task to failed.
             context = TaskRunContext.get()
-            state = await exception_to_failed_state(
-                exc,
-                message="Task run encountered an exception",
-                result_factory=getattr(context, "result_factory", None),
+            state = run_sync(
+                exception_to_failed_state(
+                    exc,
+                    message="Task run encountered an exception",
+                    result_factory=getattr(context, "result_factory", None),
+                )
             )
-            await self.set_state(state)
+            self.set_state(state)
 
-    async def handle_crash(self, exc: BaseException) -> None:
-        state = await exception_to_crashed_state(exc)
+    def handle_crash(self, exc: BaseException) -> None:
+        state = run_sync(exception_to_crashed_state(exc))
         self.logger.error(f"Crash detected! {state.message}")
         self.logger.debug("Crash details:", exc_info=exc)
-        await self.set_state(state, force=True)
-
-    async def create_task_run(self, client: PrefectClient) -> TaskRun:
-        flow_run_ctx = FlowRunContext.get()
-        parameters = self.parameters or {}
-        try:
-            task_run_name = _resolve_custom_task_run_name(self.task, parameters)
-        except TypeError:
-            task_run_name = None
-
-        # prep input tracking
-        task_inputs = {
-            k: await collect_task_run_inputs(v) for k, v in parameters.items()
-        }
-
-        # anticipate nested runs
-        task_run_ctx = TaskRunContext.get()
-        if task_run_ctx:
-            task_inputs["wait_for"] = [TaskRunResult(id=task_run_ctx.task_run.id)]  # type: ignore
-
-        # TODO: implement wait_for
-        #        if wait_for:
-        #            task_inputs["wait_for"] = await collect_task_run_inputs(wait_for)
-
-        if flow_run_ctx:
-            dynamic_key = _dynamic_key_for_task_run(
-                context=flow_run_ctx, task=self.task
-            )
-        else:
-            dynamic_key = uuid4().hex
-        task_run = await client.create_task_run(
-            task=self.task,  # type: ignore
-            name=task_run_name,
-            flow_run_id=(
-                getattr(flow_run_ctx.flow_run, "id", None)
-                if flow_run_ctx and flow_run_ctx.flow_run
-                else None
-            ),
-            dynamic_key=str(dynamic_key),
-            state=Pending(),
-            task_inputs=task_inputs,  # type: ignore
-        )
-        return task_run
-
-    @asynccontextmanager
-    async def enter_run_context(self, client: Optional[PrefectClient] = None):
-        if client is None:
-            client = self.client
-
-        if not self.task_run:
-            raise ValueError("Task run is not set")
-
-        self.task_run = await client.read_task_run(self.task_run.id)
-
-        with TaskRunContext(
-            task=self.task,
-            log_prints=self.task.log_prints or False,
-            task_run=self.task_run,
-            parameters=self.parameters,
-            result_factory=await ResultFactory.from_autonomous_task(self.task),  # type: ignore
-            client=client,
-        ):
-            self.logger = task_run_logger(task_run=self.task_run, task=self.task)  # type: ignore
-            yield
+        self.set_state(state, force=True)
 
     @contextmanager
-    def enter_run_context_sync(self, client: Optional[PrefectClient] = None):
+    def enter_run_context(self, client: Optional[SyncPrefectClient] = None):
         if client is None:
             client = self.client
         if not self.task_run:
             raise ValueError("Task run is not set")
 
-        self.task_run = run_sync(client.read_task_run(self.task_run.id))
+        self.task_run = client.read_task_run(self.task_run.id)
 
         with TaskRunContext(
             task=self.task,
             log_prints=self.task.log_prints or False,
             task_run=self.task_run,
             parameters=self.parameters,
             result_factory=run_sync(ResultFactory.from_autonomous_task(self.task)),  # type: ignore
             client=client,
         ):
-            self.logger = task_run_logger(task_run=self.task_run, task=self.task)  # type: ignore
-            yield
+            # set the logger to the task run logger
+            current_logger = self.logger
+            try:
+                self.logger = task_run_logger(task_run=self.task_run, task=self.task)  # type: ignore
+                yield
+            finally:
+                self.logger = current_logger
 
-    @asynccontextmanager
-    async def start(self):
+    @contextmanager
+    def start(self) -> Generator["TaskRunEngine", Any, Any]:
         """
         Enters a client context and creates a task run if needed.
         """
-        async with get_client() as client:
+        with get_client(sync_client=True) as client:
             self._client = client
             self._is_started = True
             try:
                 if not self.task_run:
-                    self.task_run = await self.create_task_run(client)
+                    self.task_run = run_sync(
+                        self.task.create_run(
+                            client=client,
+                            parameters=self.parameters,
+                            flow_run_context=FlowRunContext.get(),
+                            parent_task_run_context=TaskRunContext.get(),
+                        )
+                    )
+
                 yield self
             except Exception:
                 # regular exceptions are caught and re-raised to the user
                 raise
             except BaseException as exc:
                 # BaseExceptions are caught and handled as crashes
-                await self.handle_crash(exc)
+                self.handle_crash(exc)
                 raise
             finally:
                 self._is_started = False
                 self._client = None
 
-    @contextmanager
-    def start_sync(self):
-        """
-        Enters a client context and creates a task run if needed.
-        """
-        client = get_client()
-        run_sync(client.__aenter__())
-        self._client = client
-        self._is_started = True
-        try:
-            if not self.task_run:
-                self.task_run = run_sync(self.create_task_run(client))
-            yield self
-        except Exception:
-            # regular exceptions are caught and re-raised to the user
-            raise
-        except BaseException as exc:
-            # BaseExceptions are caught and handled as crashes
-            run_sync(self.handle_crash(exc))
-            raise
-        finally:
-            # quickly close client
-            run_sync(client.__aexit__(None, None, None))
-            self._is_started = False
-            self._client = None
-
     async def get_client(self):
         if not self._is_started:
             raise RuntimeError("Engine has not started.")
         else:
             return self._client
 
     def is_running(self) -> bool:
@@ -407,82 +318,106 @@
 
     def is_pending(self) -> bool:
         if getattr(self, "task_run", None) is None:
             return False  # TODO: handle this differently?
         return getattr(self, "task_run").state.is_pending()
 
 
-async def run_task(
-    task: Task[P, Coroutine[Any, Any, R]],
+def run_task_sync(
+    task: Task[P, R],
     task_run: Optional[TaskRun] = None,
     parameters: Optional[Dict[str, Any]] = None,
     wait_for: Optional[Iterable[PrefectFuture[A, Async]]] = None,
     return_type: Literal["state", "result"] = "result",
 ) -> Union[R, State, None]:
-    """
-    Runs a task against the API.
-
-    We will most likely want to use this logic as a wrapper and return a coroutine for type inference.
-    """
     engine = TaskRunEngine[P, R](task=task, parameters=parameters, task_run=task_run)
 
     # This is a context manager that keeps track of the run of the task run.
-    async with engine.start() as run:
-        await run.begin_run()
+    with engine.start() as run:
+        run.begin_run()
 
         while run.is_running():
-            async with run.enter_run_context():
+            with run.enter_run_context():
                 try:
                     # This is where the task is actually run.
-                    async with timeout(seconds=run.task.timeout_seconds):
+                    with timeout(seconds=run.task.timeout_seconds):
                         call_args, call_kwargs = parameters_to_args_kwargs(
                             task.fn, run.parameters or {}
                         )
-                        result = cast(R, await task.fn(*call_args, **call_kwargs))  # type: ignore
+                        result = cast(R, task.fn(*call_args, **call_kwargs))  # type: ignore
 
                     # If the task run is successful, finalize it.
-                    await run.handle_success(result)
-                    if return_type == "result":
-                        return result
+                    run.handle_success(result)
 
                 except Exception as exc:
-                    await run.handle_exception(exc)
+                    run.handle_exception(exc)
+
+        if run.state.is_final():
+            for hook in run.get_hooks(run.state):
+                hook()
 
         if return_type == "state":
             return run.state
-        return await run.result()
+        return run.result()
 
 
-def run_task_sync(
-    task: Task[P, R],
+async def run_task_async(
+    task: Task[P, Coroutine[Any, Any, R]],
     task_run: Optional[TaskRun] = None,
     parameters: Optional[Dict[str, Any]] = None,
     wait_for: Optional[Iterable[PrefectFuture[A, Async]]] = None,
     return_type: Literal["state", "result"] = "result",
 ) -> Union[R, State, None]:
+    """
+    Runs a task against the API.
+
+    We will most likely want to use this logic as a wrapper and return a coroutine for type inference.
+    """
     engine = TaskRunEngine[P, R](task=task, parameters=parameters, task_run=task_run)
 
     # This is a context manager that keeps track of the run of the task run.
-    with engine.start_sync() as run:
-        run_sync(run.begin_run())
+    with engine.start() as run:
+        run.begin_run()
 
         while run.is_running():
-            with run.enter_run_context_sync():
+            with run.enter_run_context():
                 try:
                     # This is where the task is actually run.
-                    with timeout_sync(seconds=run.task.timeout_seconds):
+                    with timeout_async(seconds=run.task.timeout_seconds):
                         call_args, call_kwargs = parameters_to_args_kwargs(
                             task.fn, run.parameters or {}
                         )
-                        result = cast(R, task.fn(*call_args, **call_kwargs))  # type: ignore
+                        result = cast(R, await task.fn(*call_args, **call_kwargs))  # type: ignore
 
                     # If the task run is successful, finalize it.
-                    run_sync(run.handle_success(result))
-                    if return_type == "result":
-                        return result
+                    run.handle_success(result)
 
                 except Exception as exc:
-                    run_sync(run.handle_exception(exc))
+                    run.handle_exception(exc)
+
+        if run.state.is_final():
+            for hook in run.get_hooks(run.state, as_async=True):
+                await hook()
 
         if return_type == "state":
             return run.state
-        return run_sync(run.result())
+        return run.result()
+
+
+def run_task(
+    task: Task[P, R],
+    task_run: Optional[TaskRun] = None,
+    parameters: Optional[Dict[str, Any]] = None,
+    wait_for: Optional[Iterable[PrefectFuture[A, Async]]] = None,
+    return_type: Literal["state", "result"] = "result",
+) -> Union[R, State, None]:
+    kwargs = dict(
+        task=task,
+        task_run=task_run,
+        parameters=parameters,
+        wait_for=wait_for,
+        return_type=return_type,
+    )
+    if task.isasync:
+        return run_task_async(**kwargs)
+    else:
+        return run_task_sync(**kwargs)
```

### Comparing `prefect-client-2.18.3/src/prefect/plugins.py` & `prefect-client-2.19.0/src/prefect/plugins.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/pydantic/__init__.py` & `prefect-client-2.19.0/src/prefect/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/pydantic/main.py` & `prefect-client-2.19.0/src/prefect/pydantic/main.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/results.py` & `prefect-client-2.19.0/src/prefect/results.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/runner/runner.py` & `prefect-client-2.19.0/src/prefect/runner/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,14 @@
 from pathlib import Path
 from typing import Callable, Dict, Iterable, List, Optional, Set, Union
 from uuid import UUID, uuid4
 
 import anyio
 import anyio.abc
 import pendulum
-import sniffio
-from rich.console import Console, Group
-from rich.table import Table
 
 from prefect._internal.concurrency.api import (
     create_call,
     from_async,
     from_sync,
 )
 from prefect.client.orchestration import get_client
@@ -76,41 +73,40 @@
 from prefect.client.schemas.schedules import SCHEDULE_TYPES
 from prefect.deployments.deployments import load_flow_from_flow_run
 from prefect.deployments.runner import (
     EntrypointType,
     RunnerDeployment,
 )
 from prefect.deployments.schedules import FlexibleScheduleList
-from prefect.engine import propose_state
 from prefect.events import DeploymentTriggerTypes, TriggerTypes
 from prefect.exceptions import (
     Abort,
 )
 from prefect.flows import Flow
 from prefect.logging.loggers import PrefectLogAdapter, flow_run_logger, get_logger
 from prefect.runner.server import start_webserver
 from prefect.runner.storage import RunnerStorage
 from prefect.settings import (
     PREFECT_API_URL,
     PREFECT_RUNNER_POLL_FREQUENCY,
     PREFECT_RUNNER_PROCESS_LIMIT,
     PREFECT_RUNNER_SERVER_ENABLE,
-    PREFECT_UI_URL,
     get_current_settings,
 )
 from prefect.states import Crashed, Pending, exception_to_failed_state
 from prefect.utilities.asyncutils import (
     asyncnullcontext,
     is_async_fn,
     sync_compatible,
 )
+from prefect.utilities.engine import propose_state
 from prefect.utilities.processutils import _register_signal, run_process
 from prefect.utilities.services import critical_service_loop
 
-__all__ = ["Runner", "serve"]
+__all__ = ["Runner"]
 
 
 class Runner:
     def __init__(
         self,
         name: Optional[str] = None,
         query_seconds: Optional[float] = None,
@@ -546,15 +542,14 @@
         # We must add creationflags to a dict so it is only passed as a function
         # parameter on Windows, because the presence of creationflags causes
         # errors on Unix even if set to None
         kwargs: Dict[str, object] = {}
         if sys.platform == "win32":
             kwargs["creationflags"] = subprocess.CREATE_NEW_PROCESS_GROUP
 
-        _use_threaded_child_watcher()
         flow_run_logger.info("Opening process...")
 
         env = get_current_settings().to_environment_variables(exclude_unset=True)
         env.update(
             {
                 **{
                     "PREFECT__FLOW_RUN_ID": str(flow_run.id),
@@ -1186,114 +1181,14 @@
 
 
 if sys.platform == "win32":
     # exit code indicating that the process was terminated by Ctrl+C or Ctrl+Break
     STATUS_CONTROL_C_EXIT = 0xC000013A
 
 
-def _use_threaded_child_watcher():
-    if (
-        sys.version_info < (3, 8)
-        and sniffio.current_async_library() == "asyncio"
-        and sys.platform != "win32"
-    ):
-        from prefect.utilities.compat import ThreadedChildWatcher
-
-        # Python < 3.8 does not use a `ThreadedChildWatcher` by default which can
-        # lead to errors in tests on unix as the previous default `SafeChildWatcher`
-        # is not compatible with threaded event loops.
-        asyncio.get_event_loop_policy().set_child_watcher(ThreadedChildWatcher())
-
-
-@sync_compatible
-async def serve(
-    *args: RunnerDeployment,
-    pause_on_shutdown: bool = True,
-    print_starting_message: bool = True,
-    limit: Optional[int] = None,
-    **kwargs,
-):
-    """
-    Serve the provided list of deployments.
-
-    Args:
-        *args: A list of deployments to serve.
-        pause_on_shutdown: A boolean for whether or not to automatically pause
-            deployment schedules on shutdown.
-        print_starting_message: Whether or not to print message to the console
-            on startup.
-        limit: The maximum number of runs that can be executed concurrently.
-        **kwargs: Additional keyword arguments to pass to the runner.
-
-    Examples:
-        Prepare two deployments and serve them:
-
-        ```python
-        import datetime
-
-        from prefect import flow, serve
-
-        @flow
-        def my_flow(name):
-            print(f"hello {name}")
-
-        @flow
-        def my_other_flow(name):
-            print(f"goodbye {name}")
-
-        if __name__ == "__main__":
-            # Run once a day
-            hello_deploy = my_flow.to_deployment(
-                "hello", tags=["dev"], interval=datetime.timedelta(days=1)
-            )
-
-            # Run every Sunday at 4:00 AM
-            bye_deploy = my_other_flow.to_deployment(
-                "goodbye", tags=["dev"], cron="0 4 * * sun"
-            )
-
-            serve(hello_deploy, bye_deploy)
-        ```
-    """
-    runner = Runner(pause_on_shutdown=pause_on_shutdown, limit=limit, **kwargs)
-    for deployment in args:
-        await runner.add_deployment(deployment)
-
-    if print_starting_message:
-        help_message_top = (
-            "[green]Your deployments are being served and polling for"
-            " scheduled runs!\n[/]"
-        )
-
-        table = Table(title="Deployments", show_header=False)
-
-        table.add_column(style="blue", no_wrap=True)
-
-        for deployment in args:
-            table.add_row(f"{deployment.flow_name}/{deployment.name}")
-
-        help_message_bottom = (
-            "\nTo trigger any of these deployments, use the"
-            " following command:\n[blue]\n\t$ prefect deployment run"
-            " [DEPLOYMENT_NAME]\n[/]"
-        )
-        if PREFECT_UI_URL:
-            help_message_bottom += (
-                "\nYou can also trigger your deployments via the Prefect UI:"
-                f" [blue]{PREFECT_UI_URL.value()}/deployments[/]\n"
-            )
-
-        console = Console()
-        console.print(
-            Group(help_message_top, table, help_message_bottom), soft_wrap=True
-        )
-
-    await runner.start()
-
-
 async def _run_hooks(
     hooks: List[Callable[[Flow, "FlowRun", State], None]], flow_run, flow, state
 ):
     logger = flow_run_logger(flow_run, flow)
     for hook in hooks:
         try:
             logger.info(
```

### Comparing `prefect-client-2.18.3/src/prefect/runner/server.py` & `prefect-client-2.19.0/src/prefect/runner/server.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/runner/storage.py` & `prefect-client-2.19.0/src/prefect/runner/storage.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/runner/submit.py` & `prefect-client-2.19.0/src/prefect/runner/submit.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/runner/utils.py` & `prefect-client-2.19.0/src/prefect/runner/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/runtime/deployment.py` & `prefect-client-2.19.0/src/prefect/runtime/deployment.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/runtime/flow_run.py` & `prefect-client-2.19.0/src/prefect/runtime/flow_run.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/runtime/task_run.py` & `prefect-client-2.19.0/src/prefect/runtime/task_run.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/serializers.py` & `prefect-client-2.19.0/src/prefect/serializers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json` & `prefect-client-2.19.0/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/server/api/static/prefect-logo-mark-gradient.png` & `prefect-client-2.19.0/src/prefect/server/api/static/prefect-logo-mark-gradient.png`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/settings.py` & `prefect-client-2.19.0/src/prefect/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1497,14 +1497,19 @@
 """
 
 PREFECT_RUNNER_SERVER_ENABLE = Setting(bool, default=False)
 """
 Whether or not to enable the runner's webserver.
 """
 
+PREFECT_DEPLOYMENT_SCHEDULE_MAX_SCHEDULED_RUNS = Setting(int, default=50)
+"""
+The maximum number of scheduled runs to create for a deployment.
+"""
+
 PREFECT_WORKER_HEARTBEAT_SECONDS = Setting(float, default=30)
 """
 Number of seconds a worker should wait between sending a heartbeat.
 """
 
 PREFECT_WORKER_QUERY_SECONDS = Setting(float, default=10)
 """
@@ -1610,14 +1615,19 @@
 """
 
 PREFECT_EXPERIMENTAL_ENABLE_NEW_ENGINE = Setting(bool, default=False)
 """
 Whether or not to enable experimental new engine.
 """
 
+PREFECT_EXPERIMENTAL_DISABLE_SYNC_COMPAT = Setting(bool, default=False)
+"""
+Whether or not to disable the sync_compatible decorator utility.
+"""
+
 
 # Defaults -----------------------------------------------------------------------------
 
 PREFECT_DEFAULT_RESULT_STORAGE_BLOCK = Setting(
     str,
     default=None,
 )
@@ -1741,14 +1751,15 @@
 PREFECT_API_EVENTS_RELATED_RESOURCE_CACHE_TTL = Setting(
     timedelta, default=timedelta(minutes=5)
 )
 """
 How long to cache related resource data for emitting server-side vents
 """
 
+
 # Deprecated settings ------------------------------------------------------------------
 
 
 # Collect all defined settings ---------------------------------------------------------
 
 SETTING_VARIABLES: Dict[str, Any] = {
     name: val for name, val in tuple(globals().items()) if isinstance(val, Setting)
```

### Comparing `prefect-client-2.18.3/src/prefect/software/base.py` & `prefect-client-2.19.0/src/prefect/software/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/software/conda.py` & `prefect-client-2.19.0/src/prefect/software/conda.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/software/pip.py` & `prefect-client-2.19.0/src/prefect/software/pip.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/software/python.py` & `prefect-client-2.19.0/src/prefect/software/python.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/states.py` & `prefect-client-2.19.0/src/prefect/states.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/task_engine.py` & `prefect-client-2.19.0/src/prefect/task_engine.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/task_runners.py` & `prefect-client-2.19.0/src/prefect/task_runners.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/task_server.py` & `prefect-client-2.19.0/src/prefect/task_server.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/tasks.py` & `prefect-client-2.19.0/src/prefect/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 # This file requires type-checking with pyright because mypy does not yet support PEP612
 # See https://github.com/python/mypy/issues/8645
 
 import datetime
 import inspect
 import os
-import warnings
 from copy import copy
 from functools import partial, update_wrapper
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
@@ -29,17 +28,23 @@
     overload,
 )
 from uuid import uuid4
 
 from typing_extensions import Literal, ParamSpec
 
 from prefect._internal.concurrency.api import create_call, from_async, from_sync
+from prefect.client.orchestration import PrefectClient, SyncPrefectClient
 from prefect.client.schemas import TaskRun
-from prefect.client.schemas.objects import TaskRunInput
-from prefect.context import FlowRunContext, PrefectObjectRegistry, TagsContext
+from prefect.client.schemas.objects import TaskRunInput, TaskRunResult
+from prefect.context import (
+    FlowRunContext,
+    PrefectObjectRegistry,
+    TagsContext,
+    TaskRunContext,
+)
 from prefect.futures import PrefectFuture
 from prefect.logging.loggers import get_logger, get_run_logger
 from prefect.results import ResultSerializer, ResultStorage
 from prefect.settings import (
     PREFECT_EXPERIMENTAL_ENABLE_NEW_ENGINE,
     PREFECT_EXPERIMENTAL_ENABLE_TASK_SCHEDULING,
     PREFECT_TASK_DEFAULT_RETRIES,
@@ -328,41 +333,15 @@
 
         self.retry_jitter_factor = retry_jitter_factor
         self.persist_result = persist_result
         self.result_storage = result_storage
         self.result_serializer = result_serializer
         self.result_storage_key = result_storage_key
         self.cache_result_in_memory = cache_result_in_memory
-
         self.timeout_seconds = float(timeout_seconds) if timeout_seconds else None
-        # Warn if this task's `name` conflicts with another task while having a
-        # different function. This is to detect the case where two or more tasks
-        # share a name or are lambdas, which should result in a warning, and to
-        # differentiate it from the case where the task was 'copied' via
-        # `with_options`, which should not result in a warning.
-        registry = PrefectObjectRegistry.get()
-
-        if registry and any(
-            other
-            for other in registry.get_instances(Task)
-            if other.name == self.name and id(other.fn) != id(self.fn)
-        ):
-            try:
-                file = inspect.getsourcefile(self.fn)
-                line_number = inspect.getsourcelines(self.fn)[1]
-            except TypeError:
-                file = "unknown"
-                line_number = "unknown"
-
-            warnings.warn(
-                f"A task named {self.name!r} and defined at '{file}:{line_number}' "
-                "conflicts with another task. Consider specifying a unique `name` "
-                "parameter in the task definition:\n\n "
-                "`@task(name='my_unique_name', ...)`"
-            )
         self.on_completion = on_completion
         self.on_failure = on_failure
 
         # retry_condition_fn must be a callable or None. If it is neither, raise a TypeError
         if retry_condition_fn is not None and not (callable(retry_condition_fn)):
             raise TypeError(
                 "Expected `retry_condition_fn` to be callable, got"
@@ -535,56 +514,101 @@
             on_failure=on_failure or self.on_failure,
             retry_condition_fn=retry_condition_fn or self.retry_condition_fn,
             viz_return_value=viz_return_value or self.viz_return_value,
         )
 
     async def create_run(
         self,
-        flow_run_context: FlowRunContext,
-        parameters: Dict[str, Any],
-        wait_for: Optional[Iterable[PrefectFuture]],
+        client: Optional[Union[PrefectClient, SyncPrefectClient]],
+        parameters: Dict[str, Any] = None,
+        flow_run_context: Optional[FlowRunContext] = None,
+        parent_task_run_context: Optional[TaskRunContext] = None,
+        wait_for: Optional[Iterable[PrefectFuture]] = None,
         extra_task_inputs: Optional[Dict[str, Set[TaskRunInput]]] = None,
     ) -> TaskRun:
-        # TODO: Investigate if we can replace create_task_run on the task run engine
-        # with this method. Would require updating to work without the flow run context.
         from prefect.utilities.engine import (
             _dynamic_key_for_task_run,
+            _resolve_custom_task_run_name,
             collect_task_run_inputs,
         )
 
-        dynamic_key = _dynamic_key_for_task_run(flow_run_context, self)
+        if flow_run_context is None:
+            flow_run_context = FlowRunContext.get()
+        if parent_task_run_context is None:
+            parent_task_run_context = TaskRunContext.get()
+        if parameters is None:
+            parameters = {}
+
+        try:
+            task_run_name = _resolve_custom_task_run_name(self, parameters)
+        except TypeError:
+            task_run_name = None
+
+        if flow_run_context:
+            dynamic_key = _dynamic_key_for_task_run(context=flow_run_context, task=self)
+        else:
+            dynamic_key = uuid4().hex
+
+        # collect task inputs
         task_inputs = {
             k: await collect_task_run_inputs(v) for k, v in parameters.items()
         }
+
+        # check if this task has a parent task run based on running in another
+        # task run's existing context. A task run is only considered a parent if
+        # it is in the same flow run (because otherwise presumably the child is
+        # in a subflow, so the subflow serves as the parent) or if there is no
+        # flow run
+        if parent_task_run_context:
+            # there is no flow run
+            if not flow_run_context:
+                task_inputs["__parents__"] = [
+                    TaskRunResult(id=parent_task_run_context.task_run.id)
+                ]
+            # there is a flow run and the task run is in the same flow run
+            elif (
+                flow_run_context
+                and parent_task_run_context.task_run.flow_run_id
+                == flow_run_context.flow_run.id
+            ):
+                task_inputs["__parents__"] = [
+                    TaskRunResult(id=parent_task_run_context.task_run.id)
+                ]
+
         if wait_for:
             task_inputs["wait_for"] = await collect_task_run_inputs(wait_for)
 
         # Join extra task inputs
-        extra_task_inputs = extra_task_inputs or {}
-        for k, extras in extra_task_inputs.items():
+        for k, extras in (extra_task_inputs or {}).items():
             task_inputs[k] = task_inputs[k].union(extras)
 
-        flow_run_logger = get_run_logger(flow_run_context)
-
-        task_run = await flow_run_context.client.create_task_run(
+        # create the task run
+        task_run = client.create_task_run(
             task=self,
-            name=f"{self.name} - {dynamic_key}",
-            flow_run_id=flow_run_context.flow_run.id,
-            dynamic_key=dynamic_key,
+            name=task_run_name,
+            flow_run_id=(
+                getattr(flow_run_context.flow_run, "id", None)
+                if flow_run_context and flow_run_context.flow_run
+                else None
+            ),
+            dynamic_key=str(dynamic_key),
             state=Pending(),
-            extra_tags=TagsContext.get().current_tags,
             task_inputs=task_inputs,
+            extra_tags=TagsContext.get().current_tags,
         )
+        # the new engine uses sync clients but old engines use async clients
+        if inspect.isawaitable(task_run):
+            task_run = await task_run
 
-        if flow_run_context.flow_run:
-            flow_run_logger.info(
+        if flow_run_context and flow_run_context.flow_run:
+            get_run_logger(flow_run_context).debug(
                 f"Created task run {task_run.name!r} for task {self.name!r}"
             )
         else:
-            logger.info(f"Created task run {task_run.name!r} for task {self.name!r}")
+            logger.debug(f"Created task run {task_run.name!r} for task {self.name!r}")
 
         return task_run
 
     @overload
     def __call__(
         self: "Task[P, NoReturn]",
         *args: P.args,
@@ -633,29 +657,23 @@
 
         task_run_tracker = get_task_viz_tracker()
         if task_run_tracker:
             return track_viz_task(
                 self.isasync, self.name, parameters, self.viz_return_value
             )
 
-        # new engine currently only compatible with async tasks
         if PREFECT_EXPERIMENTAL_ENABLE_NEW_ENGINE.value():
-            from prefect.new_task_engine import run_task, run_task_sync
+            from prefect.new_task_engine import run_task
 
-            run_kwargs = dict(
+            return run_task(
                 task=self,
                 parameters=parameters,
                 wait_for=wait_for,
                 return_type=return_type,
             )
-            if self.isasync:
-                # this returns an awaitable coroutine
-                return run_task(**run_kwargs)
-            else:
-                return run_task_sync(**run_kwargs)
 
         if (
             PREFECT_EXPERIMENTAL_ENABLE_TASK_SCHEDULING.value()
             and not FlowRunContext.get()
         ):
             from prefect import get_client
 
@@ -927,19 +945,20 @@
     async def _submit_async(
         self,
         parameters: Dict[str, Any],
         flow_run_context: FlowRunContext,
         wait_for: Optional[Iterable[PrefectFuture]],
         return_state: bool,
     ):
-        from prefect.new_task_engine import run_task
+        from prefect.new_task_engine import run_task_async
 
         task_runner = flow_run_context.task_runner
 
         task_run = await self.create_run(
+            client=flow_run_context.client,
             flow_run_context=flow_run_context,
             parameters=parameters,
             wait_for=wait_for,
         )
 
         future = PrefectFuture(
             name=task_run.name,
@@ -948,15 +967,15 @@
             asynchronous=(self.isasync and flow_run_context.flow.isasync),
         )
         future.task_run = task_run
         flow_run_context.task_run_futures.append(future)
         await task_runner.submit(
             key=future.key,
             call=partial(
-                run_task,
+                run_task_async,
                 task=self,
                 task_run=task_run,
                 parameters=parameters,
                 wait_for=wait_for,
                 return_type="state",
             ),
         )
```

### Comparing `prefect-client-2.18.3/src/prefect/types/__init__.py` & `prefect-client-2.19.0/src/prefect/types/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from dataclasses import dataclass
 from typing import Any, Callable, ClassVar, Generator
 
 from pydantic_core import core_schema, CoreSchema, SchemaValidator
 from typing_extensions import Self
 from datetime import timedelta
 
 
-@dataclass
 class NonNegativeInteger(int):
+    """An integer that must be greater than or equal to 0."""
+
     schema: ClassVar[CoreSchema] = core_schema.int_schema(ge=0)
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
         yield cls.validate
 
     @classmethod
@@ -21,16 +21,17 @@
         return cls.schema
 
     @classmethod
     def validate(cls, v: Any) -> Self:
         return SchemaValidator(schema=cls.schema).validate_python(v)
 
 
-@dataclass
 class PositiveInteger(int):
+    """An integer that must be greater than 0."""
+
     schema: ClassVar[CoreSchema] = core_schema.int_schema(gt=0)
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
         yield cls.validate
 
     @classmethod
@@ -40,16 +41,35 @@
         return cls.schema
 
     @classmethod
     def validate(cls, v: Any) -> Self:
         return SchemaValidator(schema=cls.schema).validate_python(v)
 
 
-@dataclass
+class NonNegativeFloat(float):
+    schema: ClassVar[CoreSchema] = core_schema.float_schema(ge=0)
+
+    @classmethod
+    def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
+        yield cls.validate
+
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: Callable[..., Any]
+    ) -> CoreSchema:
+        return cls.schema
+
+    @classmethod
+    def validate(cls, v: Any) -> Self:
+        return SchemaValidator(schema=cls.schema).validate_python(v)
+
+
 class NonNegativeDuration(timedelta):
+    """A timedelta that must be greater than or equal to 0."""
+
     schema: ClassVar = core_schema.timedelta_schema(ge=timedelta(seconds=0))
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
         yield cls.validate
 
     @classmethod
@@ -59,16 +79,17 @@
         return cls.schema
 
     @classmethod
     def validate(cls, v: Any) -> Self:
         return SchemaValidator(schema=cls.schema).validate_python(v)
 
 
-@dataclass
 class PositiveDuration(timedelta):
+    """A timedelta that must be greater than 0."""
+
     schema: ClassVar = core_schema.timedelta_schema(gt=timedelta(seconds=0))
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable[..., Any], None, None]:
         yield cls.validate
 
     @classmethod
@@ -81,10 +102,11 @@
     def validate(cls, v: Any) -> Self:
         return SchemaValidator(schema=cls.schema).validate_python(v)
 
 
 __all__ = [
     "NonNegativeInteger",
     "PositiveInteger",
+    "NonNegativeFloat",
     "NonNegativeDuration",
     "PositiveDuration",
 ]
```

### Comparing `prefect-client-2.18.3/src/prefect/utilities/annotations.py` & `prefect-client-2.19.0/src/prefect/utilities/annotations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 import warnings
 from abc import ABC
 from collections import namedtuple
 from typing import Generic, TypeVar
 
 T = TypeVar("T")
 
@@ -13,21 +12,15 @@
     """
     Base class for Prefect annotation types.
 
     Inherits from `namedtuple` for unpacking support in another tools.
     """
 
     def unwrap(self) -> T:
-        if sys.version_info < (3, 8):
-            # cannot simply return self.value due to recursion error in Python 3.7
-            # also _asdict does not follow convention; it's not an internal method
-            # https://stackoverflow.com/a/26180604
-            return self._asdict()["value"]
-        else:
-            return self.value
+        return self.value
 
     def rewrap(self, value: T) -> "BaseAnnotation[T]":
         return type(self)(value)
 
     def __eq__(self, other: object) -> bool:
         if not type(self) == type(other):
             return False
```

### Comparing `prefect-client-2.18.3/src/prefect/utilities/asyncutils.py` & `prefect-client-2.19.0/src/prefect/utilities/asyncutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,18 @@
 
     @wraps(async_fn)
     def coroutine_wrapper(*args, **kwargs):
         from prefect._internal.concurrency.api import create_call, from_sync
         from prefect._internal.concurrency.calls import get_current_call, logger
         from prefect._internal.concurrency.event_loop import get_running_loop
         from prefect._internal.concurrency.threads import get_global_loop
+        from prefect.settings import PREFECT_EXPERIMENTAL_DISABLE_SYNC_COMPAT
+
+        if PREFECT_EXPERIMENTAL_DISABLE_SYNC_COMPAT:
+            return async_fn(*args, **kwargs)
 
         global_thread_portal = get_global_loop()
         current_thread = threading.current_thread()
         current_call = get_current_call()
         current_loop = get_running_loop()
 
         if current_thread.ident == global_thread_portal.thread.ident:
```

### Comparing `prefect-client-2.18.3/src/prefect/utilities/callables.py` & `prefect-client-2.19.0/src/prefect/utilities/callables.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/collections.py` & `prefect-client-2.19.0/src/prefect/utilities/collections.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/compat.py` & `prefect-client-2.19.0/src/prefect/utilities/compat.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/context.py` & `prefect-client-2.19.0/src/prefect/utilities/context.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/dispatch.py` & `prefect-client-2.19.0/src/prefect/utilities/dispatch.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/dockerutils.py` & `prefect-client-2.19.0/src/prefect/utilities/dockerutils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/engine.py` & `prefect-client-2.19.0/src/prefect/utilities/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import contextlib
+import inspect
 import os
 import signal
 import time
 from functools import partial
 from typing import (
     Any,
     Callable,
@@ -19,15 +20,15 @@
 import anyio
 from typing_extensions import Literal
 
 import prefect
 import prefect.context
 import prefect.plugins
 from prefect._internal.concurrency.cancellation import get_deadline
-from prefect.client.orchestration import PrefectClient
+from prefect.client.orchestration import PrefectClient, SyncPrefectClient
 from prefect.client.schemas import OrchestrationResult, TaskRun
 from prefect.client.schemas.objects import (
     StateType,
     TaskRunInput,
     TaskRunResult,
 )
 from prefect.client.schemas.responses import SetStateStatus
@@ -56,14 +57,15 @@
     get_state_exception,
     is_state,
 )
 from prefect.tasks import Task
 from prefect.utilities.annotations import allow_failure, quote
 from prefect.utilities.asyncutils import (
     gather,
+    run_sync,
 )
 from prefect.utilities.collections import StopVisiting, visit_collection
 from prefect.utilities.text import truncated_to
 
 API_HEALTHCHECKS = {}
 UNTRACKABLE_TYPES = {bool, type(None), type(...), type(NotImplemented)}
 engine_logger = get_logger("engine")
@@ -383,14 +385,117 @@
     else:
         raise ValueError(
             "Neither flow run id or task run id were provided. At least one must "
             "be given."
         )
 
     # Parse the response to return the new state
+    if response.status == SetStateStatus.ACCEPT:
+        # Update the state with the details if provided
+        state.id = response.state.id
+        state.timestamp = response.state.timestamp
+        if response.state.state_details:
+            state.state_details = response.state.state_details
+        return state
+
+    elif response.status == SetStateStatus.ABORT:
+        raise prefect.exceptions.Abort(response.details.reason)
+
+    elif response.status == SetStateStatus.REJECT:
+        if response.state.is_paused():
+            raise Pause(response.details.reason, state=response.state)
+        return response.state
+
+    else:
+        raise ValueError(
+            f"Received unexpected `SetStateStatus` from server: {response.status!r}"
+        )
+
+
+def propose_state_sync(
+    client: SyncPrefectClient,
+    state: State[object],
+    force: bool = False,
+    task_run_id: Optional[UUID] = None,
+    flow_run_id: Optional[UUID] = None,
+) -> State[object]:
+    """
+    Propose a new state for a flow run or task run, invoking Prefect orchestration logic.
+
+    If the proposed state is accepted, the provided `state` will be augmented with
+     details and returned.
+
+    If the proposed state is rejected, a new state returned by the Prefect API will be
+    returned.
+
+    If the proposed state results in a WAIT instruction from the Prefect API, the
+    function will sleep and attempt to propose the state again.
+
+    If the proposed state results in an ABORT instruction from the Prefect API, an
+    error will be raised.
+
+    Args:
+        state: a new state for the task or flow run
+        task_run_id: an optional task run id, used when proposing task run states
+        flow_run_id: an optional flow run id, used when proposing flow run states
+
+    Returns:
+        a [State model][prefect.client.schemas.objects.State] representation of the
+            flow or task run state
+
+    Raises:
+        ValueError: if neither task_run_id or flow_run_id is provided
+        prefect.exceptions.Abort: if an ABORT instruction is received from
+            the Prefect API
+    """
+
+    # Determine if working with a task run or flow run
+    if not task_run_id and not flow_run_id:
+        raise ValueError("You must provide either a `task_run_id` or `flow_run_id`")
+
+    # Handle task and sub-flow tracing
+    if state.is_final():
+        if isinstance(state.data, BaseResult) and state.data.has_cached_object():
+            # Avoid fetching the result unless it is cached, otherwise we defeat
+            # the purpose of disabling `cache_result_in_memory`
+            result = state.result(raise_on_failure=False, fetch=True)
+            if inspect.isawaitable(result):
+                result = run_sync(result)
+        else:
+            result = state.data
+
+        link_state_to_result(state, result)
+
+    # Handle repeated WAITs in a loop instead of recursively, to avoid
+    # reaching max recursion depth in extreme cases.
+    def set_state_and_handle_waits(set_state_func) -> OrchestrationResult:
+        response = set_state_func()
+        while response.status == SetStateStatus.WAIT:
+            engine_logger.debug(
+                f"Received wait instruction for {response.details.delay_seconds}s: "
+                f"{response.details.reason}"
+            )
+            time.sleep(response.details.delay_seconds)
+            response = set_state_func()
+        return response
+
+    # Attempt to set the state
+    if task_run_id:
+        set_state = partial(client.set_task_run_state, task_run_id, state, force=force)
+        response = set_state_and_handle_waits(set_state)
+    elif flow_run_id:
+        set_state = partial(client.set_flow_run_state, flow_run_id, state, force=force)
+        response = set_state_and_handle_waits(set_state)
+    else:
+        raise ValueError(
+            "Neither flow run id or task run id were provided. At least one must "
+            "be given."
+        )
+
+    # Parse the response to return the new state
     if response.status == SetStateStatus.ACCEPT:
         # Update the state with the details if provided
         state.id = response.state.id
         state.timestamp = response.state.timestamp
         if response.state.state_details:
             state.state_details = response.state.state_details
         return state
```

### Comparing `prefect-client-2.18.3/src/prefect/utilities/filesystem.py` & `prefect-client-2.19.0/src/prefect/utilities/filesystem.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/hashing.py` & `prefect-client-2.19.0/src/prefect/utilities/hashing.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/importtools.py` & `prefect-client-2.19.0/src/prefect/utilities/importtools.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/math.py` & `prefect-client-2.19.0/src/prefect/utilities/math.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/names.py` & `prefect-client-2.19.0/src/prefect/utilities/names.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/processutils.py` & `prefect-client-2.19.0/src/prefect/utilities/processutils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/pydantic.py` & `prefect-client-2.19.0/src/prefect/utilities/pydantic.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/render_swagger.py` & `prefect-client-2.19.0/src/prefect/utilities/render_swagger.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/schema_tools/hydration.py` & `prefect-client-2.19.0/src/prefect/utilities/schema_tools/hydration.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/schema_tools/validation.py` & `prefect-client-2.19.0/src/prefect/utilities/schema_tools/validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,17 +63,18 @@
 
 def validate(
     obj: Dict,
     schema: Dict,
     raise_on_error: bool = False,
     preprocess: bool = True,
     ignore_required: bool = False,
+    allow_none_with_default: bool = False,
 ) -> List[JSONSchemaValidationError]:
     if preprocess:
-        schema = preprocess_schema(schema)
+        schema = preprocess_schema(schema, allow_none_with_default)
 
     if ignore_required:
         schema = remove_nested_keys(["required"], schema)
 
     if raise_on_error:
         try:
             jsonschema.validate(obj, schema, _VALIDATOR)
@@ -183,23 +184,28 @@
 
     valid = len(error_response["errors"]) == 0
     error_response["valid"] = valid
 
     return error_response
 
 
-def _fix_null_typing(key: str, schema: Dict, required_fields: List[str]):
+def _fix_null_typing(
+    key: str,
+    schema: Dict,
+    required_fields: List[str],
+    allow_none_with_default: bool = False,
+):
     """
     Pydantic V1 does not generate a valid Draft2020-12 schema for null types.
     """
     if (
         key not in required_fields
         and "type" in schema
         and schema.get("type") != "null"
-        and "default" not in schema
+        and ("default" not in schema or allow_none_with_default)
     ):
         schema["anyOf"] = [{"type": schema["type"]}, {"type": "null"}]
         del schema["type"]
 
 
 def _fix_tuple_items(schema: Dict):
     """
@@ -210,31 +216,42 @@
         and isinstance(schema["items"], list)
         and not schema.get("prefixItems")
     ):
         schema["prefixItems"] = deepcopy(schema["items"])
         del schema["items"]
 
 
-def process_properties(properties, required_fields):
+def process_properties(
+    properties: Dict,
+    required_fields: List[str],
+    allow_none_with_default: bool = False,
+):
     for key, schema in properties.items():
-        _fix_null_typing(key, schema, required_fields)
+        _fix_null_typing(key, schema, required_fields, allow_none_with_default)
         _fix_tuple_items(schema)
 
         if "properties" in schema:
             required_fields = schema.get("required", [])
             process_properties(schema["properties"], required_fields)
 
 
-def preprocess_schema(schema):
+def preprocess_schema(
+    schema: Dict,
+    allow_none_with_default: bool = False,
+):
     schema = deepcopy(schema)
 
     if "properties" in schema:
         required_fields = schema.get("required", [])
-        process_properties(schema["properties"], required_fields)
+        process_properties(
+            schema["properties"], required_fields, allow_none_with_default
+        )
 
     if "definitions" in schema:  # Also process definitions for reused models
         for definition in (schema["definitions"] or {}).values():
             if "properties" in definition:
                 required_fields = definition.get("required", [])
-                process_properties(definition["properties"], required_fields)
+                process_properties(
+                    definition["properties"], required_fields, allow_none_with_default
+                )
 
     return schema
```

### Comparing `prefect-client-2.18.3/src/prefect/utilities/services.py` & `prefect-client-2.19.0/src/prefect/utilities/services.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/templating.py` & `prefect-client-2.19.0/src/prefect/utilities/templating.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/utilities/visualization.py` & `prefect-client-2.19.0/src/prefect/utilities/visualization.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/variables.py` & `prefect-client-2.19.0/src/prefect/variables.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/workers/base.py` & `prefect-client-2.19.0/src/prefect/workers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -832,23 +832,27 @@
 
     async def _check_flow_run(self, flow_run: "FlowRun") -> None:
         """
         Performs a check on a submitted flow run to warn the user if the flow run
         was created from a deployment with a storage block.
         """
         if flow_run.deployment_id:
+            assert (
+                self._client and self._client._started
+            ), "Client must be started to check flow run deployment."
             deployment = await self._client.read_deployment(flow_run.deployment_id)
             if deployment.storage_document_id:
                 raise ValueError(
                     f"Flow run {flow_run.id!r} was created from deployment"
                     f" {deployment.name!r} which is configured with a storage block."
-                    " Please use an"
-                    " agent to execute this flow run."
+                    " Please use an agent to execute this flow run."
                 )
 
+            #
+
     async def _submit_run(self, flow_run: "FlowRun") -> None:
         """
         Submits a given flow run for execution by the worker.
         """
         run_logger = self.get_flow_run_logger(flow_run)
 
         try:
@@ -890,15 +894,15 @@
             # If the run is not ready to submit, release the concurrency slot
             if self._limiter:
                 self._limiter.release_on_behalf_of(flow_run.id)
 
         self._submitting_flow_run_ids.remove(flow_run.id)
 
     async def _submit_run_and_capture_errors(
-        self, flow_run: "FlowRun", task_status: anyio.abc.TaskStatus = None
+        self, flow_run: "FlowRun", task_status: Optional[anyio.abc.TaskStatus] = None
     ) -> Union[BaseWorkerResult, Exception]:
         run_logger = self.get_flow_run_logger(flow_run)
 
         try:
             configuration = await self._get_configuration(flow_run)
             submitted_event = self._emit_flow_run_submitted_event(configuration)
             result = await self.run(
```

### Comparing `prefect-client-2.18.3/src/prefect/workers/block.py` & `prefect-client-2.19.0/src/prefect/workers/block.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/workers/process.py` & `prefect-client-2.19.0/src/prefect/workers/process.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 Replace `my-work-pool` with the name of the work pool you want the worker
 to poll for flow runs.
 
 For more information about work pools and workers,
 checkout out the [Prefect docs](/concepts/work-pools/).
 """
 
-import asyncio
 import contextlib
 import os
 import signal
 import socket
 import subprocess
 import sys
 import tempfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, Optional, Tuple
 
 import anyio
 import anyio.abc
-import sniffio
 
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
@@ -52,28 +50,14 @@
     from prefect.client.schemas.responses import DeploymentResponse
 
 if sys.platform == "win32":
     # exit code indicating that the process was terminated by Ctrl+C or Ctrl+Break
     STATUS_CONTROL_C_EXIT = 0xC000013A
 
 
-def _use_threaded_child_watcher():
-    if (
-        sys.version_info < (3, 8)
-        and sniffio.current_async_library() == "asyncio"
-        and sys.platform != "win32"
-    ):
-        from prefect.utilities.compat import ThreadedChildWatcher
-
-        # Python < 3.8 does not use a `ThreadedChildWatcher` by default which can
-        # lead to errors in tests on unix as the previous default `SafeChildWatcher`
-        # is not compatible with threaded event loops.
-        asyncio.get_event_loop_policy().set_child_watcher(ThreadedChildWatcher())
-
-
 def _infrastructure_pid_from_process(process: anyio.abc.Process) -> str:
     hostname = socket.gethostname()
     return f"{hostname}:{process.pid}"
 
 
 def _parse_infrastructure_pid(infrastructure_pid: str) -> Tuple[str, int]:
     hostname, pid = infrastructure_pid.split(":")
@@ -164,15 +148,14 @@
         # We must add creationflags to a dict so it is only passed as a function
         # parameter on Windows, because the presence of creationflags causes
         # errors on Unix even if set to None
         kwargs: Dict[str, object] = {}
         if sys.platform == "win32":
             kwargs["creationflags"] = subprocess.CREATE_NEW_PROCESS_GROUP
 
-        _use_threaded_child_watcher()
         flow_run_logger.info("Opening process...")
 
         working_dir_ctx = (
             tempfile.TemporaryDirectory(suffix="prefect")
             if not configuration.working_dir
             else contextlib.nullcontext(configuration.working_dir)
         )
```

### Comparing `prefect-client-2.18.3/src/prefect/workers/server.py` & `prefect-client-2.19.0/src/prefect/workers/server.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect/workers/utilities.py` & `prefect-client-2.19.0/src/prefect/workers/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/src/prefect_client.egg-info/PKG-INFO` & `prefect-client-2.19.0/src/prefect_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-client
-Version: 2.18.3
+Version: 2.19.0
 Summary: Workflow orchestration and management.
 Home-page: https://www.prefect.io
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/PrefectHQ/prefect/blob/main/RELEASE-NOTES.md
 Project-URL: Documentation, https://docs.prefect.io
```

### Comparing `prefect-client-2.18.3/src/prefect_client.egg-info/SOURCES.txt` & `prefect-client-2.19.0/src/prefect_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -279,14 +279,15 @@
 src/prefect/utilities/processutils.py
 src/prefect/utilities/pydantic.py
 src/prefect/utilities/render_swagger.py
 src/prefect/utilities/services.py
 src/prefect/utilities/slugify.py
 src/prefect/utilities/templating.py
 src/prefect/utilities/text.py
+src/prefect/utilities/timeout.py
 src/prefect/utilities/visualization.py
 src/prefect/utilities/schema_tools/__init__.py
 src/prefect/utilities/schema_tools/hydration.py
 src/prefect/utilities/schema_tools/validation.py
 src/prefect/workers/__init__.py
 src/prefect/workers/base.py
 src/prefect/workers/block.py
```

### Comparing `prefect-client-2.18.3/src/prefect_client.egg-info/requires.txt` & `prefect-client-2.19.0/src/prefect_client.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prefect-client-2.18.3/versioneer.py` & `prefect-client-2.19.0/versioneer.py`

 * *Files identical despite different names*

