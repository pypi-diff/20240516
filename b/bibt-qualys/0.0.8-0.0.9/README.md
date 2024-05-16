# Comparing `tmp/bibt_qualys-0.0.8.tar.gz` & `tmp/bibt_qualys-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Nov 27 15:05:44 2023, max compression
+gzip compressed data, last modified: Mon Nov 27 18:52:31 2023, max compression
```

## Comparing `bibt_qualys-0.0.8.tar` & `bibt_qualys-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      436 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/.bumpversion.cfg
--rw-r--r--   0        0        0     1259 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      368 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/.readthedocs.yml
--rw-r--r--   0        0        0       98 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0        0 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/MANIFEST.in
--rw-r--r--   0        0        0     1758 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/test.py
--rw-r--r--   0        0        0       17 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/.github/CODEOWNERS
--rw-r--r--   0        0        0      142 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0     2488 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0        0        0     1014 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/bibt/__init__.py
--rw-r--r--   0        0        0    16645 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/bibt/qualys/Client.py
--rw-r--r--   0        0        0      428 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/bibt/qualys/__init__.py
--rw-r--r--   0        0        0       22 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/bibt/qualys/version.py
--rw-r--r--   0        0        0      634 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/docs/Makefile
--rw-r--r--   0        0        0     2658 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/docs/conf.py
--rw-r--r--   0        0        0     2456 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/docs/contributing.rst
--rw-r--r--   0        0        0     2030 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/docs/index.rst
--rw-r--r--   0        0        0      790 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/docs/make.bat
--rw-r--r--   0        0        0       65 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/docs/qualys.rst
--rw-r--r--   0        0        0      228 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/docs/modules/qualys.rst
--rw-r--r--   0        0        0     4524 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/.gitignore
--rw-r--r--   0        0        0     1054 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/LICENSE
--rw-r--r--   0        0        0      477 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/README.md
--rw-r--r--   0        0        0     1071 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1523 2023-11-27 15:05:44.000000 bibt_qualys-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      436 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/.bumpversion.cfg
+-rw-r--r--   0        0        0     1259 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      368 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/.readthedocs.yml
+-rw-r--r--   0        0        0       98 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/MANIFEST.in
+-rw-r--r--   0        0        0     2492 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/test.py
+-rw-r--r--   0        0        0       17 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      142 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     2488 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0        0        0     1014 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/bibt/__init__.py
+-rw-r--r--   0        0        0    20801 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/bibt/qualys/Client.py
+-rw-r--r--   0        0        0      428 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/bibt/qualys/__init__.py
+-rw-r--r--   0        0        0       22 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/bibt/qualys/version.py
+-rw-r--r--   0        0        0      634 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0     2658 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0     2456 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/docs/contributing.rst
+-rw-r--r--   0        0        0     2030 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/docs/index.rst
+-rw-r--r--   0        0        0      790 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/docs/make.bat
+-rw-r--r--   0        0        0       65 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/docs/qualys.rst
+-rw-r--r--   0        0        0      228 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/docs/modules/qualys.rst
+-rw-r--r--   0        0        0     4524 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1054 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/LICENSE
+-rw-r--r--   0        0        0      477 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/README.md
+-rw-r--r--   0        0        0     1071 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1523 2023-11-27 18:52:31.000000 bibt_qualys-0.0.9/PKG-INFO
```

### Comparing `bibt_qualys-0.0.8/.pre-commit-config.yaml` & `bibt_qualys-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/test.py` & `bibt_qualys-0.0.9/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,51 +17,77 @@
         "%(message)s"
     ),
     force=True,
 )
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 logging.getLogger("google").setLevel(logging.WARNING)
 
