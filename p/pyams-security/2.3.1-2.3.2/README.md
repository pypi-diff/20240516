# Comparing `tmp/pyams_security-2.3.1.tar.gz` & `tmp/pyams_security-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_security-2.3.1.tar", last modified: Sun Apr 28 14:59:42 2024, max compression
+gzip compressed data, was "dist/pyams_security-2.3.2.tar", last modified: Wed May 15 16:11:36 2024, max compression
```

## Comparing `pyams_security-2.3.1.tar` & `pyams_security-2.3.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-28 14:59:13.000000 pyams_security-2.3.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-28 14:59:13.000000 pyams_security-2.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6809 2024-04-28 14:59:42.000000 pyams_security-2.3.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)     4911 2024-04-28 14:59:13.000000 pyams_security-2.3.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1344 2024-04-28 14:59:13.000000 pyams_security-2.3.1/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 14:59:42.000000 pyams_security-2.3.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3016 2024-04-28 14:59:13.000000 pyams_security-2.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/
--rw-rw-rw-   0 root         (0) root         (0)      867 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/api/
--rw-rw-rw-   0 root         (0) root         (0)     1292 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1247 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/credential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     1792 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/credentials.rst
--rw-rw-rw-   0 root         (0) root         (0)     6424 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/manager.rst
--rw-rw-rw-   0 root         (0) root         (0)     2176 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/notifications.rst
--rw-rw-rw-   0 root         (0) root         (0)     7314 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/passwords.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/plugins.rst
--rw-rw-rw-   0 root         (0) root         (0)     5925 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/policy.rst
--rw-rw-rw-   0 root         (0) root         (0)    15805 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/principals.rst
--rw-rw-rw-   0 root         (0) root         (0)     3690 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/profiles.rst
--rw-rw-rw-   0 root         (0) root         (0)     5633 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/rest.rst
--rw-rw-rw-   0 root         (0) root         (0)     6801 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/roles.rst
--rw-rw-rw-   0 root         (0) root         (0)    21085 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/security.rst
--rw-rw-rw-   0 root         (0) root         (0)    19460 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/users.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/generations/
--rw-rw-rw-   0 root         (0) root         (0)     4533 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/generations/evolve1.py
--rw-rw-rw-   0 root         (0) root         (0)     4961 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/include.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    11198 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3910 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1506 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/names.py
--rw-rw-rw-   0 root         (0) root         (0)     4234 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/notification.py
--rw-rw-rw-   0 root         (0) root         (0)    16708 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1771 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1969 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    17962 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo
--rw-rw-rw-   0 root         (0) root         (0)    30366 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po
--rw-rw-rw-   0 root         (0) root         (0)    16946 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/locales/pyams_security.pot
--rw-rw-rw-   0 root         (0) root         (0)     2433 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     2957 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/password.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/permission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     8272 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1343 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/password-reset.pt
--rw-rw-rw-   0 root         (0) root         (0)     1165 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/register-body.pt
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/register-info.pt
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/register-message.pt
--rw-rw-rw-   0 root         (0) root         (0)    18335 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/userfolder.py
--rw-rw-rw-   0 root         (0) root         (0)     7205 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/principal.py
--rw-rw-rw-   0 root         (0) root         (0)     4658 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     3422 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/property.py
--rw-rw-rw-   0 root         (0) root         (0)     4918 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     6297 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/role.py
--rw-rw-rw-   0 root         (0) root         (0)     5067 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12790 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/security.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     9326 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/utility.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/vocabulary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6809 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2583 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 14:59:35.000000 pyams_security-2.3.1/src/pyams_security.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-01-03 10:42:42.000000 pyams_security-2.3.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-03 10:42:42.000000 pyams_security-2.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6867 2024-05-15 16:11:36.000000 pyams_security-2.3.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     4969 2024-05-15 16:04:07.000000 pyams_security-2.3.2/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2024-01-03 10:42:42.000000 pyams_security-2.3.2/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 16:11:36.000000 pyams_security-2.3.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3016 2024-05-15 16:04:07.000000 pyams_security-2.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/
+-rw-rw-rw-   0 root         (0) root         (0)      867 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/credential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/doctests/credentials.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6424 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/doctests/manager.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/doctests/notifications.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7314 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/doctests/passwords.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/doctests/plugins.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6595 2024-05-15 16:04:07.000000 pyams_security-2.3.2/src/pyams_security/doctests/policy.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15805 2024-02-03 01:43:27.000000 pyams_security-2.3.2/src/pyams_security/doctests/principals.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/doctests/profiles.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5633 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/doctests/rest.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6801 2024-02-26 22:23:14.000000 pyams_security-2.3.2/src/pyams_security/doctests/roles.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21085 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/doctests/security.rst
+-rw-rw-rw-   0 root         (0) root         (0)    19460 2024-04-09 18:28:28.000000 pyams_security-2.3.2/src/pyams_security/doctests/users.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-01-24 17:10:07.000000 pyams_security-2.3.2/src/pyams_security/generations/evolve1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4961 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    11198 2024-02-12 16:11:21.000000 pyams_security-2.3.2/src/pyams_security/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2024-02-26 22:23:14.000000 pyams_security-2.3.2/src/pyams_security/interfaces/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/interfaces/names.py
+-rw-rw-rw-   0 root         (0) root         (0)     4234 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/interfaces/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    16708 2024-04-09 18:28:28.000000 pyams_security-2.3.2/src/pyams_security/interfaces/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/interfaces/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1969 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/interfaces/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/interfaces/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    17962 2024-04-28 14:51:36.000000 pyams_security-2.3.2/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo
+-rw-rw-rw-   0 root         (0) root         (0)    30366 2024-04-28 14:51:36.000000 pyams_security-2.3.2/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po
+-rw-rw-rw-   0 root         (0) root         (0)    16946 2024-04-28 14:51:36.000000 pyams_security-2.3.2/src/pyams_security/locales/pyams_security.pot
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2957 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/password.py
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/permission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/plugin/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8272 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/plugin/group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/plugin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/plugin/templates/password-reset.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/plugin/templates/register-body.pt
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/plugin/templates/register-info.pt
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/plugin/templates/register-message.pt
+-rw-rw-rw-   0 root         (0) root         (0)    18335 2024-04-09 18:28:28.000000 pyams_security-2.3.2/src/pyams_security/plugin/userfolder.py
+-rw-rw-rw-   0 root         (0) root         (0)     7665 2024-05-15 16:04:07.000000 pyams_security-2.3.2/src/pyams_security/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2024-02-12 16:11:21.000000 pyams_security-2.3.2/src/pyams_security/principal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4658 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/property.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2024-02-26 22:23:14.000000 pyams_security-2.3.2/src/pyams_security/role.py
+-rw-rw-rw-   0 root         (0) root         (0)     5067 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12864 2024-05-15 16:04:07.000000 pyams_security-2.3.2/src/pyams_security/security.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9326 2024-02-12 16:11:21.000000 pyams_security-2.3.2/src/pyams_security/utility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2024-01-03 10:42:42.000000 pyams_security-2.3.2/src/pyams_security/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6867 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:11:27.000000 pyams_security-2.3.2/src/pyams_security.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-15 16:11:36.000000 pyams_security-2.3.2/src/pyams_security.egg-info/top_level.txt
```

### Comparing `pyams_security-2.3.1/LICENSE` & `pyams_security-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/PKG-INFO` & `pyams_security-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_security
-Version: 2.3.1
+Version: 2.3.2
 Summary: PyAMS security management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -50,14 +50,18 @@
 Finally, PyAMS_security provides ACLs and roles management, as well as custom schema fields to
 store roles assigned to principals.
 
 
 Changelog
 =========
 
