# Comparing `tmp/dub-0.0.3.tar.gz` & `tmp/dub-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dub-0.0.3.tar", last modified: Mon May 13 19:53:51 2024, max compression
+gzip compressed data, was "dub-0.0.4.tar", last modified: Thu May 16 10:30:14 2024, max compression
```

## Comparing `dub-0.0.3.tar` & `dub-0.0.4.tar`

### file list

```diff
@@ -1,90 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.482264 dub-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-13 19:53:51.482264 dub-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-05-13 19:53:43.000000 dub-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:53:51.482264 dub-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-13 19:53:43.000000 dub-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.466264 dub-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.470264 dub-0.0.3/src/dub/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.474264 dub-0.0.3/src/dub/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    83280 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    51298 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)    68151 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/metatags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.474264 dub-0.0.3/src/dub/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.474264 dub-0.0.3/src/dub/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/components/domainschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    50145 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/components/linkschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/components/tagschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/components/workspaceschema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.478264 dub-0.0.3/src/dub/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/badrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/conflict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/forbidden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/internalservererror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/inviteexpired.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/notfound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/ratelimitexceeded.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/unauthorized.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/errors/unprocessableentity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.478264 dub-0.0.3/src/dub/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.482264 dub-0.0.3/src/dub/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/adddomain.py
--rw-r--r--   0 runner    (1001) docker     (127)    49255 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/bulkcreatelinks.py
--rw-r--r--   0 runner    (1001) docker     (127)    49337 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/createlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/createtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/createworkspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/deletedomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/deletelink.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getbrowseranalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getcityanalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getclicksanalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getcountryanalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getdeviceanalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getlinkinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getlinkscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getmetatags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getosanalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getqrcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9270 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getrefereranalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/gettags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/gettimeseriesanalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/gettoplinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/gettopurls.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getworkspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/getworkspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/listdomains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/setprimarydomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/transferdomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/updatedomain.py
--rw-r--r--   0 runner    (1001) docker     (127)    49829 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/updatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    49358 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/models/operations/upsertlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/qr_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.482264 dub-0.0.3/src/dub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24355 2024-05-13 19:53:43.000000 dub-0.0.3/src/dub/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:51.474264 dub-0.0.3/src/dub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-13 19:53:51.000000 dub-0.0.3/src/dub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-13 19:53:51.000000 dub-0.0.3/src/dub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:53:51.000000 dub-0.0.3/src/dub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-13 19:53:51.000000 dub-0.0.3/src/dub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 19:53:51.000000 dub-0.0.3/src/dub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.501723 dub-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-16 10:30:14.501723 dub-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-05-16 10:30:04.000000 dub-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:30:14.501723 dub-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-16 10:30:04.000000 dub-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.485723 dub-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76999 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91910 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/clicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51298 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68151 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/metatags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/domainschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50145 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/linkschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/tagschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/workspaceschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.493723 dub-0.0.4/src/dub/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/badrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/conflict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/forbidden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/internalservererror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/inviteexpired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/notfound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/ratelimitexceeded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/unauthorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/unprocessableentity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.493723 dub-0.0.4/src/dub/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.501723 dub-0.0.4/src/dub/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/adddomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49255 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/bulkcreatelinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49337 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/createlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/createtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/createworkspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/deletedomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/deletelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getbrowsersbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getbrowsersbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getcitiesbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getcitiesbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getclickscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getclickscountdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13007 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getcountriesbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getcountriesbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getdevicesbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getdevicesbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getlinkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getlinkscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getmetatags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getosbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getosbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getqrcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getreferersbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getreferersbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettimeseriesbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettimeseriesbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettoplinksbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettoplinksbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettopurlsbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettopurlsbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getworkspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getworkspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/listdomains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/setprimarydomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/transferdomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/updatedomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49829 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/updatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49358 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/upsertlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/qr_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.501723 dub-0.0.4/src/dub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24355 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/top_level.txt
```

### Comparing `dub-0.0.3/PKG-INFO` & `dub-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dub
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # dub
         
         <div align="left">
@@ -101,24 +101,37 @@
         
         ### [qr_codes](https://github.com/dubinc/dub-python/blob/master/docs/sdks/qrcodes/README.md)
         
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/qrcodes/README.md#get) - Retrieve a QR code
         
         ### [analytics](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md)
         
