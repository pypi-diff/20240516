# Comparing `tmp/python-glanceclient-4.5.0.tar.gz` & `tmp/python-glanceclient-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-glanceclient-4.5.0.tar", last modified: Fri Mar  1 13:50:33 2024, max compression
+gzip compressed data, was "python-glanceclient-4.6.0.tar", last modified: Thu May 16 12:57:25 2024, max compression
```

## Comparing `python-glanceclient-4.5.0.tar` & `python-glanceclient-4.6.0.tar`

### file list

```diff
@@ -1,203 +1,205 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.879452 python-glanceclient-4.5.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3433 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10984 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39523 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3987 2024-03-01 13:50:33.879452 python-glanceclient-4.5.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2465 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.847445 python-glanceclient-4.5.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.847445 python-glanceclient-4.5.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.847445 python-glanceclient-4.5.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40489 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/doc/source/cli/details.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/doc/source/cli/glance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/doc/source/cli/property-keys.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2986 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.847445 python-glanceclient-4.5.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2266 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/doc/source/reference/apiv2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.847445 python-glanceclient-4.5.0/glanceclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2466 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.851446 python-glanceclient-4.5.0/glanceclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14782 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9391 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/common/https.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/common/progressbar.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21023 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4778 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/exc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27978 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.851446 python-glanceclient-4.5.0/glanceclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.851446 python-glanceclient-4.5.0/glanceclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1824 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/functional/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.851446 python-glanceclient-4.5.0/glanceclient/tests/functional/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/functional/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3143 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/functional/v1/test_readonly_glance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.851446 python-glanceclient-4.5.0/glanceclient/tests/functional/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/functional/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2699 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/functional/v2/test_http_headers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4565 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/functional/v2/test_readonly_glance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.851446 python-glanceclient-4.5.0/glanceclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/test_exc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21075 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/test_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/test_progressbar.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41794 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8964 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/test_ssl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11289 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.855447 python-glanceclient-4.5.0/glanceclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4299 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v1/test_image_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32486 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v1/test_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22491 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v1/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2549 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v1/test_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.859448 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4537 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12218 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4003 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_client_requests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55426 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4218 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25659 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_namespaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12384 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10122 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7260 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_resource_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5083 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7259 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_schemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   163344 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_shell_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2492 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11218 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2414 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.859448 python-glanceclient-4.5.0/glanceclient/tests/unit/var/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/var/badcert.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2256 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/var/ca.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2094 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/var/certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2171 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/var/expired-cert.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3247 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/var/privatekey.key
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3372 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/var/wildcard-certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2623 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/unit/var/wildcard-san-certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6882 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.859448 python-glanceclient-4.5.0/glanceclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.863449 python-glanceclient-4.5.0/glanceclient/v1/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17334 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12947 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/apiclient/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3578 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/image_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14014 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18868 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v1/versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.867450 python-glanceclient-4.5.0/glanceclient/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2148 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/image_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8118 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/image_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1916 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/image_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23269 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22024 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/metadefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7868 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/namespace_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/resource_type_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/schemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    69861 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4390 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/glanceclient/v2/versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.867450 python-glanceclient-4.5.0/python_glanceclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3987 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/python_glanceclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6752 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/python_glanceclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/python_glanceclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/python_glanceclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/python_glanceclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/python_glanceclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/python_glanceclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-03-01 13:50:33.000000 python-glanceclient-4.5.0/python_glanceclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.843444 python-glanceclient-4.5.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.875451 python-glanceclient-4.5.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/2.16.0_Release-43ebe06b74a272ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/4.3.0_Release-1a7acbd472e16c72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/4.4.0_Release-a3c89184f345e5a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/add-member-get-command-11c15e0a94ecd39a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/add-support-for-glance-download-import-method-10525254db3e8e7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/boolean-properties-strict-checking-bdd624b5da81e723.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/bp-use-keystoneauth-e12f300e58577b13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/check-for-md5-59db8fd67870b214.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/copy-existing-image-619b7e6bc3394446.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/del_from_store-2d807c3038283907.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/drop-py-2-7-f10417b8d1dd38fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/drop-python-3-6-and-3-7-0b299b4dc9673c6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/fix-undesirable-raw-python-error-66e3ddaca7b72ae2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/fix_1889666-22dc97ce577eccc6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/headers-encoding-bug-rocky-889ccd885a9cc4e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/hidden-images-support-9e2277ad62bf0d31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/http-headers-per-rfc-8187-aafa3199f863be81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/image-tasks-api-ee3ea043557a1dfa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/log-request-id-e7f67a23a0ed5c7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/multi-store-import-45d05a6193ef2c04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/multi-store-support-acc7ad0e7e8b6f99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/multihash-download-verification-596e91bf7b68e7db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/multihash-filter-ef2a48dc48fae9dc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/multihash-support-f1474590cf3ef5cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4081 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/pike-relnote-2c77b01aa8799f35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/return-request-id-to-caller-47f4c0a684b1d88e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/rm-deprecate-ssl-opts-c88225a4ba2285ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/rocky-2.11.0-ba936fd5e969198d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/sess_client_grid-3c2101609110f413.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/notes/validation-data-support-dfb2463914818cd2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.879452 python-glanceclient-4.5.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.879452 python-glanceclient-4.5.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.879452 python-glanceclient-4.5.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8999 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23567 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/earlier.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1100 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2024-03-01 13:50:33.879452 python-glanceclient-4.5.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:50:33.879452 python-glanceclient-4.5.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1490 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/tools/fix_ca_bundle.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/tools/glance.bash_completion
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2024-03-01 13:50:03.000000 python-glanceclient-4.5.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.964713 python-glanceclient-4.6.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3433 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10984 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39980 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3987 2024-05-16 12:57:25.964713 python-glanceclient-4.6.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2465 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.936711 python-glanceclient-4.6.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.936711 python-glanceclient-4.6.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.936711 python-glanceclient-4.6.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40489 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/doc/source/cli/details.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/doc/source/cli/glance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/doc/source/cli/property-keys.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2986 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.936711 python-glanceclient-4.6.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2266 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/doc/source/reference/apiv2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.936711 python-glanceclient-4.6.0/glanceclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2466 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.940711 python-glanceclient-4.6.0/glanceclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14722 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9391 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/common/https.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/common/progressbar.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21187 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4778 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/exc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27978 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.940711 python-glanceclient-4.6.0/glanceclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.940711 python-glanceclient-4.6.0/glanceclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1824 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/functional/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.940711 python-glanceclient-4.6.0/glanceclient/tests/functional/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/functional/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3143 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/functional/v1/test_readonly_glance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.940711 python-glanceclient-4.6.0/glanceclient/tests/functional/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/functional/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2699 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/functional/v2/test_http_headers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4565 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/functional/v2/test_readonly_glance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.940711 python-glanceclient-4.6.0/glanceclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/test_exc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21094 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/test_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/test_progressbar.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41794 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8964 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/test_ssl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11289 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.944712 python-glanceclient-4.6.0/glanceclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4299 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v1/test_image_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32486 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v1/test_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22491 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v1/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2549 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v1/test_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.948712 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4537 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12218 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4003 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_client_requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55426 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4218 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25659 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_namespaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12384 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10122 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7260 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_resource_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5083 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7259 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_schemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   163344 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_shell_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2492 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11218 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2414 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.948712 python-glanceclient-4.6.0/glanceclient/tests/unit/var/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/var/badcert.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2256 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/var/ca.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2094 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/var/certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2171 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/var/expired-cert.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3247 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/var/privatekey.key
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3372 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/var/wildcard-certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2623 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/unit/var/wildcard-san-certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7188 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.948712 python-glanceclient-4.6.0/glanceclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.948712 python-glanceclient-4.6.0/glanceclient/v1/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17334 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12947 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/apiclient/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3578 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/image_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14014 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18868 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v1/versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.952712 python-glanceclient-4.6.0/glanceclient/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2148 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/image_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8118 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/image_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1916 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/image_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23269 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22024 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/metadefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7868 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/namespace_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/resource_type_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/schemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    69861 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4390 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/glanceclient/v2/versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.952712 python-glanceclient-4.6.0/python_glanceclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3987 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/python_glanceclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6843 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/python_glanceclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/python_glanceclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/python_glanceclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/python_glanceclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/python_glanceclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/python_glanceclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-05-16 12:57:25.000000 python-glanceclient-4.6.0/python_glanceclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.932711 python-glanceclient-4.6.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.960712 python-glanceclient-4.6.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/2.16.0_Release-43ebe06b74a272ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/4.3.0_Release-1a7acbd472e16c72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/4.4.0_Release-a3c89184f345e5a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/4.6.0_releasenotes-99ed8ea49481ee01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/add-member-get-command-11c15e0a94ecd39a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/add-support-for-glance-download-import-method-10525254db3e8e7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/boolean-properties-strict-checking-bdd624b5da81e723.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/bp-use-keystoneauth-e12f300e58577b13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/check-for-md5-59db8fd67870b214.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/copy-existing-image-619b7e6bc3394446.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/del_from_store-2d807c3038283907.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/drop-py-2-7-f10417b8d1dd38fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/drop-python-3-6-and-3-7-0b299b4dc9673c6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/fix-undesirable-raw-python-error-66e3ddaca7b72ae2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/fix_1889666-22dc97ce577eccc6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/headers-encoding-bug-rocky-889ccd885a9cc4e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/hidden-images-support-9e2277ad62bf0d31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/http-headers-per-rfc-8187-aafa3199f863be81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/image-tasks-api-ee3ea043557a1dfa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/log-request-id-e7f67a23a0ed5c7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/multi-store-import-45d05a6193ef2c04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/multi-store-support-acc7ad0e7e8b6f99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/multihash-download-verification-596e91bf7b68e7db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/multihash-filter-ef2a48dc48fae9dc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/multihash-support-f1474590cf3ef5cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4081 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/pike-relnote-2c77b01aa8799f35.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/return-request-id-to-caller-47f4c0a684b1d88e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/rm-deprecate-ssl-opts-c88225a4ba2285ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/rocky-2.11.0-ba936fd5e969198d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/sess_client_grid-3c2101609110f413.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/notes/validation-data-support-dfb2463914818cd2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.964713 python-glanceclient-4.6.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.964713 python-glanceclient-4.6.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.964713 python-glanceclient-4.6.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8999 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23567 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/earlier.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1100 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2024-05-16 12:57:25.964713 python-glanceclient-4.6.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:57:25.964713 python-glanceclient-4.6.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1490 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/tools/fix_ca_bundle.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/tools/glance.bash_completion
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2024-05-16 12:57:02.000000 python-glanceclient-4.6.0/tox.ini
```

### Comparing `python-glanceclient-4.5.0/.zuul.yaml` & `python-glanceclient-4.6.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/AUTHORS` & `python-glanceclient-4.6.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/CONTRIBUTING.rst` & `python-glanceclient-4.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/ChangeLog` & `python-glanceclient-4.6.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 CHANGES
 =======
 