+2.3.2
+-----
+ - updated internal service identity checker
+
 2.3.1
 -----
  - updated translations
 
 2.3.0
 -----
  - allow case-insensitive local user login
```

### Comparing `pyams_security-2.3.1/docs/HISTORY.rst` & `pyams_security-2.3.2/docs/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+2.3.2
+-----
+ - updated internal service identity checker
+
 2.3.1
 -----
  - updated translations
 
 2.3.0
 -----
  - allow case-insensitive local user login
```

### Comparing `pyams_security-2.3.1/docs/README.rst` & `pyams_security-2.3.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/setup.py` & `pyams_security-2.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.3.1'
+version = '2.3.2'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_catalog',
     'pyams_zmi'
 ]
```

### Comparing `pyams_security-2.3.1/src/pyams_security/__init__.py` & `pyams_security-2.3.2/src/pyams_security/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/api/__init__.py` & `pyams_security-2.3.2/src/pyams_security/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/credential.py` & `pyams_security-2.3.2/src/pyams_security/credential.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/README.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/credentials.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/credentials.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/manager.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/manager.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/notifications.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/notifications.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/passwords.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/passwords.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/plugins.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/plugins.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/policy.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/policy.rst`

 * *Files 10% similar despite different names*

```diff
@@ -138,14 +138,35 @@
     >>> headers[0]
     ('Set-Cookie', 'auth_ticket=...!userid_type:b64unicode; Domain=example.com; Path=/; HttpOnly; SameSite=Lax')
 
     >>> headers = policy.forget(request)
     >>> headers[0]
     ('Set-Cookie', 'auth_ticket=; Domain=example.com; Max-Age=0; Path=/; expires=Wed, 31-Dec-97 23:59:59 GMT; HttpOnly; SameSite=Lax')
 