-# def test_client(capsys):
-#     with capsys.disabled():
-#         c = Client(
-#             os.environ["QUALYS_USER"],
-#             os.environ["QUALYS_PASS"],
-#             os.environ["QUALYS_URL"],
-#         )
-#         assert c.session
-#         c.close()
-#         assert not c.session
-
-
-# def test_list_scan_schedules(capsys):
-#     with capsys.disabled():
-#         c = Client(
-#             os.environ["QUALYS_USER"],
-#             os.environ["QUALYS_PASS"],
-#             os.environ["QUALYS_URL"],
-#         )
-#         scans = c.list_scan_schedules()
-#         assert len(scans) > 0
-
-
-# def test_list_scans(capsys):
-#     with capsys.disabled():
-#         c = Client(
-#             os.environ["QUALYS_USER"],
-#             os.environ["QUALYS_PASS"],
-#             os.environ["QUALYS_URL"],
-#         )
-#         scans = c.list_scans()
-#         assert len(scans) > 0
+
+def test_client(capsys):
+    with capsys.disabled():
+        c = Client(
+            os.environ["QUALYS_USER"],
+            os.environ["QUALYS_PASS"],
+            os.environ["QUALYS_URL"],
+        )
+        assert c.session
+        c.close()
+        assert not c.session
+
+
+def test_list_scan_schedules(capsys):
+    with capsys.disabled():
+        c = Client(
+            os.environ["QUALYS_USER"],
+            os.environ["QUALYS_PASS"],
+            os.environ["QUALYS_URL"],
+        )
+        scans = c.list_scan_schedules()
+        assert len(scans) > 0
+
+
+def test_list_scans(capsys):
+    with capsys.disabled():
+        c = Client(
+            os.environ["QUALYS_USER"],
+            os.environ["QUALYS_PASS"],
+            os.environ["QUALYS_URL"],
+        )
+        scans = c.list_scans()
+        assert len(scans) > 0
 
 
 def test_get_scan_result(capsys):
     with capsys.disabled():
         c = Client(
             os.environ["QUALYS_USER"],
             os.environ["QUALYS_PASS"],
             os.environ["QUALYS_URL"],
         )
         scan = c.get_scan_result(os.environ["TEST_SCAN_TITLE"], output_format="json")
         with open("test_json.json", "w+") as outfile:
             json.dump(scan, outfile, indent=2)
