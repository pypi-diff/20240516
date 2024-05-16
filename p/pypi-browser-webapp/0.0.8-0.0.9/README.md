# Comparing `tmp/pypi_browser_webapp-0.0.8.tar.gz` & `tmp/pypi_browser_webapp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_browser_webapp-0.0.8.tar", max compression
+gzip compressed data, was "pypi_browser_webapp-0.0.9.tar", max compression
```

## Comparing `pypi_browser_webapp-0.0.8.tar` & `pypi_browser_webapp-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2722 2024-05-15 15:56:44.626790 pypi_browser_webapp-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-05-15 15:56:44.627604 pypi_browser_webapp-0.0.8/pypi_browser/__init__.py
--rw-r--r--   0        0        0    13223 2024-05-15 16:06:29.200394 pypi_browser_webapp-0.0.8/pypi_browser/app.py
--rw-r--r--   0        0        0     4493 2024-05-15 16:12:10.130971 pypi_browser_webapp-0.0.8/pypi_browser/packaging.py
--rw-r--r--   0        0        0     3397 2024-05-15 15:56:44.628229 pypi_browser_webapp-0.0.8/pypi_browser/pypi.py
--rw-r--r--   0        0        0   195498 2024-05-15 15:56:44.628752 pypi_browser_webapp-0.0.8/pypi_browser/static/bootstrap-5.2.1.min.css
--rw-r--r--   0        0        0    80457 2024-05-15 15:56:44.629169 pypi_browser_webapp-0.0.8/pypi_browser/static/bootstrap-5.2.1.min.js
--rw-r--r--   0        0        0     1584 2024-05-15 15:56:44.629315 pypi_browser_webapp-0.0.8/pypi_browser/static/favicon.png
--rw-r--r--   0        0        0      380 2024-05-15 15:56:44.629430 pypi_browser_webapp-0.0.8/pypi_browser/static/site.css
--rw-r--r--   0        0        0       78 2024-05-15 15:56:44.629535 pypi_browser_webapp-0.0.8/pypi_browser/static/site.js
--rw-r--r--   0        0        0     2293 2024-05-15 15:56:44.629718 pypi_browser_webapp-0.0.8/pypi_browser/templates/_base.html
--rw-r--r--   0        0        0      743 2024-05-15 15:56:44.629842 pypi_browser_webapp-0.0.8/pypi_browser/templates/_macros.html
--rw-r--r--   0        0        0     1389 2024-05-15 15:56:44.629967 pypi_browser_webapp-0.0.8/pypi_browser/templates/home.html
--rw-r--r--   0        0        0     1397 2024-05-15 15:56:44.630129 pypi_browser_webapp-0.0.8/pypi_browser/templates/package.html
--rw-r--r--   0        0        0     2495 2024-05-15 15:56:44.630297 pypi_browser_webapp-0.0.8/pypi_browser/templates/package_file.html
--rw-r--r--   0        0        0     2434 2024-05-15 15:56:44.630465 pypi_browser_webapp-0.0.8/pypi_browser/templates/package_file_archive_path.html
--rw-r--r--   0        0        0      869 2024-05-15 16:12:42.720743 pypi_browser_webapp-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 pypi_browser_webapp-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3207 2024-05-16 16:17:08.466588 pypi_browser_webapp-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 15:56:44.627604 pypi_browser_webapp-0.0.9/pypi_browser/__init__.py
+-rw-r--r--   0        0        0    13823 2024-05-16 16:17:08.467063 pypi_browser_webapp-0.0.9/pypi_browser/app.py
+-rw-r--r--   0        0        0     6246 2024-05-16 16:17:08.467404 pypi_browser_webapp-0.0.9/pypi_browser/packaging.py
+-rw-r--r--   0        0        0     5357 2024-05-16 16:17:08.467742 pypi_browser_webapp-0.0.9/pypi_browser/pypi.py
+-rw-r--r--   0        0        0   195498 2024-05-15 15:56:44.628752 pypi_browser_webapp-0.0.9/pypi_browser/static/bootstrap-5.2.1.min.css
+-rw-r--r--   0        0        0    80457 2024-05-15 15:56:44.629169 pypi_browser_webapp-0.0.9/pypi_browser/static/bootstrap-5.2.1.min.js
+-rw-r--r--   0        0        0     1584 2024-05-15 15:56:44.629315 pypi_browser_webapp-0.0.9/pypi_browser/static/favicon.png
+-rw-r--r--   0        0        0      380 2024-05-15 15:56:44.629430 pypi_browser_webapp-0.0.9/pypi_browser/static/site.css
+-rw-r--r--   0        0        0       78 2024-05-15 15:56:44.629535 pypi_browser_webapp-0.0.9/pypi_browser/static/site.js
+-rw-r--r--   0        0        0     2293 2024-05-15 15:56:44.629718 pypi_browser_webapp-0.0.9/pypi_browser/templates/_base.html
+-rw-r--r--   0        0        0      743 2024-05-15 15:56:44.629842 pypi_browser_webapp-0.0.9/pypi_browser/templates/_macros.html
+-rw-r--r--   0        0        0     1389 2024-05-15 15:56:44.629967 pypi_browser_webapp-0.0.9/pypi_browser/templates/home.html
+-rw-r--r--   0        0        0     1627 2024-05-16 16:17:08.468081 pypi_browser_webapp-0.0.9/pypi_browser/templates/package.html
+-rw-r--r--   0        0        0     2495 2024-05-15 15:56:44.630297 pypi_browser_webapp-0.0.9/pypi_browser/templates/package_file.html
+-rw-r--r--   0        0        0     2434 2024-05-15 15:56:44.630465 pypi_browser_webapp-0.0.9/pypi_browser/templates/package_file_archive_path.html
+-rw-r--r--   0        0        0      869 2024-05-16 16:17:14.388054 pypi_browser_webapp-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3941 1970-01-01 00:00:00.000000 pypi_browser_webapp-0.0.9/PKG-INFO
```

### Comparing `pypi_browser_webapp-0.0.8/README.md` & `pypi_browser_webapp-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -52,14 +52,25 @@
 pip, then run the `pypi_browser.app:app` ASGI application using any ASGI web
 server (e.g. uvicorn).
 
 You can set these environment variables to configure the server:
 
 * `PYPI_BROWSER_PYPI_URL`: URL for the PyPI server to use (defaults to
   `https://pypi.org`)