+
+Internal service identity
+-------------------------
+
+Some tasks, like scheduler ones, can be run using a specific internal user ID:
+
+    >>> from pyramid.threadlocal import RequestContext, manager
+    >>> from pyams_security.interfaces.names import INTERNAL_USER_ID
+    >>> from pyams_utils.request import check_request
+
+    >>> manager.clear()
+    >>> request = check_request(registry=config.registry, principal_id=INTERNAL_USER_ID)
+    >>> identity = request.identity
+    >>> identity is None
+    False
+    >>> identity['userid'] == INTERNAL_USER_ID
+    True
+    >>> sorted(identity['principals'])
+    ['system.Authenticated', 'system.Everyone', 'system:internal']
+
+
 Authentication plugins are available as external packages, which can be included individually
 into Pyramid's application configuration; some examples are "pyams_auth_http", "pyams_auth_jwt",
 "pyams_auth_oauth" or "pyams_ldap".
 
 
 Test cleanup:
```

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/principals.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/principals.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/profiles.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/profiles.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/rest.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/rest.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/roles.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/roles.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/security.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/security.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/doctests/users.rst` & `pyams_security-2.3.2/src/pyams_security/doctests/users.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/generations/__init__.py` & `pyams_security-2.3.2/src/pyams_security/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/generations/evolve1.py` & `pyams_security-2.3.2/src/pyams_security/generations/evolve1.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/include.py` & `pyams_security-2.3.2/src/pyams_security/include.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/index.py` & `pyams_security-2.3.2/src/pyams_security/index.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/interfaces/__init__.py` & `pyams_security-2.3.2/src/pyams_security/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/interfaces/base.py` & `pyams_security-2.3.2/src/pyams_security/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/interfaces/names.py` & `pyams_security-2.3.2/src/pyams_security/interfaces/names.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/interfaces/notification.py` & `pyams_security-2.3.2/src/pyams_security/interfaces/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/interfaces/plugin.py` & `pyams_security-2.3.2/src/pyams_security/interfaces/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/interfaces/profile.py` & `pyams_security-2.3.2/src/pyams_security/interfaces/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/interfaces/rest.py` & `pyams_security-2.3.2/src/pyams_security/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/interfaces/site.py` & `pyams_security-2.3.2/src/pyams_security/interfaces/site.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo` & `pyams_security-2.3.2/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po` & `pyams_security-2.3.2/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/locales/pyams_security.pot` & `pyams_security-2.3.2/src/pyams_security/locales/pyams_security.pot`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/notification.py` & `pyams_security-2.3.2/src/pyams_security/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/password.py` & `pyams_security-2.3.2/src/pyams_security/password.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/permission.py` & `pyams_security-2.3.2/src/pyams_security/permission.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/plugin/__init__.py` & `pyams_security-2.3.2/src/pyams_security/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/plugin/admin.py` & `pyams_security-2.3.2/src/pyams_security/plugin/admin.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/plugin/group.py` & `pyams_security-2.3.2/src/pyams_security/plugin/group.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/plugin/templates/password-reset.pt` & `pyams_security-2.3.2/src/pyams_security/plugin/templates/password-reset.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/plugin/templates/register-body.pt` & `pyams_security-2.3.2/src/pyams_security/plugin/templates/register-body.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/plugin/templates/register-info.pt` & `pyams_security-2.3.2/src/pyams_security/plugin/templates/register-info.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/plugin/userfolder.py` & `pyams_security-2.3.2/src/pyams_security/plugin/userfolder.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/policy.py` & `pyams_security-2.3.2/src/pyams_security/policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from pyramid.authorization import ACLHelper, Authenticated, Everyone
 from pyramid.interfaces import ISecurityPolicy
 from pyramid.request import RequestLocalCache
 from zope.interface import implementer
 
 from pyams_security.interfaces import IPrincipalsGetter, IRolesGetter, ISecurityManager
 from pyams_security.interfaces.base import IPrincipalInfo
+from pyams_security.interfaces.names import INTERNAL_USER_ID
 from pyams_security.interfaces.plugin import ICredentialsPlugin
 from pyams_utils.adapter import get_adapter_weight
 from pyams_utils.dict import DotDict
 from pyams_utils.registry import get_all_utilities_registered_for, query_utility
 from pyams_utils.wsgi import wsgi_environ_cache
 
 LOGGER = logging.getLogger('PyAMS (security)')
