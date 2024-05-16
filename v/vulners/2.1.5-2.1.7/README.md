# Comparing `tmp/vulners-2.1.5.tar.gz` & `tmp/vulners-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulners-2.1.5.tar", max compression
+gzip compressed data, was "vulners-2.1.7.tar", max compression
```

## Comparing `vulners-2.1.5.tar` & `vulners-2.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35141 2024-01-22 13:31:28.174269 vulners-2.1.5/LICENSE
--rw-r--r--   0        0        0     5904 2024-01-22 13:31:28.178269 vulners-2.1.5/README.md
--rw-r--r--   0        0        0     1226 2024-01-22 13:31:28.178269 vulners-2.1.5/pyproject.toml
--rw-r--r--   0        0        0      179 2024-01-22 13:31:28.178269 vulners-2.1.5/vulners/__init__.py
--rw-r--r--   0        0        0    19087 2024-01-22 13:31:28.178269 vulners-2.1.5/vulners/base.py
--rw-r--r--   0        0        0    11174 2024-01-22 13:31:28.178269 vulners-2.1.5/vulners/vscanner.py
--rw-r--r--   0        0        0    31300 2024-01-22 13:31:28.178269 vulners-2.1.5/vulners/vulners.py
--rw-r--r--   0        0        0     6789 2024-01-22 13:31:28.813980 vulners-2.1.5/setup.py
--rw-r--r--   0        0        0     7016 2024-01-22 13:31:28.814701 vulners-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35141 2024-05-16 19:39:23.374050 vulners-2.1.7/LICENSE
+-rw-r--r--   0        0        0     5904 2024-05-16 19:39:23.374050 vulners-2.1.7/README.md
+-rw-r--r--   0        0        0     1226 2024-05-16 19:39:23.374050 vulners-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0      179 2024-05-16 19:39:23.374050 vulners-2.1.7/vulners/__init__.py
+-rw-r--r--   0        0        0    19087 2024-05-16 19:39:23.374050 vulners-2.1.7/vulners/base.py
+-rw-r--r--   0        0        0    11174 2024-05-16 19:39:23.374050 vulners-2.1.7/vulners/vscanner.py
+-rw-r--r--   0        0        0    32597 2024-05-16 19:39:23.374050 vulners-2.1.7/vulners/vulners.py
+-rw-r--r--   0        0        0     6789 2024-05-16 19:39:25.805187 vulners-2.1.7/setup.py
+-rw-r--r--   0        0        0     7016 2024-05-16 19:39:25.805874 vulners-2.1.7/PKG-INFO
```

### Comparing `vulners-2.1.5/LICENSE` & `vulners-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vulners-2.1.5/README.md` & `vulners-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `vulners-2.1.5/pyproject.toml` & `vulners-2.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vulners"
-version = "2.1.5"
+version = "2.1.7"
 description = "Python library and command-line utility for Vulners (https://vulners.com)"
 readme = "README.md"
 authors = ["Kirill Ermakov <isox@vulners.com>", "Andrei Churin <a.churin@qiwi.com>"]
 keywords = ["security", "network", "vulners", "vulnerability", "CVE"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
```

### Comparing `vulners-2.1.5/vulners/base.py` & `vulners-2.1.7/vulners/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -208,16 +208,16 @@
         body_params["apiKey"] = self._api_key
         url = self._server_url + url.format(**path_params)
         kwargs = {"params" if method in ("get", "delete") else "json": body_params}
         bucket = self._ratelimits[ratelimit_key or url]
         bucket.consume()
         response = getattr(self._sess, method)(url, **kwargs)
         self._update_ratelimit(bucket, response)
-        result = self.adapt_response(response, method, result_type)
         response.raise_for_status()
+        result = self.adapt_response(response, method, result_type)
         return result, response.headers
 
 
 _Nothing = object()
 
 
 class ParamError(ValueError):
```

### Comparing `vulners-2.1.5/vulners/vscanner.py` & `vulners-2.1.7/vulners/vscanner.py`

 * *Files identical despite different names*

### Comparing `vulners-2.1.5/vulners/vulners.py` & `vulners-2.1.7/vulners/vulners.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         "published",
         "modified",
         "lastseen",
         "href",
         "sourceHref",
         "sourceData",
         "cvelist",