+
+
+def test_list_reports(capsys):
+    with capsys.disabled():
+        c = Client(
+            os.environ["QUALYS_USER"],
+            os.environ["QUALYS_PASS"],
+            os.environ["QUALYS_URL"],
+        )
+        reports = c.list_reports()
+        with open("reports.list.json", "w+") as outfile:
+            json.dump(reports, outfile, indent=2)
+        assert len(reports) > 0
+
+
+def test_get_report_result(capsys):
+    with capsys.disabled():
+        c = Client(
+            os.environ["QUALYS_USER"],
+            os.environ["QUALYS_PASS"],
+            os.environ["QUALYS_URL"],
+        )
+        output_format, report = c.get_report_result(os.environ["TEST_REPORT_TITLE"])
+        with open(f"report.fetch.{output_format.lower()}", "w+") as outfile:
+            outfile.write(report)
```

### Comparing `bibt_qualys-0.0.8/.github/workflows/publish-to-pypi.yaml` & `bibt_qualys-0.0.9/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/bibt/__init__.py` & `bibt_qualys-0.0.9/bibt/__init__.py`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/bibt/qualys/Client.py` & `bibt_qualys-0.0.9/bibt/qualys/Client.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,31 +12,38 @@
 # names. Attribute names: ID, TITLE, OWNER_USER_NAME,
 # OWNER_USER_ID, OWNER_UNIT_ID, NETWORK_IDS,
 # LAST_UPDATE, IP_SET, APPLIANCE_LIST, DOMAIN_LIST,
 # DNS_LIST, NETBIOS_LIST, EC2_ID_LIST, asset_group_IDS,
 # ASSIGNED_USER_IDS, ASSIGNED_UNIT_IDS,
 # BUSINESS_IMPACT, CVSS, COMMENTS.
 
+QUALYS_REPORT_ENDPOINT = "/api/2.0/fo/report/"
+QUALYS_SCAN_ENDPOINT = "/api/2.0/fo/scan/"
+QUALYS_SCAN_SCHEDULE_ENDPOINT = "/api/2.0/fo/schedule/scan/"
+QUALYS_ASSET_GROUP_ENDPOINT = "/api/2.0/fo/asset/group/"
+QUALYS_ASSET_HOST_ENDPOINT = "/api/2.0/fo/asset/host/"
+QUALYS_CLOUD_AGENT_SEARCH_HOST_ASSET_ENDPOINT = "/qps/rest/2.0/search/am/hostasset"
 
 _LOGGER = logging.getLogger(__name__)
 
 # TODO: Documentation
 # TODO: kwargs?
 
 
 class Client:
-    def __init__(self, user, password, url):
-        """Creates a bibt.qualys.Client object, which may be used to
-        make Qualys API calls using the same set of credentials.
+    """Creates a ``bibt.qualys.Client`` object, which may be used to
+    make Qualys API calls using the same set of credentials.
 
-        :param str user: The Qualys username with which to authenticate.
-        :param str password: The password for the provided account username.
-        :param str url: The root domain for Qualys, e.g.
-            ``"https://qualysapi.qg1.apps.qualys.com"``.
-        """
+    :param str user: The Qualys username with which to authenticate.
+    :param str password: The password for the provided account username.
+    :param str url: The root domain for Qualys, e.g.
+        ``"https://qualysapi.qg1.apps.qualys.com"``.
+    """
+
+    def __init__(self, user, password, url):
         self.session = requests.Session()
         self.session.auth = (user, password)
         self.session.headers.update(
             {
                 "X-Requested-With": "Python.requests",
                 "Content-Type": "text/xml",
                 "Cache-Control": "no-cache",
@@ -78,54 +85,117 @@
         params["action"] = "list"
         full_resp = []
         while request_url:
             _LOGGER.debug(f"Request URL: {request_url}")
             _LOGGER.debug(f"Request params: {params}")
             resp = self._handle_request(self.session.get(request_url, params=params))
             resp_json = xmltodict.parse(
-                resp.text,
+                resp.content,
                 attr_prefix="",
                 cdata_key="text",
                 comment_key="comment",
                 force_list=force_list,
             )
 
             # handle special case of final key being different
             final_key = key
             if key == "SCHEDULE_SCAN":
                 final_key = "SCAN"
 
+            if f"{key}_LIST" not in resp_json[f"{key}_LIST_OUTPUT"]["RESPONSE"]:
+                if len(full_resp) < 1:
+                    _LOGGER.error(
+                        f"Key {key}_LIST not found in data from Qualys; ensure "
+                        "you have the correct permissions to fetch this data."
+                    )
+                    return []
+                else:
+                    break
             resp_json_data = resp_json[f"{key}_LIST_OUTPUT"]["RESPONSE"][f"{key}_LIST"][
                 final_key
             ]
             _LOGGER.debug(f"Extending list of type {key} by {len(resp_json_data)}...")
             full_resp.extend(resp_json_data)
             try:
                 params = None
                 request_url = resp_json[f"{key}_LIST_OUTPUT"]["RESPONSE"]["WARNING"][
                     "URL"
                 ]
             except KeyError:
                 request_url = None
         return full_resp
 
+    def _make_fetch_request(self, endpoint, params={}):
+        if not self.session:
+            raise Exception(
+                "Cannot make requests via a closed HTTP session! "
+                "Please create a new Client object to initialize a new session."
+            )
+        request_url = self.url + endpoint
+        params["action"] = "fetch"
+        resp = self._handle_request(self.session.get(request_url, params=params))
+        # logging.debug(str(resp.content[: min(len(resp.content), 300)] + b"..."))
+
+        if params.get("output_format") in ["json", "json_extended"]:
+            return resp.json()
+        else:
+            return resp.text
+
     def _make_delete_request(self, endpoint, id):
         if not self.session:
             raise Exception(
                 "Cannot make requests via a closed HTTP session! "
                 "Please create a new Client object to initialize a new session."
             )
 
         resp = self._handle_request(
             self.session.post(
                 self.url + endpoint, params={"action": "delete", "id": id}
             )
         )
         return resp
 
+    def _list_scans_reports(self, endpoint, key, state, force_list):
+        params = {}
+        if state:
+            params["state"] = state
+        return self._make_list_request(
+            endpoint,
+            key,
+            params=params,
+            force_list=force_list,
+        )
+
+    def _match_results(self, all_results, title, result_type):
+        ref = None
+        ref_key = "REF" if result_type == "SCAN" else "ID"
+        logging.debug(
+            f"Iterating through {len(all_results)} results to find right "
+            f"ref/id for result titled [{title}]..."
+        )
+        for result in all_results:
+            if result["TITLE"] == title:
+                logging.info(
+                    "Matching result found! ref: "
+                    f'[{result[ref_key]}] state: [{result["STATUS"]["STATE"]}] '
+                    f'launched: [{result["LAUNCH_DATETIME"]}]'
+                )
+                return result
+
+        if not ref:
+            raise Exception(
+                f"No result found for title: [{title}] "
+                f"in {len(all_results)} results."
+            )
+
+    #
+    #  Asset: Groups Endpoint
+    #  /api/2.0/fo/asset/groups
+    #
+
     def list_asset_groups(
         self,
         truncation_limit=DEFAULT_TRUNCATION,
         show_attributes=ASSET_GROUP_ATTRIBUTES_LIST,
         asset_group_title=None,
         force_list=["IP", "IP_RANGE", "DOMAIN_LIST", "DNS"],
         clean_data=True,
@@ -139,15 +209,15 @@
         params = {
             "truncation_limit": truncation_limit,
             "show_attributes": show_attributes,
         }
         if asset_group_title:
             params["title"] = asset_group_title
         resp = self._make_list_request(
-            "/api/2.0/fo/asset/group/",
+            QUALYS_ASSET_GROUP_ENDPOINT,
             "ASSET_GROUP",
             params=params,
             force_list=force_list,
         )
         if clean_data:
             _LOGGER.info("Cleaning data...")
             for i in range(len(resp)):
@@ -166,77 +236,71 @@
                             resp[i]["DOMAIN_LIST"][j]["DOMAIN"] = json.dumps(
                                 resp[i]["DOMAIN_LIST"][j]["DOMAIN"]
                             )
 
         _LOGGER.info(f"Returning data for {len(resp)} asset groups...")
         return resp
 
+    #
+    #  Asset: Host Endpoint
+    #  /api/2.0/fo/asset/host
+    #
+
     def list_hosts(
         self,
         truncation_limit=DEFAULT_TRUNCATION,
         show_attributes=ASSET_GROUP_ATTRIBUTES_LIST,
         force_list=None,
     ):
         _LOGGER.info("Requesting asset group data from Qualys...")
         _LOGGER.debug(
             f"Args: force_list={force_list} "
             f"truncation_limit=[{truncation_limit}] show_attributes=[{show_attributes}]"
         )
         resp = self._make_list_request(
-            "/api/2.0/fo/asset/host/",
+            QUALYS_ASSET_HOST_ENDPOINT,
             "HOST",
             params={
                 "truncation_limit": truncation_limit,
                 "show_attributes": show_attributes,
             },
             force_list=force_list,
         )
 
         _LOGGER.info(f"Returning data for {len(resp)} hosts...")
         return resp
 
+    #
+    #  Scan Schedules Endpoint
+    #  /api/2.0/fo/schedule/scan/
+    #
+
     def list_scan_schedules(self, force_list=["ASSET_GROUP_TITLE"]):
         """List all configured scan schedules in Qualys.
 
         :param list force_list: A list of keys to force into list format when parsing
             the returned XML into lists and dictionaries.
             Defaults to ``["ASSET_GROUP_TITLE"]``.
         :return list: A list of dicts, containing metadata for all scan schedules.
         """
         _LOGGER.info("Requesting scan schedule data from Qualys...")
         _LOGGER.debug(f"Args: force_list=[{force_list}]")
         scan_schedules = self._make_list_request(
-            "/api/2.0/fo/schedule/scan/",
+            QUALYS_SCAN_SCHEDULE_ENDPOINT,
             "SCHEDULE_SCAN",
             force_list=force_list,
         )
 
         _LOGGER.info(f"Returning data for {len(scan_schedules)} scan schedules...")
         return scan_schedules
 
-    def list_scans(
-        self,
-        force_list=None,
-    ):
-        """List all scans in Qualys.
-
-        :param list force_list: A list of keys to force into list format when parsing
-            the returned XML into lists and dictionaries. Defaults to ``None``.
-        :return list: A list of dicts, containing metadata for all Qualys scans.
-        """
-        # TODO: looping for all scans? limit?
-        _LOGGER.info("Requesting scan data from Qualys...")
-        _LOGGER.debug(f"Args: force_list={force_list}")
-        scan_data = self._make_list_request(
-            "/api/2.0/fo/scan/",
-            "SCAN",
-            force_list=force_list,
-        )
-        _LOGGER.info(f"Returning data for {len(scan_data)} scans...")
-        return scan_data
+    #
+    #  Scan Endpoint
+    #  /api/2.0/fo/scan/
+    #
 
     def _get_scanref_result(
         self,
         scan_ref,
         output_format=DEFAULT_SCAN_RESULT_OUTPUT_FORMAT,
         mode=DEFAULT_SCAN_RESULT_MODE,
     ):
@@ -247,52 +311,60 @@
             one of: "csv", "json", "csv_extended", "json_extended".
             Defaults to ``bibt.qualys.DEFAULT_SCAN_RESULT_OUTPUT_FORMAT``.
         :param str mode: Must be one of "brief" or "extended". Specifies the level
             of detail per result for Qualys to return. Defaults to
             ``bibt.qualys.DEFAULT_SCAN_RESULT_MODE``.
         :return list OR str: The scan result in the requested output format.
         """
-        # TODO: fetch req func
-        request_url = self.url + "/api/2.0/fo/scan/"
-        params = {
-            "action": "fetch",
-            "scan_ref": scan_ref,
-            "output_format": output_format,
-            "mode": mode,
-        }
-        resp = self._handle_request(self.session.get(request_url, params=params))
-        logging.debug(resp.text[: min(len(resp.text), 300)] + "...")
+        _LOGGER.info(
+            f"Getting results for: [{scan_ref}] in format "
+            f"[{output_format}] in mode [{mode}]"
+        )
+        return self._make_fetch_request(
+            QUALYS_SCAN_ENDPOINT,
+            params={"output_format": output_format, "mode": mode, "scan_ref": scan_ref},
+        )
 
-        if output_format in ["json", "json_extended"]:
-            return resp.json()
-        else:
-            return resp.text
+    def list_scans(
+        self,
+        state="Finished",
+        force_list=None,
+    ):
+        """List all scans in Qualys.
+
+        :param str state: The state of scans to return. Set to ``None`` to
+            return all scans. Defaults to ``"Finished"``.
+        :param list force_list: A list of keys to force into list format when parsing
+            the returned XML into lists and dictionaries. Defaults to ``None``.
+        :return list: A list of dicts, containing metadata for all Qualys scans.
+        """
+        _LOGGER.info("Requesting scan data from Qualys...")
+        _LOGGER.debug(f"Args: state={state} force_list={force_list}")
+        scan_data = self._list_scans_reports(
+            QUALYS_SCAN_ENDPOINT, "SCAN", state, force_list
+        )
+        _LOGGER.info(f"Returning data for {len(scan_data)} scans...")
+        return scan_data
 
     def get_scan_result(
         self,
         scan_title,
         output_format=DEFAULT_SCAN_RESULT_OUTPUT_FORMAT,
         mode=DEFAULT_SCAN_RESULT_MODE,
-        accept_scan_states=None,
         refactor_json_data=True,
     ):
         """Given a scan title, will fetch the most recent scan result.
 
         :param str scan_title: The title of the scan, e.g. "VLAN 100 Scan".
         :param str output_format: The output format of the scan results. Must be
             one of: "csv", "json", "csv_extended", "json_extended".
             Defaults to ``bibt.qualys.DEFAULT_SCAN_RESULT_OUTPUT_FORMAT``.
         :param str mode: Must be one of "brief" or "extended". Specifies the level
             of detail per result for Qualys to return. Defaults to
             ``bibt.qualys.DEFAULT_SCAN_RESULT_MODE``.
-        :param list accept_scan_states: A list of scan statuses to accept,
-            in addition to "Finished". Other potential scan states are:
-            "Queued", "Running", "Loading", "Canceling", "Canceled", "Pausing",
-            "Paused", "Resuming", and "Error". Note that it may not be possible to
-            get results for any or all of these other scan states. Defaults to ``None``.
         :param bool refactor_json_data: Whether or not to refactor "json_extended" scan
             result data into a more organized format. By default, Qualys returns a list
             of dictionaries, where: the first two dictionaries cover request metadata
             and scan result metadata respectively; the last dictionary includes special
             notes about the scan run; and each of the dictionaries in the middle contain
             result data per host. If this option is set to True, the data will be
             reformated to a dictionary with the keys: ``"request_metadata": {}``,
@@ -302,45 +374,21 @@
         :return list OR dict OR str: THe scan result data.
         """
         _LOGGER.info(f"Getting scan result for scan [{scan_title}]...")
         _LOGGER.debug(
             f"Args: scan_title=[{scan_title}] "
             f"output_format=[{output_format}] mode=[{mode}]"
         )
-        all_scans = self.list_scans()
-        scan_ref = None
-        logging.debug(
-            f"Iterating through {len(all_scans)} scans to find right scan_ref..."
-        )
-        if isinstance(accept_scan_states, list):
-            accept_scan_states.extend(["Finished"])
-        else:
-            accept_scan_states = ["Finished"]
-        for scan in all_scans:
-            if scan["TITLE"] == scan_title:
-                if scan["STATUS"]["STATE"] in accept_scan_states:
-                    logging.debug(
-                        "Matching scan found! ref: "
-                        f'[{scan["REF"]}] state: [{scan["STATUS"]["STATE"]}] '
-                        f'launched: [{scan["LAUNCH_DATETIME"]}]'
-                    )
-                    scan_ref = scan["REF"]
-                    break
-                else:
-                    logging.debug(
-                        "Matching scan found, but has state: "
-                        f'[{scan["STATUS"]["STATE"]}] ref: [{scan["REF"]}]  '
-                        f'launched: [{scan["LAUNCH_DATETIME"]}]'
-                    )
 
-        if not scan_ref:
-            raise Exception(f"No scan found for title: [{scan_title}]")
+        all_scans = self.list_scans(state="Finished")
+
+        scan = self._match_results(all_scans, scan_title, "SCAN")
 
         scan_data = self._get_scanref_result(
-            scan_ref, output_format=output_format, mode=mode
+            scan["REF"], output_format=output_format, mode=mode
         )
         if (
             output_format == "json_extended"
             and refactor_json_data
             and len(scan_data) >= 3
         ):
             if (
@@ -365,30 +413,103 @@
 
     def delete_scan_result(self, scan_ref):
         """Deletes a scan result from Qualys by its reference ID.
 
         :param str scan_ref: The scan reference ID, e.g. ``"scan/123456789.12345"``
         """
         _LOGGER.info(f"Sending delete request for scan: [{scan_ref}]")
-        self._make_delete_request("/api/2.0/fo/scan/", scan_ref)
+        self._make_delete_request(QUALYS_SCAN_ENDPOINT, scan_ref)
         _LOGGER.info(f"Scan [{scan_ref}] deleted.")
 
-    # def get_report(self, report_title):
-    # def get_kb(self)
+    #
+    # Reports Endpoint
+    # /api/2.0/fo/report/
+    #
+
+    def _get_reportid_result(self, report_id):
+        """Provided a report ID, fetches the report result from Qualys.
+            Report MUST have a state of "Finished".
+
+        :param str report_id: The report ID, e.g. ``"123456"``.
+        :return list OR str: The report result.
+        """
+        _LOGGER.info(f"Getting results for report: [{report_id}]")
+        report_data = self._make_fetch_request(
+            QUALYS_REPORT_ENDPOINT,
+            params={"id": report_id},
+        )
+        return report_data
+
+    def list_reports(
+        self,
+        state="Finished",
+        force_list=None,
+    ):
+        """List all reports in Qualys.
+
+        :param str state: The state of reports to return. Set to ``None`` to
+            return all reports. Defaults to ``"Finished"``.
+        :param list force_list: A list of keys to force into list format when parsing
+            the returned XML into lists and dictionaries. Defaults to ``None``.
+        :return list: A list of dicts, containing metadata for all Qualys reports.
+        """
+        _LOGGER.info("Requesting report data from Qualys...")
+        _LOGGER.debug(f"Args: state={state} force_list={force_list}")
+        report_data = self._list_scans_reports(
+            QUALYS_REPORT_ENDPOINT, "REPORT", state, force_list
+        )
+        _LOGGER.info(f"Returning data for {len(report_data)} reports...")
+        return report_data
+
+    def get_report_result(self, report_title):
+        """Given a report title, fetches the most recent report result.
+
+        :param str report_title: The report title for which to search.
+        :return (str, str): A tuple of ``(output_format, data)`` where
+            ``output_format`` is the configured report output format,
+            e.g. "XML", "HTML", "CSV", etc.
+        """
+        _LOGGER.info(f"Searching for result for report: [{report_title}]")
+        all_reports = self.list_reports(state="Finished")
+        report = self._match_results(all_reports, report_title, "REPORT")
+        _LOGGER.debug(
+            f"Fetching report result: id=[{report['ID']}] type="
+            f"[{report['OUTPUT_FORMAT']}] size=[{report['SIZE']}]"
+        )
+        report_data = self._get_reportid_result(report["ID"])
+        _LOGGER.info(
+            f"Returning data for report [{report_title}] "
+            f"[{report['ID']}] in format [{report['OUTPUT_FORMAT']}]"
+        )
+        return report["OUTPUT_FORMAT"], report_data
+
+    def delete_report_result(self, report_id):
+        """Deletes a report result from Qualys by its ID.
+
+        :param str report_id: The report reference ID, e.g. ``"report/123456789.12345"``
+        """
+        _LOGGER.info(f"Sending delete request for report: [{report_id}]")
+        self._make_delete_request(QUALYS_REPORT_ENDPOINT, report_id)
+        _LOGGER.info(f"Report [{report_id}] deleted.")
+
+    #
+    # Cloud Agent: Host Asset Endpoint
+    # /qps/rest/2.0/search/am/hostasset
+    #
 
     def search_hostassets(self, data, clean_data=True):
         # TODO: data cleaning?
         if not self.session:
             raise Exception(
                 "Cannot make requests via a closed HTTP session! "
                 "Please create a new Client object to initialize a new session."
             )
 
         _LOGGER.info("Requesting host asset data from Qualys...")
-        request_url = self.url + "/qps/rest/2.0/search/am/hostasset"
+        request_url = self.url + QUALYS_CLOUD_AGENT_SEARCH_HOST_ASSET_ENDPOINT
         _LOGGER.debug(f"Request url: {request_url}")
         resp = self._handle_request(
             self.session.post(
                 request_url, headers={"Accept": "application/json"}, data=data
             )
         )
         _LOGGER.debug(resp.text)
```

### Comparing `bibt_qualys-0.0.8/docs/Makefile` & `bibt_qualys-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/docs/conf.py` & `bibt_qualys-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/docs/contributing.rst` & `bibt_qualys-0.0.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/docs/index.rst` & `bibt_qualys-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/docs/make.bat` & `bibt_qualys-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/.gitignore` & `bibt_qualys-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/LICENSE` & `bibt_qualys-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bibt_qualys-0.0.8/pyproject.toml` & `bibt_qualys-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bibt-qualys"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{ name = "Matthew OBrien", email = "mobrien@broadinstitute.org" }]
 description = "Functionality often used by BITS Blue Team (Qualys)."
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.7"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `bibt_qualys-0.0.8/PKG-INFO` & `bibt_qualys-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibt-qualys
-Version: 0.0.8
+Version: 0.0.9
 Summary: Functionality often used by BITS Blue Team (Qualys).
 Project-URL: Homepage, https://github.com/broadinstitute/bibt-qualys
 Project-URL: Documentation, https://bibt-qualys.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/broadinstitute/bibt-qualys/issues
 Author-email: Matthew OBrien <mobrien@broadinstitute.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