+4.6.0
+-----
+
+* Release notes for 4.6.0
+* Do not leak X-Auth-Token when logging curl requests
+* Remove unused fallback to simplejson
+* reno: Update master for unmaintained/zed
+* Fix unit tests broken by requests-mock >= 1.12.0
+* Tests: Fix original\_only wrapper
+* reno: Update master for xena Unmaintained status
+* reno: Update master for wallaby Unmaintained status
+* reno: Update master for victoria Unmaintained status
+* Update master for stable/2024.1
+
 4.5.0
 -----
 
 * reno: Update master for yoga Unmaintained status
 * Remove incorrect validation for glance-download import method
 * Bump hacking
 * Exclude tests directory from coverage calculation
```

### Comparing `python-glanceclient-4.5.0/LICENSE` & `python-glanceclient-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/PKG-INFO` & `python-glanceclient-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-glanceclient
-Version: 4.5.0
+Version: 4.6.0
 Summary: OpenStack Image API Client Library
 Home-page: https://docs.openstack.org/python-glanceclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `python-glanceclient-4.5.0/README.rst` & `python-glanceclient-4.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/doc/source/cli/details.rst` & `python-glanceclient-4.6.0/doc/source/cli/details.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/doc/source/cli/glance.rst` & `python-glanceclient-4.6.0/doc/source/cli/glance.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/doc/source/cli/index.rst` & `python-glanceclient-4.6.0/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/doc/source/cli/property-keys.rst` & `python-glanceclient-4.6.0/doc/source/cli/property-keys.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/doc/source/conf.py` & `python-glanceclient-4.6.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/doc/source/reference/apiv2.rst` & `python-glanceclient-4.6.0/doc/source/reference/apiv2.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/doc/source/reference/index.rst` & `python-glanceclient-4.6.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/__init__.py` & `python-glanceclient-4.6.0/glanceclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/_i18n.py` & `python-glanceclient-4.6.0/glanceclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/client.py` & `python-glanceclient-4.6.0/glanceclient/client.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/common/exceptions.py` & `python-glanceclient-4.6.0/glanceclient/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/common/http.py` & `python-glanceclient-4.6.0/glanceclient/common/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,30 +11,26 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import copy
 import io
