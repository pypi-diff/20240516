# Comparing `tmp/netlink-sharepoint-base-0.0.6.tar.gz` & `tmp/netlink-sharepoint-base-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlink-sharepoint-base-0.0.6.tar", max compression
+gzip compressed data, was "netlink-sharepoint-base-0.0.7.tar", max compression
```

## Comparing `netlink-sharepoint-base-0.0.6.tar` & `netlink-sharepoint-base-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       50 2022-07-13 08:54:46.518861 netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/__init__.py
--rw-r--r--   0        0        0     2686 2023-12-13 16:04:05.633760 netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/_item.py
--rw-r--r--   0        0        0     3110 2023-11-14 10:50:38.048783 netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/_list.py
--rw-r--r--   0        0        0     3657 2023-11-13 09:15:05.505608 netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/_site.py
--rw-r--r--   0        0        0      872 2022-10-07 07:52:55.376943 netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/classes.puml
--rw-r--r--   0        0        0     1831 2022-10-07 07:52:55.392564 netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/cli.py
--rw-r--r--   0        0        0      944 2023-12-13 16:04:06.450756 netlink-sharepoint-base-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4284 2022-07-14 14:37:36.840787 netlink-sharepoint-base-0.0.6/README.md
--rw-r--r--   0        0        0     5454 2023-12-13 16:06:27.100756 netlink-sharepoint-base-0.0.6/setup.py
--rw-r--r--   0        0        0     5234 2023-12-13 16:06:27.100756 netlink-sharepoint-base-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       50 2022-07-13 08:54:46.518861 netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/__init__.py
+-rw-r--r--   0        0        0     2686 2023-12-13 16:04:05.633760 netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/_item.py
+-rw-r--r--   0        0        0     3110 2023-11-14 10:50:38.048783 netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/_list.py
+-rw-r--r--   0        0        0     3675 2024-02-13 08:06:15.447013 netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/_site.py
+-rw-r--r--   0        0        0      872 2022-10-07 07:52:55.376943 netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/classes.puml
+-rw-r--r--   0        0        0     1831 2022-10-07 07:52:55.392564 netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/cli.py
+-rw-r--r--   0        0        0      949 2024-02-13 08:08:32.029277 netlink-sharepoint-base-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4284 2022-07-14 14:37:36.840787 netlink-sharepoint-base-0.0.7/README.md
+-rw-r--r--   0        0        0     5425 2024-02-13 08:11:32.336296 netlink-sharepoint-base-0.0.7/setup.py
+-rw-r--r--   0        0        0     5205 2024-02-13 08:11:32.337342 netlink-sharepoint-base-0.0.7/PKG-INFO
```

### Comparing `netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/_item.py` & `netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/_item.py`

 * *Files identical despite different names*

### Comparing `netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/_list.py` & `netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/_list.py`

 * *Files identical despite different names*

### Comparing `netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/_site.py` & `netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/_site.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class Site:
     _url = ""
     _client_id = ""
     _client_secret = ""
 
-    def __init__(self, url: str = None, client_id: str = None, client_secret: str = None):
+    def __init__(self, url: str = None, client_id: str = None, client_secret: str = None, **kwargs) -> None:
         self._context = ClientContext(url or self._url).with_credentials(
             ClientCredential(client_id=client_id or self._client_id, client_secret=client_secret or self._client_secret)
         )
         logger.debug(f"Initialized connection Sharepoint as {self.url}")
         self._users = None
         self._lists = {}
