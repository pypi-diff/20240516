# Comparing `tmp/netlink-sharepoint-alchemy-0.0.4.tar.gz` & `tmp/netlink-sharepoint-alchemy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlink-sharepoint-alchemy-0.0.4.tar", max compression
+gzip compressed data, was "netlink-sharepoint-alchemy-0.0.5.tar", max compression
```

## Comparing `netlink-sharepoint-alchemy-0.0.4.tar` & `netlink-sharepoint-alchemy-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       31 2022-07-13 08:03:43.045725 netlink-sharepoint-alchemy-0.0.4/netlink/sharepoint/alchemy/__init__.py
--rw-r--r--   0        0        0     6995 2023-12-13 16:09:58.227848 netlink-sharepoint-alchemy-0.0.4/netlink/sharepoint/alchemy/_base.py
--rw-r--r--   0        0        0      854 2023-12-13 16:11:12.339120 netlink-sharepoint-alchemy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1526 2022-07-13 13:12:52.973899 netlink-sharepoint-alchemy-0.0.4/README.md
--rw-r--r--   0        0        0     2374 2023-12-13 16:11:31.004275 netlink-sharepoint-alchemy-0.0.4/setup.py
--rw-r--r--   0        0        0     2388 2023-12-13 16:11:31.004275 netlink-sharepoint-alchemy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       31 2022-07-13 08:03:43.045725 netlink-sharepoint-alchemy-0.0.5/netlink/sharepoint/alchemy/__init__.py
+-rw-r--r--   0        0        0     6995 2023-12-13 16:09:58.227848 netlink-sharepoint-alchemy-0.0.5/netlink/sharepoint/alchemy/_base.py
+-rw-r--r--   0        0        0      858 2024-02-13 08:21:31.852985 netlink-sharepoint-alchemy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1526 2022-07-13 13:12:52.973899 netlink-sharepoint-alchemy-0.0.5/README.md
+-rw-r--r--   0        0        0     2360 2024-02-13 08:25:02.475483 netlink-sharepoint-alchemy-0.0.5/setup.py
+-rw-r--r--   0        0        0     2374 2024-02-13 08:25:02.476631 netlink-sharepoint-alchemy-0.0.5/PKG-INFO
```

### Comparing `netlink-sharepoint-alchemy-0.0.4/netlink/sharepoint/alchemy/_base.py` & `netlink-sharepoint-alchemy-0.0.5/netlink/sharepoint/alchemy/_base.py`

 * *Files identical despite different names*

### Comparing `netlink-sharepoint-alchemy-0.0.4/pyproject.toml` & `netlink-sharepoint-alchemy-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "netlink-sharepoint-alchemy"
-version = "0.0.4"
+version = "0.0.5"
 description = "Integrate Sharepoint and SQL Alchemy"
 license = "MIT"
 authors = ["Bernhard Radermacher <bernhard.radermacher@netlink-consulting.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/netlink_python/netlink-sharepoint-alchemy"
 keywords = ["sharepoint"]
 classifiers = ["Topic :: Software Development"]
 packages = [ { include = "netlink/sharepoint/alchemy" } ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-netlink-sharepoint-base = "^0.0.6"
-netlink-alchemy = "^0.0.1"
+netlink-sharepoint-base = ">=0.0.6"
+netlink-alchemy = ">=0.0.1"
 
 [tool.poetry.dev-dependencies]
-black = "^23.12.0"
-pytest = "^7.4.3"
+black = ">=23.12.0"
+pytest = ">=7.4.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `netlink-sharepoint-alchemy-0.0.4/README.md` & `netlink-sharepoint-alchemy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `netlink-sharepoint-alchemy-0.0.4/setup.py` & `netlink-sharepoint-alchemy-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['alchemy']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['netlink-alchemy>=0.0.1,<0.0.2', 'netlink-sharepoint-base>=0.0.6,<0.0.7']
+['netlink-alchemy>=0.0.1', 'netlink-sharepoint-base>=0.0.6']
 
 setup_kwargs = {
     'name': 'netlink-sharepoint-alchemy',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Integrate Sharepoint and SQL Alchemy',
     'long_description': '# netlink-sharepoint-alchemy\n\nIntegration of Sharepoint and SQL Alchemy\n\n\nUse the pre-configured Base for Tables that reflect a Sharepoint list, and the ready-made \nORM mapped `User` to access the users of the Sharepoint.\n\n```python\nfrom netlink.sharepoint.alchemy import Base, User\n```\n\n`id` is part of `Base`.\n\nDefine a mapped list / table like this:\n\n```python\nfrom netlink.sharepoint.alchemy import Base\nfrom sqlalchemy import Column\nfrom sqlalchemy import String\nfrom netlink.alchemy import UnsignedInteger\n\n\nclass Action(Base):\n    __tablename__ = \'action\'\n    _sharepoint_list_title = "Action"\n\n    # fmt: off\n    action           = Column(String,           nullable=False, doc=\'Title\')\n    deadline         = Column(UnsignedInteger,  nullable=True, doc=\'Deadline\')\n    comment          = Column(String,           nullable=True, doc=\'Comment\')\n    # fmt: on\n```\n\nLoad data from Sharepoint (non-working, concept only)\n\n```python\nfrom sqlalchemy import create_engine\nfrom sqlalchemy.orm import Session\n\nfrom netlink.sharepoint.base import Site\nfrom netlink.sharepoint.alchemy import Base, User\n\n\nclass ActionControl(Base):\n    pass\n\n\nif __name__ == \'__main__\':\n    engine = create_engine(f"sqlite+pysqlite:///test.sqlite3", future=True)\n    Base.metadata.create_all(engine)\n    sharepoint = Site()\n    session = Session(engine)\n\n    User.bind_to_sharepoint(sharepoint)\n    User.load_from_sharepoint_list(session)\n\n    ActionControl.bind_to_sharepoint(sharepoint)\n    ActionControl.load_from_sharepoint_list(session)\n```\n\n',
     'author': 'Bernhard Radermacher',
     'author_email': 'bernhard.radermacher@netlink-consulting.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/netlink_python/netlink-sharepoint-alchemy',
```

### Comparing `netlink-sharepoint-alchemy-0.0.4/PKG-INFO` & `netlink-sharepoint-alchemy-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: netlink-sharepoint-alchemy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Integrate Sharepoint and SQL Alchemy
 Home-page: https://gitlab.com/netlink_python/netlink-sharepoint-alchemy
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
-Requires-Dist: netlink-alchemy (>=0.0.1,<0.0.2)
-Requires-Dist: netlink-sharepoint-base (>=0.0.6,<0.0.7)
+Requires-Dist: netlink-alchemy (>=0.0.1)
+Requires-Dist: netlink-sharepoint-base (>=0.0.6)
 Project-URL: Repository, https://gitlab.com/netlink_python/netlink-sharepoint-alchemy
 Description-Content-Type: text/markdown
 
 # netlink-sharepoint-alchemy
 
 Integration of Sharepoint and SQL Alchemy
```