+import json
 import logging
 import socket
 
 from keystoneauth1 import adapter
 from keystoneauth1 import exceptions as ksa_exc
 import OpenSSL
 from oslo_utils import importutils
 from oslo_utils import netutils
 import requests
 import urllib.parse
 
-try:
-    import json
-except ImportError:
-    import simplejson as json
-
 from oslo_utils import encodeutils
 
 from glanceclient.common import utils
 from glanceclient import exc
 
 osprofiler_web = importutils.try_import("osprofiler.web")
```

### Comparing `python-glanceclient-4.5.0/glanceclient/common/https.py` & `python-glanceclient-4.6.0/glanceclient/common/https.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/common/progressbar.py` & `python-glanceclient-4.6.0/glanceclient/common/progressbar.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/common/utils.py` & `python-glanceclient-4.6.0/glanceclient/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,18 @@
 
 from glanceclient._i18n import _
 from glanceclient import exc
 
 
 _memoized_property_lock = threading.Lock()
 
-SENSITIVE_HEADERS = ('X-Auth-Token', )
+# NOTE(cyril): Sensitive headers must be bytes, not strings, because when we
+# compare them to actual headers in safe_header, headers have already been
+# encoded.
+SENSITIVE_HEADERS = (b'X-Auth-Token', )
 REQUIRED_FIELDS_ON_DATA = ('disk_format', 'container_format')
 
 
 # Decorator for cli-args
 def arg(*args, **kwargs):
     def _decorator(func):
         # Because of the semantics of decorator composition if we just append