+
+  If your registry supports the pypi.org-compatible JSON API (e.g.
+  `{registry}/pypi/{package}/json`), specify your base registry URL without
+  appending `/simple` (e.g. `https://my-registry`).
+
+  If your registry only supports the traditional HTML "simple" index, specify
+  the registry URL with `/simple` at the end (e.g.
+  `https://my-registry/simple`).
+
+  Note that the [PEP691][pep691] JSON-based "simple" API is not yet supported.
+
 * `PYPI_BROWSER_PACKAGE_CACHE_PATH`: Filesystem path to use for caching
   downloaded files. This will grow forever (the app does not clean it up) so
   you may want to use `tmpreaper` or similar to manage its size.
 
 pypi-browser is an ASGI app, and while it performs a lot of I/O (downloading and
 extracting packages on-demand), some effort has been made to keep all blocking
 operations off of the main thread. It should be fairly performant.
@@ -73,7 +84,9 @@
 Once installed, you can run
 
 ```bash
 $ make start-dev
 ```
 
 to run a copy of the application locally with hot reloading enabled.
+
+[pep691]: https://peps.python.org/pep-0691/
```

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/app.py` & `pypi_browser_webapp-0.0.9/pypi_browser/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,17 +70,24 @@
         response = await call_next(request)
         # TODO: There should be a better way to do this...
         response.headers['Cache-Control'] = 'no-cache'
         return response
 
 
 config = starlette.config.Config()
+pypi_url = config('PYPI_BROWSER_PYPI_URL', default='https://pypi.org').rstrip('/')
+repo: pypi.PythonRepository
+if pypi_url.endswith('/simple'):
+    repo = pypi.SimpleRepository(pypi_url)
+else:
+    repo = pypi.LegacyJsonRepository(pypi_url)
+
 pypi_config = pypi.PyPIConfig(
+    repo=repo,
     cache_path=config('PYPI_BROWSER_PACKAGE_CACHE_PATH', default='/tmp'),
-    pypi_url=config('PYPI_BROWSER_PYPI_URL', default='https://pypi.org'),
 )
 
 templates = Jinja2Templates(
     directory=os.path.join(install_root, 'templates'),
 )
 
 
@@ -111,24 +118,33 @@
 async def package(request: Request) -> Response:
     package_name = request.path_params['package']
     normalized_package_name = pypi_browser.packaging.pep426_normalize(package_name)
     if package_name != normalized_package_name:
         return RedirectResponse(request.url_for('package', package=normalized_package_name))
 
     try:
-        version_to_files = await pypi.files_for_package(pypi_config, package_name)
+        version_to_files = await pypi.files_by_version(pypi_config, package_name)
     except pypi.PackageDoesNotExist:
         return PlainTextResponse(
             f'Package {package_name!r} does not exist on PyPI.',
             status_code=404,
         )
     else:
+        def _version_sort_key(version: str | None) -> packaging.version.Version:
+            if version is not None:
+                try:
+                    return packaging.version.parse(version)
+                except packaging.version.InvalidVersion:
+                    pass
+            # Not really correct, but just throw everything we can't parse at the bottom.
+            return packaging.version.Version('0.0.0')
+
         version_to_files_sorted = sorted(
             version_to_files.items(),
-            key=lambda item: packaging.version.parse(item[0]),
+            key=lambda item: _version_sort_key(item[0]),
             reverse=True,
         )
         return templates.TemplateResponse(
             'package.html',
             {
                 'request': request,
                 'package': package_name,
```

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/pypi.py` & `pypi_browser_webapp-0.0.9/pypi_browser/pypi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,113 @@
+import abc
 import base64