```

### Comparing `netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/classes.puml` & `netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/classes.puml`

 * *Files identical despite different names*

### Comparing `netlink-sharepoint-base-0.0.6/netlink/sharepoint/base/cli.py` & `netlink-sharepoint-base-0.0.7/netlink/sharepoint/base/cli.py`

 * *Files identical despite different names*

### Comparing `netlink-sharepoint-base-0.0.6/pyproject.toml` & `netlink-sharepoint-base-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "netlink-sharepoint-base"
-version = "0.0.6"
+version = "0.0.7"
 description = "Basic Tools for interaction with Sharepoint Sites"
 license = "MIT"
 authors = ["Bernhard Radermacher <bernhard.radermacher@netlink-consulting.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/netlink_python/netlink-sharepoint-base"
 keywords = ["sharepoint"]
 classifiers = ["Topic :: Software Development"]
 packages = [ { include = "netlink/sharepoint/base" } ]
 
 [tool.poetry.scripts]
 sharepoint_list_info = 'netlink.sharepoint.base.cli:print_list_info'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-netlink-logging = "^0.1.14"
-Office365-REST-Python-Client = "^2.3.12"
-click = "^8.1.3"
-toml = "^0.10.2"
+netlink-logging = ">=0.1.14"
+Office365-REST-Python-Client = ">=2.3.12"
+click = ">=8.1.3"
+toml = ">=0.10.2"
 
 [tool.poetry.dev-dependencies]
-black = "^23.12.0"
+black = ">=23.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `netlink-sharepoint-base-0.0.6/README.md` & `netlink-sharepoint-base-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `netlink-sharepoint-base-0.0.6/setup.py` & `netlink-sharepoint-base-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 packages = \
 ['base']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Office365-REST-Python-Client>=2.3.12,<3.0.0',
- 'click>=8.1.3,<9.0.0',
- 'netlink-logging>=0.1.14,<0.2.0',
- 'toml>=0.10.2,<0.11.0']
+['Office365-REST-Python-Client>=2.3.12',
+ 'click>=8.1.3',
+ 'netlink-logging>=0.1.14',
+ 'toml>=0.10.2']
 
 entry_points = \
 {'console_scripts': ['sharepoint_list_info = '
                      'netlink.sharepoint.base.cli:print_list_info']}
 
 setup_kwargs = {
     'name': 'netlink-sharepoint-base',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Basic Tools for interaction with Sharepoint Sites',
     'long_description': '# netlink-sharepoint-base\n\n## Basic Tools for interaction with Sharepoint Sites\n\nThis has been moved from `netlink-sharepoint`\n\nFor now only **Lists** are considered.\n\n## `sharepoint_list_info`\n\nScript to help mapping\n\n```shell\nUsage: sharepoint_list_info.py [OPTIONS] [NAME]...\n\n  Print information about SharePoint List(s)\n\n  NAME is not provided, all lists are returned.\n\nOptions:\n  -u, --url           TEXT  Sharepoint URL\n  -i, --client-id     TEXT  Client ID\n  -s, --client-secret TEXT  Client Secret\n  -t, --toml          FILE  TOML file with \'url\', \'client_id\', and \'client_secret\'\n  -f, --fields              include fields\n  --hidden                  include hidden lists (and fields)\n```\n\n## `netlink.sharepoint.base.Site`\n\nMain class representing a Sharepoint site. Can either be used directly providing the parameters\n\n- url\n- client_id\n- client_secret\n\nor inherited from\n\n```python\nfrom netlink.sharepoint.base import Site as _Site\n\n\nclass Site(_Site):\n    _url = "https://somewhere.sharepoint.com/sites/something"\n    _client_id = "00000000-0000-0000-0000-000000000000"\n    _client_secret = "abcdefghijklmnopqrstuvwxyz01234567890+/abcd="\n```\n\n### url\n\n_read-only_\n\n### users\n\n_read-only (always a copy of the actual data)_\n\nDict of the users of the site.\n\n| Column | Type | Description |\n|--------|:-----:|-----|\n| id | int | reference key for AuthorID, EditorID, etc. |\n| family_name | str | a.k.a. last name |\n| given_name | str | a.k.a. first name |\n| name | str | {family_name}, {given_name} |\n| email | str | |\n\n**Note** This is based on a default Sharepoint setup. This might not work for you.\n\n### get_list(name)\n\nReturns a Sharepoint List object (`office365.sharepoint.lists.list.List`) by **name**.\n\n### get_lists(hidden=False)\n\nReturns a list of Sharepoint List objects (`office365.sharepoint.lists.list.List`). If `hidden` is `True`, internal\nLists are included.\n\n### get_list_items(name)\n\nReturns list of all items (`office365.sharepoint.listitems.listitem.ListItem`) from **name**d Sharepoint List.\n\n### get_list_columns(name, hidden=False)\n\nReturns list of columns (a.k.a. Fields) of the **name**d Sharepoint List. If `hidden` is `True`, internal columns are\nincluded.\n\n### commit()\n\nSend all pending updates to Sharepoint.\n\n## `netlink.sharepoint.base.List`\n\nClass representing a Sharepoint List. This is a `collections.abc.Mapping`. Contents are mapped with the unique `id` of\nthe item in the Sharepoint List.\n\nWhen inherited from, class attribute\n\n- `_title` must be set.\n\n- `_map` should be set, but can be overridden. This maps the python name (best to use a valid attribute-name)\n  to the respective internal Sharepoint name. Do not map \'id\' or \'ID\', this is done automatically as the primary key.\n\n- `_upper_case` can be set to be used in `normalize` to enforce that the respective columns are set to uppercase.\n\n- `_required` can be set to ensure that the respective columns are not empty (as defined by Python: `None`, empty\n  string, or numeric zero).\n\nAt this point very optimistic (as in none-at-all) locking is used.\n\nThe item itself keeps information if data has been changed.\n\n### load()\n\nLoads all items from the Sharepoint List.\n\n### rollback()\n\nClears all local entries and calls `load`. At this time there is no difference, but when adding items will be supported,\nthis would clear them.\n\n### get(item, buffered=True)\n\nLoads (if nor already loaded) item based on unique `id`. If `buffered` is `False`, read from Sharepoint is forced.\n\n### commit()\n\nCommit all changed items to Sharepoint.\n\n### normalize()\n\nProcesses `_upper_case` for all items.\n\nConsider overriding this to set columns based on other columns.\n\n### validate()\n\nProcesses `_required` for all items.\n\nConsider overriding this to check list-wide constraints, like composite unique keys.\n\n## Item\n\nThis is a special class that gets build dynamically for each List. It is a `collections.abc.MutableMapping`.\n\nIt handles keeping state of changes and processes the actual mapping between Python and Sharepoint columns (fields).\n\n### commit(lazy=False)\n\nUpdate the internal `office365.sharepoint.listitems.listitem.ListItem` with any pending changes. If `lazy` is `True`,\nchanges are not sent to Sharepoint, providing the option to send on List or Site level.\n\n## License\n\nMIT\n',
     'author': 'Bernhard Radermacher',
     'author_email': 'bernhard.radermacher@netlink-consulting.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/netlink_python/netlink-sharepoint-base',
```

### Comparing `netlink-sharepoint-base-0.0.6/PKG-INFO` & `netlink-sharepoint-base-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: netlink-sharepoint-base
-Version: 0.0.6
+Version: 0.0.7
 Summary: Basic Tools for interaction with Sharepoint Sites
 Home-page: https://gitlab.com/netlink_python/netlink-sharepoint-base
 License: MIT
 Keywords: sharepoint
 Author: Bernhard Radermacher
 Author-email: bernhard.radermacher@netlink-consulting.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
-Requires-Dist: Office365-REST-Python-Client (>=2.3.12,<3.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: netlink-logging (>=0.1.14,<0.2.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: Office365-REST-Python-Client (>=2.3.12)
+Requires-Dist: click (>=8.1.3)
+Requires-Dist: netlink-logging (>=0.1.14)
+Requires-Dist: toml (>=0.10.2)
 Project-URL: Repository, https://gitlab.com/netlink_python/netlink-sharepoint-base
 Description-Content-Type: text/markdown
 
 # netlink-sharepoint-base
 
 ## Basic Tools for interaction with Sharepoint Sites
```

