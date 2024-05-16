# Comparing `tmp/cekit-4.9.0.tar.gz` & `tmp/cekit-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cekit-4.9.0.tar", last modified: Thu Sep  7 08:06:38 2023, max compression
+gzip compressed data, was "cekit-4.9.1.tar", last modified: Thu Sep  7 14:43:45 2023, max compression
```

## Comparing `cekit-4.9.0.tar` & `cekit-4.9.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.744859 cekit-4.9.0/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1074 2023-09-07 08:06:38.000000 cekit-4.9.0/LICENSE
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-09-07 08:06:38.000000 cekit-4.9.0/MANIFEST.in
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-09-07 08:06:38.744859 cekit-4.9.0/PKG-INFO
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      465 2023-09-07 08:06:38.000000 cekit-4.9.0/README.rst
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.742859 cekit-4.9.0/cekit/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3832 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/builder.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.743859 cekit-4.9.0/cekit/builders/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/builders/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1560 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/builders/buildah.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     9442 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/builders/docker_builder.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    21910 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/builders/osbs.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1711 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/builders/podman.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.743859 cekit-4.9.0/cekit/cache/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/cache/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3601 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/cache/artifact.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     5730 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/cache/cli.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      354 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/cekit_types.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    15304 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/cli.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     2290 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/config.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1346 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/crypto.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.743859 cekit-4.9.0/cekit/descriptor/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      682 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     6579 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/base.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1367 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/env.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1174 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/execute.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    19410 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/image.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1005 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/label.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1098 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/module.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1588 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/modules.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     4396 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/osbs.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      913 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/overrides.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     6338 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/packages.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1666 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/port.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    25109 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/resource.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1090 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/run.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      677 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/descriptor/volume.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      177 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/errors.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.743859 cekit-4.9.0/cekit/generator/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/generator/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    27221 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/generator/base.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      469 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/generator/behave.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      989 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/generator/docker.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3852 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/generator/legacy_version.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    14205 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/generator/osbs.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1639 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/log.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     5123 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/template_helper.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.744859 cekit-4.9.0/cekit/templates/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/templates/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3420 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/templates/help.jinja
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    10582 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/templates/template.jinja
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.744859 cekit-4.9.0/cekit/test/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/test/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     2564 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/test/behave_runner.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     2591 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/test/behave_tester.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3200 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/test/collector.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    21957 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/tools.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit/version.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 08:06:38.743859 cekit-4.9.0/cekit.egg-info/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit.egg-info/PKG-INFO
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1383 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        1 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       74 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit.egg-info/entry_points.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       99 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit.egg-info/requires.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        6 2023-09-07 08:06:38.000000 cekit-4.9.0/cekit.egg-info/top_level.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      638 2023-09-07 08:06:38.000000 cekit-4.9.0/requirements.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      499 2023-09-07 08:06:38.744859 cekit-4.9.0/setup.cfg
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      899 2023-09-07 08:06:38.000000 cekit-4.9.0/setup.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:45.024287 cekit-4.9.1/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1074 2023-09-07 14:43:44.000000 cekit-4.9.1/LICENSE
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-09-07 14:43:44.000000 cekit-4.9.1/MANIFEST.in
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-09-07 14:43:45.025287 cekit-4.9.1/PKG-INFO
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      465 2023-09-07 14:43:44.000000 cekit-4.9.1/README.rst
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:45.023286 cekit-4.9.1/cekit/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3832 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/builder.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:45.023286 cekit-4.9.1/cekit/builders/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/builders/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1560 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/builders/buildah.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     9442 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/builders/docker_builder.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    21914 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/builders/osbs.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1711 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/builders/podman.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:45.024287 cekit-4.9.1/cekit/cache/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/cache/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3601 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/cache/artifact.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     5730 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/cache/cli.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      354 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/cekit_types.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    15304 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/cli.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     2290 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/config.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1346 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/crypto.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:45.024287 cekit-4.9.1/cekit/descriptor/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      682 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     6579 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/base.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1367 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/env.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1174 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/execute.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    19410 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/image.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1005 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/label.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1098 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/module.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1588 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/modules.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     4396 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/osbs.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      913 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/overrides.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     6338 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/packages.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1666 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/port.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    25109 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/resource.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1090 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/run.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      677 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/descriptor/volume.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      177 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/errors.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:45.024287 cekit-4.9.1/cekit/generator/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/generator/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    27221 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/generator/base.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      469 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/generator/behave.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      989 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/generator/docker.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3852 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/generator/legacy_version.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    14205 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/generator/osbs.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1639 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/log.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     5123 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/template_helper.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:45.024287 cekit-4.9.1/cekit/templates/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/templates/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3420 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/templates/help.jinja
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    10582 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/templates/template.jinja
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:45.024287 cekit-4.9.1/cekit/test/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/test/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     2564 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/test/behave_runner.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     2591 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/test/behave_tester.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3200 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/test/collector.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    21957 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/tools.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit/version.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-09-07 14:43:45.023286 cekit-4.9.1/cekit.egg-info/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1383 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        1 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       74 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit.egg-info/entry_points.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       99 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit.egg-info/requires.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        6 2023-09-07 14:43:44.000000 cekit-4.9.1/cekit.egg-info/top_level.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      638 2023-09-07 14:43:44.000000 cekit-4.9.1/requirements.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      499 2023-09-07 14:43:45.025287 cekit-4.9.1/setup.cfg
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      899 2023-09-07 14:43:44.000000 cekit-4.9.1/setup.py
```

### Comparing `cekit-4.9.0/LICENSE` & `cekit-4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/PKG-INFO` & `cekit-4.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cekit
-Version: 4.9.0
+Version: 4.9.1
 Summary: Container image creation tool
 Home-page: https://github.com/cekit/cekit