@@ -94,14 +95,25 @@
             context = request.context
         principals = {Everyone}
         principal_id = None
         identity = self.cookie_helper.identify(request)
         if identity is not None:
             principal_id = identity['userid']
         else:
+            try:
+                request_principal_id = request.principal.id
+            except AttributeError:
+                pass
+            else:
+                if request_principal_id == INTERNAL_USER_ID:
+                    principal_id = request_principal_id
+                    identity = {
+                        'userid': principal_id
+                    }
+        if not principal_id:
             for plugin in self.credentials_plugins:
                 credentials = plugin.extract_credentials(request)
                 if (credentials is not None) and (sm is not None):
                     principal_id = sm.authenticate(credentials, request)
                     if IPrincipalInfo.providedBy(principal_id):
                         principal_id = principal_id.id
                     if principal_id is not None:
```

### Comparing `pyams_security-2.3.1/src/pyams_security/principal.py` & `pyams_security-2.3.2/src/pyams_security/principal.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/profile.py` & `pyams_security-2.3.2/src/pyams_security/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/property.py` & `pyams_security-2.3.2/src/pyams_security/property.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/rest.py` & `pyams_security-2.3.2/src/pyams_security/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/role.py` & `pyams_security-2.3.2/src/pyams_security/role.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/schema.py` & `pyams_security-2.3.2/src/pyams_security/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/security.py` & `pyams_security-2.3.2/src/pyams_security/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from zope.interface import implementer
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_security.interfaces import GrantedRoleEvent, IContentRoles, \
     IDefaultProtectionPolicy, IProtectedObject, IRoleProtectedObject, ISecurityContext, \
     RevokedRoleEvent
 from pyams_security.interfaces.base import FORBIDDEN_PERMISSION, IPrincipalInfo, IRole, PUBLIC_PERMISSION, ROLE_ID
-from pyams_security.interfaces.names import ADMIN_USER_ID
+from pyams_security.interfaces.names import ADMIN_USER_ID, INTERNAL_USER_ID
 from pyams_security.permission import get_edit_permission
 from pyams_utils.adapter import adapter_config, get_annotation_adapter
 from pyams_utils.factory import factory_config
 from pyams_utils.registry import get_pyramid_registry, query_utility
 from pyams_utils.request import check_request, request_property
 
 __docformat__ = 'restructuredtext'
@@ -201,14 +201,15 @@
         # and 'public' permission to everyone
         result = []
         registry = get_pyramid_registry()
         if asbool(registry.settings.get('pyams.security.deny_forbidden_to_admin', True)):
             result.append((Deny, Everyone, {FORBIDDEN_PERMISSION}))
         result.extend([
             (Allow, ADMIN_USER_ID, ALL_PERMISSIONS),
+            (Allow, INTERNAL_USER_ID, ALL_PERMISSIONS),
             (Allow, Everyone, {PUBLIC_PERMISSION})
         ])
         # grant access to all roles permissions
         for role_id in self.get_granted_roles():
             role = query_utility(IRole, role_id)
             if role is not None:
                 result.append((Allow, ROLE_ID.format(role_id), role.permissions))
```

### Comparing `pyams_security-2.3.1/src/pyams_security/site.py` & `pyams_security-2.3.2/src/pyams_security/site.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/tests/__init__.py` & `pyams_security-2.3.2/src/pyams_security/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/tests/test_utilsdocs.py` & `pyams_security-2.3.2/src/pyams_security/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/tests/test_utilsdocstrings.py` & `pyams_security-2.3.2/src/pyams_security/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/utility.py` & `pyams_security-2.3.2/src/pyams_security/utility.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security/vocabulary.py` & `pyams_security-2.3.2/src/pyams_security/vocabulary.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.1/src/pyams_security.egg-info/PKG-INFO` & `pyams_security-2.3.2/src/pyams_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-security
-Version: 2.3.1
+Version: 2.3.2
 Summary: PyAMS security management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -50,14 +50,18 @@
 Finally, PyAMS_security provides ACLs and roles management, as well as custom schema fields to
 store roles assigned to principals.
 
 
 Changelog
 =========
 
+2.3.2
+-----
+ - updated internal service identity checker
+
 2.3.1
 -----
  - updated translations
 
 2.3.0
 -----
  - allow case-insensitive local user login
```

### Comparing `pyams_security-2.3.1/src/pyams_security.egg-info/SOURCES.txt` & `pyams_security-2.3.2/src/pyams_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