+import collections
 import contextlib
 import dataclasses
+import html.parser
 import itertools
 import os.path
 import typing
 import urllib.parse
 
 import aiofiles.os
 import httpx
 
+from pypi_browser import packaging
+
+
+class PythonRepository(abc.ABC):
+
+    @abc.abstractmethod
+    async def files_for_package(self, package_name: str) -> dict[str, str]:
+        """Return mapping from filename to file URL for files in a package."""
+
+
+class HTMLAnchorParser(html.parser.HTMLParser):
+    anchors: set[str]
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.anchors = set()
+
+    def handle_starttag(self, tag: str, attrs: list[tuple[str, str | None]]) -> None:
+        if tag == 'a':
+            if href := dict(attrs).get('href'):
+                self.anchors.add(href)
+
 
 @dataclasses.dataclass(frozen=True)
-class PyPIConfig:
-    cache_path: str
+class SimpleRepository(PythonRepository):
+    """Old-style "simple" PyPI registry serving HTML files."""
+    # TODO: Also handle PEP691 JSON simple repositories.
     pypi_url: str
 
+    async def files_for_package(self, package_name: str) -> dict[str, str]:
+        async with httpx.AsyncClient() as client:
+            resp = await client.get(
+                f'{self.pypi_url}/{package_name}',
+                follow_redirects=True,
+            )
+            if resp.status_code == 404:
+                raise PackageDoesNotExist(package_name)
+            parser = HTMLAnchorParser()
+            parser.feed(resp.text)
+
+            def clean_url(url: str) -> str:
+                parsed = urllib.parse.urlparse(urllib.parse.urljoin(str(resp.url), url))
+                return parsed._replace(fragment='').geturl()
+
+            return {
+                (urllib.parse.urlparse(url).path).split('/')[-1]: clean_url(url)
+                for url in parser.anchors
+            }
 
-class PackageDoesNotExist(Exception):
-    pass
 
+@dataclasses.dataclass(frozen=True)
+class LegacyJsonRepository(PythonRepository):
+    """Non-standardized JSON API compatible with pypi.org's /pypi/*/json endpoints."""
+    pypi_url: str
 
-async def package_metadata(
-    config: PyPIConfig,
-    client: httpx.AsyncClient,
-    package: str,
-) -> typing.Dict[typing.Any, typing.Any]:
-    resp = await client.get(f'{config.pypi_url}/pypi/{package}/json')
-    if resp.status_code == 404:
-        raise PackageDoesNotExist(package)
-    resp.raise_for_status()
-    return resp.json()
+    async def files_for_package(self, package_name: str) -> dict[str, str]:
+        async with httpx.AsyncClient() as client:
+            resp = await client.get(
+                f'{self.pypi_url}/pypi/{package_name}/json',
+                follow_redirects=True,
+            )
+            if resp.status_code == 404:
+                raise PackageDoesNotExist(package_name)
+            resp.raise_for_status()
+            return {
+                file_['filename']: urllib.parse.urljoin(str(resp.url), file_['url'])
+                for file_ in itertools.chain.from_iterable(resp.json()['releases'].values())
+            }
 
 
-async def files_for_package(config: PyPIConfig, package: str) -> typing.Dict[str, typing.Set[str]]:
-    async with httpx.AsyncClient() as client:
-        metadata = await package_metadata(config, client, package)
+@dataclasses.dataclass(frozen=True)
+class PyPIConfig:
+    repo: PythonRepository
+    cache_path: str
+
+
+class PackageDoesNotExist(Exception):
+    pass
 
-    return {
-        version: {file_['filename'] for file_ in files}
-        for version, files in metadata['releases'].items()
-        if len(files) > 0
-    }
+
+async def files_by_version(config: PyPIConfig, package: str) -> dict[str | None, set[str]]:
+    ret = collections.defaultdict(set)
+    for filename in await config.repo.files_for_package(package):
+        try:
+            version = packaging.guess_version_from_filename(filename)
+        except ValueError:
+            # Possible with some very poorly-formed packages that used to be
+            # allowed on PyPI. Just skip them when this happens.
+            pass
+        else:
+            ret[version].add(filename)
+    return ret
 
 
 class CannotFindFileError(Exception):
     pass
 
 
 def _storage_path(config: PyPIConfig, package: str, filename: str) -> str:
@@ -77,29 +140,23 @@
     May be instant if the file is already cached; otherwise it will download
     it and may take a while.
     """
     stored_path = _storage_path(config, package, filename)
     if await aiofiles.os.path.exists(stored_path):
         return stored_path
 
-    async with httpx.AsyncClient() as client:
-        metadata = await package_metadata(config, client, package)
+    filename_to_url = await config.repo.files_for_package(package)
+    try:
+        url = filename_to_url[filename]
+    except KeyError:
+        raise CannotFindFileError(package, filename)
 
-        # Parsing versions from non-wheel Python packages isn't perfectly
-        # reliable, so just search through all releases until we find a
-        # matching file.
-        for file_ in itertools.chain.from_iterable(metadata['releases'].values()):
-            if file_['filename'] == filename:
-                url = urllib.parse.urljoin(config.pypi_url, file_['url'])
-                break
-        else:
-            raise CannotFindFileError(package, filename)
-
-        await aiofiles.os.makedirs(os.path.dirname(stored_path), exist_ok=True)
+    await aiofiles.os.makedirs(os.path.dirname(stored_path), exist_ok=True)
 
+    async with httpx.AsyncClient() as client:
         async with _atomic_file(stored_path) as f:
             async with client.stream('GET', url) as resp:
                 resp.raise_for_status()
                 async for chunk in resp.aiter_bytes():
                     await f.write(chunk)
 
         return stored_path
```

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/static/bootstrap-5.2.1.min.css` & `pypi_browser_webapp-0.0.9/pypi_browser/static/bootstrap-5.2.1.min.css`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/static/bootstrap-5.2.1.min.js` & `pypi_browser_webapp-0.0.9/pypi_browser/static/bootstrap-5.2.1.min.js`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/static/favicon.png` & `pypi_browser_webapp-0.0.9/pypi_browser/static/favicon.png`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/templates/_base.html` & `pypi_browser_webapp-0.0.9/pypi_browser/templates/_base.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/templates/_macros.html` & `pypi_browser_webapp-0.0.9/pypi_browser/templates/_macros.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/templates/home.html` & `pypi_browser_webapp-0.0.9/pypi_browser/templates/home.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/templates/package.html` & `pypi_browser_webapp-0.0.9/pypi_browser/templates/package.html`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,23 @@
 
     <p>
     <tt>{{package}}</tt> has {{version_to_files|length}} version{{version_to_files|length|pluralize}} and {{total_files}} file{{total_files|pluralize}}.
         Select a file below to explore it.
     </p>
     {% for version, files in version_to_files %}
         <div class="card bg-light mb-3">
-            <div class="card-header"><h5 class="mb-0">{{version}}</h5></div>
+            <div class="card-header">
+                <h5 class="mb-0">
+                    {% if version is not none %}
+                        {{version}}
+                    {% else %}
+                        (unparseable version)
+                    {% endif %}
+                </h5>
+            </div>
             <div class="list-group list-group-flush">
                 {% for file in files|sort %}
                     <a class="list-group-item list-group-item-action" href="{{url_for('package_file', package=package, filename=file)}}">
                         <span class="font-monospace small">{{file}}</span>
                         {{macros.package_type_pill(file)}}
                     </a>
                 {% endfor %}
```

#### html2text {}

```diff
@@ -4,11 +4,12 @@
 ************ {{{{ppaacckkaaggee}}}} ************
    1. _B_r_o_w_s_e
    2. {{package}}
 {{package}} has {{version_to_files|length}} version{
 {version_to_files|length|pluralize}} and {{total_files}} file{
 {total_files|pluralize}}. Select a file below to explore it.
 {% for version, files in version_to_files %}
-**** {{{{vveerrssiioonn}}}} ****
+**** {{%% iiff vveerrssiioonn iiss nnoott nnoonnee %%}} {{{{vveerrssiioonn}}}} {{%% eellssee %%}} ((uunnppaarrsseeaabbllee vveerrssiioonn)) {{%%
+eennddiiff %%}} ****
 {% for file in files|sort %} _{_{_f_i_l_e_}_}_ _{_{_m_a_c_r_o_s_._p_a_c_k_a_g_e___t_y_p_e___p_i_l_l_(_f_i_l_e_)_}_}_ {%
 endfor %}
 {% endfor %} {% endblock %} {# vim: ft=jinja #}
```

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/templates/package_file.html` & `pypi_browser_webapp-0.0.9/pypi_browser/templates/package_file.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.8/pypi_browser/templates/package_file_archive_path.html` & `pypi_browser_webapp-0.0.9/pypi_browser/templates/package_file_archive_path.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.8/pyproject.toml` & `pypi_browser_webapp-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypi-browser-webapp"
-version = "0.0.8"
+version = "0.0.9"
 description = "PyPI package browsing web application"
 authors = ["Chris Kuehl <ckuehl@ckuehl.me>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "pypi_browser"}]
 
 [tool.poetry.dependencies]
```