-        * [clicks](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#clicks) - Retrieve clicks analytics
-        * [timeseries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries analytics
-        * [countries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#countries) - Retrieve country analytics
-        * [cities](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#cities) - Retrieve city analytics
-        * [devices](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#devices) - Retrieve device analytics
-        * [browsers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#browsers) - Retrieve browser analytics
-        * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve OS analytics
-        * [referers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referers) - Retrieve referer analytics
-        * [top_links](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_links) - Retrieve top links
-        * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs
+        * [~~timeseries~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics :warning: **Deprecated** Use `timeseries` instead.
+        * [~~country~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#country) - Retrieve top countries by clicks :warning: **Deprecated** Use `countries` instead.
+        * [~~city~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning: **Deprecated** Use `cities` instead.
+        * [~~device~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#device) - Retrieve top devices by clicks :warning: **Deprecated** Use `devices` instead.
+        * [~~browser~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#browser) - Retrieve top browsers by clicks :warning: **Deprecated** Use `browsers` instead.
+        * [~~os~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve top OS by clicks :warning: **Deprecated** Use `os` instead.
+        * [~~referer~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referer) - Retrieve top referers by clicks :warning: **Deprecated** Use `referers` instead.
+        * [~~top_links~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :warning: **Deprecated** Use `top_links` instead.
+        * [~~top_urls~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use `top_urls` instead.
+        
+        ### [analytics.clicks](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md)
+        
+        * [count](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#count) - Retrieve the total clicks count
+        * [timeseries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click analytics
+        * [countries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#countries) - Retrieve top countries by clicks
+        * [cities](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#cities) - Retrieve top cities by clicks
+        * [devices](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#devices) - Retrieve top devices by clicks
+        * [browsers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#browsers) - Retrieve top browsers by clicks
+        * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#os) - Retrieve top OS by clicks
+        * [referers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#referers) - Retrieve top referers by clicks
+        * [top_links](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#top_links) - Retrieve top links by clicks
+        * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks
+        * [~~get_clicks_count_deprecated~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the total clicks count :warning: **Deprecated** Use `count` instead.
         
         ### [workspaces](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md)
         
         * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces
         * [create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#create) - Create a workspace
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#get) - Retrieve a workspace
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dub Version: 0.0.3 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: dub Version: 0.0.4 Summary: Python Client SDK
 Generated by Speakeasy Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy License: UNKNOWN Description: # dub
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## ð **Welcome to your new SDK!** ð It has been generated successfully
 based on your OpenAPI spec. However, it is not yet ready for production use.
@@ -36,65 +36,91 @@
 Update a link * [create_many](https://github.com/dubinc/dub-python/blob/master/
 docs/sdks/links/README.md#create_many) - Bulk create links * [upsert](https://
 github.com/dubinc/dub-python/blob/master/docs/sdks/links/README.md#upsert) -
 Upsert a link ### [qr_codes](https://github.com/dubinc/dub-python/blob/master/
 docs/sdks/qrcodes/README.md) * [get](https://github.com/dubinc/dub-python/blob/
 master/docs/sdks/qrcodes/README.md#get) - Retrieve a QR code ### [analytics]
 (https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md) * [clicks](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/analytics/README.md#clicks) - Retrieve clicks analytics * [timeseries]
-(https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md#timeseries) - Retrieve timeseries analytics * [countries](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md#countries) - Retrieve country analytics * [cities](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#cities)
-- Retrieve city analytics * [devices](https://github.com/dubinc/dub-python/
-blob/master/docs/sdks/analytics/README.md#devices) - Retrieve device analytics
-* [browsers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-analytics/README.md#browsers) - Retrieve browser analytics * [os](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#os) -
-Retrieve OS analytics * [referers](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/analytics/README.md#referers) - Retrieve referer analytics *
-[top_links](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-analytics/README.md#top_links) - Retrieve top links * [top_urls](https://
+README.md) * [~~timeseries~~](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics
+:warning: **Deprecated** Use `timeseries` instead. * [~~country~~](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#country)
+- Retrieve top countries by clicks :warning: **Deprecated** Use `countries`
+instead. * [~~city~~](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning:
+**Deprecated** Use `cities` instead. * [~~device~~](https://github.com/dubinc/
+dub-python/blob/master/docs/sdks/analytics/README.md#device) - Retrieve top
+devices by clicks :warning: **Deprecated** Use `devices` instead. *
+[~~browser~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+analytics/README.md#browser) - Retrieve top browsers by clicks :warning:
+**Deprecated** Use `browsers` instead. * [~~os~~](https://github.com/dubinc/
+dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve top OS by
+clicks :warning: **Deprecated** Use `os` instead. * [~~referer~~](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referer)
+- Retrieve top referers by clicks :warning: **Deprecated** Use `referers`
+instead. * [~~top_links~~](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :
+warning: **Deprecated** Use `top_links` instead. * [~~top_urls~~](https://
 github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md#top_urls) - Retrieve top URLs ### [workspaces](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md) * [list](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#list) -
-Retrieve a list of workspaces * [create](https://github.com/dubinc/dub-python/
-blob/master/docs/sdks/workspaces/README.md#create) - Create a workspace * [get]
-(https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/
-README.md#get) - Retrieve a workspace ### [tags](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/tags/README.md) * [list](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/tags/README.md#list) - Retrieve a list
-of tags * [create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-tags/README.md#create) - Create a new tag ### [domains](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/domains/README.md) * [list](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#list) -
-Retrieve a list of domains * [add](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/domains/README.md#add) - Add a domain * [delete](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#delete) -
-Delete a domain * [update](https://github.com/dubinc/dub-python/blob/master/
-docs/sdks/domains/README.md#update) - Update a domain * [set_primary](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
-README.md#set_primary) - Set a domain as primary * [transfer](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#transfer)
-- Transfer a domain ### [metatags](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/metatags/README.md) * [get](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/metatags/README.md#get) - Retrieve the metatags
-for a URL ## Error Handling Handling errors in this SDK should largely match
-your expectations. All operations return a response object or raise an error.
-If Error objects are specified in your OpenAPI Spec, the SDK will raise the
-appropriate Error type. | Error Object | Status Code | Content Type | | -------
-------------------- | -------------------------- | -------------------------- |
-| errors.BadRequest | 400 | application/json | | errors.Unauthorized | 401 |
-application/json | | errors.Forbidden | 403 | application/json | |
-errors.NotFound | 404 | application/json | | errors.Conflict | 409 |
-application/json | | errors.InviteExpired | 410 | application/json | |
-errors.UnprocessableEntity | 422 | application/json | |
+README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use
+`top_urls` instead. ### [analytics.clicks](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/clicks/README.md) * [count](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#count) - Retrieve the
+total clicks count * [timeseries](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click
+analytics * [countries](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/clicks/README.md#countries) - Retrieve top countries by clicks * [cities]
+(https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/
+README.md#cities) - Retrieve top cities by clicks * [devices](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#devices) -
+Retrieve top devices by clicks * [browsers](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/clicks/README.md#browsers) - Retrieve top browsers
+by clicks * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+clicks/README.md#os) - Retrieve top OS by clicks * [referers](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#referers) -
+Retrieve top referers by clicks * [top_links](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/clicks/README.md#top_links) - Retrieve top links
+by clicks * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks *
+[~~get_clicks_count_deprecated~~](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the
+total clicks count :warning: **Deprecated** Use `count` instead. ###
+[workspaces](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+workspaces/README.md) * [list](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces *
+[create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/
+README.md#create) - Create a workspace * [get](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/workspaces/README.md#get) - Retrieve a workspace
+### [tags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/tags/
+README.md) * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+tags/README.md#list) - Retrieve a list of tags * [create](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/tags/README.md#create) - Create a new
+tag ### [domains](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+domains/README.md) * [list](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/domains/README.md#list) - Retrieve a list of domains * [add](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#add) - Add
+a domain * [delete](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+domains/README.md#delete) - Delete a domain * [update](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/domains/README.md#update) - Update a
+domain * [set_primary](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/domains/README.md#set_primary) - Set a domain as primary * [transfer]
+(https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
+README.md#transfer) - Transfer a domain ### [metatags](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/metatags/README.md) * [get](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/README.md#get) -
+Retrieve the metatags for a URL ## Error Handling Handling errors in this SDK
+should largely match your expectations. All operations return a response object
+or raise an error. If Error objects are specified in your OpenAPI Spec, the SDK
+will raise the appropriate Error type. | Error Object | Status Code | Content
+Type | | -------------------------- | -------------------------- | ------------
+-------------- | | errors.BadRequest | 400 | application/json | |
+errors.Unauthorized | 401 | application/json | | errors.Forbidden | 403 |
+application/json | | errors.NotFound | 404 | application/json | |
+errors.Conflict | 409 | application/json | | errors.InviteExpired | 410 |
+application/json | | errors.UnprocessableEntity | 422 | application/json | |
 errors.RateLimitExceeded | 429 | application/json | |
 errors.InternalServerError | 500 | application/json | | errors.SDKError | 4xx-
 5xx | */* | ### Example ```python import dub from dub.models import errors,
 operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res = None try:
 res = s.links.list(request=operations.GetLinksRequest()) except
 errors.BadRequest as e: # handle exception raise(e) except errors.Unauthorized
 as e: # handle exception raise(e) except errors.Forbidden as e: # handle
```

### Comparing `dub-0.0.3/README.md` & `dub-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -94,24 +94,37 @@
 
 ### [qr_codes](docs/sdks/qrcodes/README.md)
 
 * [get](docs/sdks/qrcodes/README.md#get) - Retrieve a QR code
 
 ### [analytics](docs/sdks/analytics/README.md)
 
-* [clicks](docs/sdks/analytics/README.md#clicks) - Retrieve clicks analytics
-* [timeseries](docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries analytics
-* [countries](docs/sdks/analytics/README.md#countries) - Retrieve country analytics
-* [cities](docs/sdks/analytics/README.md#cities) - Retrieve city analytics
-* [devices](docs/sdks/analytics/README.md#devices) - Retrieve device analytics
-* [browsers](docs/sdks/analytics/README.md#browsers) - Retrieve browser analytics
-* [os](docs/sdks/analytics/README.md#os) - Retrieve OS analytics
-* [referers](docs/sdks/analytics/README.md#referers) - Retrieve referer analytics
-* [top_links](docs/sdks/analytics/README.md#top_links) - Retrieve top links
-* [top_urls](docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs
+* [~~timeseries~~](docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics :warning: **Deprecated** Use `timeseries` instead.
+* [~~country~~](docs/sdks/analytics/README.md#country) - Retrieve top countries by clicks :warning: **Deprecated** Use `countries` instead.
+* [~~city~~](docs/sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning: **Deprecated** Use `cities` instead.
+* [~~device~~](docs/sdks/analytics/README.md#device) - Retrieve top devices by clicks :warning: **Deprecated** Use `devices` instead.
+* [~~browser~~](docs/sdks/analytics/README.md#browser) - Retrieve top browsers by clicks :warning: **Deprecated** Use `browsers` instead.
+* [~~os~~](docs/sdks/analytics/README.md#os) - Retrieve top OS by clicks :warning: **Deprecated** Use `os` instead.
+* [~~referer~~](docs/sdks/analytics/README.md#referer) - Retrieve top referers by clicks :warning: **Deprecated** Use `referers` instead.
+* [~~top_links~~](docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :warning: **Deprecated** Use `top_links` instead.
+* [~~top_urls~~](docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use `top_urls` instead.
+
+### [analytics.clicks](docs/sdks/clicks/README.md)
+
+* [count](docs/sdks/clicks/README.md#count) - Retrieve the total clicks count
+* [timeseries](docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click analytics
+* [countries](docs/sdks/clicks/README.md#countries) - Retrieve top countries by clicks
+* [cities](docs/sdks/clicks/README.md#cities) - Retrieve top cities by clicks
+* [devices](docs/sdks/clicks/README.md#devices) - Retrieve top devices by clicks
+* [browsers](docs/sdks/clicks/README.md#browsers) - Retrieve top browsers by clicks
+* [os](docs/sdks/clicks/README.md#os) - Retrieve top OS by clicks
+* [referers](docs/sdks/clicks/README.md#referers) - Retrieve top referers by clicks
+* [top_links](docs/sdks/clicks/README.md#top_links) - Retrieve top links by clicks
+* [top_urls](docs/sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks
+* [~~get_clicks_count_deprecated~~](docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the total clicks count :warning: **Deprecated** Use `count` instead.
 
 ### [workspaces](docs/sdks/workspaces/README.md)
 
 * [list](docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces
 * [create](docs/sdks/workspaces/README.md#create) - Create a workspace
 * [get](docs/sdks/workspaces/README.md#get) - Retrieve a workspace
```

#### html2text {}

```diff
@@ -26,51 +26,70 @@
 Create a new link * [count](docs/sdks/links/README.md#count) - Retrieve the
 number of links * [get](docs/sdks/links/README.md#get) - Retrieve a link *
 [delete](docs/sdks/links/README.md#delete) - Delete a link * [update](docs/
 sdks/links/README.md#update) - Update a link * [create_many](docs/sdks/links/
 README.md#create_many) - Bulk create links * [upsert](docs/sdks/links/
 README.md#upsert) - Upsert a link ### [qr_codes](docs/sdks/qrcodes/README.md) *
 [get](docs/sdks/qrcodes/README.md#get) - Retrieve a QR code ### [analytics]
-(docs/sdks/analytics/README.md) * [clicks](docs/sdks/analytics/
-README.md#clicks) - Retrieve clicks analytics * [timeseries](docs/sdks/
-analytics/README.md#timeseries) - Retrieve timeseries analytics * [countries]
-(docs/sdks/analytics/README.md#countries) - Retrieve country analytics *
-[cities](docs/sdks/analytics/README.md#cities) - Retrieve city analytics *
-[devices](docs/sdks/analytics/README.md#devices) - Retrieve device analytics *
-[browsers](docs/sdks/analytics/README.md#browsers) - Retrieve browser analytics
-* [os](docs/sdks/analytics/README.md#os) - Retrieve OS analytics * [referers]
-(docs/sdks/analytics/README.md#referers) - Retrieve referer analytics *
-[top_links](docs/sdks/analytics/README.md#top_links) - Retrieve top links *
-[top_urls](docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs ###
-[workspaces](docs/sdks/workspaces/README.md) * [list](docs/sdks/workspaces/
-README.md#list) - Retrieve a list of workspaces * [create](docs/sdks/
-workspaces/README.md#create) - Create a workspace * [get](docs/sdks/workspaces/
-README.md#get) - Retrieve a workspace ### [tags](docs/sdks/tags/README.md) *
-[list](docs/sdks/tags/README.md#list) - Retrieve a list of tags * [create]
-(docs/sdks/tags/README.md#create) - Create a new tag ### [domains](docs/sdks/
-domains/README.md) * [list](docs/sdks/domains/README.md#list) - Retrieve a list
-of domains * [add](docs/sdks/domains/README.md#add) - Add a domain * [delete]
-(docs/sdks/domains/README.md#delete) - Delete a domain * [update](docs/sdks/
-domains/README.md#update) - Update a domain * [set_primary](docs/sdks/domains/
-README.md#set_primary) - Set a domain as primary * [transfer](docs/sdks/
-domains/README.md#transfer) - Transfer a domain ### [metatags](docs/sdks/
-metatags/README.md) * [get](docs/sdks/metatags/README.md#get) - Retrieve the
-metatags for a URL ## Error Handling Handling errors in this SDK should largely
-match your expectations. All operations return a response object or raise an
-error. If Error objects are specified in your OpenAPI Spec, the SDK will raise
-the appropriate Error type. | Error Object | Status Code | Content Type | | ---
------------------------ | -------------------------- | ------------------------
--- | | errors.BadRequest | 400 | application/json | | errors.Unauthorized | 401
-| application/json | | errors.Forbidden | 403 | application/json | |
-errors.NotFound | 404 | application/json | | errors.Conflict | 409 |
-application/json | | errors.InviteExpired | 410 | application/json | |
-errors.UnprocessableEntity | 422 | application/json | |
-errors.RateLimitExceeded | 429 | application/json | |
-errors.InternalServerError | 500 | application/json | | errors.SDKError | 4xx-
-5xx | */* | ### Example ```python import dub from dub.models import errors,
+(docs/sdks/analytics/README.md) * [~~timeseries~~](docs/sdks/analytics/
+README.md#timeseries) - Retrieve timeseries click analytics :warning:
+**Deprecated** Use `timeseries` instead. * [~~country~~](docs/sdks/analytics/
+README.md#country) - Retrieve top countries by clicks :warning: **Deprecated**
+Use `countries` instead. * [~~city~~](docs/sdks/analytics/README.md#city) -
+Retrieve top cities by clicks :warning: **Deprecated** Use `cities` instead. *
+[~~device~~](docs/sdks/analytics/README.md#device) - Retrieve top devices by
+clicks :warning: **Deprecated** Use `devices` instead. * [~~browser~~](docs/
+sdks/analytics/README.md#browser) - Retrieve top browsers by clicks :warning:
+**Deprecated** Use `browsers` instead. * [~~os~~](docs/sdks/analytics/
+README.md#os) - Retrieve top OS by clicks :warning: **Deprecated** Use `os`
+instead. * [~~referer~~](docs/sdks/analytics/README.md#referer) - Retrieve top
+referers by clicks :warning: **Deprecated** Use `referers` instead. *
+[~~top_links~~](docs/sdks/analytics/README.md#top_links) - Retrieve top links
+by clicks :warning: **Deprecated** Use `top_links` instead. * [~~top_urls~~]
+(docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs by clicks :
+warning: **Deprecated** Use `top_urls` instead. ### [analytics.clicks](docs/
+sdks/clicks/README.md) * [count](docs/sdks/clicks/README.md#count) - Retrieve
+the total clicks count * [timeseries](docs/sdks/clicks/README.md#timeseries) -
+Retrieve timeseries click analytics * [countries](docs/sdks/clicks/
+README.md#countries) - Retrieve top countries by clicks * [cities](docs/sdks/
+clicks/README.md#cities) - Retrieve top cities by clicks * [devices](docs/sdks/
+clicks/README.md#devices) - Retrieve top devices by clicks * [browsers](docs/
+sdks/clicks/README.md#browsers) - Retrieve top browsers by clicks * [os](docs/
+sdks/clicks/README.md#os) - Retrieve top OS by clicks * [referers](docs/sdks/
+clicks/README.md#referers) - Retrieve top referers by clicks * [top_links]
+(docs/sdks/clicks/README.md#top_links) - Retrieve top links by clicks *
+[top_urls](docs/sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks *
+[~~get_clicks_count_deprecated~~](docs/sdks/clicks/
+README.md#get_clicks_count_deprecated) - Retrieve the total clicks count :
+warning: **Deprecated** Use `count` instead. ### [workspaces](docs/sdks/
+workspaces/README.md) * [list](docs/sdks/workspaces/README.md#list) - Retrieve
+a list of workspaces * [create](docs/sdks/workspaces/README.md#create) - Create
+a workspace * [get](docs/sdks/workspaces/README.md#get) - Retrieve a workspace
+### [tags](docs/sdks/tags/README.md) * [list](docs/sdks/tags/README.md#list) -
+Retrieve a list of tags * [create](docs/sdks/tags/README.md#create) - Create a
+new tag ### [domains](docs/sdks/domains/README.md) * [list](docs/sdks/domains/
+README.md#list) - Retrieve a list of domains * [add](docs/sdks/domains/
+README.md#add) - Add a domain * [delete](docs/sdks/domains/README.md#delete) -
+Delete a domain * [update](docs/sdks/domains/README.md#update) - Update a
+domain * [set_primary](docs/sdks/domains/README.md#set_primary) - Set a domain
+as primary * [transfer](docs/sdks/domains/README.md#transfer) - Transfer a
+domain ### [metatags](docs/sdks/metatags/README.md) * [get](docs/sdks/metatags/
+README.md#get) - Retrieve the metatags for a URL ## Error Handling Handling
+errors in this SDK should largely match your expectations. All operations
+return a response object or raise an error. If Error objects are specified in
+your OpenAPI Spec, the SDK will raise the appropriate Error type. | Error
+Object | Status Code | Content Type | | -------------------------- | ----------
+---------------- | -------------------------- | | errors.BadRequest | 400 |
+application/json | | errors.Unauthorized | 401 | application/json | |
+errors.Forbidden | 403 | application/json | | errors.NotFound | 404 |
+application/json | | errors.Conflict | 409 | application/json | |
+errors.InviteExpired | 410 | application/json | | errors.UnprocessableEntity |
+422 | application/json | | errors.RateLimitExceeded | 429 | application/json |
+| errors.InternalServerError | 500 | application/json | | errors.SDKError |
+4xx-5xx | */* | ### Example ```python import dub from dub.models import errors,
 operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res = None try:
 res = s.links.list(request=operations.GetLinksRequest()) except
 errors.BadRequest as e: # handle exception raise(e) except errors.Unauthorized
 as e: # handle exception raise(e) except errors.Forbidden as e: # handle
 exception raise(e) except errors.NotFound as e: # handle exception raise(e)
 except errors.Conflict as e: # handle exception raise(e) except
 errors.InviteExpired as e: # handle exception raise(e) except
```

### Comparing `dub-0.0.3/setup.py` & `dub-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='dub',
-    version='0.0.3',
+    version='0.0.4',
     author='Speakeasy',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/dubinc/dub-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `dub-0.0.3/src/dub/_hooks/registration.py` & `dub-0.0.4/src/dub/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/_hooks/sdkhooks.py` & `dub-0.0.4/src/dub/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/_hooks/types.py` & `dub-0.0.4/src/dub/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/analytics.py` & `dub-0.0.4/src/dub/clicks.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from dub import utils
 from dub._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from dub.models import components, errors, operations
 from typing import List, Optional
 
-class Analytics:
+class Clicks:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def clicks(self, request: operations.GetClicksAnalyticsRequest) -> operations.GetClicksAnalyticsResponse:
-        r"""Retrieve clicks analytics
-        Retrieve the number of clicks for a link, a domain, or the authenticated workspace.
+    def count(self, request: operations.GetClicksCountRequest) -> operations.GetClicksCountResponse:
+        r"""Retrieve the total clicks count
+        Retrieve the total number of clicks for a link, a domain, or the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getClicksAnalytics', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetClicksAnalyticsGlobals(
+        hook_ctx = HookContext(operation_id='getClicksCount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetClicksCountGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/clicks', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/count', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -56,15 +56,15 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetClicksAnalyticsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetClicksCountResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[float])
                 res.number = out
             else:
@@ -147,27 +147,27 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def timeseries(self, request: operations.GetTimeseriesAnalyticsRequest) -> operations.GetTimeseriesAnalyticsResponse:
-        r"""Retrieve timeseries analytics
-        Retrieve the number of clicks for a link, a domain, or the authenticated workspace over a period of time.
+    def timeseries(self, request: operations.GetTimeseriesByClicksRequest) -> operations.GetTimeseriesByClicksResponse:
+        r"""Retrieve timeseries click analytics
+        Retrieve timeseries click analytics for a link, a domain, or the authenticated workspace over a period of time.
         """
-        hook_ctx = HookContext(operation_id='getTimeseriesAnalytics', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetTimeseriesAnalyticsGlobals(
+        hook_ctx = HookContext(operation_id='getTimeseriesByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetTimeseriesByClicksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/timeseries', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/timeseries', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -192,15 +192,15 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetTimeseriesAnalyticsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetTimeseriesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[operations.ResponseBody]])
                 res.response_bodies = out
             else:
@@ -283,27 +283,27 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def countries(self, request: operations.GetCountryAnalyticsRequest) -> operations.GetCountryAnalyticsResponse:
-        r"""Retrieve country analytics
+    def countries(self, request: operations.GetCountriesByClicksRequest) -> operations.GetCountriesByClicksResponse:
+        r"""Retrieve top countries by clicks
         Retrieve the top countries by number of clicks for a link, a domain, or the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getCountryAnalytics', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetCountryAnalyticsGlobals(
+        hook_ctx = HookContext(operation_id='getCountriesByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetCountriesByClicksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/country', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/countries', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -328,20 +328,20 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetCountryAnalyticsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetCountriesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetCountryAnalyticsResponseBody]])
+                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetCountriesByClicksResponseBody]])
                 res.response_bodies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -419,27 +419,27 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def cities(self, request: operations.GetCityAnalyticsRequest) -> operations.GetCityAnalyticsResponse:
-        r"""Retrieve city analytics
+    def cities(self, request: operations.GetCitiesByClicksRequest) -> operations.GetCitiesByClicksResponse:
+        r"""Retrieve top cities by clicks
         Retrieve the top countries by number of clicks for a link, a domain, or the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getCityAnalytics', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetCityAnalyticsGlobals(
+        hook_ctx = HookContext(operation_id='getCitiesByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetCitiesByClicksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/city', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/cities', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -464,20 +464,20 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetCityAnalyticsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetCitiesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetCityAnalyticsResponseBody]])
+                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetCitiesByClicksResponseBody]])
                 res.response_bodies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -555,27 +555,27 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def devices(self, request: operations.GetDeviceAnalyticsRequest) -> operations.GetDeviceAnalyticsResponse:
-        r"""Retrieve device analytics
+    def devices(self, request: operations.GetDevicesByClicksRequest) -> operations.GetDevicesByClicksResponse:
+        r"""Retrieve top devices by clicks
         Retrieve the top devices by number of clicks for a link, a domain, or the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getDeviceAnalytics', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetDeviceAnalyticsGlobals(
+        hook_ctx = HookContext(operation_id='getDevicesByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetDevicesByClicksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/device', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/devices', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -600,20 +600,20 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetDeviceAnalyticsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetDevicesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetDeviceAnalyticsResponseBody]])
+                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetDevicesByClicksResponseBody]])
                 res.response_bodies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -691,27 +691,27 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def browsers(self, request: operations.GetBrowserAnalyticsRequest) -> operations.GetBrowserAnalyticsResponse:
-        r"""Retrieve browser analytics
+    def browsers(self, request: operations.GetBrowsersByClicksRequest) -> operations.GetBrowsersByClicksResponse:
+        r"""Retrieve top browsers by clicks
         Retrieve the top browsers by number of clicks for a link, a domain, or the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getBrowserAnalytics', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetBrowserAnalyticsGlobals(
+        hook_ctx = HookContext(operation_id='getBrowsersByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetBrowsersByClicksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/browser', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/browsers', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -736,20 +736,20 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetBrowserAnalyticsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetBrowsersByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetBrowserAnalyticsResponseBody]])
+                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetBrowsersByClicksResponseBody]])
                 res.response_bodies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -827,27 +827,27 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def os(self, request: operations.GetOSAnalyticsRequest) -> operations.GetOSAnalyticsResponse:
-        r"""Retrieve OS analytics
+    def os(self, request: operations.GetOSByClicksRequest) -> operations.GetOSByClicksResponse:
+        r"""Retrieve top OS by clicks
         Retrieve the top OS by number of clicks for a link, a domain, or the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getOSAnalytics', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetOSAnalyticsGlobals(
+        hook_ctx = HookContext(operation_id='getOSByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetOSByClicksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/os', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/os', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -872,20 +872,20 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetOSAnalyticsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetOSByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetOSAnalyticsResponseBody]])
+                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetOSByClicksResponseBody]])
                 res.response_bodies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -963,27 +963,27 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def referers(self, request: operations.GetRefererAnalyticsRequest) -> operations.GetRefererAnalyticsResponse:
-        r"""Retrieve referer analytics
+    def referers(self, request: operations.GetReferersByClicksRequest) -> operations.GetReferersByClicksResponse:
+        r"""Retrieve top referers by clicks
         Retrieve the top referers by number of clicks for a link, a domain, or the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getRefererAnalytics', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetRefererAnalyticsGlobals(
+        hook_ctx = HookContext(operation_id='getReferersByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetReferersByClicksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/referer', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/referers', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -1008,20 +1008,20 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetRefererAnalyticsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetReferersByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetRefererAnalyticsResponseBody]])
+                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetReferersByClicksResponseBody]])
                 res.response_bodies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -1099,27 +1099,27 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def top_links(self, request: operations.GetTopLinksRequest) -> operations.GetTopLinksResponse:
-        r"""Retrieve top links
+    def top_links(self, request: operations.GetTopLinksByClicksRequest) -> operations.GetTopLinksByClicksResponse:
+        r"""Retrieve top links by clicks
         Retrieve the top links by number of clicks for a domain or the authenticated workspace.
         """
-        hook_ctx = HookContext(operation_id='getTopLinks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetTopLinksGlobals(
+        hook_ctx = HookContext(operation_id='getTopLinksByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetTopLinksByClicksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/top_links', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/top_links', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -1144,20 +1144,20 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetTopLinksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetTopLinksByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetTopLinksResponseBody]])
+                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetTopLinksByClicksResponseBody]])
                 res.response_bodies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
@@ -1235,27 +1235,27 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def top_urls(self, request: operations.GetTopURLsRequest) -> operations.GetTopURLsResponse:
-        r"""Retrieve top URLs
+    def top_urls(self, request: operations.GetTopURLsByClicksRequest) -> operations.GetTopURLsByClicksResponse:
+        r"""Retrieve top URLs by clicks
         Retrieve the top URLs by number of clicks for a given short link.
         """
-        hook_ctx = HookContext(operation_id='getTopURLs', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.GetTopURLsGlobals(
+        hook_ctx = HookContext(operation_id='getTopURLsByClicks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetTopURLsByClicksGlobals(
             workspace_id=self.sdk_configuration.globals.workspace_id,
             project_slug=self.sdk_configuration.globals.project_slug,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/analytics/top_urls', request, _globals)
+        url = utils.generate_url(base_url, '/analytics/clicks/top_urls', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -1280,28 +1280,166 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetTopURLsResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        res = operations.GetTopURLsByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetTopURLsResponseBody]])
+                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetTopURLsByClicksResponseBody]])
                 res.response_bodies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BadRequest)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.Unauthorized)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 403:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.Forbidden)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 404:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.NotFound)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 409:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.Conflict)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 410:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.InviteExpired)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 422:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.UnprocessableEntity)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 429:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.RateLimitExceeded)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 500:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.InternalServerError)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+        return res
+
+    
+    
+    def get_clicks_count_deprecated(self, request: operations.GetClicksCountDeprecatedRequest) -> operations.GetClicksCountDeprecatedResponse:
+        r"""Retrieve the total clicks count
+        Retrieve the total number of clicks for a link, a domain, or the authenticated workspace.
+
+        Deprecated method: This method is deprecated. Use dub.analytics.clicks.count instead.. Use count instead.
+        """
+        hook_ctx = HookContext(operation_id='getClicksCountDeprecated', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetClicksCountDeprecatedGlobals(
+            workspace_id=self.sdk_configuration.globals.workspace_id,
+            project_slug=self.sdk_configuration.globals.project_slug,
+        )
+        
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(base_url, '/analytics/clicks', request, _globals)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['400','401','403','404','409','410','422','429','4XX','500','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        res = operations.GetClicksCountDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
+        
+        if http_res.status_code == 200:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[float])
+                res.number = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 400:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.BadRequest)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):
```

### Comparing `dub-0.0.3/src/dub/domains.py` & `dub-0.0.4/src/dub/domains.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/links.py` & `dub-0.0.4/src/dub/links.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/metatags.py` & `dub-0.0.4/src/dub/metatags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/components/domainschema.py` & `dub-0.0.4/src/dub/models/components/domainschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class Type(str, Enum):
     r"""The type of redirect to use for this domain."""
     REDIRECT = 'redirect'
     REWRITE = 'rewrite'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `dub-0.0.3/src/dub/models/components/httpmetadata.py` & `dub-0.0.4/src/dub/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/components/linkschema.py` & `dub-0.0.4/src/dub/models/components/linkschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/components/tagschema.py` & `dub-0.0.4/src/dub/models/components/tagschema.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 
+
 class Color(str, Enum):
     r"""The color of the tag."""
     RED = 'red'
     YELLOW = 'yellow'
     GREEN = 'green'
     BLUE = 'blue'
     PURPLE = 'purple'
```

### Comparing `dub-0.0.3/src/dub/models/components/workspaceschema.py` & `dub-0.0.4/src/dub/models/components/workspaceschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
+
 class Plan(str, Enum):
     r"""The plan of the workspace."""
     FREE = 'free'
     PRO = 'pro'
     BUSINESS = 'business'
     BUSINESS_PLUS = 'business plus'
     BUSINESS_EXTRA = 'business extra'
     BUSINESS_MAX = 'business max'
     ENTERPRISE = 'enterprise'
 
+
 class Role(str, Enum):
     r"""The role of the authenticated user in the workspace."""
     OWNER = 'owner'
     MEMBER = 'member'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `dub-0.0.3/src/dub/models/errors/__init__.py` & `dub-0.0.4/src/dub/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/errors/badrequest.py` & `dub-0.0.4/src/dub/models/errors/badrequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class Code(str, Enum):
     r"""A short code indicating the error code returned."""
     BAD_REQUEST = 'bad_request'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.3/src/dub/models/errors/conflict.py` & `dub-0.0.4/src/dub/models/errors/conflict.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class ConflictCode(str, Enum):
     r"""A short code indicating the error code returned."""
     CONFLICT = 'conflict'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.3/src/dub/models/errors/forbidden.py` & `dub-0.0.4/src/dub/models/errors/forbidden.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class ForbiddenCode(str, Enum):
     r"""A short code indicating the error code returned."""
     FORBIDDEN = 'forbidden'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.3/src/dub/models/errors/internalservererror.py` & `dub-0.0.4/src/dub/models/errors/internalservererror.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class InternalServerErrorCode(str, Enum):
     r"""A short code indicating the error code returned."""
     INTERNAL_SERVER_ERROR = 'internal_server_error'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.3/src/dub/models/errors/inviteexpired.py` & `dub-0.0.4/src/dub/models/errors/inviteexpired.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class InviteExpiredCode(str, Enum):
     r"""A short code indicating the error code returned."""
     INVITE_EXPIRED = 'invite_expired'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.3/src/dub/models/errors/notfound.py` & `dub-0.0.4/src/dub/models/errors/notfound.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class NotFoundCode(str, Enum):
     r"""A short code indicating the error code returned."""
     NOT_FOUND = 'not_found'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.3/src/dub/models/errors/ratelimitexceeded.py` & `dub-0.0.4/src/dub/models/errors/ratelimitexceeded.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class RateLimitExceededCode(str, Enum):
     r"""A short code indicating the error code returned."""
     RATE_LIMIT_EXCEEDED = 'rate_limit_exceeded'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.3/src/dub/models/errors/sdkerror.py` & `dub-0.0.4/src/dub/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/errors/unauthorized.py` & `dub-0.0.4/src/dub/models/errors/unauthorized.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class UnauthorizedCode(str, Enum):
     r"""A short code indicating the error code returned."""
     UNAUTHORIZED = 'unauthorized'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.3/src/dub/models/errors/unprocessableentity.py` & `dub-0.0.4/src/dub/models/errors/unprocessableentity.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import Optional
 
+
 class UnprocessableEntityCode(str, Enum):
     r"""A short code indicating the error code returned."""
     UNPROCESSABLE_ENTITY = 'unprocessable_entity'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.3/src/dub/models/internal/globals.py` & `dub-0.0.4/src/dub/models/internal/globals.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/adddomain.py` & `dub-0.0.4/src/dub/models/operations/adddomain.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class AddDomainGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
+
 class Type(str, Enum):
     r"""The type of redirect to use for this domain."""
     REDIRECT = 'redirect'
     REWRITE = 'rewrite'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `dub-0.0.3/src/dub/models/operations/bulkcreatelinks.py` & `dub-0.0.4/src/dub/models/operations/bulkcreatelinks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/createlink.py` & `dub-0.0.4/src/dub/models/operations/createlink.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/createtag.py` & `dub-0.0.4/src/dub/models/operations/createtag.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class CreateTagGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
+
 class Color(str, Enum):
     r"""The color of the tag. If not provided, a random color will be used from the list: red, yellow, green, blue, purple, pink, brown."""
     RED = 'red'
     YELLOW = 'yellow'
     GREEN = 'green'
     BLUE = 'blue'
     PURPLE = 'purple'
```

### Comparing `dub-0.0.3/src/dub/models/operations/createworkspace.py` & `dub-0.0.4/src/dub/models/operations/createworkspace.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/deletedomain.py` & `dub-0.0.4/src/dub/models/operations/deletedomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/deletelink.py` & `dub-0.0.4/src/dub/models/operations/deletelink.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/getbrowseranalytics.py` & `dub-0.0.4/src/dub/models/operations/getbrowsersbyclicksdeprecated.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetBrowserAnalyticsGlobals:
+class GetBrowsersByClicksDeprecatedGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
-class GetBrowserAnalyticsQueryParamInterval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+
+class GetBrowsersByClicksDeprecatedQueryParamInterval(str, Enum):
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
-class GetBrowserAnalyticsQueryParamCountry(str, Enum):
+
+class GetBrowsersByClicksDeprecatedQueryParamCountry(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -279,30 +281,30 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetBrowserAnalyticsRequest:
+class GetBrowsersByClicksDeprecatedRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[GetBrowserAnalyticsQueryParamInterval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[GetBrowsersByClicksDeprecatedQueryParamInterval] = dataclasses.field(default=GetBrowsersByClicksDeprecatedQueryParamInterval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
-    country: Optional[GetBrowserAnalyticsQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
+    country: Optional[GetBrowsersByClicksDeprecatedQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
     r"""The city to retrieve analytics for."""
     device: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'device', 'style': 'form', 'explode': True }})
     r"""The device to retrieve analytics for."""
     browser: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'browser', 'style': 'form', 'explode': True }})
     r"""The browser to retrieve analytics for."""
@@ -320,23 +322,23 @@
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBrowserAnalyticsResponseBody:
+class GetBrowsersByClicksDeprecatedResponseBody:
     browser: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('browser') }})
     r"""The name of the browser"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
     r"""The number of clicks from this browser"""
     
 
 
 
 @dataclasses.dataclass
-class GetBrowserAnalyticsResponse:
+class GetBrowsersByClicksDeprecatedResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    response_bodies: Optional[List[GetBrowserAnalyticsResponseBody]] = dataclasses.field(default=None)
+    response_bodies: Optional[List[GetBrowsersByClicksDeprecatedResponseBody]] = dataclasses.field(default=None)
     r"""The top browsers by number of clicks"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/getcityanalytics.py` & `dub-0.0.4/src/dub/models/operations/getcitiesbyclicks.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetCityAnalyticsGlobals:
+class GetCitiesByClicksGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
-class GetCityAnalyticsQueryParamInterval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+
+class GetCitiesByClicksQueryParamInterval(str, Enum):
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
-class GetCityAnalyticsQueryParamCountry(str, Enum):
+
+class GetCitiesByClicksQueryParamCountry(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -279,30 +281,30 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetCityAnalyticsRequest:
+class GetCitiesByClicksRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[GetCityAnalyticsQueryParamInterval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[GetCitiesByClicksQueryParamInterval] = dataclasses.field(default=GetCitiesByClicksQueryParamInterval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
-    country: Optional[GetCityAnalyticsQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
+    country: Optional[GetCitiesByClicksQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
     r"""The city to retrieve analytics for."""
     device: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'device', 'style': 'form', 'explode': True }})
     r"""The device to retrieve analytics for."""
     browser: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'browser', 'style': 'form', 'explode': True }})
     r"""The browser to retrieve analytics for."""
@@ -317,15 +319,16 @@
     qr: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'qr', 'style': 'form', 'explode': True }})
     r"""Filter for QR code scans. If true, filter for QR codes only. If false, filter for links only. If undefined, return both."""
     root: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'root', 'style': 'form', 'explode': True }})
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
-class GetCityAnalyticsCountry(str, Enum):
+
+class GetCitiesByClicksCountry(str, Enum):
     r"""The 2-letter country code of the city: https://d.to/geo"""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -573,25 +576,25 @@
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetCityAnalyticsResponseBody:
+class GetCitiesByClicksResponseBody:
     city: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city') }})
     r"""The name of the city"""
-    country: GetCityAnalyticsCountry = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country') }})
+    country: GetCitiesByClicksCountry = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country') }})
     r"""The 2-letter country code of the city: https://d.to/geo"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
     r"""The number of clicks from this city"""
     
 
 
 
 @dataclasses.dataclass
-class GetCityAnalyticsResponse:
+class GetCitiesByClicksResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    response_bodies: Optional[List[GetCityAnalyticsResponseBody]] = dataclasses.field(default=None)
+    response_bodies: Optional[List[GetCitiesByClicksResponseBody]] = dataclasses.field(default=None)
     r"""The top cities by number of clicks"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/getclicksanalytics.py` & `dub-0.0.4/src/dub/models/operations/getclickscount.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 import dataclasses
 from ...models.components import httpmetadata as components_httpmetadata
 from enum import Enum
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetClicksAnalyticsGlobals:
+class GetClicksCountGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
+
 class Interval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
+
 class Country(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
@@ -277,25 +279,25 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetClicksAnalyticsRequest:
+class GetClicksCountRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[Interval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[Interval] = dataclasses.field(default=Interval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
     country: Optional[Country] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
@@ -317,13 +319,13 @@
     root: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'root', 'style': 'form', 'explode': True }})
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
 
 @dataclasses.dataclass
-class GetClicksAnalyticsResponse:
+class GetClicksCountResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
     number: Optional[float] = dataclasses.field(default=None)
     r"""The number of clicks"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/getcountryanalytics.py` & `dub-0.0.4/src/dub/models/operations/getcountriesbyclicks.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetCountryAnalyticsGlobals:
+class GetCountriesByClicksGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
-class GetCountryAnalyticsQueryParamInterval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+
+class GetCountriesByClicksQueryParamInterval(str, Enum):
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
-class GetCountryAnalyticsQueryParamCountry(str, Enum):
+
+class GetCountriesByClicksQueryParamCountry(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -279,30 +281,30 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetCountryAnalyticsRequest:
+class GetCountriesByClicksRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[GetCountryAnalyticsQueryParamInterval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[GetCountriesByClicksQueryParamInterval] = dataclasses.field(default=GetCountriesByClicksQueryParamInterval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
-    country: Optional[GetCountryAnalyticsQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
+    country: Optional[GetCountriesByClicksQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
     r"""The city to retrieve analytics for."""
     device: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'device', 'style': 'form', 'explode': True }})
     r"""The device to retrieve analytics for."""
     browser: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'browser', 'style': 'form', 'explode': True }})
     r"""The browser to retrieve analytics for."""
@@ -317,15 +319,16 @@
     qr: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'qr', 'style': 'form', 'explode': True }})
     r"""Filter for QR code scans. If true, filter for QR codes only. If false, filter for links only. If undefined, return both."""
     root: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'root', 'style': 'form', 'explode': True }})
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
-class GetCountryAnalyticsCountry(str, Enum):
+
+class GetCountriesByClicksCountry(str, Enum):
     r"""The 2-letter country code: https://d.to/geo"""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -573,23 +576,23 @@
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetCountryAnalyticsResponseBody:
-    country: GetCountryAnalyticsCountry = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country') }})
+class GetCountriesByClicksResponseBody:
+    country: GetCountriesByClicksCountry = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country') }})
     r"""The 2-letter country code: https://d.to/geo"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
     r"""The number of clicks from this country"""
     
 
 
 
 @dataclasses.dataclass
-class GetCountryAnalyticsResponse:
+class GetCountriesByClicksResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    response_bodies: Optional[List[GetCountryAnalyticsResponseBody]] = dataclasses.field(default=None)
+    response_bodies: Optional[List[GetCountriesByClicksResponseBody]] = dataclasses.field(default=None)
     r"""The top countries by number of clicks"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/getdeviceanalytics.py` & `dub-0.0.4/src/dub/models/operations/gettimeseriesbyclicks.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetDeviceAnalyticsGlobals:
+class GetTimeseriesByClicksGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
-class GetDeviceAnalyticsQueryParamInterval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+
+class QueryParamInterval(str, Enum):
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
-class GetDeviceAnalyticsQueryParamCountry(str, Enum):
+
+class QueryParamCountry(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -279,30 +281,30 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetDeviceAnalyticsRequest:
+class GetTimeseriesByClicksRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[GetDeviceAnalyticsQueryParamInterval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[QueryParamInterval] = dataclasses.field(default=QueryParamInterval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
-    country: Optional[GetDeviceAnalyticsQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
+    country: Optional[QueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
     r"""The city to retrieve analytics for."""
     device: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'device', 'style': 'form', 'explode': True }})
     r"""The device to retrieve analytics for."""
     browser: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'browser', 'style': 'form', 'explode': True }})
     r"""The browser to retrieve analytics for."""
@@ -320,23 +322,23 @@
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDeviceAnalyticsResponseBody:
-    device: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('device') }})
-    r"""The name of the device"""
+class ResponseBody:
+    start: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start') }})
+    r"""The starting timestamp of the interval"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
-    r"""The number of clicks from this device"""
+    r"""The number of clicks in the interval"""
     
 
 
 
 @dataclasses.dataclass
-class GetDeviceAnalyticsResponse:
+class GetTimeseriesByClicksResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    response_bodies: Optional[List[GetDeviceAnalyticsResponseBody]] = dataclasses.field(default=None)
-    r"""The top devices by number of clicks"""
+    response_bodies: Optional[List[ResponseBody]] = dataclasses.field(default=None)
+    r"""The number of clicks over a period of time"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/getlinkinfo.py` & `dub-0.0.4/src/dub/models/operations/getlinkinfo.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/getlinks.py` & `dub-0.0.4/src/dub/models/operations/getlinks.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class GetLinksGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
+
 class Sort(str, Enum):
     r"""The field to sort the links by. The default is `createdAt`, and sort order is always descending."""
     CREATED_AT = 'createdAt'
     CLICKS = 'clicks'
     LAST_CLICKED = 'lastClicked'
```

### Comparing `dub-0.0.3/src/dub/models/operations/getlinkscount.py` & `dub-0.0.4/src/dub/models/operations/getlinkscount.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 class GetLinksCountGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
+
 class Two(str, Enum):
     TAG_ID = 'tagId'
 
+
 class One(str, Enum):
     DOMAIN = 'domain'
 
 
 @dataclasses.dataclass
 class GetLinksCountRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
```

### Comparing `dub-0.0.3/src/dub/models/operations/getmetatags.py` & `dub-0.0.4/src/dub/models/operations/getmetatags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/getosanalytics.py` & `dub-0.0.4/src/dub/models/operations/getosbyclicks.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetOSAnalyticsGlobals:
+class GetOSByClicksGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
-class GetOSAnalyticsQueryParamInterval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+
+class GetOSByClicksQueryParamInterval(str, Enum):
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
-class GetOSAnalyticsQueryParamCountry(str, Enum):
+
+class GetOSByClicksQueryParamCountry(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -279,30 +281,30 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetOSAnalyticsRequest:
+class GetOSByClicksRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[GetOSAnalyticsQueryParamInterval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[GetOSByClicksQueryParamInterval] = dataclasses.field(default=GetOSByClicksQueryParamInterval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
-    country: Optional[GetOSAnalyticsQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
+    country: Optional[GetOSByClicksQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
     r"""The city to retrieve analytics for."""
     device: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'device', 'style': 'form', 'explode': True }})
     r"""The device to retrieve analytics for."""
     browser: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'browser', 'style': 'form', 'explode': True }})
     r"""The browser to retrieve analytics for."""
@@ -320,23 +322,23 @@
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOSAnalyticsResponseBody:
+class GetOSByClicksResponseBody:
     os: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('os') }})
     r"""The name of the OS"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
     r"""The number of clicks from this OS"""
     
 
 
 
 @dataclasses.dataclass
-class GetOSAnalyticsResponse:
+class GetOSByClicksResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    response_bodies: Optional[List[GetOSAnalyticsResponseBody]] = dataclasses.field(default=None)
+    response_bodies: Optional[List[GetOSByClicksResponseBody]] = dataclasses.field(default=None)
     r"""The top OS by number of clicks"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/getqrcode.py` & `dub-0.0.4/src/dub/models/operations/getqrcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 from ...models.components import httpmetadata as components_httpmetadata
 from enum import Enum
 from typing import Optional
 
+
 class Level(str, Enum):
     r"""The level of error correction to use for the QR code. Defaults to `L` if not provided."""
     L = 'L'
     M = 'M'
     Q = 'Q'
     H = 'H'
```

### Comparing `dub-0.0.3/src/dub/models/operations/getrefereranalytics.py` & `dub-0.0.4/src/dub/models/operations/getosbyclicksdeprecated.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetRefererAnalyticsGlobals:
+class GetOSByClicksDeprecatedGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
-class GetRefererAnalyticsQueryParamInterval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+
+class GetOSByClicksDeprecatedQueryParamInterval(str, Enum):
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
-class GetRefererAnalyticsQueryParamCountry(str, Enum):
+
+class GetOSByClicksDeprecatedQueryParamCountry(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -279,30 +281,30 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetRefererAnalyticsRequest:
+class GetOSByClicksDeprecatedRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[GetRefererAnalyticsQueryParamInterval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[GetOSByClicksDeprecatedQueryParamInterval] = dataclasses.field(default=GetOSByClicksDeprecatedQueryParamInterval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
-    country: Optional[GetRefererAnalyticsQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
+    country: Optional[GetOSByClicksDeprecatedQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
     r"""The city to retrieve analytics for."""
     device: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'device', 'style': 'form', 'explode': True }})
     r"""The device to retrieve analytics for."""
     browser: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'browser', 'style': 'form', 'explode': True }})
     r"""The browser to retrieve analytics for."""
@@ -320,23 +322,23 @@
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetRefererAnalyticsResponseBody:
-    referer: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('referer') }})
-    r"""The name of the referer. If unknown, this will be `(direct)`"""
+class GetOSByClicksDeprecatedResponseBody:
+    os: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('os') }})
+    r"""The name of the OS"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
-    r"""The number of clicks from this referer"""
+    r"""The number of clicks from this OS"""
     
 
 
 
 @dataclasses.dataclass
-class GetRefererAnalyticsResponse:
+class GetOSByClicksDeprecatedResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    response_bodies: Optional[List[GetRefererAnalyticsResponseBody]] = dataclasses.field(default=None)
-    r"""The top referers by number of clicks"""
+    response_bodies: Optional[List[GetOSByClicksDeprecatedResponseBody]] = dataclasses.field(default=None)
+    r"""The top OS by number of clicks"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/gettags.py` & `dub-0.0.4/src/dub/models/operations/gettags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/gettimeseriesanalytics.py` & `dub-0.0.4/src/dub/models/operations/getdevicesbyclicks.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetTimeseriesAnalyticsGlobals:
+class GetDevicesByClicksGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
-class QueryParamInterval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+
+class GetDevicesByClicksQueryParamInterval(str, Enum):
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
-class QueryParamCountry(str, Enum):
+
+class GetDevicesByClicksQueryParamCountry(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -279,30 +281,30 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetTimeseriesAnalyticsRequest:
+class GetDevicesByClicksRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[QueryParamInterval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[GetDevicesByClicksQueryParamInterval] = dataclasses.field(default=GetDevicesByClicksQueryParamInterval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
-    country: Optional[QueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
+    country: Optional[GetDevicesByClicksQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
     r"""The city to retrieve analytics for."""
     device: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'device', 'style': 'form', 'explode': True }})
     r"""The device to retrieve analytics for."""
     browser: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'browser', 'style': 'form', 'explode': True }})
     r"""The browser to retrieve analytics for."""
@@ -320,23 +322,23 @@
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ResponseBody:
-    start: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start') }})
-    r"""The starting timestamp of the interval"""
+class GetDevicesByClicksResponseBody:
+    device: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('device') }})
+    r"""The name of the device"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
-    r"""The number of clicks in the interval"""
+    r"""The number of clicks from this device"""
     
 
 
 
 @dataclasses.dataclass
-class GetTimeseriesAnalyticsResponse:
+class GetDevicesByClicksResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    response_bodies: Optional[List[ResponseBody]] = dataclasses.field(default=None)
-    r"""The number of clicks over a period of time"""
+    response_bodies: Optional[List[GetDevicesByClicksResponseBody]] = dataclasses.field(default=None)
+    r"""The top devices by number of clicks"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/gettoplinks.py` & `dub-0.0.4/src/dub/models/operations/gettopurlsbyclicks.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetTopLinksGlobals:
+class GetTopURLsByClicksGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
-class GetTopLinksQueryParamInterval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+
+class GetTopURLsByClicksQueryParamInterval(str, Enum):
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
-class GetTopLinksQueryParamCountry(str, Enum):
+
+class GetTopURLsByClicksQueryParamCountry(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -279,30 +281,30 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetTopLinksRequest:
+class GetTopURLsByClicksRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[GetTopLinksQueryParamInterval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[GetTopURLsByClicksQueryParamInterval] = dataclasses.field(default=GetTopURLsByClicksQueryParamInterval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
-    country: Optional[GetTopLinksQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
+    country: Optional[GetTopURLsByClicksQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
     r"""The city to retrieve analytics for."""
     device: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'device', 'style': 'form', 'explode': True }})
     r"""The device to retrieve analytics for."""
     browser: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'browser', 'style': 'form', 'explode': True }})
     r"""The browser to retrieve analytics for."""
@@ -320,23 +322,23 @@
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetTopLinksResponseBody:
-    link: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('link') }})
-    r"""The unique ID of the short link"""
+class GetTopURLsByClicksResponseBody:
+    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
+    r"""The destination URL"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
-    r"""The number of clicks from this link"""
+    r"""The number of clicks from this URL"""
     
 
 
 
 @dataclasses.dataclass
-class GetTopLinksResponse:
+class GetTopURLsByClicksResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    response_bodies: Optional[List[GetTopLinksResponseBody]] = dataclasses.field(default=None)
-    r"""The top links by number of clicks"""
+    response_bodies: Optional[List[GetTopURLsByClicksResponseBody]] = dataclasses.field(default=None)
+    r"""The top URLs by number of clicks"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/gettopurls.py` & `dub-0.0.4/src/dub/models/operations/gettopurlsbyclicksdeprecated.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
 from enum import Enum
 from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetTopURLsGlobals:
+class GetTopURLsByClicksDeprecatedGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
-class GetTopURLsQueryParamInterval(str, Enum):
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+
+class GetTopURLsByClicksDeprecatedQueryParamInterval(str, Enum):
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     ONEH = '1h'
     TWENTY_FOURH = '24h'
     SEVEND = '7d'
     THIRTYD = '30d'
     NINETYD = '90d'
     YTD = 'ytd'
     ONEY = '1y'
     ALL = 'all'
 
-class GetTopURLsQueryParamCountry(str, Enum):
+
+class GetTopURLsByClicksDeprecatedQueryParamCountry(str, Enum):
     r"""The country to retrieve analytics for."""
     AF = 'AF'
     AL = 'AL'
     DZ = 'DZ'
     AS = 'AS'
     AD = 'AD'
     AO = 'AO'
@@ -279,30 +281,30 @@
     RS = 'RS'
     SX = 'SX'
     SS = 'SS'
     XK = 'XK'
 
 
 @dataclasses.dataclass
-class GetTopURLsRequest:
+class GetTopURLsByClicksDeprecatedRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
-    r"""The domain of the short link."""
+    r"""The domain to filter analytics for."""
     key: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'key', 'style': 'form', 'explode': True }})
     r"""The short link slug."""
     link_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'linkId', 'style': 'form', 'explode': True }})
     r"""The unique ID of the short link on Dub."""
     external_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'externalId', 'style': 'form', 'explode': True }})
     r"""This is the ID of the link in the your database. Must be prefixed with 'ext_' when passed as a query parameter."""
-    interval: Optional[GetTopURLsQueryParamInterval] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
-    r"""The interval to retrieve analytics for. Takes precedence over start and end."""
+    interval: Optional[GetTopURLsByClicksDeprecatedQueryParamInterval] = dataclasses.field(default=GetTopURLsByClicksDeprecatedQueryParamInterval.TWENTY_FOURH, metadata={'query_param': { 'field_name': 'interval', 'style': 'form', 'explode': True }})
+    r"""The interval to retrieve analytics for. Takes precedence over start and end. If undefined, defaults to 24h."""
     start: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'start', 'style': 'form', 'explode': True }})
     r"""The start date and time when to retrieve analytics from."""
     end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end', 'style': 'form', 'explode': True }})
     r"""The end date and time when to retrieve analytics from. If not provided, defaults to the current date."""
-    country: Optional[GetTopURLsQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
+    country: Optional[GetTopURLsByClicksDeprecatedQueryParamCountry] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country', 'style': 'form', 'explode': True }})
     r"""The country to retrieve analytics for."""
     city: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'city', 'style': 'form', 'explode': True }})
     r"""The city to retrieve analytics for."""
     device: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'device', 'style': 'form', 'explode': True }})
     r"""The device to retrieve analytics for."""
     browser: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'browser', 'style': 'form', 'explode': True }})
     r"""The browser to retrieve analytics for."""
@@ -320,23 +322,23 @@
     r"""Filter for root domains. If true, filter for domains only. If false, filter for links only. If undefined, return both."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetTopURLsResponseBody:
+class GetTopURLsByClicksDeprecatedResponseBody:
     url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
     r"""The destination URL"""
     clicks: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks') }})
     r"""The number of clicks from this URL"""
     
 
 
 
 @dataclasses.dataclass
-class GetTopURLsResponse:
+class GetTopURLsByClicksDeprecatedResponse:
     http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    response_bodies: Optional[List[GetTopURLsResponseBody]] = dataclasses.field(default=None)
+    response_bodies: Optional[List[GetTopURLsByClicksDeprecatedResponseBody]] = dataclasses.field(default=None)
     r"""The top URLs by number of clicks"""
```

### Comparing `dub-0.0.3/src/dub/models/operations/getworkspace.py` & `dub-0.0.4/src/dub/models/operations/getworkspace.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/getworkspaces.py` & `dub-0.0.4/src/dub/models/operations/getworkspaces.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/listdomains.py` & `dub-0.0.4/src/dub/models/operations/listdomains.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/setprimarydomain.py` & `dub-0.0.4/src/dub/models/operations/setprimarydomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/transferdomain.py` & `dub-0.0.4/src/dub/models/operations/transferdomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/updatedomain.py` & `dub-0.0.4/src/dub/models/operations/updatedomain.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class UpdateDomainGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
+
 class UpdateDomainType(str, Enum):
     r"""The type of redirect to use for this domain."""
     REDIRECT = 'redirect'
     REWRITE = 'rewrite'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `dub-0.0.3/src/dub/models/operations/updatelink.py` & `dub-0.0.4/src/dub/models/operations/updatelink.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/models/operations/upsertlink.py` & `dub-0.0.4/src/dub/models/operations/upsertlink.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/qr_codes.py` & `dub-0.0.4/src/dub/qr_codes.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/sdk.py` & `dub-0.0.4/src/dub/sdk.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/sdkconfiguration.py` & `dub-0.0.4/src/dub/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '0.0.1'
-    sdk_version: str = '0.0.3'
-    gen_version: str = '2.329.0'
-    user_agent: str = 'speakeasy-sdk/python 0.0.3 2.329.0 0.0.1 dub'
+    sdk_version: str = '0.0.4'
+    gen_version: str = '2.332.4'
+    user_agent: str = 'speakeasy-sdk/python 0.0.4 2.332.4 0.0.1 dub'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `dub-0.0.3/src/dub/tags.py` & `dub-0.0.4/src/dub/tags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/utils/retries.py` & `dub-0.0.4/src/dub/utils/retries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/utils/utils.py` & `dub-0.0.4/src/dub/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub/workspaces.py` & `dub-0.0.4/src/dub/workspaces.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.3/src/dub.egg-info/PKG-INFO` & `dub-0.0.4/src/dub.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dub
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # dub
         
         <div align="left">
@@ -101,24 +101,37 @@
         
         ### [qr_codes](https://github.com/dubinc/dub-python/blob/master/docs/sdks/qrcodes/README.md)
         
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/qrcodes/README.md#get) - Retrieve a QR code
         
         ### [analytics](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md)
         
-        * [clicks](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#clicks) - Retrieve clicks analytics
-        * [timeseries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries analytics
-        * [countries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#countries) - Retrieve country analytics
-        * [cities](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#cities) - Retrieve city analytics
-        * [devices](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#devices) - Retrieve device analytics
-        * [browsers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#browsers) - Retrieve browser analytics
-        * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve OS analytics
-        * [referers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referers) - Retrieve referer analytics
-        * [top_links](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_links) - Retrieve top links
-        * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs
+        * [~~timeseries~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics :warning: **Deprecated** Use `timeseries` instead.
+        * [~~country~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#country) - Retrieve top countries by clicks :warning: **Deprecated** Use `countries` instead.
+        * [~~city~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning: **Deprecated** Use `cities` instead.
+        * [~~device~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#device) - Retrieve top devices by clicks :warning: **Deprecated** Use `devices` instead.
+        * [~~browser~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#browser) - Retrieve top browsers by clicks :warning: **Deprecated** Use `browsers` instead.
+        * [~~os~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve top OS by clicks :warning: **Deprecated** Use `os` instead.
+        * [~~referer~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referer) - Retrieve top referers by clicks :warning: **Deprecated** Use `referers` instead.
+        * [~~top_links~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :warning: **Deprecated** Use `top_links` instead.
+        * [~~top_urls~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use `top_urls` instead.
+        
+        ### [analytics.clicks](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md)
+        
+        * [count](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#count) - Retrieve the total clicks count
+        * [timeseries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click analytics
+        * [countries](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#countries) - Retrieve top countries by clicks
+        * [cities](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#cities) - Retrieve top cities by clicks
+        * [devices](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#devices) - Retrieve top devices by clicks
+        * [browsers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#browsers) - Retrieve top browsers by clicks
+        * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#os) - Retrieve top OS by clicks
+        * [referers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#referers) - Retrieve top referers by clicks
+        * [top_links](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#top_links) - Retrieve top links by clicks
+        * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks
+        * [~~get_clicks_count_deprecated~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the total clicks count :warning: **Deprecated** Use `count` instead.
         
         ### [workspaces](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md)
         
         * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces
         * [create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#create) - Create a workspace
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#get) - Retrieve a workspace
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dub Version: 0.0.3 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: dub Version: 0.0.4 Summary: Python Client SDK
 Generated by Speakeasy Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy License: UNKNOWN Description: # dub
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## ð **Welcome to your new SDK!** ð It has been generated successfully
 based on your OpenAPI spec. However, it is not yet ready for production use.
@@ -36,65 +36,91 @@
 Update a link * [create_many](https://github.com/dubinc/dub-python/blob/master/
 docs/sdks/links/README.md#create_many) - Bulk create links * [upsert](https://
 github.com/dubinc/dub-python/blob/master/docs/sdks/links/README.md#upsert) -
 Upsert a link ### [qr_codes](https://github.com/dubinc/dub-python/blob/master/
 docs/sdks/qrcodes/README.md) * [get](https://github.com/dubinc/dub-python/blob/
 master/docs/sdks/qrcodes/README.md#get) - Retrieve a QR code ### [analytics]
 (https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md) * [clicks](https://github.com/dubinc/dub-python/blob/master/docs/
-sdks/analytics/README.md#clicks) - Retrieve clicks analytics * [timeseries]
-(https://github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md#timeseries) - Retrieve timeseries analytics * [countries](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md#countries) - Retrieve country analytics * [cities](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#cities)
-- Retrieve city analytics * [devices](https://github.com/dubinc/dub-python/
-blob/master/docs/sdks/analytics/README.md#devices) - Retrieve device analytics
-* [browsers](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-analytics/README.md#browsers) - Retrieve browser analytics * [os](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#os) -
-Retrieve OS analytics * [referers](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/analytics/README.md#referers) - Retrieve referer analytics *
-[top_links](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-analytics/README.md#top_links) - Retrieve top links * [top_urls](https://
+README.md) * [~~timeseries~~](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/analytics/README.md#timeseries) - Retrieve timeseries click analytics
+:warning: **Deprecated** Use `timeseries` instead. * [~~country~~](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#country)
+- Retrieve top countries by clicks :warning: **Deprecated** Use `countries`
+instead. * [~~city~~](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/analytics/README.md#city) - Retrieve top cities by clicks :warning:
+**Deprecated** Use `cities` instead. * [~~device~~](https://github.com/dubinc/
+dub-python/blob/master/docs/sdks/analytics/README.md#device) - Retrieve top
+devices by clicks :warning: **Deprecated** Use `devices` instead. *
+[~~browser~~](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+analytics/README.md#browser) - Retrieve top browsers by clicks :warning:
+**Deprecated** Use `browsers` instead. * [~~os~~](https://github.com/dubinc/
+dub-python/blob/master/docs/sdks/analytics/README.md#os) - Retrieve top OS by
+clicks :warning: **Deprecated** Use `os` instead. * [~~referer~~](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/README.md#referer)
+- Retrieve top referers by clicks :warning: **Deprecated** Use `referers`
+instead. * [~~top_links~~](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/analytics/README.md#top_links) - Retrieve top links by clicks :
+warning: **Deprecated** Use `top_links` instead. * [~~top_urls~~](https://
 github.com/dubinc/dub-python/blob/master/docs/sdks/analytics/
-README.md#top_urls) - Retrieve top URLs ### [workspaces](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md) * [list](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/README.md#list) -
-Retrieve a list of workspaces * [create](https://github.com/dubinc/dub-python/
-blob/master/docs/sdks/workspaces/README.md#create) - Create a workspace * [get]
-(https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/
-README.md#get) - Retrieve a workspace ### [tags](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/tags/README.md) * [list](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/tags/README.md#list) - Retrieve a list
-of tags * [create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
-tags/README.md#create) - Create a new tag ### [domains](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/domains/README.md) * [list](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#list) -
-Retrieve a list of domains * [add](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/domains/README.md#add) - Add a domain * [delete](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#delete) -
-Delete a domain * [update](https://github.com/dubinc/dub-python/blob/master/
-docs/sdks/domains/README.md#update) - Update a domain * [set_primary](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
-README.md#set_primary) - Set a domain as primary * [transfer](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#transfer)
-- Transfer a domain ### [metatags](https://github.com/dubinc/dub-python/blob/
-master/docs/sdks/metatags/README.md) * [get](https://github.com/dubinc/dub-
-python/blob/master/docs/sdks/metatags/README.md#get) - Retrieve the metatags
-for a URL ## Error Handling Handling errors in this SDK should largely match
-your expectations. All operations return a response object or raise an error.
-If Error objects are specified in your OpenAPI Spec, the SDK will raise the
-appropriate Error type. | Error Object | Status Code | Content Type | | -------
-------------------- | -------------------------- | -------------------------- |
-| errors.BadRequest | 400 | application/json | | errors.Unauthorized | 401 |
-application/json | | errors.Forbidden | 403 | application/json | |
-errors.NotFound | 404 | application/json | | errors.Conflict | 409 |
-application/json | | errors.InviteExpired | 410 | application/json | |
-errors.UnprocessableEntity | 422 | application/json | |
+README.md#top_urls) - Retrieve top URLs by clicks :warning: **Deprecated** Use
+`top_urls` instead. ### [analytics.clicks](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/clicks/README.md) * [count](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#count) - Retrieve the
+total clicks count * [timeseries](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/clicks/README.md#timeseries) - Retrieve timeseries click
+analytics * [countries](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/clicks/README.md#countries) - Retrieve top countries by clicks * [cities]
+(https://github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/
+README.md#cities) - Retrieve top cities by clicks * [devices](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#devices) -
+Retrieve top devices by clicks * [browsers](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/clicks/README.md#browsers) - Retrieve top browsers
+by clicks * [os](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+clicks/README.md#os) - Retrieve top OS by clicks * [referers](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/clicks/README.md#referers) -
+Retrieve top referers by clicks * [top_links](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/clicks/README.md#top_links) - Retrieve top links
+by clicks * [top_urls](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/clicks/README.md#top_urls) - Retrieve top URLs by clicks *
+[~~get_clicks_count_deprecated~~](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/clicks/README.md#get_clicks_count_deprecated) - Retrieve the
+total clicks count :warning: **Deprecated** Use `count` instead. ###
+[workspaces](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+workspaces/README.md) * [list](https://github.com/dubinc/dub-python/blob/
+master/docs/sdks/workspaces/README.md#list) - Retrieve a list of workspaces *
+[create](https://github.com/dubinc/dub-python/blob/master/docs/sdks/workspaces/
+README.md#create) - Create a workspace * [get](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/workspaces/README.md#get) - Retrieve a workspace
+### [tags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/tags/
+README.md) * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+tags/README.md#list) - Retrieve a list of tags * [create](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/tags/README.md#create) - Create a new
+tag ### [domains](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+domains/README.md) * [list](https://github.com/dubinc/dub-python/blob/master/
+docs/sdks/domains/README.md#list) - Retrieve a list of domains * [add](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#add) - Add
+a domain * [delete](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+domains/README.md#delete) - Delete a domain * [update](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/domains/README.md#update) - Update a
+domain * [set_primary](https://github.com/dubinc/dub-python/blob/master/docs/
+sdks/domains/README.md#set_primary) - Set a domain as primary * [transfer]
+(https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
+README.md#transfer) - Transfer a domain ### [metatags](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/metatags/README.md) * [get](https://
+github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/README.md#get) -
+Retrieve the metatags for a URL ## Error Handling Handling errors in this SDK
+should largely match your expectations. All operations return a response object
+or raise an error. If Error objects are specified in your OpenAPI Spec, the SDK
+will raise the appropriate Error type. | Error Object | Status Code | Content
+Type | | -------------------------- | -------------------------- | ------------
+-------------- | | errors.BadRequest | 400 | application/json | |
+errors.Unauthorized | 401 | application/json | | errors.Forbidden | 403 |
+application/json | | errors.NotFound | 404 | application/json | |
+errors.Conflict | 409 | application/json | | errors.InviteExpired | 410 |
+application/json | | errors.UnprocessableEntity | 422 | application/json | |
 errors.RateLimitExceeded | 429 | application/json | |
 errors.InternalServerError | 500 | application/json | | errors.SDKError | 4xx-
 5xx | */* | ### Example ```python import dub from dub.models import errors,
 operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res = None try:
 res = s.links.list(request=operations.GetLinksRequest()) except
 errors.BadRequest as e: # handle exception raise(e) except errors.Unauthorized
 as e: # handle exception raise(e) except errors.Forbidden as e: # handle
```

### Comparing `dub-0.0.3/src/dub.egg-info/SOURCES.txt` & `dub-0.0.4/src/dub.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 src/dub/__init__.py
 src/dub/analytics.py
+src/dub/clicks.py
 src/dub/domains.py
 src/dub/links.py
 src/dub/metatags.py
 src/dub/qr_codes.py
 src/dub/sdk.py
 src/dub/sdkconfiguration.py
 src/dub/tags.py
@@ -44,30 +45,40 @@
 src/dub/models/operations/adddomain.py
 src/dub/models/operations/bulkcreatelinks.py
 src/dub/models/operations/createlink.py
 src/dub/models/operations/createtag.py
 src/dub/models/operations/createworkspace.py
 src/dub/models/operations/deletedomain.py
 src/dub/models/operations/deletelink.py
-src/dub/models/operations/getbrowseranalytics.py
-src/dub/models/operations/getcityanalytics.py
-src/dub/models/operations/getclicksanalytics.py
-src/dub/models/operations/getcountryanalytics.py
-src/dub/models/operations/getdeviceanalytics.py
+src/dub/models/operations/getbrowsersbyclicks.py
+src/dub/models/operations/getbrowsersbyclicksdeprecated.py
+src/dub/models/operations/getcitiesbyclicks.py
+src/dub/models/operations/getcitiesbyclicksdeprecated.py
+src/dub/models/operations/getclickscount.py
+src/dub/models/operations/getclickscountdeprecated.py
+src/dub/models/operations/getcountriesbyclicks.py
+src/dub/models/operations/getcountriesbyclicksdeprecated.py
+src/dub/models/operations/getdevicesbyclicks.py
+src/dub/models/operations/getdevicesbyclicksdeprecated.py
 src/dub/models/operations/getlinkinfo.py
 src/dub/models/operations/getlinks.py
 src/dub/models/operations/getlinkscount.py
 src/dub/models/operations/getmetatags.py
-src/dub/models/operations/getosanalytics.py
+src/dub/models/operations/getosbyclicks.py
+src/dub/models/operations/getosbyclicksdeprecated.py
 src/dub/models/operations/getqrcode.py
-src/dub/models/operations/getrefereranalytics.py
+src/dub/models/operations/getreferersbyclicks.py
+src/dub/models/operations/getreferersbyclicksdeprecated.py
 src/dub/models/operations/gettags.py
-src/dub/models/operations/gettimeseriesanalytics.py
-src/dub/models/operations/gettoplinks.py
-src/dub/models/operations/gettopurls.py
+src/dub/models/operations/gettimeseriesbyclicks.py
+src/dub/models/operations/gettimeseriesbyclicksdeprecated.py
+src/dub/models/operations/gettoplinksbyclicks.py
+src/dub/models/operations/gettoplinksbyclicksdeprecated.py
+src/dub/models/operations/gettopurlsbyclicks.py
+src/dub/models/operations/gettopurlsbyclicksdeprecated.py
 src/dub/models/operations/getworkspace.py
 src/dub/models/operations/getworkspaces.py
 src/dub/models/operations/listdomains.py
 src/dub/models/operations/setprimarydomain.py
 src/dub/models/operations/transferdomain.py
 src/dub/models/operations/updatedomain.py
 src/dub/models/operations/updatelink.py
```