-Download-URL: https://github.com/cekit/cekit/archive/4.9.0.tar.gz
+Download-URL: https://github.com/cekit/cekit/archive/4.9.1.tar.gz
 Author: CEKit team
 Author-email: cekit@cekit.io
 License: MIT
 License-File: LICENSE
 
 CEKit
 =====
```

### Comparing `cekit-4.9.0/cekit/builder.py` & `cekit-4.9.1/cekit/builder.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/builders/buildah.py` & `cekit-4.9.1/cekit/builders/buildah.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/builders/docker_builder.py` & `cekit-4.9.1/cekit/builders/docker_builder.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/builders/osbs.py` & `cekit-4.9.1/cekit/builders/osbs.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
 
             # Get the latest commit hash
             commit = run_wrapper(["git", "rev-parse", "HEAD"], True).stdout
 
             # Parse the dist-git repository url
             url = urlparse(url)
             # Construct the url again, with a hash and removed username and password, if any
-            src = "https://{}/git{}#{}".format(url.hostname, url.path, commit)
+            src = "git+https://{}/git{}#{}".format(url.hostname, url.path, commit)
 
             target = self.generator.image.get("osbs", {}).get("koji_target")
 
             # If target was not specified in the image descriptor
             if not target:
                 # Default to computed target based on branch
                 target = "{}-containers-candidate".format(self.git.branch)
```

### Comparing `cekit-4.9.0/cekit/builders/podman.py` & `cekit-4.9.1/cekit/builders/podman.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/cache/artifact.py` & `cekit-4.9.1/cekit/cache/artifact.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/cache/cli.py` & `cekit-4.9.1/cekit/cache/cli.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/cli.py` & `cekit-4.9.1/cekit/cli.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/config.py` & `cekit-4.9.1/cekit/config.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/crypto.py` & `cekit-4.9.1/cekit/crypto.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/__init__.py` & `cekit-4.9.1/cekit/descriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/base.py` & `cekit-4.9.1/cekit/descriptor/base.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/env.py` & `cekit-4.9.1/cekit/descriptor/env.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/execute.py` & `cekit-4.9.1/cekit/descriptor/execute.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/image.py` & `cekit-4.9.1/cekit/descriptor/image.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/label.py` & `cekit-4.9.1/cekit/descriptor/label.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/module.py` & `cekit-4.9.1/cekit/descriptor/module.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/modules.py` & `cekit-4.9.1/cekit/descriptor/modules.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/osbs.py` & `cekit-4.9.1/cekit/descriptor/osbs.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/overrides.py` & `cekit-4.9.1/cekit/descriptor/overrides.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/packages.py` & `cekit-4.9.1/cekit/descriptor/packages.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/port.py` & `cekit-4.9.1/cekit/descriptor/port.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/resource.py` & `cekit-4.9.1/cekit/descriptor/resource.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/run.py` & `cekit-4.9.1/cekit/descriptor/run.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/descriptor/volume.py` & `cekit-4.9.1/cekit/descriptor/volume.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/generator/base.py` & `cekit-4.9.1/cekit/generator/base.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/generator/docker.py` & `cekit-4.9.1/cekit/generator/docker.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/generator/legacy_version.py` & `cekit-4.9.1/cekit/generator/legacy_version.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/generator/osbs.py` & `cekit-4.9.1/cekit/generator/osbs.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/log.py` & `cekit-4.9.1/cekit/log.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/template_helper.py` & `cekit-4.9.1/cekit/template_helper.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/templates/help.jinja` & `cekit-4.9.1/cekit/templates/help.jinja`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/templates/template.jinja` & `cekit-4.9.1/cekit/templates/template.jinja`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/test/behave_runner.py` & `cekit-4.9.1/cekit/test/behave_runner.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/test/behave_tester.py` & `cekit-4.9.1/cekit/test/behave_tester.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/test/collector.py` & `cekit-4.9.1/cekit/test/collector.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit/tools.py` & `cekit-4.9.1/cekit/tools.py`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/cekit.egg-info/PKG-INFO` & `cekit-4.9.1/cekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cekit
-Version: 4.9.0
+Version: 4.9.1
 Summary: Container image creation tool
 Home-page: https://github.com/cekit/cekit
-Download-URL: https://github.com/cekit/cekit/archive/4.9.0.tar.gz
+Download-URL: https://github.com/cekit/cekit/archive/4.9.1.tar.gz
 Author: CEKit team
 Author-email: cekit@cekit.io
 License: MIT
 License-File: LICENSE
 
 CEKit
 =====
```

### Comparing `cekit-4.9.0/cekit.egg-info/SOURCES.txt` & `cekit-4.9.1/cekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/requirements.txt` & `cekit-4.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `cekit-4.9.0/setup.py` & `cekit-4.9.1/setup.py`

 * *Files identical despite different names*