```

### Comparing `python-glanceclient-4.5.0/glanceclient/exc.py` & `python-glanceclient-4.6.0/glanceclient/exc.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/shell.py` & `python-glanceclient-4.6.0/glanceclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/functional/README.rst` & `python-glanceclient-4.6.0/glanceclient/tests/functional/README.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/functional/base.py` & `python-glanceclient-4.6.0/glanceclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/functional/v1/test_readonly_glance.py` & `python-glanceclient-4.6.0/glanceclient/tests/functional/v1/test_readonly_glance.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/functional/v2/test_http_headers.py` & `python-glanceclient-4.6.0/glanceclient/tests/functional/v2/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/functional/v2/test_readonly_glance.py` & `python-glanceclient-4.6.0/glanceclient/tests/functional/v2/test_readonly_glance.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/test_base.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/test_client.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/test_exc.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/test_exc.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/test_http.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/test_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 def original_only(f):
     @functools.wraps(f)
     def wrapper(self, *args, **kwargs):
         if not hasattr(self.client, 'log_curl_request'):
             self.skipTest('Skip logging tests for session client')
 
         return f(self, *args, **kwargs)
+    return wrapper
 
 
 class TestClient(testtools.TestCase):
 
     scenarios = [
         ('httpclient', {'create_client': '_create_http_client'}),
         ('session', {'create_client': '_create_session_client'})
```

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/test_progressbar.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/test_progressbar.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/test_shell.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/test_ssl.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/test_ssl.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/test_utils.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v1/test_image_members.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v1/test_image_members.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v1/test_images.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v1/test_images.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v1/test_shell.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v1/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v1/test_versions.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v1/test_versions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/base.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/base.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/fixtures.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/fixtures.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_cache.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_cache.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_client_requests.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_client_requests.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_images.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_images.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_info.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_info.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_members.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_members.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_namespaces.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_namespaces.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_objects.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_objects.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_properties.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_properties.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_resource_types.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_resource_types.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_metadefs_tags.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_metadefs_tags.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_schemas.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_schemas.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_shell_v2.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_shell_v2.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_tags.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_tags.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_tasks.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_tasks.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/v2/test_versions.py` & `python-glanceclient-4.6.0/glanceclient/tests/unit/v2/test_versions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/var/ca.crt` & `python-glanceclient-4.6.0/glanceclient/tests/unit/var/ca.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/var/certificate.crt` & `python-glanceclient-4.6.0/glanceclient/tests/unit/var/certificate.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/var/expired-cert.crt` & `python-glanceclient-4.6.0/glanceclient/tests/unit/var/expired-cert.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/var/privatekey.key` & `python-glanceclient-4.6.0/glanceclient/tests/unit/var/privatekey.key`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/var/wildcard-certificate.crt` & `python-glanceclient-4.6.0/glanceclient/tests/unit/var/wildcard-certificate.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/unit/var/wildcard-san-certificate.crt` & `python-glanceclient-4.6.0/glanceclient/tests/unit/var/wildcard-san-certificate.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/tests/utils.py` & `python-glanceclient-4.6.0/glanceclient/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import copy
+from email.message import EmailMessage
 import io
 import json
 import testtools
 from urllib import parse
 
 from glanceclient.v2 import schemas
 
@@ -108,15 +109,20 @@
         :param version: HTTP Version
         :param status: Response status code
         :param reason: Status code related message.
         """
         self.body = body
         self.reason = reason
         self.version = version
-        self.headers = headers
+        # NOTE(tkajinam): Make the FakeResponse class compatible with
+        # http.client.HTTPResponse
+        # https://docs.python.org/3/library/http.client.html
+        self.headers = EmailMessage()
+        for header_key in headers:
+            self.headers[header_key] = headers[header_key]
         self.headers['x-openstack-request-id'] = 'req-1234'
         self.status_code = status_code
         self.raw = RawRequest(headers, body=body, reason=reason,
                               version=version, status=status_code)
 
     @property
     def status(self):
```

### Comparing `python-glanceclient-4.5.0/glanceclient/v1/__init__.py` & `python-glanceclient-4.6.0/glanceclient/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v1/apiclient/base.py` & `python-glanceclient-4.6.0/glanceclient/v1/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v1/apiclient/exceptions.py` & `python-glanceclient-4.6.0/glanceclient/v1/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v1/apiclient/utils.py` & `python-glanceclient-4.6.0/glanceclient/v1/apiclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v1/client.py` & `python-glanceclient-4.6.0/glanceclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v1/image_members.py` & `python-glanceclient-4.6.0/glanceclient/v1/image_members.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v1/images.py` & `python-glanceclient-4.6.0/glanceclient/v1/images.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v1/shell.py` & `python-glanceclient-4.6.0/glanceclient/v1/shell.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v1/versions.py` & `python-glanceclient-4.6.0/glanceclient/v1/versions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/__init__.py` & `python-glanceclient-4.6.0/glanceclient/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/cache.py` & `python-glanceclient-4.6.0/glanceclient/v2/cache.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/client.py` & `python-glanceclient-4.6.0/glanceclient/v2/client.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/image_members.py` & `python-glanceclient-4.6.0/glanceclient/v2/image_members.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/image_schema.py` & `python-glanceclient-4.6.0/glanceclient/v2/image_schema.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/image_tags.py` & `python-glanceclient-4.6.0/glanceclient/v2/image_tags.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/images.py` & `python-glanceclient-4.6.0/glanceclient/v2/images.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/info.py` & `python-glanceclient-4.6.0/glanceclient/v2/info.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/metadefs.py` & `python-glanceclient-4.6.0/glanceclient/v2/metadefs.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/namespace_schema.py` & `python-glanceclient-4.6.0/glanceclient/v2/namespace_schema.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/resource_type_schema.py` & `python-glanceclient-4.6.0/glanceclient/v2/resource_type_schema.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/schemas.py` & `python-glanceclient-4.6.0/glanceclient/v2/schemas.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/shell.py` & `python-glanceclient-4.6.0/glanceclient/v2/shell.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/tasks.py` & `python-glanceclient-4.6.0/glanceclient/v2/tasks.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/glanceclient/v2/versions.py` & `python-glanceclient-4.6.0/glanceclient/v2/versions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/python_glanceclient.egg-info/PKG-INFO` & `python-glanceclient-4.6.0/python_glanceclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-glanceclient
-Version: 4.5.0
+Version: 4.6.0
 Summary: OpenStack Image API Client Library
 Home-page: https://docs.openstack.org/python-glanceclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `python-glanceclient-4.5.0/python_glanceclient.egg-info/SOURCES.txt` & `python-glanceclient-4.6.0/python_glanceclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 releasenotes/notes/.placeholder
 releasenotes/notes/2.16.0_Release-43ebe06b74a272ba.yaml
 releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml
 releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml
 releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml
 releasenotes/notes/4.3.0_Release-1a7acbd472e16c72.yaml
 releasenotes/notes/4.4.0_Release-a3c89184f345e5a2.yaml
+releasenotes/notes/4.6.0_releasenotes-99ed8ea49481ee01.yaml
 releasenotes/notes/add-member-get-command-11c15e0a94ecd39a.yaml
 releasenotes/notes/add-support-for-glance-download-import-method-10525254db3e8e7a.yaml
 releasenotes/notes/boolean-properties-strict-checking-bdd624b5da81e723.yaml
 releasenotes/notes/bp-use-keystoneauth-e12f300e58577b13.yaml
 releasenotes/notes/check-for-md5-59db8fd67870b214.yaml
 releasenotes/notes/copy-existing-image-619b7e6bc3394446.yaml
 releasenotes/notes/del_from_store-2d807c3038283907.yaml
@@ -148,14 +149,15 @@
 releasenotes/notes/return-request-id-to-caller-47f4c0a684b1d88e.yaml
 releasenotes/notes/rm-deprecate-ssl-opts-c88225a4ba2285ad.yaml
 releasenotes/notes/rocky-2.11.0-ba936fd5e969198d.yaml
 releasenotes/notes/sess_client_grid-3c2101609110f413.yaml
 releasenotes/notes/validation-data-support-dfb2463914818cd2.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/earlier.rst
 releasenotes/source/index.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
```

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/check-for-md5-59db8fd67870b214.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/check-for-md5-59db8fd67870b214.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/hidden-images-support-9e2277ad62bf0d31.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/hidden-images-support-9e2277ad62bf0d31.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/http-headers-per-rfc-8187-aafa3199f863be81.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/http-headers-per-rfc-8187-aafa3199f863be81.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/multi-store-support-acc7ad0e7e8b6f99.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/multi-store-support-acc7ad0e7e8b6f99.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/multihash-download-verification-596e91bf7b68e7db.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/multihash-download-verification-596e91bf7b68e7db.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/multihash-support-f1474590cf3ef5cf.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/multihash-support-f1474590cf3ef5cf.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/notes/pike-relnote-2c77b01aa8799f35.yaml` & `python-glanceclient-4.6.0/releasenotes/notes/pike-relnote-2c77b01aa8799f35.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/source/conf.py` & `python-glanceclient-4.6.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/releasenotes/source/earlier.rst` & `python-glanceclient-4.6.0/releasenotes/source/earlier.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/run_tests.sh` & `python-glanceclient-4.6.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/setup.cfg` & `python-glanceclient-4.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/setup.py` & `python-glanceclient-4.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/tools/fix_ca_bundle.sh` & `python-glanceclient-4.6.0/tools/fix_ca_bundle.sh`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/tools/glance.bash_completion` & `python-glanceclient-4.6.0/tools/glance.bash_completion`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.5.0/tox.ini` & `python-glanceclient-4.6.0/tox.ini`

 * *Files identical despite different names*