+        "vulnStatus",
+        "assigned",
     )
 
     __search = Endpoint(
         method="post",
         url="/api/v3/search/lucene/",
         params=[
             ("query", String()),
@@ -586,16 +588,53 @@
         offset: Skip this amount of items. 10000 is the hard limit.
         filter: Dict of fields to filter, eg { 'OS': 'Centos', 'OSVersion': '7'}
         sort: Field to sort, eg 'modified' or '-modified' to sort desc
         """
 
         return self.__report("scanlist", offset, limit, filter or {}, sort)
 
-    get_webhooks = Endpoint(
+    get_subscriptions = Endpoint(
+        method="get",
+        url="/api/v3/subscriptions/listEmailSubscriptions/",
+        content_handler=lambda hooks, _: hooks["subscriptions"],
+    )
+
+    add_subscription = Endpoint(
+        method="post",
+        url="/api/v3/subscriptions/addEmailSubscription/",
+        params=[
+            ("query", String()),
+            ("email", String()),
+            ("format", String(default="html", choices=("html", "json", "pdf"))),
+            ("crontab", String(allow_null=True, default=None)),
+            ("query_type", String(default="lucene")),
+        ]
+    )
+
+    edit_subscription = Endpoint(
         method="post",
+        url="/api/v3/subscriptions/editEmailSubscription/",
+        params=[
+            ("subscriptionid", String()),
+            ("format", String(allow_null=True, default=None, choices=("html", "json", "pdf"))),
+            ("crontab", String(allow_null=True, default=None)),
+            ("active", String(allow_null=True, default=None, choices=("yes", "no", "true", "false"))),
+        ]
+    )
+
+    delete_subscription = Endpoint(
+        method="post",
+        url="/api/v3/subscriptions/removeEmailSubscription/",
+        params=[
+            ("subscriptionid", String()),
+        ]
+    )
+
+    get_webhooks = Endpoint(
+        method="get",
         url="/api/v3/subscriptions/listWebhookSubscriptions/",
         content_handler=lambda hooks, _: hooks["subscriptions"],
     )
 
     add_webhook = Endpoint(
         method="post",
         url="/api/v3/subscriptions/addWebhookSubscription/",
```

### Comparing `vulners-2.1.5/setup.py` & `vulners-2.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['appdirs>=1.4.4,<2.0.0', 'requests>=2.31.0,<3.0.0', 'six>=1.16.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'vulners',
-    'version': '2.1.5',
+    'version': '2.1.7',
     'description': 'Python library and command-line utility for Vulners (https://vulners.com)',
     'long_description': '# [Vulners API v3](https://vulners.com) Python wrapper\n\n\n# Description\nPython 2/3 library for the [Vulners Database](https://vulners.com).\nIt provides *search, data retrieval, archive and vulnerability scanning* API\'s for the integration purposes.\nWith this library you can create powerful security tools and get access to the world largest security database.\n\n## Python version\nLibrary was tested on a *python2* and *python3*.\n\n## How to install\n\nPackage is available with [PyPI](https://pypi.python.org/pypi) \n\nYou can use pip for the installation\n\n```bash\npip install -U vulners\n```\n\n## Obtaining Vulners API key\n\nPlease, register at [Vulners website](https://vulners.com).\nGo to the personal menu by clicking at your name at the right top corner.\nFollow "API KEYS" tab.\nGenerate API key with scope "api" and use it with the library.\n\n# Functions and methods\n\nAll the callable methods are using [Vulners REST API](https://vulners.com/docs).\n\n### Search in database\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\nheartbleed_related = vulners_api.find_all("heartbleed", limit=10)\n```\n### Get information about document by identificator\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\nCVE_2017_14174 = vulners_api.get_bulletin("CVE-2017-14174")\n```\n### Get information about multiple documents by identificators\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\nCVE_DATA = vulners_api.get_multiple_bulletins(["CVE-2017-14174", "CVE-2016-1175"])\n```\n### Search for the public available exploits\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\nwordpress_exploits = vulners_api.find_exploit_all("wordpress 4.7.0")\n```\n### Get vulnerabilities and exploits by software name and version\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\n\nresults = vulners_api.get_software_vulnerabilities("httpd", "1.3")\nvulnerabilities_list = [results[key] for key in results if key not in ("info", "blog", "bugbounty")]\n```\n### Get vulnerabilities by CPE product and version string\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\n\ncpe_results = vulners_api.get_cpe_vulnerabilities("cpe:/a:cybozu:garoon:4.2.1")\ncpe_vulnerabilities_list = [cpe_results[key] for key in cpe_results if key not in ("info", "blog", "bugbounty")]\n```\n### Get references for the vulnerability\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\nreferences = vulners_api.get_bulletin_references("CVE-2014-0160")\n```\n### Get Windows KB superseeding and parentseeding information\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\n# Superseeding information will be returned as a dict\n# with two keys: "superseeds" and "parentseeds".\n# Superseeds means "what KB are covered by this KB".\n# Parentseeds means "what KB are covering this KB".\nsuperseeds = vulners_api.get_kb_seeds("KB4524135")\n```\n### Get Windows KB updates list and download urls\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\nmicrosoft_updates_for_kb = vulners_api.get_kb_updates("KB4524135")\nupdates_download_links = [update["href"] for update in microsoft_updates_for_kb]\n```\n### Score any vulnerability description using [Vulners AI](https://lab.wallarm.com/new-from-wallarm-research-first-ai-based-tool-to-predict-vulnerability-risk-2d0a7e9b3474)\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\ntext_ai_score = vulners_api.get_ai_score("My cool vulnerability description")\n```\n### Get possible query autocompletions\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\npossible_autocomplete = vulners_api.query_autocomplete("heartbleed")\n\n```\n### Download whole database collection and work with data locally\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\nall_cve = vulners_api.get_collection("cve")\n```\n### Audit Windows hosts for installed security KB\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\nwin_vulners = vulners_api.kb_audit(os="Windows Server 2012 R2", kb_list=["KB4072650", "KB2959936", "KB2894856", "KB2896496"])\nneed_2_install_kb = win_vulners["kbMissed"]\naffected_cve = win_vulners["cvelist"]\n```\n### Audit Linux hosts for vulnerabilities (RPM/DEB based)\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\n\n# Example for CentOS 7\n# You can use it for any RPM based OS\n# Execute command: rpm -qa --qf \'%{NAME}-%{VERSION}-%{RELEASE}.%{ARCH}\\\\n\'\n# Use it as package variable input\n\ncentos_vulnerabilities = vulners_api.os_audit(os="centos", version="7", packages=["glibc-common-2.17-157.el7_3.5.x86_64"])\nvulnerable_packages = centos_vulnerabilities.get("packages")\nmissed_patches_ids = centos_vulnerabilities.get("vulnerabilities")\ncve_list = centos_vulnerabilities.get("cvelist")\nhow_to_fix = centos_vulnerabilities.get("cumulativeFix")\n\n# Example for Debian 8\n# You can use it for any DEB based OS\n# Execute command: dpkg-query -W -f=\'${Package} ${Version} ${Architecture}\\\\n\'\n# Use it as package variable input\n\ndebian_vulnerabilities = vulners_api.os_audit(os="debian", version="8", packages=[\'uno-libs3 4.3.3-2+deb8u7 amd64\'])\n```\n\n### Download Linux (RPM/DEB based) vulnerability assessment data for local processing\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\n\n# Example for CentOS 7\ncentos_vulnerabilities_data = vulners_api.get_distributive("CentOS", "7")\n```\n### Download web application vulnerability detection regex collection\n```python\nimport vulners\n\nvulners_api = vulners.VulnersApi(api_key="YOUR_API_KEY_HERE")\nrules = vulners_api.get_web_application_rules()\n```\n',
     'author': 'Kirill Ermakov',
     'author_email': 'isox@vulners.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `vulners-2.1.5/PKG-INFO` & `vulners-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulners
-Version: 2.1.5
+Version: 2.1.7
 Summary: Python library and command-line utility for Vulners (https://vulners.com)
 Keywords: security,network,vulners,vulnerability,CVE
 Author: Kirill Ermakov
 Author-email: isox@vulners.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

